# Basic test

**Version**: 1

**Purpose**: Verify that the spatial data set contains at least one Area Management, Restriction/Regulation Zones and Reporting Units feature.

**Prerequisites**

**Test method**

* Check that the set of [features](#features) in the spatial data set is not empty. Otherwise report [noFeature](#noFeature)

**Reference(s)**: 

* [TG DS-AM](./README.md#ref_TG_DS_AM) 5.4, 5.5

**Test type**: Automated

**Notes**

There is no requirement that we could reference in the Technical Guidelines. Maybe such a requirement should be added in the future revision?

## Messages

Identifier  |  Message text (parAMeters start with '$')
----------- | -------------------------------------------------------------------------
noFeature <a nAMe="noFeature"/>  |  	The XML documents representing the spatial data set do not contain a feature of any of the spatial object types in the 'Area Management, Restriction/Regulation Zones and Reporting Units - Area Management, Restriction/Regulation Zones and Reporting Units' or 'Area Management, Restriction/Regulation Zones and Reporting Units - Maritime Units' application schemas. Therefore, the spatial data set cannot conform to this conformance class. If you have expected to find spatial objects from the application schema in the data set, please consult the statistics information to see the spatial object types that have been found.

## Contextual XPath references

The nAMespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-gml/README#nAMespaces).

Abbreviation                                          |  XPath expression
----------------------------------------------------- | ------------------------------------------------------------------
features <a name="features"></a>   |  //schema-element(am:ManagementRestrictionOrRegulationZone) \|
