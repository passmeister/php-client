# Swagger\Client\PassApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createOrUpdatePass**](PassApi.md#createOrUpdatePass) | **POST** /pass | This method creates or (if the pass id already exists) updates a pass, so you don&#39;t have to track ids and creation status of your passes.
[**deletePass**](PassApi.md#deletePass) | **DELETE** /pass | Delete pass by pass id.
[**getPass**](PassApi.md#getPass) | **GET** /pass | Get pass information by pass id.
[**passList**](PassApi.md#passList) | **GET** /pass/list | Retrieve the list of active pass ids for a given pass type.
[**passSync**](PassApi.md#passSync) | **POST** /pass/sync | Send updates to all active passes for a given pass type.


# **createOrUpdatePass**
> createOrUpdatePass($pass_type_id, $pass_id)

This method creates or (if the pass id already exists) updates a pass, so you don't have to track ids and creation status of your passes.

This method creates or (if the pass id already exists) updates a pass, so you don't have to track ids and creation status of your passes.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\PassApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$pass_type_id = new \stdClass; // object | your pass type id, for example P963493 (Urban Fitness)
$pass_id = new \stdClass; // object | id of the pass (provided by you when creating the pass or automatically set by passmeister)

try {
    $apiInstance->createOrUpdatePass($pass_type_id, $pass_id);
} catch (Exception $e) {
    echo 'Exception when calling PassApi->createOrUpdatePass: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pass_type_id** | [**object**](../Model/.md)| your pass type id, for example P963493 (Urban Fitness) |
 **pass_id** | [**object**](../Model/.md)| id of the pass (provided by you when creating the pass or automatically set by passmeister) | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deletePass**
> deletePass($pass_type_id, $pass_id)

Delete pass by pass id.

Delete pass by pass id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\PassApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$pass_type_id = new \stdClass; // object | your pass type id, for example P963493 (Urban Fitness)
$pass_id = new \stdClass; // object | id of the pass

try {
    $apiInstance->deletePass($pass_type_id, $pass_id);
} catch (Exception $e) {
    echo 'Exception when calling PassApi->deletePass: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pass_type_id** | [**object**](../Model/.md)| your pass type id, for example P963493 (Urban Fitness) |
 **pass_id** | [**object**](../Model/.md)| id of the pass |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getPass**
> getPass($pass_type_id, $pass_id)

Get pass information by pass id.

Get pass information by pass id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\PassApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$pass_type_id = new \stdClass; // object | your pass type id, for example P963493 (Urban Fitness)
$pass_id = new \stdClass; // object | id of the pass

try {
    $apiInstance->getPass($pass_type_id, $pass_id);
} catch (Exception $e) {
    echo 'Exception when calling PassApi->getPass: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pass_type_id** | [**object**](../Model/.md)| your pass type id, for example P963493 (Urban Fitness) |
 **pass_id** | [**object**](../Model/.md)| id of the pass |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **passList**
> passList($pass_type_id, $page, $limit)

Retrieve the list of active pass ids for a given pass type.

Retrieve the list of active pass ids for a given pass type.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\PassApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$pass_type_id = new \stdClass; // object | your pass type id, for example P963493 (Urban Fitness)
$page = new \stdClass; // object | 
$limit = new \stdClass; // object | 

try {
    $apiInstance->passList($pass_type_id, $page, $limit);
} catch (Exception $e) {
    echo 'Exception when calling PassApi->passList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pass_type_id** | [**object**](../Model/.md)| your pass type id, for example P963493 (Urban Fitness) |
 **page** | [**object**](../Model/.md)|  | [optional]
 **limit** | [**object**](../Model/.md)|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **passSync**
> passSync($pass_type_id)

Send updates to all active passes for a given pass type.

For example: you changed the pass type layout and now you want to update all installed passes. (The API call only confirms the scheduling of the updates, actual updating of passes on your customers devices can take a while.)

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\PassApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$pass_type_id = new \stdClass; // object | your pass type id, for example P963493 (Urban Fitness)

try {
    $apiInstance->passSync($pass_type_id);
} catch (Exception $e) {
    echo 'Exception when calling PassApi->passSync: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pass_type_id** | [**object**](../Model/.md)| your pass type id, for example P963493 (Urban Fitness) |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

