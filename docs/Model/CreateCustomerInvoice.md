# CreateCustomerInvoice

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ref** | **string** | Optional reference to avoid double creations. Only one invoice can be created per reference. | [optional] 
**order_lines** | [**\Swagger\Client\Model\CreateOrderLine[]**](CreateOrderLine.md) | Orderlines for the invoice | 
**manual_transfer** | [**\Swagger\Client\Model\ManualSettleTransfer**](ManualSettleTransfer.md) | Optional manual tranfer. If given the invoice will be settled using the manual transfer transaction. | [optional] 
**payment_method** | **string** | Payment method id to use for invoice. Must be provided if no manual transfer is given. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


