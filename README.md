# zJSON

## Overview

The JSON Document Class

This is just a clone of the original [zJSON](https://github.com/se38/zJSON).

See [documentation](https://github.com/se38/zJSON/wiki).

Deprecated! see[HowTo: Migrating from zJSON to /ui2/cl_json](https://blogs.sap.com/2023/05/11/howto-migrating-from-zjson-to-ui2-cl_json/).

## Required Packages
None

## Installation

This project is supported by <a href="https://github.com/larshp/abapGit">ABAPGit Project</a>. Download ZIP file or integrate this project to him.

## Changelog

- Changes v2.35 - 2021-04-21
  - Fixed issue #31 (colons in field values)
  
- Changes v2.34 - 2021-01-22
  - New option: mapping names between ABAP and JSON

- Changes v2.33 - 2019-03-29
  - New option: replace double underscores in fieldnames with CamelCase

- Changes v2.32 - 2019-03-16
  - New option: replace underscores in fieldnames with hyphen
  
- Changes v2.31 (2015-05-29)
  - GIT bug #18: Unescape Slash ("/" -> "/")

- Changes v2.30 (2015-05-05)
  - GIT bug #17: APPEND_DATA: malformed JSON

- Changes v2.29 (2015-02-08)
  - GIT enhancement #16: wdr_simple_name_value_list not present on 7.00 systems

]- Changes v2.28 (2015-01-23)
  - GIT enhancement #10: New function: Clear data
  - GIT enhancement #12: Export + Import name/value pairs
  - GIT enhancement #13: Float as type P
  - GIT enhancement #14: Set new version number
  - GIT bug #15: Component name "DATA" breaks CREATE_WITH_DATA

- Changes v0.2.27 (2014-10-31)
  - GIT enhancement #9: Handle Data References

- Changes v0.2.26 (2014-04-30)
  - GIT enhancement #5: Controll the removal of line breaks in method set_json
  - GIT bug #6: Missing unit tests for "boolean"
  - GIT bug #7: NUMC fields are surrounded with quotes again (incompatible change!)
  - GIT enhancement #8: transform_simple with attribute names in lower case

- Changes v0.2.25 (2014-04-02)
  - GIT enhancement #2: handling of boolean values (input)
  - GIT enhancement #4: handling of data reference objects

- Changes v0.2.24 (2014-01-05)
  - GIT enhancement #1: handling of boolean values (output)
  
- Changes v0.2.23 (2013-09-05)
  - changed license (Apache, Version 2.0)

- Changes v0.2.22 (2013-07-13)
  - Solved issue #49: 0.2.21 breaks compatibility with NW 7.01
  - Solved issue #50: Dump in method transform_simple (ABAP -> JSON)

- Changes v0.2.21 (2013-04-18)
  - Enhancement #16: Performance issue with large tables
  - Solved issue #46: Transform Simple: Raise exception cx_xslt_format_error
  - Solved issue #47: GET_DATA: parse is called twice
  - Enhancement #48: Lower case field names in TRANSFORM_SIMPLE
  
- Changes v0.2.20 (2013-04-10)
  - Solved issue #34: Wrong output of binary data in method GET_DATA
  - Solved issue #44: Handling DREF & OREF objects that are initial
  - Enhancement #45: Dref: create data ref in GET_DATA

- Changes v0.2.19 (2013-03-01)
  - Enhancement #41: Catchable errors
  - Solved issue #43: Simple Transformation: check basis release

- Changes v0.2.18 (2013-02-12)
  - Enhancement #40: JSON document class now downward compatible to basis release 7.01

- Changes v0.2.17 (2013-02-01)
  - Enhancement #36: Use new kernel functions to parse JSON (usage: see updated wiki)

- Changes v0.2.16 (2013-01-31)
  - Enhancement #32: Javascript Escape of characters "<" + ">"
  - solved Issue #33: Unescape characters in method GET_DATA
  - Enhancement #38: Issue with datatype P longer than 20 characters
  - Enhancement #39: Support for datatype X

- Changes v0.2.15 (2013-01-12)
  - solved issue #35: Whitespace at start of array causes parse error

- Changes v0.2.14 (2012-10-27)
  - solved issue #28: Endless Loop with wrong JSON format
  - enhancement #29: use of conversion exits (usage: see updated wiki)
  - solved issue #30: Problem with method get_value (-> new method "key_exists()")

- Changes v0.2.13 (2012-10-05)
  - enhancement #25: Namespace Replace Pattern (usage: see unit test "test_namespace")
  - enhancement #26: Special Date format (usage: see unit tests "test_date_format" + "test_date_format_reverse")
  - enhancement #27: High memory consumption in get_json() with large JSON (usage: see updated wiki)

- Changes v0.2.12 (2012-09-19)
  - solved issue #23: Issue when the resulting JSON ends with an object
  - solved issue #22: NUMC with zero value
  - updated unit tests

- Changes v0.2.11 (2012-09-11) do not install, contains mayor issues
  - solved issue #22: Bug at elimination of quotation marks

- Changes v0.2.10 (2012-08-10) do not install, contains mayor issues
  - solved issue #20: error while parsing nested arrays
  - enhancement #21: performance issues with large JSON
  - Unit tests updated (escape characters)

- Changes v0.2.9 (2012-06-20)
  - enhancement #13: suppress "itab"
  - solved issue #17: Problem with numbers with leading zeros
  - solved issue #18: Problem with value array (unstructured table)
  - enhancement #19: Unit Tests

- Changes v0.2.8 (2012-03-22)
  - solved issue #12 json->dumps(): problems with mixed objects/arrays

- Changes v0.2.7 (2012-03-08)
  - solved issue #10 json->dumps(): Shortdump if a value is empty
  - solved issue #11 Escaping single quote leads to inconsistent JSON

- Changes v0.2.6 (2012-02-28)
  - solved issue #8 bugfix: get_data(): malformatted TIMS field
  - solved issue #9 enhancement: json->dumps()

- Changes v0.2.5 (2012-02-10)
  - solved issue #6 bugfix: Wrong response of get_data()
  - solved issue #7 bugfix: get_json(): don't add "missing" braces, if it's a collection

- Changes v0.2.4 (2012-02-08)
  - solved issue #5 bugfix for CamelCase key fields

- Changes v0.2.3 (2011-12-15)
  - solved issue #2 (enhancement): new method "get_data"
  - solved issue #3: Only add braces {} in get_json() if it's really an object
  - solved issue #4: Escape non-printable/special characters

- Changes v0.2.2 (2011-10-03)
  - solved issue #1: CX_SY_RANGE_OUT_OF_BOUNDS exception when SET_JSON is called without a value

- Changes v0.2.1 (2011-08-31)
  - new public method APPEND_DATA
  - XSTRING and DataRefs as possible data types
  - minor changes

- Changes v0.2.0 (2010-11-28)
  - first public release of JSON document class