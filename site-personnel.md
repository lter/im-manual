# Site Personnel Lists 

## Overview
It's helpful to have an overview of how the community platform works before detailing the process of adding new people. There are two major components to the SalesForce installation behind the community platform:
* The Client (or Customer or Constituent) Relationship Management System (CRM) is basically just a relational database that is structured to hold the kind of data that organizations usually need about the people who participate in them. New participants have to be added to the CRM before anything else can happen and licenses to the CRM are expensive (therefore limited to the LTER Network Office, or LNO). 
* The community platform houses the interactions between people ("users") and groups within the Network. Customer User licenses allow individuals to login, easily update their own information, join and leave groups, post updates, and ask questions.  The thing that ties these two components together is a relationship between a single "contact" (created by the Network Office) and the related "user" (created by the Network Office when a person is added and updated by the individual).

![](images/community-platform-overview.png)


Rather than having an individual simply associated with a site or not, the new system maintains a record of prior associations and allows multiple simultaneous associations (with different sites, in different roles, and with different institutions). This is valuable for understanding how individuals interact with the Network across their careers. To accomplish it, however, we need to update **affiliations**, rather than just sites.

## Making individual updates

Sometimes, it's important to add an individual to your site right away. To add key personnel to your site between major updates, log in to LTERHub and [create a case](https://lternetwork.force.com/lterhub/s/contactsupport) with their name, role, and email address. The LNO will create a contact and a user for them and trigger a message to login and fill in other key information.

Once a user is created and they have logged in, they are able to update their own information, including email (which automatically updates the login email within 24 hours), site and institutional affiliations, ORCID, social media accounts, and research interests. They can also join discussion groups and update committee memberships.

## Making bulk updates **(new January 12, 2022)**

