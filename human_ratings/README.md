# Human Ratings of Simplifications

In this folder you will find the ratings that were used in section 6 "Evaluating Evaluation Metrics" of the paper.



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
