# Generative AI Applications: Research Report

*Information current as of 7 November 2026.*

This report reviews ten established applications of generative AI. Each section covers the business value, technical challenges and weak points of the use case, then lists existing implementations.

Figures published by vendors are marked as vendor-reported, because they have rarely been independently audited. Sources for the figures are linked where they appear.

## Contents

1. [Software development](#1-software-development)
2. [Customer support](#2-customer-support)
3. [Marketing and content creation](#3-marketing-and-content-creation)
4. [Image, video and audio production](#4-image-video-and-audio-production)
5. [Clinical documentation](#5-clinical-documentation)
6. [Drug discovery](#6-drug-discovery)
7. [Legal research and drafting](#7-legal-research-and-drafting)
8. [Financial services](#8-financial-services)
9. [Enterprise knowledge search](#9-enterprise-knowledge-search)
10. [Education and tutoring](#10-education-and-tutoring)

## 1. Software development

**Business value:** Coding assistants and agents write, explain, test and refactor code, which can shorten delivery time and reduce repetitive work. In a [controlled experiment](https://arxiv.org/abs/2302.06590), developers using GitHub Copilot finished a small, well-defined task 55.8% faster than a control group.

**Technical challenges and weak points:** Gains on real codebases are harder to measure. [METR's early-2025 trial](https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/) found that experienced open-source developers took 19% longer with AI tools. Its [2026 follow-up](https://metr.org/blog/2026-02-24-uplift-update/) suggests that developers are probably faster now, but METR calls that data unreliable because many developers refused to work without AI, which skewed the sample. Security is the other main weakness: Veracode found that AI-generated code [introduced risky security flaws in 45% of tests](https://www.veracode.com/resources/analyst-reports/2025-genai-code-security-report/). Output still depends on human review, and large codebases are difficult to fit into a model's context.

**Existing implementations:**

- **[GitHub Copilot](https://github.com/features/copilot):** An AI pair programmer and coding agent built into editors and GitHub.
- **[Claude Code](https://claude.com/product/claude-code):** Anthropic's coding agent, which reads, edits and runs code from the terminal and other developer tools.
- **[Cursor](https://cursor.com):** An AI-first code editor with codebase-aware chat and agents.
- **[OpenAI Codex](https://chatgpt.com/codex/):** OpenAI's software engineering agent, which carries out coding tasks and proposes changes.

## 2. Customer support

**Business value:** AI agents answer routine requests around the clock across chat, email and voice, which lowers the cost per contact and shortens wait times. The market is now large enough to attract major acquisitions: in June 2026 [Salesforce agreed to buy Fin, formerly Intercom, for about $3.6 billion](https://investor.salesforce.com/news/news-details/2026/Salesforce-Signs-Definitive-Agreement-to-Acquire-Fin/), with closing expected in its fiscal fourth quarter. The same release says Fin's agents resolve 76% of support volume on average, which is a vendor-reported figure given without a methodology.

**Technical challenges and weak points:** Useful agents need accurate knowledge bases, secure connections to systems such as billing and order management, and clear rules for handing over to people. Resolution rates are also hard to compare, because each vendor defines "resolved" differently. Cost savings can hide a drop in quality. Klarna, an early and prominent adopter, [resumed hiring human agents in 2025](https://www.entrepreneur.com/business-news/klarna-ceo-reverses-course-by-hiring-more-humans-not-ai/491396) after its CEO said that an excessive focus on cost had [led to lower quality](https://www.techspot.com/news/107881-klarna-hiring-humans-again-ai-replacements-fail-deliver.html).

**Existing implementations:**

- **[Fin](https://fin.ai):** A customer service AI agent working across chat, email, phone and messaging channels.
- **[Sierra](https://sierra.ai):** A platform for building branded customer-facing AI agents.
- **[Salesforce Agentforce](https://www.salesforce.com/agentforce/):** A platform for building AI agents that work with Salesforce data and workflows.
- **[Zendesk AI agents](https://www.zendesk.com/service/ai/):** AI agents and agent-assist tools built into the Zendesk service platform.

## 3. Marketing and content creation

**Business value:** Generative tools speed up the production of ad copy, emails, product descriptions and campaign visuals. They also make it cheaper to adapt content for different audiences, languages and channels, so small teams can test more ideas without a matching rise in agency or production costs.

**Technical challenges and weak points:** Content must match the brand's voice, stay factually accurate and meet advertising rules, which usually requires brand guidance, approved source material and human approval. The main weak point is sameness: when competitors use the same tools, content becomes generic and harder to tell apart. Publishing more also doesn't prove business impact, so teams need to track conversions and revenue rather than output volume. Unchecked claims and unclear ownership of generated assets add legal risk.

**Existing implementations:**

- **[Jasper](https://www.jasper.ai):** An AI content platform for marketing teams, with brand voice controls.
- **[Canva Magic Studio](https://www.canva.com/magic/):** Generative design and writing tools built into Canva.
- **[Adobe Firefly](https://www.adobe.com/products/firefly.html):** Adobe's generative image and video tools for creative work.
- **[HubSpot AI](https://www.hubspot.com/products/artificial-intelligence):** AI features for content, campaigns and customer data within HubSpot's marketing platform.

## 4. Image, video and audio production

**Business value:** Text-to-image, video and voice models reduce the cost of concept art, storyboards, training videos, voice-overs and dubbing. Companies can produce localized material in many languages without new shoots or recording sessions, and creative teams can explore more options early in a project.

**Technical challenges and weak points:** Video models are expensive to run, and keeping characters and scenes consistent across shots remains difficult. Copyright is the largest open risk: [Disney and Universal sued Midjourney](https://www.yahoo.com/news/disney-universal-sue-ai-firm-053621337.html) in 2025, and Midjourney argues that AI training is fair use. Realistic synthetic media also enables deepfakes and voice fraud, so consent and content labeling matter. The market is unstable too: [OpenAI announced in March 2026 that it would discontinue Sora](https://macrumors.com/2026/03/24/openai-discontinuing-sora-ai-video-app/), which shows the risk of building production workflows on a single tool.

**Existing implementations:**

- **[Runway](https://runway.com):** Generative video models and editing tools for creative professionals.
- **[Google Veo](https://deepmind.google/models/veo/):** Google DeepMind's video generation model family.
- **[Midjourney](https://www.midjourney.com):** A generative service known for stylized, high-quality images.
- **[ElevenLabs](https://elevenlabs.io):** AI voice generation, dubbing and voice agent tools.
- **[Synthesia](https://www.synthesia.io):** A platform for creating presenter-led videos with AI avatars, widely used for corporate training.

## 5. Clinical documentation

**Business value:** Ambient AI scribes listen to patient visits and draft clinical notes, which aims to reduce paperwork and clinician burnout. The measured benefit so far is real but modest. A [multi-site JAMA study](https://www.news-medical.net/news/20260401/AI-scribes-modestly-reduce-clinician-documentation-time-and-EHR-use.aspx) of five US hospitals over more than two years linked AI scribes to about 16 fewer minutes of documentation per day, a 10% reduction.

**Technical challenges and weak points:** These systems must handle medical vocabulary, accents and overlapping speech, then fit into electronic health record workflows. Errors carry clinical risk because an omitted or invented detail can end up in a patient's permanent record, so clinicians must check every note. That review can absorb part of the time saved. Providers also need patient consent, strong protection of health data and compliance with rules such as HIPAA in the US.

**Existing implementations:**

- **[Abridge](https://www.abridge.com):** An ambient AI platform that turns patient conversations into clinical notes.
- **[Microsoft Dragon Copilot](https://www.microsoft.com/en-us/health-solutions/clinical-workflow/dragon-copilot):** A clinical assistant that combines ambient note-taking and dictation with information retrieval.
- **[Ambience Healthcare](https://www.ambiencehealthcare.com):** An ambient AI platform for documentation, coding and related clinical workflows.
- **[Nabla](https://www.nabla.com):** An ambient AI assistant that helps clinicians generate notes.

## 6. Drug discovery

**Business value:** Generative models can propose new molecules and predict protein structures and interactions, which could reduce the time and cost of early research. The clearest milestone is Insilico Medicine's rentosertib, a candidate for idiopathic pulmonary fibrosis. It reported [positive Phase IIa results](https://www.nature.com/articles/s41591-025-03743-2) and [dosed its first Phase III patient in September 2026](https://insilico.com/news/isn1009261-insilico-medicine-doses-first-patient-genesis-ipf-3). Insilico describes this as the first Phase III trial of a generative AI-driven drug.

**Technical challenges and weak points:** Models depend on limited, often proprietary biological data, and a molecule that looks promising in a model may still be impossible to synthesize, unsafe or ineffective. AI can speed up discovery, but it doesn't remove the need for long clinical trials: Insilico expects another three to four years from the start of Phase III to approval under favorable conditions. No drug discovered with generative AI has yet been shown to succeed through approval, and timelines can slip. For example, Isomorphic Labs moved its target for first clinical trials [from the end of 2025 to the end of 2026](https://www.investing.com/news/stock-market-news/googlebacked-ai-drug-discovery-startup-isomorphic-labs-delays-clinical-trial-timeline-4456134).

**Existing implementations:**

- **[Insilico Medicine](https://insilico.com):** A clinical-stage biotech that uses generative AI for target discovery and molecule design.
- **[Isomorphic Labs](https://www.isomorphiclabs.com):** An Alphabet company applying AI models to drug design.
- **[AlphaFold Server](https://alphafoldserver.com):** A free research tool, powered by AlphaFold 3, that predicts the structure of biomolecules.
- **[NVIDIA BioNeMo](https://docs.nvidia.com/bionemo-framework/latest/):** A framework for building and training AI models for biology and chemistry.

## 7. Legal research and drafting

**Business value:** Legal AI tools search case law, summarize documents, review contracts and prepare first drafts. This can cut the hours spent on routine work and speed up due diligence, while freeing lawyers for judgment-heavy tasks.

**Technical challenges and weak points:** Fabricated or inaccurate citations are the critical weakness, and connecting a model to legal databases reduces this risk without removing it. A [Stanford study](https://hai.stanford.edu/news/ai-trial-legal-models-hallucinate-1-out-6-or-more-benchmarking-queries) of specialized tools found that Lexis+ AI and Ask Practical Law AI gave incorrect information more than 17% of the time, and Westlaw AI-Assisted Research more than 34% of the time. Those 2024 results may not reflect current versions. Mistakes also have professional consequences: [Damien Charlotin's database](https://www.damiencharlotin.com/hallucinations/) lists 2,266 legal cases involving AI-generated hallucinations. Law firms must also protect client confidentiality and verify all output.

**Existing implementations:**

- **[Harvey](https://www.harvey.ai):** An AI platform for law firms and in-house legal teams.
- **[CoCounsel Legal](https://legal.thomsonreuters.com/en/products/cocounsel-legal):** Thomson Reuters' AI assistant for legal research, drafting and document review.
- **[Lexis+ with Protégé](https://www.lexisnexis.com/en-us/products/lexis-plus-protege.page):** LexisNexis's legal research platform with an AI assistant.

## 8. Financial services

**Business value:** Banks and investment firms use generative AI to summarize research, analyze filings and contracts, draft reports and help staff find internal information. These tools can make analysts and advisers more productive across very large organizations. JPMorganChase's internal LLM Suite portal was [used by 200,000 people by May 2025](https://www.americanbanker.com/news/how-jpmorganchase-democratized-employee-access-to-gen-ai).

**Technical challenges and weak points:** Financial firms operate under strict rules on privacy, record-keeping, model risk and client advice, so outputs must be accurate, explainable and traceable to their sources. A small numerical error can have serious consequences, and models can state a wrong figure confidently. Connecting tools securely to internal data is often the hardest step, as JPMorganChase has noted. Broad usage also doesn't prove financial return. In MIT's widely reported, [methodologically debated](https://www.zirous.com/insights/a-clearer-view-of-mits-genai-data-what-95-of-genai-projects-fail-really-means/) ["GenAI Divide" research](https://fortune.com/2025/08/18/mit-report-95-percent-generative-ai-pilots-at-companies-failing-cfo/), most company pilots across industries showed no measurable effect on profit and loss.

**Existing implementations:**

- **[JPMorganChase LLM Suite](https://www.americanbanker.com/news/how-jpmorganchase-democratized-employee-access-to-gen-ai):** An internal portal that gives employees access to external large language models (no public product page, so the link goes to press coverage).
- **[Morgan Stanley AI tools](https://www.morganstanley.com/press-releases/key-milestone-in-innovation-journey-with-openai):** OpenAI-based internal tools for the firm's financial advisers.
- **[AlphaSense](https://www.alpha-sense.com):** A market intelligence platform with AI search and summaries across financial content.
- **[Hebbia](https://www.hebbia.com):** An AI platform that analyzes large document sets for investors and other financial professionals.

## 9. Enterprise knowledge search

**Business value:** Employees can ask questions in plain language and get answers drawn from documents, email, chat and business systems. This saves time spent searching, helps new hires get up to speed and keeps knowledge from being lost in separate tools. Most of these products use retrieval-augmented generation (RAG), which retrieves relevant company content and passes it to a language model.

**Technical challenges and weak points:** Answers are only as good as the underlying content, and many companies have outdated, duplicated or conflicting documents. Access control is a key challenge because the system must respect each user's permissions, otherwise it can expose confidential information that was poorly secured but previously hard to find. Connecting to many data sources takes ongoing effort, and retrieved documents can carry prompt injection attacks. The value is also difficult to prove, because small time savings spread across many employees rarely show up clearly in financial results.

**Existing implementations:**

- **[Glean](https://www.glean.com):** A work AI platform that searches across company applications while respecting permissions.
- **[Microsoft 365 Copilot](https://www.microsoft.com/en-us/microsoft-365/copilot):** An assistant that works across Microsoft 365 apps and company data.
- **[Gemini Enterprise](https://cloud.google.com/gemini-enterprise):** Google Cloud's platform for company-wide AI agents and search.
- **[NotebookLM](https://notebooklm.google):** A Google research assistant that answers questions using the sources a user provides.

## 10. Education and tutoring

**Business value:** AI tutors can offer personalized help at any time and at far lower cost than human tutoring. Teachers can also use them to prepare lessons, generate practice material and give faster feedback. This could widen access to individual support for students who can't afford private tutoring.

**Technical challenges and weak points:** The biggest weakness is that a tool can improve short-term performance without building lasting skills, especially if it gives students the answer. Evidence is mixed so far. A [randomized trial of 2,379 undergraduates](https://www.iza.org/publications/dp/18989/the-effects-of-course-integrated-ai-tutoring-student-performance-and-engagement-a-randomized-university-trial) at a US public university found that access to a GPT-4o-based tutor lowered final grades by 0.37 standard deviations and reduced course participation. By contrast, [a study at a Chilean university](https://docs.iza.org/dp18513.pdf) that paired a course-specific assistant with guidance on its use reported better final-exam results. The two studies aren't directly comparable, but together they suggest that design and guidance matter. Other challenges include accuracy, age-appropriate safety, protection of student data and academic integrity.

**Existing implementations:**

- **[Khanmigo](https://www.khanmigo.ai):** Khan Academy's AI tutor and teaching assistant.
- **[Duolingo Max](https://blog.duolingo.com/duolingo-max/):** A Duolingo subscription tier with AI-powered language practice features.
- **[Claude for Education](https://claude.com/solutions/education):** Anthropic's offering for universities, designed to support student learning and academic work.

## Conclusion

Across these use cases, generative AI works best when it assists people on well-defined tasks and has access to reliable data. The recurring weak points are inaccurate output, security and privacy risks, unclear legal questions, and the difficulty of proving a financial return. Results also vary widely between organizations, so vendor figures are best treated as a starting point and tested through a controlled pilot.
