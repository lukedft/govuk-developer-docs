---
owner_slack: "#search-team"
title: Check for spelling suggestions failed
parent: "/manual.html"
layout: manual_layout
section: Icinga alerts
last_reviewed_on: 2017-10-02
review_in: 3 months
---

Indicates that the Jenkins [search_test_spelling_suggestions healthcheck job]
(https://deploy.publishing.service.gov.uk/job/search_test_spelling_suggestions/)
has failed.

The healthcheck sends queries to the search API and checks that the response
contains the expected spelling suggestions.

The Jenkins job will still succeed even if the search results are poor and will
only fail if something actually goes wrong. For example, if a request to the
search API fails.

Check the output of the job on the relevant environment for more information.
