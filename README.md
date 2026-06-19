# PromptDeck AI

I built this initially to be a place to store prompt templates for marketing, analysis, and learning. Over time, it slowly turned into a workspace where prompts can be built, improved, analyzed, compared, and run directly with AI. 

To put it simply, PromptDeck is for drafting clearer and more specific prompts that provide better results from AI tools. Opposed to the manual task of prompting, where lack of detail, context, and structure can lead to vague or inconsistent responses, this tool speeds that whole process up. 

## How to use the site

Start by going to the Builder page. Write what you want the AI to do, choose a persona or response tone if helpful, add any context or constraints, then click Generate. You can copy the finished prompt into an AI tool, or use the Run with AI section to test it directly inside the site.

If you do not want to start from scratch, go to Templates, pick a prompt card, and it will load into the Builder. From there you can edit it, generate the final prompt, and use it however you want.

# Pages

### Builder

The Builder is where you create prompts from scratch. You can choose a persona and a response tone, then type in your task, context, output format, and select extra enhancements.

Upon generating your prompt, you can use the Run with AI section for testing prompts directly. This is optional and is usable with a an API key or local model.

For cloud AI, choose the cloud option, pick a provider, paste your API key, and run the prompt.

For local AI, download the this `index.html` file make sure Ollama (or other) is running on your computer. Open Command Prompt and go to the file path where this `index.html` is saved. Start a local server by typing `python -m http.server 8765`. Then open `http://127.0.0.1:8765/index.html` in your browser. Once the site is open locally, go to Builder, scroll to Run with AI, choose Local AI, click Check Local AI, pick a model, generate a prompt, and click Run Prompt.

### Library

The Library stores prompts you save while using the site. It is useful for keeping prompts you want to reuse or improve on later.

### Analyzer

The Analyzer reviews a prompt and gives feedback on its quality, clarity, context, constraints, formatting, and overall usefulness. It is meant to help improve prompts before using them.

The way it works is by scoring the prompt across several prompt quality dimensions instead of just checking for random keywords. It looks for whether the prompt has a clear persona or role, if the task is specific and action oriented, if there is enough context about the audience or situation, if the desired output format is clear, if the prompt includes useful constraints or guardrails, and if it uses stronger prompting techniques like examples, structured sections, step by step reasoning, clarification requests, or XML style organization. Each area gets its own score, then the Analyzer combines those scores into one overall quality score. After that, it gives feedback based on the weakest areas first, so the suggestions are focused on what would most improve the prompt rather than giving generic advice. 

### Workflow

The Workflow page creates step by step AI workflows. You give it a goal, choose a workflow type, and it creates a structured process with prompts for each step. Instead of giving you one prompt, it breaks the work into a sequence of smaller prompts that are easier to run and review. Essentially a structured plan with each step labeled, explained, and paired with a prompt.

You would ideally use it when a task is too big for one prompt. For example, instead of asking a model to build a full strategy in one shot, the Workflow page can help you first define the problem, gather information, analyze options, create recommendations, and then turn everything into a final deliverable.

### Templates

The Templates page includes 400+ prompt templates across categories like marketing, branding, analysis, coding, AI building, learning, cybersecurity, and more. Clicking a card sends it to the Builder to which you refine content and generate the prompt.

### Compare
The Compare page allows the comparison of different prompts side by side before you use them. Just paste two prompt versions and see which one is likely to perform better based on clarity, context, structure, constraints, output format, and overall usefulness.

Useful when you are deciding between two ways of asking for the same thing. For example, you might compare an original prompt against an improved version from the Builder or Analyzer. The point is to make prompt selection less random. 
