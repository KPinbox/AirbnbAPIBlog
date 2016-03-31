---
layout: post
order: "9"
group: "Public"
group_id: 0
subgroup: "Get Info"
subgroup_id: 1
sort_order: 1
title: "Get Host Listings"
description: "Returns information about all the listings a user hosts."
method: "GET"
endpoint_url: "https://api.airbnb.com/v2/listings"

complete_curl_request: "curl -X GET -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -d \"_format=v1_legacy_long\" -d \"_limit=10\" -d \"_offset=0\" -d \"has_availability=false\" -d \"user_id=57297136\" https://api.airbnb.com/v2/listings"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Desired currency" },
	{ key: "_format", value: "v1_legacy_long", description: "Not sure..." },
	{ key: "_limit", value: "10", description: "Max listings to return" },
	{ key: "_offset", value: "0", description: "Listing offset" },
	{ key: "has_availability", value: "false", description: "Whether to show listings that are currently active or not" },
	{ key: "user_id", value: "57297136", description: "The ID of the user whose listings you'd like to get" }
]

required_header_parameters: [
]

---
{% include JB/setup %}
