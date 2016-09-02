# CardTransaction

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Transaction id assigned by Reepay | 
**state** | **string** | State of the transaction, one of the following: &#x60;pending&#x60;, &#x60;processing&#x60;, &#x60;settled&#x60;, &#x60;refunded&#x60;, &#x60;failed&#x60;, &#x60;cancelled&#x60; | 
**invoice** | **string** | Invoice id | 
**type** | **string** | Transaction type, one of the following: &#39;settle&#39;, &#39;refund&#39; | 
**amount** | **int** | The transaction amount | 
**settled** | [**\DateTime**](\DateTime.md) | When the transaction was settled, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | 
**failed** | [**\DateTime**](\DateTime.md) | When the transaction failed, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | 
**refunded** | [**\DateTime**](\DateTime.md) | When the transaction was refunded, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | 
**created** | [**\DateTime**](\DateTime.md) | Date when the transaction was created. In [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | 
**card** | [**\Swagger\Client\Model\Card**](Card.md) | Card used for transaction | 
**error** | **string** | Error code if failed | [optional] 
**ref_transaction** | **string** | Id of a possible referenced transaction | [optional] 
**gw_id** | **string** | Gateway id for card | [optional] 
**last_failed** | [**\DateTime**](\DateTime.md) | When the card transaction last failed, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 
**first_failed** | [**\DateTime**](\DateTime.md) | When the card transaction first failed, in [ISO-8601](http://en.wikipedia.org/wiki/ISO_8601) extended offset date-time format. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


