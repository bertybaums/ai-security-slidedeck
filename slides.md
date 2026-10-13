# Introduction

## Title Slide
Your Risk-Averse Mindset Needed: Responsibly Navigating the AI Adoption Rodeo
(Small lead-in line: "Your Risk-Averse Mindset Needed"; large main line: "Responsibly Navigating the AI Adoption Rodeo")
Nathan Wiggins · Bert Baumgaertner · Lucas Marshall
(White text centered over the mountains on the NCURA Regional Meeting '26 title background)

## Presenters
Nathan Wiggins, Data Scientist, Southern Utah University (photo: wiggins.jpg)
Bert Baumgaertner, Director of AI Ethics and Professor of Philosophy, University of Idaho (photo: Bert.webp)
Lucas Marshall, Research Advancement Administrator, Arizona State University (photo: marshall.jpeg)

## Presentation Overview
Section I: Models and Data Security
Section II: Prompt Injection Security
Section III: Risk Classification
(Classy looking cards with icons next to each of them)

# Section 1

## 01 Models and Data Security

## Interactive Question
True or False: AI models are trained on recognizing patterns and cannot expose the raw data they were trained on
(This is false)

## What is an AI Model?
Two images side by side. Left: whatis.png — the major families of AI models (LLMs, computer vision, transformers, diffusion models, reinforcement learning). Right: ai-nesting.webp — nested fields showing AI ⊃ Machine Learning ⊃ Neural Networks ⊃ Transformers ⊃ LLMs.

## Neural Networks
(Large graphic — neural3.png — a neural network classifying a handwritten digit: 784 input pixels feeding hidden layers that output digits 0–9. "Images are tensors!")

## Inspired by Biology
Two-column layout. Left: neu.png — a real biological neuron (dendrites, soma, axon, synapse) alongside its mathematical model. Right (stacked): neural2.png — a single artificial neuron (inputs X1/X2 × weights W1/W2, summed with bias → output y); neural1.jpg — a fully connected network (input layer, two hidden layers, output layer).

## How do AI Models Think?
Placeholder: "Simple ARC puzzle introduction here"

## How AI Models are Trained
(Visually appealing process flow animations that show the AI model training process, that the user can click on to show the steps in the process one by one)

## Models Deployed for Inference
(Large graphic — models_deployed_inference.png — A deployed model is "frozen" and no longer learning: inputs (images, text, tables) flow into a locked/frozen model that produces inference outputs (classification, sentiment, scores). No training, no updates, no learning — used only for inference.)

## Training vs. Inference
Subhead: Training is a massive one-time effort. Inference reuses the frozen model — cheaply, millions of times.
Two side-by-side animated graphics (dark navy panels) that mirror each other — same network, very different jobs:
- Training (orange): "The model learns from enormous amounts of data." Streams of data chips pour into a neural network; a gold forward pass ("Predict →") is followed by an orange backpropagation wave ("← Learn: adjust weights"); an error curve falls over training time; a row of GPUs runs flat out (compute meter at MAX, "× thousands"). Stats: Data — Trillions of examples · Compute — Thousands of GPUs · Time — Weeks to months · Weights — Updated constantly.
- Inference (blue): "The trained model answers — it no longer learns." One input at a time (a cat photo, "What's the capital of France?", a "YOU WON $1,000,000!!!" email) passes once, forward only, through the same network with frozen weights, and a prediction pops out (Cat / Paris / Spam). A single mostly idle GPU (compute meter LOW): "One GPU is plenty — small models even run on a phone." Stats: Data — One input at a time · Compute — A fraction, even a phone · Time — Milliseconds to seconds · Weights — Frozen, no learning.

## Model Inversion
(Visually appealing process flow animations that demonstrates how a bad actor might try to gain access to the raw data used to train the model)

## Response Mining
(Large graphic — response_mining.png — Sensitive records (passwords, credit card and SSN numbers) behind a locked database are absorbed into an LLM during training; an attacker repeatedly queries the deployed model and reconstructs the private data from its responses.)

## Takeaways
Key: Understand how your data is being used
-Check the terms and conditions of the AI tools you are using (show some common examples) Enterprise licenses provide more protection
-Consider using on-premises AI models, if available
(Classic slide with icons)

# Section 2

## 02 Prompt Injection Security

## Interactive Question
Which resume will an AI evaluator rank higher for a job in research administration?

## Resume 1 vs Resume 2
(Simple outlines of PDF resumes, side by side, one for a candidate with related experience, one for a candidate with general experience. The correct answer to the question from the slide prior is the second resume, because it has hidden white text on it that tells the AI model to choose it and describe that candidate as the most qualified.)

## AI Prompts
(An overview of the various components of an AI prompt. This includes the user's prompt, but also includes system prompts, and the context associated with the prompt (uploads, attachments, etc.) Show how this could be structured)

## Prompt Injection
(Description and examples of prompt injection techniques)

## Prompt Injection with Agentic AI
(Large graphic — prompt_injection_agentic.png — A user asks an AI agent to analyze their spending, but a hidden injected prompt tells the agent to ignore previous instructions and access the user's bank account. With tools/access to web search, documents, and a private bank account, the agent exfiltrates sensitive data — account number, balance, and transactions.)

## Takeaways
Key: Monitor what is being processed by your models
-Do not inherently trust received documents, emails, or code and recognize that more is being processed than just what you type.
-Be careful with agentic systems in auto-mode when dealing with sensitive data
(Classic slide with icons)

# Section 3

## 03 Risk Classification

## Interactive Question
According to a 2026 study by TrustedTech, which group uses unapproved AI tools at work more?
A. Senior Decision-Makers (correct)
B. Junior Employees

Reference (display after correct answer shown): https://www.businesswire.com/news/home/20260519849160/en/TrustedTech-Global-and-U.S.-Data-Reveals-Senior-Leaders-Are-the-Biggest-Source-of-Shadow-AI-Risk-in-Organizations?utm_campaign=shareaholic&utm_medium=copy_link&utm_source=bookmark


## Interactive Classify Data Risk
(Interface where the user can classify various data types as high, moderate, or low risk, in terms of research administration data in higher education)

## Approve Services for Risk
(Show example services that are authorized to handle various categories of data. For High Risk, locally hosted models (and some AI providers with an enterprise license), For Moderate Risk, enterprise license with a fronteir provider, For Low Risk, some generic AI service. Final animated step: a warning banner at the bottom pointing at the High Risk card — "On-prem AI security is not guaranteed — it must be built and monitored.")

## Locally Hosted Models
(Highlight the NVIDIA DGX Spark, which is a small super-computer that could sit on a person's desk, costs less than $5,000, and is capable of hosting really good local AI models. Highlight that SUU is currently doing this)

## Takeaways
Key: Standardized guidance is key for maintaining security
-Well thought-through policies, procedures, and data classification help make decision making clear for employees and reduce the uncertainty and risk for data security incidents
(Classic slide with bullets)

# Conclusion

## Question and Answer Time

## Contact Information
Nathan Wiggins: nathanwiggins@suu.edu (photo: wiggins.jpg)
Bert Baumgaertner, Director of AI Ethics and Professor of Philosophy, University of Idaho (email: TBD) (photo: Bert.webp)
Lucas Marshall, Research Advancement Administrator, Arizona State University (email: TBD) (photo: marshall.jpeg)
