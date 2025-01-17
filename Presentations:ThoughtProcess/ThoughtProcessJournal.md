Week of 2/24/19
---------------

-   At this stage, I was looking for a way to make my "evictions" dataset work. However, I realized it would be practically unrealistic to find outcomes for evictions cases, for the following reasons:

-   Web scraped the [2018 Landlord Watchlist](https://landlordwatchlist.com/)
-   The landlord tenant cases are removed from the eCourts systems 2 weeks after dispostion. I tried to input some case numbers from [Marshal Evictions](https://data.cityofnewyork.us/City-Government/Evictions/6z8x-wfk4/data) but none worked :frowning:
-   Luckily I was able to find the [Housing Litgations](https://data.cityofnewyork.us/Housing-Development/Housing-Litigations/59kj-x8nc) dataset. This dataset has outcomes of cases involving tenant harassment.
-   I realized that this dataset can give me what I need because it has *some* case outcomes for tenant harassment cases. After fitlering for what I need, I realize that I have a dataset of about 1300 observations!

Week of 3/3/19
--------------

-   Initial exploration of the Housing Litigations dataset
-   Exploratory analysis and connected it to pluto dataset
-   Also connected the Evictions dataset to the pluto dataset
-   Downloaded a database from [Are you rent stablized](https://chenrick.carto.com/datasets), joined evictions and harassment datasets to this database

Week of 3/10/19
---------------

-   Realized that the Housing Litigations dataset might be biased bc there are about 900 no harassment cases and 100 harassment case findings
-   Should probably include all cases even if they are not tenant harassment cases, but cold water, no heat etc.
-   Today, Clare have me the idea to do a spatial cluster analysis that would incorporate the following: 1. Identify where evictions are filed 2. Identify where Harassment and other cases are filed 3. different types of work order 311 complaints 4. In sum, do all these overlap? Are hotspots of evictions filings mapping to hotspots of harassment cases

Week of 3/11/19
---------------

-   Did preliminary spatial analyses (maps) + exploratory anlyases (graphs)
-   Realized that studying evictions is impossible because it is multifaceted. However, I discovered that I am more interested in the aftermath of evictions. In other words, examining displacement patterns in NYC.
-   I rediscovered the NYC Housing Vacancy Survey and downloaded the 2017 survey results.I can do a cross sectional analysis of this dataset
-   With the NYC Housing Vacancy Survey, I can see where people reside after being evicted from their former residence. I can also see where people now reside for a variety of other reasons (seeking greater housing affordability, moving to be close to work, moving to be close relatives). Therefore, I can examine 'moving' patterns for truly evicted v. those who are seeking different opportunities.
-   The NYC HVS is good because it gives me estimates for individuals, as well as, their demographics. However, there are some shortcomings that I will note as I continue with the project, as well as on my final deliverable.
-   Rediscovered this article: *The Right to Stay Put, Revisited: Gentrification and Resistance to Displacement in New York City*, I think I will do a replication of this study for 2017 data.

Weeks of 3/18/19 + 3/25/19
--------------------------

-   Not much progress still connfused on how I would use the NYCHVS
-   The week leading up to 3/25/19, I was preparing for the midterm presentation, I did alot of exploratory analysis, mapping, etc.
-   I fumbled in these two weeks because I did not clean the entire datatset, which I should have retrospectively reflecting on this.
-   After 3/25/19, we got our feedback and that left me more confused on what I wanted to do with the survey

Week of 4/1/19
--------------

-   I got feedback on running structural models, which left me confused. I know I researched SEM in the Psychology sense and then structural equations in the Economics sense and both left me pretty confused.
-   This week I did not accomplish much to be honest except being confused on what my options were.

Week of 4/8/19
--------------

-   Met with Yoav this week and was suggested to read the *Book of Why* to create a causal model to understand the evictions process.
-   By the end of the week I ended up reeading the first 7 chapters. Unfortunately, this is all that I have read (by the end of the project), but I did learn the general idea about the other side of causal inference.

Week of 4/15/19
---------------

-   Drafted causal diagrams and my causal model.
-   Completely cleaned the NYCHVS 2017 for households and NYCHVS 2017 for individuals and joined them

Week of 4/22/19
---------------

-   Decided to role with my 'income/rent' causal model, therefore I started pulling data from the 2017 American Community Survey
-   I also scraped data from NYU Furman's Center
-   Created indicator variables that would suggest if a household's income was less than their neighborhood's median household income. Also if a household's rent was less than their neighborhood's median rent.
-   Ran preliminary models and educated myself on the *survey* R package!

Week of 4/29/19
---------------

-   Preparation for final presentation (primarily happened on the weekend - I was pulled into 2 emergency work meetings!)
-   EDA keeping in mind new focus on economic constraints
-   Finalized models, images, and explanations of Judea Pearl's causal inference!

Week of 5/6/19
--------------

-   Presentations are today...hopefully with some feedback, I can look into the neighborhood idea :)
