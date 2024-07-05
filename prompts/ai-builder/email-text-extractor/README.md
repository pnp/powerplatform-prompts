# Email Text Extractor

## Description

This prompt helps extracting text from emails. 

Take a look at the following link to learn more on how to use this prompt:
* [[Power Automate Cookbook] How to extract text from emails using AI Builder GPT capability](https://powerusers.microsoft.com/t5/Power-Automate-Cookbook/How-to-extract-text-from-emails-using-AI-Builder-GPT-capability/td-p/2199362)

  <a href="http://www.youtube.com/watch?feature=player_embedded&v=UchRykL7me8" target="_blank">
  <img src="http://img.youtube.com/vi/UchRykL7me8/mqdefault.jpg" alt="Watch the video" width="240" height="180" />
  </a>

## Prompt

Extract the 'orderNumber', 'deliveryNumber' and find the 'status' of the following email.
The status can be 'Done' or 'N/A' or 'Undone'.
Use CSV format for your answer.
Add headers 'Order Number', 'Delivery Number' and 'Status'.
Add a line break at the end of your CSV lines. 
If the text below has less than couple of words or looks like a placeholder text, respond "Sorry, I can't extract information", otherwise respond with the extracted information.
 
[text]

### Supported Language(s)

[English](./en-us/prompt.md)

## Prerequisites

* Your environment in the US
* A Power Apps or Power Automate license.
* Dataverse database installed on the environment.
* An AI Builder add-on

## Authors

Solution|Author(s)
--------|---------
Email Text Extractor | [Philippe Larrue](https://github.com/Phil-cmd) ([LinkedIn](https://www.linkedin.com/in/philippe-larrue-2946942/)), Microsoft

## Minimal Path to Awesome

* Copy the prompt
* Paste prompt into the tool of your choice (AIBuilder Azure Open AI, Power Apps Copilot, etc)

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/ai-builder/email-text-extractor" aria-hidden="true" />
