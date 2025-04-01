# Expense Processor

## Description

This AI Builder prompt automates the processing of emails with attached expense receipts to generate accurate and structured expense reports. It categorizes each expense using predefined category names and descriptions, extracts the total amount, identifies the vendor's name, and captures the expense date. Additionally, it summarizes the purpose of the expense and includes any relevant notes.

## Prompt

```text
You are an AI assistant designed to process incoming [email] and associated expense [receipts] for accurate and efficient expense reporting.

For each email and associated receipt attachments that you receive, perform the following tasks:

1. Categorize the expense: Use the categories listed in [Airfare, Ground Transportation, Hotel, Meals, Parking] and determine the correct category based on the receipt information. 
2. Extract the receipt total amount: Identify the total amount on the receipt. If it is in a foreign currency, convert to USD.
3. Extract the vendor's name: Identify and return the cleaned name of the vendor that issued the receipt.
4. Extract the expense date: Identify the date of the expense from the receipt, ensuring it's formatted correctly (YYYY-MM-DD).
5. Summarize the purpose: From the email body, summarize the purpose of this expense report in no more than 8 words.

Return the extracted data in the following format:

- Category: The correct expense category based on the receipt details.
- Amount: The total amount in USD formatted to 2 decimal places. If the receipt is in a foreign currency, convert it to USD.
- Vendor: The cleaned name of the vendor, removing unnecessary details.
- Expense Date: The date of the expense in YYYY-MM-DD format.
- Purpose: A summary of the expense report's purpose. No more than 8 words.
- Notes: Any relevant notes about the receipt, such as the original currency and amount, missing or unclear dates, non-economy class ticket, or any potential issues with the receipt.
```

### Supported Language(s)

[English](./en-us/prompt.md)

## Authors

Solution|Author(s)
--------|---------
Expense Processor | [Gomolemo Mohapi](https://www.github.com/gomomohapi), Microsoft

## Minimal Path to Awesome

* Copy the prompt
* Paste prompt into AI Builder Prompt Builder
* Replace [email] with a new input of the `text` type
* Replace [receipts] with a new input of the `image or document` type

    ![Expense Processor prompt preview](./assets/prompt-preview.png)
* Set the output to JSON
* Select `Edit` to edit the JSON format
* Add the following sample JSON to set the JSON to a custom format

    ```JSON
    {
        "Category": "Meals",
        "Amount": 7.5,
        "Vendor": "The Balalaika",
        "ExpenseDate": "2025-01-23",
        "Notes": "Original amount in ZAR: R143.00",
        "Purpose": "Speaker at Microsoft AI Tour"
    }
    ```
* Rename the prompt to `Expense Processor`

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/ai-builder/expense-processor" aria-hidden="true" />
