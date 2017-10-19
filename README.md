Page-Views-on-English-Wikipedia

The purpose of the project is to do the Data Curation on a dataset of monthly traffic on English Wikipedia from Januray 2008 to September 2017. In this project, two different API endpoints, Pagecounts API and Pageviews API, are needed to collect the required data.

The legacy Pagecounts API provides access to desktop and mobile traffic data from January 2008 through July 2016. (https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end)

The Pageviews API provides access to desktop, mobile web, and mobile app traffic data from July 2015 through September 2017. (https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end )


Data

The data_pageviews_pagecounts.ipynb file downloads the Pagecounts and Pageviews data from Wikipedia.

Pagecounts gives the desktop and mobile traffic data from January 2008 to July 2016.

Pageviews gives the desktop, mobile web and mobile app data from July 2015 to September 2017.

plot_pageviews_pagecounts.R plots the trafiic data that is downloaded from data_pageviews_pagecounts.ipynb

A final dataset is created with the following fields

Year

Month

Pagecount_all_views

Pagecount_desktop_views

Pagecount_mobile_views

Pageview_all_views

Pageview_desktop_views

Pageview_mobile_views



Analysis

A time series graph is created from the dataset. It represents the mobile and desktop traffic data of both Pagecounts and Pageviews, and also the total mobile and desktop data for each of the APIs.