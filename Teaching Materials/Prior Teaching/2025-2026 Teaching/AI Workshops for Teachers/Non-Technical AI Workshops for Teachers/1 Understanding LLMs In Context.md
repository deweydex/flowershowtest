---
title: "1 Understanding LLMs In Context"
description: "A 30-Minute Exploration for Educators"
---

## Section 1: What Is a Large Language Model? (10 minutes)

A Large Language Model (LLM) is a type of artificial intelligence trained on vast amounts of text to predict what words come next in a sequence. Think of it less as a *knowing entity* and more as a sophisticated *pattern completion system*. When you provide a prompt, the model generates text by continuously predicting the most statistically likely next token (word or word-piece) based on patterns learned during training.

### Key Concepts

**Training:** LLMs learn from enormous text datasets (books, websites, articles) by identifying statistical relationships between words, phrases, and concepts. They do not “understand” in the human sense; they recognize and reproduce patterns.

**Parameters:** The billions of numerical values that encode these patterns. More parameters generally means more nuanced pattern recognition, but not necessarily more accurate knowledge.

**Tokens:** The basic units LLMs process. A token might be a whole word, part of a word, or punctuation. The model predicts tokens one at a time, building responses sequentially.

### A Hermeneutic of Suspicion

Understanding how LLMs work should make us appropriately skeptical of their outputs. Because they operate through statistical pattern matching rather than understanding, several consequences follow:

- **Fluency does not equal accuracy:** LLMs generate grammatically correct, coherent-sounding text even when the content is false

- **Confidence is not reliability:** The model has no mechanism to assess its own certainty or indicate when it lacks information

- **Patterns reflect training data:** Outputs reproduce whatever patterns exist in the training corpus, including biases, errors, and outdated information

- **Reasoning is simulated:** What appears to be logical thinking is pattern matching that mimics reasoning structures from training data

### Reflection Question

*If an LLM generates text by predicting what is statistically likely to come next, what implications might this have for the accuracy or originality of its outputs? How might we teach students to evaluate AI-generated text critically?*

---

## Section 2: LLMs vs. Search Engines (10 minutes)

Understanding the difference between LLMs and search engines is crucial for developing appropriate critical evaluation strategies. The distinction shapes what kinds of errors we should expect and what verification methods make sense.

### Search Engines

Search engines like Google index existing web content and return links to sources. They *retrieve* information that already exists somewhere. When you search, you get pointers to documents written by identifiable authors. The search engine does not create content; it finds and ranks existing content. This means errors typically come from poor source selection rather than fabrication.

### Large Language Models

LLMs *generate* new text based on patterns. They do not retrieve specific documents or cite sources (unless specifically designed to do so). The text they produce is a statistical synthesis, not a quotation from an existing source. This fundamental difference in operation creates different risk profiles:

- Generated text may not correspond to any real source

- “Hallucinations” occur when the model generates plausible-sounding but false information

- There is no built-in mechanism for verifying factual accuracy

- Citations, when provided, may be fabricated with the same confidence as real ones

### Why This Matters for Evaluation

With search engines, critical evaluation focuses on source credibility: Who published this? What’s their expertise? What biases might they have? With LLMs, we need different questions: Could this information be verified? Does this claim require sources that the model couldn’t access? Are there precision claims (specific quotes, exact statistics, detailed citations) that warrant extra skepticism?

### Reflection Question

*How might students’ prior experiences with search engines create false confidence in LLM outputs? What specific strategies could help them develop appropriate skepticism?*

---

## Section 3: Retrieval-Augmented Generation (RAG) (10 minutes)

To address some limitations of pure LLMs, many commercial systems now use Retrieval-Augmented Generation (RAG). This architecture combines the generative capabilities of LLMs with actual information retrieval. Understanding RAG helps us calibrate our suspicion—it solves some problems but creates new ones.

### How RAG Works

When you query a RAG system, it first searches a database of documents (which might include web pages, PDFs, or proprietary content) to find relevant information. It then provides this retrieved content to the LLM as context, and the LLM generates a response based on both its training and the retrieved documents.

### What RAG Improves

RAG systems can cite sources, provide more current information, and ground responses in actual documents. When working well, they give users something to verify against. This is a meaningful improvement over pure generation, where verification may be impossible.

### What RAG Does Not Solve

The LLM still synthesizes and paraphrases the retrieved content. It may:

- Misinterpret sources

- Combine information inappropriately across multiple documents

- Present retrieved information with unwarranted confidence

- Retrieve low-quality or biased sources

- Fail to retrieve the most relevant documents

Additionally, users often cannot tell whether a response comes from RAG retrieval or pure generation. Different tools use different architectures, and these change frequently without notice.

### Maintaining Critical Distance

Even with citations, verification remains the user’s responsibility. RAG makes verification *possible* in more cases, but does not make it automatic. We should teach students to treat citations from AI systems as leads to investigate, not as proof of accuracy.

### Reflection Question

*Given that RAG systems combine retrieval and generation, how might we help students develop appropriate critical evaluation skills for AI-generated content that includes citations? What would those verification practices look like in practice?*
