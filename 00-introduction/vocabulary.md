# GenAI Vocabulary

Terms from my research report, [Generative AI Applications](generative-ai-applications-report.md), explained in my own words.

## Generative AI

**Definition:** Generative AI is a technology used to generate new content. Each model is trained on its own type of data.

**Example from the report:** Pictures in Midjourney, video in Veo, voice in ElevenLabs (section 4).

## LLM

**Definition:** LLM is a large language model that uses text as input and output. It is a type of Generative AI.

**Example from the report:** JPMorganChase's internal LLM Suite portal gives staff access to LLMs that help them summarize research and draft reports (section 8).

## RAG

**Definition:** RAG (retrieval-augmented generation) is a technique used around an LLM, which only has the limited information it was trained on. RAG retrieves important context from an outside source, such as company documents, and puts it into the prompt so it can lead the generation.

**Example from the report:** Most enterprise knowledge search products use RAG to answer questions from company content (section 9).

## Hallucination

**Definition:** Hallucinations happen when a model gives a confident answer that is false or invented, because it follows statistical links and does not check facts.

**Example from the report:** Linking legal databases to a model reduces the risk of fabricated citations, but does not remove it (section 7).

## AI agent

**Definition:** AI agent is a technology that plans its own steps and uses tools to reach a goal. It can also coordinate other, smaller agents.

**Example from the report:** Claude Code reads, edits and runs code (section 1).

## Context window

**Definition:** Context window (measured in tokens) is the amount of information a model can see at one time. It includes the prompt, chat history, files and the response itself.

**Example from the report:** Large codebases are difficult to fit into a model's context (section 1).

## Knowledge base

**Definition:** Knowledge base is information prepared by people that a model or an agent can look up. It can include company documentation, files and other artifacts.

**Example from the report:** Support agents need accurate knowledge bases (section 2), and outdated or conflicting documents weaken enterprise search answers (section 9).

## Access control

**Definition:** Access control means that a user can find a piece of information only if they have permission to see it.

**Example from the report:** Enterprise search must respect each user's permissions, otherwise it can expose confidential information that was poorly secured (section 9).

## Human-in-the-loop

**Definition:** Human-in-the-loop means that a person checks AI output before it is used, to avoid harmful mistakes.

**Example from the report:** Clinicians must check every AI-written note (section 5), and law firms must verify all output (section 7).

## Synthetic media

**Definition:** Synthetic media is image, video or audio created by AI that can look or sound real. It makes labeling necessary, so people understand that some material is not real but created by AI.

**Example from the report:** Realistic synthetic media enables deepfakes and voice fraud, so consent and content labeling matter (section 4).

## Ambient AI scribe

**Definition:** Ambient AI scribe is AI that works in the background, listening to the doctor-patient dialog and making draft notes. The doctor still has to check the notes, which takes time.

**Example from the report:** A multi-site study linked AI scribes to about 16 fewer minutes of documentation per day, a 10% reduction (section 5).

## Pilot

**Definition:** Pilot is a small trial in a company that gives proof of concept: it shows whether AI really makes people more productive or not.

**Example from the report:** Most company pilots in MIT's "GenAI Divide" research showed no measurable effect on profit and loss (section 8).

## Prompt injection

**Definition:** Prompt injection is an attack in which someone hides instructions inside content that a model reads, such as a document or an email. The model cannot always tell who the instructions came from, so it may leak confidential data.

**Example from the report:** Documents retrieved by enterprise search can carry prompt injection attacks (section 9).

## Model risk

**Definition:** Model risk is the risk of misusing information when people make decisions based on a response from a model.

**Example from the report:** Models can state a wrong figure confidently, so analysts could use it in a report, and a company could lose money or break rules because of that number (section 8).

## Fair use

**Definition:** Fair use is a rule in US copyright law that allows, in some cases, using other people's work without permission. It matters for GenAI because models are trained on existing works, and it is still unclear whether that is allowed.

**Example from the report:** Disney and Universal sued Midjourney, and Midjourney argues that AI training is fair use (section 4).
