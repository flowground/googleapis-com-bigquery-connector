# ![LOGO](logo.png) BigQuery **flow**ground Connector

## Description

A generated **flow**ground connector for the BigQuery API (version v2).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/bigquery/v2/swagger.json<br/>
Generated at: 2019-05-07T17:41:13+03:00

## API Description

A data platform for customers to create, manage, share and query data.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all projects to which you have been granted any project role.

*Tags:* `projects`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of results to return
* `pageToken` - _optional_ - Page token, returned by a previous call, to request the next page of results
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists all datasets in the specified project to which you have been granted the READER dataset role.

*Tags:* `datasets`

#### Input Parameters
* `all` - _optional_ - Whether to list all datasets, including hidden ones
* `filter` - _optional_ - An expression for filtering the results of the request by label. The syntax is "labels.<name>[:<value>]". Multiple filters can be ANDed together by connecting with a space. Example: "labels.department:receiving labels.active". See Filtering datasets using labels for details.
* `maxResults` - _optional_ - The maximum number of results to return
* `pageToken` - _optional_ - Page token, returned by a previous call, to request the next page of results
* `projectId` - _required_ - Project ID of the datasets to be listed
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a new empty dataset.

*Tags:* `datasets`

#### Input Parameters
* `projectId` - _required_ - Project ID of the new dataset
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the dataset specified by the datasetId value. Before you can delete a dataset, you must delete all its tables, either manually or by specifying deleteContents. Immediately after deletion, you can create another dataset with the same name.

*Tags:* `datasets`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of dataset being deleted
* `deleteContents` - _optional_ - If True, delete all the tables in the dataset. If False and the dataset contains tables, the request will fail. Default is False
* `projectId` - _required_ - Project ID of the dataset being deleted
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns the dataset specified by datasetID.

*Tags:* `datasets`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the requested dataset
* `projectId` - _required_ - Project ID of the requested dataset
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates information in an existing dataset. The update method replaces the entire dataset resource, whereas the patch method only replaces fields that are provided in the submitted dataset resource. This method supports patch semantics.

*Tags:* `datasets`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the dataset being updated
* `projectId` - _required_ - Project ID of the dataset being updated
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates information in an existing dataset. The update method replaces the entire dataset resource, whereas the patch method only replaces fields that are provided in the submitted dataset resource.

*Tags:* `datasets`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the dataset being updated
* `projectId` - _required_ - Project ID of the dataset being updated
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists all tables in the specified dataset. Requires the READER dataset role.

*Tags:* `tables`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the tables to list
* `maxResults` - _optional_ - Maximum number of results to return
* `pageToken` - _optional_ - Page token, returned by a previous call, to request the next page of results
* `projectId` - _required_ - Project ID of the tables to list
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a new, empty table in the dataset.

*Tags:* `tables`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the new table
* `projectId` - _required_ - Project ID of the new table
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the table specified by tableId from the dataset. If the table contains data, all the data will be deleted.

*Tags:* `tables`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the table to delete
* `projectId` - _required_ - Project ID of the table to delete
* `tableId` - _required_ - Table ID of the table to delete
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified table resource by table ID. This method does not return the data in the table, it only returns the table resource, which describes the structure of this table.

*Tags:* `tables`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the requested table
* `projectId` - _required_ - Project ID of the requested table
* `selectedFields` - _optional_ - List of fields to return (comma-separated). If unspecified, all fields are returned
* `tableId` - _required_ - Table ID of the requested table
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates information in an existing table. The update method replaces the entire table resource, whereas the patch method only replaces fields that are provided in the submitted table resource. This method supports patch semantics.

*Tags:* `tables`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the table to update
* `projectId` - _required_ - Project ID of the table to update
* `tableId` - _required_ - Table ID of the table to update
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates information in an existing table. The update method replaces the entire table resource, whereas the patch method only replaces fields that are provided in the submitted table resource.

*Tags:* `tables`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the table to update
* `projectId` - _required_ - Project ID of the table to update
* `tableId` - _required_ - Table ID of the table to update
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves table data from a specified set of rows. Requires the READER dataset role.

