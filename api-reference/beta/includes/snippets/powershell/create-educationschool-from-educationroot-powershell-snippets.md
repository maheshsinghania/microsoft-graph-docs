---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Education

$params = @{
	DisplayName = "Fabrikam High School"
	Description = "Magnate school for the arts. Los Angeles School District"
	ExternalSource = "String"
	PrincipalEmail = "AmyR@fabrikam.com"
	PrincipalName = "Amy Roebuck"
	ExternalPrincipalId = "14007"
	HighestGrade = "12"
	LowestGrade = "9"
	SchoolNumber = "10002"
	Address = @{
		City = "Los Angeles"
		CountryOrRegion = "United States"
		PostalCode = "98055"
		State = "CA"
		Street = "12345 Main St."
	}
	ExternalId = "10002"
	Phone = "+1 (253) 555-0102"
}

New-MgEducationSchool -BodyParameter $params

```