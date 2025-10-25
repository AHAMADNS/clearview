# Clearview Design Notes

## ER Diagram
- See `er-diagram.png` (placeholder). Replace with exported PNG from Lucidchart/diagrams.net.

## Object Relationships (summary)
- Account 1 — * N Contact (Contacts related to an Account)
- Account 1 — * N Opportunity (Opportunities belong to Accounts)
- Custom object `Survey__c` 1 — * N `Survey_Response__c`

## Key Fields
- Account: Name, AccountNumber, Industry
- Contact: FirstName, LastName, Email, AccountId
- Survey__c: Name, Status__c, StartDate__c
- Survey_Response__c: Survey__c (lookup), Respondent__c (Contact lookup), Score__c

## Notes
- Use standard Account/Contact where possible.
- Start with minimal required fields and expand as we implement features.
- Consider sharing model with stakeholders and iterate on `docs/er-diagram.png`.
