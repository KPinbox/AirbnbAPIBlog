---
layout: post
order: "10"
group: "Host"
group_id: 2
subgroup: "Messages"
subgroup_id: 20
sort_order: 220
title: "Get Host Messages"
description: "Returns host messages."
warning: "<strong>NOTE:</strong> This is a logged-in endpoint and requires an <strong>access_token</strong>. See <a href=\"#login-by-email\">Login Endpoints.</a>"
method: "GET"
endpoint_url: "https://api.airbnb.com/v2/threads"

complete_curl_request: "curl -X GET -H \"X-Airbnb-OAuth-Token: 9wled6f39td9vksj280twe10w\" -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -d \"_format=for_mobile_inbox\" -d \"_limit=10\" -d \"_offset=0\" -d \"role=host\" https://api.airbnb.com/v2/threads"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Desired currency" },
	{ key: "_format", value: "for_mobile_inbox", description: "Format.  Not sure what values this takes." },
	{ key: "_offset", value: "0", description: "Number of message threads to offset in search" },
	{ key: "_limit", value: "10", description: "Number of message threads to display at once" },
	{ key: "role", value: "host", description: "Type of threads to retrieve. \"guest\", \"host\", or don't include this param for both" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "3m0ky1cmj6jm4x3sjm8sx8osf", description: "Airbnb auth token (from auth-ing with login endpoints)" }
]

---
{% include JB/setup %}
