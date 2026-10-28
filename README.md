# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies

## Algorithm

## 1. INTRODUCTION

AI-powered text summarization is the process of using Artificial Intelligence to shorten a long document while keeping its important information. Prompting techniques help AI understand what type of summary the user needs.

In this experiment, four prompting techniques are applied to different AI platforms to identify which combination produces the best summary for undergraduate students.

## 2. PROMPTING TECHNIQUES WITH EXAMPLES

### Zero-Shot Prompting

Definition: Zero-shot prompting means asking an AI to perform a task without giving any examples.

Example prompt:

Summarize the article “The Basics of Blockchain Technology” in 100 words. Use simple English and include the meaning of blockchain, how it works, its advantages, and its applications.

Expected output:

Blockchain is a digital system used to store information securely. Data is stored in blocks connected in a chain. Each block contains transaction details and a unique cryptographic hash. Blockchain is decentralized, meaning that information is shared across multiple computers. It provides transparency, security, and traceability. Blockchain is used in cryptocurrency, healthcare, banking, and supply chain management. However, some blockchain systems consume high amounts of energy and may process transactions slowly.

Result: Zero-shot prompting is simple and fast, but the summary may miss some important details.

### Few-Shot Prompting

Definition: Few-shot prompting means giving the AI one or more examples of the expected output before asking it to perform the task.

Example prompt:

Example input: Artificial Intelligence enables computers to perform tasks that normally require human intelligence.

Example summary: AI helps computers perform intelligent tasks.

Now summarize “The Basics of Blockchain Technology” in the same style. Use simple sentences and include only the main ideas.

Expected output:

Blockchain is a technology that stores data in connected blocks. It allows multiple computers to share and verify information. Cryptographic methods help protect the data. Blockchain is used in digital payments, healthcare, and supply chains. Its major benefits are transparency and security, although scalability and energy consumption can be challenges.

Result: Few-shot prompting helps maintain a consistent style and makes summaries more suitable for students.

###  Chain-of-Thought Prompting

Definition: Chain-of-thought prompting encourages the AI to approach a task through a structured sequence of steps. For this experiment, the AI can be asked to analyze the article's main ideas and then produce a summary without displaying private internal reasoning.

Example prompt:

Analyze the article “The Basics of Blockchain Technology.” Identify its main topic, important concepts, advantages, limitations, and applications. Then use these points to write a clear 100-word summary for undergraduate students. Check that the summary does not contain unsupported information.

Expected output:

Blockchain is a digital ledger that records transactions in connected blocks. Each block is linked to the previous block using cryptographic methods. Copies of the ledger may be maintained across a network of computers, helping participants verify transactions. Blockchain can improve transparency, data integrity, and traceability. It is used in cryptocurrency, banking, healthcare, and supply chain management. However, some systems face challenges such as high energy consumption, limited transaction speed, and scalability. Blockchain is useful when multiple parties need to share and verify records securely.

Result: Structured prompting can improve completeness and organization, especially for technical articles.

### Role-Based Prompting

Definition: Role-based prompting instructs the AI to act as a specific expert or professional to produce an appropriate response.

Example prompt:

Act as an experienced computer science professor. Summarize the article “The Basics of Blockchain Technology” for undergraduate students in 100 words. Explain technical terms in simple English and include the working principle, advantages, limitations, and real-world applications.

Expected output:

Blockchain is a technology that stores digital information in blocks linked together in a chain. Each block contains records and a cryptographic hash that helps detect changes. Instead of depending on a single central authority, many blockchain networks allow multiple computers to maintain and verify records. This makes blockchain useful for secure transactions and transparent record-keeping. Its applications include cryptocurrency, banking, healthcare, and product tracking. However, blockchain may have problems with transaction speed, scalability, and energy use. Understanding these benefits and limitations helps students identify where blockchain technology can be used effectively.

Result: Role-based prompting helps the AI adapt its language, tone, and level of explanation to the target audience.

## 3.AI PLATFORMS USED

