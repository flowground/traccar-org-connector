# ![LOGO](logo.png) traccar **flow**ground Connector

## Description

A generated **flow**ground connector for the traccar API (version 4.3).

Generated from: https://api.apis.guru/v2/specs/traccar.org/4.3/swagger.json<br/>
Generated at: 2019-05-07T17:44:25+03:00

## API Description

Open Source GPS Tracking Platform

## Authorization

Supported authorization schemes:
- Basic Authentication

## Actions

### Fetch a list of Attributes

> Without params, it returns a list of Attributes the user has access to

#### Input Parameters
* `all` - _optional_ - Can only be used by admins or managers to fetch all entities
* `userId` - _optional_ - Standard users can use this only with their own _userId_
* `deviceId` - _optional_ - Standard users can use this only with _deviceId_s, they have access to
* `groupId` - _optional_ - Standard users can use this only with _groupId_s, they have access to
* `refresh` - _optional_

### Create an Attribute

### Delete an Attribute

#### Input Parameters
* `id` - _required_

### Update an Attribute

#### Input Parameters
* `id` - _required_

### Fetch a list of Calendars

> Without params, it returns a list of Calendars the user has access to

#### Input Parameters
* `all` - _optional_ - Can only be used by admins or managers to fetch all entities
* `userId` - _optional_ - Standard users can use this only with their own _userId_

### Create a Calendar

### Delete a Calendar

#### Input Parameters
* `id` - _required_

### Update a Calendar

#### Input Parameters
* `id` - _required_

### Fetch a list of Saved Commands

> Without params, it returns a list of Drivers the user has access to

#### Input Parameters
* `all` - _optional_ - Can only be used by admins or managers to fetch all entities
* `userId` - _optional_ - Standard users can use this only with their own _userId_
* `deviceId` - _optional_ - Standard users can use this only with _deviceId_s, they have access to
* `groupId` - _optional_ - Standard users can use this only with _groupId_s, they have access to
* `refresh` - _optional_

### Create a Saved Command

### Fetch a list of Saved Commands supported by Device at the moment

> Return a list of saved commands linked to Device and its groups, filtered by current Device protocol support

#### Input Parameters
* `deviceId` - _optional_ - Standard users can use this only with _deviceId_s, they have access to

### Dispatch commands to device

> Dispatch a new command or Saved Command if _body.id_ set

### Fetch a list of available Commands for the Device or all possible Commands if Device ommited

#### Input Parameters
* `deviceId` - _optional_
* `textChannel` - _optional_

### Delete a Saved Command

#### Input Parameters
* `id` - _required_

### Update a Saved Command

#### Input Parameters
* `id` - _required_

### Fetch a list of Devices

> Without any params, returns a list of the user's devices

#### Input Parameters
* `all` - _optional_ - Can only be used by admins or managers to fetch all entities
* `userId` - _optional_ - Standard users can use this only with their own _userId_
* `id` - _optional_ - To fetch one or more devices. Multiple params can be passed like `id=31&id=42`
* `uniqueId` - _optional_ - To fetch one or more devices. Multiple params can be passed like `uniqueId=333331&uniqieId=44442`

### Create a Device

### Delete a Device

#### Input Parameters
* `id` - _required_

### Update a Device

#### Input Parameters
* `id` - _required_

### Update total distance and hours of the Device

#### Input Parameters
* `id` - _required_

### Fetch a list of Drivers

> Without params, it returns a list of Drivers the user has access to

#### Input Parameters
* `all` - _optional_ - Can only be used by admins or managers to fetch all entities
* `userId` - _optional_ - Standard users can use this only with their own _userId_
* `deviceId` - _optional_ - Standard users can use this only with _deviceId_s, they have access to
* `groupId` - _optional_ - Standard users can use this only with _groupId_s, they have access to
* `refresh` - _optional_

### Create a Driver

### Delete a Driver

#### Input Parameters
* `id` - _required_

### Update a Driver

#### Input Parameters
* `id` - _required_

### get_events__id_

#### Input Parameters
* `id` - _required_

### Fetch a list of Geofences

> Without params, it returns a list of Geofences the user has access to

#### Input Parameters
* `all` - _optional_ - Can only be used by admins or managers to fetch all entities
* `userId` - _optional_ - Standard users can use this only with their own _userId_
* `deviceId` - _optional_ - Standard users can use this only with _deviceId_s, they have access to
* `groupId` - _optional_ - Standard users can use this only with _groupId_s, they have access to
* `refresh` - _optional_

