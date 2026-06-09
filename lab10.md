# Stressor analysis

Have the following columns

- Stressor #
- Stressor Name
- Detection
- Attractor: Business impact
- Attractor: Business Reaction
- Residue (delta)

## Exercise

|#|Name|Detection|Attractor: Business Impact|Attractor: Business reaction|Residue (delta)|
|---|---|---|---|---|---|
|1|Giant fire-breathing lizard destroys competitor|-|News, smoke|Less volume of offers requested|We stop sending them offer requests and stop listening to their own channel; we remove them as a party|We need a management compenent for competitors (add, remove)
|2|Competitor API down|Timeouts/monitoring|Delay in getting/sending requests|Retry of use asynchronous mecanism|Retry mecanism|
|3|Competitor API contract change|Error rate/monitoring or they notify us|No request processed until resolution|We have to change our integration|Contract testing or business protocol for api changes to give time to adapt adapter|
|4|Competitor mortgage model/parameters change|Notificatiton and errors|Errors/no more processed|idem|idem|
|4b|New model parameters|Notification|New data to process|Update model to be able to provide/process it|Adapter and mortgage rate request model update|
|5a|We add parameters to our own data model|Internal decision|Inaccurate mortgage predictions|We request it from the customer or we propose an agreement to competitors to provide the data|Request or agreement with competitor or establish a body to help intermediate in those information requests|
|5b|We stop using some model parameters|Internal deicison|-|We may remove the data collection|We maintain the required parameters from competitors to know if they still need it. They might want to maintain our own API descriptions that show the parameters we are still using. + notifications on API/parameters changes Historical DB clean?|
|6|Intermediate broker needs to centralize the comparison app|Legal notice||We move those features to broker. We don't need to integrate/maintain alist of competitors.|Remove adaptors, keep one to the broker app|
|7|Our competitor uses dummy customers to do rate comparisons|||Dummy requests could get marketing information about our strategy|Add common person identifier to the request. Attention privacy regulations|
|8|Regulatory changes; immediate rate comparisons required|Legal notification|Real-time mortgage quoting and loading|Sytem adaption|Real time apis, inform user if retrieval didn't work for a competitor. Timeout for rate retrieval|
|9|Comparison over additional products|Business decision|Adapt the system|Adapt the system|Typed APIs or typed messages|
|10|Competitors sends us garbage data|Errors/validation errors|We can't provide rates|Notify the competitor that it needs to fix stuff/decline his message|Legal cohersion to fix the issue as we lose potential customers|
|11|Mortgage calculator is down|test|test|test|test|
|12|Fusion/acquisition of competitor|test|test|test|test|
|13|Merger of banks|test|test|test|test|
|14|Competitor does not respond to the customer|test|test|test|
|15|Customer sends multiple requests|test|test|test|
|16|Identity fraud by customer|test|test|test|
|17|DDOS by the banks/customers|test|test|test|
|18|Standardization requirements of the API|test|test|test|
|19|Regulation auditing for ten years|test|test|test|
|20|Maximum retention times|test|test|test|
|21|Customer removes consent|test|test|test|
|22|DDOS attack|test|test|test|
|23|Competitor impersonation by hacker|test|test|test|
|24|Malicious abuse of our API|test|test|test|
|25|Withdrawing of competitor|test|test|test|
|26|Egress/ingress costs higher than expected|test|test|test|
|27|Regution change: imposed data model that do not fit ours|test|test|test|
|28|Change of policy on what we want to publish|test|test|test|
|29|Marketing wants to propose a markdown on rate quoted|test|test|test|
|30|Interest rates changes|test|test|test|
|31|Customer request for unsupported country|test|test|test|
|32|Housing crisis: nobody buys homes|test|
|33|Competitor with smaller costs always underquote you/proposes smaller costs|test|
|34|Environmental regulation: additional checks to do on each home|test|
|35|Environmental regulation: additional checks to do on each home|test|
|36|Multilingual requirements|test|
|37|multicurrency requirements|test|
|38|Change from national to european scope|test|
|39|Multiple rates scenario|test|
|40|Migration cloud to on-prem|test|
|41|Network congestion because of this system|test|
|42|Malicious content in the files send by banks|test|
|43|Dangerous firewall rules|test|
|44|Americans request access to customer details - banks owned by foreign mother company|test|
|45|Database corruption|test|
|46|Cloud is down|test|
|47|Mortgage calculation needs to be transparent to customer|test|
|48|How would mortgage brokers interact with the system|test|
|49|Customer dies: do we need to keep the data|test|
|50|What if we want to keep all competitor offers for analytics?|test|
|51|Competitor fraud; wrong mortage rates shared|test|
|52|Slow sharing of offers by competitor|test|
|53|Application can be reached from multiple devices|test|
|54|Customer identity verification required|test|
|55|Customer blacklisted|test|
|56|Information asymmetry about clients shared|test|
|57|Package deals of competitors mispresenting their rate|test|
|58|Mortgage rate needs to be public and we are forced to only use some parameters|test|
|59|Transparency to governement on offers made|test|
|60|Marketing promises unrealistic mortgage rates|test|
|61|AI agents recurring requests DDOS on the service|test|
|62|Management wants to use AI for mortgage calculation|test|
|63|Regulation: every proposal needs to be approved by human|test|
|64|Bank wants to offer competitive rate requests via chatbot/whatapp/sms|test|
|65|Businesses want to also use that calculator and system|test|
|66|Bank needs to followup on every customer|test|
|67|Big data storage|test|
|68|Nuclear apocalypse: how to do the process by hand|test|
|69|Invasion of Europe|test|
|70|Worldwide hardware shortage|test|
|71|Dissolution of European union/the euro|test|
|72|Hyperinflation: we don't know what mortage we can give|test|
|73|Comparing exotic mortagage products (dynamic rates, etc)|test|
|74|Unification of Europe: bigger market|test|
|75|Outsourcing/swap out of the mortgage system|test|
|76|What if regulation force you to have a MCP to request mortgages?|test|
|77|Legal requirement to not share personal information|test|
|78|Preferential rates (bank employees) lower the quality of rates provided by your competitors|test|


