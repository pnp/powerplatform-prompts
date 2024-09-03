# Fundraiser Information

## Description

This prompt helps with providing information on fundraisers using an input variable and data from the Dataverse table, Fundraiser, in the sample Fundraiser Power Apps model-driven app.

## Prompt

Answer in English as bullet points in a professional tone. Provide details on {Fundraiser.Name} {Fundraiser.Category} {Fundraiser.Total Donations} {Fundraiser. Goal} and please mentioned the [user question] in the header of the response.

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Fundraiser information | [Elaiza Benitez](https://github.com/elaizabenitez.png), Microsoft

## Pre-requisite
* This prompt is dependant on the sample Fundraiser Power Apps model-driven app. Refer to [Get sample apps](https://aka.ms/sample-model-driven-apps) for steps in installing sample apps and data.

## Minimal Path to Awesome

* In your custom copilot in Copilot Studio, create a new Topic with a minimum of 5 trigger phrases. The following are examples.
```
Please tell me information about my fundraisers
Summarize donations received for my fundraisers
I want to know information about donations for my fundraisers in different categories
I need to know information on donations received for my fundraisers
What donations have I received for my fundraisers
```
* Add the Call an action node and select **Create a prompt**
* The AI Builder prompt builder will appear within Copilot Studio. Enter a name for your prompt such as `Fundraiser information prompt`
* Select **Input** under Settings to the right of the screen and select **Add input**
* In the **Name** field enter `user question` and in the **Sample data** field, enter `What are my top 3 fundraisers by total donations?`
* Select **Data used (preview)** and select **+ Add data**
* Search for the *Fundraiser* table and select it.
* Copy the prompt and paste into the **Prompt** field.
* Replace all data variables in the prompt with curly braces by selecting **+ Insert**, then select **Fundraiser** and search for the columns **Name**, **Category**, **Total Donations** and **Fundraiser Goal**.
* Replace [user question] with the input variable created earlier by selecting **+ Insert**, then select **user question**
* Select **Test prompt**
* Once tested, select **Save custom prompt**
* In Copilot Studio, search for the _Fundraiser information prompt_ action and select it. The prompt action will now be added to the Topic of your custom copilot.

For a step-by-step walkthrough, watch [Build prompt actions for your copilot](aka.ms/ai-in-action/copilot-studio/ep3)

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/ai-builder/fundraiser-information" aria-hidden="true" />
