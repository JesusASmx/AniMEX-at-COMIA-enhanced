###### _For the ones who asked in the COMIA conference for the enhanced results :)


# Anime Project at COMIA, enhanced results!

Here you can find the code for our paper at COMIA2023 (Mexican Conference of Articial Intelligence), but with this changes:
* Instead of using the split described on the paper (who considers the genre balancing), we consider the maximum amount of samples. Results here droped from 0.55 to 0.51/0.50 (i.e. models were unable to detect correlation). As a concequence, we decide to add TF-IDF (and the results upgraded an average of 13 points!).
* We consider two cases: where an anime is unpopular when its score is 7 or below (called 7-binary), and where 6.62 is the thresshold of popularity (called Balanced).
* We added TF-IDF. This is the leaderboard of all macro F1's:

1. **7-binary Support Vector Machine:** 0.776
1. **7-binary MultiLayer Perceptron:** 0.767
1. **7-binary Logistic Regression:** 0.765
1. **Balanced Support Vector Machine:** 0.714
1. **Balanced Logistic Regression:** 0.709
1. **Balanced MultiLayer Perceptron:** 0.685

Conclusions: This 13-point jump should not be surprising. Quick statistics shows that this complex phenomenom is underrepresented by our data (and, unfortunately, by any free data available), and we have the biased luck to obtain clusters separable by simplest methods such as Logistic Regression. Moreover, SVM outperforming everyone suggests that the boundaries between clusters are multilineal (if we remove some samples, we can even solve the task with a mere horizontal line).
