# User API
---

## List
List all users of an account. Account is automatically detected from the logged in user.

Endpoint: `[base_url]/user-accounts/`

*Note: Only users with admin/account_holder roles can access this api.*

## Details
Fetch details of a user.

Endpoint: `[base_url]/user-accounts/:user_account_id`

Output:  
- `id` Integer  
- `name` String (Full name)  
- `first_name` String  
- `last_name` String  
- `email` String  
- `username` String  
- `position` String  
- `roles` List(Role object)  
- `monitored_contracts` List  

Sample output for `[base_url]/user-accounts/2`

```
{
    "id": 2,
    "name": "Juan dela Cruz",
    "first_name": "Juan",
    "last_name": "dela Cruz",
    "email": "username@gmail.com",
    "username": "username",
    "position": "Sr. Engineer A",
    "roles": [
        {
            "id": 1,
            "name": "Account Holder"
        },
        {
            "id": 2,
            "name": "Project Inspector"
        },
        {
            "id": 3,
            "name": "Accounting Personnel"
        }
    ],
    "monitored_contracts": [
        {
            "id": 1,
            "contract_id": "NIAR3-TARZAM-2019-32-Iba (Upper Prenza)",
            "implementation_year": "2019-07-30"
        },
        {
            "id": 6,
            "contract_id": "NIAR3-TARZAM-2020-01-AMBALINGIT CIS",
            "implementation_year": "2020-03-25"
        },
        {
            "id": 7,
            "contract_id": "NIAR3-TARZAM-2022-01-UPPER PRENZA CIS",
            "implementation_year": "2022-01-03"
        }
    ]
}
```

## Create
Create a user.

Endpoint: `[base_url]/user-accounts/create/`

JSON Data:  
- `role_id` Integer  
- `username` String  
- `password` String  

Rules:  
- Only admin/account holder can create a new user.

## Update
Update a user.

Endpoint: `[base_url]/user-accounts/update/`

JSON Data:  
- `id` Integer
- `password` String (Optional)
- `first_name` String (Optional)
- `last_name` String (Optional)
- `email` String (Optional)
- `position` String (Optional)
- `is_account_holder` Bool
- `is_project_inspector` Bool
- `is_financial_encoder` Bool
- `is_viewer` Bool 

## Update User Password
Update password of the current logged in user.

Endpoint: `[base_url]/user-accounts/update-password/`

JSON Data:
- `new_password` String (Required)

## Project Inspectors
Get list of all project inspectors of the account of the current user.

Endpoint: `[base_url]/user-accounts/project-inspectors`

Output Data:  

List of object with the following data  
- `id` Integer
- `username` String
- `first_name` String
- `last_name` String