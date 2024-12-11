# Automatic Absence Management

## Description

This prompt helps automate employee absence management. It notifies the relevant parties, updates the shared calendar, and handles additional tasks based on absence length and replacement requests.

## Prompt
I want to create a flow to manage team absences automatically. The flow should start when an employee sends an email with the subject 'Absence' and specifies the start and end dates in the body of the email. The flow should perform the following actions:

- Extract the start and end dates of the absence from the body of the email.
- Update a shared team calendar with an event titled 'Absence: [Employee Name]' and the corresponding dates.
- Send an email to the employee's direct supervisor notifying them of the absence.
- If the absence is longer than 3 days, notify the HR department.
- If the employee requested a replacement, automatically assign a task in Microsoft Planner to the designated substitute.
- Confirm to the employee via email that their absence has been processed."

Flow Technical Details:

Trigger:

- When a new email is received in a specific folder (e.g., "Absences").

Actions:

- Extract the start and end dates from the email using dynamic content expressions.
- Create an event in the shared team calendar using Microsoft Graph or the Office 365 Calendar connector.
- Send notifications via email and Teams messages based on the defined conditions.
- Create a task in Planner if a substitute is requested.

[Open in Power Automate](https://make.powerautomate.com/create/fromNaturalLanguage?prompt=I%20want%20to%20create%20a%20flow%20to%20manage%20team%20absences%20automatically.%20The%20flow%20should%20start%20when%20an%20employee%20sends%20an%20email%20with%20the%20subject%20%27Absence%27%20and%20specifies%20the%20start%20and%20end%20dates%20in%20the%20body%20of%20the%20email.%20The%20flow%20should%20perform%20the%20following%20actions%3A%20-%20Extract%20the%20start%20and%20end%20dates%20of%20the%20absence%20from%20the%20body%20of%20the%20email.%20-%20Update%20a%20shared%20team%20calendar%20with%20an%20event%20titled%20%27Absence%3A%20%5BEmployee%20Name%5D%27%20and%20the%20corresponding%20dates.%20-%20Send%20an%20email%20to%20the%20employee%27s%20direct%20supervisor%20notifying%20them%20of%20the%20absence.%20-%20If%20the%20absence%20is%20longer%20than%203%20days%2C%20notify%20the%20HR%20department.%20-%20If%20the%20employee%20requested%20a%20replacement%2C%20automatically%20assign%20a%20task%20in%20Microsoft%20Planner%20to%20the%20designated%20substitute.%20-%20Confirm%20to%20the%20employee%20via%20email%20that%20their%20absence%20has%20been%20processed.&from=Copilot&utm_source=PromptLibrary)

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Automatic Absence Management | [Cristian Rodriguez](https://github.com/script32)

## Minimal Path to Awesome

* Copy the prompt
* Paste prompt into the Power Automate Copilot

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/power-automate/automatic-absence-management" aria-hidden="true" />
