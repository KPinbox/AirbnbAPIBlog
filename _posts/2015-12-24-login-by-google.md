---
layout: post
order: "6"
group: "Public"
group_id: 0
subgroup: "Login"
subgroup_id: 0
sort_order: 0
title: "Login By Google"
description: "Returns an access_token, given a valid Google user OAuth access token. See <a href=\"https://developers.google.com/identity/protocols/OAuth2\" target=\"_blank\">the Google docs</a> to learn how to generate a Google access token."
warning: "<strong>NOTE:</strong> The returned <strong>access_token</strong> is required to hit logged-in endpoints."
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/authorize"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -F assertion_type=https://www.googleapis.com/oauth2/v1/userinfo -F assertion=va29.rgKq-cvJJ6IetZLecDvv2gxJ92tPYf5kEtL_PS98cEc5x1240n2aelp4uZ22xdWsLu2e -F prevent_account_creation=true https://api.airbnb.com/v1/authorize"

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
	{ key: "assertion_type", value: "https://www.googleapis.com/oauth2/v1/userinfo", description: "Required for Google authentication." },
	{ key: "prevent_account_creation", value: "true", description: "For sign-in, as opposed to registration." }
]

required_form_parameters: [
	{ key: "assertion", value: "va29.rgKq-cvJJ6IetZLecDvv2gxJ92tPYf5k...", description: "Google user's access token." }
]
---
{% include JB/setup %}
