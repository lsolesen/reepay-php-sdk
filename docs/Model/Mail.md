# Mail

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique mail id assigned by Reepay | 
**state** | **string** | The mail state one of the following: &#x60;pending&#x60;, &#x60;error&#x60;, &#x60;disabled&#x60;, &#x60;rejected&#x60;, &#x60;sent&#x60;, &#x60;not_allowed&#x60;, &#x60;no_recipient&#x60; | 
**customer** | **string** | Customer handle | [optional] 
**subscription** | **string** | Subscription handle | [optional] 
**invoice** | **string** | Invoice id | [optional] 
**created** | [**\DateTime**](\DateTime.md) | When the mail was created, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | 
**sent** | [**\DateTime**](\DateTime.md) | When the mail was sent to mail gateway, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**events** | [**\Swagger\Client\Model\MailEvent[]**](MailEvent.md) | List of events for mail | 
**from** | **string** | From address | 
**to** | **string[]** | List of To addresses | 
**cc** | **string[]** | List of Cc addresses | [optional] 
**bcc** | **string[]** | List of Bcc addresses | [optional] 
**subject** | **string** | Subject | 
**text** | **string** | Text content | [optional] 
**html** | **string** | HTML content | [optional] 
**mail_type** | **string** | The mail type (see documentation) | 
**last_send_error** | [**\DateTime**](\DateTime.md) | When sending failed last, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**first_send_error** | [**\DateTime**](\DateTime.md) | When sending failed the first time, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**reply_to** | **string** | Reply-To address | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


