# Swagger\Client\UserApi

All URIs are relative to *https://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteUser**](UserApi.md#deleteUser) | **DELETE** /v1/user/{id} | Delete user
[**getUser**](UserApi.md#getUser) | **GET** /v1/user/{id} | Get user
[**getUsers**](UserApi.md#getUsers) | **GET** /v1/user | Get users
[**inviteUser**](UserApi.md#inviteUser) | **POST** /v1/user/invite | Invite user
[**inviteUserAccept**](UserApi.md#inviteUserAccept) | **POST** /v1/user/invite/{token} | Accept invite
[**inviteUserGet**](UserApi.md#inviteUserGet) | **GET** /v1/user/invite/{token} | Get invite
[**resetPassword**](UserApi.md#resetPassword) | **POST** /v1/user/reset_password | Reset password request
[**resetPasswordWithToken**](UserApi.md#resetPasswordWithToken) | **POST** /v1/user/reset_password/{token} | Reset password
[**updateAuth**](UserApi.md#updateAuth) | **PUT** /v1/user/{id}/groups | Update user groups
[**updatePassword**](UserApi.md#updatePassword) | **PUT** /v1/user/{id}/password | Change password
[**updateUser**](UserApi.md#updateUser) | **PUT** /v1/user/{id} | Update user
[**verifyEmail**](UserApi.md#verifyEmail) | **POST** /v1/user/verify_email/{token} | Verify email
[**verifyEmailRequest**](UserApi.md#verifyEmailRequest) | **POST** /v1/user/{id}/verify_email | Send verification email


# **deleteUser**
> deleteUser($id)

Delete user



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$id = "id_example"; // string | User id

try {
    $api_instance->deleteUser($id);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| User id |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getUser**
> \Swagger\Client\Model\UserAccount getUser($id)

Get user



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$id = "id_example"; // string | User id

try {
    $result = $api_instance->getUser($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->getUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| User id |

### Return type

[**\Swagger\Client\Model\UserAccount**](../Model/UserAccount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getUsers**
> \Swagger\Client\Model\UserAccount[] getUsers()

Get users



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();

try {
    $result = $api_instance->getUsers();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->getUsers: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\UserAccount[]**](../Model/UserAccount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **inviteUser**
> \Swagger\Client\Model\UserAccount inviteUser($body)

Invite user



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$body = new \Swagger\Client\Model\InviteUser(); // \Swagger\Client\Model\InviteUser | 

try {
    $result = $api_instance->inviteUser($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->inviteUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\InviteUser**](../Model/\Swagger\Client\Model\InviteUser.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\UserAccount**](../Model/UserAccount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **inviteUserAccept**
> \Swagger\Client\Model\UserAccount inviteUserAccept($token, $body)

Accept invite



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$token = "token_example"; // string | Invite token
$body = new \Swagger\Client\Model\InviteUserAccept(); // \Swagger\Client\Model\InviteUserAccept | 

try {
    $result = $api_instance->inviteUserAccept($token, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->inviteUserAccept: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **string**| Invite token |
 **body** | [**\Swagger\Client\Model\InviteUserAccept**](../Model/\Swagger\Client\Model\InviteUserAccept.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\UserAccount**](../Model/UserAccount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **inviteUserGet**
> \Swagger\Client\Model\UserAccount inviteUserGet($token)

Get invite



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$token = "token_example"; // string | Invite token

try {
    $result = $api_instance->inviteUserGet($token);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->inviteUserGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **string**| Invite token |

### Return type

[**\Swagger\Client\Model\UserAccount**](../Model/UserAccount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **resetPassword**
> resetPassword($body)

Reset password request



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$body = new \Swagger\Client\Model\UserResetRequestPassword(); // \Swagger\Client\Model\UserResetRequestPassword | 

try {
    $api_instance->resetPassword($body);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->resetPassword: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\UserResetRequestPassword**](../Model/\Swagger\Client\Model\UserResetRequestPassword.md)|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **resetPasswordWithToken**
> \Swagger\Client\Model\User resetPasswordWithToken($token, $body)

Reset password



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$token = "token_example"; // string | Reset password token
$body = new \Swagger\Client\Model\UpdateUserPassword(); // \Swagger\Client\Model\UpdateUserPassword | 

try {
    $result = $api_instance->resetPasswordWithToken($token, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->resetPasswordWithToken: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **string**| Reset password token |
 **body** | [**\Swagger\Client\Model\UpdateUserPassword**](../Model/\Swagger\Client\Model\UpdateUserPassword.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\User**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateAuth**
> \Swagger\Client\Model\UserAccount updateAuth($id, $body)

Update user groups



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$id = "id_example"; // string | User id
$body = new \Swagger\Client\Model\UpdateUserGroups(); // \Swagger\Client\Model\UpdateUserGroups | 

try {
    $result = $api_instance->updateAuth($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->updateAuth: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| User id |
 **body** | [**\Swagger\Client\Model\UpdateUserGroups**](../Model/\Swagger\Client\Model\UpdateUserGroups.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\UserAccount**](../Model/UserAccount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updatePassword**
> \Swagger\Client\Model\UserAccount updatePassword($id, $body)

Change password



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$id = "id_example"; // string | User id
$body = new \Swagger\Client\Model\UpdateUserPassword(); // \Swagger\Client\Model\UpdateUserPassword | 

try {
    $result = $api_instance->updatePassword($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->updatePassword: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| User id |
 **body** | [**\Swagger\Client\Model\UpdateUserPassword**](../Model/\Swagger\Client\Model\UpdateUserPassword.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\UserAccount**](../Model/UserAccount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateUser**
> \Swagger\Client\Model\UserAccount updateUser($id, $body)

Update user



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$id = "id_example"; // string | User id
$body = new \Swagger\Client\Model\UpdateUser(); // \Swagger\Client\Model\UpdateUser | 

try {
    $result = $api_instance->updateUser($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->updateUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| User id |
 **body** | [**\Swagger\Client\Model\UpdateUser**](../Model/\Swagger\Client\Model\UpdateUser.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\UserAccount**](../Model/UserAccount.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **verifyEmail**
> \Swagger\Client\Model\User verifyEmail($token)

Verify email



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$token = "token_example"; // string | Verify email token

try {
    $result = $api_instance->verifyEmail($token);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->verifyEmail: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **string**| Verify email token |

### Return type

[**\Swagger\Client\Model\User**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **verifyEmailRequest**
> verifyEmailRequest($id)

Send verification email



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\UserApi();
$id = "id_example"; // string | User id

try {
    $api_instance->verifyEmailRequest($id);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->verifyEmailRequest: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**| User id |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

