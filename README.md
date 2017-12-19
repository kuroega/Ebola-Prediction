# Ebola-Prediction
The final project of Intro to Machine Learning (EL-GY 9123)

Since **Ebola Virus** busted out to be a super threat to the human being in all over the world, we have a concern about the future of our life. The undergoing medical research may also be assisted by the prediction of the virus spreading. In our project, we conducted a simple but dedicated approach to predict the virus versus the temperature of the locations/ countries that have reported confirmed Ebola cases. 
The following are the basic steps to run the project in this notebook

1. Load data source 
2. Cleanse data format and extract data
3. Test data using different models
4. Data visualization

You can walk through detailed instruction to run the project by editing and running the notebook on your premise.

### Data Source 

The dataset can be downloaded freely from https://ds-ec2.scraperwiki.com/g7nnqgn/ckm9nsfssakeuor/cgi-bin/csv/ebola_data_db_format.csv

The domain is https://data.humdata.org/ebola, a very helpful website of sharing open dataset about Ebola. It has one of the highest Click rate and also Authenticity. 

### Cleanse Data

We used the most popular and powerful libararies for raw data processing

- Pandas
- Numpy
- Matplotlib
- Sklearn

all can be installed by `pip3 install`, and of course, we recommend you to choose Python `3.5.0` kernel.

### Model Selection

### Conclusion
The quadradic model is approximately best fit for our prediction. It is also very simply understandable and intuitive that Ebola or some similar virus can be faster spreaded under an environment with higher average annual temperature. Thus we verified, geographically speaking, the countries in western African (Guinea, Liberia) can be directly threated by Ebola since its geographical specifications and underdeveloped poor medical treatment.
