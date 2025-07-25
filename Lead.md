# What is a Lead in Salesforce Sales Cloud?

In Salesforce Sales Cloud, a Lead represents a potential customer — someone who has shown interest in your product or service but hasn't made a full purchase yet. Think of a Lead as the first step in the sales process.

## Example of a Lead

1. Imagine you run a software company.  
   Someone named Jane Doe visits your website and fills out a contact form to get more information.  
   You collect her details: Name, Email, Company, Phone, etc.

2. This information becomes a Lead in Salesforce.  
   Jane Doe is a Lead — she’s interested, but your sales team hasn’t yet verified if she’s a good fit.

Once your team contacts her and confirms she’s truly interested and qualified (for example, she has the budget and authority to buy), you can convert this Lead into:
- An Account (Jane’s company)
- A Contact (Jane herself)
- And possibly an Opportunity (a potential deal)

## 💡 What is a Converted Lead?

In Salesforce, a Lead is someone who might be interested in your product or service (like a potential customer).  
When that lead becomes more serious — for example, they’re ready to talk about buying — you convert them into:
- An Account (the company),
- A Contact (the person), and
- An Opportunity (the potential sale).

## 🔁 How Can Leads Be Converted?

- You can convert them manually in Salesforce.
- Or, you can do it programmatically using the `convertLead()` function in code.

## 🔒 What Happens After Conversion?

Once a lead is converted:
- It becomes read-only (you can't edit it anymore by default).
- You can still view or search for it.
- Only users with special permission ("View and Edit Converted Leads") can update it.

## 🧾 Special Fields Set During Conversion

When a lead is converted, Salesforce fills in some special fields:

| Field                      | What It Means                                |
| -------------------------- | -------------------------------------------- |
| **IsConverted**             | True if the lead has been converted.         |
| **ConvertedDate**           | The date the lead was converted.             |
| **ConvertedAccountId**      | The ID of the new Account that was created.  |
| **ConvertedContactId**      | The ID of the new Contact.                   |
| **ConvertedOpportunityId**  | The ID of the Opportunity (if one was made). |
| **Status**                  | The lead's final status before conversion.   |
