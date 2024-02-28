# swagger_client.HintingApi

All URIs are relative to *http://font.rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**font_id_hint_get**](HintingApi.md#font_id_hint_get) | **GET** /font/{id}/hint | 

# **font_id_hint_get**
> font_id_hint_get(id, type, hintcomponsites=hintcomponsites, adjustsubglyphs=adjustsubglyphs, binaryresult=binaryresult)



Hint the font and download the result.

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
api_instance = swagger_client.HintingApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID
type = 'type_example' # str | Hinting type(directwire/windows-gdi/grayscale/remove)
hintcomponsites = true # bool | Should hint composite glyphs? (optional) (default to true)
adjustsubglyphs = true # bool | Should adjust sub glyphs? (optional) (default to true)
binaryresult = false # bool | Return converted file in binary format, the default is base64 json response. (optional) (default to false)

try:
    api_instance.font_id_hint_get(id, type, hintcomponsites=hintcomponsites, adjustsubglyphs=adjustsubglyphs, binaryresult=binaryresult)
except ApiException as e:
    print("Exception when calling HintingApi->font_id_hint_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Font ID | 
 **type** | **str**| Hinting type(directwire/windows-gdi/grayscale/remove) | 
 **hintcomponsites** | **bool**| Should hint composite glyphs? | [optional] [default to true]
 **adjustsubglyphs** | **bool**| Should adjust sub glyphs? | [optional] [default to true]
 **binaryresult** | **bool**| Return converted file in binary format, the default is base64 json response. | [optional] [default to false]

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

