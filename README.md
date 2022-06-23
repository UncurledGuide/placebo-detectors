# Heart Attack Data Analysis
*AI Camp 2022 - Team Placebo Detectors*
### Introduction
Our dataset, collected from Kaggle, predicts whether or not certain individuals had a heart attack through focusing on varying health conditions these subjects have.This dataset considered 14 different variables, including age, chest pain, resting blood sugar, and maximum heart rate achieved. We used this dataset to create multiple visual models to predict a risk of heart attack.

### Project Content
- Homepage
 ![](app/static/assets/img/homepg.png)
- Introduction
- Exploratory Data Analysis
  - Dataset
  - Correlation heatmap
  - Graphs for heart attack risk
- Integrating machine learning
  - KNN model
  - SVM model
  - Random forests model
  - Gradient Boosting model
  - Confusion matrixes
- Conclusion
- Our Team

### Exploratory Data Analysis
- Our website includes a sample of our raw data set and its columns
- We included a correlation heatmap to show relationships between different variables
- To help viewers understand the data better, we included graphs that show the heart attack risk by age and sex

### Models
- We used several models to present our data such as KNN, SVM, Random Forests, and Gradient Boosting.
- Our KNN model allowed us to calculate the best accuracy of classifying whether someone will experience a heart attack
- Our SVM model is a model that finds a hyperplane (a divider) in an N-dimensional space. The hyperplane helps separate and distinctly classify data points.
- Our Random Forests model had the highest accuracy. There are various decision trees, each of which makes use of dataset samples. From the top of each tree, a random node is chosen, and it proceeds down the tree, picking a random node at each level until it reaches the bottom, which is the prediction. This process is repeated several times, and the final prediction is the average of all the predictions
- Our Gradient Boosting Model makes the assumption that the next model presented minimizes the overall prediction error when combined with previous models. Its goal is to approximate the best output value based on the input values.
- We also used a confusion matrix to help us understand how well our models are performing, what kind of errors are being made, and an overview of what we need to change to make our model as efficient and accurate as possible.

### Conclusion
- We compared each model's accuracy, precision, and recall values to determine which model performed the best
- This project was significant as it helped us predict whether a person will have a heart attack or not, which is beneficial to those who want more health awareness.

### Quickstart
**DS/ML Part**: 

Run final_project_all_models.ipynb in the ml folder.

**Web Application Part**: 

Enter the app folder in the terminal:

`cd app`

Start the flask server:

`python -m main`

Click the link appears in the terminal. Done!



### File Structure
The files/directories which you will need to edit are **bolded**

**DO NOT TOUCH OTHER FILES. THIS MAY RESULT IN YOUR PROJECT BEING UNABLE TO RUN**

- .gitignore
- config.py
- Dockerfile
- READMD.md
- entrypoint.sh
- nginx_host
- host_config
- app/
     - **main.py**
     - **requirements.txt**
     - **utils.py**
     - templates/
          - **index.html**
     - static/
          - css/
               - **styles.css**
          - images/
               - **KNNmodel.png**
          - js/
               - **scripts.js**
- ml/
     - final_project_all_models.ipynb
     - heart.csv
### main.py ###
Contains the main flask app itself.
### requirements.txt ###
Contains list of packages and modules required to run the flask app. Edit only if you are using additional packages that need to be pip installed in order to run the project.

To generate a requirements.txt file you can run

`pip list --format=freeze > app/requirements.txt`

the requirements.txt file will then be updated. Keep in mind: some packages you install on one operating system may not be available on another. You will have to debug and resolve this yourself if this is the case.
### static/ ###
Contains the static images, CSS, & JS files used by the flask app for the webpage. You will need to create this and put files in it. Place all your images used for your website in static/images/ so that you can then reference them in your html files. You can also place your css files in this folder, to reference them like static/css/styles.css
### utils.py ###
Contains common functions used by the flask app. Put things here that are used more than once in the flask app.
### templates/ ###
Contains the HTML pages used for the webpage. Edit these to fit your project. index.html is the demo page. Optionally, you can add another team.html page or include a team section in index.html. 
### Files used for deployment ###
`config.py`
`Dockerfile`
`entrypoint.sh`
`nginx_host`
`host_config`

**Only modify `host_config`. Do not touch the other files.**
