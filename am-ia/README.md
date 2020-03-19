# Conformance class: Information accessibility, Area Management, Restriction/Regulation Zones and Reporting Units (DRAFT)

Conformance class for the requirements related to the accessibility of referenced information, for example, information stored in registries (code lists, coordinate reference systems).

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schemas, Area Management, Restriction/Regulation Zones and Reporting Units".

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification on Area Management, Restriction/Regulation Zones and Reporting Units](http://inspire.ec.europa.eu/id/ats/data-am/3.1).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the data set, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-ia/README#ref_TG_DS_tmpl) | [Information accessibility](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/information-accessibility) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-AM](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-ia/README#ref_TG_DS_HY) | [GML application schemas, Area Management, Restriction/Regulation Zones and Reporting Units](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-gml) | INSPIRE spatial data set encoded in GML, Area Management, Restriction/Regulation Zones and Reporting Units features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature type is:

ManagementRestrictionOrRegulationZone

*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-AM <a name="ref_TG_DS_AM"></a>   | [INSPIRE Data Specification on Area Management, Restriction/Regulation Zones and Reporting Units – Technical Guidelines version 3.1](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_AM_v3.0.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-AM](#ref_TG_DS_AM)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code lists](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-ia/code-list)  | ready for review  | A.6.1 |
| [Feature references](http://inspire.ec.europa.eu/id/ats/data-hy/3.1/am-ia/features)  | ready for review  | A.1.4 |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
gml            | http://www.opengis.net/gml/3.2
am          | http://inspire.ec.europa.eu/schemas/am/4.0

The following variables are used to refer to the corresponding Xpath expressions in all test descriptions:

Variable       | Value
-------------- | -------------------------------------------------
$features      |  //schema-element(am:ManagementRestrictionOrRegulationZone) \|
