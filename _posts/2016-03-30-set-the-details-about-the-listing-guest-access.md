---
layout: post
order: "27"
title: "Set The Details About the Listing Guest Access"
description: "This updates the \"guest access\" field of the listing."
warning: "<strong>NOTE:</strong> The returned <strong>access_token</strong> is required to hit logged-in endpoints."
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/listings/12132179/update"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/json; charset=UTF-8\" --data-binary \"{\"listing\":{\"access\":\"Hdjdj\"}}\" --compressed https://api.airbnb.com/v1/listings/12132179/update"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "9nwld6we4td9vkwj160teb49a", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "3m0ky1cmj6jm4x3sjm3sx8osf", description: "Airbnb auth token (from auth-ing with login endpoints)" },
	{ key: "Content-Type", value: "application/json; charset=UTF-8", description: "Content type" }
]

body: '{"listing":{"access":"Hdjdj"}}'

---
{% include JB/setup %}
