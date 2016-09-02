# SupersedeSubscriptionPlan

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the plan | 
**description** | **string** | Description of the plan | [optional] 
**vat** | **float** | Optional vat for this plan. Account default is used if none given. | [optional] 
**amount** | **int** | Amount for the plan in the smallest unit for the account currency including VAT | 
**quantity** | **int** | Optional default quantity of the subscription plan product for new subscriptions. Default is 1. | [optional] 
**prepaid** | **bool** | Subscriptions can either be prepaid where an amount is paid in advance, or the opposite. This setting only relates to handling of pause scenarios. | [default to false]
**dunning_plan** | **string** | Dunning plan handle | [optional] 
**renewal_reminder_email_days** | **int** | Optional renewal reminder email settings. Number of days before next billing to send a reminder email. | [optional] 
**trial_reminder_email_days** | **int** | Optional end of trial reminder email settings. Number of days before end of trial to send a reminder email. | [optional] 
**partial_period_handling** | **string** | How to handle a potential initial partial billing period for fixed day scheduling. The options are to bill for a full period, bill prorated for the partial period, bill a zero amoumt, or not to consider the period before first fixed day a billing period. The default is to bill prorated. Options: &#x60;bill_full&#x60;, &#x60;bill_prorated&#x60;, &#x60;bill_zero_amount&#x60;, &#x60;no_bill&#x60;. | [optional] 
**fixed_count** | **int** | Fixed number of renewals for subscriptions using this plan. Equals the number of scheduled invoices. | [optional] 
**fixed_life_time_unit** | **string** | Time unit use for fixed life time | [optional] 
**fixed_life_time_length** | **int** | Fixed life time length for subscriptions using this plan. E.g. 12 months. Subscriptions will cancel after the fixed life time and expire when the active billing cycle ends. | [optional] 
**trial_interval_unit** | **string** | Time unit for free trial period | [optional] 
**trial_interval_length** | **int** | Free trial interval length. E.g. 1 month. | [optional] 
**interval_length** | **int** | The length of intervals. E.g. every second month or every 14 days. | 
**schedule_type** | **string** | Scheduling type, one of the following: &#x60;manual&#x60;, &#x60;daily&#x60;, &#x60;weekly_fixedday&#x60;, &#x60;month_startdate&#x60;, &#x60;month_fixedday&#x60;, &#x60;month_lastday&#x60;. See documentation for descriptions of the different types. | 
**schedule_fixed_day** | **int** | If a fixed day scheduling type is used a fixed day must be provided. For months the allowed value is 1-28 for weeks it is 1-7 | [optional] 
**base_month** | **int** | For fixed month schedule types the base month can be used to control which months are eligible for start of first billing period. The eligible months are calculated as &#x60;base_month + k * interval_length&#x60; up to 12. E.g. to use quaterly billing in the months jan-apr-jul-oct, base_month 1 and inrerval_length 3 can be used. If not defined the first fixed day will be used as start of first billing period. | [optional] 
**supersede_mode** | **string** | Action to take after a subscription plan is superseded, one of the following: &#x60;no_sub_update&#x60;, &#x60;scheduled_sub_update&#x60;, &#x60;instant_sub_update&#x60;. Default is &#x60;no_sub_update&#x60;. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


