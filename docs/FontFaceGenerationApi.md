# swagger_client.FontFaceGenerationApi

All URIs are relative to *http://font.rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**font_convert_fontface_schedule_get**](FontFaceGenerationApi.md#font_convert_fontface_schedule_get) | **GET** /font/convert/fontface/schedule | 
[**font_convert_fontface_schedule_put**](FontFaceGenerationApi.md#font_convert_fontface_schedule_put) | **PUT** /font/convert/fontface/schedule | 
[**font_id_convert_fontface_get**](FontFaceGenerationApi.md#font_id_convert_fontface_get) | **GET** /font/{id}/convert/fontface | 

# **font_convert_fontface_schedule_get**
> font_convert_fontface_schedule_get(id)



Get details about the schduled font-face conversion.

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
api_instance = swagger_client.FontFaceGenerationApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Schedule ID

try:
    api_instance.font_convert_fontface_schedule_get(id)
except ApiException as e:
    print("Exception when calling FontFaceGenerationApi->font_convert_fontface_schedule_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Schedule ID | 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_convert_fontface_schedule_put**
> font_convert_fontface_schedule_put(fontid)



Schdule a font-face conversion. If your font file is greater than 2 MB choose the schedule option, since synchronous requests may timeout.

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
api_instance = swagger_client.FontFaceGenerationApi(swagger_client.ApiClient(configuration))
fontid = 'fontid_example' # str | Font ID

try:
    api_instance.font_convert_fontface_schedule_put(fontid)
except ApiException as e:
    print("Exception when calling FontFaceGenerationApi->font_convert_fontface_schedule_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fontid** | **str**| Font ID | 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_id_convert_fontface_get**
> font_id_convert_fontface_get(id, targetformats=targetformats, binaryresult=binaryresult)



Generate @font-face kit of the font and download the result.

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
api_instance = swagger_client.FontFaceGenerationApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID
targetformats = 'targetformats_example' # str | Target formats (comma seperated list) you want to include in font-face kit. Options can include all or some from this list(ttf,woff,woff2,svg,eot). (optional)
binaryresult = false # bool | Return converted file in binary format, the default is base64 json response. (optional) (default to false)

try:
    api_instance.font_id_convert_fontface_get(id, targetformats=targetformats, binaryresult=binaryresult)
except ApiException as e:
    print("Exception when calling FontFaceGenerationApi->font_id_convert_fontface_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Font ID | 
 **targetformats** | **str**| Target formats (comma seperated list) you want to include in font-face kit. Options can include all or some from this list(ttf,woff,woff2,svg,eot). | [optional] 
 **binaryresult** | **bool**| Return converted file in binary format, the default is base64 json response. | [optional] [default to false]

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

