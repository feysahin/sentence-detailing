# Sentence Detailing and Its Applications
The repository of the study of "Sentence Detailing and Its Applications" which suggests a new method for data augmentation in Turkish language.

This paper was studied by [Feyza Sahin](https://github.com/feysahin) and [Mehmet Fatih Aamasyali](https://github.com/mfatihamasyali) with the contributions of [Besher Alkurdi](https://github.com/mrbesher).

## Dataset
[TR-News](https://huggingface.co/datasets/batubayk/TR-News)

## Codes
In the folder `codes` we have preprocessing, training and classification code files.

`sort_date.ipynb`: After the dataset is sorted by date, it is splitted into train and test set with %90 and %10 percentages respectively and the train set is halved for several times. 

`create_ws`: The data set created here consists of sentences as labels and words of these sentences as input.

`preprocess_datasets`: Standardization of the dataset by the topic column was applied.
1000 samples was chosen by the selected topic classes.
Preprocessing was applied to both backtranslated and sentence detailed datasets.

`preprocess_test`: Similar process was applied for the test set also.

`mt5_train_generate`: The mT5 model architecture was used in this study. Training and generation is applied here.

`classification_tfidf_5fold.ipynb` & `classification_tfidf_5fold.ipynb`: Classification task was executed including cross validation with k=5 for both vectorization methods TF-IDF and Word2Vec.


