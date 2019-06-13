# Concordance_Based_Metrics_Survival
In this project, we implement joint concordance index (from https://arxiv.org/pdf/1810.11207.pdf) and concordance index (Wolbers et.al.). An application to compute joint cnocordance index is https://mlinterpreter.shinyapps.io/concordance/. 

Functions defined below can be found in New_Cindex_paper_upload.Rmd

## Cindex_estimator_efficient: function to compute the concordance index (from Wolbers) 
Input: Prediction vector for the event type of interest (risk predicted by the model for the event type of interest), 

Time_survival: time-to-event data for each subject,  

Censoring: censoring information for each subject, 0 is censored and 1 is not censored

Cause: event type of interest, 

Time: time horizon at which c-index is computed

Output: Concordance index

## JCindex_estimator_combined 

Input: 

Prediction matrix: prediction vector for each event type stacked into a matrix, 

Time_survival: time-to-event data for each subject,  

Censoring: censoring information for each subject,  0 is censored and 1 is not censored

Cause: event type of interest, 

Time: time horizon at which c-index is computed, 

type_estimator: 'naive' or 'weighted'

Output: Joint Concordance index

## References

[1] Wolbers, M., Blanche, P., Koller, M. T., Witteman, J. C., & Gerds, T. A. (2014). Concordance for prognostic models with competing risks. Biostatistics, 15(3), 526-539.
