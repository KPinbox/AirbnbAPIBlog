---
layout: post
order: "0"
group: "Public"
group_id: 0
subgroup: "Get Info"
subgroup_id: 1
sort_order: 1
title: "Listing Search"
description: "Returns listings that fit the given search parameters."
method: "GET"
endpoint_url: "https://api.airbnb.com/v2/search_results"

complete_sample_request_url: "https://api.airbnb.com/v2/search_results?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD&_format=for_search_results_with_minimal_pricing&_limit=10&_offset=0&fetch_facets=true&guests=1&ib=false&ib_add_photo_flow=true&location=Lake%20Tahoe%2C%20CA%2C%20US&min_bathrooms=0&min_bedrooms=0&min_beds=1&min_num_pic_urls=10&price_max=210&price_min=40&sort=1&user_lat=37.3398634&user_lng=-122.0455164"

basic_sample_request_url: "https://api.airbnb.com/v2/search_results?client_id=3092nxybyb0otqw18e8nh5nty"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Desired currency" },
	{ key: "_format", value: "for_search_results || for_search_results_with_minimal_pricing", description: "Search with pricing or not." },
	{ key: "_limit", value: "10", description: "Number of listings to show at a time." },
	{ key: "_offset", value: "0", description: "Number of listings to offset in search." },
	{ key: "guests", value: "1", description: "Number of guests." },
	{ key: "ib", value: "false", description: "Not sure." },
	{ key: "ib_add_photo_flow", value: "true", description: "Not sure." },
	{ key: "location", value: "Los%20Angeles%2C%20CA", description: "Search by location name -- if unsure of lat/lng, etc." },
	{ key: "min_bathrooms", value: "0", description: "Minimum number of bathrooms." },
	{ key: "min_bedrooms", value: "0", description: "Minimum number of bedrooms." },
	{ key: "min_beds", value: "0", description: "Minimum number of beds." },
	{ key: "price_min", value: "40", description: "Minimum price." },
	{ key: "price_max", value: "210", description: "Maximum price." },
	{ key: "min_num_pic_urls", value: "10", description: "Minimum number of pictures." },
	{ key: "sort", value: "1", description: "Sorting order (1: forward order, 0: reverse order)." },
	{ key: "suppress_facets", value: "true", description: "Not sure." },
	{ key: "user_lat", value: "37.18722222222222", description: "Latitude search coordinate." },
	{ key: "user_lng", value: "-122.42833333333333", description: "Longitude search coordinate." }
]

---
{% include JB/setup %}
