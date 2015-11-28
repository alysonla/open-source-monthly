# Open Source Monthly

This is a repo to track issues for the Open Source Monthly dashboard.

![open-source-monthly-filters](https://cloud.githubusercontent.com/assets/2623954/10778809/99c4113c-7ce6-11e5-8141-fcbff5fdc66b.gif)

The dashboard shows the activity on GitHub.com for open source Organizations by month. Data is pulled from the [githubarchive](https://www.githubarchive.org/), which is collected from the GitHub [Events API](https://developer.github.com/v3/activity/events/types/).

http://alysonla.github.io/open-source-monthly/

_Note: It may be somewhat slow to load at first as it's querying ~90k orgs & 6M rows of data._

## About the charts:

On the __left__ side is a __bar chart__ of total "Event Types" for each activity type on GitHub.com stored on the GitHub Archive. On the __right__ is a __time series chart__ showing the total org events (contributions) by day as a solid line as well as a dotted trend line. __Below__ is a __tree map chart__ that shows the repos in the org - the more contributions, the larger the box.

Hover over the charts for tooltips & on the org octicon for more information.

If you're curious about a certain repo, click on the box & the other charts will update to reflect the breakdown of event types & timeline specific to that repo.

If you're curious about a certain spike, you can click on the date & again the charts will update.

Looking at the facebook org, you can click on the 'Public' event & see that fb open sourced these 9 repos last month. :tada:

<img width="1037" alt="screenshot 2015-10-27 19 31 39" src="https://cloud.githubusercontent.com/assets/2623954/10778829/bacd0618-7ce6-11e5-976a-98bed3c9c5ec.png">

To remove filters, click in the bottom left corner of the chart or click __‘reset’__.

Last, you can pick more than one org to compare activity.

<img width="1034" alt="screenshot 2015-10-24 19 40 24" src="https://cloud.githubusercontent.com/assets/2623954/10778836/cde34c9e-7ce6-11e5-9974-81bfa318dd8d.png">

### Technical details

This dashboard was built using [Tableau](http://www.tableau.com/) & is hosted for free on [Tableau Public](https://public.tableau.com/s/) (like GitHub.com but for data analysts). Hosting is limited to 10M rows & this filtered data set came to ~6M rows. Data is pulled using the Tableau / Google BigQuery native connector.

### Glossary

Click [here](https://docs.google.com/spreadsheets/d/11nuCoX39ezNzlM3_Mz_gG14R82AnMR8de-oD4P9LclM/edit#gid=0&vpid=A2) for a glossary of terms.

### Resources

* [Google BigQuery Tutorial](https://www.thinkful.com/learn/google-bigquery-tutorial/)
* [Tableau Public Resources](https://public.tableau.com/s/resources)