Usually, there are a few times a year when many people need to be added at once. Edits to LTER site personnel can now be made directly in [the LTERHub-ex-im google sheets document](https://docs.google.com/spreadsheets/d/1TSmzt-Cg2xIKlJ3uin8EoMclACThkPiWqwroG3JoPdQ/edit#gid=293749749). Lead site information managers for each site have read access to the file, but edit permissions will be granted on a sheet-by-sheet basis to only one individual per site.

### Overall workflow ###
-  The LTERHub-ex-im file updates automatically creates a backup and downloads current information in the LTERHub **on the 15th of each month**. Each site has its own tab in the spreadsheet. Before you plan to make edits, please identify one editor per site and request file edit access for them by logging into the LTERHub and [creating a case](https://lternetwork.force.com/lterhub/s/contactsupport). Your sheet will be refreshed at the same time edit access is granted. 
-  Using the instructions below, make edits to your site's personnel list. Where you do not have changes to make, simply leave the field blank or with the existing information.  Try to concentrate the editing into a short period of time to avoid the issue of users logging in and making their own conflicting edits.
-  While you are making edits, your case remains open in LTERHub. When edits are completed, update your case to notify the LTER Network Office. 
-  At this time, uploading back to LTERHub is not fully automated so that any unexpected behaviors can be quickly identified and corrected. When your upload has been completed, the spreadsheet will be refreshed and you will be notified, so you can easily confirm that the information is correct.
-  Your case will be closed out.

### Row and Column Descriptions ###

**Rows**
**Row 1** lists the common-language descriptions of each field. **Row 2** lists the SalesForce names for each field. This assists in upload and cannot be edited.
Each row represents an affiliation between an individual and a site in a particular role, for a specific period of time. Within each sheet, records are sorted first by "Current"/"Former" status and then alphabetically by last name. Be aware that the same individual may have both current and former affiliations. 

**Columns:**
-  **Database Keys:**
   -  A.  **Affiliation ID** *(hidden and protected)*: The unique key for the specific affiliation (role-site/institution-individual combination)
   -  B.  **Contact ID** *(hidden and protected)*: The unique key for the individual contact associated with that affiliation
   -  C.  **Account ID** *(hidden and protected)*: The unique key for the account (site or institution) associated with that affiliation
   -  D.  **Profile ID** *(hidden and protected)*: The unique key for the user associated with that affiliation
  
-  **Site Information:**  
   -  E.  **Acronym**: The 3-letter site acronym. This should **always** match the spreadsheet tab in which you are editing. If an affiliation with a different site needs to be created or edited, that should be done by the individual or by the designated editor for that site.
   
-  **Contact-related information:**  	
   -  F.  **Last Name**: Last name of the individual contact (can accept un-hyphenated last names)
   -  G.  **First Name**: First name of the individual contact	
   -  H.  **Middle Name**: Middle name of the individual contact (if known)
   -  I.  **Email**: Active email address of the individual contact. Be cautious in changing this. It also serves as the user's login and (especially for former site participants) you may not have the most current information.	
   -  J.  **ORCID**: Once entered, this is unlikely to change.	Users will be prompted to update ORCIDs on site registration.
   -  P.  **Site-Contact ID**: If your site uses a unique identifier for individuals that could aid in matching site and network-level information, this is the place to enter it. If you do not use such a system, please leave this field blank.	*(Located at the end as only a few sites use this field.)*

-  **Affiliation-related information:**
   -  K.  **Role (Affiliation)**: Recall that participants may have multiple simultaneous affiliations. This field holds the role for one type of affiliation with a particular site. The (limited) choices for this field are available in the drop down. Please DO NOT add choices that do not appear in the drop down selector. *Options for "Role" are detailed later on this page.
   -  L.  **Start Year (Affiliation)**: The year that this affiliation started - to the best of your knowledge. This information is not strictly required and participants can update this information directly when they register on the site.	
   -  M.  **End Year (Affiliation)**: 	The year that this affiliation ended - to the best of your knowledge. This information is not strictly required and participants can update this information directly when they register on the site. When an entered end year is less than the current year, the affiliation status will be automatically converted to "Former" at the time data is uploaded.
   -  N.  **Status (Affiliation)**: Status" has 2 options: "Current" or "Former." This reflects an individual's affiliation with the site. All newly affiliated individuals should be listed as "Current." When an individual leaves your site, they should be identified as "Former" for your site and an end date entered for their role. When their status changes to "Former" at all sites with which they had an affiliation, their LTER status will automatically change to "Inactive". As long as they maintain an active affiliation with any LTER site, their LTER status will be "Active." This field controls whether individuals appear in the site directory for the affiliated site.
   -  O.  **Primary (Affiliation)**: This boolean field identifies this affiliation as the primary one for the associated individual. In general, it should be set by the individual during the registration process.	
 
-  **User-related information:**
   -  Q.  **Active User?**: If the individual has registered, this field contains the login of the associated user. If it is blank, it likely means that the user has not registered or has not been properly associated with this affiliation.

### Specific Use Cases ###

*  **New participants:** Add new site participants at the bottom of your site's sheet, below the existing entries. Often, individuals who are new to your site actually have a prior LTER identity. When they are using the same email address, these duplicates will be caught on creation. If they are using a new email address, the LNO will eventually find and resolve them.  Fill in:	
   * Last Name 
   * First Name
   * Middle Name (if known) 
   * Email 
   * ORCID (if known): Use the full http format, e.g https://orcid.org/0000-0003-2833-956X
   * Role (with respect to your site): If the individual will hold multiple roles, add them each on a new line.	
   * Start Year (Affiliation): For new individuals, this will typically be the current year.	
   * End Year (Affiliation): For new individuals, leave this blank.
   * Status (Affiliation): Choose "Current"
   * Primary (Affiliation): If you are quite confident that this affiliation is the primary LTER affiliation for this individual, enter TRUE or conversely, FALSE. Otherwise, leave this field blank.
   * Site-Contact ID: If your site uses this field, enter the site-id for the individual. Enter the same site-id for all affiliations that individual may have with your site. If your site doesn't use this field (most sites) leave it blank.	
   * Active User?: **Leave this field blank**
   
*  **Adding roles:** Add new roles at the bottom of your site's sheet, below the existing entries and the new participants. Separate new roles from new participants with a blank line. Copy contact-related information (Last Name, First Name, Middle Name, Email, and ORCID) from an existing affiliation for that individual and update the affiliation-related information as needed.

* **Ending roles:** To end a role for an individual, simply enter the year that they stopped serving in that role into the "End Year (Affiliation)" field. If they never served that role, please contact Marty Downs (downs@nceas.ucsb.edu) for troubleshooting assistance.

* **Former participants:** Only current participants should be displaying in the [LTER directory](https://lternetwork.force.com/lterhub/s/directory). If individuals are showing up that are no longer affiliated with your site, it's usually because the LTER Network Office has no information to indicate that they are no longer actively associated with your site. In these cases, simply change the "Status (Affiliation)" field to "Former". If you can make a fair guess at an end year, include that information. If you can't guess within a year or two, leave it blank. 

## Detailed Field descriptions and options 

A few fields use limited options and will not accept any text other than the below.

* Site options: AND, ARC, BES, BLE, BNZ, CAP, CCE, CDR, CWT, FCE, GCE, HBR, HFR, JRN, KBS, KNZ, LUQ, MCM, MCR, MSP, NES, NGA, NTL, NWT, PAL, PIE, SBC, SEV, SGS, VCR
    * Special Options: EDI, LNO, INT, NWK are for personnel associated with the Environmental Data Initiative (EDI), LTER Network Office (LNO), International LTER (INT), and the Network as a whole (NWK)--for example, staff of related organizations and networks. 
* Site Role:
    * **Lead Principal Investigator:** The primary individual who is responsible for the scientific or technical direction of the project.
    * **Co-Principal Investigator:** The individuals who are formally responsible for the scientific or technical direction of the project. (Cover page investigators.) 
    * **Investigator:** An individual with substantial scientific involvement in the LTER, but who is not a Co-Principal Investigator(s). LTER Investigators need not be funded by the project.
    * **Postdoctoral Associate:** An individual with a doctoral-level degree who does research at the site, but does not hold a permanent position. Generally Postdocs are less than 5 years post-degree.
    * **Graduate Student:** A part-time or full-time student working on the project in a research capacity who holds at least a bachelor's degree and is enrolled in a degree program leading to an advanced degree.  
    * **Undergraduate Student:** A student working on the project in a research capacity who is enrolled in a degree program (part-time or full-time) leading to a bachelor's or associate's degree. 
    * **Information Manager:** A person at an LTER site that spends some or all of their time in the process of data and information management. This person may or may not be the site representative to the information management committee.
    * **Education Manager:** A person at an LTER site that spends some or all of their time in the process of education/outreach. This person may or may not be the site representative to the education/outreach committee.  
    * **Other Professional:** A person who may or may not hold a doctoral degree or its equivalent, who is considered a professional and is not reported as a Principal Investigator, Co-principal Investigator, Investigator, Postdoctoral Associate or Student. Examples include research associates, physicians, veterinarians, system experts, computer programmers and design engineers.
    * **Technical/Research Staff:** Technicians and field research personnel. 
    * **Administrative Staff:** Persons working on the project in a non-research capacity in an administrative role. 
    * **Other Staff:** Persons working on the project in a non-research capacity, such as draftsmen, animal caretakers, electricians and custodial personnel. 
    * **Interested Party:** A person who is associated with an LTER site or the Network through interest, educational programs, public outreach etc., may include educational or community partners, neighbors, board members, etc. 
    * **Retired:** _Emeritus_ Investigators who maintain an active interest in the site and the Network. Not necessarily the same as past network members (who are designated as "Former"). 

* Less-frequently used Site Role options, for individuals that you want to associate with your site in specific roles:
    * K-12 Teacher
    * Volunteer
    * Media
