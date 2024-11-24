### Project Title
Predicting the Popularity of Dog Breeds
(UC Berkely Prof Cert in ML : Capstone Project)

Daniel Trezise

#### Executive summary
Can a machine learning model accurately predict the poplularity of a breed by learning key features of all the breeds?

#### Rationale
Both breeders and dog enthusiasts would benefit from such a model. 
It will help identify what qualities to look for when selecting a dog for ownership or breeding.
Owners can avoid breeds that have undesireable traits and find a suitable companion.
Breeders can make an informed decision on which breeds they may want to develop.

#### Research Question
Can a model predict the poplularity of a breed from a selection of common features accross all breeds?

#### Data Sources
I will be compiling the following 5 datasets of various features to evaluate and build a working model.

Dog Intelligence:
https://www.kaggle.com/datasets/thedevastator/canine-intelligence-and-size?select=dog_intelligence.csv

Dog Breeds Around the World:
https://www.kaggle.com/datasets/prajwaldongre/top-dog-breeds-around-the-world

American Kennel Club Info:
https://www.kaggle.com/datasets/thedevastator/canine-intelligence-and-size?select=dog_intelligence.csv

One Hundred Dogs:
https://www.dogbreedslist.info/all-dog-breeds/page-1.html

Best in Show
https://www.kaggle.com/datasets/paultimothymooney/best-in-show-data-about-dogs

#### Methodology

Data Exploration and Preprocessing:

I have made a quick inspection of the four datasets I will be using. There will need to be some clean up and feature engineering to build a final dataset that is prepared for analysis and modeling. Some of the issues that need to be addressed:

Each dataset has an index of dogs but not all have the same amount and ranking. I will need to make some choices to either reduce the dataset to the dog included in each set or consider filling in missing data if necessary. I may need to explore the excluded dogs in a separate investigation of why they didn’t make the cut.
There are several formatting issues across the datasets that would need to be addressed including scaling, encoding and converting data types.
During this cleaning and inspection process I will be considering each feature closely to see where new feature engineering would be beneficial and to see if the exploration process reveals any new unexpected insights into the data.

Data Analysis and Feature Selection:

I will be using several tools such as correlation and various visualizations to aid in identifying the relationships between features and which are likely to have the greatest impact on modeling.
I will also explore polynomial features for specific existing features and find the best complexity for that feature or multiple features.

Model Development:

Linear Regression
Logistic Regression
Decision Trees
Random Forest
Naive Bayes
Gaussian Mixture (GMM)
K-Nearest Neighbors (KNN)
Support Vector Machines (SVM)
Neural Network

#### Results

I worked with each of the models listed in my plan, but only 4 models performed well with this dataset.
Linear Regression did a very respectable job out of the gate but failed to capture the curve of the data.
Polynomial Regression, K-Nearest Neighbors and Neural Network models all performed well.
There's good reason to consider each of these, but in the end the Polynomial Regression model fit the data the best.

Following are the accuracy and r2 scores for each model:

Linear Regression
Accuracy Score = 0.8522976547707313       R2 Score = 0.8522976547707313

Polynomial Regression (3)
 Accuracy Score = 0.9764262088076493 R2 Score = 0.9764262088076493

KNN Result: Best Model = KNN 2
KNN 2 Score = 0.4166666666666667       KNN 2 R2 Score = 0.9288926331128542

NN Best Model: Using standardization scaler on features¶
Score = 0.9861111111111112       R2 Score = 0.9551142431038605

#### In conclusion
the model scored well in predicting the popularity of a breed from a selection of features.


#### Next steps
1. Several of the models I wanted to explore failed to produce results with the features I selected. I would revisit exploring those models with a different feature set focusing more on classification.
2. There are nearly recognized dog breeds in the world, but my final compiled dataset only contained full data for 103. I would like to fill in the missing data on the excluded breeds.
3. I was specifically interested in exploring further the relationship of intelligence with training and popularity.
4. I reduced the feature set a lot from the original merged dataset. I would like to reintroduce features I had excluded into the current working models and see how they affect the model.
5. To expand upon this project, the next big step would be to create a more complex model looking at pedigree lines and predicting which lines would breed well together.


#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
Daniel Trezise
dan@dantrezise.com
818-445-9141 
