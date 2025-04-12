# YOUR PROMPT NAME 

Rental Property Inspection

## Description

This prompt helps with generating a structured data model in PowerApps for a rental inspection system, including tables, relationships, and key fields to track properties, inspections, issues, and inspectors efficiently.

## Prompt

Create a rental inspection data model with the following tables: Properties (ID, Address, Type, Status), Inspections (ID, Property as Lookup, Inspector, Date, Status, Notes), Issues (ID, Inspection as Lookup, Description, Category, Severity, Status, Photo), and Inspectors (ID, Name, Contact, Assigned Properties). A property can have multiple inspections, an inspection can have multiple issues, and inspectors can be assigned to multiple properties.

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Rental Property Inspection | [Markus Franz](https://www.github.com/mmbr1606) 

## Minimal Path to Awesome

* Copy the prompt
* Paste prompt into the tool of your choice (AIBuilder Azure Open AI, Power Apps Copilot, etc)

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/prompts/power-apps/rental-property-inspection" aria-hidden="true" />
