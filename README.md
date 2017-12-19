# Ebola-Prediction

Group 64: *Yuxiang Wang, Zixun Zheng*

The final project of Intro to Machine Learning (EL-GY 9123)

Since **Ebola Virus** busted out to be a super threat to the human being in all over the world, we have a concern about the future of our life. The undergoing medical research may also be assisted by the prediction of the virus spreading. In our project, we conducted a simple but dedicated approach to predict the virus versus the temperature of the locations/ countries that have reported confirmed Ebola cases. 
The following are the basic steps to run the project in this notebook

1. Load data source 
2. Cleanse data format and extract data
3. Test data using different models
4. Data visualization

You can walk through detailed instruction to run the project by editing and running the notebook on your premise. **We put very specific instructions in the notebook code section through comments.**

### Data Source 

The dataset can be downloaded freely from https://ds-ec2.scraperwiki.com/g7nnqgn/ckm9nsfssakeuor/cgi-bin/csv/ebola_data_db_format.csv

The domain is https://data.humdata.org/ebola, a very helpful website of sharing open dataset about Ebola. It has one of the highest Click rate and also Authenticity. 

### Cleanse Data

We used the most popular and powerful libararies for structral or raw data processing

- Pandas
- Numpy
- Matplotlib
- Sklearn

> all can be installed by `pip3 install`, and of course, we recommend you to choose Python `3.5.0` kernel.

1. The dataset cannot be used directly, we extracted the columns that represent the `comfirmed Ebola cases` and `total Ebola cases` for a given `date` over a range in the year of 2015. 

2. To normalize the data, we convert `date` to `the day in year` and divided by the maximum `day` value in our data as we usually do for data normalization.

3. Also, we combined the Ebola case numbers with its corresponding `country`. 

4. The temperature data is downloaded from several authorized websites, for the sake of clear presentation of the temperature data, we organized them in a list and hard-code instead of `get` from web.

5. To study the underlying relation of temperature and Ebola cases that comfirmed, we use annual highest, lowest and average temperature to replace `country` column.

### Model Selection
For our problem, we want to find a great model to show how temperature and date relate to the probability of ebola. So, we try to find a "great" order of model that makes the predict precisely. In this program, we use from the 1st-order model to the 9th-order model for trainning and test, and then plot the result to find the "great" order model.

### Conclusion
The quadradic model is approximately best fit for our prediction. It is also very simply understandable and intuitive that Ebola or some similar virus can be faster spreaded under an environment with higher average annual temperature. Thus we verified, geographically speaking, the countries in western African (Guinea, Liberia) can be directly threated by Ebola since its geographical specifications and underdeveloped poor medical treatment.
