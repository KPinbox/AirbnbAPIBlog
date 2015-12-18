---
layout: post
order: "2"
title: "View User Info"
description: ""
method: "GET"
endpoint_url: "https://api.airbnb.com/v2/users/(user ID here)"

complete_sample_request_url: "https://api.airbnb.com/v2/users/2917444?client_id=3092nxybyb0otqw18e8nh5nty&_format=v1_legacy_show"

basic_sample_request_url: "https://api.airbnb.com/v2/users/2917444?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD&_format=v1_legacy_show"

category: "endpoint"
tags: []

default_required_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" },
	{ key: "_format", value: "v1_legacy_show", description: "API result format (just put this -- it'll work without it, but it won't have as much data)" }
]

required_parameters: []

optional_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings." }
]

---
{% include JB/setup %}
