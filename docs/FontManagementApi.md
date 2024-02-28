# swagger_client.FontManagementApi

All URIs are relative to *http://font.rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**font_delete**](FontManagementApi.md#font_delete) | **DELETE** /font | 
[**font_list_get**](FontManagementApi.md#font_list_get) | **GET** /font/list | 
[**font_post**](FontManagementApi.md#font_post) | **POST** /font | 

# **font_delete**
> font_delete(id)



Delete a Font. 

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: X-EverythingFonts-Api-Secret
configuration = swagger_client.Configuration()
configuration.api_key['X-EverythingFonts-Api-Secret'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-EverythingFonts-Api-Secret'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.FontManagementApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID

try:
    api_instance.font_delete(id)
except ApiException as e:
    print("Exception when calling FontManagementApi->font_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Font ID | 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/xml, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_list_get**
> font_list_get(start=start, public=public)



Get a list of fonts in the system.

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: X-EverythingFonts-Api-Secret
configuration = swagger_client.Configuration()
configuration.api_key['X-EverythingFonts-Api-Secret'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-EverythingFonts-Api-Secret'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.FontManagementApi(swagger_client.ApiClient(configuration))
start = 0 # int | Response is paged. This parameter controls where response starts the listing at (optional) (default to 0)
public = false # bool | Should the public fonts be included in the listing? (optional) (default to false)

try:
    api_instance.font_list_get(start=start, public=public)
except ApiException as e:
    print("Exception when calling FontManagementApi->font_list_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **start** | **int**| Response is paged. This parameter controls where response starts the listing at | [optional] [default to 0]
 **public** | **bool**| Should the public fonts be included in the listing? | [optional] [default to false]

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_post**
> font_post(font=font)



Add a new font to your private collection.

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: X-EverythingFonts-Api-Secret
configuration = swagger_client.Configuration()
configuration.api_key['X-EverythingFonts-Api-Secret'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-EverythingFonts-Api-Secret'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.FontManagementApi(swagger_client.ApiClient(configuration))
font = 'font_example' # str |  (optional)

try:
    api_instance.font_post(font=font)
except ApiException as e:
    print("Exception when calling FontManagementApi->font_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **font** | **str**|  | [optional] 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

