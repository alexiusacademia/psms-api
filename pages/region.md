# Region API

Regions of the country.

## List

List all the regions

Endpoint:  `[base_url]/regions/`

Sample output:

```
[
    {
        "id": 1,
        "name": "CAR",
        "created_on": "2021-05-14T22:13:29.934340+08:00",
        "code": "car"
    },
    {
        "id": 2,
        "name": "Region I",
        "created_on": "2021-05-14T22:13:29.934586+08:00",
        "code": "region_1"
    },
    {
        "id": 3,
        "name": "Region II",
        "created_on": "2021-05-14T22:13:29.934677+08:00",
        "code": "region_2"
    },
    {
        "id": 4,
        "name": "Region III",
        "created_on": "2021-05-14T22:13:29.934752+08:00",
        "code": "region_3"
    },
    {
        "id": 5,
        "name": "Region IVA",
        "created_on": "2021-05-14T22:13:29.934824+08:00",
        "code": "region_4a"
    },
    {
        "id": 6,
        "name": "Region IVB",
        "created_on": "2021-05-14T22:13:29.934891+08:00",
        "code": "region_4b"
    },
    {
        "id": 7,
        "name": "Region V",
        "created_on": "2021-05-14T22:13:29.934959+08:00",
        "code": "region_5"
    },
    {
        "id": 8,
        "name": "Region VI",
        "created_on": "2021-05-14T22:13:29.935024+08:00",
        "code": "region_6"
    },
    {
        "id": 9,
        "name": "Region VII",
        "created_on": "2021-05-14T22:13:29.935087+08:00",
        "code": "region_7"
    },
    {
        "id": 10,
        "name": "Region VIII",
        "created_on": "2021-05-14T22:13:29.935150+08:00",
        "code": "region_8"
    },
    {
        "id": 11,
        "name": "Region IX",
        "created_on": "2021-05-14T22:13:29.935213+08:00",
        "code": "region_9"
    },
    {
        "id": 12,
        "name": "Region X",
        "created_on": "2021-05-14T22:13:29.935274+08:00",
        "code": "region_10"
    },
    {
        "id": 13,
        "name": "Region XI",
        "created_on": "2021-05-14T22:13:29.935337+08:00",
        "code": "region_11"
    },
    {
        "id": 14,
        "name": "Region XII",
        "created_on": "2021-05-14T22:13:29.935398+08:00",
        "code": "region_12"
    },
    {
        "id": 15,
        "name": "Region XIII",
        "created_on": "2021-05-14T22:13:29.935461+08:00",
        "code": "region_13"
    },
    {
        "id": 16,
        "name": "ARMM",
        "created_on": "2021-05-14T22:13:29.935522+08:00",
        "code": "armm"
    },
    {
        "id": 17,
        "name": "NCR",
        "created_on": "2021-05-14T22:13:29.935584+08:00",
        "code": "ncr"
    }
]
```

## Single Region Detail

Show a region details.

Endpoint:  `[base_url]/accounts/details/:region_id`

Sample output for `[base_url]/accounts/details/1`:

```
{
    "id": 1,
    "name": "CAR",
    "created_on": "2021-05-14T22:13:29.934340+08:00",
    "code": "car"
}
```