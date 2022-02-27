# Account API
---

## Create
Creating a new account.  

Endpoint:  `[base_url]/accounts/create/`

JSON Data:  
`office_name` String  
`username` String  
`password` String  
`first_name` String  
`last_name` String  
`email` String  
`subscription_type` Integer (Optional)

* To get the options for subscription types, fetch it from its [api](/pages/subscription_types.md).

## Details
Fetch the details of the account of the current user.  

Endpoint:  `[base_url]/accounts/details/`

This api doesn't take any params as the backend gets the current user's account id automatically.

## Update
Update an account detail.

Endpoint:  `[base_url]/accounts/update/`

JSON Data:  
`office_name` String (Optional)
