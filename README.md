Latest releases added to https://github.com/navancommits/SitecoreCompleteInstallAssistant

# Sitecore Commerce Install Assistant (SCIA) : GUI-based installation for Sitecore Commerce Instances
KEY FEATURE:
- The tool is based on Sitecore Install Assistant (SIA) naming convention. So, if you installed Sitecore through SIA, just change the SiteNamePrefix field in the SiteInfo tab and the other fields will be automatically filled for you except for Solr and Braintree setting.

What is added in SCIA_2.8
- Auto-download pre-requisites from dev.sitecore.net
- the exe must now be placed in the same location as Sitecore.Commerce.WDP.2020.08-6.0.238 folder if you are copying pre-requisites manually

What is added in SCIA_2.7 
- Streamlined enabling/disabling of Install/Uninstall buttons
- Fixed issues picking up correct values for ports
- Preview button is enabled throughout the steps
- Only after the user validates the db connectivity, next button gets enabled for step 2
- All menu buttons get enabled only after crossing step 2
- After step 2, Press Validate All button to fix validation issues and then the install/uninstall buttons get enabled/disabled 
- Opened delete button after step 1 so that it can be useful in deleting orphan data by just entering a site prefix

What is added in SCIA_2.6 
- Built for x64 processor 
- Tested for more scenarios, stores and retrieves SCIA data

What is added in SCIA_2.5 
- Pops default settings first time
- User persists settings
- Settings picked up and SCIA details stored in db on install
- Next time, SCIA details like port info picked automatically

What is added in SCIA_2.4 (Unstable)
- Even smaller exe, 300 KB
- Preview button to view PS Script at any point of filling details
- Settings form for one-time or once-in-a-while settings like Braintree, site suffix etc.

What is added in SCIA_2.3
- Its a smaller exe
- Zap functionality is cleaner
- Pre-requisites form has URLs for easy access

What is added in SCIA_2.2
- DB Connection Check
- Solr Url Check
- Validates if Solr version is 8.4.0
- Locked down controls to streamline user entry
- Validate All button

What is added in SCIA_2.1
- Zap that removes both Commerce and Sitecore footprints from the machine in one-shot
- Removed a few validations from uninstall button to make launch easier

The #Sitecore Commerce Install Assistant (SCIA) supports Sitecore Commerce 10 installation as of now. Built as a #dotnet 2019 Windows Application, it can -

- Generate install and uninstall scripts for Sitecore Commerce 10
- Launch powershell to perform the install /uninstall
- Track commerce installations in a machine in order to enable uninstall in a later stage 
- If trying a second or multiple Commerce instances in a machine, takes care of making things unique for successful install 
- Starts from where SIA finishes: it can install commerce on Sitecore SXA websites... 
- Auto-populate as much info with respect to SXA site... user just has to enter site prefix
- Pre-generate and auto-fill fields as much... yes, solr details are populated automatically
- Show default values for overriding.... from settings form
- Alert if an installation is Sitecore-based and also checks SXA as stated above and doesn't launch commerce install (Done)

How to use?
 - After having installed Sitecore SXA website using SIA, Download the SCIA zip, unzip it, just add the exe under  \Sitecore.Commerce.WDP.2020.08-6.0.238\SIF.Sitecore.Commerce.5.0.49 
 - Right click the exe and "RUN AS ADMINISTRATOR"
 
 For more details, check these blogs:
- https://navansitecorenotes.blogspot.com/2020/10/a-sneak-peek-at-scia-features-part-1.html
- https://navansitecorenotes.blogspot.com/2020/10/sitecore-commerce-installer-scia.html

Done:
- Pre-requisites listing check tab
- Db connectivity check
- Solr connectivity check
- Settings tab that stores one-time input like solr, braintree etc. 
- Store and pick specific details of the instance inc. port 
- Solution for PS task issues occuring during repeat runs 
- Option to cleanup C:\certificates, c:\users, solr folders, services, webroot, app pools, dbs related to whole of Sitecore Instance  
- Download and install pre-requisites like Redis, aspnetcorev2 (windows bundle 3.1.6 and above) etc.

To do:
- Support for Sitecore Commerce 9.3 
- Look at support for versions earlier than Sitecore Commerce 9.3
