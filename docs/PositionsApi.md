# ks_api_client.PositionsApi

All URIs are relative to *https://tradeapi.kotaksecurities.com/apim*

Method  | Description
------------- | -------------
[**positions**](PositionsApi.md#positions) | Get&#39;s positions.

# **positions**
> object positions(position_type)

Get's positions.

Return positions of provided position type.

### Example(position_type="TODAYS")


```python

from ks_api_client import ks_api

client = ks_api.KSTradeApi(access_token = "access_token", userid = "userid", \
                 consumer_key = "consumer_key", ip = "IP", app_id = "app_id")

#First initialize session and generate session token

try:
    # Get's position by position_type.
    client.positions(position_type = "TODAYS")
except Exception as e:
    print("Exception when calling PositionsApi->positions: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **position_type** | **str**| Type of position - TODAYS | 

### Return type

**object**

### Sample response
```python
{
  "Success": [
    {
      "actualNetTrdValue": 0,
      "averageStockPrice": 0,
      "buyOpenQtyLot": 1,
      "buyOpenVal": 2133,
      "buyTradedQtyLot": 0,
      "buyTradedVal": 0,
      "buyTrdAvg": 0,
      "deliveryStatus": 0,
      "denominator": 1,
      "exchange": "NN",
      "expiryDate": "-",
      "exposureMargin": 0,
      "exposureMarginTotal": 0,
      "grossUtilization": 426.6,
      "instrumentName": "ACC-EQ",
      "instrumentToken": 727,
      "lastPrice": 2274,
      "marginType": "N",
      "marketLot": 1,
      "maxCODQty": 1,
      "multiplier": 1,
      "netChange": -18,
      "netTrdQtyLot": 0,
      "netTrdValue": 0,
      "normalSqOffQty": 0,
      "optionType": "- ",
      "percentChange": -0.01,
      "premium": 0,
      "qtyUnit": "",
      "rbiRefRate": 1,
      "realizedPL": 0,
      "segment": "EQ",
      "sellOpenQtyLot": 0,
      "sellOpenVal": 0,
      "sellTradedQtyLot": 0,
      "sellTradedVal": 0,
      "sellTrdAvg": 0,
      "spanMargin": 0,
      "spanMarginTotal": 0,
      "spreadTotal": 0,
      "strikePrice": 0,
      "symbol": "ACC",
      "totalStock": 0
    }
  ]
}
```

### HTTP request headers

 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Gets the Positoin data for a client account. |  -  |
**400** | Invalid or missing input parameters |  -  |
**403** | Invalid session, please re-login to continue |  -  |
**429** | Too many requests to the API |  -  |
**500** | Unexpected error |  -  |
**502** | Not able to communicate with OMS |  -  |
**503** | Trade API service is unavailable |  -  |
**504** | Gateway timeout, trade API is unreachable |  -  |



### Example(position_type="STOCKS")


```python

from ks_api_client import ks_api

client = ks_api.KSTradeApi(access_token = "access_token", userid = "userid", \
                 consumer_key = "consumer_key", ip = "IP", app_id = "app_id")

#First initialize session and generate session token

try:
    # Get's position by position_type.
    client.positions(position_type = "STOCKS")
except Exception as e:
    print("Exception when calling PositionsApi->positions: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **position_type** | **str**| Type of position - STOCKS | 

### Return type

**object**

### Sample response
```python
{
  "Success": [
    {
      "actualNetTrdValue": 0,
      "averageStockPrice": 0,
      "buyOpenQtyLot": 1,
      "buyOpenVal": 2133,
      "buyTradedQtyLot": 0,
      "buyTradedVal": 0,
      "buyTrdAvg": 0,
      "deliveryStatus": 0,
      "denominator": 1,
      "exchange": "NN",
      "expiryDate": "-",
      "exposureMargin": 0,
      "exposureMarginTotal": 0,
      "grossUtilization": 426.6,
      "instrumentName": "ACC-EQ",
      "instrumentToken": 727,
      "lastPrice": 2274,
      "marginType": "N",
      "marketLot": 1,
      "maxCODQty": 1,
      "multiplier": 1,
      "netChange": -18,
      "netTrdQtyLot": 0,
      "netTrdValue": 0,
      "normalSqOffQty": 0,
      "optionType": "- ",
      "percentChange": -0.01,
      "premium": 0,
      "qtyUnit": "",
      "rbiRefRate": 1,
      "realizedPL": 0,
      "segment": "EQ",
      "sellOpenQtyLot": 0,
      "sellOpenVal": 0,
      "sellTradedQtyLot": 0,
      "sellTradedVal": 0,
      "sellTrdAvg": 0,
      "spanMargin": 0,
      "spanMarginTotal": 0,
      "spreadTotal": 0,
      "strikePrice": 0,
      "symbol": "ACC",
      "totalStock": 0
    }
  ]
}
```

### HTTP request headers

 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Gets the Positoin data for a client account. |  -  |
**400** | Invalid or missing input parameters |  -  |
**403** | Invalid session, please re-login to continue |  -  |
**429** | Too many requests to the API |  -  |
**500** | Unexpected error |  -  |
**502** | Not able to communicate with OMS |  -  |
**503** | Trade API service is unavailable |  -  |
**504** | Gateway timeout, trade API is unreachable |  -  |


### Example(position_type="OPEN")


```python

from ks_api_client import ks_api

client = ks_api.KSTradeApi(access_token = "access_token", userid = "userid", \
                 consumer_key = "consumer_key", ip = "IP", app_id = "app_id")

#First initialize session and generate session token

try:
    # Get's position by position_type.
    client.positions(position_type = "OPEN")
except Exception as e:
    print("Exception when calling PositionsApi->positions: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **position_type** | **str**| Type of position - OPEN | 

### Return type

**object**

### Sample response
```python
{
  "Success": [
    {
      "actualNetTrdValue": 0,
      "averageStockPrice": 0,
      "buyOpenQtyLot": 1,
      "buyOpenVal": 2133,
      "buyTradedQtyLot": 0,
      "buyTradedVal": 0,
      "buyTrdAvg": 0,
      "deliveryStatus": 0,
      "denominator": 1,
      "exchange": "NN",
      "expiryDate": "-",
      "exposureMargin": 0,
      "exposureMarginTotal": 0,
      "grossUtilization": 426.6,
      "instrumentName": "ACC-EQ",
      "instrumentToken": 727,
      "lastPrice": 2274,
      "marginType": "N",
      "marketLot": 1,
      "maxCODQty": 1,
      "multiplier": 1,
      "netChange": -18,
      "netTrdQtyLot": 0,
      "netTrdValue": 0,
      "normalSqOffQty": 0,
      "optionType": "- ",
      "percentChange": -0.01,
      "premium": 0,
      "qtyUnit": "",
      "rbiRefRate": 1,
      "realizedPL": 0,
      "segment": "EQ",
      "sellOpenQtyLot": 0,
      "sellOpenVal": 0,
      "sellTradedQtyLot": 0,
      "sellTradedVal": 0,
      "sellTrdAvg": 0,
      "spanMargin": 0,
      "spanMarginTotal": 0,
      "spreadTotal": 0,
      "strikePrice": 0,
      "symbol": "ACC",
      "totalStock": 0
    }
  ]
}
```

### HTTP request headers

 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Gets the Positoin data for a client account. |  -  |
**400** | Invalid or missing input parameters |  -  |
**403** | Invalid session, please re-login to continue |  -  |
**429** | Too many requests to the API |  -  |
**500** | Unexpected error |  -  |
**502** | Not able to communicate with OMS |  -  |
**503** | Trade API service is unavailable |  -  |
**504** | Gateway timeout, trade API is unreachable |  -  |



[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
