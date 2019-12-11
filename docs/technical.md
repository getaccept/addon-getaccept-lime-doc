hero: Close your Lime CRM deals faster with GetAccept

# Technical

### GetAccept has only database structure dependencies. 

## Table and Fields
These tables and fields are required to be able to run the GetAccept integration (all these are "standard" in the most common databases). If you have other tables and fields that you use it is possible to do customization to fit you needs, but these have to be discussed with GetAccept or Lime.

### Tables we use:
document, person, company, coworker

### Fields
#### Person
Database name | type 
------------ | ------------- 
name | text field  
email | link field  
phone | text field  
company | relation field  

#### Coworker
Database name | type 
------------ | ------------- 
name | text field  
email | link field  
phone | text field  

#### Document
Database name | type 
------------ | ------------- 
comment | text field  

### Relations between tables:
(There has to be a relation between the object you place the GetAccept integration on AND the document table.)

# Two ways integration
Requires the Lime CRM API and a api key. This feature allows GetAccept to automatically post back a signed copy of your signed documents to Lime CRM. It will download the signed document with the signing certificate and store it back in the CRM.

### How to set it up in LIME CRM
1. Create a API-user.
2. Give correct permissions to the user (should follow the Lime CRM standard rules (Add/Read/Write)) 

### How to set it up in GetAccept.
1. Log on to the GetAccept web application. app.getaccept.com
2. Go to Settings --> Integrations
3. Add your api key and the server url to the integration page. (this is individual information and something that is done in the Lime Server)

Ex: Domain URL: https://[URL]/[DatabaseName] https://gaCRMDemo/getaccept-CRM

Ex: API-key: 3FD114540187E43A9264743B7742528429511C042237ACF10034DEBEAADF770ECFBD8F966187491C7C62

## Document table setup
You need to have the following fields in the Document table to be able to use the two way integration:

#### Document
Database name | type | values
------------ | ------------- | -------------
getacceptstatus | Option field |  name: Draft, key: draft, name: Sent, key: sent, name: Reviewed, key: reviewed, name: Signed, key: signed 
sent_with_ga | yes/no field  |  yes/no
comment | text field  |  
type | option field  |  name: Agreement, key: agreement

IMPORTANT: The getacceptstatus field is implemented now to be able to use in the feature. It will only set status Signed until next version, you can skip all options but signed until new feature has been implemented..

All the code in this add-on is owned and maintained by GetAccept.
