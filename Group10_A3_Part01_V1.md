# Comp 3040 A3 API Specification and Review Presentation

## API Description

The API will provide users the provider's phone number of the COVID-19 and Flu vaccination sites. The user will have to enter the provider's name, address, and type to get the provider's phone number.  

## Endpoints

There is only one endpoint for this API.

### `GET` /providerNumber

The URL of endpoint is : https://geoportal.gov.mb.ca/manitoba-covid-19-and-flu-vaccination-sites-1/providerNumber

## Parameters

### 1. providerName (String)

- The name of the provider of flu shots - a required parameter with type string.
 
### 2. providerAddress (String)

- The address of the provider of flu shots - a required parameter with type string.

### 3. providerType (String)

- The type of the provider of flu shots - a required parameter with type string.



## Resources

```
"results": {
  {
    "providerType" : providerType,
    "providerName" : providerName,
    "address" : providerAddress,
    "phone" : phoneNumber
  }
},
"status" : ""
```
## Sample Request

`https://geoportal.gov.mb.ca/manitoba-covid-19-and-flu-vaccination-sites-1/providerNumber?provider_type="Pharmacy"&provider_name="Spring Meadow Pharmacy"&address="19 1783 Plessis Rd"`

## Sample Response

```
"results": {
  {
    "providerType" : "Pharmacy",
    "providerName" : "Spring Meadow Pharmacy",
    "address" : "19 1783 Plessis Rd",
    "phone" : "204-504-2037"
  }
},
"status" : "success"
```
