# Swagger\Client\InvoiceApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelAllDunningPending**](InvoiceApi.md#cancelAllDunningPending) | **POST** /v1/invoice/cancel_all_dunning_pending/subscription/{handle} | Cancel all dunning and pending
[**cancelInvoice**](InvoiceApi.md#cancelInvoice) | **POST** /v1/invoice/{id}/cancel | Cancel invoice
[**getInvoice**](InvoiceApi.md#getInvoice) | **GET** /v1/invoice/{id} | Get invoice
[**getInvoices**](InvoiceApi.md#getInvoices) | **GET** /v1/invoice | Get list of invoices
[**manualSettle**](InvoiceApi.md#manualSettle) | **POST** /v1/invoice/{id}/manual_settle | Manual settle
[**reactivate**](InvoiceApi.md#reactivate) | **POST** /v1/invoice/{id}/reactivate | Reactivate invoice
[**refund**](InvoiceApi.md#refund) | **POST** /v1/invoice/{id}/refund | Refund settled invoice
[**transactionDetails**](InvoiceApi.md#transactionDetails) | **GET** /v1/invoice/{id}/card_transaction/{transaction}/details | Get card transaction details


# **cancelAllDunningPending**
> \Swagger\Client\Model\Invoice[] cancelAllDunningPending($handle)

Cancel all dunning and pending



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\InvoiceApi();
$handle = "handle_example"; // string | Subscriptiom handle

try {
    $result = $api_instance->cancelAllDunningPending($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoiceApi->cancelAllDunningPending: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscriptiom handle |

### Return type

[**\Swagger\Client\Model\Invoice[]**](../Model/Invoice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **cancelInvoice**
> \Swagger\Client\Model\Invoice cancelInvoice($id)

Cancel invoice



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\InvoiceApi();
$id = "id_example"; // string | Invoice id

try {
    $result = $api_instance->cancelInvoice($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoiceApi->cancelInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Invoice id |

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getInvoice**
> \Swagger\Client\Model\Invoice getInvoice($id)

Get invoice



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\InvoiceApi();
$id = "id_example"; // string | Invoice id

try {
    $result = $api_instance->getInvoice($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoiceApi->getInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Invoice id |

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getInvoices**
> \Swagger\Client\Model\InvoiceSearch getInvoices($page, $size, $search, $sort)

Get list of invoices



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\InvoiceApi();
$page = 1; // int | Page number to get
$size = 20; // int | Page size to use
$search = "search_example"; // string | Optional search expression
$sort = "sort_example"; // string | Optional sorting expression

try {
    $result = $api_instance->getInvoices($page, $size, $search, $sort);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoiceApi->getInvoices: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Page number to get | [optional] [default to 1]
 **size** | **int**| Page size to use | [optional] [default to 20]
 **search** | **string**| Optional search expression | [optional]
 **sort** | **string**| Optional sorting expression | [optional]

### Return type

[**\Swagger\Client\Model\InvoiceSearch**](../Model/InvoiceSearch.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **manualSettle**
> \Swagger\Client\Model\Invoice manualSettle($id, $body)

Manual settle



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\InvoiceApi();
$id = "id_example"; // string | Invoice id
$body = new \Swagger\Client\Model\ManualSettleTransfer(); // \Swagger\Client\Model\ManualSettleTransfer | 

try {
    $result = $api_instance->manualSettle($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoiceApi->manualSettle: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Invoice id |
 **body** | [**\Swagger\Client\Model\ManualSettleTransfer**](../Model/\Swagger\Client\Model\ManualSettleTransfer.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **reactivate**
> \Swagger\Client\Model\Invoice reactivate($id)

Reactivate invoice



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\InvoiceApi();
$id = "id_example"; // string | Invoice id

try {
    $result = $api_instance->reactivate($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoiceApi->reactivate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Invoice id |

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **refund**
> \Swagger\Client\Model\Invoice refund($id, $body)

Refund settled invoice



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\InvoiceApi();
$id = "id_example"; // string | Invoice id
$body = new \Swagger\Client\Model\RefundInvoice(); // \Swagger\Client\Model\RefundInvoice | 

try {
    $result = $api_instance->refund($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoiceApi->refund: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Invoice id |
 **body** | [**\Swagger\Client\Model\RefundInvoice**](../Model/\Swagger\Client\Model\RefundInvoice.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **transactionDetails**
> map[string,object] transactionDetails($id, $transaction)

Get card transaction details



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\InvoiceApi();
$id = "id_example"; // string | Invoice id
$transaction = "transaction_example"; // string | Transaction id

try {
    $result = $api_instance->transactionDetails($id, $transaction);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoiceApi->transactionDetails: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Invoice id |
 **transaction** | **string**| Transaction id |

### Return type

[**map[string,object]**](../Model/map.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

