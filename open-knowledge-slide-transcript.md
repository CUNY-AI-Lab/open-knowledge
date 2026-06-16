# AI & Open Educational Resources - Slide Deck Transcript

Audience: Open Knowledge Fellowship participants.

Scope: spoken transcript keyed to the current 35-slide deck in `index.html`.

Source basis: current local `index.html` and visible slide content. This follows the actual slide order after the chatbot slide was removed.

## Slide 1 - AI & Open Educational Resources

Welcome to the CUNY AI Lab session on AI and Open Educational Resources. Today we are looking at how these systems work, what they make easier, what they put at risk, and how to decide where AI belongs in OER work.

## Slide 2 - Whether You Use AI Is Your Call

We start with Langdon Winner's question: what kind of world are we building as we use AI? Winner asks us to look at technologies as forms of life, not just tools. AI is already part of teaching and learning, including for students, and the Graduate Center's draft guidance leaves decisions about AI use to you. Before using it in teaching or OER work, ask what AI changes in your classroom and in the knowledge commons in which you participate.

## Slide 3 - AI Basics

Part one covers the basics. We will start with what large language models do, how training works, and why the training data matters for open educational resources.

## Slide 4 - Large Language Models Predict Tokens

A large language model, or LLM, generates an answer through inference. Inference builds the output one token at a time. A token can be a word, part of a word, a number, or punctuation. The model reads the context, predicts the next token, adds it to the output, and repeats.

## Slide 5 - How Large Language Models Are Trained

Training repeats one task at huge scale. The model guesses a hidden next token, checks the guess, and shifts its weights. Later tuning uses examples and human rankings.

## Slide 6 - Unpacking The Pile

Many commercial AI companies hide or obfuscate their training data. The Pile is useful because EleutherAI documented the dataset openly. It is an 825 GiB English corpus built from 22 sources, including Wikipedia, Project Gutenberg, Stack Exchange, GitHub, arXiv, PubMed Central, FreeLaw, and Books3. Books3 is the contested part. It contains about 196,000 books copied from Bibliotik, a private book-piracy site.

## Slide 7 - What It Can Do Now

Part two moves from training to use. Once the model has been trained, the practical question is what current systems can do, what they still get wrong, and what changes when tools are added.

## Slide 8 - Rewarded for Guessing

Kalai and coauthors argue that hallucinations persist because training and evaluation reward guessing over acknowledging uncertainty. Pretraining learns patterns. For rare facts, the model often relies on nearby patterns, so a wrong answer can sound fluent. Benchmarks also reward test-taking. Accuracy scoreboards give credit for a lucky guess and no credit for uncertainty.

## Slide 9 - Grounding the Answer

Prompt a frontier model for today's weather. A grounded system searches a live source before answering. Tools let the model use information outside its training data. A system can search the web or a catalog, read a file you provide, or run code and read the result.

## Slide 10 - Working in a Loop

Agentic systems revise each tool call from the last result. Test-time computing gives the loop more passes. OpenClaw and Hermes agents run the loop by checking results and choosing another step. In tool calling, a search can return weak hits and trigger a better query. Code can return an error and trigger a patch. OCR can produce bad text and trigger tighter instructions.

## Slide 11 - Problematics

Part three turns to the worries. The point is not to treat every worry as equal, or to dismiss them all. The goal is to identify which worries matter for OER and which responses have force.

## Slide 12 - What Happens to "Open"

Open licensing lets people reuse work if they credit the source and give back to the commons. Model builders can train on the work while dropping the credit and returning nothing. That creates a pressure on the open bargain: if people expect open work to be scraped without return, some people stop sharing and the commons shrinks.

## Slide 13 - Chatbots Take the Audience

When a chatbot answers the question, people stop clicking through to the source. On a volunteer-run commons, readers are also the people who maintain the resource. Referral traffic to open sites has fallen hard, and Wikipedia is seeing human visits slide while bot traffic climbs.

## Slide 14 - Academic Publishers Are Selling Scholarly Writing to AI Companies

Some academic publishers have made AI licensing deals for scholarly writing without asking authors or paying them. Taylor & Francis took 10 million dollars from Microsoft, and Wiley took 44 million dollars. The Authors Guild says authors were not asked or paid. The writing sold in these deals is the closed, paywalled kind that authors sign over to publishers.

## Slide 15 - A License Alone Will Not Stop Model Training

In 2025, courts ruled that training can be fair use even on copyrighted work. Anthropic paid 1.5 billion dollars for pirating books, not for training on them. Restrictive licenses mostly affect ordinary reusers. Collective responses, like Creative Commons preference signals or Wikimedia charging scrapers for access, have more force.

