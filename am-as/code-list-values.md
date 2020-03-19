# Code list values

**Version**: 1

**Purpose**: Verify whether all attributes whose value type is a code list take the values set out therein

**Prerequisites**

**Test method**

When an attribute has a code list as its type, verify that the values comply with the definitions and include the values set out in Annex II of the regulation. To pass this tests that any instance of an attribute

* takes only values explicitly specified in the INSPIRE code list register when the code list‘s extensibility is 'none'.

Otherwise report [disallowedCodeListValue](#disallowedCodeListValue).

In the Area Management, Restriction/Regulation Zones and Reporting Units application schema, the following properties have to be tested:
* [EnvironmentalDomain](#EnvironmentalDomain). Valid values:
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/air
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/climateAndClimateChange
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/healthProtection
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/landUse
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/naturalResources
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/natureAndBiodiversity
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/noise
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/soil
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/sustainableDevelopment
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/waste
  * http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/water


The following is not applicable for this application schema as no extensions are allowed. It is still included here as a reminder in case extensions will be allowed in the future:

Inspect the code list valued property elements. If a value is not one of the values listed above, review the code list definition to check that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule and that all extensions conform to the requirements. This is a manual test.
  
**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (1)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (1)l
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (2)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (4)

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
disallowedCodeListValue <a name="disallowedCodeListValue"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that is not one of the allowed values listed at $codelist. 

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
EnvironmentalDomain <a name="EnvironmentalDomain"></a>   | //schema-element(am:ManagementRestrictionOrRegulationZone)/am:environmentalDomain/@href:xlink