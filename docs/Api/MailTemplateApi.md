# Swagger\Client\MailTemplateApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAll**](MailTemplateApi.md#getAll) | **GET** /v1/mail_template | Get all templates
[**getAllCustom**](MailTemplateApi.md#getAllCustom) | **GET** /v1/mail_template/all_custom | 
[**getMailTemplate**](MailTemplateApi.md#getMailTemplate) | **GET** /v1/mail_template/{mail_type} | Get template
[**getSample**](MailTemplateApi.md#getSample) | **GET** /v1/mail_template/sample | Get sample data
[**preview**](MailTemplateApi.md#preview) | **POST** /v1/mail_template/{mail_type}/preview | Preview template
[**reset**](MailTemplateApi.md#reset) | **POST** /v1/mail_template/{mail_type}/reset | Reset template
[**save**](MailTemplateApi.md#save) | **PUT** /v1/mail_template/{mail_type} | Update template
[**verifyMailTemplate**](MailTemplateApi.md#verifyMailTemplate) | **POST** /v1/mail_template/verify | Verify template


# **getAll**
> \Swagger\Client\Model\MailTemplate[] getAll()

Get all templates



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailTemplateApi();

try {
    $result = $api_instance->getAll();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailTemplateApi->getAll: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\MailTemplate[]**](../Model/MailTemplate.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getAllCustom**
> \Swagger\Client\Model\MailTemplate[] getAllCustom()



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailTemplateApi();

try {
    $result = $api_instance->getAllCustom();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailTemplateApi->getAllCustom: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\MailTemplate[]**](../Model/MailTemplate.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getMailTemplate**
> \Swagger\Client\Model\MailTemplate getMailTemplate($mail_type)

Get template



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailTemplateApi();
$mail_type = "mail_type_example"; // string | Mail type

try {
    $result = $api_instance->getMailTemplate($mail_type);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailTemplateApi->getMailTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mail_type** | **string**| Mail type |

### Return type

[**\Swagger\Client\Model\MailTemplate**](../Model/MailTemplate.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSample**
> map[string,object] getSample()

Get sample data



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailTemplateApi();

try {
    $result = $api_instance->getSample();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailTemplateApi->getSample: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**map[string,object]**](../Model/map.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **preview**
> \Swagger\Client\Model\MailTemplatePreviewContent preview($mail_type, $body)

Preview template



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailTemplateApi();
$mail_type = "mail_type_example"; // string | Mail type
$body = new \Swagger\Client\Model\PreviewMailTemplate(); // \Swagger\Client\Model\PreviewMailTemplate | 

try {
    $result = $api_instance->preview($mail_type, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailTemplateApi->preview: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mail_type** | **string**| Mail type |
 **body** | [**\Swagger\Client\Model\PreviewMailTemplate**](../Model/\Swagger\Client\Model\PreviewMailTemplate.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\MailTemplatePreviewContent**](../Model/MailTemplatePreviewContent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **reset**
> \Swagger\Client\Model\MailTemplate reset($mail_type)

Reset template



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailTemplateApi();
$mail_type = "mail_type_example"; // string | Mail type

try {
    $result = $api_instance->reset($mail_type);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailTemplateApi->reset: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mail_type** | **string**| Mail type |

### Return type

[**\Swagger\Client\Model\MailTemplate**](../Model/MailTemplate.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **save**
> \Swagger\Client\Model\MailTemplate save($mail_type, $body)

Update template



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailTemplateApi();
$mail_type = "mail_type_example"; // string | Mail type
$body = new \Swagger\Client\Model\UpdateMailTemplate(); // \Swagger\Client\Model\UpdateMailTemplate | 

try {
    $result = $api_instance->save($mail_type, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailTemplateApi->save: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mail_type** | **string**| Mail type |
 **body** | [**\Swagger\Client\Model\UpdateMailTemplate**](../Model/\Swagger\Client\Model\UpdateMailTemplate.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\MailTemplate**](../Model/MailTemplate.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **verifyMailTemplate**
> \Swagger\Client\Model\MailTemplateVerifyContent verifyMailTemplate($body)

Verify template



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailTemplateApi();
$body = new \Swagger\Client\Model\MailTemplateVerifyRequest(); // \Swagger\Client\Model\MailTemplateVerifyRequest | 

try {
    $result = $api_instance->verifyMailTemplate($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailTemplateApi->verifyMailTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\MailTemplateVerifyRequest**](../Model/\Swagger\Client\Model\MailTemplateVerifyRequest.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\MailTemplateVerifyContent**](../Model/MailTemplateVerifyContent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

