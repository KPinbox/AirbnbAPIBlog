---
layout: post
order: "14"
title: "Create empty listing"
description: "Create empty listing to host -- you can update the listing with information in other requests."
warning: "<strong>NOTE:</strong> The returned <strong>access_token</strong> is required to hit logged-in endpoints."
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/listings/create"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/json; charset=UTF-8\" --data-binary \"{\"room_type_category\":\"private_room\",\"property_type_id\":2,\"bathrooms\":1,\"person_capacity\":1,\"beds\":1,\"bedrooms\":1,\"city\":\"Sunnyvale, California, US\"}\" --compressed https://api.airbnb.com/v1/listings/create"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "9nwld6we4td9vkwj160teb49a", description: "Airbnb auth token (from auth-ing with login endpoints)" }
]

default_required_header_parameters: [
	{ key: "Content-Type", value: "application/json; charset=UTF-8", description: "Content type" }
]

body: '{"room_type_category":"private_room","property_type_id":2,"bathrooms":1,"person_capacity":1,"beds":1,"bedrooms":1,"city":"Sunnyvale, California, US"}'
---
{% include JB/setup %}