### Create a Geofence

### Delete a Geofence

#### Input Parameters
* `id` - _required_

### Update a Geofence

#### Input Parameters
* `id` - _required_

### Fetch a list of Groups

> Without any params, returns a list of the Groups the user belongs to

#### Input Parameters
* `all` - _optional_ - Can only be used by admins or managers to fetch all entities
* `userId` - _optional_ - Standard users can use this only with their own _userId_

### Create a Group

### Delete a Group

#### Input Parameters
* `id` - _required_

### Update a Group

#### Input Parameters
* `id` - _required_

### Fetch a list of Maintenance

> Without params, it returns a list of Maintenance the user has access to

#### Input Parameters
* `all` - _optional_ - Can only be used by admins or managers to fetch all entities
* `userId` - _optional_ - Standard users can use this only with their own _userId_
* `deviceId` - _optional_ - Standard users can use this only with _deviceId_s, they have access to
* `groupId` - _optional_ - Standard users can use this only with _groupId_s, they have access to
* `refresh` - _optional_

### Create a Maintenance

### Delete a Maintenance

#### Input Parameters
* `id` - _required_

### Update a Maintenance

#### Input Parameters
* `id` - _required_

### Fetch a list of Notifications

> Without params, it returns a list of Notifications the user has access to

#### Input Parameters
* `all` - _optional_ - Can only be used by admins or managers to fetch all entities
* `userId` - _optional_ - Standard users can use this only with their own _userId_
* `deviceId` - _optional_ - Standard users can use this only with _deviceId_s, they have access to
* `groupId` - _optional_ - Standard users can use this only with _groupId_s, they have access to
* `refresh` - _optional_

### Create a Notification

### Send test notification to current user via Email and SMS

### Fetch a list of available Notification types

### Delete a Notification

#### Input Parameters
* `id` - _required_

### Update a Notification

#### Input Parameters
* `id` - _required_

### Unlink an Object from another Object

### Link an Object to another Object

### Fetches a list of Positions

> Without any params, it returns a list of last known positions for all the user's Devices. _from_ and _to_ fields are not required with _id_

#### Input Parameters
* `deviceId` - _optional_ - _deviceId_ is optional, but requires the _from_ and _to_ parameters when used
* `from` - _optional_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`
* `to` - _optional_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`
* `id` - _optional_ - To fetch one or more positions. Multiple params can be passed like `id=31&id=42`

### Fetch a list of Events within the time period for the Devices or Groups

> At least one _deviceId_ or one _groupId_ must be passed

#### Input Parameters
* `deviceId` - _optional_
* `groupId` - _optional_
* `type` - _optional_ - % can be used to return events of all types
* `from` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`
* `to` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`

### Fetch a list of Positions within the time period for the Devices or Groups

> At least one _deviceId_ or one _groupId_ must be passed

#### Input Parameters
* `deviceId` - _optional_
* `groupId` - _optional_
* `from` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`
* `to` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`

### Fetch a list of ReportStops within the time period for the Devices or Groups

> At least one _deviceId_ or one _groupId_ must be passed

#### Input Parameters
* `deviceId` - _optional_
* `groupId` - _optional_
* `from` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`
* `to` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`

### Fetch a list of ReportSummary within the time period for the Devices or Groups

> At least one _deviceId_ or one _groupId_ must be passed

#### Input Parameters
* `deviceId` - _optional_
* `groupId` - _optional_
* `from` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`
* `to` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`

### Fetch a list of ReportTrips within the time period for the Devices or Groups

> At least one _deviceId_ or one _groupId_ must be passed

#### Input Parameters
* `deviceId` - _optional_
* `groupId` - _optional_
* `from` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`
* `to` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`

### Fetch Server information

### Update Server information

### Close the Session

### Fetch Session information

#### Input Parameters
* `token` - _optional_

### Create a new Session

### Fetch server Statistics

#### Input Parameters
* `from` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`
* `to` - _required_ - in IS0 8601 format. eg. `1963-11-22T18:30:00Z`

### Fetch a list of Users

#### Input Parameters
* `userId` - _optional_ - Can only be used by admin or manager users

### Create a User

### Delete a User

#### Input Parameters
* `id` - _required_

### Update a User

#### Input Parameters
* `id` - _required_

## License

**flow**ground :- Telekom iPaaS / traccar-org-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
