# Conformance class: Application schema, Area Management, Restriction/Regulation Zones and Reporting Units

Conformance class for the requirements associated with the application schema. 

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schemas, Area Management, Restriction/Regulation Zones and Reporting Units".

This conformance class is part of the [INSPIRE Data Specification on Area Management, Restriction/Regulation Zones and Reporting Units](http://inspire.ec.europa.eu/id/ats/data-am/3.0).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

none

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-AM](http://inspire.ec.europa.eu/id/ats/data-am/3.0/am-as/README#ref_TG_DS_AM) | [GML application schemas, Area Management, Restriction/Regulation Zones and Reporting Units](http://inspire.ec.europa.eu/id/ats/data-am/3.0/am-gml) | INSPIRE spatial data set encoded in GML, Area Management, Restriction/Regulation Zones and Reporting Units features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature types in the application schema are:

* ManagementRestrictionOrRegulationZone


*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-AM <a name="ref_TG_DS_AM"></a>   | [INSPIRE Data Specification on Area Management, Restriction/Regulation Zones and Reporting Units – Technical Guidelines version 3.0](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_AM_v3.0.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-AM](#ref_TG_DS_AM)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code list values](http://inspire.ec.europa.eu/id/ats/data-am/3.0/am-as/code-list-values)  | Draft  | A.1.3  |
| [Constraints](http://inspire.ec.europa.eu/id/ats/data-am/3.0/am-as/constraints)  | Draft  | A.1.6  |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
am             | http://inspire.ec.europa.eu/schemas/am/4.02
au             | http://inspire.ec.europa.eu/schemas/au/4.0
net            | http://inspire.ec.europa.eu/schemas/net/4.0
base           | http://inspire.ec.europa.eu/schemas/base/3.3
gml            | http://www.opengis.net/gml/3.2
wfs            | http://www.opengis.net/wfs/2.0
xsi            | http://www.w3.org/2001/XMLSchema-instance
xlink          | http://www.w3.org/1999/xlink
xml            | http://www.w3.org/XML/1998/namespace

