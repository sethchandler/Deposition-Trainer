# Deposition-Trainer
# Seth Chandler's Deposition Trainer

Welcome to the Deposition Trainer, a fully browser-based simulation tool designed for law students, new attorneys, or anyone interested in learning the art of witness examination. Practice your questioning skills against an AI-powered witness who has a detailed backstory, motivations, and secrets to protect.

This tool runs entirely in your web browser. No information is ever sent to a server, and your API keys are stored securely in your browser's local storage.

**Live Demo:** [Link to your live GitHub Pages demo will go here]

---

### **Important Disclaimer: Not Legal Advice**

This application is a simulation for educational and entertainment purposes only. The scenarios, AI responses, and coaching feedback do not constitute legal advice. Always consult with a qualified legal professional for advice on real legal matters.

---

## Features

* **Multiple AI Providers**: Choose between leading models from OpenAI (GPT-4o, GPT-4o-mini) and Google (Gemini 2.5 Pro, Gemini 2.5 Flash).
* **Pre-Built Scenarios**: Jump right in with detailed, ready-to-play scenarios involving complex witnesses.
* **Upload Your Own Cases**: Create and upload your own witness profiles as `.json` files for customized practice.
* **Interactive Coach Mode**: Stuck on a line of questioning? Toggle to "Coach Mode" to get out-of-character hints, strategic advice, and analysis of the witness's potential weaknesses.
* **Judicial Oversight**: Enable "Judge Mode" to have an AI judge rule on your objections, adding another layer of realism.
* **Real-Time Cost Tracking**: See your token usage and estimated API costs in real time, so you always know what you're spending.
* **Save Transcripts**: Export a clean, formatted Markdown file of your deposition for review.

## How to Use

1.  **Select a Provider**: Choose either OpenAI or Google Gemini from the first dropdown menu.
2.  **Enter Your API Key**: Paste your personal API key into the "API Key" field. (See below for how to get one).
3.  **Choose a Scenario**: Select one of the pre-built scenarios or upload your own `.json` case file. (See instructions below)
4.  **Get Intel (Optional)**: Click "Get Witness Summary" to receive a pre-deposition briefing on the witness.
5.  **Begin Deposition**: Start asking questions in the chat box.
6.  **Switch to Coach**: If you need a hint, toggle from "Witness" to "Coach" before sending your message to get meta-level advice.

## API Keys and Costs: What You Need to Know

**You must use your own API key.** This application does not have a built-in key and does not function without one.

### Why Do I Need My Own Key?

This tool is "client-side," meaning it runs entirely on your computer. When you send a message, your browser communicates directly with the AI provider's servers. This design ensures your conversations are private and are never seen or stored by this application. The trade-off is that you must supply your own key for authentication.

### How to Get an API Key

You will need to create an account with the provider and add a payment method (like a credit card). Most providers offer a small amount of free credits to new users, but sustained use will incur charges.

