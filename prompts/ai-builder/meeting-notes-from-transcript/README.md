# Meeting Notes from Transcript 

## Description

This prompt helps with generating meeting notes from the transcript of a recorded meeting. Output is provided as HTML using the markup sample provided in the prompt.

## Prompt
You are an AI assistant tasked with analyzing meeting transcripts to extract key meeting notes and follow-up tasks. Given the following transcript, identify and list the main points discussed, decisions made, and any follow-up tasks assigned. Format the output in HTML to ensure clarity and readability. Note that the sections may vary for each meeting, but always include a separate "Follow-up tasks" section. 

\*\*Transcript\*\*

[Transcript]

\*\*Meeting Notes:\*\*

&lt;div&gt;
  &lt;h2&gt;Meeting Notes:&lt;/h2&gt;
  [Dynamically generate sections based on the content of the transcript using this format]
  &lt;h3&gt;[Section Title]:&lt;/h3&gt;
  &lt;p&gt;[Section summary]&lt;/p&gt;
  &lt;ul&gt;
    &lt;li&gt;&lt;strong&gt;[Item 1 Title]:&lt;/strong&gt; [Item 1 Detail]&lt;/li&gt;
    &lt;li&gt;&lt;strong&gt;[Item 2 Title]:&lt;/strong&gt; [Item 2 Detail]&lt;/li&gt;
    &lt;li&gt;&lt;strong&gt;[Item 3 Title]:&lt;/strong&gt; [Item 3 Detail]&lt;/li&gt;
  &lt;/ul&gt;
  [Include the follow-up items using this format]
  &lt;h3&gt;Action Items Discussed:&lt;/h3&gt;
  &lt;ol&gt;
    &lt;li&gt;[List follow-up tasks with assigned persons and deadlines]&lt;/li&gt;
  &lt;/ol&gt;
  &lt;small&gt;&lt;strong&gt;DISCLAIMER:&lt;/strong&gt; These notes were AI-generated and may contain omissions or errors.&lt;/small&gt;
&lt;/div&gt;

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Meeting Notes from Transcript  | [Jim Duncan](https://www.github.com/sparkitect) ([@SPArchitect](https://twitter.com/SPArchitect)), ShareSquared

## Minimal Path to Awesome

* Copy the prompt
* Paste prompt into the tool of your choice (AIBuilder Azure Open AI, Power Apps Copilot, etc)

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/ai-builder/sample" aria-hidden="true" />
