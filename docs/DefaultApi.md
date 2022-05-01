# \DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**IsPhoneRegPost**](DefaultApi.md#IsPhoneRegPost) | **Post** /IsPhoneReg | 检查手机号是否注册
[**JuguguLoginCodeandReturnInfoPost**](DefaultApi.md#JuguguLoginCodeandReturnInfoPost) | **Post** /Jugugu_LoginCodeandReturnInfo | ①获取验证码图片
[**JugugugRegAndVerifyandReturnInfoPost**](DefaultApi.md#JugugugRegAndVerifyandReturnInfoPost) | **Post** /Jugugug_RegAndVerifyandReturnInfo | ③注册Jugugu



## IsPhoneRegPost

> InlineResponse200 IsPhoneRegPost(ctx, optional)

检查手机号是否注册

检查手机号是否注册，返回“true”和“false”字符串

### Required Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***IsPhoneRegPostOpts** | optional parameters | nil if no parameters

### Optional Parameters

Optional parameters are passed through a pointer to a IsPhoneRegPostOpts struct


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject** | [**optional.Interface of InlineObject**](InlineObject.md)|  | 

### Return type

[**InlineResponse200**](inline_response_200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: */*

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## JuguguLoginCodeandReturnInfoPost

> InlineResponse2001 JuguguLoginCodeandReturnInfoPost(ctx, optional)

①获取验证码图片

获取用于防御机器人的验证码图片，phone的传参必须为空字符串

### Required Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***JuguguLoginCodeandReturnInfoPostOpts** | optional parameters | nil if no parameters

### Optional Parameters

Optional parameters are passed through a pointer to a JuguguLoginCodeandReturnInfoPostOpts struct


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject2** | [**optional.Interface of InlineObject2**](InlineObject2.md)|  | 

### Return type

[**InlineResponse2001**](inline_response_200_1.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## JugugugRegAndVerifyandReturnInfoPost

> InlineResponse2001 JugugugRegAndVerifyandReturnInfoPost(ctx, optional)

③注册Jugugu

注册jugugu，注意三点 1.phone的传参必须为11位的国内手机号。 2.robotcodeid和robotcode是通过【①】获得 3.code短信验证码通过【②】 4.paymentpassword区块链短密钥，该密钥为用户进行链上交互使用，密钥设置长度>9位，且包含0-1 A-B a-b 已经特殊字符[~!@#$%^&*?_+;',./\\|·！￥（）{}：“《》？、，。；’”\"《》…-]+

### Required Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***JugugugRegAndVerifyandReturnInfoPostOpts** | optional parameters | nil if no parameters

### Optional Parameters

Optional parameters are passed through a pointer to a JugugugRegAndVerifyandReturnInfoPostOpts struct


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject1** | [**optional.Interface of InlineObject1**](InlineObject1.md)|  | 

### Return type

[**InlineResponse2001**](inline_response_200_1.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