## Slide 16 - When Open Knowledge Becomes Weights

Wiley's 5Rs ask whether people can keep, revise, remix, reuse, and share a resource. When model builders turn that material into weights, the checks change. Can people download and run the weights? Can people inspect the training data and code, or are they kept behind closed doors? Does the license permit reuse, or does it stay semi-permissive or restrictive? Does the model require costly hardware by design?

## Slide 17 - Public AI

A closed model is owned and run by one company, and that company decides who can use it and how. Public AI points in a different direction: open models that can be run outside a single company and governed in public. The CUNY AI Lab runs on models like these as a public service and stores none of your data.

## Slide 18 - The CUNY AI Lab

The CUNY AI Lab is a faculty- and staff-led group at the Graduate Center. The lab builds and runs AI infrastructure for teaching and research across CUNY. It is public and non-commercial, runs on open models, and does not train on your data.

## Slide 19 - Your OER Work

Part four turns to your OER work. The question now is where AI can help with open materials while keeping a person responsible for the result.

## Slide 20 - Where It Helps with OER Work

For OER, a few uses are worth considering when a person owns the result. AI can draft alt text and captions that people then check. It can turn scanned pages and old PDFs into editable, publishable text. It can help produce rough drafts and translations that a subject expert revises into shape.

## Slide 21 - Judging Appropriate Use

A few questions matter in every case. Is a person accountable for the result? Is AI assistance disclosed? Has the output been checked against a reliable source? Is the model grounded in sources you trust?

## Slide 22 - From Idea to Artifact

For OER, subject experts can now build the resource they imagine without writing every line themselves. That matters for digitizing archives, making interactive resources, and lowering the barrier for people who have disciplinary expertise but no coding background.

## Slide 23 - Manifold Companion

Manifold Companion is a document-processing platform for CUNY's Manifold instance. It turns scanned pages and PDFs into publication-ready texts. AI handles the first pass, including OCR and structure, while humans review the text and export it for publication.

## Slide 24 - Lalli, Il Venditore di Sogni

This project digitizes the manuscripts of Italian-American writer Franco Lalli, then publishes them as an open, searchable archive. The pipeline combines OCR and translation, and visitors can browse the original text beside the translation with scholarly metadata.

## Slide 25 - Italian American Open Syllabus

The Italian American Open Syllabus is a curated, peer-reviewed collection of open essays and reading lists on Italian-American literature and culture. AI helped with a specific production task: converting Word contributions into clean parsed HTML and attaching a stylesheet. The editing and scholarship remained human work.

## Slide 26 - Impariamo l'Italiano

Impariamo l'Italiano is a set of interactive Italian-learning games, including Wordle, memory, a verb-tense wheel, and crosswords. The site is free and requires no login. Bea built the site with AI assistance despite having no coding background, and Stefano later made a multilingual version called LanGames.

## Slide 27 - Cloze Reader

Cloze Reader is a small OER reading-practice tool built by one of today's presenters. It turns passages into fill-in-the-blank exercises that support close reading and vocabulary practice.

## Slide 28 - ThinkWith

ThinkWith was built by first-year writing instructor Nicole Walker after CUNY AI Lab workshops. A student pastes in a source passage, a cultural artifact, and a paragraph connecting the two. The model gives feedback on the connection. The tool sends students back to revise rather than writing the paragraph for them. The limit is that the judge is still a model, so the teacher still has to judge the result.

## Slide 29 - Informed Refusal and Informed Adoption

Adopting AI and refusing AI are both legitimate choices. The point is to have reasons. Use AI where it helps, with someone accountable for the result, and say why. Decline AI where it does not fit, and say why. The Graduate Center guidance leaves room for that.

## Slide 30 - Discussion Question 1

Where in your teaching would a grounded, course-specific assistant help, and where would it get in the way?

## Slide 31 - Discussion Question 2

What would informed refusal look like in your field? What would you want to tell a student about it?

## Slide 32 - Discussion Question 3

If you released an OER, how would you want AI to be allowed to use it, or not?

## Slide 33 - Discussion Question 4

What is one resource you have wanted to build but could not? Could anything here lower that barrier?

## Slide 34 - Discussion Question 5

Which of today's worries still feels unresolved to you?

## Slide 35 - References

The reference slide lists the sources behind the talk, including Kalai et al. on hallucinations, Stanford HAI's AI Index, the Open Source Initiative, OLMo, David Wiley on the 5 R's, UNESCO on open education, the Authors Guild and The Bookseller on publisher licensing deals, Open Future and Internet Policy Review on public AI and the commons, Langdon Winner on technology and politics, Creative Commons on AI training and signals, Open Future and Verhulst on openness, and Wikimedia on crawler load and paid API access.
