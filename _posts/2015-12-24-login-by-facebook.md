---
layout: post
order: "4"
group: "Public"
group_id: 0
subgroup: "Login"
subgroup_id: 0
title: "Login By Facebook"
description: "Returns an access_token, given a valid Facebook user OAuth access token. See <a href=\"https://developers.facebook.com/docs/facebook-login/access-tokens\" target=\"_blank\">the Facebook docs</a> to learn how to generate an FB access token."
warning: "<strong>NOTE:</strong> The returned <strong>access_token</strong> is required to hit logged-in endpoints."
method: "POST"
endpoint_url: "https://api.airbnb.com/v1/authorize"

complete_curl_request: "curl -X POST -d \"client_id=3092nxybyb0otqw18e8nh5nty\" -d \"locale=en-US\" -d \"currency=USD\" -F assertion_type=https://graph.facebook.com/me -F assertion=CAAAAIEMtwcwBAMTO70riSczKIgT3Nv0EnaZBWmObwt914WAJYRsxZAekHZBLnpqOauZAZATjpmZB8rQF58GlSK5mjX1RbrSXnS7OjkPhqjjKcArd6sDAz83V8zltWogJMsosYJHt7AIz60XTetwUiOmz7OS4rBllLvqBDsW1niOZBKKZBweWAdcasedZBNjbNfoVntlWFx7Uc2hpSR9ROWYAWjXqdHoyjkXafceeJsmCuTKDwZCED -F prevent_account_creation=true https://api.airbnb.com/v1/authorize"

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
	{ key: "assertion_type", value: "https://graph.facebook.com/me", description: "Required for Facebook authentication." },
	{ key: "prevent_account_creation", value: "true", description: "For sign-in, as opposed to registration." }
]

required_form_parameters: [
	{ key: "assertion", value: "CAAAAIEMtwcwBAMTO70riSczKIgT3Nv0E...", description: "Facebook user's access token." }
]
---
{% include JB/setup %}
