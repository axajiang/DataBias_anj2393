# DataBias_anj2393

This project tests the Perspective API toxicity model for bias against capitalization and case-sensitivity through running comments and queries into the model and measuring their accuracy dependent on their capitalization. This will tested using the scale of anything above 0.5 as toxic and less than 0.5 as non-toxic. 

My hypothesis was that the Perspective model will be less likely to mark all lower case content as toxic than capitalized content, even if the written content is the same.

# Results
For the 10 toxic lowercase comments, 9 out of 10 were correctly analyzed and rated, giving the Perspective model a 90% accuracy rate.

For the 10 non-toxic lowercase comments, 10 out of 10 were correctly analyzed and rated, giving the Perspective model a 100% accuracy rate.

For the 10 toxic uppercase comments, 9 out of 10 were correctly analyzed and rated, giving the Perspective model a 90% accuracy rate.

For the 10 non-toxic uppercase comments, 9 out of 10 were correctly analyzed and rated, giving the Perspective model a 90% accuracy rate.


Based on these results, I learned that the model is slightly biased towards uppercase capitalization of comments, even though the content is the same - uppercase content tends to be rated as more toxic solely because of its capitalization. I was surprised by how close the accuracy percentages were, and also how the capitalization did not seem to have a large effect on the toxicity value for already toxic content, but more heavily influenced the nontoxic content. 

I think biases relevant to case-sensitivity or capitalization might exist in the model because more instances of toxic language are likely to be uppercase, biasing the model to assume that uppercase capitalization is indicative of toxicity. It is likely the model was made with public comments or entries, where most of the time people do not type in all-caps unless it is emphatic, typically to denote yelling or threatening - both associated with online toxicity. This assignment may me more deeply consider the importance of regulating machine learning models and training with clean data to avoid bias, even for small grammatical things like capitalization. It is difficult to tell from just the toxicity results how the model comes to its conclusion, so testing for bias becomes increasingly important. 