*Tags:* `tabledata`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the table to read
* `maxResults` - _optional_ - Maximum number of results to return
* `pageToken` - _optional_ - Page token, returned by a previous call, identifying the result set
* `projectId` - _required_ - Project ID of the table to read
* `selectedFields` - _optional_ - List of fields to return (comma-separated). If unspecified, all fields are returned
* `startIndex` - _optional_ - Zero-based index of the starting row to read
* `tableId` - _required_ - Table ID of the table to read

### Streams data into BigQuery one record at a time without needing to run a load job. Requires the WRITER dataset role.

*Tags:* `tabledata`

#### Input Parameters
* `datasetId` - _required_ - Dataset ID of the destination table.
* `projectId` - _required_ - Project ID of the destination table.
* `tableId` - _required_ - Table ID of the destination table.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists all jobs that you started in the specified project. Job information is available for a six month period after creation. The job list is sorted in reverse chronological order, by job creation time. Requires the Can View project role, or the Is Owner project role if you set the allUsers property.

*Tags:* `jobs`

#### Input Parameters
* `allUsers` - _optional_ - Whether to display jobs owned by all users in the project. Default false
* `maxCreationTime` - _optional_ - Max value for job creation time, in milliseconds since the POSIX epoch. If set, only jobs created before or at this timestamp are returned
* `maxResults` - _optional_ - Maximum number of results to return
* `minCreationTime` - _optional_ - Min value for job creation time, in milliseconds since the POSIX epoch. If set, only jobs created after or at this timestamp are returned
* `pageToken` - _optional_ - Page token, returned by a previous call, to request the next page of results
* `projectId` - _required_ - Project ID of the jobs to list
* `projection` - _optional_ - Restrict information returned to a set of selected fields
    Possible values: full, minimal.
* `stateFilter` - _optional_ - Filter for job state

### Starts a new asynchronous job. Requires the Can View project role.

*Tags:* `jobs`

#### Input Parameters
* `projectId` - _required_ - Project ID of the project that will be billed for the job
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns information about a specific job. Job information is available for a six month period after creation. Requires that you're the person who ran the job, or have the Is Owner project role.

*Tags:* `jobs`

#### Input Parameters
* `jobId` - _required_ - [Required] Job ID of the requested job
* `location` - _optional_ - The geographic location of the job. Required except for US and EU. See details at https://cloud.google.com/bigquery/docs/locations#specifying_your_location.
* `projectId` - _required_ - [Required] Project ID of the requested job
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Requests that a job be cancelled. This call will return immediately, and the client will need to poll for the job status to see if the cancel completed successfully. Cancelled jobs may still incur costs.

*Tags:* `jobs`

#### Input Parameters
* `jobId` - _required_ - [Required] Job ID of the job to cancel
* `location` - _optional_ - The geographic location of the job. Required except for US and EU. See details at https://cloud.google.com/bigquery/docs/locations#specifying_your_location.
* `projectId` - _required_ - [Required] Project ID of the job to cancel
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Runs a BigQuery SQL query synchronously and returns query results if the query completes within a specified timeout.

*Tags:* `jobs`

#### Input Parameters
* `projectId` - _required_ - Project ID of the project billed for the query
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves the results of a query job.

*Tags:* `jobs`

#### Input Parameters
* `jobId` - _required_ - [Required] Job ID of the query job
* `location` - _optional_ - The geographic location where the job should run. Required except for US and EU. See details at https://cloud.google.com/bigquery/docs/locations#specifying_your_location.
* `maxResults` - _optional_ - Maximum number of results to read
* `pageToken` - _optional_ - Page token, returned by a previous call, to request the next page of results
* `projectId` - _required_ - [Required] Project ID of the query job
* `startIndex` - _optional_ - Zero-based index of the starting row
* `timeoutMs` - _optional_ - How long to wait for the query to complete, in milliseconds, before returning. Default is 10 seconds. If the timeout passes before the job completes, the 'jobComplete' field in the response will be false

### Returns the email address of the service account for your project used for interactions with Google Cloud KMS.

*Tags:* `projects`

#### Input Parameters
* `projectId` - _required_ - Project ID for which the service account is requested.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-bigquery-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
