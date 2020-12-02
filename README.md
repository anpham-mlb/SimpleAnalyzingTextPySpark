## PySpark
Using PySpark to find the distribution of words, the most common words and the average frequency in books. Two books used were Agile Processes in Software Engineering and Extreme Programming and Scrum Handbook. 

## Details
### Step 1: Import pyspark and initialize Spark
Create a SparkConf object that contains information about your application by SparkContext.
### Step 2: Create Resilient Distributed Datasets (RDDs)
A SparkContext can be used to create Resilient Distributed Datasets (RDDs) on a cluster.
### Step 3: Cleaning/Manipulating text
Using regular expression to perform the following tasks on the RDDs:
- Removes all characters which are not alphabets except space(s).
- Changes all upper case letters to lowercase..
- Removes all leading or trailing spaces.
### Step 4: Transforming the Data/Counting the words
Apply a transformation that will split each element of the RDD by its spaces and then create a word pairs for e.g. ('agile', 1), ('handbook', 1). Then, count the frequency of each word and display the top 20 most frequent words.
### Step 5: Removing Stop Words
In natural language processing, useless words (data), are referred to as stop words. NLTK(Natural Language Toolkit) in python has a list of stopwords stored in 16 different languages. NLTK will be used to remove stop words.
### Step 6: Find the average occurrence of a word
Find the total number of words and divide that by the number of unique words.
