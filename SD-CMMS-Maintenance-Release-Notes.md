## SD CMMS Maintenance Releases

### 2.0.1

#### Enhancements

- Re-numbered objects to ISV range.

#### Bug Fixes

- Fixed a compile error in a Codeunit.

### 2.0.0

#### Enhancements

- Updated the About Page.

- Updated the Chart Control to the latest version in the Simply Dynamics Control Suite.

- Updated the HTML Editor to the latest version of the Simply Dynamics Control Suite.

- Added a check on ad-hoc Jobs, that if "Meter Required" is ticked, then a Fixed Asset is mandatory on the Job Card.

- Fixed an issue where on the Job status, after all remaining quantities/amounts were posted, users could not complete the job using the page action 'Finish job'.

- Updated the code to use the new Simply Dynamics import/export module.

- Updated the code to use the ISV Simply Dynamics Controls.

- Posted jobs are not being updated on RC cues 'Completed Jobs' and 'Completed Jobs - Today'

- Added functionality to not allow users to complete/finish lines if any unposted job task/kit lines exist.

- Re-brand and re-name the 'Archived' functionality in Maintenance Manager to 'Finished'. (Users will see the Jobs as Open, In Progress, Complete, and Finished). Create new Finished Cues and display on the Role Centres. The Finished Cues will look to the Archived table.

- Add a warning on Posting of a Job if the Unit Cost is 0 (for both Items and Resources) but allow to post.

- Change to logic to not allow users to reset an 'In Progress' Job back to 'Open'.

- Allow Users to enter a Negative Quantity in Jobs.

- Do not allow users to change Roster plan lines if same line is marked as active.

- In a Job created by the Create Scheduled Jobs functionality, we need to be able to add tasks and kits to the Jobs in addition to those tasks and kits copied in to the Job from the Plan.

- In the Component Register Card, move the Fixed Asset Description to be directly underneath the Fixed Asset No.

- Create a check that will not allow users to delete jobs with status 'In Progress'.

- When running the Action 'Create Scheduled Job', add a check not to create Jobs for incomplete Rosters/Plans. Active Rosters should have a Plan Code and a Schedule Code.

- On the Job Card, subpage Job Kit, the field Quantity should not calculate with minus sign.

- The Instructions Icon in the Job Task Card was showing an incorrect image.

- Added functionality to check on deleting a Plan, if the Plan has active Plan and Roster lines (and prevent users from deleting).

- Removed the Add-In option on the Import/Export Action on the Setup Card.

- The Chart Control is showing 'Credit Controller Visual' - this should be 'Maintenance Manager Visual'.

- In the Plan Kit Sub-List, display the Related Code's Description.

- In the SD-M Plan Card, renamed the Kit field at Task level to Task Kit for clarity.

- In the SD-M Schedule Card - promoted the Schedule Code and Description to the General FastTab.

- Add the Master Data Menu Items, in the Master Data Menu of the Role Center, as Actions in the Setup Card.

- Updated the Plan Line visibility in Roster List. Enabled lines are now bold.

- Object Reshuffle.

- Created a change to the logic where the Item Journal was not transferring costs from the Job Kit lines, but was validating from Item Card.

- W1 Release.

- Create a Component Register Card.

- Split out the Job Posting and the Job Archiving functionality.

- Allow for Partial Posting of Jobs (posting of Tasks).

- Functionality changes to Quantity, Quantity to Consume, Quantity Consumed.

- In the Plan Setup tab in the Job Card, select off the new hierarchy (Rosters, Fixed Assets, Plans).

- Add the New Job Action to the Ribbon on the Role Centre Item.

- In the Create Scheduled Jobs Action, add the new Roster/Plan combination structure.

- Put the Create Schedule Action in the Setup Card onto the Role Centre.

- Task Card - Move the Plan Kit to a FactBox.

- Tasks - improvements to the Instructions Editor - Moving an Image.

- New structure for Schedules, Maintenance Rosters, and Plans.

- Upgrade to the new html editor.

- Upgrade to new charts.

- Create an Assignable 'Equipment' List.

- In the Subpage SD-M Plan Kit SubList, update the Unit Cost from related source card.

- In the Subpage SD-M Plan Kit SubList, validate the field UOM from source.

- Page SD-M Plan Task Card, in subpage Plan Kit, add field Amount.

- Page SD-M Plan Card, subpage Plan Tasks, add a drilldown on field 'Kit'.

- Post and Archive Job - change logic so that type Resource is also posted.

- In the Page SD-M Job Task SubList, force the user to supply a task description and not allow blank lines to be inserted.

- Page SD-M Job Card - on creating a new Job via the function Schedule Job change logic of updating the Quantity to Consume.

- Page SD-M Job Card - remove the New action on the Task and Kits line.

- In the SD-M Archive Job List remove the Delete action.

- Page SD-M Job List on action 'Delete' raise a message to confirm record deletion.

- Page SD-M Schedule Job - New Job generation filter options.

- Page SD-M Manager Role Center - update navigation pane item caption.

- Surface our SD Job Queues Page in SD Maintenance Manager.

