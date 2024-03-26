# ApexWidgets
## DelegateApproversSchedule
DelegateApproversSchedule uses a custom sObject to schedule specific time periods to delegate Approval Processes from one User to another.

The sObject is called Approval_Delegation__c with the following custom fields:
  * Delegator__c -> Lookup(User): The user who will be delegating their approval processes
  * Delegatee__c -> Lookup(User): The user who will be the receiving the approval processes
  * Start_Time__c -> Date/Time: Date and time when the delegation will start
  * End_Time__c -> Date/Time: Date and time when the delegation will end
  * Active__c -> Checkbox: Checkbox to active and deactive the delegation (Automated but can be manually changed)
  * Timeout__c -> Checkbox: Read-only field to check if a certain amount of time has passed since the End Time so that the queries don't get too crowded
