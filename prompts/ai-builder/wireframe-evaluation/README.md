# App Wireframe UI/UX Analyzer

## Description

This prompt analyzes an app wireframe image and provides structured UI/UX feedback. It evaluates layout, navigation, readability, accessibility, consistency, and branding, identifying usability issues and suggesting improvements in a JSON format.

## Prompt

```text
Analyze the uploaded [wireframe] of an app and provide UI/UX feedback. Evaluate layout, navigation, readability, accessibility, consistency, and branding. Identify usability issues and suggest improvements
```

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
App Wireframe UI/UX Analyzer | [April Dunnam](https://www.github.com/aprildunnam), Microsoft

## Minimal Path to Awesome

- Copy the prompt
- Paste prompt into AI Builder Prompt Builder
- Replace [wireframe] by a new input of the `image or document (preview)` type
- Set the output to JSON
- Select `Edit` to edit the JSON format
- Add the following sample JSON to set the JSON to a custom format

```JSON
{
  "visual_hierarchy": {
    "feedback": "Brief analysis of layout and content organization",
    "issues": "• Issue 1\n• Issue 2\n• Issue 3",
    "suggestions": "1. Suggestion 1\n2. Suggestion 2\n3. Suggestion 3"
  },
  "navigation": {
    "feedback": "Brief analysis of navigation and user flow",
    "issues": "• Issue 1\n• Issue 2\n• Issue 3",
    "suggestions": "1. Suggestion 1\n2. Suggestion 2\n3. Suggestion 3"
  },
  "readability_accessibility": {
    "feedback": "Brief analysis of readability and accessibility",
    "issues": "• Issue 1\n• Issue 2\n• Issue 3",
    "suggestions": "1. Suggestion 1\n2. Suggestion 2\n3. Suggestion 3"
  },
  "consistency_branding": {
    "feedback": "Brief analysis of design consistency and branding",
    "issues": "• Issue 1\n• Issue 2\n• Issue 3",
    "suggestions": "1. Suggestion 1\n2. Suggestion 2\n3. Suggestion 3"
  },
  "overall_feedback": "Summary of key findings and top-priority improvements"
}

```

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/ai-builder/social-media-engagement-analyzer" aria-hidden="true" />
