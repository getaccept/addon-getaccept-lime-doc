hero: Integrate Lime CRM with six different ERP systems

# Changelog for Lime CRM Add-on

## v3.2.3

**Released:** 2019-08-29

**Authors:** Stefan Tägt

**Bug Fixes / Minor improvements:**

* The field on Company for Turnover LYTD is now based on invoice_date instead of paid_date.

## v3.2.2

**Released:** 2019-08-28

**Authors:** Fredrik Eriksson

**Bug Fixes / Minor improvements:**

* Field for customer number on the invoice card is now set also by the synchronization (and not just the initial migration).

## v3.2.1

**Released:** 2019-06-30

**Authors:** Fredrik Eriksson

**Bug Fixes / Minor improvements:**

* Navision changed to NAV when displaying ERP system name on Actionpad buttons.

## v3.2.0

**Released:** 2019-06-28

**Authors:** Andrea Pettersson and Fredrik Eriksson

**New Features:**

* Possibility to restrict which user groups that have access to the send to ERP buttons.
* Changes to Invoice Overview graph:
    * Is now showing all invoices (paid or not).
    * Amount is now without VAT.
    * Month and Quarter now always based on invoice date (instead of paid date if one existed).

## v3.1.0

**Released:** 2019-06-12

**Authors:** Fredrik Eriksson

**New Features:**

* Support for ERP Connector add-on ERP Master.

**Bug Fixes / Minor improvements:**

* Corrected erroneous localization strings.

## v3.0.1

**Released:** 2019-06-07

**Authors:** Fredrik Eriksson and Stefan Tägt

**Bug Fixes / Minor improvements:**

* Added missing files for calling Syncify cloud service to installation package.

## v3.0.0

**Released:** 2019-05-10

**Authors:** Fredrik Eriksson

**New Features:**

* Invoice address fields introduced. These are now sent instead of the postal address when sending a new/updated customer to the ERP system.
* Turnover Last Year To Date field added to company (visible on company card only).
* Invoice row main tab visible.
* Invoice rows are now related to the company which means there is a sub tab on companies showing all invoice rows directly.

**Bug Fixes / Minor improvements:**

* New table icons added to match new look in Lime CRM. Old icons are kept under lisa/icons/legacy folder.
* Following naming standards in add-on requirements.
* Improved localizations.
* Minor UI improvements: Removed dark-grey area behind send button and rounded corners on alert.

## v2.1.0

**Released:** 2019-03-29

**Authors:** Fredrik Eriksson

**New Features:**

* All documentation gathered in one place and now lives together with the code.

## v2.0.6

**Released:** 2019-02-18

**Authors:** Fredrik Eriksson

**Bug Fixes / Minor improvements:**

* Comments in VBA code to clarify how to configure the Consts.

## v2.0.5

**Released:** 2018-12-12

**Authors:** Fredrik Eriksson

**Bug Fixes / Minor improvements:**

* Fixes due to new Lime Store and LIP versions.

## v2.0.4

**Released:** 2018-12-12

**Authors:** Sofie Helgesson

**Bug Fixes / Minor improvements:**

* Updated pictures for Lime Store.

## v2.0.3

**Released:** 2018-11-22

**Authors:** Fredrik Eriksson

**Bug Fixes / Minor improvements:**

* Possibility to set config parameter logLevel to 'debug' or 'info'.
* Error message now does not show the complete JSON.

## v2.0.2

**Released:** 2018-05-16

**Authors:** Emil Jönsson and Fredrik Eriksson

**Bug Fixes / Minor improvements:**

* Bug that error message when sending to Fortnox was not shown and logged correctly is now fixed.

## v2.0.1

**Released:** 2018-03-26

**Authors:** Lisa Stenberg

**Bug Fixes / Minor improvements:**

* Bug: Now last five years of invoices are shown in the dashboard, as expected, instead of last four as before.

## v2.0.0

**Released:** 2018-03-02

**Authors:** Fredrik Eriksson

* Support for Syncify cloud service.
* Restructured code.
* Restructured files.
* Many minor improvements/simplifications in the code.
* Now showing message to user on success and error.
* Added metadata folder with metadata.json.
* Removed content from README.md since it is in either installation instructions pdf or on the [Lime CRM Wiki](https://docs.lime-crm.com/addons/erpconnector/start).
* New installation instructions pdf.
* Added CHANGELOG.md.
* Tables, fields and localizations now installable by LIP instead of SQL scripts.
* Added files to lip/lisa/descriptives containing descriptive expressions on tables invoice and invoicerow.
* Added visitingaddress in call to Syncify cloud service.
* Call to local Syncify service now made from javascript instead of VBA.
* Added spinning loader to show user that sending is in progress.
* Graph now falls back to invoice_date if paid_date is empty.
* Buttons for create/update are disabled until the call is complete.
* Handling if new customer is sent twice without erpid to avoid doubles in ERP system (only issue for cloud systems).

## v1.0.0

**Released:** 2017-04-30

**Authors:** Magnus Fagerlund, Christian Sandtveit, Kamilla Svendsen

* First release.
