# Swagger\Client\DunningPlanApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDunningPlanJson**](DunningPlanApi.md#createDunningPlanJson) | **POST** /v1/dunning_plan | Create dunning plan
[**deleteDunningPlan**](DunningPlanApi.md#deleteDunningPlan) | **DELETE** /v1/dunning_plan/{handle} | Delete dunning plan
[**getDunningPlan**](DunningPlanApi.md#getDunningPlan) | **GET** /v1/dunning_plan/{handle} | Get dunning plan
[**getDunningPlans**](DunningPlanApi.md#getDunningPlans) | **GET** /v1/dunning_plan | Get list of dunning plans
[**updateJson**](DunningPlanApi.md#updateJson) | **PUT** /v1/dunning_plan/{handle} | Update dunning plan


# **createDunningPlanJson**
> \Swagger\Client\Model\DunningPlan createDunningPlanJson($body)

Create dunning plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DunningPlanApi();
$body = new \Swagger\Client\Model\CreateDunningPlan(); // \Swagger\Client\Model\CreateDunningPlan | 

try {
    $result = $api_instance->createDunningPlanJson($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DunningPlanApi->createDunningPlanJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateDunningPlan**](../Model/\Swagger\Client\Model\CreateDunningPlan.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\DunningPlan**](../Model/DunningPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteDunningPlan**
> \Swagger\Client\Model\DunningPlan deleteDunningPlan($handle)

Delete dunning plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DunningPlanApi();
$handle = "handle_example"; // string | Dunning plan handle

try {
    $result = $api_instance->deleteDunningPlan($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DunningPlanApi->deleteDunningPlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Dunning plan handle |

### Return type

[**\Swagger\Client\Model\DunningPlan**](../Model/DunningPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getDunningPlan**
> \Swagger\Client\Model\DunningPlan getDunningPlan($handle)

Get dunning plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DunningPlanApi();
$handle = "handle_example"; // string | Dunning plan handle

try {
    $result = $api_instance->getDunningPlan($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DunningPlanApi->getDunningPlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Dunning plan handle |

### Return type

[**\Swagger\Client\Model\DunningPlan**](../Model/DunningPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getDunningPlans**
> \Swagger\Client\Model\DunningPlan[] getDunningPlans()

Get list of dunning plans



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DunningPlanApi();

try {
    $result = $api_instance->getDunningPlans();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DunningPlanApi->getDunningPlans: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\DunningPlan[]**](../Model/DunningPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateJson**
> \Swagger\Client\Model\DunningPlan updateJson($handle, $body)

Update dunning plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DunningPlanApi();
$handle = "handle_example"; // string | Dunning plan handle
$body = new \Swagger\Client\Model\UpdateDunningPlan(); // \Swagger\Client\Model\UpdateDunningPlan | 

try {
    $result = $api_instance->updateJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DunningPlanApi->updateJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Dunning plan handle |
 **body** | [**\Swagger\Client\Model\UpdateDunningPlan**](../Model/\Swagger\Client\Model\UpdateDunningPlan.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\DunningPlan**](../Model/DunningPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

