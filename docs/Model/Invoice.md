# Invoice

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Invoice id assigned by Reepay | 
**customer** | **string** | Customer handle | 
**subscription** | **string** | Subscription handle, will be null for a one-time customer invoice | [optional] 
**plan** | **string** | Subscription plan handle for the plan used to automatically create the invoice. Will be null for one-time invoices. | [optional] 
**state** | **string** | The invoice state one of the following: &#x60;pending&#x60;, &#x60;dunning&#x60;, &#x60;settled&#x60;, &#x60;cancelled&#x60;, &#x60;failed&#x60; | 
**amount** | **int** | The invoice amount including VAT | 
**number** | **int** | Sequential invoice number | 
**currency** | **string** | Currency for the account in [ISO 4217](http://da.wikipedia.org/wiki/ISO_4217) three letter alpha code | 
**due** | [**\DateTime**](\DateTime.md) | When is the invoice due, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | 
**failed** | [**\DateTime**](\DateTime.md) | When the invoice failed, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**settled** | [**\DateTime**](\DateTime.md) | When the invoice settled, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**cancelled** | [**\DateTime**](\DateTime.md) | When the invoice was cancelled, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**credits** | [**\Swagger\Client\Model\CreditInvoice[]**](CreditInvoice.md) | Credits applied to invoice | 
**adjustments** | [**\Swagger\Client\Model\InvoiceAdjustment[]**](InvoiceAdjustment.md) | Invoice adjustments | [optional] 
**created** | [**\DateTime**](\DateTime.md) | When the invoice was created, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | 
**plan_version** | **int** | Subscription plan version | [optional] 
**dunning_plan** | **string** | Dunning plan handle | [optional] 
**discount_amount** | **int** | The potential discount amount deducted from the invoice amount including VAT | 
**org_amount** | **int** | The invoice original amount including VAT, may differ from amount if adjustments have been applied for the invoice | 
**amount_vat** | **int** | The invoice vat amount calculated as rounded summed fractional vats for each orderline | 
**amount_ex_vat** | **int** | The invoice amount without vat | 
**settled_amount** | **int** | Settled amount | 
**refunded_amount** | **int** | Refunded amount | 
**period_number** | **int** | The subscription period this invoice is for | [optional] 
**order_lines** | [**\Swagger\Client\Model\OrderLine[]**](OrderLine.md) | Order lines for invoice sorted by descending timestamp | 
**additional_costs** | **string[]** | Additional costs for invoice | 
**card_transactions** | [**\Swagger\Client\Model\CardTransaction[]**](CardTransaction.md) | Invoice card transactions | 
**manual_transactions** | [**\Swagger\Client\Model\ManualTransaction[]**](ManualTransaction.md) | Invoice manual transactions | 
**credit_notes** | [**\Swagger\Client\Model\InvoiceCreditNote[]**](InvoiceCreditNote.md) | Invoice credit notes | [optional] 
**dunning_start** | [**\DateTime**](\DateTime.md) | When dunning for the invoice was started, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**dunning_count** | **int** | Number of dunning events for invoice (number of reminders sent) | [optional] 
**dunning_expired** | [**\DateTime**](\DateTime.md) | When dunning for the invoice expired, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**period_from** | [**\DateTime**](\DateTime.md) | The start of billing period if the invoice is for a specific billing period, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**period_to** | [**\DateTime**](\DateTime.md) | The end of billing period if the invoice is for a specific billing period, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


