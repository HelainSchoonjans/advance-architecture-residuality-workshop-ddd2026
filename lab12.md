# incidence matrix

Make one for the stressors and the architecture - is there some missing spots?

## Stressors

|#|Name|Detection|Attractor: Business Impact|Attractor: Business reaction|Residue (delta)|
|---|---|---|---|---|---|
|1|Giant fire-breathing lizard destroys competitor|-|News, smoke|Less volume of offers requested|We stop sending them offer requests and stop listening to their own channel; we remove them as a party|We need a management compenent for competitors (add, remove)
|2|Competitor API down|Timeouts/monitoring|Delay in getting/sending requests|Retry or use asynchronous mecanism|Retry mecanism|
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

## Incidence matrix

||Customer management|quotation ui|competition mgt ui|comparison ui|mortgage quotation adapter|customer directory|quote archive|competitor repository|comparison backen|competitor rate adapter|retry mecanism|quotation api|Total
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Giant fire-breathing lizard destroys competitor|0|0|0|0|0|0|0|1|1|1|1|0|4
|Competitor API down|0|0|0|0|0|0|0|0|0|0|1|0|1
|Competitor API contract change|0|0|0|0|0|0|0|0|0|1|0|0|1
|Competitor mortgage model/parameters change|0|0|0|0|0|0|0|1|0|1|0|0|2
|New model parameters|0|1|0|0|0|0|0|0|1|0|0|0|2
|We add parameters to our own data model|0|1|0|0|0|0|0|0|1|0|0|0|2
|We stop using some model parameters|0|1|0|0|0|0|0|0|1|0|0|1|3
|Intermediate broker needs to centralize the comparison app|1|1|1|1|1|1|0|0|0|0|0|0|6
|Our competitor uses dummy customers to do rate comparisons|0|0|0|0|0|0|0|0|0|0|0|0|0
|Regulatory changes; immediate rate comparisons required|0|1|1|1|1|0|0|0|0|0|0|0|4
|Comparison over additional products|1|1|1|1|1|1|1|0|0|0|0|0|7
|Competitors sends us garbage data|0|0|0|0|0|0|0|0|0|1|1|0|2
|Total|2|6|3|3|3|2|1|2|4|4|3|1|34