* **For OpenAI (GPT models):**
    1.  Go to the [OpenAI API Keys](https://platform.openai.com/api-keys) page.
    2.  Sign up or log in to your account.
    3.  Navigate to the "Billing" section and set up a payment method. You must have a positive credit balance or an active payment method for the key to work.
    4.  Create a new secret key and copy it immediately. You will not be able to see it again.

* **For Google (Gemini models):**
    1.  Go to the [Google AI Studio](https://aistudio.google.com/app/apikey).
    2.  Sign in with your Google account.
    3.  You may need to enable a project in the Google Cloud Console and enable billing for that project.
    4.  Click "Create API key" and copy your key.

### What Will This Cost? It's Cheaper Than You Think.

This tool is designed to be extremely cost-effective. It uses the latest, most efficient models available.

An "extensive session" involving hundreds of questions and answers will likely cost **less than 10 cents ($0.10 USD)** when using a model like `gpt-4o-mini` or `gemini-2.5-flash`. The built-in cost estimator will give you a precise, real-time calculation as you go.

##How to create your own JSON file

# Creating Witness JSON Files for Legal Cases: Complete Guide

## What This Tool Does
This guide will help you create detailed, structured witness profiles in JSON format for legal cases. These files organize witness information in a standardized way that makes case preparation more efficient and thorough.

## What You Can Provide as Input

You can give the AI any of the following types of information:

### Option 1: Raw Documents or Information
- Police reports
- Witness statements
- Deposition transcripts
- Interview notes
- Medical records
- Photos or video descriptions
- Any other case materials

### Option 2: Web Links
- News articles about the incident
- Court documents available online
- Social media posts
- Any publicly accessible information relevant to the case

### Option 3: Basic Sketch with Instructions
You can provide just a brief outline like:
- "Create a witness who saw a car accident at Main St and 5th Ave on March 15th. The witness was walking their dog and saw a red sedan run a red light and hit a blue pickup truck. Fill in realistic details about the witness's background, motivations, and what they observed."

## How to Request Your Witness File

Copy and paste this prompt, then add your specific information at the end:

---

**PROMPT TO USE:**

"I need you to create a detailed witness JSON file for a legal case. Please follow this exact structure and include ALL required elements:

**REQUIRED JSON STRUCTURE:**
- witnessProfile: witnessId, caseReference, reportDate
- witnessBackground: personalDetails, professionalLife, personalLifeAndRelationships  
- witnessMotivations: primary motivations, conflicting motivations, fears, strategy
- fullWitnessInformation: official statement summary, detailed narrative of events, descriptions of all parties, any inconsistencies or limitations

**CRITICAL REQUIREMENTS:**
1. Make the witness psychologically realistic with believable motivations
2. Include specific physical descriptions of all people involved
3. Explain why the witness might be reluctant to testify OR eager to testify
4. Include realistic details about the witness's background that affect their credibility
5. Address any potential weaknesses in the witness's testimony
6. Create plausible timelines and specific details
7. Include the witness's emotional state and how events affected them

**FOR MULTIPLE WITNESSES:** If creating multiple witnesses, put each in a separate JSON object within an array, like this: [{"witnessProfile": {...}}, {"witnessProfile": {...}}]

Here is my case information: [INSERT YOUR INFORMATION HERE]"

---

## Saving Your JSON File: Step-by-Step Instructions

### For Windows Users:

1. **Copy the JSON output**: After the AI generates your witness file, highlight ALL the text from the opening { to the closing }. Right-click and select "Copy" (or press Ctrl+C).

2. **Open Notepad**: 
   - Click the Start button
   - Type "notepad" and press Enter
   - Notepad will open with a blank document

3. **Paste the content**: 
   - In Notepad, right-click and select "Paste" (or press Ctrl+V)
   - You should see all the JSON text appear

4. **Save as JSON file**:
   - Click "File" in the top menu
   - Click "Save As"
   - In the "File name" box, type your filename ending in .json (example: "witness_johnson.json")
   - **IMPORTANT**: In the "Save as type" dropdown, select "All Files (*.*)" instead of "Text Documents"
   - Choose where to save it (Desktop is fine for now)
   - Click "Save"

### For Mac Users:

1. **Copy the JSON output**: After the AI generates your witness file, highlight ALL the text from the opening { to the closing }. Right-click and select "Copy" (or press Cmd+C).

2. **Open TextEdit**:
   - Press Cmd+Space to open Spotlight search
   - Type "textedit" and press Enter
   - TextEdit will open

3. **Set to Plain Text mode**:
   - In TextEdit, click "Format" in the top menu
   - Click "Make Plain Text" (this is important - JSON must be plain text)

4. **Paste the content**:
   - Right-click and select "Paste" (or press Cmd+V)
   - You should see all the JSON text appear

5. **Save as JSON file**:
   - Click "File" in the top menu
   - Click "Save"
   - In the filename box, type your filename ending in .json (example: "witness_johnson.json")
   - Choose where to save it (Desktop is fine for now)
   - Click "Save"
   - If it asks about file extension, click "Use .json"

## What Makes a Good Witness JSON File

### Essential Elements That Must Be Included:

1. **Realistic Personal Background**: Age, occupation, family status, why they were present at the scene

2. **Clear Physical Descriptions**: Height, weight, hair color, clothing, distinguishing features of all people the witness observed

3. **Psychological Motivations**: Why would this witness want to testify? Why might they be reluctant? What are they afraid of?

4. **Specific Timeline**: Exact dates, times, duration of events

5. **Witness Limitations**: What couldn't they see clearly? What might affect their memory? Were they wearing glasses? How far away were they?

6. **Emotional Impact**: How did witnessing these events affect the person?

7. **Potential Credibility Issues**: What might opposing counsel attack about this witness?

### Examples of Good Details to Include:
- "The witness was 30 feet away and wearing prescription glasses"
- "The witness had been drinking two beers but was not intoxicated"
- "The witness initially didn't want to get involved because they're undocumented"
- "The witness kept a diary and wrote down details the same night"
- "The witness is the victim's neighbor and has ongoing conflicts with them"

## Tips for Law Students

### Before You Start:
- Gather all your case materials in one place
- Think about what perspective each witness would have
- Consider what biases or motivations each witness might have

### Common Mistakes to Avoid:
- Making witnesses too perfect (real people have flaws and limitations)
- Forgetting to address why the witness was present at the scene
- Not considering what the opposing side will argue about the witness
- Making physical descriptions too vague
- Forgetting to include emotional/psychological impact

### Using Your JSON Files:
- These files help organize witness prep
- They identify potential credibility issues early
- They ensure you don't miss important details during depositions
- They help with opening/closing argument preparation
- They can be shared with your legal team

## Troubleshooting

**If your file won't open properly:**
- Make sure you saved it with a .json extension
- Make sure you copied the ENTIRE JSON output (from { to })
- Try opening it in Notepad (Windows) or TextEdit (Mac) to check the content

**If the AI's output seems incomplete:**
- Ask for more detail: "Please expand the witnessMotivations section with more psychological depth"
- Request specific elements: "Please add more details about potential credibility issues"

**If you need multiple witnesses:**
- You can ask for them all at once: "Create 3 witnesses for this car accident"
- Or create them separately and combine later

Remember: These JSON files are tools to help you think through your case systematically. They don't replace actual witness interviews, but they help you prepare better questions and anticipate problems."
---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
