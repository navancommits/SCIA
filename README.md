# Sitecore Commerce Install Assistant (SCIA) : GUI-based installation for Sitecore Commerce Instances
KEY FEATURE:
- The tool is based on Sitecore Install Assistant (SIA) naming convention. So, if you installed Sitecore through SIA, just change the SiteNamePrefix field in the SiteInfo tab and the other fields will be automatically filled for you except for Solr and Braintree setting.

What is added in SCIA_2.2
- DB Connection Check
- Solr Url Check
- Validates if Solr version is 8.4.0
- Locked down controls to streamline user entry
- Validate All button

What is added in SCIA_2.1
- Zap that removes both Commerce and Sitecore footprints from the machine in one-shot
- Removed a few validations from uninstall button to make launch easier

The #Sitecore Commerce Install Assistant (SCIA) supports Sitecore Commerce 10 installation as of now. Built as a #dotnetcore 2019 Windows Application, it can -

- Generate install and uninstall scripts for Sitecore Commerce 10
- Launch powershell to perform the install /uninstall
- Track commerce installations in a machine in order to enable uninstall in a later stage (in progress)
- If trying a second or multiple Commerce instances in a machine, takes care of making things unique for successful install (Done)
- Starts from where SIA finishes: it can install commerce on Sitecore SXA websites... (Done, finds if the site is SXA-enabled)
- Auto-populate as much info with respect to SXA site... (Done)
- Pre-generate and auto-fill fields as much... (Done)
- Show default values for overriding.... (Done)
- Alert if an installation is Sitecore-based and also checks SXA as stated above and doesn't launch commerce install (Done)

How to use?
 - After having installed Sitecore SXA website using SIA, Download the SCIA zip, unzip it, just add the exe under  \Sitecore.Commerce.WDP.2020.08-6.0.238\SIF.Sitecore.Commerce.5.0.49 
 - Right click the exe and "RUN AS ADMINISTRATOR"
 
 For more details, check these blogs:
- https://navansitecorenotes.blogspot.com/2020/10/a-sneak-peek-at-scia-features-part-1.html
- https://navansitecorenotes.blogspot.com/2020/10/sitecore-commerce-installer-scia.html

Work in progress:
- Pre-requisites listing check tab - Done
- Db connectivity check
- Solr connectivity check
- Settings tab that stores one-time input like solr, braintree etc. 
- Store and pick specific details of the instance inc. port 
- Support for Sitecore Commerce 9.3
- Look at support for versions earlier than Sitecore Commerce 9.3
- Solution for PS task issues occuring during repeat runs - Done
- Option to cleanup C:\certificates, c:\users, solr folders, services, webroot, app pools, dbs related to whole of Sitecore Instance  - Done
- Download and install pre-requisites like Redis, aspnetcorev2 (windows bundle 3.1.6 and above) etc.
