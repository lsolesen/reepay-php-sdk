# Swagger\Client\CreditApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelCredit**](CreditApi.md#cancelCredit) | **POST** /v1/credit/{handle}/cancel | Cancel credit
[**createCreditJson**](CreditApi.md#createCreditJson) | **POST** /v1/credit | Create credit
[**getCredit**](CreditApi.md#getCredit) | **GET** /v1/credit/{handle} | Get credit
[**getCredits**](CreditApi.md#getCredits) | **GET** /v1/credit/subscription/{handle} | Get credits for subscription


# **cancelCredit**
> \Swagger\Client\Model\Credit cancelCredit($handle)

Cancel credit



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CreditApi();
$handle = "handle_example"; // string | Credit handle

try {
    $result = $api_instance->cancelCredit($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CreditApi->cancelCredit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Credit handle |

### Return type

[**\Swagger\Client\Model\Credit**](../Model/Credit.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createCreditJson**
> \Swagger\Client\Model\Credit createCreditJson($body)

Create credit



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CreditApi();
$body = new \Swagger\Client\Model\CreateCredit(); // \Swagger\Client\Model\CreateCredit | 

try {
    $result = $api_instance->createCreditJson($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CreditApi->createCreditJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateCredit**](../Model/\Swagger\Client\Model\CreateCredit.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Credit**](../Model/Credit.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCredit**
> \Swagger\Client\Model\Credit getCredit($handle)

Get credit



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CreditApi();
$handle = "handle_example"; // string | Credit handle

try {
    $result = $api_instance->getCredit($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CreditApi->getCredit: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Credit handle |

### Return type

[**\Swagger\Client\Model\Credit**](../Model/Credit.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCredits**
> \Swagger\Client\Model\Credit[] getCredits($handle)

Get credits for subscription



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CreditApi();
$handle = "handle_example"; // string | Subscription handle

try {
    $result = $api_instance->getCredits($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CreditApi->getCredits: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |

### Return type

[**\Swagger\Client\Model\Credit[]**](../Model/Credit.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

