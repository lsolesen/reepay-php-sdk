# Swagger\Client\SubscriptionApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelChangePlan**](SubscriptionApi.md#cancelChangePlan) | **POST** /v1/subscription/{handle}/cancel_change_plan | Cancel pending plan change
[**cancelSubscription**](SubscriptionApi.md#cancelSubscription) | **POST** /v1/subscription/{handle}/cancel | Cancel subscription
[**changeNextPeriodStartJson**](SubscriptionApi.md#changeNextPeriodStartJson) | **POST** /v1/subscription/{handle}/change_next_period_start | Change next renewal date
[**changePlanJson**](SubscriptionApi.md#changePlanJson) | **POST** /v1/subscription/{handle}/change_plan | Change plan
[**createSubscriptionDiscount**](SubscriptionApi.md#createSubscriptionDiscount) | **POST** /v1/subscription/{handle}/discount | Add subscription discount
[**createSubscriptionInvoice**](SubscriptionApi.md#createSubscriptionInvoice) | **POST** /v1/subscription/{handle}/invoice | Create invoice ondemand for subscription
[**createSubscriptionJson**](SubscriptionApi.md#createSubscriptionJson) | **POST** /v1/subscription | Create subscription
[**deleteSubscriptionDiscount**](SubscriptionApi.md#deleteSubscriptionDiscount) | **DELETE** /v1/subscription/{handle}/discount/{sdHandle} | Delete subscription discount
[**expire**](SubscriptionApi.md#expire) | **POST** /v1/subscription/{handle}/expire | Expire subscription
[**getSubscription**](SubscriptionApi.md#getSubscription) | **GET** /v1/subscription/{handle} | Get subscription
[**getSubscriptionDiscount**](SubscriptionApi.md#getSubscriptionDiscount) | **GET** /v1/subscription/{handle}/discount/{sdHandle} | Get subscription discount
[**getSubscriptionDiscounts**](SubscriptionApi.md#getSubscriptionDiscounts) | **GET** /v1/subscription/{handle}/discount | Get subscription discounts
[**getSubscriptionPaymentMethods**](SubscriptionApi.md#getSubscriptionPaymentMethods) | **GET** /v1/subscription/{handle}/payment_method | Get payment methods
[**getSubscriptions**](SubscriptionApi.md#getSubscriptions) | **GET** /v1/subscription | Get list of subscriptions
[**intervalAmount**](SubscriptionApi.md#intervalAmount) | **GET** /v1/subscription/{handle}/interval_amount | Calculate interval amount
[**removeAllPaymentMethods**](SubscriptionApi.md#removeAllPaymentMethods) | **DELETE** /v1/subscription/{handle}/payment_method | Remove all payment methods
[**removePaymentMethod**](SubscriptionApi.md#removePaymentMethod) | **DELETE** /v1/subscription/{handle}/payment_method/{method_id} | Remove payment method
[**setCardPaymentMethodJson**](SubscriptionApi.md#setCardPaymentMethodJson) | **POST** /v1/subscription/{handle}/payment_method/card | Set card payment method
[**uncancel**](SubscriptionApi.md#uncancel) | **POST** /v1/subscription/{handle}/uncancel | Uncancel subscription


# **cancelChangePlan**
> \Swagger\Client\Model\Subscription cancelChangePlan($handle)

Cancel pending plan change



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle

try {
    $result = $api_instance->cancelChangePlan($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->cancelChangePlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |

### Return type

[**\Swagger\Client\Model\Subscription**](../Model/Subscription.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **cancelSubscription**
> \Swagger\Client\Model\Subscription cancelSubscription($handle)

Cancel subscription



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle

try {
    $result = $api_instance->cancelSubscription($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->cancelSubscription: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |

### Return type

[**\Swagger\Client\Model\Subscription**](../Model/Subscription.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **changeNextPeriodStartJson**
> \Swagger\Client\Model\Subscription changeNextPeriodStartJson($handle, $body)

Change next renewal date



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle
$body = new \Swagger\Client\Model\ChangeNextPeriodStart(); // \Swagger\Client\Model\ChangeNextPeriodStart | 

try {
    $result = $api_instance->changeNextPeriodStartJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->changeNextPeriodStartJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **body** | [**\Swagger\Client\Model\ChangeNextPeriodStart**](../Model/\Swagger\Client\Model\ChangeNextPeriodStart.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Subscription**](../Model/Subscription.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **changePlanJson**
> \Swagger\Client\Model\Subscription changePlanJson($handle, $body)

Change plan



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle
$body = new \Swagger\Client\Model\ChangePlan(); // \Swagger\Client\Model\ChangePlan | 

try {
    $result = $api_instance->changePlanJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->changePlanJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **body** | [**\Swagger\Client\Model\ChangePlan**](../Model/\Swagger\Client\Model\ChangePlan.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Subscription**](../Model/Subscription.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createSubscriptionDiscount**
> \Swagger\Client\Model\SubscriptionDiscount createSubscriptionDiscount($handle, $body)

Add subscription discount



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle
$body = new \Swagger\Client\Model\CreateSubscriptionDiscount(); // \Swagger\Client\Model\CreateSubscriptionDiscount | 

try {
    $result = $api_instance->createSubscriptionDiscount($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->createSubscriptionDiscount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **body** | [**\Swagger\Client\Model\CreateSubscriptionDiscount**](../Model/\Swagger\Client\Model\CreateSubscriptionDiscount.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\SubscriptionDiscount**](../Model/SubscriptionDiscount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createSubscriptionInvoice**
> \Swagger\Client\Model\Invoice createSubscriptionInvoice($handle, $body)

Create invoice ondemand for subscription



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle
$body = new \Swagger\Client\Model\CreateSubscriptionInvoice(); // \Swagger\Client\Model\CreateSubscriptionInvoice | 

try {
    $result = $api_instance->createSubscriptionInvoice($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->createSubscriptionInvoice: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **body** | [**\Swagger\Client\Model\CreateSubscriptionInvoice**](../Model/\Swagger\Client\Model\CreateSubscriptionInvoice.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Invoice**](../Model/Invoice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createSubscriptionJson**
> \Swagger\Client\Model\Subscription createSubscriptionJson($body)

Create subscription



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$body = new \Swagger\Client\Model\CreateSubscription(); // \Swagger\Client\Model\CreateSubscription | 

try {
    $result = $api_instance->createSubscriptionJson($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->createSubscriptionJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateSubscription**](../Model/\Swagger\Client\Model\CreateSubscription.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Subscription**](../Model/Subscription.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteSubscriptionDiscount**
> \Swagger\Client\Model\SubscriptionDiscount deleteSubscriptionDiscount($handle, $sd_handle)

Delete subscription discount



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle
$sd_handle = "sd_handle_example"; // string | Subscription discount handle

try {
    $result = $api_instance->deleteSubscriptionDiscount($handle, $sd_handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->deleteSubscriptionDiscount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **sd_handle** | **string**| Subscription discount handle |

### Return type

[**\Swagger\Client\Model\SubscriptionDiscount**](../Model/SubscriptionDiscount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **expire**
> \Swagger\Client\Model\Subscription expire($handle)

Expire subscription



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle

try {
    $result = $api_instance->expire($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->expire: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |

### Return type

[**\Swagger\Client\Model\Subscription**](../Model/Subscription.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSubscription**
> \Swagger\Client\Model\Subscription getSubscription($handle)

Get subscription



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle

try {
    $result = $api_instance->getSubscription($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->getSubscription: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |

### Return type

[**\Swagger\Client\Model\Subscription**](../Model/Subscription.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSubscriptionDiscount**
> \Swagger\Client\Model\SubscriptionDiscount getSubscriptionDiscount($handle, $sd_handle)

Get subscription discount



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle
$sd_handle = "sd_handle_example"; // string | Subscription discount handle

try {
    $result = $api_instance->getSubscriptionDiscount($handle, $sd_handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->getSubscriptionDiscount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **sd_handle** | **string**| Subscription discount handle |

### Return type

[**\Swagger\Client\Model\SubscriptionDiscount**](../Model/SubscriptionDiscount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSubscriptionDiscounts**
> \Swagger\Client\Model\SubscriptionDiscount[] getSubscriptionDiscounts($handle)

Get subscription discounts



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle

try {
    $result = $api_instance->getSubscriptionDiscounts($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->getSubscriptionDiscounts: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |

### Return type

[**\Swagger\Client\Model\SubscriptionDiscount[]**](../Model/SubscriptionDiscount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSubscriptionPaymentMethods**
> \Swagger\Client\Model\PaymentMethods getSubscriptionPaymentMethods($handle)

Get payment methods



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle

try {
    $result = $api_instance->getSubscriptionPaymentMethods($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->getSubscriptionPaymentMethods: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |

### Return type

[**\Swagger\Client\Model\PaymentMethods**](../Model/PaymentMethods.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getSubscriptions**
> \Swagger\Client\Model\SubscriptionSearch getSubscriptions($page, $size, $search, $sort)

Get list of subscriptions



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$page = 1; // int | Page number to get
$size = 20; // int | Page size to use
$search = "search_example"; // string | Optional search expression
$sort = "sort_example"; // string | Optional sorting expression

try {
    $result = $api_instance->getSubscriptions($page, $size, $search, $sort);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->getSubscriptions: ', $e->getMessage(), PHP_EOL;
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

[**\Swagger\Client\Model\SubscriptionSearch**](../Model/SubscriptionSearch.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **intervalAmount**
> \Swagger\Client\Model\IntervalAmount intervalAmount($handle, $from, $to)

Calculate interval amount



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle
$from = "2015-05-30"; // string | From date on the form yyyy-MM-dd
$to = "2015-07-15"; // string | To date on the form yyyy-MM-dd

try {
    $result = $api_instance->intervalAmount($handle, $from, $to);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->intervalAmount: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **from** | **string**| From date on the form yyyy-MM-dd |
 **to** | **string**| To date on the form yyyy-MM-dd |

### Return type

[**\Swagger\Client\Model\IntervalAmount**](../Model/IntervalAmount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **removeAllPaymentMethods**
> \Swagger\Client\Model\PaymentMethods removeAllPaymentMethods($handle)

Remove all payment methods



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle

try {
    $result = $api_instance->removeAllPaymentMethods($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->removeAllPaymentMethods: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |

### Return type

[**\Swagger\Client\Model\PaymentMethods**](../Model/PaymentMethods.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **removePaymentMethod**
> \Swagger\Client\Model\PaymentMethods removePaymentMethod($handle, $method_id)

Remove payment method



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle
$method_id = "method_id_example"; // string | Payment method id

try {
    $result = $api_instance->removePaymentMethod($handle, $method_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->removePaymentMethod: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **method_id** | **string**| Payment method id |

### Return type

[**\Swagger\Client\Model\PaymentMethods**](../Model/PaymentMethods.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **setCardPaymentMethodJson**
> \Swagger\Client\Model\PaymentMethods setCardPaymentMethodJson($handle, $body)

Set card payment method



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle
$body = new \Swagger\Client\Model\SetCardPaymentMethod(); // \Swagger\Client\Model\SetCardPaymentMethod | 

try {
    $result = $api_instance->setCardPaymentMethodJson($handle, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->setCardPaymentMethodJson: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |
 **body** | [**\Swagger\Client\Model\SetCardPaymentMethod**](../Model/\Swagger\Client\Model\SetCardPaymentMethod.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\PaymentMethods**](../Model/PaymentMethods.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **uncancel**
> \Swagger\Client\Model\Subscription uncancel($handle)

Uncancel subscription



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\SubscriptionApi();
$handle = "handle_example"; // string | Subscription handle

try {
    $result = $api_instance->uncancel($handle);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionApi->uncancel: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **handle** | **string**| Subscription handle |

### Return type

[**\Swagger\Client\Model\Subscription**](../Model/Subscription.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

