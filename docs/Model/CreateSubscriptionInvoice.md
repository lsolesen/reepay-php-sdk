# CreateSubscriptionInvoice

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ref** | **string** | Optional reference to avoid double creations. Only one invoice can be created per reference. | [optional] 
**instant** | **bool** | Create and process transaction instantly and only create invoice for successful transaction (default false) | [optional] [default to false]
**due** | **string** | Optional due date and time on the form yyyy-MM-dd, yyyyMMdd, yyyy-MM-ddTHH:mm and yyyy-MM-ddTHH:mm:ss from which the invoice is eligible to be collected | [optional] 
**plan_manual** | **bool** | Create manually for plan by adding plan product as orderline (default false) | [optional] [default to false]
**collect_additional_costs** | **bool** | Collect pending additional costs and transfer to invoice (default true) | [optional] [default to false]
**collect_credit** | **bool** | Collect pending credit and transfer to invoice (default true) | [optional] [default to false]
**apply_discounts** | **bool** | Apply potential discounts for the subscription to the invoice order lines (default true) | [optional] [default to false]
**order_lines** | [**\Swagger\Client\Model\CreateOrderLine[]**](CreateOrderLine.md) | Optional orderlines for the invoice | [optional] 
**manual_transfer** | [**\Swagger\Client\Model\ManualSettleTransfer**](ManualSettleTransfer.md) | Optional manual tranfer. If given the invoice will be settled using the manual transfer transaction. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


