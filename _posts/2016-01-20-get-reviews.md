---
layout: post
order: "2"
title: "Get Reviews"
description: "Returns reviews for a given listing."
method: "GET"
endpoint_url: "https://api.airbnb.com/v2/reviews"

complete_sample_request_url: "https://api.airbnb.com/v2/reviews?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD&_format=for_mobile_client&_limit=20&_offset=0&_order=language&listing_id=2056659&role=all"

basic_sample_request_url: "https://api.airbnb.com/v2/reviews?client_id=3092nxybyb0otqw18e8nh5nty&listing_id=2056659&role=all"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" },
	{ key: "role", value: "all", description: "Not sure, but it's required." }
]

required_url_parameters: [
	{ key: "listing_id", value: "2056659", description: "ID of the listing you'd like to view reviews for." }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Desired currency" },
	{ key: "_format", value: "for_mobile_client || for_search_results || for_search_results_with_minimal_pricing", description: "Not sure what the difference is." },
	{ key: "_limit", value: "10", description: "Number of reviews to show at a time." },
	{ key: "_offset", value: "0", description: "Number of reviews to offset." }
]

---
{% include JB/setup %}
