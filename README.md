# SCIA
The #Sitecore Commerce Install Assistant (SCIA) supports Sitecore Commerce 10 installation as of now. Built as a #dotnetcore 2019 Windows Application, it can -

Generate install and uninstall scripts for Sitecore Commerce 10
Launch powershell to perform the install /uninstall
Track commerce installations in a machine in order to enable uninstall in a later stage
If trying a second or multiple Commerce instances in a machine, takes care of making things unique for successful install
Picks up the websites in a machine and lists down those to continue commerce install from there...
Auto-populate as much info with respect to SXA site...
Pre-generate and auto-fill fields as much...
Alert if an XP installation doesn't have sxa enabled and doesn't launch commerce install

How to use?
 - After having installed Sitecore SXA website using SIA, Download the SCIA zip, unzip it, add it under  \Sitecore.Commerce.WDP.2020.08-6.0.238\SIF.Sitecore.Commerce.5.0.49 along with all pre-requisites
 - Right click the exe and "Run as Administrator"
 
 For more details, check these blogs:
 https://navansitecorenotes.blogspot.com/2020/10/a-sneak-peek-at-scia-features-part-1.html
 https://navansitecorenotes.blogspot.com/2020/10/sitecore-commerce-installer-scia.html
