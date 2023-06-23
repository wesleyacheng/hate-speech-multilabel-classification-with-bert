# hate-speech-multilabel-classification-with-bert

First posted on [Kaggle](https://www.kaggle.com/code/wesleyacheng/hate-speech-multilabel-classification-with-bert).

I've recently stumbled upon a very comprehensive dataset on measurement of hate speech from my alma mater, UC Berkeley. It aggregated social media comments from Youtube, Reddit, and Twitter.

The interesting thing about the dataset is the annotator's profile with attributes such as ideology, income, race, and etc. is included in the dataset. This is, unfortunately, uncommon in most social media dataset and so I was intrigued about this.
I also find the paper's idea of data perspectivism interesting as it argues that the disagreement of the annotator on the attributes of a hate speech is informative, rather than throwing it away.

<img width="1110" alt="hate speech distribution" src="https://github.com/wesleyacheng/hate-speech-multilabel-classification-with-bert/assets/15952538/11e0909a-f8b6-4349-9d4c-ae8effc65b90">


Although, we are not leveraging the annotator's information in this model, I encourage you to explore the dataset and maybe leverage the annotator's information to make variations of this classifier.

Here I made a Hate Speech MultiLabel Classifier to classify independent targets of race, religion, origin, gender, sexuality, age, disability by doing transfer learning on [BERT](https://huggingface.co/datasets/ucberkeley-dlab/measuring-hate-speech) with the [UC Berkeley D-Lab's Hate Speech Dataset](https://huggingface.co/datasets/ucberkeley-dlab/measuring-hate-speech) from the paper [The Measuring Hate Speech Corpus: Leveraging Rasch Measurement Theory for Data Perspectivism](https://aclanthology.org/2022.nlperspectives-1.11.pdf).
