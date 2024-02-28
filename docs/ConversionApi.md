# swagger_client.ConversionApi

All URIs are relative to *http://font.rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**font_convert_schedule_get**](ConversionApi.md#font_convert_schedule_get) | **GET** /font/convert/schedule | 
[**font_convert_schedule_put**](ConversionApi.md#font_convert_schedule_put) | **PUT** /font/convert/schedule | 
[**font_convert_targets_get**](ConversionApi.md#font_convert_targets_get) | **GET** /font/convert/targets | 
[**font_id_convert_get**](ConversionApi.md#font_id_convert_get) | **GET** /font/{id}/convert | 

# **font_convert_schedule_get**
> font_convert_schedule_get(id)



Get details about the schduled font conversion.

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
api_instance = swagger_client.ConversionApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Schedule ID

try:
    api_instance.font_convert_schedule_get(id)
except ApiException as e:
    print("Exception when calling ConversionApi->font_convert_schedule_get: %s\n" % e)
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

# **font_convert_schedule_put**
> font_convert_schedule_put(fontid, targetformat)



Schdule a font conversion. If your font file is greater than 2 MB choose the schedule option, since synchronous requests may timeout.

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
api_instance = swagger_client.ConversionApi(swagger_client.ApiClient(configuration))
fontid = 'fontid_example' # str | Font ID
targetformat = 'targetformat_example' # str | Target Format to convert to 

try:
    api_instance.font_convert_schedule_put(fontid, targetformat)
except ApiException as e:
    print("Exception when calling ConversionApi->font_convert_schedule_put: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fontid** | **str**| Font ID | 
 **targetformat** | **str**| Target Format to convert to  | 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_convert_targets_get**
> font_convert_targets_get(sourceformat)



Get the possible conversion targets for a given source format.

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
api_instance = swagger_client.ConversionApi(swagger_client.ApiClient(configuration))
sourceformat = 'sourceformat_example' # str | Source Format

try:
    api_instance.font_convert_targets_get(sourceformat)
except ApiException as e:
    print("Exception when calling ConversionApi->font_convert_targets_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sourceformat** | **str**| Source Format | 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_id_convert_get**
> font_id_convert_get(id, targetformat, binaryresult=binaryresult)



Convert the font to the target format and download the result.

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
api_instance = swagger_client.ConversionApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID
targetformat = 'targetformat_example' # str | Target format you want to convert to
binaryresult = false # bool | Return converted file in binary format, the default is base64 json response. (optional) (default to false)

try:
    api_instance.font_id_convert_get(id, targetformat, binaryresult=binaryresult)
except ApiException as e:
    print("Exception when calling ConversionApi->font_id_convert_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Font ID | 
 **targetformat** | **str**| Target format you want to convert to | 
 **binaryresult** | **bool**| Return converted file in binary format, the default is base64 json response. | [optional] [default to false]

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

