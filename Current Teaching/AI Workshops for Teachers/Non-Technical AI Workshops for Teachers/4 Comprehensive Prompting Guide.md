---
title: "4 Comprehensive Prompting Guide"
description: "Effective Strategies for Working with Large Language Models"
---

# Effective Strategies for Working with Large Language Models

## Introduction

Large Language Models (LLMs) are not search engines. They generate responses through pattern matching and statistical prediction rather than retrieving existing information. Understanding this fundamental difference is crucial for effective prompting. This guide synthesizes research-based best practices with practical teaching experience to help you craft prompts that work with how LLMs actually function.

**Key principle:** Getting good responses often means adding explanatory context and preference information to your instruction or query. One-line prompts rarely produce optimal results because they lack the information the model needs to understand your specific needs.

---

## The Four-Component Framework

Effective prompts typically include four key components. While not every prompt requires all four, consciously considering each element improves results significantly.

### 1. Goal: What You Want Accomplished

The goal states what you would like the tool to do, create, find, accomplish, address, or answer. Be specific about the desired outcome.

**Important consideration:** If you ask for something specific that requires very specific contextual information but don’t include that information, you’ll either get unsuitable responses or, worse, responses that sound appropriate but contain fabrications or errors you might not notice.

*Example goals:*

- “Generate a lesson plan for teaching fractions to adult learners”

- “Create a professional summary for a LinkedIn profile”

- “Draft a cover letter connecting my experience to this role”

- “Summarize the main arguments from these sources and identify common themes”

### 2. Format: How the Response Should Be Structured

Format specifies the shape, structure, or form the response should take. This includes length, organization, and structural elements.

*Format considerations:*

- Should it be bullet points, paragraphs, or a numbered list?

- How long should it be? (word count, paragraph count, page length)

- Should sources be included? If so, in what citation style?

- Do you have an example format you could include?

- What sections or components should be included?

*Example format specifications:*

- “Write this as three paragraphs: introduction, body, conclusion”

- “Provide a bullet point list with 5-7 items, each 1-2 sentences long”

- “Structure this as a formal business letter with proper salutation and closing”

### 3. Tone: The Voice and Emotional Quality

Tone describes how the response should sound or feel. This encompasses formality, emotional character, and the relationship you’re establishing with the reader.

*Tone dimensions:*

- **Formality:** Professional, academic, conversational, casual

- **Emotional character:** Upbeat, serious, humorous, empathetic, matter-of-fact

- **Complexity:** Technical jargon vs. plain language

- **Energy:** Enthusiastic, measured, understated

*Example tone specifications:*

- “Professional but approachable, avoiding corporate jargon”

- “Friendly and encouraging, suitable for adult learners”

- “Academic but accessible, explaining technical concepts clearly”

### 4. Context: Information Needed to Complete the Task

Context provides the necessary information, background, and circumstances that enable effective completion of the task. This is often the most important component for preventing hallucinations and irrelevant responses.

*What to include in context:*

- Who is the audience? (12-year-olds, business executives, adult learners)

- What is the purpose? (For a job application, for teaching, for internal communication)

- Where will this be used? (LinkedIn profile, company memo, academic paper)

- What background information is needed? (Your experience, the job description, relevant data)

- What constraints exist? (Company policies, assignment requirements, word limits)

**Critical safety note:** Never include personal information like addresses, phone numbers, bank details, or other sensitive data in prompts. Remove these from any documents you upload.

---

## Practical Examples

### Example 1: Cover Letter

**Weak prompt:** “Write me a cover letter.”

**Strong prompt:**

Goal: I need a draft cover letter for a customer service position. Context: I have 3 years of retail experience and 2 years in hospitality. The job posting emphasizes conflict resolution and team collaboration. The company is a mid-sized tech startup with a casual but professional culture. Format: Three paragraphs: (1) introduction connecting my experience to the role, (2) main body describing specific relevant experiences, (3) conclusion expressing enthusiasm for the position. Approximately 300-350 words total. Tone: Professional but friendly and approachable, not overly formal. Avoid corporate jargon. I want to sound confident but not arrogant.

### Example 2: Educational Content

**Weak prompt:** “Explain fractions.”

**Strong prompt:**

