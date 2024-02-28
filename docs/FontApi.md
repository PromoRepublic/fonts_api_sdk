# swagger_client.FontApi

All URIs are relative to *http://font.rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**font_fontid_glyph_id_get**](FontApi.md#font_fontid_glyph_id_get) | **GET** /font/{fontid}/glyph/{id} | 
[**font_fontid_glyph_id_image_get**](FontApi.md#font_fontid_glyph_id_image_get) | **GET** /font/{fontid}/glyph/{id}/image | 
[**font_fontid_glyph_list_get**](FontApi.md#font_fontid_glyph_list_get) | **GET** /font/{fontid}/glyph/list | 
[**font_get**](FontApi.md#font_get) | **GET** /font | 
[**font_id_coverage_get**](FontApi.md#font_id_coverage_get) | **GET** /font/{id}/coverage | 
[**font_id_file_fileid_get**](FontApi.md#font_id_file_fileid_get) | **GET** /font/{id}/file/{fileid} | 
[**font_id_files_get**](FontApi.md#font_id_files_get) | **GET** /font/{id}/files | 
[**font_id_get**](FontApi.md#font_id_get) | **GET** /font/{id} | 
[**font_id_image_get**](FontApi.md#font_id_image_get) | **GET** /font/{id}/image | 
[**font_id_license_get**](FontApi.md#font_id_license_get) | **GET** /font/{id}/license | 
[**font_id_name_get**](FontApi.md#font_id_name_get) | **GET** /font/{id}/name | 

# **font_fontid_glyph_id_get**
> font_fontid_glyph_id_get(fontid, id)



Get the details about a single glyph.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
fontid = 'fontid_example' # str | Font ID
id = 'id_example' # str | Glyph ID

try:
    api_instance.font_fontid_glyph_id_get(fontid, id)
except ApiException as e:
    print("Exception when calling FontApi->font_fontid_glyph_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fontid** | **str**| Font ID | 
 **id** | **str**| Glyph ID | 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_fontid_glyph_id_image_get**
> font_fontid_glyph_id_image_get(fontid, id, format)



Get the image of a single glyph.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
fontid = 'fontid_example' # str | Font ID
id = 'id_example' # str | Glyph ID
format = 'format_example' # str | Format of the image returned

try:
    api_instance.font_fontid_glyph_id_image_get(fontid, id, format)
except ApiException as e:
    print("Exception when calling FontApi->font_fontid_glyph_id_image_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fontid** | **str**| Font ID | 
 **id** | **str**| Glyph ID | 
 **format** | **str**| Format of the image returned | 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_fontid_glyph_list_get**
> font_fontid_glyph_list_get(fontid)



Get the details about all the glyphs of the font(browse).

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
fontid = 'fontid_example' # str | Font ID

try:
    api_instance.font_fontid_glyph_list_get(fontid)
except ApiException as e:
    print("Exception when calling FontApi->font_fontid_glyph_list_get: %s\n" % e)
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

# **font_get**
> font_get(id=id)



Gets a `Font` with a given `id`.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID (optional)

try:
    api_instance.font_get(id=id)
except ApiException as e:
    print("Exception when calling FontApi->font_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Font ID | [optional] 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_id_coverage_get**
> font_id_coverage_get(id)



Get the unicode coverage of the font.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID

try:
    api_instance.font_id_coverage_get(id)
except ApiException as e:
    print("Exception when calling FontApi->font_id_coverage_get: %s\n" % e)
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
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_id_file_fileid_get**
> font_id_file_fileid_get(id, fileid)



Get the details about a single font file associated with the font.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID
fileid = 'fileid_example' # str | File ID

try:
    api_instance.font_id_file_fileid_get(id, fileid)
except ApiException as e:
    print("Exception when calling FontApi->font_id_file_fileid_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Font ID | 
 **fileid** | **str**| File ID | 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_id_files_get**
> font_id_files_get(id)



Get the files associated with the font.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID

try:
    api_instance.font_id_files_get(id)
except ApiException as e:
    print("Exception when calling FontApi->font_id_files_get: %s\n" % e)
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
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_id_get**
> font_id_get(id)



Get the metadata details of the font.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID

try:
    api_instance.font_id_get(id)
except ApiException as e:
    print("Exception when calling FontApi->font_id_get: %s\n" % e)
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
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_id_image_get**
> font_id_image_get(id, type)



Get the details about a single font file associated with the font.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID
type = 'type_example' # str | Font preview type. Must be one of the following values: preview/bigpreview/waterfall/contact

try:
    api_instance.font_id_image_get(id, type)
except ApiException as e:
    print("Exception when calling FontApi->font_id_image_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Font ID | 
 **type** | **str**| Font preview type. Must be one of the following values: preview/bigpreview/waterfall/contact | 

### Return type

void (empty response body)

### Authorization

[X-EverythingFonts-Api-Secret](../README.md#X-EverythingFonts-Api-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_id_license_get**
> font_id_license_get(id)



Get the license text of the font.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID

try:
    api_instance.font_id_license_get(id)
except ApiException as e:
    print("Exception when calling FontApi->font_id_license_get: %s\n" % e)
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
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **font_id_name_get**
> font_id_name_get(id)



Get the name of the font.

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
api_instance = swagger_client.FontApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | Font ID

try:
    api_instance.font_id_name_get(id)
except ApiException as e:
    print("Exception when calling FontApi->font_id_name_get: %s\n" % e)
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
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

