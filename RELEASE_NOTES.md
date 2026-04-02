# v1.0.0

## Features


* **Budget Planning:** Plan program-wise budgets using categories and sub-categories to break down allocations into manageable sections and keep your team aligned.
* **Lead, Donor & Grant Management:** Automatically convert qualified leads into donors. Manage donor information and track the full lifecycle of each grant from application to closure.
* **Expense & Utilization Tracking:** Link expenses directly to specific grants and budgets, ensuring accurate fund utilization tracking for stress-free audits.
* **Real-Time Reports & Dashboards:** Instantly view fund utilization through live visual dashboards and reports.
* **Document Repository:** Securely store compliance and legal documents (e.g., FCRA certificates, 80G registrations), track expiry dates, and receive automated renewal notifications.

## Bug Fixes

* Fixes budget sub-category link validation bugs in Utilisation Records.
  Properly validates budget sub-category links in the utilisation record to prevent data mapping errors. ([#9efaccd](https://github.com/T4GC-Official/funder_management_system/commit/9efaccd))

* Fixes auto-generation of Budget Sub-Category naming series.
  Automatically generates the naming series for sub-categories within a Budget Plan and automatically calculates and updates the budget breakdown accurately. ([#c48fd0b](https://github.com/T4GC-Official/funder_management_system/commit/c48fd0b), [#8537e13](https://github.com/T4GC-Official/funder_management_system/commit/8537e13))

* Prevents quick entry for Budget Sub-categories and makes currency field read-only.
  Removes the quick entry option for budget sub-categories to enforce structured data entry, and sets the currency field as read-only to avoid unintended edits. ([#c9c5592](https://github.com/T4GC-Official/funder_management_system/commit/c9c5592), [#0043dba](https://github.com/T4GC-Official/funder_management_system/commit/0043dba))

* Fixes granting agreement progress bar visibility for restricted users.
  Refines permissions so users with read-only access can properly view the grant agreement progress bar without encountering access restriction issues. ([#53c5428](https://github.com/T4GC-Official/funder_management_system/commit/53c5428))

* Fixes the issue where cancelled Expense Items remained in the Utilisation Record.
  Automatically strips visually cancelled Expense Item rows from child tables and properly removes them from the Utilisation Record before deletion. ([#07da6cf](https://github.com/T4GC-Official/funder_management_system/commit/07da6cf), [#2b33a60](https://github.com/T4GC-Official/funder_management_system/commit/2b33a60))

* Fixes fetching logic for POC assigned emails within Lead creation.
  Updates the system to accurately fetch the Point of Contact (POC) email when assigning POCs within the lead doctype and re-aligns the email field position. ([#7d18569](https://github.com/T4GC-Official/funder_management_system/commit/7d18569), [#dc05fe9](https://github.com/T4GC-Official/funder_management_system/commit/dc05fe9))

* Fixes navigation errors in reports and resolves a syntax error.
  Corrects navigation flows within system reports and fixes syntax errors that were impacting overall execution stability. ([#a0ba218](https://github.com/T4GC-Official/funder_management_system/commit/a0ba218), [#457575a](https://github.com/T4GC-Official/funder_management_system/commit/457575a))

* Fixes permission issues with Budget Plan Document cancellations.
  Allows `fms_admin` to cancel a Budget Plan doctype while explicitly removing the baseline Submit permission. Fixes underlying fundraising permission errors for Currency. ([#ee5dd3d](https://github.com/T4GC-Official/funder_management_system/commit/ee5dd3d), [#177b2ea](https://github.com/T4GC-Official/funder_management_system/commit/177b2ea), [#649be9c](https://github.com/T4GC-Official/funder_management_system/commit/649be9c))

* Fixes data loss risks by adding user confirmation prior to reloading.
  Forces a manual user confirmation prompt before the app natively reloads an open document, effectively preventing accidental data loss of unsaved changes. ([#4238926](https://github.com/T4GC-Official/funder_management_system/commit/4238926))
