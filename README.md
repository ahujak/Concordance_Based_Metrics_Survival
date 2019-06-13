# Concordance_Based_Metrics_Survival
In this project, we implement joint concordance index (from https://arxiv.org/pdf/1810.11207.pdf) and concordance index (Wolbers et.al.). 
## Cindex_estimator_efficient: function to compute the concordance index (from Wolbers) 
Input: Prediction vector for the event type of interest (risk predicted by the model for the event type of interest), 

Time_survival: time-to-event data for each subject,  

Censoring: censoring information for each subject, 

Cause: event type of interest, 

Time: time horizon at which c-index is computed

Output: Concordance index
