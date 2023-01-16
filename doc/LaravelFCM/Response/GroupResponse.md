# LaravelFCM\Response\GroupResponse | Laravel / Lumen package for Firebase Cloud Messaging    

## [Laravel / Lumen package for Firebase Cloud Messaging](../../index.md)

- [Classes](../../classes.md)
- [Namespaces](../../namespaces.md)
- [Interfaces](../../interfaces.md)
- [Traits](../../traits.md)
- [Index](../../doc-index.md)
- [Search](../../search.md)

>class

>    [LaravelFCM](../../LaravelFCM.md)` / `[Response](../../LaravelFCM/Response.md)` / `(GroupResponse)
## GroupResponse

class **GroupResponse**        extends [<abbr title="LaravelFCM\Response\BaseResponse">BaseResponse</abbr>](../../LaravelFCM/Response/BaseResponse.md)        implements
        [<abbr title="LaravelFCM\Response\GroupResponseContract">GroupResponseContract</abbr>](../../LaravelFCM/Response/GroupResponseContract.md) [View source](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/GroupResponse.php)






### Constants

|   |   |
|---|---|
|SUCCESS||
|FAILURE||
|ERROR||
|MESSAGE_ID||
|FAILED_REGISTRATION_IDS||

### Properties

|   |   |   |   |
|---|---|---|---|
|<a name="property_logEnabled"></a>protected bool|$logEnabled||<small>from&nbsp;[../../LaravelFCM/Response/BaseResponse.md#property_logEnabled](<abbr title="LaravelFCM\Response\BaseResponse">BaseResponse</abbr>)</small>|
|<a name="property_logger"></a>protected <abbr title="Monolog\Logger">Logger</abbr>|$logger|The logger.|<small>from&nbsp;[../../LaravelFCM/Response/BaseResponse.md#property_logger](<abbr title="LaravelFCM\Response\BaseResponse">BaseResponse</abbr>)</small>|
|<a name="property_retryAfter"></a> int|string|null|$retryAfter|The value of the first Retry-After header in the response.|<small>from&nbsp;[../../LaravelFCM/Response/BaseResponse.md#property_retryAfter](<abbr title="LaravelFCM\Response\BaseResponse">BaseResponse</abbr>)</small>|
|<a name="property_numberTokensSuccess"></a>protected int|$numberTokensSuccess|||
|<a name="property_numberTokensFailure"></a>protected int|$numberTokensFailure|||
|<a name="property_tokensFailed"></a>protected array|$tokensFailed|||
|<a name="property_to"></a>protected string|$to|||
### Methods

|   |   |   |   |
|---|---|---|---|
||<a name="#method___construct"></a>__construct(<abbr title="Psr\Http\Message\ResponseInterface">ResponseInterface</abbr> $response, string $to, <abbr title="Monolog\Logger">Logger</abbr> $logger)|GroupResponse constructor.||
|int|string|null|<a name="#method_getRetryAfterHeaderValue"></a>getRetryAfterHeaderValue()|No description|from&nbsp;[../../LaravelFCM/Response/BaseResponse.md#method_getRetryAfterHeaderValue](<abbr title="LaravelFCM\Response\BaseResponse">BaseResponse</abbr>)|
|void|<a name="#method_parseResponse"></a>parseResponse(array $responseInJson)|parse the response.||
|void|<a name="#method_logResponse"></a>logResponse()|Log the response.||
|int|<a name="#method_numberSuccess"></a>numberSuccess()|Get the number of device reached with success.||
|int|<a name="#method_numberFailure"></a>numberFailure()|Get the number of device which thrown an error.||
|array|<a name="#method_tokensFailed"></a>tokensFailed()|Get all token in group that fcm cannot reach.||


### Details
<a name id="method___construct"></a>

### 
  **__construct**(<abbr title="Psr\Http\Message\ResponseInterface">ResponseInterface</abbr> $response, string $to, <abbr title="Monolog\Logger">Logger</abbr> $logger)

[at line 46](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/GroupResponse.php#L46)

GroupResponse constructor.        

#### Parameters

|   |   |   |
|---|---|---|
|<abbr title="Psr\Http\Message\ResponseInterface">ResponseInterface</abbr>|$response||string|$to||<abbr title="Monolog\Logger">Logger</abbr>|$logger|
<a name id="method_getRetryAfterHeaderValue"></a>

### 
 int|string|null **getRetryAfterHeaderValue**()in [../../LaravelFCM/Response/BaseResponse.md#method_getRetryAfterHeaderValue](<abbr title="LaravelFCM\Response\BaseResponse">BaseResponse</abbr>)

[at line 83](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/BaseResponse.php#L83)



#### Return Value

|   |   |
|---|---|
|int|string|null|

<a name id="method_parseResponse"></a>

### 
protected void **parseResponse**(array $responseInJson)

[at line 58](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/GroupResponse.php#L58)

parse the response.        

#### Parameters

|   |   |   |
|---|---|---|
|array|$responseInJson|

#### Return Value

|   |   |
|---|---|
|void|

<a name id="method_logResponse"></a>

### 
protected void **logResponse**()

[at line 74](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/GroupResponse.php#L74)

Log the response.        

#### Return Value

|   |   |
|---|---|
|void|

<a name id="method_numberSuccess"></a>

### 
 int **numberSuccess**()

[at line 121](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/GroupResponse.php#L121)

Get the number of device reached with success.        

#### Return Value

|   |   |
|---|---|
|int|

<a name id="method_numberFailure"></a>

### 
 int **numberFailure**()

[at line 131](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/GroupResponse.php#L131)

Get the number of device which thrown an error.        

#### Return Value

|   |   |
|---|---|
|int|

<a name id="method_tokensFailed"></a>

### 
 array **tokensFailed**()

[at line 141](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/GroupResponse.php#L141)

Get all token in group that fcm cannot reach.        

#### Return Value

|   |   |
|---|---|
|array|

_Generated by [Doctum, a API Documentation generator and fork of Sami](https://github.com/code-lts/doctum)._