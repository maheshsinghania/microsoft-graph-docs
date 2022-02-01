---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
	"@odata.type" = "#microsoft.graph.cloudPcProvisioningPolicy"
	Description = "Description value"
	DisplayName = "Display Name value"
	DomainJoinConfiguration = @{
		DomainJoinType = "hybridAzureADJoin"
		OnPremisesConnectionId = "16ee6c71-fc10-438b-88ac-daa1ccafffff"
	}
	Id = "1d164206-bf41-4fd2-8424-a3192d39ffff"
	ImageDisplayName = "Windows-10 19h1-evd"
	ImageId = "MicrosoftWindowsDesktop_Windows-10_19h1-evd"
	ImageType = "gallery"
	OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff"
}

New-MgDeviceManagementVirtualEndpointProvisioningPolicy -BodyParameter $params

```