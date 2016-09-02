# Swagger\Client\AgreementApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createCardGatewayAgreement**](AgreementApi.md#createCardGatewayAgreement) | **POST** /v1/agreement/card_gateway | Create card gateway agreement
[**deleteCardGatewayAgreement**](AgreementApi.md#deleteCardGatewayAgreement) | **DELETE** /v1/agreement/card_gateway/{id} | Delete card gateway agreement
[**getCardGatewayAgreement**](AgreementApi.md#getCardGatewayAgreement) | **GET** /v1/agreement/card_gateway/{id} | Get card gateway agreement
[**getCardGatewayAgreements**](AgreementApi.md#getCardGatewayAgreements) | **GET** /v1/agreement/card_gateway | Get all card gateway agreements
[**updateCardGatewayAgreement**](AgreementApi.md#updateCardGatewayAgreement) | **PUT** /v1/agreement/card_gateway/{id} | Update card gateway agreement


# **createCardGatewayAgreement**
> \Swagger\Client\Model\CardGatewayAgreement createCardGatewayAgreement($body)

Create card gateway agreement



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AgreementApi();
$body = new \Swagger\Client\Model\CreateCardGatewayAgreement(); // \Swagger\Client\Model\CreateCardGatewayAgreement | 

try {
    $result = $api_instance->createCardGatewayAgreement($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AgreementApi->createCardGatewayAgreement: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CreateCardGatewayAgreement**](../Model/\Swagger\Client\Model\CreateCardGatewayAgreement.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\CardGatewayAgreement**](../Model/CardGatewayAgreement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteCardGatewayAgreement**
> \Swagger\Client\Model\CardGatewayAgreement deleteCardGatewayAgreement($id)

Delete card gateway agreement



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AgreementApi();
$id = "id_example"; // string | Agreement id

try {
    $result = $api_instance->deleteCardGatewayAgreement($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AgreementApi->deleteCardGatewayAgreement: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Agreement id |

### Return type

[**\Swagger\Client\Model\CardGatewayAgreement**](../Model/CardGatewayAgreement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCardGatewayAgreement**
> \Swagger\Client\Model\CardGatewayAgreement getCardGatewayAgreement($id)

Get card gateway agreement



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AgreementApi();
$id = "id_example"; // string | Agreement id

try {
    $result = $api_instance->getCardGatewayAgreement($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AgreementApi->getCardGatewayAgreement: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Agreement id |

### Return type

[**\Swagger\Client\Model\CardGatewayAgreement**](../Model/CardGatewayAgreement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getCardGatewayAgreements**
> \Swagger\Client\Model\CardGatewayAgreement[] getCardGatewayAgreements($only_active)

Get all card gateway agreements



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AgreementApi();
$only_active = false; // bool | 

try {
    $result = $api_instance->getCardGatewayAgreements($only_active);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AgreementApi->getCardGatewayAgreements: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **only_active** | **bool**|  | [optional] [default to false]

### Return type

[**\Swagger\Client\Model\CardGatewayAgreement[]**](../Model/CardGatewayAgreement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateCardGatewayAgreement**
> \Swagger\Client\Model\CardGatewayAgreement updateCardGatewayAgreement($id, $body)

Update card gateway agreement



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AgreementApi();
$id = "id_example"; // string | Agreement id
$body = new \Swagger\Client\Model\UpdateCardGatewayAgreement(); // \Swagger\Client\Model\UpdateCardGatewayAgreement | 

try {
    $result = $api_instance->updateCardGatewayAgreement($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AgreementApi->updateCardGatewayAgreement: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| Agreement id |
 **body** | [**\Swagger\Client\Model\UpdateCardGatewayAgreement**](../Model/\Swagger\Client\Model\UpdateCardGatewayAgreement.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\CardGatewayAgreement**](../Model/CardGatewayAgreement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

