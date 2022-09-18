# ML2
**Machine Learning Zoom Camp- Session 2**  
notes:   
1. pd.read_csv(<file_path_string>) - read csv files  
2. df.head() - take a look of the dataframe  
3. df.columns - retrieve colum names of a dataframe  
4. df.columns.str.lower() - lowercase all the letters  
5. df.columns.str.replace(' ', '_') - replace the space separator  
6. df.dtypes - retrieve data types of all features  
7. df.index - retrieve indices of a dataframe  

**Pandas attributes and methods:**

1. df[col].unique() - returns a list of unique values in the series  
2. df[col].nunique() - returns the number of unique values in the series  
3. df.isnull().sum() - retunrs the number of null values in the dataframe  


**Matplotlib and seaborn methods:**  

1. %matplotlib inline - assure that plots are displayed in jupyter notebook's cells  
2. sns.histplot() - show the histogram of a series  


  **Numpy methods:**

1. np.log1p() - applies log transformation to a variable and adds one to each result
Long-tail distributions usually confuse the ML models, so the recommendation is to transform the target variable distribution to a normal one whenever possible.


**Setting up the validation framework**


In general, the dataset is split into three parts: training, validation, and test. For each partition, we need to obtain feature matrices (X) and y vectors of targets. First, the size of partitions is calculated, records are shuffled to guarantee that values of the three partitions contain non-sequential records of the dataset, and the partitions are created with the shuffled indices.  


**Pandas attributes and methods:**  

1. df.iloc[] - returns subsets of records of a dataframe, being selected by numerical indices  
2. df.reset_index() - restate the orginal indices  
3. del df[col] - eliminates target variable  


**Numpy methods:**  

1. np.arange() - returns an array of numbers
2. np.random.shuffle() - returns a shuffled array
3. np.random.seed() - set a seed
