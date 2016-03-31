---
layout: post
order: "41"
group: "Host"
subgroup: "Listing"
title: "Set Special Daily Pricing"
description: "Set special pricing for a specific day."
warning: "<strong>NOTE:</strong> This is a logged-in endpoint and requires an <strong>access_token</strong>. See <a href=\"#login-by-email\">Login Endpoints.</a>"
method: "PUT"
endpoint_url: "https://api.airbnb.com/v2/calendars/12132179/2016-04-15/2016-04-15"

complete_curl_request: "curl -X POST -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/json; charset=UTF-8\" --data-binary '{\"daily_price\":60,\"demand_based_pricing_overridden\":true,\"availability\":\"available\"}' --compressed https://api.airbnb.com/v2/batch/?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD&_format=host_calendar"

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
