layout: page
title: "Site Identifiers"
permalink: /site-identifier/


# LTER Site Identifiers #
*Proposed plan - developed by Marty Downs (LNO), Tim Whiteaker (BLE), An Nguyen (BLE)
Draft: 2021-10-15*

**Goal:** Obtain unique identifiers for LTER sites analogous to ORCIDs for individuals that can be used to identify products and data associated with LTER programs. 

**Why:** 
Unique identifiers are recommended by FAIR guidelines to disambiguate organizations and their relationships in metadata. See, for example, DataONE’s [FAIR Assessment report](https://search.dataone.org/quality/https%3A%2F%2Fpasta.lternet.edu%2Fpackage%2Fmetadata%2Feml%2Fknb-lter-ble%2F1%2F7) or EDI's [audit tools](https://portal.edirepository.org/nis/auditReport.jsp). Ultimately, a unique site identifier can be used to link data, papers, people, and projects to the site for improved reporting. It is also on the ORCID development roadmap for use as primary affiliation.

**What:**
There are several options for systems of unique identifiers, but the [Research Organization Registry (ROR)](https://ror.org/) seems to be gaining the most traction with publishers and data repositories. ROR’s focus is the “affiliation use case” - identifying which organizations are associated with which research outputs.  

ROR has agreed to provide identifiers to all LTER sites as a batch and link them to the LTER Network. The LTER Network Office will request RORs as a batch, based on information supplied by the sites. This will help surface questions before RORs are awarded and create a more consistent structure.

The ROR structure allows three types of organizational relationships, with multiple instances of each:

-  **Parent Institutions:** A site should include both the LTER Network and their home institution as “parent” organizations
    -  Long Term Ecological Research Network
    -  University to which the LTER grant is awarded
-  **Related Institutions:** This is closest to partners and would include the field station or Experimental Forest or Range where an LTER site is located (such as Kellogg Biological Station for KBS LTER or Toolik Field Station for Arctic LTER); outreach partners (such as Asombro for Jornada LTER or Bell Museum for MSP LTER); and the institutions of co-PIs and cooperators, such as CalState Northridge for Moorea Coral Reef LTER.
    -  Environmental Data Initiative
    -  Related field stations
    -  Co-PI institutions
    -  Outreach partners https://portal.edirepository.org/nis/auditReport.jsp
-  **Child:** Sub- or spinoff organizations.

When an ROR is created, sites can use that identifier in EML metadata to identify data associated with a site, for example:
```
    <contact>
      <organizationName>NTL LTER</organizationName>
      <address>
        <deliveryPoint>680 North Park Street</deliveryPoint>
        <city>Madison</city>
        <administrativeArea>WI</administrativeArea>
        <postalCode>53706</postalCode>
        <country>United States</country>
      </address>
      <electronicMailAddress>infomgr@lter.limnology.wisc.edu</electronicMailAddress>
      <userId directory=" https://ror.org">23435@#$%#@</userId>
    </contact>
```
    
If you want to simultaneously recognize your connection with a university or field station, consider including their identifier in the `<associatedParty>` element with appropriate role descriptions.

They can also use ROR's (and other identifier systems) to decribe the publisher:
```
  <publisher>
    <organizationName>Environmental Data Initiative</organizationName>
    <electronicMailAddress>info@environmentaldatainitiative.org</electronicMailAddress>
    <onlineUrl>https://environmentaldatainitiative.org</onlineUrl>
    <userId directory="https://ror.org/">0330j0z60</userId>
    <userId directory="https://grid.ac/institutes/">grid.511300.6</userId>
    <userId directory="https://isni.oclc.org/isni/">0000000495505609</userId>>  
  </publisher>
```

## Action requested: ##
Each site Information Manager should enter information relevant to their ROR identifier in the shared spreadsheet as described below. 


### How to request an ROR identifier ###

1. Visit the [ROR Homepage](https://ror.org/) to learn about ROR IDs.
2. Check if your LTER Program has an ROR ID on the [search page](https://ror.org/search).
    - Assuming that the program does not already exist, continue to item 3. 
    - If the program does exist in the ROR directory, you will be requesting a change the [ROR update form](https://docs.google.com/forms/d/e/1FAIpQLSdJYaMTCwS7muuTa-B_CnAtCSkKzt19lkirAKG4u7umH9Nosg/viewform). You will need the site's existing ROR and should follow the guidelines below in completing the questionairre.  
3. Go to the [LTER google sheet](https://docs.google.com/spreadsheets/d/1qiUMJ1jm_EDa2uM_qQY-U6To7qleQJnntcl1a-VM3m8/edit#gid=0), and enter your information according to the instructions below. When we have received information from all sites (or as many as we can get) we will review for consistency and submit to ROR as a group.
4. Because the ROR is curated, it may still take a few months for the request to be reviewed and the identifier assigned - but doing this as a group will definitely expedite the process. The LNO will alert sites when identifiers have been assigned.

### Instructions for completing ROR spreadsheet ###

|Question|Response|Questions/Notes|
|---|---|---|
|Email|Your email address|In theory, this is for correspondence about assigning the ROR, but it is probably wise to use an IM institutional address if you have one.|
|Agree to be contacted|Yes||
|Your name|Your name|The name of the individual completing the information|
|Your organizational affiliation|Your preferred affiliation|Used only to identify the contact. This can be university, agency, or site.|
|Your role/title|Your role or title in relationship to the organizational affiliation above||
|What are you registering?|“Add a new organization to ROR” (or, if the organization already exists, “Modify the information in an existing ROR record”)||
|...please confirm that your organization is within this scope|Yes|We have already confirmed that LTERs are appropriate for ROR|
|Have you checked that this organization already has an ROR...|Yes|If your site already has an ROR, you shouldn’t have gotten this far.|
|Name of organization to be added|Name of your LTER, in the form: \<Your Site Name\> LTER (i.e “Beaufort Lagoon Ecosystems LTER”)||
|Organization website|link to LTER site home page||
|Provide a link to a webpage with research publications associated with this organization|link to your site bibliography page|This can be on your own website, your Zotero library, or on the Network website, for example: https://lternet.edu/bibliography/?lterSite=Beaufort+Lagoon+Ecosystem&searchButton=Search|
|Type of organization|Other|The Allowed types are: Education, Healthcare, Company, Archive, Nonprofit, Government, Facility, Other. We discussed this with ROR and agreed that none of the other types work for LTERs. “Education” is strictly for schools and universities. “Facility” fits the related field stations, but not the LTERs.|  
|Wikipedia page|Wikipedia page of the organization (if available): For example, for the LTER Network: https://en.wikipedia.org/wiki/Long_Term_Ecological_Research_Network|Search here: https://en.wikipedia.org/wiki/Main_Page. This should be the wikipedia page of the LTER site, if the LTER site has a wikipedia page. If the site does not have a wikipedia page, either create one or leave this cell empty. It may be tempting to use a related page, but the point is to disambiguate organizational references, so better to leave it blank if the reference is not to the same entity. This information is not essential if you don't already have one.| 
|Wikidata ID for the organization (if available)|For example: https://www.wikidata.org/wiki/Q6673290 or n/a if not available.|Search at the top right, here: https://www.wikidata.org/wiki/Wikidata:Main_Page. Instructions for obtaining a wikidata ID are linked. (It can be really fast if you just want the ID.)| 
|ISNI ID for the organization (if available)|For example: https://isni.org/isni/0000000088203822|Search ISNI here: https://isni.oclc.org/xslt/DB=1.2/SET=2/TTL=1/CMD?ACT=SRCH&IKT=8006&SRT=LST_nd&TRM=LTER|
|GRID ID for the organization (if available)|n/a|Or search here, if you think your site might have one: https://www.grid.ac/institutes|
Crossref funder ID for the organization (if available)|n/a unless your site funds other organizations and therefore has its own crossref funder ID||
|Organization abbreviation|Three letter abbreviation of your site e.g., "BLE," “AND”, “LNO”, etc.|Can accept more than 1|
|Other variations of the organization name|Include at least: 1) The name of the site completely spelled out, with both “long-term” and “long term”; 2) The three-letter abbreviation, plus the LTER abbreviation (e.g. MCR LTER); 3) Any other variations of the name (e.g. Niwot or Niwot Ridge, Moorea or Mo’orea, etc.)|See MCM’s listing for an example.|
|Related Organizations (Fill or create a new column for each related organization.)| The LTER Network will be a  parent to LTER sites and sites can also add other parent and related organizations. For example, they may want to include their institutions as a second “parent” organization or a field station, CZO, NEON site, outreach partner, etc. at the same location as a “related” organization.|Other LTER sites should be related automatically by virtue of having the same parent.| 
|City|city (or location) of the **site**, rather than the home institution|ROR uses GeoNames for this field, so what you want is the name of the location in GeoNames database that best represents the location of your site.|
|Country|The country (or continent) associated with the location of the research site||
