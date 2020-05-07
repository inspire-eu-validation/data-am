# Code list values

**Purpose**: Verify whether all attributes whose value type is a code list take the values set out therein

**Prerequisites**

**Test method**

* Check that all the [EnvironmentalDomain](#EnvironmentalDomain) elements has a xlink:href attribute pointing to a [valid value](#validValue). If the check fails report [disallowedCodeListValue](#disallowedCodeListValue).


| <a name="validValue"></a> Valid values for xlink:href attribute of [EnvironmentalDomain](#EnvironmentalDomain) element | 
| ---- | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/air | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/climateAndClimateChange | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/healthProtection | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/landUse | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/naturalResources | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/natureAndBiodiversity | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/noise | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/soil | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/sustainableDevelopment | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/waste | 
| http://inspire.ec.europa.eu/codelist/EnvironmentalDomain/water | 

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (1)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (1)l
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (2)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (4)

**Test type**: Automated

**Notes**

The multiplicity of [EnvironmentalDomain](#EnvironmentalDomain) is 1 or more.

The following is not applicable for this application schema as no extensions are allowed. It is still included here as a reminder in case extensions will be allowed in the future:

Inspect the code list valued property elements. If a value is not one of the values listed above, review the code list definition to check that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule and that all extensions conform to the requirements. This is a manual test.

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
disallowedCodeListValue <a name="disallowedCodeListValue"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that is not one of the allowed values listed at $codelist. 

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-as/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
EnvironmentalDomain <a name="EnvironmentalDomain"></a>   | //schema-element(am:ManagementRestrictionOrRegulationZone)/am:environmentalDomain
