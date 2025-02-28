# Social Media Engagement Analyzer

## Description

This prompt analyzes social media interactions to measure engagement and user activity. It will output a JSON object which you can use to send to a back-end service.

## Prompt

```text
Analyze this [social media post] and these [comments] to determine sentiment and engagement potential. Exclude the comments from the original author. Please give me advice on how to improve the engagement next time.
```

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Social Media Engagement Analyzer | [Daniel Laskewitz](https://www.github.com/laskewitz), Microsoft

## Minimal Path to Awesome

- Copy the prompt
- Paste prompt into AI Builder Prompt Builder
- Replace [social media post] by a new input of the `image or document (preview)` type
- Replace [comments] by a new input of the `image or document (preview)` type
- Set the output to JSON
- Select `Edit` to edit the JSON format
- Add the following sample JSON to set the JSON to a custom format

```JSON
{
  "sentiment": "positive",
  "score": {
    "impressions": 20954,
    "members_reached": 11701,
    "reactions": 340,
    "comments": 37,
    "reposts": 47
  },
  "engagement_potential": 8.5,
  "advice": "To improve engagement next time, consider incorporating more interactive elements such as polls or questions to encourage more comments. Additionally, sharing personal insights or experiences related to the learning path can make the post more relatable and engaging. Regularly responding to comments can also help maintain and boost engagement."
}
```

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/ai-builder/social-media-engagement-analyzer" aria-hidden="true" />
