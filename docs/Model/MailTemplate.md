# MailTemplate

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**disabled** | **bool** | Should this email be sent by Reepay | [default to false]
**subject** | **string** | Mail subject | 
**cc** | **string[]** | Optional cc addresses in RFC-822 format | [optional] 
**updated** | [**\DateTime**](\DateTime.md) | Date and time for last template update | [optional] 
**mail_from** | **string** | Sender address to use in RFC-822 format. If not set the default account mail settings sender address will be used. | 
**text_body** | **string** | Text body template content | 
**html_body** | **string** | HTML body template content | 
**mail_type** | **string** | Mail type, one of the following: &#x60;invoice_card_receipt&#x60;, &#x60;invoice_manual_receipt&#x60;, &#x60;invoice_zero_amount_receipt&#x60;, &#x60;invoice_dunning_notification&#x60;, &#x60;invoice_dunning_notification_no_payment_method&#x60;, &#x60;signup_receipt&#x60;, &#39;signup_receipt_request_payment_method&#39;,&#x60;subscription_cancelled&#x60;, &#x60;subscription_uncancelled&#x60;, &#x60;subscription_expired&#x60;, &#x60;subscription_expired_dunning&#x60;, &#x60;subscription_change&#x60;, &#x60;subscription_renewal_reminder&#x60;, &#x60;subscription_trial_end_reminder&#x60;, &#x60;user_account_invite&#x60;, &#x60;user_account_notification&#x60;, &#x60;user_reset_password&#x60; | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


