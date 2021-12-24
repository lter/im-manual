# Creating EML

The [Ecological Metadata Language (EML)](https://eml.ecoinformatics.org/) is an XML schema for describing ecological datasets.
EDI maintains [best practices for EML](https://ediorg.github.io/data-package-best-practices/) that you should review when writing your own EML.

There are many one-off solutions for creating EML at LTER sites. Some common ones are listed below, as well as some newer offerings from EDI.

## LTER Core Metabase

Some LTER sites manage dataset metadata using a Postgres database schema called [Metabase](https://github.com/lter/LTER-core-metabase).
It is maintained by LTER IMs, as is the companion R code called [MetaEgress](https://github.com/BLE-LTER/MetaEgress) for generating EML from Metabase.
The original Metabase was developed at GCE, but the current version (called LTER Core Metabase) is in use at BLE and JRN.

## DEIMS

DEIMS is a Drupal-based solution for LTER websites.  It includes the capability to generate EML.
If you're using DEIMS, then you should probably using it to create EML.
If you're not already using DEIMS, it's not worth installing DEIMS just to write EML.

## EMLassemblyline

[EMLassemblyline](https://github.com/EDIorg/emlAssemblyLine) is an R package for creating EML.
It is maintained by EDI and is used by several LTER sites such as HBR, JRN, NES, and NTL.

## ezEML

[ezEML](https://ezeml.edirepository.org/eml/user_guide) is an online interface for creating EML.
If you're starting from scratch and don't want to write any code or maintain your own metadata database, then this solution is definitely worth checking out.
It's tailored toward scientists who may not have someone on their team skilled in EML (or the technologies used to create EML locally).
