# kubernetes_asyncio.client.ExtensionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_api_group**](ExtensionsApi.md#get_api_group) | **GET** /apis/extensions/ | 


# **get_api_group**
> V1APIGroup get_api_group()



get information of a group

### Example

* Api Key Authentication (BearerToken): 
```python
from __future__ import print_function
import time
import kubernetes_asyncio.client
from kubernetes_asyncio.client.rest import ApiException
from pprint import pprint

# Configure API key authorization: BearerToken
configuration = kubernetes_asyncio.client.Configuration()
configuration.api_key['authorization'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['authorization'] = 'Bearer'

# create an instance of the API class
api_instance = kubernetes_asyncio.client.ExtensionsApi(kubernetes_asyncio.client.ApiClient(configuration))

try:
    api_response = api_instance.get_api_group()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ExtensionsApi->get_api_group: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**V1APIGroup**](V1APIGroup.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

