# ![LOGO](logo.png) SqlManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the SqlManagementClient API (version 2017-03-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/sql-longTermRetention/2017-03-01-preview/swagger.json<br/>
Generated at: 2019-06-11T18:14:23+03:00

## API Description

The Azure SQL Database management API provides a RESTful set of web APIs that interact with Azure SQL Database services to manage your databases. The API enables users to create, retrieve, update, and delete databases, servers, and other entities.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists the long term retention backups for a given location.

*Tags:* `LongTermRetentionBackups`

#### Input Parameters
* `locationName` - _required_ - The location of the database
* `onlyLatestPerDatabase` - _optional_ - Whether or not to only get the latest backup for each database.
* `databaseState` - _optional_ - Whether to query against just live databases, just deleted databases, or all databases.
    Possible values: All, Live, Deleted.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `api-version` - _required_ - The API version to use for the request.

### Lists the long term retention backups for a given server.

*Tags:* `LongTermRetentionBackups`

#### Input Parameters
* `locationName` - _required_ - The location of the database
* `longTermRetentionServerName` - _required_ - The name of the server
* `onlyLatestPerDatabase` - _optional_ - Whether or not to only get the latest backup for each database.
* `databaseState` - _optional_ - Whether to query against just live databases, just deleted databases, or all databases.
    Possible values: All, Live, Deleted.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `api-version` - _required_ - The API version to use for the request.

### Lists all long term retention backups for a database.

*Tags:* `LongTermRetentionBackups`

#### Input Parameters
* `locationName` - _required_ - The location of the database
* `longTermRetentionServerName` - _required_ - The name of the server
* `longTermRetentionDatabaseName` - _required_ - The name of the database
* `onlyLatestPerDatabase` - _optional_ - Whether or not to only get the latest backup for each database.
* `databaseState` - _optional_ - Whether to query against just live databases, just deleted databases, or all databases.
    Possible values: All, Live, Deleted.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `api-version` - _required_ - The API version to use for the request.

### Deletes a long term retention backup.

*Tags:* `LongTermRetentionBackups`

#### Input Parameters
* `locationName` - _required_ - The location of the database
* `longTermRetentionServerName` - _required_ - The name of the server
* `longTermRetentionDatabaseName` - _required_ - The name of the database
* `backupName` - _required_ - The backup name.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `api-version` - _required_ - The API version to use for the request.

### Gets a long term retention backup.

*Tags:* `LongTermRetentionBackups`

#### Input Parameters
* `locationName` - _required_ - The location of the database.
* `longTermRetentionServerName` - _required_ - The name of the server
* `longTermRetentionDatabaseName` - _required_ - The name of the database
* `backupName` - _required_ - The backup name.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `api-version` - _required_ - The API version to use for the request.

### Gets a database's long term retention policy.

*Tags:* `BackupLongTermRetentionPolicies`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `serverName` - _required_ - The name of the server.
* `databaseName` - _required_ - The name of the database.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `api-version` - _required_ - The API version to use for the request.

### Gets a database's long term retention policy.

*Tags:* `BackupLongTermRetentionPolicies`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `serverName` - _required_ - The name of the server.
* `databaseName` - _required_ - The name of the database.
* `policyName` - _required_ - The policy name. Should always be Default.
    Possible values: default.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `api-version` - _required_ - The API version to use for the request.

### Sets a database's long term retention policy.

*Tags:* `BackupLongTermRetentionPolicies`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `serverName` - _required_ - The name of the server.
* `databaseName` - _required_ - The name of the database.
* `policyName` - _required_ - The policy name. Should always be Default.
    Possible values: default.
* `subscriptionId` - _required_ - The subscription ID that identifies an Azure subscription.
* `api-version` - _required_ - The API version to use for the request.

## License

**flow**ground :- Telekom iPaaS / azure-com-sql-long-term-retention-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
