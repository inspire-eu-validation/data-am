# Constraints

**Version**: 1

**Purpose**: Verify that the features provided in the dataset adhere to the constraints specified in the INSPIRE application schema.

**Prerequisites**

**Test method**

Verify that the OCL constraints listed below that are specified in the UML model of the application schema are met, i.e. validate features against the constraints. For unmet constraints report [constraintViolation](#constraintViolation). 

For constraints that require retrieving a referenced resource and the resource cannot be retrieved, report [brokenLink](#brokenLink). The test accepts the following two types of content in @xlink:href attributes: Either a "#" followed by a @gml:id in the same document or a HTTP URI.

Automated tests:

* Specify at least the most specific legal instrument; "At least the most specific legal instrument that required the establishment of zone shall be provided using the [legalBasis](#legalBasis) association role.".

* competentAuthority.role shall be "amthority"; OCL: "inv: competentAuthority.role = RelatedPartyRoleValue::amthority". The role attribute of the [competentAuthority](#competentAuthority) shall take the value “amthority”

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-am/3.2/am-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (2)
* [TG DS-AM](http://inspire.ec.europa.eu/id/ats/data-am/3.2/am-as/README#ref_TG_DS_Am)) 5.4

**Test type**: Automated

**Notes** 


## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
constraintViolation <a name="constraintViolation"/>  |  XML document '$filename', $featureType '$gmlid': The constraint '$constraint' is violated.
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP.

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-am/3.2/am-as/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
legalBasis <a name="legalBasis"></a> 	| 	//schema-element(am:ManagementRestrictionOrRegulationZone)/am:legalBasis
competentAuthority <a name="competentAuthority"></a> 	| 	//schema-element(am:ManagementRestrictionOrRegulationZone)/am:competentAuthority

