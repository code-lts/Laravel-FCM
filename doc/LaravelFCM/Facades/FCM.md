# LaravelFCM\Facades\FCM | Laravel / Lumen package for Firebase Cloud Messaging    

## [Laravel / Lumen package for Firebase Cloud Messaging](../../index.md)

- [Classes](../../classes.md)
- [Namespaces](../../namespaces.md)
- [Interfaces](../../interfaces.md)
- [Traits](../../traits.md)
- [Index](../../doc-index.md)
- [Search](../../search.md)

>class

>    [LaravelFCM](../../LaravelFCM.md)` / `[Facades](../../LaravelFCM/Facades.md)` / `(FCM)
## FCM

class **FCM**        extends <abbr title="Illuminate\Support\Facades\Facade">Facade</abbr> [View source](https://github.com/code-lts/Laravel-FCM/blob/main/src/Facades/FCM.php)






### Methods

|   |   |   |   |
|---|---|---|---|
|static&nbsp;|<a name="#method_getFacadeAccessor"></a>getFacadeAccessor()|No description||
|static&nbsp;[<abbr title="LaravelFCM\Response\GroupResponse">GroupResponse</abbr>](../../LaravelFCM/Response/GroupResponse.md)|<a name="#method_sendToGroup"></a>sendToGroup(string|string[] $notificationKey, <abbr title="LaravelFCM\Facades\Options|null">Options|null</abbr> $options, <abbr title="LaravelFCM\Facades\PayloadNotification|null">PayloadNotification|null</abbr> $notification, <abbr title="LaravelFCM\Facades\PayloadData|null">PayloadData|null</abbr> $data)|No description||


### Details
<a name id="method_getFacadeAccessor"></a>

### 
staticprotected  **getFacadeAccessor**()

[at line 12](https://github.com/code-lts/Laravel-FCM/blob/main/src/Facades/FCM.php#L12)


<a name id="method_sendToGroup"></a>

### 
static [<abbr title="LaravelFCM\Response\GroupResponse">GroupResponse</abbr>](../../LaravelFCM/Response/GroupResponse.md) **sendToGroup**(string|string[] $notificationKey, <abbr title="LaravelFCM\Facades\Options|null">Options|null</abbr> $options, <abbr title="LaravelFCM\Facades\PayloadNotification|null">PayloadNotification|null</abbr> $notification, <abbr title="LaravelFCM\Facades\PayloadData|null">PayloadData|null</abbr> $data)

[at line 10](https://github.com/code-lts/Laravel-FCM/blob/main/src/Facades/FCM.php#L10)



#### Parameters

|   |   |   |
|---|---|---|
|string|string[]|$notificationKey||<abbr title="LaravelFCM\Facades\Options|null">Options|null</abbr>|$options||<abbr title="LaravelFCM\Facades\PayloadNotification|null">PayloadNotification|null</abbr>|$notification||<abbr title="LaravelFCM\Facades\PayloadData|null">PayloadData|null</abbr>|$data|

#### Return Value

|   |   |
|---|---|
|[<abbr title="LaravelFCM\Response\GroupResponse">GroupResponse</abbr>](../../LaravelFCM/Response/GroupResponse.md)|

_Generated by [Doctum, a API Documentation generator and fork of Sami](https://github.com/code-lts/doctum)._