# Swagger\Client\DiscountApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDiscount**](DiscountApi.md#createDiscount) | **POST** /v1/discount | Create discount
[**deleteDiscount**](DiscountApi.md#deleteDiscount) | **DELETE** /v1/discount/{handle} | Delete discount
[**getDiscount**](DiscountApi.md#getDiscount) | **GET** /v1/discount/{handle} | Get discount
[**getDiscounts**](DiscountApi.md#getDiscounts) | **GET** /v1/discount | Get list of discounts
[**undeleteDiscount**](DiscountApi.md#undeleteDiscount) | **POST** /v1/discount/{handle}/undelete | Undelete discount


# **createDiscount**
> \Swagger\Client\Model\Discount createDiscount($body)

Create discount



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DiscountApi();
$body = new \Swagger\Client\Model\CreateDiscount(); // \Swagger\Client\Model\CreateDiscount | 

try {
    $result = $api_instance->createDiscount($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DiscountApi->createDiscount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateDiscount**](../Model/\Swagger\Client\Model\CreateDiscount.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Discount**](../Model/Discount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteDiscount**
> \Swagger\Client\Model\Discount deleteDiscount($handle)

Delete discount



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DiscountApi();
$handle = "handle_example"; // string | Discount handle

try {
    $result = $api_instance->deleteDiscount($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DiscountApi->deleteDiscount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Discount handle |

### Return type

[**\Swagger\Client\Model\Discount**](../Model/Discount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getDiscount**
> \Swagger\Client\Model\Discount getDiscount($handle)

Get discount



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DiscountApi();
$handle = "handle_example"; // string | Discount handle

try {
    $result = $api_instance->getDiscount($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DiscountApi->getDiscount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Discount handle |

### Return type

[**\Swagger\Client\Model\Discount**](../Model/Discount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getDiscounts**
> \Swagger\Client\Model\DiscountSearch getDiscounts($page, $size, $search, $sort)

Get list of discounts



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DiscountApi();
$page = 1; // int | Page number to get
$size = 20; // int | Page size to use
$search = "search_example"; // string | Optional search expression
$sort = "sort_example"; // string | Optional sorting expression

try {
    $result = $api_instance->getDiscounts($page, $size, $search, $sort);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DiscountApi->getDiscounts: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Page number to get | [default to 1]
 **size** | **int**| Page size to use | [default to 20]
 **search** | **string**| Optional search expression |
 **sort** | **string**| Optional sorting expression |

### Return type

[**\Swagger\Client\Model\DiscountSearch**](../Model/DiscountSearch.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **undeleteDiscount**
> \Swagger\Client\Model\Discount undeleteDiscount($handle)

Undelete discount



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DiscountApi();
$handle = "handle_example"; // string | Discount handle

try {
    $result = $api_instance->undeleteDiscount($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DiscountApi->undeleteDiscount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Discount handle |

### Return type

[**\Swagger\Client\Model\Discount**](../Model/Discount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

