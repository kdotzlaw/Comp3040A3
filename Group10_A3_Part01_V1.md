# Comp 3040 A3 API Specification and Review Presentation

## API Description

The API will provide users the provider's phone number of the Covid-19 and Flu vaccination sites. The user will have to enter the provider name, address, and provider type to get the provider's phone number.  

## Endpoints

There is only one endpoint for this API.

### `GET` /providerNumber

the URL of endpoint is : https://geoportal.gov.mb.ca/manitoba-covid-19-and-flu-vaccination-sites-1/providerNumber

## Parameters

### 1. Provider Name (String)

 It is the name of the provider of flu shots. It is a required parameter 
 and the type of this parameter must be string.
 
 
### 2. Provider Address (String)

It is the address of the provider of flu shots. It is also a required paramter
and the type of parameter is string.

### 3. Provider Type (String)

It is the type of the provider of flu shots. It is a required parameter and the
type of parameter is string.



## Resources

```
"results": [
  {
    "provider_type" : "",
    "provider_name" : "",
    "status" : "",
    "date" : "",
    "date_updated" : "",
    "vaccination_comments" : "",
    "note" : "",
    "address" : "",
    "phone" : ""
  },
  ...
],
"status" : ""
```
## Sample Request

`https://geoportal.gov.mb.ca/manitoba-covid-19-and-flu-vaccination-sites-1/providerNumber?provider_type="Pharmacy"&provider_name="Spring Meadow Pharmacy"&address="19 1783 Plessis Rd"`
