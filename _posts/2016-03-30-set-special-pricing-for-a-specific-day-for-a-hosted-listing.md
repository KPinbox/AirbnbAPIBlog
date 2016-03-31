---
layout: post
order: "41"
title: "Set special pricing for a specific day for a hosted listing"
description: "As the title says..."
warning: "<strong>NOTE:</strong> The returned <strong>access_token</strong> is required to hit logged-in endpoints."
method: "PUT"
endpoint_url: "https://api.airbnb.com/v2/calendars/12132179/2016-04-15/2016-04-15"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" id \"_format=host_calendar\" -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/json; charset=UTF-8\" --data-binary \"{\"daily_price\":60,\"demand_based_pricing_overridden\":true,\"availability\":\"available\"}\" --compressed https://api.airbnb.com/v2/batch/"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "9nwld6we4td9vkwj160teb49a", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings" },
	{ key: "_format", value: "host_calendar", description: "Specify to update host calendar." }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "3m0ky1cmj6jm4x3sjm3sx8osf", description: "Airbnb auth token (from auth-ing with login endpoints)" },
	{ key: "Content-Type", value: "application/json; charset=UTF-8", description: "Content type" }
]

body: '{"daily_price":60,"demand_based_pricing_overridden":true,"availability":"available"}'

---
{% include JB/setup %}
