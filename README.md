# Device Provisioning Sample App

This app is a companion for my "Create IoT Solutions" course at Pluralsight. 

`dotnet build`

## Creating a certificate

Execute the following command:

`dotnet run setup`

This will create the certificate, which can then be used to create an individual enrollment.

## Simulate a device

Execute the following command:

`dotnet run {id-scope}`

The `{id-scope}` parameter is the ID Scope of your device provisioning service. 

```
dotnet add package Microsoft.Azure.Devices.Client
dotnet add package Microsoft.Azure.Devices.Provisioning.Client
dotnet add package Microsoft.Azure.Devices.Provisioning.Transport.Amqp

```