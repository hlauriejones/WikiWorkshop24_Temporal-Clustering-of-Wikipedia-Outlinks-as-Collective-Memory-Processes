# WikiWorkshop_Temporal-Clustering-of-Wikipedia-Outlinks-as-Collective-Memory-Processes

Wikipedia can be a site of collective memory processes. The outlinks present in Wikipedia articles related to the 2011 Arab Spring are analyzed and compared across English and Arabic language editions. An inductive analysis identifies three latent classes of link addition and removal behavior reflecting distinctive forgetting and remembering processes.

**Introduction**

Wikipedia’s revision histories for articles about contemporary events are compelling empirical sites to observe processes related to framing, sensemaking, and collective memory (Ferron and Massa, 2011; Luyt, 2016; Porter et al., 2020). Wikipedia is available across language editions and there are no requirements or guarantees that different language editions discuss topics similarly. There is an assumption that the linguistic editions of Wikipedia represent the linguistic community that speaks it (Bao et al., 2012; Hale, 2014). Outlinks help readers navigate through related topics and are strong signals of relation-
ships between articles. We combine revision histories, language editions, and outlinks to identify and compare temporal clusters of outlinks in Wikipedia articles over time as proxies for collective memory practices.

**Methods**

The revision histories for the English and Arabic articles for the “Arab Spring” and a monthly sample of revision content was retrieved using the MediaWiki API. The revision content was filtered to body text (paragraph tags), outlinks were parsed from this content, and outlink redirects were resolved. For each revision in the sample, the outlinks were one hot encoded as a binary vector of whether the link was present and these vectors were concatenated to produce a binary matrix of revisions by out-
links. Pairwise similarities between outlinks were computed using a cosine similarity distance metric to measure which links co-occurred with each other across time. This symmetric outlink similarity matrix was hierarchically clustered and iterated until it converged on interpretable findings. Outlinks’ cluster membership was then qualita-
tively evaluated. The count of outlinks belonging to each cluster were aggregated as time series.

**References**

[Bao et al.2012] Patti Bao, Brent Hecht, Samuel Carton,
Mahmood Quaderi, Michael Horn, and Darren Gergle.
2012. Omnipedia: Bridging the wikipedia language gap.
In Proceedings of the SIGCHI Conference on Human
Factors in Computing Systems, CHI ’12, pages 1075–
1084, New York, NY, USA. ACM.

[Ferron and Massa2011] Michela Ferron and Paolo
Massa. 2011. Collective memory building in Wikipedia:
the case of North African uprisings. In Proceedings of the
7th International Symposium on Wikis and Open Collab-
oration, WikiSym ’11, pages 114–123, New York, NY,
USA, October. Association for Computing Machinery.

[Hale2014] Scott A. Hale. 2014. Multilinguals and
Wikipedia editing. In Proceedings of the 2014 ACM
conference on Web science, WebSci ’14, pages 99–108,
New York, NY, USA, June. Association for Computing
Machinery.

[Luyt2016] Brendan Luyt. 2016. Wikipedia, collective
memory, and the vietnam war. Journal of the Association
for Information Science and Technology, 67(8):1956–
1961, August.

[Porter et al.2020] Emily Porter, P. M. Krafft, and Brian
Keegan. 2020. Visual narratives and collective memory
across peer-produced accounts of contested sociopolit-
ical events. ACM Transactions on Social Computing,
3(1):4:1–4:20, February.