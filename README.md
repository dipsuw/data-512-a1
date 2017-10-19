# data-512-a1
Repository for Data curation assignment in D516
## Goal of the project:
Goal of the project is to create a reproducible workflow for constructing, analyzing, and publishing a dataset of monthly traffic on English Wikipedia from July 1 2008 through September 30 2017. The three central stages of reproducible workflow are: 
* data processing
* data analysis
* data analysis
## Data Curation
Data curation is the management of data throughout its lifecycle, from creation and initial storage to the time when it is archived or becomes obsolete and is deleted. 
## License of the source data
* MIT License(https://opensource.org/licenses/MIT)
## Wikimedia Foundation terms of use
https://wikimediafoundation.org/wiki/Terms_of_Use/en
## Relevant API documentation
* The legacy Pagecounts API (documentation, endpoint) provides access to desktop and mobile traffic data from January 2008 through July 2016. [Documentation for pagecount](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts)
* The Pageviews API (documentation, endpoint) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through September 2017. [Documentation for pageviews](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)
## Source data
Json files from api calls:
* pagecounts_desktop-site_200801-201607
* pagecounts_mobile-site_200801-201607
* pageviews_all-sites_201507-201709
* pageviews_mobile-app_201507-201709
* pageviews_mobile-web_201507-201709
## Final data
* en-wikipedia_traffic_200801-201709
#### Values of all fields in Final data file
Column name | Value | Description
--- | --- | ---
year | YYYY | Year of Wikipedia traffic from 2008-2017
month | MM | Month of Wikipedia traffic from Jan 2008- Sept 2017
timestamp | MMDDYYYY | Timestamp(Datetime format)to create the time series chart
pagecount_all_views | num_views | Number of pagecounts for mobile and desktop
pagecount_desktop_views | num_views | Number of pagecounts for desktop
pagecount_mobile_views | num_views | Number of pagecounts for mobile
pageview_all_views | num_views | Number of pageviews for mobile and desktop
pageview_desktop_views | num_views | Number of pageviews for desktop
pageview_mobile_views | num_views | Number of pageviews for mobile

## Known issues or special considerations with the data 
* Pageview API excludes spiders/crawlers, while data from the Pagecounts API does not.

## Visualization of data

