# Service Vehicle Specialisation for Farming Simulator 22

 `Farming Simulator  22`   `Revision:  FS22-01`

## Usage
This specialisation is free for use in any Farming Simulator vehicle mod for both ***Private*** and ***Public*** release.

## Publishing
The publishing of this specialisation when not included as part of a vehicle mod is not permitted.

## Modification / Converting
Only GtX | Andy is permitted to make modifications to this code including but not limited to bug fixes, enhancements or the addition of new features.

Converting this specialisation or parts of it to other version of the Farming Simulator series is not permitted without written approval from GtX | Andy.

## Versioning
All versioning is controlled by GtX | Andy and not by any other page, individual or company.

## Mods Using Spec
[🎁 Field Service Trailer](https://www.farming-simulator.com/mod.php?&mod_id=246043&title=fs2022)

> ***Important: The dismantling of this vehicle or the removal of any parts for use on other publicly released mods is strictly prohibited without written approval from GtX | Andy***

## Documentation
Not all features are required. The service script can operate with just a `Vehicle Trigger` and `Player Trigger` as shown below.

>### vehicle.xml

```xml
<vehicle type="myServiceVehicle" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="../../../../shared/xml/schema/vehicle.xsd">
    <service>
        <workshop playerTriggerNode="sellTrigger" vehicleTriggerNode="sellAreaTrigger" />
    </service>
</vehicle>
```
>### modDesc.xml

```xml
<modDesc>
    <specializations>
        <specialization name="serviceVehicle"   className="ServiceVehicle"   filename="scripts/ServiceVehicle.lua"/>
    </specializations>

    <vehicleTypes>
        <type name="myServiceVehicle" parent="baseFillable" className="Vehicle" filename="$dataS/scripts/vehicles/Vehicle.lua">
            <specialization name="serviceVehicle"/>
        </type>
    </vehicleTypes>
</modDesc>
```

## Copyright
Copyright (c) 2018 [GtX (Andy)](https://github.com/GtX-Andy)