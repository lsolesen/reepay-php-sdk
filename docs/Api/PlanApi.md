# Swagger\Client\PlanApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPlanJson**](PlanApi.md#createPlanJson) | **POST** /v1/plan | Create plan
[**deletePlan**](PlanApi.md#deletePlan) | **DELETE** /v1/plan/{handle} | Delete plan
[**getCurrentPlan**](PlanApi.md#getCurrentPlan) | **GET** /v1/plan/{handle}/current | Get plan
[**getPlan**](PlanApi.md#getPlan) | **GET** /v1/plan/{handle}/{version} | Get plan version
[**getPlans**](PlanApi.md#getPlans) | **GET** /v1/plan/{handle} | Get list of plan versions
[**getPlansList**](PlanApi.md#getPlansList) | **GET** /v1/plan | Get list of plans
[**supersedePlanJson**](PlanApi.md#supersedePlanJson) | **POST** /v1/plan/{handle} | Supersede plan
[**updatePlanJson**](PlanApi.md#updatePlanJson) | **PUT** /v1/plan/{handle} | Update plan


# **createPlanJson**
> \Swagger\Client\Model\Plan createPlanJson($body)

Create plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\PlanApi();
$body = new \Swagger\Client\Model\CreateSubscriptionPlan(); // \Swagger\Client\Model\CreateSubscriptionPlan | 

try {
    $result = $api_instance->createPlanJson($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PlanApi->createPlanJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateSubscriptionPlan**](../Model/\Swagger\Client\Model\CreateSubscriptionPlan.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Plan**](../Model/Plan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deletePlan**
> \Swagger\Client\Model\Plan deletePlan($handle)

Delete plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\PlanApi();
$handle = "handle_example"; // string | Subscription plan handle

try {
    $result = $api_instance->deletePlan($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PlanApi->deletePlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription plan handle |

### Return type

[**\Swagger\Client\Model\Plan**](../Model/Plan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCurrentPlan**
> \Swagger\Client\Model\Plan getCurrentPlan($handle)

Get plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\PlanApi();
$handle = "handle_example"; // string | Plan handle

try {
    $result = $api_instance->getCurrentPlan($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PlanApi->getCurrentPlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Plan handle |

### Return type

[**\Swagger\Client\Model\Plan**](../Model/Plan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPlan**
> \Swagger\Client\Model\Plan getPlan($handle, $version)

Get plan version



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\PlanApi();
$handle = "handle_example"; // string | Plan handle
$version = 56; // int | Plan version

try {
    $result = $api_instance->getPlan($handle, $version);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PlanApi->getPlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Plan handle |
 **version** | **int**| Plan version |

### Return type

[**\Swagger\Client\Model\Plan**](../Model/Plan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPlans**
> \Swagger\Client\Model\Plan[] getPlans($handle)

Get list of plan versions



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\PlanApi();
$handle = "handle_example"; // string | Plan handle

try {
    $result = $api_instance->getPlans($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PlanApi->getPlans: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Plan handle |

### Return type

[**\Swagger\Client\Model\Plan[]**](../Model/Plan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPlansList**
> \Swagger\Client\Model\Plan[] getPlansList($only_active)

Get list of plans



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\PlanApi();
$only_active = false; // bool | 

try {
    $result = $api_instance->getPlansList($only_active);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PlanApi->getPlansList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **only_active** | **bool**|  | [optional] [default to false]

### Return type

[**\Swagger\Client\Model\Plan[]**](../Model/Plan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **supersedePlanJson**
> \Swagger\Client\Model\Plan supersedePlanJson($handle, $body)

Supersede plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\PlanApi();
$handle = "handle_example"; // string | Plan handle
$body = new \Swagger\Client\Model\SupersedeSubscriptionPlan(); // \Swagger\Client\Model\SupersedeSubscriptionPlan | 

try {
    $result = $api_instance->supersedePlanJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PlanApi->supersedePlanJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Plan handle |
 **body** | [**\Swagger\Client\Model\SupersedeSubscriptionPlan**](../Model/\Swagger\Client\Model\SupersedeSubscriptionPlan.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Plan**](../Model/Plan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updatePlanJson**
> \Swagger\Client\Model\Plan updatePlanJson($handle, $body)

Update plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\PlanApi();
$handle = "handle_example"; // string | Subscription handle
$body = new \Swagger\Client\Model\UpdateSubscriptionPlan(); // \Swagger\Client\Model\UpdateSubscriptionPlan | 

try {
    $result = $api_instance->updatePlanJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PlanApi->updatePlanJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **body** | [**\Swagger\Client\Model\UpdateSubscriptionPlan**](../Model/\Swagger\Client\Model\UpdateSubscriptionPlan.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Plan**](../Model/Plan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

