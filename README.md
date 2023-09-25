###### _For the ones who asked in the COMIA conference for the enhanced results, I apologize to wait so long to publicly upload the code. I delayed so long since I was thinking to include them into the next paper but, considering that I decided to scrap a new dataset for that paper, here you have the enhanced results, as promised! :)_


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

Conclusions: This 13-point jump is almost unreal considering the complexity of the dataset. We suspect that it is due some sort of overfitting, considering that results drop 6-7 points in the so-called "Balanced" dataset, with almost 10,000 samples, while the 7-binary dataset has around 6000 samples.
