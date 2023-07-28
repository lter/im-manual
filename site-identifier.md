layout: page
title: "Site Identifiers"
permalink: /site-identifier/


# LTER Site Identifiers #
*Proposed plan - developed by Marty Downs (LNO), Tim Whiteaker (BLE), An Nguyen (BLE)
Draft: 2021-10-15*
Updated: 2023-07-28

Each LTER site has a unique entry in the Research Organization Registry.

**Why:** 
Unique identifiers are recommended by FAIR guidelines to disambiguate organizations and their relationships in metadata. See, for example, DataONE’s [FAIR Assessment report](https://search.dataone.org/quality/https%3A%2F%2Fpasta.lternet.edu%2Fpackage%2Fmetadata%2Feml%2Fknb-lter-ble%2F1%2F7). EDI is developing R tools to accomplish the same checks. Ultimately, a unique site identifier can be used to link data, papers, people, and projects to the site for improved reporting. It is also on the ORCID development roadmap for use as primary affiliation.

**What:**
There are several options for systems of unique identifiers, but the [Research Organization Registry (ROR)](https://ror.org/) seems to be gaining the most traction with publishers and data repositories. ROR’s focus is the “affiliation use case” - identifying which organizations are associated with which research outputs.  

ROR has provided identifiers to all LTER sites as a batch and links them to the LTER Network.

The ROR structure allows three types of organizational relationships, with multiple instances of each:

-  **Parent Institutions:** A site should include both the LTER Network and their home institution as “parent” organizations
    -  Long Term Ecological Research Network
    -  University to which the LTER grant is awarded
-  **Related Institutions:** This is closest to partners and would include the field station or Experimental Forest or Range where an LTER site is located (such as Kellogg Biological Station for KBS LTER or Toolik Field Station for Arctic LTER); outreach partners (such as Asombro for Jornada LTER or Bell Museum for MSP LTER); and the institutions of co-PIs and cooperators, such as CalState Northridge for Moorea Coral Reef LTER.
    -  Environmental Data Initiative
    -  Related field stations
    -  Co-PI institutions
    -  Outreach partners
-  **Child:** Sub- or spinoff organizations.

When an ROR is created, sites can use that identifier in EML metadata to identify data associated with a site, for example:

```xml
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
      <userId directory=" https://ror.org">https://ror.org/04gq8q482</userId>
    </contact>
```
    
In addition to identifying associations directly within the ROR record (LTER network, home institution, EDI, etc.) they can also be specified in the EML  `<associatedParty>` element with appropriate role descriptions. It would make sense to use this option for dataset specific affiliations.

```xml
    <associatedParty>
      <organizationName>United States Geological Survey</organizationName>
      <onlineUrl>http://www.usgs.gov/</onlineUrl>
      <userId directory="https://ror.org/">https://ror.org/035a68863</userId>
      <role>instrumentation provider</role>
    </associatedParty>

```

The `<publisher>` element will be used by EDI and will be automatically inserted (replaced) upon data submission:

```xml
  <publisher>
    <organizationName>Environmental Data Initiative</organizationName>
    <electronicMailAddress>info@environmentaldatainitiative.org</electronicMailAddress>
    <onlineUrl>https://environmentaldatainitiative.org</onlineUrl>
    <userId directory="https://ror.org/">https://ror.org/0330j0z60</userId>
    <userId directory="https://grid.ac/institutes/">grid.511300.6</userId>
    <userId directory="https://isni.oclc.org/isni/">0000000495505609</userId>>  
  </publisher>
```
#### Best Practice Considerations ####

EML does not allow to distinguish between a user id and an organization id within one party element. Hence, the recommendation is to use one party element only for an organization with its ROR id and not try to overload the `<userID>` element by entering both the ORCID for a person and the ROR for the person's organization within one party element. 

A ROR ID consists of a unique 9-character string appended to the ROR domain. The preferred form of a ROR identifier is the entire URL: https://ror.org/02mhbdp94 rather than ror.org/02mhbdp94 or 02mhbdp94, although the ROR API will recognize all three of these forms as ROR IDs.


## Action requested: ##
Each site Information Manager should enter information relevant to their ROR identifier in the shared spreadsheet as described below. 


### How to request or update an ROR identifier ###

1. Visit the [ROR Homepage](https://ror.org/) to learn about ROR IDs.
2. Check if your LTER Program has an ROR ID on the [search page](https://ror.org/search).
 
    - If the program does not exist in the ROR directory, or if it contains inaccuracies, request a change through the [ROR update form](https://docs.google.com/forms/d/e/1FAIpQLSdJYaMTCwS7muuTa-B_CnAtCSkKzt19lkirAKG4u7umH9Nosg/viewform).
    - When a site moves institutions or needs to update partners, simply request a change to ROR metadata through the [ROR update form](https://docs.google.com/forms/d/e/1FAIpQLSdJYaMTCwS7muuTa-B_CnAtCSkKzt19lkirAKG4u7umH9Nosg/viewform). The site identifier will remain the same, but parent institution or other metadata will be updated.
