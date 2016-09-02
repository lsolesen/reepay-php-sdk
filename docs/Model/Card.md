# Card

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique id for payment method | 
**state** | **string** | State of the payment method: &#x60;active&#x60;, &#x60;inactivated&#x60; or &#x60;failed&#x60; | 
**customer** | **string** | Customer by handle | 
**failed** | [**\DateTime**](\DateTime.md) | Date when the payment method failed. In ISO-8601 extended offset date-time format. | [optional] 
**created** | [**\DateTime**](\DateTime.md) | Date when the payment method was created. In ISO-8601 extended offset date-time format. | 
**gw_ref** | **string** | Card gateway reference id | 
**card_type** | **string** | Card type | 
**exp_date** | **string** | Card expire date on form MM-YY | [optional] 
**masked_card** | **string** | Masked card number | [optional] 
**last_success** | [**\DateTime**](\DateTime.md) | Date and time of last succesfull use of the card. In ISO-8601 extended offset date-time format. | [optional] 
**last_failed** | [**\DateTime**](\DateTime.md) | Date and time of last failed use of the card. In ISO-8601 extended offset date-time format. | [optional] 
**first_fail** | [**\DateTime**](\DateTime.md) | Date and time of first succesfull use of the card. In ISO-8601 extended offset date-time format. | [optional] 
**error_code** | **string** | An error code from the last failed use of the card | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


