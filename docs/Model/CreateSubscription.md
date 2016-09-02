# CreateSubscription

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer** | **string** | Customer handle | 
**plan** | **string** | Plan handle | 
**amount** | **int** | Optional custom per quantity plan price including VAT. If provided the plan price billed for each billing period will be overridden by this price. | [optional] 
**quantity** | **int** | Optional quantity of the plan product for this subscription. If not provided the default is the default plan quantity defined for the plan. | [optional] 
**test** | **bool** | Test flag. If given it will be verified that the account state matches the intended create state. | [optional] [default to false]
**handle** | **string** | Per account unique handle for the subscription. Max length 255 with allowable characters [a-zA-Z0-9_.-@]. Must be provided if generate_handle not defined. | [optional] 
**card** | **string** | If signup method &#39;card&#39; is used a card id of an existing card must be provided | [optional] 
**signup_method** | **string** | The signup method, how to get the payment information from customer, one of the following: &#x60;card&#x60;, &#x60;card_token&#x60;, &#x60;email&#x60;, &#x60;link&#x60; | 
**conditional_create** | **bool** | If the subscription is eligable to bill for the first period right away, this option will make the creation conditional on a successfull payment of the first invoice. Will require a signup method of &#x60;card&#x60; or &#x60;card_token&#x60;. Default is false. | [optional] [default to false]
**plan_version** | **int** | Optional plan version, default is to use newest version of plan | [optional] 
**generate_handle** | **bool** | Auto generate handle on the form sub-[sequence_number] | [optional] [default to false]
**start_date** | **string** | Date and time on the form &#x60;yyyy-MM-dd&#x60;, &#x60;yyyyMMdd&#x60;, &#x60;yyyy-MM-ddTHH:mm&#x60; and &#x60;yyyy-MM-ddTHH:mm:ss&#x60; from which the subscription is eligible to schedule first invoice. If no time part is given start of day will be used. A start date in the past can be used, but no more than one period length in the past. A start date in tje past can result in an instant invoice for a past billing period start. Default value is current date and time. | [optional] 
**end_date** | **string** | Fixed date and time on the form &#x60;yyyy-MM-dd&#x60;, &#x60;yyyyMMdd&#x60;, &#x60;yyyy-MM-ddTHH:mm&#x60; and &#x60;yyyy-MM-ddTHH:mm:ss&#x60; where the subscription will automatically cancel. The subscription will expire at the end of the billing period containing the end date. Default is no fixed end date. | [optional] 
**grace_duration** | **int** | A grace duration in seconds from the creation of a subscription where no dunning process is started for a failing invoice. This allows a certain amount of time for the customer to sign up with a payment method. | [optional] 
**card_token** | **string** | If signup method &#39;card_token&#39; is used a card token must be provided | [optional] 
**no_trial** | **bool** | Override plan trial settings and disable trial | [optional] [default to false]
**subscription_discounts** | [**\Swagger\Client\Model\CreateSubscriptionDiscount[]**](CreateSubscriptionDiscount.md) | Discounts to attach to subscription | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


