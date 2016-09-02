# Swagger\Client\CustomerApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activatePaymentMethod**](CustomerApi.md#activatePaymentMethod) | **POST** /v1/customer/{handle}/payment_method/{method_id}/activate | Activate payment method
[**addCardJson**](CustomerApi.md#addCardJson) | **POST** /v1/customer/{handle}/payment_method/card | Add card payment method
[**createCustomerInvoice**](CustomerApi.md#createCustomerInvoice) | **POST** /v1/customer/{handle}/invoice | Create invoice ondemand for customer
[**createCustomerJson**](CustomerApi.md#createCustomerJson) | **POST** /v1/customer | Create customer
[**createCustomerNoteJson**](CustomerApi.md#createCustomerNoteJson) | **POST** /v1/customer/{handle}/note | Create customer note
[**deleteCustomer**](CustomerApi.md#deleteCustomer) | **DELETE** /v1/customer/{handle} | Delete customer
[**getCard**](CustomerApi.md#getCard) | **GET** /v1/customer/{handle}/payment_method/card/{id} | Get card
[**getCardDetails**](CustomerApi.md#getCardDetails) | **GET** /v1/customer/{handle}/payment_method/card/{id}/details | Get gateway card details
[**getCustomer**](CustomerApi.md#getCustomer) | **GET** /v1/customer/{handle} | Get customer
[**getCustomerNotes**](CustomerApi.md#getCustomerNotes) | **GET** /v1/customer/{handle}/note | Get customer notes
[**getCustomerPaymentMethods**](CustomerApi.md#getCustomerPaymentMethods) | **GET** /v1/customer/{handle}/payment_method | Get payment methods
[**getCustomers**](CustomerApi.md#getCustomers) | **GET** /v1/customer | Get list of customers
[**importCardJson**](CustomerApi.md#importCardJson) | **POST** /v1/customer/{handle}/payment_method/card_import | Import card payment method
[**inactivatePaymentMethod**](CustomerApi.md#inactivatePaymentMethod) | **POST** /v1/customer/{handle}/payment_method/{method_id}/inactivate | Inactivate payment method
[**updateCustomerJson**](CustomerApi.md#updateCustomerJson) | **PUT** /v1/customer/{handle} | Update customer


# **activatePaymentMethod**
> \Swagger\Client\Model\PaymentMethods activatePaymentMethod($handle, $method_id)

Activate payment method



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle
$method_id = "method_id_example"; // string | Payment method id

try {
    $result = $api_instance->activatePaymentMethod($handle, $method_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->activatePaymentMethod: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |
 **method_id** | **string**| Payment method id |

### Return type

[**\Swagger\Client\Model\PaymentMethods**](../Model/PaymentMethods.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **addCardJson**
> \Swagger\Client\Model\Card addCardJson($handle, $body)

Add card payment method



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle
$body = new \Swagger\Client\Model\CardToken(); // \Swagger\Client\Model\CardToken | 

try {
    $result = $api_instance->addCardJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->addCardJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |
 **body** | [**\Swagger\Client\Model\CardToken**](../Model/\Swagger\Client\Model\CardToken.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Card**](../Model/Card.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createCustomerInvoice**
> \Swagger\Client\Model\Invoice createCustomerInvoice($handle, $body)

Create invoice ondemand for customer



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle
$body = new \Swagger\Client\Model\CreateCustomerInvoice(); // \Swagger\Client\Model\CreateCustomerInvoice | 

try {
    $result = $api_instance->createCustomerInvoice($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->createCustomerInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |
 **body** | [**\Swagger\Client\Model\CreateCustomerInvoice**](../Model/\Swagger\Client\Model\CreateCustomerInvoice.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createCustomerJson**
> \Swagger\Client\Model\Customer createCustomerJson($body)

Create customer



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$body = new \Swagger\Client\Model\CreateCustomer(); // \Swagger\Client\Model\CreateCustomer | 

try {
    $result = $api_instance->createCustomerJson($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->createCustomerJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateCustomer**](../Model/\Swagger\Client\Model\CreateCustomer.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Customer**](../Model/Customer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createCustomerNoteJson**
> \Swagger\Client\Model\CustomerNote createCustomerNoteJson($handle, $body)

Create customer note



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | 
$body = new \Swagger\Client\Model\CreateCustomerNote(); // \Swagger\Client\Model\CreateCustomerNote | 

try {
    $result = $api_instance->createCustomerNoteJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->createCustomerNoteJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**|  |
 **body** | [**\Swagger\Client\Model\CreateCustomerNote**](../Model/\Swagger\Client\Model\CreateCustomerNote.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\CustomerNote**](../Model/CustomerNote.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteCustomer**
> \Swagger\Client\Model\Customer deleteCustomer($handle)

Delete customer



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle

try {
    $result = $api_instance->deleteCustomer($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->deleteCustomer: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |

### Return type

[**\Swagger\Client\Model\Customer**](../Model/Customer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCard**
> \Swagger\Client\Model\Card getCard($handle, $id)

Get card



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle
$id = "id_example"; // string | Card id

try {
    $result = $api_instance->getCard($handle, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->getCard: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |
 **id** | **string**| Card id |

### Return type

[**\Swagger\Client\Model\Card**](../Model/Card.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCardDetails**
> map[string,object] getCardDetails($handle, $id)

Get gateway card details



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle
$id = "id_example"; // string | Card id

try {
    $result = $api_instance->getCardDetails($handle, $id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->getCardDetails: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |
 **id** | **string**| Card id |

### Return type

[**map[string,object]**](../Model/map.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCustomer**
> \Swagger\Client\Model\Customer getCustomer($handle)

Get customer



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle

try {
    $result = $api_instance->getCustomer($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->getCustomer: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |

### Return type

[**\Swagger\Client\Model\Customer**](../Model/Customer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCustomerNotes**
> \Swagger\Client\Model\CustomerNote[] getCustomerNotes($handle)

Get customer notes



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle

try {
    $result = $api_instance->getCustomerNotes($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->getCustomerNotes: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |

### Return type

[**\Swagger\Client\Model\CustomerNote[]**](../Model/CustomerNote.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCustomerPaymentMethods**
> \Swagger\Client\Model\PaymentMethods getCustomerPaymentMethods($handle)

Get payment methods



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle

try {
    $result = $api_instance->getCustomerPaymentMethods($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->getCustomerPaymentMethods: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |

### Return type

[**\Swagger\Client\Model\PaymentMethods**](../Model/PaymentMethods.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCustomers**
> \Swagger\Client\Model\CustomerSearch getCustomers($page, $size, $search, $sort)

Get list of customers



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$page = 1; // int | Page number to get
$size = 20; // int | Page size to use
$search = "search_example"; // string | Optional search expression
$sort = "sort_example"; // string | Optional sorting expression

try {
    $result = $api_instance->getCustomers($page, $size, $search, $sort);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->getCustomers: ', $e->getMessage(), PHP_EOL;
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

[**\Swagger\Client\Model\CustomerSearch**](../Model/CustomerSearch.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **importCardJson**
> \Swagger\Client\Model\Card importCardJson($handle, $body)

Import card payment method



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle
$body = new \Swagger\Client\Model\CardImport(); // \Swagger\Client\Model\CardImport | 

try {
    $result = $api_instance->importCardJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->importCardJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |
 **body** | [**\Swagger\Client\Model\CardImport**](../Model/\Swagger\Client\Model\CardImport.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Card**](../Model/Card.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **inactivatePaymentMethod**
> \Swagger\Client\Model\PaymentMethods inactivatePaymentMethod($handle, $method_id)

Inactivate payment method



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle
$method_id = "method_id_example"; // string | Payment method id

try {
    $result = $api_instance->inactivatePaymentMethod($handle, $method_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->inactivatePaymentMethod: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |
 **method_id** | **string**| Payment method id |

### Return type

[**\Swagger\Client\Model\PaymentMethods**](../Model/PaymentMethods.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateCustomerJson**
> \Swagger\Client\Model\Customer updateCustomerJson($handle, $body)

Update customer



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CustomerApi();
$handle = "handle_example"; // string | Customer handle
$body = new \Swagger\Client\Model\UpdateCustomer(); // \Swagger\Client\Model\UpdateCustomer | 

try {
    $result = $api_instance->updateCustomerJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CustomerApi->updateCustomerJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Customer handle |
 **body** | [**\Swagger\Client\Model\UpdateCustomer**](../Model/\Swagger\Client\Model\UpdateCustomer.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Customer**](../Model/Customer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

