---
layout: post
order: "13"
group: "Host"
group_id: 2
subgroup: "Messages"
subgroup_id: 20
sort_order: 220
title: "Pre-approve/Decline Reservation Request"
description: "Pre-approve or decline a request for reserving your listing."
warning: "<strong>NOTE:</strong> This is a logged-in endpoint and requires an <strong>access_token</strong>. See <a href=\"#login-by-email\">Login Endpoints.</a>"
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/threads/184980528/update"

complete_curl_request: "curl -X POST -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/x-www-form-urlencoded; charset=UTF-8\" --data-binary \"listing_id=11040894&message=&status=preapproved\" --compressed https://api.airbnb.com/v1/threads/184980528/update?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings" }
]

required_form_parameters: [
	{ key: "listing_id", value: "11040894", description: "Listing ID for the reservation request." },
	{ key: "message", value: "Hi%20there", description: "Message you'd like to add to the reservation response." },
	{ key: "status", value: "preapproved", description: "Response to reservation request -- can be either \"preapproved\" or \"denied\"" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "9nwld6we4td9vkwj160teb49a", description: "Airbnb auth token (from auth-ing with login endpoints)" }
]

default_required_header_parameters: [
	{ key: "Content-Type", value: "application/x-www-form-urlencoded; charset=UTF-8", description: "Content type" }
]

---
{% include JB/setup %}
