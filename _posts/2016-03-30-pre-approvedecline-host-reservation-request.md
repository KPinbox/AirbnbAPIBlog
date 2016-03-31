---
layout: post
order: "13"
title: "Pre-approve/Decline Host Reservation Request"
description: "Pre-approve or decline a request for reserving your listing."
warning: "<strong>NOTE:</strong> The returned <strong>access_token</strong> is required to hit logged-in endpoints."
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/threads/184980528/update"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/x-www-form-urlencoded; charset=UTF-8\" --data-binary \"listing_id=11040894&message=&status=preapproved\" --compressed https://api.airbnb.com/v1/threads/184980528/update"

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
