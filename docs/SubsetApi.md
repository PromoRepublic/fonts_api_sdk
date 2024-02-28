# swagger_client.SubsetApi

All URIs are relative to *http://font.rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**font_id_subset_get**](SubsetApi.md#font_id_subset_get) | **GET** /font/{id}/subset | 
[**font_subset_ranges_get**](SubsetApi.md#font_subset_ranges_get) | **GET** /font/subset/ranges | 

# **font_id_subset_get**
> font_id_subset_get(id, glyphs, use_cssrange=use_cssrange, custom_glyphs=custom_glyphs, binaryresult=binaryresult)



Subset the font and download the result.

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
api_instance = swagger_client.SubsetApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID
glyphs = 'glyphs_example' # str | Comma seperated glyph ranges or single glyphs. e.g 0x61-0x7A,0x30-0x39
use_cssrange = false # bool | Affects how the custom_glyphs string is processed. Default is set to false. (optional) (default to false)
custom_glyphs = 'custom_glyphs_example' # str | A literal string whose value will be converted to unicode values. If the paramater use_cssrange is set to true this will be treated as CSS unicode ranges. (optional)
binaryresult = false # bool | Return converted file in binary format, the default is base64 json response. (optional) (default to false)

try:
    api_instance.font_id_subset_get(id, glyphs, use_cssrange=use_cssrange, custom_glyphs=custom_glyphs, binaryresult=binaryresult)
except ApiException as e:
    print("Exception when calling SubsetApi->font_id_subset_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Font ID | 
 **glyphs** | **str**| Comma seperated glyph ranges or single glyphs. e.g 0x61-0x7A,0x30-0x39 | 
 **use_cssrange** | **bool**| Affects how the custom_glyphs string is processed. Default is set to false. | [optional] [default to false]
 **custom_glyphs** | **str**| A literal string whose value will be converted to unicode values. If the paramater use_cssrange is set to true this will be treated as CSS unicode ranges. | [optional] 
 **binaryresult** | **bool**| Return converted file in binary format, the default is base64 json response. | [optional] [default to false]

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_subset_ranges_get**
> font_subset_ranges_get()



Get the subset unicode ranges.

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
api_instance = swagger_client.SubsetApi(swagger_client.ApiClient(configuration))

try:
    api_instance.font_subset_ranges_get()
except ApiException as e:
    print("Exception when calling SubsetApi->font_subset_ranges_get: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