[File:ChatGPT-Logo.svg - Wikimedia Commons](https://images.openai.com/static-rsc-4/iIwQvt6lHcQFgj7BguLsxseHBBrUFkMcXG5YNkmFFW4lfJVJx4j903Vj6U7eh4G1RxYAM5rcotiwXgmy1bpDjVeUGauxGKEaWacWqJ6UawIltioycNX9Ru1jiDHQJ6b718nA6kh8GV93DvtXMfEhj4O5IYd7IWQ4fxKOZEoQ6CY?purpose=inline)

ChatGPT

ChatGPT generates summaries, explains technical concepts, and follows detailed instructions.

Example: “Summarize blockchain in 100 words using simple English for engineering students.”

[Gemini – Google’s AI Assistant for Smart Conversations & Productivity – Daidu.ai](https://images.openai.com/static-rsc-4/ptJvxAnbpHSz9oKwhiZCWU9MTvmPl997rGrZd4wqTgvg18xJPt8X3ASwCANnmkTN4cvnMJqTW5csYg-Wx_SyU_pL6waVf_YLfxdwlsLklzd2H22udrktQ6oVGaeLOvjKRl8y4lJCZGtYV2I-4GwcwBjAGawfKX-wZYbv6TzRORU?purpose=inline)

Google Gemini

Gemini can summarize text, identify key ideas, and organize information into readable formats.

Example: “Extract the main ideas from the blockchain article and present them as a short summary.”

[Claude](https://images.openai.com/static-rsc-4/cLHBfiXuOV35_PSb5wC1jXivsAXbOR_8j6QIuMUVJNmHhvqDTZSAjip3DZXEZE8rrigO3zrBPXPTm3OPFqtXG1oYbfxtfR2epfKwRiaR-r0auw26KWwnnPiRgtOfu6qqeScD6KjrINNkb8STcXPBIHcixXdk1xpiKuwC8UdBT_8?purpose=inline)

Claude

Claude can work with lengthy text and produce well-organized summaries when given suitable input.

Example: “Summarize the blockchain article, preserving its key concepts, advantages, and limitations.”

[Workshop Presencial Copilot en Acción - Versión 2 | FORTION SAS Medellín](https://images.openai.com/static-rsc-4/ZqytWYCDj6KJnvCqQ6lRtawhEw5OCgC1y1UkVntc9lo8Hg8ouN-Jj_rZ3YVMuC-gZIex_GaOpZ9hg3s0fHWlpwKt1lqvOEYamzjx7_k_2D1HBsve0bIRevJOprPzsobcpv-MX6IGgiWUwKqQRlwCCVvKGH977h0ImP34TRNYV-c?purpose=inline)

Microsoft Copilot

Copilot can help summarize technical information and present important points in a concise format.

Example: “Create a student-friendly summary of blockchain technology with its uses and challenges.”

## 4. EVALUATION CRITERIA WITH EXAMPLES

| Criterion       | Meaning                                    | Example                                                                 |
| --------------- | ------------------------------------------ | ----------------------------------------------------------------------- |
| Accuracy        | Correctness of information                 | Correctly explaining that blocks are linked using cryptographic hashes. |
| Coherence       | Logical flow of ideas                      | Explaining blockchain definition before its working and applications.   |
| Simplicity      | Ease of understanding                      | Using “digital record book” to explain a ledger.                        |
| Speed           | Time taken to generate the summary         | Recording the time from submitting the prompt to receiving the result.  |
| User experience | Ease of using and understanding the result | A clear, well-formatted summary that students can read easily.          |

## 5. COMPARISON OF PROMPTING TECHNIQUES

The following table shows an illustrative comparison of the expected strengths of each technique. These are qualitative expectations, not measured experimental results.

| Prompting technique | Accuracy            | Coherence | Simplicity | Speed     |
| ------------------- | ------------------- | --------- | ---------- | --------- |
| Zero-Shot           | Good                | Good      | Good       | Very fast |
| Few-Shot            | Good                | Very good | Very good  | Fast      |
| Chain-of-Thought    | Very good potential | Very good | Good       | Moderate  |
| Role-Based          | Good to very good   | Very good | Very good  | Fast      |

Example: Zero-shot prompting may produce a quick summary, while role-based prompting may provide a more student-friendly explanation because it specifies the intended audience.

## 6. CROSS-PLATFORM COMPARISON

Each AI platform should be tested with the same article, word limit, and prompting instructions to make the comparison fair.

| AI platform | Main feature to evaluate      | Example evaluation                                           |
| ----------- | ----------------------------- | ------------------------------------------------------------ |
| ChatGPT     | Instruction following         | Does it include all required concepts within 100 words?      |
| Gemini      | Key-point extraction          | Does it identify the main ideas without unnecessary details? |
| Claude      | Organization and completeness | Does it preserve the article's important explanations?       |
| Copilot     | Conciseness and readability   | Is the summary clear and easy to read?                       |

Actual performance depends on the model version, prompt, and input article. No platform can be declared the winner without testing the outputs.

## 7. PROCEDURE

1. Select a technical article of approximately 500 words on “The Basics of Blockchain Technology.”
2. Open ChatGPT, Gemini, Claude, and Copilot.
3. Enter the same article into each platform.
4. Apply Zero-Shot, Few-Shot, Chain-of-Thought, and Role-Based Prompting separately.
5. Save each generated summary.
6. Evaluate every summary using accuracy, coherence, simplicity, speed, and user experience.
7. Compare the results and identify the best-performing combination.

## 8. SAMPLE EVALUATION TABLE

Use the following table to record your results after testing. The scores below are examples only and should be replaced with your actual observations.

Scoring: 1 = Poor, 2 = Fair, 3 = Good, 4 = Very Good, 5 = Excellent.

| Platform and technique | Accuracy | Coherence | Simplicity | Speed | User experience |
| ---------------------- | -------- | --------- | ---------- | ----- | --------------- |
| ChatGPT – Zero-Shot    | 4        | 4         | 4          | 5     | 4               |
| ChatGPT – Few-Shot     | 4        | 5         | 5          | 4     | 5               |
| Gemini – Role-Based    | 4        | 4         | 5          | 4     | 4               |
| Claude – Few-Shot      | 5        | 5         | 4          | 4     | 5               |
| Copilot – Zero-Shot    | 4        | 4         | 4          | 5     | 4               |

Example interpretation: If Claude's few-shot summary receives high accuracy and coherence scores during actual testing, it may be a suitable choice for producing complete and well-organized educational summaries. This conclusion must be verified using the same test conditions for all platforms.



## Result


