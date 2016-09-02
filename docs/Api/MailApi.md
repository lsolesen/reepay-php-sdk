# Swagger\Client\MailApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getMail**](MailApi.md#getMail) | **GET** /v1/mail/{id} | Get mail
[**getMails**](MailApi.md#getMails) | **GET** /v1/mail | Get list of mails


# **getMail**
> \Swagger\Client\Model\Mail getMail($id)

Get mail



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailApi();
$id = "id_example"; // string | Mail id

try {
    $result = $api_instance->getMail($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailApi->getMail: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Mail id |

### Return type

[**\Swagger\Client\Model\Mail**](../Model/Mail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getMails**
> \Swagger\Client\Model\MailList getMails($page, $size, $customer, $subscription, $invoice, $created_before)

Get list of mails



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\MailApi();
$page = 1; // int | Page number to get
$size = 20; // int | Page size to use
$customer = "customer_example"; // string | Customer handle
$subscription = "subscription_example"; // string | Subscription handle
$invoice = "invoice_example"; // string | Invoice id
$created_before = "created_before_example"; // string | Optionally get mails created before this date, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format.

try {
    $result = $api_instance->getMails($page, $size, $customer, $subscription, $invoice, $created_before);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MailApi->getMails: ', $e->getMessage(), PHP_EOL;
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
 **created_before** | **string**| Optionally get mails created before this date, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional]

### Return type

[**\Swagger\Client\Model\MailList**](../Model/MailList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