Goal: Create a one-page explanation of how to add fractions with different denominators. Context: My students are adult learners (ages 25-45) returning to education. Many have math anxiety. They need this for a workplace training program. Use everyday examples like measuring ingredients or splitting bills. Format: Start with a simple explanation, then provide 3 worked examples of increasing complexity, then 3 practice problems. Keep sentences short (under 20 words). Tone: Encouraging and patient. Avoid academic language. Make it feel achievable, not intimidating.

---

## Official Prompting Guides

Each LLM provider offers official documentation. These guides reflect how each specific model has been designed and trained. Always consult official sources rather than user-generated guides.

### Claude (Anthropic)

Official prompting guide: [https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)

Key emphasis: Clear instructions, examples, and chain-of-thought prompting. Anthropic’s guides are particularly strong on using XML tags for structure and providing detailed examples.

### ChatGPT (OpenAI)

Official prompting guide: [https://platform.openai.com/docs/guides/prompt-engineering](https://platform.openai.com/docs/guides/prompt-engineering)

Key emphasis: Write clear instructions, provide reference text, split complex tasks into simpler subtasks, and give the model time to think. OpenAI emphasizes iterative refinement.

### Gemini (Google)

Official prompting guide: [https://ai.google.dev/gemini-api/docs/prompting-intro](https://ai.google.dev/gemini-api/docs/prompting-intro)

Key emphasis: Be specific and clear, break down complex requests, and use examples. Google’s documentation particularly focuses on multimodal prompting (text + images).

### DeepSeek

Official documentation: [https://api-docs.deepseek.com/](https://api-docs.deepseek.com/)

Key emphasis: DeepSeek’s documentation focuses more on technical API usage. Their prompting guidance emphasizes clear, structured inputs and leveraging their model’s strong reasoning capabilities.

---

## Common Themes Across Official Guides

Despite differences in presentation, official guides share several core recommendations:

1. **Be specific:** Vague prompts produce vague results

1. **Provide examples:** Show the model what you want rather than just describing it

1. **Break down complex tasks:** Multiple simple prompts often work better than one complex prompt

1. **Give context:** Don’t assume the model knows your situation or needs

1. **Iterate:** First attempts rarely produce perfect results—refine based on output

1. **Specify format:** Tell the model how to structure its response

---

## What’s Discouraged

Official guides consistently warn against:

- **One-line prompts without context:** “Write a report” tells the model almost nothing about what you actually need

- **Assuming the model has information it doesn’t:** It can’t access your files, know your preferences, or read your mind

- **Treating it like a search engine:** LLMs generate, they don’t retrieve. Different tools need different approaches

- **Contradictory instructions:** “Be brief but comprehensive” confuses the model

- **Expecting perfection on first try:** Plan to iterate and refine

---

## Critical Evaluation and Verification

Even with perfect prompts, LLM outputs require critical evaluation. Remember:

- LLMs can generate false information with complete confidence

- Citations may be fabricated—verify every source

- Factual accuracy requires your verification, not the model’s

- Tone and appropriateness need human judgment

- You remain responsible for what you submit or publish

**For more on critical evaluation:** See the Understanding AI Tool Limitations handout for specific strategies on developing appropriate skepticism while using these tools effectively.

---

## Iterative Refinement

Professional use of LLMs typically involves iteration:

1. **Start with a structured prompt** using the four-component framework

1. **Review the output critically** for accuracy, tone, and appropriateness

1. **Refine your prompt** based on what worked and what didn’t

1. **Request specific changes** rather than starting over

1. **Verify factual claims** and edit for your voice and needs

Example refinement sequence:

Initial: “This is too formal for my purposes.” Refinement: “Please revise this with a more conversational tone, as if explaining to a colleague rather than writing a formal report.” Initial: “This is too long.” Refinement: “Please condense this to approximately 200 words, keeping only the most essential points about X, Y, and Z.”

---

## Additional Resources

**Course materials:**

- Understanding How LLMs Work (foundational concepts)

- Understanding AI Tool Limitations (critical evaluation)

- Educational Prompting Examples (detailed examples)

**Learning approach:**

The best way to improve your prompting is through deliberate practice. Try the four-component framework with real tasks you need to accomplish. Notice what works and what doesn’t. Compare outputs across different models. Save your effective prompts for future reference. Treat prompting as a skill that develops through use, not a formula to memorize.
