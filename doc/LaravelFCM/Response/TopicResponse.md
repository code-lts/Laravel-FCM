# LaravelFCM\Response\TopicResponse | Laravel / Lumen package for Firebase Cloud Messaging    

## [Laravel / Lumen package for Firebase Cloud Messaging](../../index.md)

- [Classes](../../classes.md)
- [Namespaces](../../namespaces.md)
- [Interfaces](../../interfaces.md)
- [Traits](../../traits.md)
- [Index](../../doc-index.md)
- [Search](../../search.md)

>class

>    [LaravelFCM](../../LaravelFCM.md)` / `[Response](../../LaravelFCM/Response.md)` / `(TopicResponse)
## TopicResponse

class **TopicResponse**        extends [<abbr title="LaravelFCM\Response\BaseResponse">BaseResponse</abbr>](../../LaravelFCM/Response/BaseResponse.md)        implements
        [<abbr title="LaravelFCM\Response\TopicResponseContract">TopicResponseContract</abbr>](../../LaravelFCM/Response/TopicResponseContract.md) [View source](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/TopicResponse.php)






### Constants

|   |   |
|---|---|
|SUCCESS||
|FAILURE||
|ERROR||
|MESSAGE_ID||
|LIMIT_RATE_TOPICS_EXCEEDED||

### Properties

|   |   |   |   |
|---|---|---|---|
|<a name="property_logEnabled"></a>protected bool|$logEnabled||<small>from&nbsp;[../../LaravelFCM/Response/BaseResponse.md#property_logEnabled](<abbr title="LaravelFCM\Response\BaseResponse">BaseResponse</abbr>)</small>|
|<a name="property_logger"></a>protected <abbr title="Monolog\Logger">Logger</abbr>|$logger|The logger.|<small>from&nbsp;[../../LaravelFCM/Response/BaseResponse.md#property_logger](<abbr title="LaravelFCM\Response\BaseResponse">BaseResponse</abbr>)</small>|
|<a name="property_topic"></a>protected Topics|$topic|||
|<a name="property_messageId"></a>protected string|$messageId|||
|<a name="property_error"></a>protected string|$error|||
|<a name="property_needRetry"></a>protected bool|$needRetry|||
### Methods

|   |   |   |   |
|---|---|---|---|
||<a name="#method___construct"></a>__construct(<abbr title="Psr\Http\Message\ResponseInterface">ResponseInterface</abbr> $response, [<abbr title="LaravelFCM\Message\Topics">Topics</abbr>](../../LaravelFCM/Message/Topics.md) $topic, <abbr title="Monolog\Logger">Logger</abbr> $logger)|TopicResponse constructor.||
||<a name="#method_parseResponse"></a>parseResponse(array $responseInJson)|parse the response.||
||<a name="#method_logResponse"></a>logResponse()|Log the response.||
|bool|<a name="#method_isSuccess"></a>isSuccess()|true if topic sent with success.||
|string|<a name="#method_error"></a>error()|return error message. you should test if it&#039;s necessary to resent it.||
|bool|<a name="#method_shouldRetry"></a>shouldRetry()|return true if it&#039;s necessary resent it using exponential backoff.||


### Details
<a name id="method___construct"></a>

### 
  **__construct**(<abbr title="Psr\Http\Message\ResponseInterface">ResponseInterface</abbr> $response, [<abbr title="LaravelFCM\Message\Topics">Topics</abbr>](../../LaravelFCM/Message/Topics.md) $topic, <abbr title="Monolog\Logger">Logger</abbr> $logger)

[at line 47](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/TopicResponse.php#L47)

TopicResponse constructor.        

#### Parameters

|   |   |   |
|---|---|---|
|<abbr title="Psr\Http\Message\ResponseInterface">ResponseInterface</abbr>|$response||[<abbr title="LaravelFCM\Message\Topics">Topics</abbr>](../../LaravelFCM/Message/Topics.md)|$topic||<abbr title="Monolog\Logger">Logger</abbr>|$logger|
<a name id="method_parseResponse"></a>

### 
protected  **parseResponse**(array $responseInJson)

[at line 58](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/TopicResponse.php#L58)

parse the response.        

#### Parameters

|   |   |   |
|---|---|---|
|array|$responseInJson|
<a name id="method_logResponse"></a>

### 
protected  **logResponse**()

[at line 100](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/TopicResponse.php#L100)

Log the response.        
<a name id="method_isSuccess"></a>

### 
 bool **isSuccess**()

[at line 119](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/TopicResponse.php#L119)

true if topic sent with success.        

#### Return Value

|   |   |
|---|---|
|bool|

<a name id="method_error"></a>

### 
 string **error**()

[at line 130](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/TopicResponse.php#L130)

return error message
you should test if it's necessary to resent it.        

#### Return Value

|   |   |
|---|---|
|string|error

<a name id="method_shouldRetry"></a>

### 
 bool **shouldRetry**()

[at line 140](https://github.com/code-lts/Laravel-FCM/blob/main/src/Response/TopicResponse.php#L140)

return true if it's necessary resent it using exponential backoff.        

#### Return Value

|   |   |
|---|---|
|bool|

_Generated by [Doctum, a API Documentation generator and fork of Sami](https://github.com/code-lts/doctum)._