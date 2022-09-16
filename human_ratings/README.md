# Human Ratings of Simplifications

In this folder you will find the ratings that were used in sections 5 "Rating Simplifications in ASSET" and 6 "Evaluating Evaluation Metrics" of the paper.

# Section 5 - "Rating Simplifications in ASSET"

File: `asset_pairwise_comparisons_with_turkcorpus_and_hsplit.csv`

## Collection of Human Ratings
Description extracted from the paper:
> For each of the 359 original sentences in the test set, we randomly sampled one reference simplification from ASSET and one from TurkCorpus, and then asked qualified workers to choose which simplification answers best each of the following questions:  
• Fluency: Which sentence is more fluent?  
• Meaning: Which sentence expresses the original meaning the best?  
• Simplicity: Which sentence is easier to read and understand?
Workers were also allowed to judge simplifications as “similar” when they could not determine which one was better. The same process was followed to compare simplifications in ASSET against those in HSplit.

Details in 

# Section 6 - "Evaluating Evaluation Metrics"

File: `human_ratings.csv`

## Collection of Human Ratings
Description extracted from the paper:
> We randomly chose 100 original sentences from ASSET and, for each of them, we sampled one system simplification. The automatic simplifications were selected so that the distribution of simplification transformations (e.g. sentence splitting, compression, paraphrases) would match that from human simplifications in ASSET. That was done so that we could obtain a sample that has variability in the types of rewritings performed. For each sentence pair (original and automatic simplification), we crowdsourced 15 human ratings on fluency (i.e. grammaticality), adequacy (i.e. meaning preservation) and simplicity, using the same worker selection criteria and HIT design of the Qualification Test as in § 5.1.

## File format
The ratings are in a .csv format where columns are the following:
* **original**: Plain text original sentence.
* **simplification**: Plain text system simplification sampled from multiple systems (Hybrid, PBMT-R, SBMT-SARI, ACCESS, DMASS-DCSS, NTS-SARI).
* **original\_sentence\_id**: Positional id of the original sentence in the ASSET test set.
* **aspect**: Aspect that is evaluated: meaning, fluency and simplicity.
* **worker\_id**: Anonymised worker id.
* **rating**: Human rating in the range of 0 to 100 included.
