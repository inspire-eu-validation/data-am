# Constraints

**Purpose**: Verify that the features provided in the dataset adhere to the constraints specified in the INSPIRE application schema.

**Prerequisites**

**Test method**

The following checks are performed for every feature in the dataset.

* Check that at least one [legalBasis](#legalBasis) is provided.

* Check that at least one [legalBasis](#legalBasis) with xlink:href attribute or [LegislationCitation](#legislationCitation) child element is provided.

* Check manually that "At least the most specific legal instrument that required the establishment of zone is provided using the [legalBasis](#legalBasis) association role.".

* Check that at least one [competentAuthority](#competentAuthority) is provided.

* Check that at least one [role](#role) is provided.

* Check that at least one [role](#role) has an attribute xlink:href with value 'http://inspire.ec.europa.eu/codelist/RelatedPartyRoleValue/authority'.

**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (2)
* [TG DS-AM](./README.md#ref_TG_DS_Am) 5.4

**Test type**: Automated

**Notes** 

The multiplicity of [legalBasis](#legalBasis) is 1 or more.

The multiplicity of [competentAuthority](#competentAuthority) is 1 or more.

Verify that the OCL constraints that are specified in the UML model of the application schema are met, i.e. validate features against the constraints. For unmet constraints report [constraintViolation](#constraintViolation).

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
constraintViolation <a name="constraintViolation"/>  |  XML document '$filename', $featureType '$gmlid': The constraint '$constraint' is violated.

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
legalBasis <a name="legalBasis"></a> 	| 	//schema-element(am:ManagementRestrictionOrRegulationZone)/am:legalBasis
LegislationCitation <a name="LegislationCitation"></a> 	| 	//schema-element(am:ManagementRestrictionOrRegulationZone)/am:legalBasis/base2:LegislationCitation
competentAuthority <a name="competentAuthority"></a> 	| 	//schema-element(am:ManagementRestrictionOrRegulationZone)/am:competentAuthority
role <a name="role"></a> 	| 	//schema-element(am:ManagementRestrictionOrRegulationZone)/am:competentAuthority/base2:RelatedParty/base2:role
