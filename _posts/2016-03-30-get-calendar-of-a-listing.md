---
layout: post
order: "39"
group: "Host"
subgroup: "Listing"
title: "Get Calendar Info"
description: "Get the calendar info for a listing the user is hosting."
warning: "<strong>NOTE:</strong> This is a logged-in endpoint and requires an <strong>access_token</strong>. See <a href=\"#login-by-email\">Login Endpoints.</a>"
method: "GET"
endpoint_url: "https://api.airbnb.com/v2/batch/"

complete_curl_request: "curl -X POST -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/json; charset=UTF-8\" --data-binary '{\"operations\":[{\"method\":\"GET\",\"path\":\"/calendar_days\",\"query\":{\"start_date\":\"2016-01-30\",\"listing_id\":\"12132179\",\"_format\":\"host_calendar\",\"end_date\":\"2017-03-30\"}},{\"method\":\"GET\",\"path\":\"/dynamic_pricing_controls/12132179\",\"query\":{}}],\"_transaction\":false}' --compressed https://api.airbnb.com/v2/batch/?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "9nwld6we4td9vkwj160teb49a", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "3m0ky1cmj6jm4x3sjm3sx8osf", description: "Airbnb auth token (from auth-ing with login endpoints)" },
	{ key: "Content-Type", value: "application/json; charset=UTF-8", description: "Content type" }
]

body: '{"operations":[{"method":"GET","path":"/calendar_days","query":{"start_date":"2016-01-30","listing_id":"12132179","_format":"host_calendar","end_date":"2017-03-30"}},{"method":"GET","path":"/dynamic_pricing_controls/12132179","query":{}}],"_transaction":false}'

---
{% include JB/setup %}
