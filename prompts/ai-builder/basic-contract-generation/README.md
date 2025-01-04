# Basic Contract Generation

## Description

This solution enables users to automatically generate professional contracts using a combination of AI Builder, Power Automate, and SharePoint. The process dynamically fills a Word template with user-provided data, formats it into a complete contract, and optionally converts it to PDF before sending it to the intended recipients.

## Prompt

Generate a professional service contract based on the following inputs:  
- Client Name: [ClientName]  
- Client Address: [ClientAddress]  
- Start Date: [StartDate]  
- Services Included: [Services]  
- Contract Duration: [Duration]  
- Additional Terms: [Terms]  

The contract must include:  
1. A formal introduction naming the parties.  
2. Clear service details and obligations.  
3. Terms and conditions.  
4. A signature section for both parties.  

Format the contract in a professional tone.

### Supported Language(s)

[English](./en-us/prompt.md)

---

## Authors

Solution|Author(s)
--------|---------
Basic Contract Generation | [Cristian Rodriguez](https://github.com/script32)

---

## Minimal Path to Awesome

### Prerequisites

1. **Access to Power Automate** with premium connectors.  
2. **SharePoint Online** library to store templates and generated contracts.  
3. **AI Builder License** for GPT model integration.  
4. A Word document template (`.docx`) with placeholders for dynamic content.  

---

### Step 1: Create the Word Template
1. Open Microsoft Word and create a contract template with placeholders. Example:
   ```
   **CONTRACT AGREEMENT**

   This contract is made between [ClientName], located at [ClientAddress], and [YourCompany], effective as of [StartDate].

   **Services Provided**:  
   [Services]

   **Duration**:  
   [Duration]

   **Terms and Conditions**:  
   [Terms]

   **Signatures**:
   ________________________  
   Client Signature  

   ________________________  
   Company Signature
   ```
2. Save the template as `ContractTemplate.docx`.
3. Upload the template to a SharePoint document library (e.g., `Templates`).

---

### Step 2: Create the Power Automate Flow

#### **Trigger**
1. Choose a trigger such as:
   - **When a form response is submitted (Microsoft Forms)**.
   - **When a new item is added to a SharePoint list**.

#### **Steps**
1. **Get Data**:
   - Retrieve data from the trigger, such as client name, address, and services.

2. **AI Builder Integration**:
   - Add the action **Generate Text with GPT (AI Builder)**.
   - Use the following prompt:
     ```
     Generate a professional service contract based on the following inputs:
     - Client Name: [ClientName]
     - Client Address: [ClientAddress]
     - Start Date: [StartDate]
     - Services Included: [Services]
     - Contract Duration: [Duration]
     - Additional Terms: [Terms]
     
     The contract must include:
     1. A formal introduction naming the parties.
     2. Clear service details and obligations.
     3. Terms and conditions.
     4. A signature section for both parties.

     Format the contract in a professional tone.
     ```
   - Map the variables to dynamic content from the trigger.

3. **Fill the Word Template**:
   - Add the action **Populate a Microsoft Word Template**.
   - Select the `ContractTemplate.docx` file from SharePoint.
   - Map placeholders (`[ClientName]`, `[Services]`, etc.) to the data retrieved from the trigger.

4. **Save the Generated Contract**:
   - Use the action **Create File (SharePoint)** to save the populated Word document in a designated folder (e.g., `GeneratedContracts`).

5. **Convert to PDF (Optional)**:
   - Add the action **Convert Word Document to PDF**.
   - Save the PDF version in a specified folder.

6. **Send the Contract**:
   - Add the action **Send an Email (Outlook)**.
   - Attach the generated Word/PDF document and send it to the client.

---

### Step 3: Test the Flow
1. Submit a form response or add an item to the SharePoint list.
2. Verify that:
   - The contract is correctly generated and saved in the designated folder.
   - The email with the attachment is sent to the client.

---

### Example Output

**Word Template Example**:
```
**CONTRACT AGREEMENT**

This contract is made between John Doe, located at 123 Main Street, and Synerbyte, effective as of 2024-12-13.

**Services Provided**:  
- IT Maintenance  
- Cloud Integration  

**Duration**:  
12 Months

**Terms and Conditions**:  
- All payments are due within 30 days of invoice.
- Support is available 24/7 during the contract period.

**Signatures**:
________________________  
John Doe (Client)  

________________________  
Synerbyte (Company)
```

---

## Disclaimer

**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

<img src="https://m365-visitor-stats.azurewebsites.net/powerplatform-prompts/samples/ai-builder/basic-contract-generation" aria-hidden="true" />
