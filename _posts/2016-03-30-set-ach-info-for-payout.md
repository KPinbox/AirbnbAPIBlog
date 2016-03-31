---
layout: post
order: "42"
title: "Set ACH Info for Payout"
description: "Set the account's payout information so Airbnb can pay the user."
warning: "<strong>NOTE:</strong> The returned <strong>access_token</strong> is required to hit logged-in endpoints."
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/payout_infos/create_ach"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -d \"account_name=Bank+of+America\" -d \"account_number=000043901948\" -d \"account_type=Checking\" -d \"country=US\" -d \"payout_address1=1641+Lachine+Drive\" -d \"payout_address2=\" -d \"payout_city=Sunnyvale\" -d \"payout_country=US\" -d \"payout_state=CA\" -d \"payout_zip=94087\" -d \"routing_number=121000123\" -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/x-www-form-urlencoded; charset=UTF-8\" https://api.airbnb.com/v1/payout_infos/create_ach"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "9nwld6we4td9vkwj160teb49a", description: "API Key" }
]

required_url_parameters: [
	{ key: "account_name", value: "Bank+of+America", description: "Account name to save as" },
	{ key: "account_number", value: "000043901448", description: "Bank account number." },
	{ key: "account_type", value: "Checking", description: "Bank account type (\"Savings\" or \"Checking\")" },
	{ key: "country", value: "US", description: "Not sure what this is for." },
	{ key: "payout_address1", value: "1641+Lachine+Drive", description: "Address1 of the payout" },
	{ key: "payout_address2", value: "Suite+2", description: "Address2 of the payout" },
	{ key: "payout_city", value: "Sunnyvale", description: "City of the payout" },
	{ key: "payout_country", value: "US", description: "Country of the payout" },
	{ key: "payout_state", value: "CA", description: "State of the payout" },
	{ key: "payout_zip", value: "94087", description: "Zip code of the payout" },
	{ key: "routing_number", value: "121000123", description: "Bank account routing number" },
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "3m0ky1cmj6jm4x3sjm3sx8osf", description: "Airbnb auth token (from auth-ing with login endpoints)" },
	{ key: "Content-Type", value: "application/x-www-form-urlencoded; charset=UTF-8", description: "Content type" }
]
---
{% include JB/setup %}
