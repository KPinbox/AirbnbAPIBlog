---
layout: post
order: "5"
title: "Login By Email"
description: "Returns an access_token, given a valid user account email and password."
warning: "<strong>NOTE:</strong> <strong>access_token</strong> is required to hit this endpoint."
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/threads/create"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -F grant_type=password -F password=asdf1234 -F username=airbnbdev@gmail.com https://api.airbnb.com/v1/authorize"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings" }
]

default_required_form_parameters: [
	{ key: "grant_type", value: "password", description: "Required for email authentication (as opposed to OAuth)" }
]

required_form_parameters: [
	{ key: "username", value: "airbnbdev@gmail.com", description: "Account's email address" },
	{ key: "password", value: "asdf1234", description: "Account's clear-text password (note: endpoint uses HTTPS)" }
]
---
{% include JB/setup %}
