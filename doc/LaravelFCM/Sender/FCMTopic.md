# LaravelFCM\Sender\FCMTopic | Laravel / Lumen package for Firebase Cloud Messaging    

## [Laravel / Lumen package for Firebase Cloud Messaging](../../index.md)

- [Classes](../../classes.md)
- [Namespaces](../../namespaces.md)
- [Interfaces](../../interfaces.md)
- [Traits](../../traits.md)
- [Index](../../doc-index.md)
- [Search](../../search.md)

>class

>    [LaravelFCM](../../LaravelFCM.md)` / `[Sender](../../LaravelFCM/Sender.md)` / `(FCMTopic)
## FCMTopic

class **FCMTopic**        extends [<abbr title="LaravelFCM\Sender\HTTPSender">HTTPSender</abbr>](../../LaravelFCM/Sender/HTTPSender.md) [View source](https://github.com/code-lts/Laravel-FCM/blob/main/src/Sender/FCMTopic.php)






### Constants

|   |   |
|---|---|
|CREATE||
|SUBSCRIBE||
|UNSUBSCRIBE||

### Properties

|   |   |   |   |
|---|---|---|---|
|<a name="property_client"></a>protected <abbr title="GuzzleHttp\ClientInterface">ClientInterface</abbr>|$client|The client used to send messages.|<small>from&nbsp;[../../LaravelFCM/Sender/HTTPSender.md#property_client](<abbr title="LaravelFCM\Sender\HTTPSender">HTTPSender</abbr>)</small>|
|<a name="property_url"></a>protected string|$url|The URL entry point.|<small>from&nbsp;[../../LaravelFCM/Sender/HTTPSender.md#property_url](<abbr title="LaravelFCM\Sender\HTTPSender">HTTPSender</abbr>)</small>|
|<a name="property_logger"></a>protected <abbr title="Monolog\Logger">Logger</abbr>|$logger|The logger.|<small>from&nbsp;[../../LaravelFCM/Sender/HTTPSender.md#property_logger](<abbr title="LaravelFCM\Sender\HTTPSender">HTTPSender</abbr>)</small>|
### Methods

|   |   |   |   |
|---|---|---|---|
||<a name="#method___construct"></a>__construct(<abbr title="GuzzleHttp\ClientInterface">ClientInterface</abbr> $client, string $url, <abbr title="Monolog\Logger">Logger</abbr> $logger)|Initializes a new sender object.|from&nbsp;[../../LaravelFCM/Sender/HTTPSender.md#method___construct](<abbr title="LaravelFCM\Sender\HTTPSender">HTTPSender</abbr>)|
|bool|<a name="#method_createTopic"></a>createTopic(string $topicId, string $registrationId, string $serverKey = null, string $senderId = null)|Create a topic.||
|bool|<a name="#method_subscribeTopic"></a>subscribeTopic(string $topicId, array|string $recipientsTokens, string $serverKey = null, string $senderId = null)|Add subscription to a topic.||
|bool|<a name="#method_unsubscribeTopic"></a>unsubscribeTopic(string $topicId, array|string $recipientsTokens, string $serverKey = null, string $senderId = null)|Remove subscription from a topic.||
|bool|<a name="#method_isValidResponse"></a>isValidResponse(<abbr title="Psr\Http\Message\ResponseInterface">ResponseInterface</abbr> $response)|No description||


### Details
<a name id="method___construct"></a>

### 
  **__construct**(<abbr title="GuzzleHttp\ClientInterface">ClientInterface</abbr> $client, string $url, <abbr title="Monolog\Logger">Logger</abbr> $logger)in [../../LaravelFCM/Sender/HTTPSender.md#method___construct](<abbr title="LaravelFCM\Sender\HTTPSender">HTTPSender</abbr>)

[at line 37](https://github.com/code-lts/Laravel-FCM/blob/main/src/Sender/HTTPSender.php#L37)

Initializes a new sender object.        

#### Parameters

|   |   |   |
|---|---|---|
|<abbr title="GuzzleHttp\ClientInterface">ClientInterface</abbr>|$client||string|$url||<abbr title="Monolog\Logger">Logger</abbr>|$logger|
<a name id="method_createTopic"></a>

### 
 bool **createTopic**(string $topicId, string $registrationId, string $serverKey = null, string $senderId = null)

[at line 30](https://github.com/code-lts/Laravel-FCM/blob/main/src/Sender/FCMTopic.php#L30)

Create a topic.        

#### Parameters

|   |   |   |
|---|---|---|
|string|$topicId||string|$registrationId||string|$serverKey|(optional) The server key|string|$senderId|(optional) The sender Id

#### Return Value

|   |   |
|---|---|
|bool|

<a name id="method_subscribeTopic"></a>

### 
 bool **subscribeTopic**(string $topicId, array|string $recipientsTokens, string $serverKey = null, string $senderId = null)

[at line 54](https://github.com/code-lts/Laravel-FCM/blob/main/src/Sender/FCMTopic.php#L54)

Add subscription to a topic.        

#### Parameters

|   |   |   |
|---|---|---|
|string|$topicId||array|string|$recipientsTokens||string|$serverKey|(optional) The server key|string|$senderId|(optional) The sender Id

#### Return Value

|   |   |
|---|---|
|bool|

<a name id="method_unsubscribeTopic"></a>

### 
 bool **unsubscribeTopic**(string $topicId, array|string $recipientsTokens, string $serverKey = null, string $senderId = null)

[at line 75](https://github.com/code-lts/Laravel-FCM/blob/main/src/Sender/FCMTopic.php#L75)

Remove subscription from a topic.        

#### Parameters

|   |   |   |
|---|---|---|
|string|$topicId||array|string|$recipientsTokens||string|$serverKey|(optional) The server key|string|$senderId|(optional) The sender Id

#### Return Value

|   |   |
|---|---|
|bool|

<a name id="method_isValidResponse"></a>

### 
 bool **isValidResponse**(<abbr title="Psr\Http\Message\ResponseInterface">ResponseInterface</abbr> $response)

[at line 91](https://github.com/code-lts/Laravel-FCM/blob/main/src/Sender/FCMTopic.php#L91)



#### Parameters

|   |   |   |
|---|---|---|
|<abbr title="Psr\Http\Message\ResponseInterface">ResponseInterface</abbr>|$response|

#### Return Value

|   |   |
|---|---|
|bool|

_Generated by [Doctum, a API Documentation generator and fork of Sami](https://github.com/code-lts/doctum)._