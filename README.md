# Building Your Own AI Assistant - Web Automation with Gemini

🖥️ A hands-on demo from my **DevFest London** talk: ***Building Your Own AI Assistant - Web Automation with Gemini***.  
This project demonstrates how to combine Gemini with browser automation to create a personal AI assistant that can perform real web tasks such as searching, extracting data, and summarizing content.

---

## Prerequisites

- Windows, macOS, or Linux laptop  
- [Google AI Studio](https://aistudio.google.com/) for a Gemini API key  

---

## Installation Guide for Windows  

**Note:** This is a modified version of the official documentation, which you can find here 👉️ [Documentation](https://github.com/browser-use/web-ui/blob/main/README.md)  

### Make sure you have Git and Python 3.11

- If you don’t have Git installed, download it from the [official website](https://git-scm.com/downloads).  
- If you don’t have Python 3.11, download it from the Microsoft Store or the [official Python website](https://www.python.org/downloads/).  

Once both are installed, search for **Git CMD** in your applications.  
It should look like the Command Prompt but with colors.  

### Step 1: Clone the repository
`git clone https://github.com/browser-use/web-ui.git`
`cd web-ui`

### Step 2: Set up the Python environment
`python -m venv .venv`

Activate the virtual environment:
`.venv\Scripts\activate`

### Step 3: Install dependencies
`pip install -r requirements.txt`

Install the browser in Playwright:
`playwright install --with-deps`

### Step 4: Configure environment
**Note:** If you only want to try it out, you can skip this step and add your API key directly in the website.

Create a copy of the example environment file:
`copy .env.example .env`

Open `.env` in your preferred text editor and add your API keys and other settings.

### Step 5: Run the Web UI
**run the web-ui:**
`python webui.py --ip 127.0.0.1 --port 7788`

**Access the WebUI:** Open your web browser and navigate to http://127.0.0.1:7788

Check the official documentation if you want to use your own browser or configure additional options.

---

## Installation Guide for macOS/Linux

- Most Linux distributions and macOS already have Git and Python pre-installed, so you can open your terminal and run the following steps:

### Step 1: Clone the repository
`git clone https://github.com/browser-use/web-ui.git`
`cd web-ui`

### Step 2: Set up the Python environment
`python -m venv .venv`

Activate the virtual environment:
`source .venv/bin/activate`

### Step 3: Install Dependencies
`pip install -r requirements.txt`

**Install Browser in playwright:**
`playwright install --with-deps`

### Step 4: Configure Environment
**Note:** If you only want to try it out, you can skip this step and add your API key directly in the website.

Create a copy of the example environment file:
`copy .env.example .env`

open `.env` in your preferred text editor and add your API keys and other settings

### Step 5: Enjoy the web-ui
**run the web-ui:**
`python webui.py --ip 127.0.0.1 --port 7788`

**Access the WebUI:** Open your web browser and navigate to http://127.0.0.1:7788

Check out official documentation if you want to use your own browser or configue something else.

---

Once you can access the web interface, try a few examples on your own.

---

## General Examples

**1. current stock price and latest quaterly earnings**
Find the current stock price and a summary of the latest quarterly earnings report for Apple, Tesla, and Microsoft. Put the data in a bulleted list.

**2. write a summary**
find out today's tech news and summarize it in 300 words.


## Examples for AI assisntant

**1. Add items to my grocery list**
Go to ubereats.com and add 2% milk and table salt to my cart from walmart.

**2. Job hunting assistant**
You are a job-hunt assistant.  
1. Go to https://www.linkedin.com/jobs/  
2. Find the first “Top job picks for you” listing.  
3. Open its job description.  
4. Extract the “Responsibilities” section (or equivalent).  
5. Summarize those responsibilities in a few sentences.  
6. Compose an email message to me that includes:
   - A short subject line  
   - A greeting  
   - The summary of the responsibilities  
   - The link to the job posting  
   - A polite closing  

Send me only the email text (subject + body) on abcd@gmail.com

## Advance Examples

Check out demo section of orginal repo: https://github.com/browser-use/browser-use?tab=readme-ov-file#demos
