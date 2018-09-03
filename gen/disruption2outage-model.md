# 100disruptions.json

## Add Column

## Add Node/Literal

## PyTransforms
#### _gmlpoint_
From column: _location / features / geometry / coordinates_
``` python
return "<gml:Point><gml:pos>"+getValue("coordinates")[12:29]+" "+getValue("coordinates")[31+12:48+12]+"</gml:pos></gml:Point>"
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _begin_ | `urn:default:baseUri:#DateTimeInterval.start` | `Domain.DateTimeInterval1`|
| _cause_ | `urn:default:baseUri:#Outage.cause` | `Operations.Outage1`|
| _city_ | `urn:default:baseUri:#TownDetail.name` | `Common.TownDetail1`|
| _component_ | `urn:default:baseUri:#IdentifiedObject.name` | `Core.Equipment1`|
| _end_ | `urn:default:baseUri:#DateTimeInterval.end` | `Domain.DateTimeInterval1`|
| _expectedEnd_ | `urn:default:baseUri:#DateTimeInterval.end` | `Domain.DateTimeInterval2`|
| _gmlpoint_ | `http://www.opengis.net/ont/geosparql#asGML` | `Point1`|
| _households_ | `urn:default:baseUri:#ServicePointOutageSummary.totalCount` | `Operations.ServicePointOutageSummary1`|
| _id_ | `uri` | `Operations.Outage1`|
| _lastUpdated_ | `urn:default:baseUri:#Document.lastModifiedDateTime` | `Operations.Outage1`|
| _maintenance_ | `urn:default:baseUri:#Outage.isPlanned` | `Operations.Outage1`|
| _message_ | `urn:default:baseUri:#IdentifiedObject.description` | `Operations.Outage1`|
| _organisation_ | `urn:default:baseUri:#IdentifiedObject.name` | `PaymentMetering.ServiceSupplier1`|
| _planned_ | `urn:default:baseUri:#Outage.isPlanned` | `Operations.Outage1`|
| _plannedBegin_ | `urn:default:baseUri:#DateTimeInterval.start` | `Domain.DateTimeInterval2`|
| _plannedEnd_ | `urn:default:baseUri:#DateTimeInterval.end` | `Domain.DateTimeInterval2`|
| _postalCode_ | `urn:default:baseUri:#StreetAddress.postalCode` | `Common.StreetAddress1`|
| _status_ | `urn:default:baseUri:#Status.value` | `Common.Status1`|
| _street_ | `urn:default:baseUri:#StreetDetail.name` | `Common.StreetDetail1`|
| _timestamp_ | `urn:default:baseUri:#Document.createdDateTime` | `Operations.Outage1`|
| _titel_ | `urn:default:baseUri:#Document.title` | `Operations.Outage1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `Common.Location1` | `urn:default:baseUri:#Location.mainAddress` | `Common.StreetAddress1`|
| `Common.Location1` | `urn:default:baseUri:#StreetAddress.townDetail` | `Common.TownDetail1`|
| `Common.StreetAddress1` | `urn:default:baseUri:#StreetAddress.streetDetail` | `Common.StreetDetail1`|
| `Operations.Incident1` | `http://www.purl.org/EnergyAlert/ExtensionOntology#Incident_Location` | `Common.Location1`|
| `Operations.Outage1` | `http://www.opengis.net/ont/geosparql#hasGeometry` | `Point1`|
| `Operations.Outage1` | `urn:default:baseUri:#Document.status` | `Common.Status1`|
| `Operations.Outage1` | `http://www.purl.org/EnergyAlert/ExtensionOntology#Outage_Equipments` | `Core.Equipment1`|
| `Operations.Outage1` | `urn:default:baseUri:#Outage.actualPeriod` | `Domain.DateTimeInterval1`|
| `Operations.Outage1` | `urn:default:baseUri:#Outage.estimatedPeriod` | `Domain.DateTimeInterval2`|
| `Operations.Outage1` | `urn:default:baseUri:#Outage_Incident` | `Operations.Incident1`|
| `Operations.Outage1` | `urn:default:baseUri:#Outage.summary` | `Operations.ServicePointOutageSummary1`|
| `Operations.Outage1` | `http://www.purl.org/EnergyAlert/ExtensionOntology#Outage_ServiceSupplier` | `PaymentMetering.ServiceSupplier1`|
