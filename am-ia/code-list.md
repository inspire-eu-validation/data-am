# Code lists

**Purpose**: Verify that code lists extensions can be accessed.

**Prerequisites**

**Test method**

* Verify that any code list extensions are publicly accessible via HTTP, i.e. inspect extensible code list valued property elements. If a reference (@xlink:href) has a value that does not start with http://inspire.ec.europa.eu/codelist/, verify that a HTTP GET request to the URI retrieves a document. Otherwise report [brokenLink](#brokenLink).

This data theme currently has the following extensible code list:

* [ZoneTypeCode](#ZoneTypeCode) : https://inspire.ec.europa.eu/codelist/ZoneTypeCode

This data theme currently has the following empty code list:

* [SpecialisedZoneTypeCode](#SpecialisedZoneTypeCode) : https://inspire.ec.europa.eu/codelist/SpecialisedZoneTypeCode

**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (3)

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP. Every code list value must be made available in an online registry. 

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression				|Multiplicity       |Voidable
---------------------------------------------------------- | -------------------------------|-------------------|---------
ZoneTypeCode <a name ="ZoneTypeCode"></a>	| //schema-element(am:ManagementRestrictionOrRegulationZone)/am:zoneType/@xlink:href | 1..\* | No
SpecialisedZoneTypeCode <a name ="SpecialisedZoneTypeCode"></a>	| //schema-element(am:ManagementRestrictionOrRegulationZone)/am:specialisedZoneType/@xlink:href | 0..1 | Yes
