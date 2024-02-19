# Device Provisioning Exmaple App
This example code aims at showing a device provisioning use case. The code is constructed on the https://github.com/MattHoneycutt/ps-create-iot-solutions/blob/master/device-provisioning-sample/

Check the dotnet command is executable on your environment, if not install it. 
## Install the  reqired libs
```
dotnet add package Microsoft.Azure.Devices.Client
dotnet add package Microsoft.Azure.Devices.Provisioning.Client
dotnet add package Microsoft.Azure.Devices.Provisioning.Transport.Amqp

```
## Creating a certificate

Execute the following command:

`dotnet run setup`

This will create the certificate, which can then be used to create an individual enrollment.

## Build the code

`dotnet build`

## Simulate a device

Execute the following command:

`dotnet run {id-scope}`

The `{id-scope}` parameter is the ID Scope of your device provisioning service. 

