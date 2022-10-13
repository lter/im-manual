# Creating EML

The [Ecological Metadata Language (EML)](https://eml.ecoinformatics.org/) is an XML schema for describing ecological datasets.
EDI maintains [best practices for EML](https://ediorg.github.io/data-package-best-practices/) that you should review when writing your own EML.

There are many one-off solutions for creating EML at LTER sites. Some common ones are listed below, as well as some newer offerings from EDI.

## ezEML

[ezEML](https://ezeml.edirepository.org) is an online form based EML editor.
ezEML has developed into a very simple approach for generating metadata files at three levels:

* If you're starting from scratch or don't have much experience with metadata.
* If you need to gather metadata from a researcher or student at your site, you can let them start from a template that you have created.
* Set ezEML up for your site's metadata management: 
  + Import EML snippets from other files. This option lets you set up something akin to a metadata database from which to import parts needed for a new EML file. 
  + Import datapackages (EML and data) from the EDI repository for updates and new versions.
  
Extensive documentation may be found in the [user guide](https://ezeml.edirepository.org/eml/user_guide) or on [YouTube](https://www.youtube.com/playlist?list=PLi1PZkcSXdAKTtpgyHnd8GjtL6kRMMGFR).


## LTER Core Metabase

Some LTER sites manage dataset metadata using a Postgres database schema called [Metabase](https://github.com/lter/LTER-core-metabase).
It is maintained by LTER IMs, as is the companion R code called [MetaEgress](https://github.com/BLE-LTER/MetaEgress) for generating EML from Metabase.
The original Metabase was developed at GCE, but the current version (called LTER Core Metabase) is in use at BLE and JRN.


## EMLassemblyline

[EMLassemblyline](https://ediorg.github.io/EMLassemblyline/) is an R package for creating EML.
It is maintained by EDI and is used by several LTER sites such as HBR, JRN, NES, and NTL.


## DEIMS

DEIMS used to be a [Drupal](https://www.drupal.org/)-based solution for LTER websites. Drupal is a flexible content management system / programming environment that supports metadata based LTER websites well due to its database backend. It can also be used to generate EML. Recent efforts of upgrading from the original DEIMS to Drupal 8/9 are well documented in this [git repository](https://github.com/lter/Deims7-8-Migration) and modules for extracting and ingesting metadata have been developed.
