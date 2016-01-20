---
layout: post
order: "7"
title: "Get Messages"
description: "Returns message threads, given an AirBnB access token (from authenticating with login endpoints)."
warning: "<strong>NOTE:</strong> <strong>access_token</strong> is required to hit this endpoint."
method: "GET"
endpoint_url: "https://api.airbnb.com/v1/threads"

complete_curl_request: "curl -X GET -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -d \"offset=0\" -d \"items_per_page=10\" -d \"role=guest\" -H \"X-Airbnb-OAuth-Token:3m0ky1cmj6jm4x3sjm8sx8osf\" https://api.airbnb.com/v1/threads"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Desired currency" },
	{ key: "offset", value: "0", description: "Number of message threads to offset in search" },
	{ key: "items_per_page", value: "10", description: "Number of message threads to display at once" },
	{ key: "role", value: "guest", description: "Type of threads to retrieve. \"guest\", \"host\", or don't include this param for both" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "3m0ky1cmj6jm4x3sjm8sx8osf", description: "Airbnb auth token (from authing with login endpoints)" }
]

---
{% include JB/setup %}
