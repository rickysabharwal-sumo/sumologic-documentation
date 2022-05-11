---
slug: /send-data/sources/use-json-configure-sources
---

# Use JSON to Configure Sources

Sources can be configured by using UTF-8 encoded JSON files. Installed Collectors can use JSON files to configure its Sources when using [Local Configuration File Management](/docs/send-data/sources/use-json-configure-sources/local-configuration-file-management). You can also configure Sources for Hosted and Installed Collectors with the Collector Management API.

:::important
JSON files need to be UTF-8 encoded following [RFC 8259](https://tools.ietf.org/html/rfc8259).
:::

See the following topics for additional information:

 * Collector Management API
 * [JSON Source Parameters for Hosted Collectors](json-parameters-hosted-sources.md)
 * [JSON Source Parameters for Installed Collectors](json-parameters-installed-sources.md)
 * [View or Download Collector or Source JSON Configuration](local-configuration-file-management/view-download-source-json-configuration.md)

## Defining a Source JSON file

When registering a Collector, you can define a source JSON file using the `sources` or `syncSources` parameter in your
[user.properties](../../installed-collectors/collector-installation-reference/user-properties.md) or [sumo.conf](../../installed-collectors/collector-installation-reference/sumoconf-for-legacy-collectors.md) configuration file. These parameters are used the first time a collector is set up.

| Parameter |  Type |  Description |
|--|--|--|
| sources | String   | Sets the JSON file describing sources to configure on registration. To make changes to collector sources after the Collector has been configured, you can use the Collector Management API or the Sumo web application. |
| syncSources   | String   | Sets the JSON file describing sources to configure on registration, which will be continuously monitored and synchronized with the Collector's configuration. |

For more information on setting the `syncSources` parameter, see [Local Configuration File Management](/docs/send-data/sources/use-json-configure-sources/local-configuration-file-management). 

## Using JSON to configure multiple Sources

You can use JSON to configure multiple sources in either of the following ways:

 * Create a single JSON file with the configuration information for all the sources (sources.json).
 * Create individual JSON files, one for each source, and then combine them in a single folder. You then configure the source folder instead of the individual sources.

:::note
The maximum number of Sources allowed on a Collector is 1,000.
:::

See [Options for specifying sources in local configuration file(s)](/docs/send-data/sources/use-json-configure-sources/local-configuration-file-management) for more information.

## Types of Sources

Each source can have its own unique fields in addition to the generic fields listed in the previous table. The next table lists the valid field types. The sections that follow list the unique parameters for each and the associated JSON examples.

## Log Sources for Installed Collectors

| Field Type | Type Value |
|--|--|
| [Local File Source](json-parameters-installed-sources.md#local-file-source) | LocalFile | 
| [Remote File Source](json-parameters-installed-sources.md#remote-file-source) | RemoteFileV2 | 
| [Local Windows Event Log Source](json-parameters-installed-sources.md#local-windows-event-log-source) | LocalWindowsEventLog | 
| [Remote Windows Event Log Source](json-parameters-installed-sources.md#remote-windows-event-log-source) | RemoteWindowsEventLog | 
| [Local Windows Performance Source](json-parameters-installed-sources.md#local-windows-performance-source) | LocalWindowsPerfMon | 
| [Remote Windows Performance Source](json-parameters-installed-sources.md#remote-windows-performance-source) | RemoteWindowsPerfMon | 
| [Windows Active Directory Source](json-parameters-installed-sources.md#windows-active-directory-source) | ActiveDirectory | 
| [Syslog Source](json-parameters-installed-sources.md#syslog-source)	 | Syslog | 
| [Script Source](json-parameters-installed-sources.md#script-source) | Script | 
| [Docker Log Source](json-parameters-installed-sources.md#docker-log-source) | DockerLog | 
| [Docker Stats Source](json-parameters-installed-sources.md#docker-stats-source) | DockerStats | 

## Metric Sources for Installed Collectors

| Field Type | Type Value |
|--|--|
| [Host Metrics Source](json-parameters-installed-sources.md#host-metrics-source)  | SystemStats |
| [Streaming Metrics Source](json-parameters-installed-sources.md#streaming-metrics-source) | StreamingMetrics |


### Log Sources for Hosted Collectors

| Field Type | Type Value |
|--|--|
| [Akamai SIEM API Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/akamai-siem-api-source.md) | Universal | 
| [Amazon S3 Source](json-parameters-hosted-sources.md#amazon-s3-source) | Polling | 
| [AWS S3 Archive Source](json-parameters-hosted-sources.md#aws-s3-archive-source) | Polling | 
| [AWS CloudFront Source](json-parameters-hosted-sources.md#aws-cloudfront-source) | Polling | 
| [AWS CloudTrail Source](json-parameters-hosted-sources.md#aws-cloudtrail-source) | Polling
| [AWS Elastic Load Balancing Source](json-parameters-hosted-sources.md#aws-elastic-load-balancing-source) | Polling | 
| [AWS Kinesis Firehose for Logs Source](json-parameters-hosted-sources.md#aws-kinesis-firehose-for-logs-source) | HTTP | 
| [AWS S3 Audit Source](json-parameters-hosted-sources.md#aws-s3-audit-source) | Polling | 
| [AWS Metadata (Tag) Source](json-parameters-hosted-sources.md#aws-metadata-tag-source) | Polling | 
| [Azure Event Hubs Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/azure-event-hubs-source.md) | Universal | 
| [Carbon Black Cloud Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/carbon-black-cloud-source.md) | Universal | 
| [Carbon Black Inventory Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/carbon-black-inventory-source.md) | Universal | 
| [Cloud Syslog Source](json-parameters-hosted-sources.md#cloud-syslog-source) | Cloudsyslog | 
| [Cisco AMP Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/cisco-amp-source.md) | Universal | 
| [Crowdstrike FDR Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/crowdstrike-fdr-source.md) | Universal | 
| [CrowdStrike Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/crowdstrike-source.md) | 	Universal | 
| [CSE AWS EC2 Inventory Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/cse-aws-ec-inventory-source.md) | Universal | 
| [Cybereason Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/cybereason-source.md) | Universal | 
| [Duo Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/duo-source.md) | Universal | 
| [Google Cloud Platform Source](json-parameters-hosted-sources.md#google-cloud-platform-source) | HTTP | 
| [HTTP Source](json-parameters-hosted-sources.md#http-source) | HTTP | 
| [Microsoft Graph Security API Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/microsoft-graph-security-api-source.md) | Universal | 
| [Mimecast Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/mimecast-source.md) | Universal | 
| [Netskope Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/netskope-source.md) | Universal | 
| [Okta Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/okta-source.md) | Universal | 
| [Palo Alto Cortex XDR](../sources-hosted-collectors/cloud-to-cloud-integration-framework/palo-alto-cortex-xdr-source.md) | Universal | 
| [Proofpoint On Demand Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/proofpoint-on-demand-source.md) | Universal | 
| [Proofpoint TAP Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/proofpoint-tap-source.md) | Universal | 
| [Salesforce Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/salesforce-source.md) | Universal | 
| [Sophos Central Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/sophos-central-source.md) | Universal | 
| [Tenable Source](../sources-hosted-collectors/cloud-to-cloud-integration-framework/tenable-source.md) | Universal | 

### Metrics sources for hosted collectors

| Field Type | Type Value |
|--|--|
| [AWS CloudWatch Source](json-parameters-hosted-sources.md#aws-cloudwatch-source) | Polling |

## Common parameters for log source types

The following parameters are used for log Sources except for Syslog. Syslog Sources do not support Multiline Detection, which means the common parameters `multilineProcessingEnabled`, `useAutolineMatching` and `manualPrefixRegexp` are not applicable. If you provide these in the configuration they will be ignored.

| Parameter | Type | Required? | Default | Description | Access |
|--|--|--|--|--|--|
| `sourceType` | String | Yes |  | Type the correct type of Source. | not modifiable | 
| `name` | String | Yes |  | Type a desired name of the Source. The name must be unique per Collector. This value is assigned to the [built-in metadata](../../../search/get-started-with-search/search-basics/built-in-metadata.md) field `_source` and can be a maximum of 128 characters. | modifiable | 
| `description` | String | No | null | Type a description of the Source. | modifiable | 
| `fields` | JSON Object | No | null | JSON map of key-value fields (metadata) to apply to the Collector or Source. | modifiable | 
| `hostName` | String | No | null | Type a host name of the Source. This value is assigned to the built-in metadata field `_sourceHost`. The hostname can be a maximum of 128 characters.<br/>Not supported with Windows Local Event Source and Windows Local Performance Source. | modifiable | 
| `category` | String | No | null | Type a category of the source. This value is assigned to the built-in metadata field `_sourceCategory`. See [best practices](../../design-deployment/best-practices-source-categories.md) for details. | modifiable | 

**Timestamp Processing**

| Parameter | Type | Required? | Default | Description | Access |
|--|--|--|--|--|--|
| `automaticDateParsing` | Boolean | No | true | Determines if timestamp information is parsed or not. Type `true` to enable automatic parsing of dates (the default setting); type `false` to disable. If disabled, no timestamp information is parsed at all. | modifiable | 
| `timeZone` | String | No | null | Type the time zone you'd like the source to use in TZ database format. Example:`"America/Los_Angeles"`. See [time zone format](#time-zone-format) for details. | modifiable | 
| `forceTimeZone` | Boolean | No | false | Type `true` to force the Source to use a specific time zone, otherwise type false to use the time zone found in the logs. The default setting is false. | modifiable | 
| `defaultDateFormat` | String | No | null | (Deprecated) The default format for dates used in your logs. For more information about timestamp options, see Timestamps, Time Zones, Time Ranges, and Date Formats.  See the replacement object, `defaultDateFormats`, below. | modifiable | 
| `defaultDateFormats` | Object array | No | null | Define formats for the dates present in your log messages. You can specify a locator regex to identify where timestamps appear in log lines. <br/>The defaultDateFormats object has two elements:<br/>`format` (required)—Specify the date format.<br/>`locator` (optional)—A regular expression that specifies the location of the timestamp in your log lines. For example, `\[time=(.*)\]`<br/>For an example, see Timestamp example, below. For more information about timestamp options, see Timestamps, Time Zones, Time Ranges, and Date Formats | modifiable | 

**Multiline Processing**

| Parameter | Type | Required? | Default | Description | Access |
|--|--|--|--|--|--|
| `multilineProcessingEnabled` | Boolean | No | true | Type true to enable; type false to disable. The default setting is true. Consider setting to false to avoid unnecessary processing if you are collecting single message per line files (for example, Linux system.log). If you're working with multiline messages (for example, log4J or exception stack traces), keep this setting enabled. | modifiable | 
| `useAutolineMatching` | Boolean | No | true | Type true to enable if you'd like message boundaries to be inferred automatically; type false to prevent message boundaries from being automatically inferred (equivalent to the Infer Boundaries option in the UI). The default setting is true. | modifiable | 
| `manualPrefixRegexp` | String | No | null | When using useAutolineMatching=false, type a regular expression that matches the first line of the message to manually create the boundary. Note that any special characters in the regex, such as backslashes or double quotes, must be escaped. For example, this expression:<br/>`^\[\d{4}-\d{2}-\d{2}\s+\d{2}:\d{2}:\d{2}\.\d{3}\].*`<br/>should be escaped like this:<br/>`^\\[\\d{4}-\\d{2}-\\d{2}\\s+\\d{2}:\\d{2}:\\d{2}\\.\\d{3}\\].*`  | 	modifiable  | 

**Processing Rules**

| Parameter | Type | Required? | Default | Description | Access |
|--|--|--|--|--|--|
| `filters` | String | array | 	No | `[ ]` | If you'd like to add a filter to the Source, type the name of the filter (Exclude, Include, Mask, Hash, or Forward. Review the [Rules and Limitations](../../../manage/collection/processing-rules/include-and-exclude-rules.md) for filters and see [Creating processing rules using JSON](#creating-processing-rules-using-json). | modifiable | 

**When collection should begin**

| Parameter | Type | Required? | Default | Description | Access |
|--|--|--|--|--|--|
| `cutoffTimestamp` | Long | No | 0 (collects all data) | Can be specified instead of cutoffRelativeTime to only collect data more recent than this timestamp, specified as milliseconds since epoch (13 digit). You can use this site to convert to epoch time: http://www.epochconverter.com/<br/>Times in the future are supported. For a [Local File Source](../sources-installed-collectors/local-file-source.md), this cutoff applies to the "modified" time of the file, not the time of the individual log lines. For example, if you have a file that contains logs with timestamps spanning an entire week and set the `cutoffTimestamp` to two days ago, all of the logs from the entire week will be ingested since the file itself was modified more recent than the `cutoffTimestamp`. A processing rule could be used to filter logs that match unneeded log messages.<br/>Review timestamp considerations to understand how Sumo interprets and processes timestamps. | modifiable | 
| `cutoffRelativeTime` | String | No |  | Can be specified instead of `cutoffTimestamp` to provide a relative offset with respect to the current time.<br/>`time` can be either months (`M`), weeks (`w`), days (`d`), hours (`h`), or minutes (`m`). Use 0m to indicate the current time.Times in the future are not supported.<br/>Example: use -1h, -1d, or -1w to collect data that's less than one hour, one day, or one week old, respectively.<br/>For a [Local File Source](../sources-installed-collectors/local-file-source.md), this cutoff applies to the "modified" time of the file, not the time of the individual log lines. For example, if you have a file that contains logs with timestamps spanning an entire week and set the cutoffRelativeTime to two days ago, all of the logs from the entire week will be ingested since the file itself was modified more recent than the cutoffRelativeTime. A processing rule could be used to filter logs that match unneeded log messages.<br/>Review timestamp considerations to understand how Sumo interprets and processes timestamps. | not modifiable | 

## Non-configurable parameters

The following parameters are automatically configured by the Sumo Logic Service. Don't include them in the sources JSON file, except for when making API requests. When making an API request you will need to provide the `id`  parameter in the JSON file.

 * id
 * alive - This parameter is updated based on if Sumo receives a heartbeat message every 15 seconds. A heartbeat checks for successful connectivity. If no successful heartbeat message is received after 30 minutes this becomes false.
 * status

## Time zone format

In a JSON source configuration, a string for the `timeZone` setting does not follow the same format as the time zone setting shown in the Sumo Logic Web Application. The JSON `timeZone` property uses the underlying TZ database time zone format instead of (GMT+11:00) style values.

Example:

```
"timeZone": "America/Los_Angeles",
```

You can find a list of time zone environment variables in this [Wikipedia article](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).  

## Timestamp example

The following is a Timestamp example in JSON with two default date formats, `yyyy-MM-dd HH:mm:ss` and `yyMMdd HH:mm:ss:`

```json
{
    "source": {
        "name": "test",
        "defaultDateFormats": [{
            "format": "yyyy-MM-dd HH:mm:ss",
            "locator": "time=(.*),"
        }, {
            "format": "yyMMdd HH:mm:ss"
        }]
    }
}
```

## Creating processing rules using JSON

You can include processing (filtering) rules when using JSON to configure sources. A filter specifies rules about which messages are sent to Sumo Logic.

 * Exclude—Removes messages before ingestion to Sumo Logic. Think of Exclude as a "denylist" filter. For more information, see [Include and Exclude Rules](../../../manage/collection/processing-rules/include-and-exclude-rules.md).
 * Include—Sends only the data you explicitly define to Sumo Logic. Think of Include as an "allowlist" filter. For more information, see [Include and Exclude Rules](../../../manage/collection/processing-rules/include-and-exclude-rules.md).
 * Hash—Replaces a message with a unique, randomly-generated code to protect sensitive or proprietary information, such as credit card numbers or user names. By hashing this type of data you can still track it, even though it's fully hidden. For more information, see [Hash Rules](../../../manage/collection/processing-rules/hash-rules.md).
 * Mask—Replaces an expression with a mask string that you can customize; especially useful for protecting passwords or other data you wouldn't normally track. For more information, see [Mask Rules].
 * Forward—Sends matching log messages to a data forwarding destination. For more information, see [Example: data forwarding rule](#example-data-forwarding-rule) below.

| Parameter | Type | Required? | Description | Access |
|--|--|--|--|--|
| `name` | String | Yes | A name for the rule. | Modifiable | 
`filterType` | Yes | The filter type. Must be one of the following: Exclude, Include, Hash, Mask, or Forward. | Modifiable | 
| `regexp` | String | Yes | A regular expression used to define the filter. If filterType = Mask or Hash, this regular expression must have at least one matching group, specifying the regions to be replaced by a mask or hash.<br/>For multiline messages, add single line modifiers (?s) to the beginning and end of the expression to support matching your string regardless of where it occurs in the message. For example: `(?s).*secur.*(?s)`<br/>Syslog UDP messages may contain a trailing newline character, which will require the above regular expression to properly match your string. | Modifiable | 
| `mask` | String | Yes | when | `filterType = "Mask"` | The mask string used when covering the matching log text. | Modifiable | 
| `transparentForwarding` | Boolean | No | Syslog forwarding by default prepends a timestamp and hostname to messages to ensure they comply with RFC 3164. If your syslog messages already comply, you can disable this feature by specifying this parameter as false. | Modifiable | 

### Example: exclude filter

The following is an example of a filter to exclude messages containing a
specified keyword.

```
"filters":[{
      "filterType":"Exclude",
      "name":"filter_auditd",
      "regexp":".*exe=\"\\/usr\\/sbin\\/crond\".*terminal=cron\\sres=success.*"
    }],
```

When excluding messages based on a string that contains special characters, for example `*("test")*,`you will need to double-escape the special characters so they're valid within the JSON.

Filter name cannot exceed 32 characters.

Example message content to filter:

```
*("test")*
```

Standard Regex (this is the syntax if you create the filter using the UI):

```
\*\("test"\)\*
```

Filter syntax in JSON:

```
\\*\\(\"test\"\\)\\*
```

Filter example in JSON with double-escaped special characters:

```
{
    "source": {
        "name": "test",
        "filters": [{
            "filterType": "Exclude",
            "name": "Filter keyword",
            "regexp": "\\*\\(\"test\"\\)\\*"
        }]
    }
}
```

### Example: mask filter

The following is an example of a filter to mask messages containing an authorization token.

Example message content to filter:

```
auth":"Basic cABC123vZDAwfvDldmlfZ568dWQ6vvhjER4dgyR33lP"
```

Standard Regex, this is the syntax if you create the filter using the UI:

```
auth"\s*:\s*"Basic\s*([^"]+)"
```

Filter syntax in JSON:

```
auth\"\\s*:\\s*\"Basic\\s*([^\"]+)\"
```

Filter example in JSON with double-escaped special characters:

```
"filters":[{
      "filterType":"Mask",
      "name":"masktoken",
      "regexp":"auth\"\\s*:\\s*\"Basic\\s*([^\"]+)\"",
      "mask":"##TOKEN##"
    },
```

### Example: data forwarding rule

In the JSON below for a source, the filters array specifies a data forwarding rule. Before you can configure a data forwarding rule in JSON, you must obtain the **sinkId** for the data forwarding data destination. For instructions, see [Get sinkId for a data forwarding destination](#get-sinkid-for-a-data-forwarding-destination)
below.

```json
{
     "api.version": "v1",
     "sources": [{
          "sourceType": "Syslog",
          "name": "example",
          "port": 514,
          "protocol": "TCP",
          "encoding": "UTF-8",
          "category": "example",
          "useAutolineMatching": false,
          "multilineProcessingEnabled": false,
          "timeZone": "UTC",
          "automaticDateParsing": true,
          "forceTimeZone": false,
          "defaultDateFormat": "dd/MMM/yyyy HH:mm:ss",
          "filters": [{ 
               "filterType": "Forward",
               "name": "example",
               "regexp": "(?s).*(?s)",
               "sinkId": 22,
               "transparentForwarding": false
           }]  
     }]
}
```

## Get sinkId for a data forwarding destination

To determine the sinkId for a data forwarding destination, you use the Sumo web app to create a test data forwarding rule. Sumo updates the JSON configuration for the source with the sinkId of the destination you select. Then you can view the JSON configuration for the source, make a note of the sinkId, and then delete the test processing rule.

These instruction assume you have already created a data forwarding destination.

1. Follow the instructions in [Configure processing rules for data forwarding](../../../manage/data-forwarding/data-forwarding-installed-collectors.md#configure-processing-rules-for-data-forwarding) to add a data forwarding rule to a source on an installed collector. As part of this process, you will select the data forwarding destination to which you want to forward data.
1. To view the JSON configuration for the source you updated in the previous step: 

   1. Select **Manage Data \> Collection \> Collection**. 
   1. Click the icon to the right of the source. The API usage information panel appears. Make a note of the sinkId in the filter section of the JSON. 

    ![sink id](/img/send-data/sinkId.png)

1. Click the icon to the right of the Source. Make a note of the sinkId in the filter section of the JSON.
1. Click Done to close the API usage information panel.
1. Now that you have determined the sinkId for the data forwarding destination, delete the test rule.

   1. Select **Manage Data \> Collection \> Collection**. 
   1. Navigate to the source to which you added the test rule. 
   1. In the **Processing Rules** section of the page, click the delete icon to the right of the test rule. 

    ![proc rule](/img/send-data/proc-rule.png)

Now that you have the sinkId for the data forwarding destination, you can define the filter array in the JSON for your source, following the example in [Example: Data Forwarding Rule](#example-data-forwarding-rule) above.
