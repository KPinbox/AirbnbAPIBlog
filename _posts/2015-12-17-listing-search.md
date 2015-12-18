---
layout: post
order: "0"
title: "Listing Search"
description: ""
method: "GET"
endpoint_url: "https://api.airbnb.com/v2/search_results"

complete_sample_request_url: "https://api.airbnb.com/v2/search_results?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD&_format=for_search_results&_limit=10&_offset=0&guests=1&ib=false&ib_add_photo_flow=true&location=Los%20Angeles%2C%20CA&min_bathrooms=0&min_bedrooms=0&min_beds=0&min_num_pic_urls=10&mobile_session_id=&sort=1&suppress_facets=true&user_lat=37.34722222222222&user_lng=-122.04833333333333"

basic_sample_request_url: "https://api.airbnb.com/v2/search_results?client_id=3092nxybyb0otqw18e8nh5nty"

category: "endpoint"
tags: []

default_required_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

required_parameters: []

optional_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Desired currency" },
	{ key: "_format", value: "for_search_results", description: "Not sure what this is for." },
	{ key: "_limit", value: "10", description: "Number of listings to show at a time." },
	{ key: "_offset", value: "0", description: "Number of listings to offset in search." },
	{ key: "guests", value: "1", description: "Number of guests." },
	{ key: "ib", value: "false", description: "Not sure." },
	{ key: "ib_add_photo_flow", value: "true", description: "Not sure." },
	{ key: "location", value: "Los%20Angeles%2C%20CA", description: "Search by location name -- if unsure of lat/lng, etc." },
	{ key: "min_bathrooms", value: "0", description: "Minimum number of bathrooms." },
	{ key: "min_bedrooms", value: "0", description: "Minimum number of bedrooms." },
	{ key: "min_beds", value: "0", description: "Minimum number of beds." },
	{ key: "min_num_pic_urls", value: "10", description: "Minimum number of pictures." },
	{ key: "sort", value: "1", description: "Sorting order (1: forward order, 0: reverse order)." },
	{ key: "suppress_facets", value: "true", description: "Not sure." },
	{ key: "user_lat", value: "37.18722222222222", description: "Latitude search coordinate." },
	{ key: "user_lng", value: "-122.42833333333333", description: "Longitude search coordinate." }
]

---
{% include JB/setup %}
