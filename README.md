_For the ones who asked for the enhanced results, I apologize to wait so long to publicly upload the code :) I delayed so long since I decided to put everything in the next paper. However, sinice I decided to scrap a new dataset for that paper, here you have the enhanced results, as promised! :)_


**Anime Project at COMIA, enhanced results!**

Here you can find the code for our paper at COMIA2023 (Mexican Conference of Articial Intelligence), but with this changes:
1.- Instead of using the split described on the paper (who considers the genre balancing), we consider the maximum amount of samples. Results here droped from 0.55 to 0.51/0.50 (i.e. totally random)
2.- We consider two cases: where an anime is unpopular when its score is 7 or below (called 7-binary), and where 6.62 is the thresshold of popularity (called Balanced).
3.- We added TF-IDF. This is the leaderboard of all macro F1's:

1.- **7-binary Support Vector Machine:** 0.776
2.- **7-binary MultiLayer Perceptron:** 0.767
3.- **7-binary Logistic Regression:** 0.765
4.- **Balanced Support Vector Machine:** 0.714
5.- **Balanced Logistic Regression:** 0.709
6.- **Balanced MultiLayer Perceptron:** 0.685
