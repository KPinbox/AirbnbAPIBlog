---
layout: post
order: "23"
title: "Submit security verification code"
description: "Submit the security verification code to verify the account."
warning: "<strong>NOTE:</strong> The returned <strong>access_token</strong> is required to hit logged-in endpoints."
method: "POST"
endpoint_url: "https://api.airbnb.com/v2/security_checks/{userID}"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/json; charset=UTF-8\" --data-binary \"{\"data\":{\"phone_number_id\":27231699,\"code\":\"0545\"},\"strategy\":\"phone_verification\",\"activity_type\":\"mobile\"}\" --compressed https://api.airbnb.com/v2/security_checks/57297136"

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
	{ key: "X-Airbnb-OAuth-Token", value: "3m0ky1cmj6jm4x3sjm3sx8osf", description: "Airbnb auth token (from auth-ing with login endpoints)" },
	{ key: "Content-Type", value: "application/json; charset=UTF-8", description: "Content type" }
]

body: '{"data":{"phone_number_id":27231699,"code":"0545"},"strategy":"phone_verification","activity_type":"mobile"}'

---
{% include JB/setup %}
