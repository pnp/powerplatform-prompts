# Feedback Classification

## Description

This prompt helps to designed to classify text from surveys, reviews, or any diologe, and determine if the user is asking a question, offering a suggestion, or simply leaving a closed end comment.

## Prompt

Categorize [text] into one of the given categories: “Suggestion”, “Question”, “Comment”. Return only one of the given categories. If the text isn’t offering a suggestion, or asking a question, simply respond with the comment classification. As a result, output one of the following options in JSON format as an array: {“Classification”: [Suggestion]}, {“Classification”: [Question]}, {“Classification”: [Comment]}.

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Feedback Classification | [Reid Schmidling](https://github.com/schmid1208)

## Minimal Path to Awesome

* Log into Power Autoamte, or Power Apps
* Along the left menu find AI Hub or AI Prompts
* Create a new prompt
* Copy the prompt
* Paste prompt into the prompt you just created
* Click save, and use the prompt

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**
