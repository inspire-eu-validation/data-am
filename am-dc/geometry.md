# Boundary

**Version**: 1

**Purpose**: Verify whether in all cases, where the geometry of a spatial object is derived from another spatial object, the geometries of the two objects are consistent.

**Prerequisites**

**Test method**

For all objects in an AM data set, whose [geometry](#geometry) has been derived from another spatial object, compare the geometries of the two objects. The test is passed when the geometries are consistent.

Inspect that the [geometry](#geometry) of each instance [administrative boundary](#AdministrativeBoundary) correspond to an edge in the topological structure formed by the complete boundary graph, including the boundaries of all levels.

**Reference(s)**: 

* [TG DS-AM](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-dc/README#ref_TG_DS_am) IR requirement Section 4.4 (5)

**Test type**: manual

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-am/3.1/am-dc/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
ManagementRestrictionOrRegulationZone <a name="ManagementRestrictionOrRegulationZone"></a>   | //schema-element(am:ManagementRestrictionOrRegulationZone)
geometry <a name="geometry"></a>  | $ManagementRestrictionOrRegulationZone/*:geometry
