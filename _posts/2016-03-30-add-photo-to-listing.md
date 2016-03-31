---
layout: post
order: "14"
title: "Add photo to listing"
description: "Add a photo to the listing."
warning: "<strong>NOTE:</strong> The returned <strong>access_token</strong> is required to hit logged-in endpoints."
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/listings/12132179/update"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: multipart/form-data; boundary=d27a2537-d9c1-40e4-b1f9-209eb38d45ff\" -F name=\"photos[]\" -F filename=\"~/Pictures/captured_photo1459370793915.jpg\" https://api.airbnb.com/v1/listings/12132179/update"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "9nwld6we4td9vkwj160teb49a", description: "Airbnb auth token (from auth-ing with login endpoints)" }
]

default_required_header_parameters: [
	{ key: "Content-Type", value: "multipart/form-data; boundary=d27a2537-d9c1-40e4-b1f9-209eb38d45ff", description: "Content type" }
]

default_required_form_parameters: [
	{ key: "name", value: "photos[]", description: "Require for uploading picture" }
]

default_required_form_parameters: [
	{ key: "filename", value: "~/Pictures/captured_photo1459370793915.jpg", description: "Filename location" }
]
---
{% include JB/setup %}
