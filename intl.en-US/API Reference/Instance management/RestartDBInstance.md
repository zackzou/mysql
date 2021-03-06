# RestartDBInstance {#doc_api_1059304 .reference}

You can call this operation to restart an RDS instance.

**Note:** If a large number of transactions need to be submitted or rolled back, the restart process may take about one more minute.

This operation must meet the following requirements:

-   The instance is in the running state.
-   The instance is not performing a backup task.

## Debugging {#apiExplorer .section}

You can use [OpenAPI Explorer](https://api.aliyun.com/#product=Rds&api=RestartDBInstance) to perform debugging.

OpenAPI Explorer provides various functions to simplify API usage. For example, you can retrieve APIs, call APIs, and generate SDK sample code.

## Request parameters {#parameters .section}

|Parameter|Type|Required|Example|Description|
|---------|----|--------|-------|-----------|
|Action|String|Yes|RestartDBInstance| The operation that you want to perform. Set this parameter to RestartDBInstance.

 |
|DBInstanceId|String|Yes|rm-uf6wjk5xxxxxx| The ID of the instance.

 |
|ClientToken|String|No|ETnLKlblzczshOTUbOCzxxxxxx| The client token that is used to guarantee the idempotency of requests. The client token is generated by the client and is unique among different requests. It is a string of up to 64 ASCII characters.

 |
|AccessKeyId|String|No|LTAIfCxxxxxxx| The AccessKey ID issued by Alibaba Cloud for users to access services.

 |

## Response parameters {#resultMapping .section}

|Parameter|Type|Example|Description|
|---------|----|-------|-----------|
|RequestId|String|65BDA532-28AF-4122-AA39-B382721EEE64| The ID of the request.

 |

## Examples {#demo .section}

Request example

``` {#request_demo}

http(s)://rds.aliyuncs.com/?Action=RestartDBInstance
&DBInstanceId=rm-uf6wjk5xxxxxxxxxx
&<Common request parameters>
```

Normal response examples

`XML` format

``` {#codeblock_676_62e_0u9}
<RestartDBInstanceResponse>
	  <RequestId> 65BDA532-28AF-4122-AA39-B382721EEE64</RequestId></RestartDBInstanceResponse>
```

`JSON` format

``` {#codeblock_k7m_ksf_19q}
{
	"RequestId":" 65BDA532-28AF-4122-AA39-B382721EEE64"
}
```

## Error codes {#section_oi0_rq5_p7v .section}

For a list of error codes, visit the [API Error Center](https://error-center.alibabacloud.com/status/product/Rds).

