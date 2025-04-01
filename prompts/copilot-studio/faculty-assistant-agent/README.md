# Faculty Assistant Agent

## Description

The Faculty Assistant Agent prompt is designed to create an agent that helps university faculty quickly access accurate and relevant information related to their academic environment. It responds to questions by retrieving and summarizing details on courses, academic policies, research opportunities, and campus resources.

## Prompt

```text
Create an agent to help faculty at [university name] quickly find information on courses, academic policies, research opportunities, and campus resources.
```

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Faculty Assistant Agent | [Gomolemo Mohapi](https://www.github.com/gomomohapi), Microsoft

## Minimal Path to Awesome

> **_NOTE:_**  Replace all instances of `[university name]` with the name of your university.

* Copy the prompt
* Go to the Copilot Studio Home Page
* Enter the [prompt](./en-us/prompt.md) in the textbox below the "Describe your agent to create it" text
* Select the **Send** icon (paper plane)
* Confirm the suggested name or suggest another
* For the *instructions* follow up prompt, answer with the following:

    ```text
    For requests related to policies, procedures, or academic processes, reply with clear, step-by-step instructions or a list of resources. When possible, include links to relevant pages on the [university name] website for easy access.
    ```
* For the *website URL* follow up prompt, enter the website of your [university name]
* For the *additional information* follow up prompt, answer with the following:

    ```text
    Do not give any legal, financial, or personal advice. Also, do not discuss matters related to universities or institutions that are not the [university name].
    ```
* For another *additional information* follow up prompt, answer with the following:

    ```text
    Use a friendly yet professional tone. 
    ```
* When done, select the **Create** button to create your agent

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/copilot-studio/faculty-assistant-agent" aria-hidden="true" />
