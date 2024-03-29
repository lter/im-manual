## Entry types and required fields for LTER bibliography entries

NSF uses a fairly narrow set of entry types for annual report and public access repository reporting. In general, it makes sense to align the LTER publication database with those types, but we are allowing a few additional types to accommodate technical reports, gray literature, and a miscellaneous type to accommodate awkward and unanticipated modes of publication, such as maps and software packages. The required fields for each entry type are the same as NSF’s and are listed below the entry type.

* article - An article from a journal or magazine. 
   * Required fields: author, title, journal, year
   * Optional fields: volume, number, pages, month, note
* book - A book with an explicit publisher
   * Required fields: author or editor, title, publisher, year
   * Optional fields: volume or number, series, address, edition, month, note
* booklet- A work that is printed and bound, but without a named publisher or sponsoring institution.
   * Required field: title
   * Optional fields: author, howpublished, address, month, year, note
* inbook - A part of a book, which may be a chapter (or section or whatever) and/or a range of pages.
   * Required fields: author or editor, title, chapter and/or pages, publisher, year
   * Optional fields: volume or number, series, type, address, edition, month, note
* incollection - A part of a book having its own title
   * Required fields: author, title, booktitle, publisher, year
   * Optional fields: editor, volume or number, series, type, chapter, pages, address, edition, month, note
* mastersthesis or phdthesis - master's or doctoral thesis
   * Required fields: author, title, school, year, type (masters, doctoral)
   * Optional fields: address, month, note
* proceedings - The proceedings of a conference
   * Required fields: title, year
   * Optional fields: editor, volume or number, series, address, month, organization, publisher, note
* inproceedings - An article in a conference proceedings
   * Required fields: author, title, booktitle, year
   * Optional fields: editor, volume or number, series, pages, address, month, organization, publisher, note

### Additional standard BibTex entry types that are acceptable for the LTER Network bibliography

* techreport - A report published by a school or other institution, usually numbered within a series (also appropriate for government reports and gray literature)
   * Required fields: author, title, institution/organization, year
   * Optional fields: type, number, address, month, note
* manual - Technical documentation
   * Required field: title
   * Optional fields: author, organization, address, edition, month, year, note
* misc - Use this type when nothing else fits. (Appropriate for maps, patents, software, etc. Please strive to include as much detail as possible, especially year and howpublished)
   * Required fields: none.
   * Optional fields: author, title, howpublished, month, year, note.

### Sources:
[Bibtex entry definitions and required fields](https://www.openoffice.org/bibliographic/bibtex-defs.html)

[NSF reporting entry types](https://www.research.gov/common/robohelp/public/WebHelp/Project_Reports.htm#project_reports_htm_how_to_add_p_2803)
