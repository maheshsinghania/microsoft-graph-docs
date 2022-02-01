---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
	Subject = "Let's go for lunch"
	Body = @{
		ContentType = "HTML"
		Content = "Does late morning work for you?"
	}
	Start = @{
		DateTime = "2019-06-15T12:00:00"
		TimeZone = "Pacific Standard Time"
	}
	End = @{
		DateTime = "2019-06-15T14:00:00"
		TimeZone = "Pacific Standard Time"
	}
	Location = @{
		DisplayName = "Harry's Bar"
	}
	Attendees = @(
		@{
			EmailAddress = @{
				Address = "adelev@contoso.onmicrosoft.com"
				Name = "Adele Vance"
			}
			Type = "required"
		}
	)
}

New-MgGroupEvent -GroupId $groupId -BodyParameter $params

```