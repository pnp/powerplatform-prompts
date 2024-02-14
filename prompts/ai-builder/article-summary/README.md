# Article summary

## Description

This prompt helps with summarizing long articles in a few points, which significantly speed up process of understanding what is inside. It can be used for own purposes, results can be shared with other users or be part of app summarizing available articles (knowledge) in company.

Prompt has two parameters:
- input_text - text which you want to summarize.
- number_of_bullet_points - declaration in how many bullet points text should be summarize.

> TIP: If you want more precise summary, split your text into several parts and run this prompt one by one, on smaller portion of text and merge results after you process everything.

Anatomy of the prompt:
- clear objective: summary,
- specific subject: article,
- specific length: number of bullet points,
- specific format: bullet points.

All taken together give specific instruction.

Recommended implementation approach:
1) Sign in to [Power Apps](https://make.powerapps.com/) or [Power Automate](https://make.powerautomate.com/).
2) On the left pane, select <b>AI Prompt</b>.
3) In hero section select <b>Create text with GPT using a prompt</b>.
4) In new pop-up window press <b>Create custom prompt</b> button in down right corner.
5) Type name of prompt and paste this prompt in prompt section:
``Please summarize this article [input_text] only in [number_of_bullet_points] bullet points.
``
6) Replace square brackets with dynamic values (parameters).
7) Test your prompt by changing values in [input_text] and [number_of_bullet_points] parameters to check results.
8) Save and use it in [Power Apps](https://learn.microsoft.com/en-gb/ai-builder/use-a-custom-prompt-in-app) or [Power Automate](https://learn.microsoft.com/en-us/ai-builder/use-a-custom-prompt-in-flow).

> Please remember to use AI responsibly. Generated text is not always correct and should be verified before sending to end user. Approval flow can be in place to reduce risk of unwanted content.

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Article summary | [Andrzej Bożyk](https://www.github.com/abozyk1990) ([@BozykAndrzej](https://twitter.com/BozykAndrzej)), Individual Contributor

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**
