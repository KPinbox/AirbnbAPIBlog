---
layout: post
order: "1"
title: "View Listing Info"
description: "Returns detailed information about a listing, given its ID (e.g., found in the search endpoint reponse)."
method: "GET"
endpoint_url: "https://api.airbnb.com/v2/listings/(listing ID here)"

complete_sample_request_url: "https://api.airbnb.com/v2/listings/5116458?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD&_format=v1_legacy_for_p3&_source=mobile_p3&number_of_guests=1"

basic_sample_request_url: " https://api.airbnb.com/v2/listings/5116458?client_id=3092nxybyb0otqw18e8nh5nty&_format=v1_legacy_for_p3"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" },
	{ key: "_format", value: "v1_legacy_for_p3", description: "API result format (just put this -- it won't work without it)" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "_source", value: "mobile_p3", description: "Not sure. I'm guessing this means the request is coming from an Android mobile phone." },
	{ key: "number_of_guests", value: "1", description: "Determines listing availability dates based on the # of guests." }
]

---
{% include JB/setup %}
