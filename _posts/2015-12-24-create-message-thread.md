---
layout: post
order: "8"
group: "User"
subgroup: "Messages"
title: "Create Message Thread"
description: "Creates a message thread and a stay request, given a valid  access token and a listing ID."
warning: "<strong>NOTE:</strong> This is a logged-in endpoint and requires an <strong>access_token</strong>. See <a href=\"#login-by-email\">Login Endpoints.</a>"
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/threads/create"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -F \"message=Hi!\" -F \"checkout_date=2018-04-02T22:00:00.000-0700\" -F \"checkin_date=2018-04-01T00:00:00.000-0700\" -F  \"number_of_guests=1\" -F \"listing_id=10166581\" -H \"X-Airbnb-OAuth-Token:3m0ky1cmj6jm4x3sjm8sx8osf\" https://api.airbnb.com/v1/threads/create"

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
	{ key: "listing_id", value: "10166581", description: "ID of the listing you'd like to message" },
	{ key: "number_of_guests", value: "1", description: "Number of guests in the request." },
	{ key: "checkin_date", value: "2018-04-01T00:00:00.000-0700", description: "Requested check-in date." },
	{ key: "checkout_date", value: "2018-04-02T00:00:00.000-0700", description: "Requested check-out date." },
	{ key: "message", value: "Hi!", description: "Initial message to send (empty to send request only)." }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "3m0ky1cmj6jm4x3sjm8sx8osf", description: "Airbnb auth token (from auth-ing with login endpoints)" }
]

---
{% include JB/setup %}
