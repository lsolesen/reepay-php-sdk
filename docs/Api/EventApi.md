# Swagger\Client\EventApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getEvent**](EventApi.md#getEvent) | **GET** /v1/event/{id} | Get event
[**getEvents**](EventApi.md#getEvents) | **GET** /v1/event | Get list of events


# **getEvent**
> \Swagger\Client\Model\Event getEvent($id)

Get event



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\EventApi();
$id = "id_example"; // string | Event id

try {
    $result = $api_instance->getEvent($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventApi->getEvent: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Event id |

### Return type

[**\Swagger\Client\Model\Event**](../Model/Event.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getEvents**
> \Swagger\Client\Model\EventList getEvents($page, $size, $customer, $subscription, $invoice)

Get list of events



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\EventApi();
$page = 1; // int | Page number to get
$size = 20; // int | Page size to use
$customer = "customer_example"; // string | Customer handle
$subscription = "subscription_example"; // string | Subscription handle
$invoice = "invoice_example"; // string | Invoice id

try {
    $result = $api_instance->getEvents($page, $size, $customer, $subscription, $invoice);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventApi->getEvents: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Page number to get | [optional] [default to 1]
 **size** | **int**| Page size to use | [optional] [default to 20]
 **customer** | **string**| Customer handle | [optional]
 **subscription** | **string**| Subscription handle | [optional]
 **invoice** | **string**| Invoice id | [optional]

### Return type

[**\Swagger\Client\Model\EventList**](../Model/EventList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

