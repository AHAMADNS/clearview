# Clearview Design Notes

## ER Diagram
- See `https://lucid.app/lucidchart/ca116313-477d-4042-869a-5b72181082dd/edit?viewport_loc=-347%2C-481%2C2601%2C1170%2C0_0&invitationId=inv_c5e2605d-a40b-461e-a20e-0bc19ed08b52` 

## Object Relationships (summary)
HCP__c (Healthcare Provider) includes a lookup to Territory__c, linking each provider to a specific region.

Product__c stores product metadata including drug type and expiry period.

Sample_Request__c connects to both HCP__c and Product__c, capturing who requested the sample and which product was requested. It also tracks quantity, status, priority, and request date.

Inventory__c links each Product__c to a Territory__c, enabling territory-level tracking of available stock.

Territory__c defines geographic regions and includes a region picklist.

## Key Fields


## Notes

