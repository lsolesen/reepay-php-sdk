# Swagger\Client\OrganisationApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getOrganisation**](OrganisationApi.md#getOrganisation) | **GET** /v1/organisation | Get organisation
[**update**](OrganisationApi.md#update) | **PUT** /v1/organisation | Update organisation


# **getOrganisation**
> \Swagger\Client\Model\Organisation getOrganisation()

Get organisation



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\OrganisationApi();

try {
    $result = $api_instance->getOrganisation();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrganisationApi->getOrganisation: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\Organisation**](../Model/Organisation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **update**
> \Swagger\Client\Model\Organisation update($body)

Update organisation



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\OrganisationApi();
$body = new \Swagger\Client\Model\UpdateOrganisation(); // \Swagger\Client\Model\UpdateOrganisation | 

try {
    $result = $api_instance->update($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrganisationApi->update: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\UpdateOrganisation**](../Model/\Swagger\Client\Model\UpdateOrganisation.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Organisation**](../Model/Organisation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