- Allow users to add a Quantity to the Job Kit when creating a once off Job (i.e. the Job is not based on a Scheduled Plan.)

- Job Card - Promote fields on FastTabs.

- Plan Card - Promote Description field on the FastTab.

#### Bug Fixes

- Fixed an issue where in the Roster Card, when a New Plan was selected, the Plan Card opened but was not blank - the Plan Card showed the details of another already existing Plan.

- Fixed an issue in the Roster Card, where when a New Plan was selected, and escape was selected from the Plan Card, a message window was raised.

- Fixed a bug where the Res. Ledger Entries, created by the Maintenance Job Postings, were being stamped with the No. Series of the Item Journal Batch Name specified on the SD-M Setup Card.

- Fixed a bug where the Item Ledger Entries, created by the Maintenance Job Postings, were being stamped with the No. Series of the Resource Journal Batch Name specified on the SD-M Setup Card.

- Fixed an issue where the "Last No. Used" on the "No. Series Line" table was not being updated/stamped when Resource Journal Lines or Item Journal Lines were Posted (as per standard NAV) when a Maintenance Job was Posted.

- Fixed an issue whereby If there was nothing to Post for an "In Progress" Job, users were not prompted that 'There is nothing to Post'.

- Fixed an issue where in the Chart Control, drilling down on Completed, In Progress, and Overdue Jobs by Status all showed a list of Open Jobs.

- Fixed an issue where if a Job of status Open was changed to status Completed, an error message was raised.

- Fixed an issue where the create 'New Job' action, on the Plan Code field, gives a lookup on Roster Plan lines that are not enabled/active.

- When the action 'Create Scheduled Job" is run with no 'To Date' specified, the Action does nothing - a change was made to raise a message.

- Change job status Open to status Completed results with an error message (job created using function 'New Job')

- Fixed an issue in the Roster card where on the Plans FastTab, when choosing the line Action 'Plan Card', the Plan Card that opens is blank.

- Creating a new Plan from the Roster Card results in an error message raised on the Plan Card when updating the Plan Kit.

- The Rosters List/Card Page FactBoxes were not showing the correct number of Jobs.

- In the Manager Role Centre, users were unable to drill through on the Plans Cue in the Manager Activities Group.

- 2017 Compliance.

- Fixed an issue where users needed to press ok twice to exit the SD-M Component Register Card.

- Fixed an issue where instructions were not being saved in the SD-M Component Register Card.

- In the SD-M Plan Task Card, changed the Plan Kit List to Task Kit.

- When returning from the SD-M Plan Task Card to the SD-M Plan Card, the FlowFields (Kit and Amount LCY) for the newly added Tasks were not updated until the Page was refreshed.

- In the SD-M Plan Card, Plan Equipment FastTab, there was no way to create a new Equipment Code on the fly.

- In the SD-M Setup Card the Title of FastTab was renamed from Default JournalS to Default Journals.

- Fixed an issue when updating a Plan in the Roster - End Date issue when updating section 'Plans' line.

- Fixed issue when adding Items to Kits - allow users to input the Quantity (it was working off the Quantity to Consume) and use the value entered in Quantity in the calcs.

- Fixed issue in Task Card, Instructions field, where Images saved were disappearing.

- The focus on open page SD-M Plan Task Card was on the Instructions field.

- Maintenance Plan List - String length error was raised on input of Plan Code.

- Instructions were not always saved when entered into the SD-M Job Task Card.

- In the SD-M Plan Task Card, on creation of an additional new Plan Kit line, the line was not assigned to the parent Plan Task.

- On the SD-M Manager Role Center, the cue field 'Completed Job' was not filtering data correctly.

- SD-M Job Kit SubList update Job Kit lines - field 'Quantity Consumed' was updated before Job lines were posted.

- For a Job with all tasks/kits completed, the Job Status was not automatically updated as Complete.

- Plan Task lines Kits were not transferred into Jobs.

- Page SD-M Job List FactBox Job Details - field drill down not working.

### 1.0.0

#### Enhancements

- Created Setup table, pages and associated functionality.

- Created Maintenance Roster table, pages and associated functionality. 

- Created Fixed Asset table, pages and associated functionality. 

- Created SD-M Maintenance Plans table, pages and associated functionality. 

- Created Plan, Task and Kit tables, pages and associated functionality. 

- Created Meter Reading table, pages and associated functionality. 

- Created Schedule table, pages and associated functionality. 

- Created Job, Task and Kit tables, pages and associated functionality. 

- Created SD-M Job Archive, Task Archive and Kit Archive tables, pages and associated functionality. 

- Created Role Centers: Manager Role Center - Creates Jobs. Worker Role Center - Completes Jobs. Mobile Role Center - Mobile version of the Worker Role Center. 

- Created a customised, slimmed down, version of the standard NAV Requisition Worksheet that focuses on Maintenance Job Data (non-completed jobs) and generates Purchase Orders. 

- Created HTML Editor Control Add In XMLPort. 

- Created import/export Xmlports for Setup and Historic Data. 

- Cleaned up code.

