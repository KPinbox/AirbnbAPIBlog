---
layout: post
order: "20"
group: "Host"
group_id: 2
subgroup: "Verification"
title: "Get Phone Number(s)"
description: "Get phone numbers that airbnb has to display to user so he/she can choose one to complete the security check and verify his/her account."
method: "GET"
endpoint_url: "https://api.airbnb.com/v2/security_checks/{userID}"

complete_curl_request: "curl -X GET -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/x-www-form-urlencoded; charset=UTF-8\" --compressed  https://api.airbnb.com/v2/security_checks/57297136"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Desired currency" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "9nwld6we4td9vkwj160teb49a", description: "Airbnb auth token (from auth-ing with login endpoints)" }
]

default_required_header_parameters: [
	{ key: "Content-Type", value: "application/x-www-form-urlencoded; charset=UTF-8", description: "Content type" }
]

---
{% include JB/setup %}
