# Covid19-WebScrape-Plus
Brand New to Github and still getting this dataset compiled.  As timeseries data from BNO, Worldometer, and Wiki just started, I need to supplement with JHU data up to that date.  I then will probably create a "fixed" JHU timeseries with a few of the obvious errors corrected and put out a base dataset that is supplemented with past two days of data.  More to come.  See more stuff below.

Just started working on this as I'm doing coronavirus for my Master's thesis. Starting with just the raw data. BNO and Worldometer are manually scraped as often as I can, then using a script to create the csv. Wikipedia is scraped with a script, but I have not scheduled it yet. This isn't a complete time series, but meant to act as a "live feed" and log to fix/supplement JHU data with "current" numbers as their github is usually once a day update. Link to folder at bottom of post.

An example of a JHU issue is recently they had a day where UK has 1 new case. The idea is I can keep a "fixed jhu" csv at some point with a log of points that were corrected. I'm going to work on scraping time series data for states/territories/provinces/counties for the major countries being hit next, as the wikipedia pages for most seem to have this and are relatively reliable and I should be able to automate a pull from there. Still exploring everything.

JHU Dataset github for reference: https://github.com/CSSEGISandData/COVID-19

Currently each data set is stored in a csv as shown and also unpivoted with "type". Planning on adding multiple fields to each such as Active, Days in, Days in First Death, New Cases, Previous New, etc..

Let me know if you have requests for fields or just anything else related to coronavirus datasets. Main need probably will be lat and long. Haven't started looking into adding this on yet EXCEPT for the wiki pull which I formatted to match the johns hopkins data set. See note below. I know there are some automatic tools for this.

I've also never done github, but I can probably figure that out shortly. For now they are stored in a google drive shared folder.

SOURCES:

BNO - https://bnonews.com/index.php/2020/02/the-latest-coronavirus-cases/

World - US - Australia - Canada links

Worldometer - https://www.worldometers.info/coronavirus/

Wikipedia

US - https://en.wikipedia.org/wiki/2020_coronavirus_pandemic_in_the_United_States

World - https://en.wikipedia.org/wiki/2019%E2%80%9320_coronavirus_pandemic_by_country_and_territory

NOTE: wiki_jhu_unpivot attempts to map the wikipedia data to the same format as unpivoted JHU dataset. This includes mapping country names and also mapping their lat/long coordinates. My original thought is to add this on top of their dataset for updates throughout the day.. but haven't finished that yet.

FOLDER

https://drive.google.com/open?id=1--t62vjrh8DC-lPYFvPGm2P4Qc7JSzNf