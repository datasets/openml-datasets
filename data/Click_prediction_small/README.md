The resources for this dataset can be found at https://www.openml.org/d/1219

Author: Tencent Inc.  
Source: [KDD Cup](https://www.kddcup2012.org/) - 2012  
Please cite:   

This data is derived from the 2012 KDD Cup. The data is subsampled to 1% of the original number of instances, downsampling the majority class (click=0) so that the target feature is reasonably balanced (5 to 1).

The data is about advertisements shown alongside search results in a search engine, and whether or not people clicked on these ads. 
The task is to build the best possible model to predict whether a user will click on a given ad.

A search session contains information on user id, the query issued by the user, ads displayed to the user, and target feature indicating whether a user clicked at least one of the ads in this session. The number of ads displayed to a user in a session is called ‘depth’. The order of an ad in the displayed list is called ‘position’.  An ad is displayed as a short text called ‘title’, followed by a slightly longer text called ’description’, and a URL  called ‘display URL’.   
To construct this dataset each session was split into multiple instances. Each instance describes an ad displayed under a certain setting  (‘depth’, ‘position’).  Instances with the same user id, ad id, query, and setting are merged. Each ad and each user have some additional properties located in separate data files that can be looked up using ids in the instances.

The dataset has the following features:  
* Click – binary variable indicating whether a user clicked on at least one ad. 
* Impression - the number of search sessions in which AdID was impressed by UserID who issued Query.
* Url_hash - URL is hashed for anonymity
* AdID 
* AdvertiserID - some advertisers consistently optimize their ads, so the title and description of their ads are more attractive than those of others’ ads.
* Depth - number of ads displayed to a user in a session
* Position - order of an ad in the displayed list
* QueryID - is the key of the data file 'queryid_tokensid.txt'. (follow the link to the original KDD Cup page, track 2)
* KeywordID - is the key of  'purchasedkeyword_tokensid.txt' (follow the link to the original KDD Cup page, track 2)
* TitleID - is the key of 'titleid_tokensid.txt'
* DescriptionID - is the key of 'descriptionid_tokensid.txt' (follow the link to the original KDD Cup page, track 2)
* UserID – is also the key of 'userid_profile.txt' (follow the link to the original KDD Cup page, track 2). 0 is a special value denoting that the user could be identified.