# Construction Site Safety Compliance Checker

## Description

This prompt analyzes an image of a construction site to detect safety violations, assess OSHA compliance, and identify potential hazards. It evaluates personal protective equipment (PPE) usage, fall risks, equipment placement, fire hazards, and general site cleanliness. The output provides a structured safety assessment, assigns a risk level, and suggests corrective actions to improve worker safety and regulatory compliance.

## Prompt

```text
Analyze the [construction site] to detect safety violations and assess OSHA compliance. Identify potential hazards such as missing PPE, improper scaffolding, fall risks, or equipment obstructions. Provide structured feedback on violations and suggest corrective actions.
```

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Construction Site Safety Compliance Checker | [April Dunnam](https://www.github.com/aprildunnam), Microsoft

## Minimal Path to Awesome

- Copy the prompt
- Paste prompt into AI Builder Prompt Builder
- Replace [construction site] by a new input of the `image or document (preview)` type
- Set the output to JSON
- Select `Edit` to edit the JSON format
- Add the following sample JSON to set the JSON to a custom format

```JSON
{
  "OSHA_compliance": "Yes/No",
  "detected_hazards": {
    "PPE_violations": "List of missing or improperly used personal protective equipment",
    "fall_risks": "Description of unprotected edges, lack of guardrails, etc.",
    "equipment_safety": "Assessment of machinery placement and safety measures",
    "fire_safety": "Evaluation of fire hazard risks (flammable materials, blocked exits, etc.)",
    "site_clutter": "Yes/No - Are there obstructions that create tripping or operational hazards?"
  },
  "risk_level": "Low/Medium/High",
  "recommendations": "Actionable steps to improve compliance and safety."
}
```

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/ai-builder/construction-site-osha-eval" aria-hidden="true" />
