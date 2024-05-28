# Comparing `tmp/emotion_analysis-0.1.1.tar.gz` & `tmp/emotion_analysis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotion_analysis-0.1.1.tar", last modified: Tue May 28 02:31:27 2024, max compression
+gzip compressed data, was "emotion_analysis-0.1.2.tar", last modified: Tue May 28 03:13:25 2024, max compression
```

## Comparing `emotion_analysis-0.1.1.tar` & `emotion_analysis-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      297 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/PKG-INFO
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/emotion_analysis/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      462 2024-05-27 16:11:32.000000 emotion_analysis-0.1.1/emotion_analysis/__init__.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     4287 2024-05-27 16:54:30.000000 emotion_analysis-0.1.1/emotion_analysis/bert_pcc_score_emotions.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    14768 2024-05-27 16:39:22.000000 emotion_analysis-0.1.1/emotion_analysis/data_preprocessing.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      421 2024-05-28 02:25:32.000000 emotion_analysis-0.1.1/emotion_analysis/dataset_upload.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     5281 2024-05-25 21:05:45.000000 emotion_analysis-0.1.1/emotion_analysis/frnn.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     4443 2024-05-27 21:14:04.000000 emotion_analysis-0.1.1/emotion_analysis/roberta_pcc_score_emotions.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2381 2024-05-28 02:28:21.000000 emotion_analysis-0.1.1/emotion_analysis/tweets_embedding.py
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/emotion_analysis.egg-info/
--rw-r--r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      297 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      495 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        1 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       81 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/requires.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       23 2024-05-28 02:31:27.000000 emotion_analysis-0.1.1/emotion_analysis.egg-info/top_level.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       38 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/setup.cfg
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      558 2024-05-28 02:30:56.000000 emotion_analysis-0.1.1/setup.py
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 02:31:27.499341 emotion_analysis-0.1.1/tests/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 16:13:33.000000 emotion_analysis-0.1.1/tests/__init__.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    10136 2024-05-27 21:13:11.000000 emotion_analysis-0.1.1/tests/test.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 03:13:25.388268 emotion_analysis-0.1.2/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      297 2024-05-28 03:13:25.388268 emotion_analysis-0.1.2/PKG-INFO
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 03:13:25.388268 emotion_analysis-0.1.2/emotion_analysis/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      462 2024-05-27 16:11:32.000000 emotion_analysis-0.1.2/emotion_analysis/__init__.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2184 2024-05-28 03:08:43.000000 emotion_analysis-0.1.2/emotion_analysis/bert_pcc_score_emotions.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    13125 2024-05-28 03:01:22.000000 emotion_analysis-0.1.2/emotion_analysis/data_preprocessing.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     5281 2024-05-25 21:05:45.000000 emotion_analysis-0.1.2/emotion_analysis/frnn.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2145 2024-05-28 03:09:56.000000 emotion_analysis-0.1.2/emotion_analysis/roberta_pcc_score_emotions.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2381 2024-05-28 02:28:21.000000 emotion_analysis-0.1.2/emotion_analysis/tweets_embedding.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 03:13:25.388268 emotion_analysis-0.1.2/emotion_analysis.egg-info/
+-rw-r--r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      297 2024-05-28 03:13:25.000000 emotion_analysis-0.1.2/emotion_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      460 2024-05-28 03:13:25.000000 emotion_analysis-0.1.2/emotion_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        1 2024-05-28 03:13:25.000000 emotion_analysis-0.1.2/emotion_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       81 2024-05-28 03:13:25.000000 emotion_analysis-0.1.2/emotion_analysis.egg-info/requires.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       23 2024-05-28 03:13:25.000000 emotion_analysis-0.1.2/emotion_analysis.egg-info/top_level.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       38 2024-05-28 03:13:25.388268 emotion_analysis-0.1.2/setup.cfg
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      558 2024-05-28 03:12:02.000000 emotion_analysis-0.1.2/setup.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 03:13:25.388268 emotion_analysis-0.1.2/tests/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 16:13:33.000000 emotion_analysis-0.1.2/tests/__init__.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    14384 2024-05-28 03:12:50.000000 emotion_analysis-0.1.2/tests/test.py
```

### Comparing `emotion_analysis-0.1.1/emotion_analysis/data_preprocessing.py` & `emotion_analysis-0.1.2/emotion_analysis/data_preprocessing.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 from nltk.corpus import stopwords
 import contractions
 from wordcloud import WordCloud
 import matplotlib.pyplot as plt
 import seaborn as sns
 import os
 from nltk import ngrams
-
-# Download NLTK data if not already downloaded
 import nltk
 
+# Download NLTK data if not already downloaded
 nltk.download("stopwords")
 stop_words = set(stopwords.words("english"))
 nltk.download("punkt")
 
 print(
     "EXPAND CONTRACTION, REMOVE HTML TAGS, NON-ASCII, TWEET CLEANING, DATA PREPROCESSING START!"
 )
@@ -52,88 +51,66 @@
 print("\n\n Removing NON-ASCII Applying Process End!")
 
 
 def tweet_cleaning(tweet):
     """
     Perform general preprocessing of the tweet, including removing stop words.
     """
-    # Replace '\n' with a space
     tweet = tweet.replace("\\n", " ")
 
-    # Expand contractions
     tweet = expand_contractions(tweet)
-
-    # Remove HTML tags
     tweet = remove_html_tags(tweet)
-
-    # Remove non-ASCII characters
     tweet = remove_non_ascii(tweet)
-
-    # Remove '#', '@', and URLs
     tweet = re.sub(r"#|@[^\s]+|https?:\/\/.*[\r\n]*", "", tweet)
-
-    # Remove digits
     tweet = re.sub(r"\d+", "", tweet)
 
-    # Replace old-style smilies with textual descriptions
     smilies = {
         ":)": "smiley",
         ":-)": "smiley",
         ":(": "sad",
         ":/": "skeptical",
         ":D": "laughing",
         ":o": "surprise",
         ":O": "surprise",
     }
     for smile, desc in smilies.items():
         tweet = tweet.replace(smile, desc)
 
-    # Transform emojis to their textual descriptions
     tweet = demojize(tweet).replace(":", "").replace("_", " ")
 
-    # Remove punctuation and convert to lowercase
     tweet = re.sub(r"[^\w\s]", "", tweet.lower())
-
-    # Remove extra whitespaces
     tweet = re.sub(r"\s+", " ", tweet).strip()
 
     return tweet
 
 
 print("\n\n Tweet Cleaning Applying Process End!")
 
 
 def transform_data(file_name):
     """
     Transform the original dataset into a DataFrame suitable for further processing.
     """
-    # Read the dataset
     data = pd.read_csv(file_name, sep="\t")
-    # Clean tweets
     data["Cleaned_tweet"] = data["Tweet"].apply(tweet_cleaning)
-    # Remove stopwords
     data["Cleaned_tweet_wt_stopwords"] = data["Cleaned_tweet"].apply(
         lambda x: " ".join([word for word in x.split() if word not in stop_words])
     )
-    # Extract class as integer
     data["Class"] = data["Intensity Class"].str.split(":").str[0]
-    # Drop unnecessary columns
     data = data.drop(["Intensity Class", "Affect Dimension"], axis=1)
     return data
 
 
 def upload_datasets(file_train, file_dev, file_test):
     """
     Compose emotion datasets in DataFrames for train, development, and test sets.
     """
-    # Transform individual datasets
     train_data = transform_data(file_train)
     dev_data = transform_data(file_dev)
     test_data = transform_data(file_test)
-    # Concatenate train and dev sets
     combined_train_data = pd.concat([train_data, dev_data], ignore_index=True)
     return train_data, dev_data, combined_train_data, test_data
 
 
 def namestr(obj, namespace):
     """
     This function returns the name of 'obj' variable
@@ -153,32 +130,26 @@
     plt.figure(figsize=(10, 5))
     plt.imshow(wordcloud, interpolation="bilinear")
     plt.axis("off")
     if title:
         plt.title(title)
 
 
-import os
-
-# Create directories to save plots
 plot_dir = "plots"
 emotions = ["Anger", "Joy", "Sadness", "Fear"]
 for emotion in emotions:
     folder_path = os.path.join(plot_dir, emotion)
     if not os.path.exists(folder_path):
         os.makedirs(folder_path)
 
 
 def save_plot(plt, filename, folder, subfolder):
     """
     Save the plot in the specified folder with the given filename.
     """
-    print("Plot Dir:", plot_dir)
-    print("Folder:", folder)
-    print("Subfolder:", subfolder)
     folder_path = os.path.join(plot_dir, folder, subfolder)
     if not os.path.exists(folder_path):
         os.makedirs(folder_path)
     filepath = os.path.join(folder_path, filename)
     plt.savefig(filepath)
     plt.close()
 
@@ -202,15 +173,14 @@
         )
 
 
 def plot_statistics(train_data, dev_data, combined_train_data, test_data, emotion):
     """
     Plot advanced statistics including word counts and save the plots.
     """
-    # Plot word counts
     datasets = [
         ("Train", train_data),
         ("Dev", dev_data),
         ("Combined Train", combined_train_data),
         ("Test", test_data),
     ]
     for name, data in datasets:
@@ -224,28 +194,26 @@
         save_plot(
             plt,
             f"{emotion.lower()}_{name.lower()}_wordcount_distribution.png",
             emotion,
             name.lower(),
         )
 
-    # Plot class distribution
     plt.figure(figsize=(10, 5))
     sns.countplot(data=train_data, x="Class")
     plt.title(f"{emotion} - Class Distribution - Train")
     plt.xlabel("Class")
     plt.ylabel("Frequency")
     save_plot(plt, f"{emotion.lower()}_train_class_distribution.png", emotion, "train")
 
 
 def plot_additional_statistics(train_data, dev_data, test_data, emotion):
     """
     Plot additional statistics and save the plots.
     """
-    # Plot tweet length distribution
     plt.figure(figsize=(10, 5))
     sns.histplot(
         train_data["Cleaned_tweet"].apply(len),
         bins=30,
         kde=True,
         color="skyblue",
         label="Train",
@@ -268,15 +236,14 @@
     plt.xlabel("Tweet Length")
     plt.ylabel("Frequency")
     plt.legend()
     save_plot(
         plt, f"{emotion.lower()}_tweet_length_distribution.png", emotion, "additional"
     )
 
-    # Plot cleaned tweet length distribution without stopwords
     plt.figure(figsize=(10, 5))
     sns.histplot(
         train_data["Cleaned_tweet_wt_stopwords"].apply(len),
         bins=30,
         kde=True,
         color="skyblue",
         label="Train",
@@ -319,52 +286,44 @@
         hue=word_freq.index,
         legend=False,
         palette="viridis",
     )
     plt.title(title)
     plt.xlabel("Frequency")
     plt.ylabel("Words")
-    plt.gca().invert_yaxis()  # Invert y-axis to display highest frequency words at the top
+    plt.gca().invert_yaxis()
     save_plot(
         plt,
         f"{title.lower().replace(' ', '_')}_top_{n}_words.png",
         "top_n_words",
         "top_words",
     )
 
 
 def plot_ngrams_frequency(data, n=2, top_n=10, title=None, emotion=None):
     """
     Plot the frequency of n-grams (bi-grams or tri-grams) in the dataset.
     """
-    # Tokenize the cleaned tweets
     tokenized_tweets = data["Cleaned_tweet"].apply(lambda x: x.split())
-
-    # Generate n-grams
     ngrams_list = [ngrams(tokens, n) for tokens in tokenized_tweets]
-
-    # Flatten the list of n-grams
     ngrams_flat = [item for sublist in ngrams_list for item in sublist]
-
-    # Calculate frequency of n-grams
     ngrams_freq = pd.Series(ngrams_flat).value_counts()[:top_n]
 
-    # Plot the frequency
     plt.figure(figsize=(10, 5))
     sns.barplot(
         x=ngrams_freq.values,
         y=[" ".join(ngram) for ngram in ngrams_freq.index],
         hue=ngrams_freq.index,
         legend=False,
         palette="viridis",
     )
     plt.title(title)
     plt.xlabel("Frequency")
     plt.ylabel(f"{n}-grams")
-    plt.gca().invert_yaxis()  # Invert y-axis to display highest frequency n-grams at the top
+    plt.gca().invert_yaxis()
     save_plot(
         plt,
         f"{title.lower().replace(' ', '_')}_top_{n}_words.png",
         folder="top_n_words",
         subfolder="top_words",
     )
 
@@ -372,25 +331,21 @@
 def calculate_statistics(dataset):
     """
     Calculate imbalance ratio, characteristics, and other useful information for the dataset.
     """
     print("Characteristics of ", namestr(dataset, globals())[0])
     print("Number of instances: ", len(dataset))
 
-    # Get class sizes
     class_sizes = [
         len(dataset[dataset["Class"] == i]) for i in sorted(dataset["Class"].unique())
     ]
-
-    # Find the smallest class size other than zero
     min_size_other_than_zero = min(size for size in class_sizes if size > 0)
 
     print("Size of the smallest class (excluding class 0): ", min_size_other_than_zero)
 
-    # Calculate imbalance ratio (IR) only if there are instances in all classes other than zero
     if min_size_other_than_zero > 0:
         imbalance_ratio = round(max(class_sizes) / min_size_other_than_zero, 2)
         print("Imbalance Ratio (IR): ", imbalance_ratio)
     else:
         print(
             "Imbalance Ratio (IR): N/A (Some classes other than 0 have zero instances)"
         )
@@ -399,35 +354,28 @@
 
 
 def plot_characteristics_and_ir(datasets):
     """
     Plot characteristics and imbalance ratio (IR) for each emotion dataset.
     """
     plt.figure(figsize=(10, 6))
-
-    # Extract dataset names and corresponding IR values
     dataset_names = [namestr(dataset, globals())[0] for dataset in datasets]
     ir_values = [calculate_imbalance_ratio(dataset) for dataset in datasets]
 
-    # Plotting characteristics
     plt.bar(dataset_names, ir_values, color="skyblue")
     plt.title("Imbalance Ratio (IR) for Different Emotion Datasets")
     plt.xlabel("Dataset")
     plt.ylabel("Imbalance Ratio (IR)")
     plt.xticks(rotation=45, ha="right")
     plt.tight_layout()
 
-    # Add IR values as annotations
     for i, ir in enumerate(ir_values):
         plt.text(i, ir, str(ir), ha="center", va="bottom")
 
-    # Save the plot
     plt.savefig("imbalance_ratios_plot.png")
-
-    # Show the plot
     plt.show()
 
 
 def calculate_imbalance_ratio(dataset):
     """
     Calculate imbalance ratio (IR) for the dataset.
     """
@@ -444,50 +392,45 @@
 
 def plot_dataset_statistics(datasets):
     """
     Plot various statistics for each emotion dataset.
     """
     plt.figure(figsize=(12, 8))
 
-    # Initialize lists to store statistics
     num_instances = []
     smallest_class_size = []
     imbalance_ratios = []
 
     for dataset in datasets:
-        # Calculate statistics
         num_instances.append(len(dataset))
         class_sizes = [
             len(dataset[dataset["Class"] == i])
             for i in sorted(dataset["Class"].unique())
         ]
         min_size_other_than_zero = min(size for size in class_sizes if size > 0)
         if min_size_other_than_zero > 0:
             imbalance_ratio = round(max(class_sizes) / min_size_other_than_zero, 2)
         else:
             imbalance_ratio = None
 
         smallest_class_size.append(min_size_other_than_zero)
         imbalance_ratios.append(imbalance_ratio)
 
-    # Plot number of instances
     plt.subplot(3, 1, 1)
     plt.bar(range(len(datasets)), num_instances, color="skyblue")
     plt.title("Number of Instances in Each Emotion Dataset")
     plt.ylabel("Number of Instances")
     plt.xticks(range(len(datasets)), ["Anger", "Joy", "Sadness", "Fear"])
 
-    # Plot smallest class size
     plt.subplot(3, 1, 2)
     plt.bar(range(len(datasets)), smallest_class_size, color="orange")
     plt.title("Size of the Smallest Class (Excluding Class 0) in Each Emotion Dataset")
     plt.ylabel("Smallest Class Size")
     plt.xticks(range(len(datasets)), ["Anger", "Joy", "Sadness", "Fear"])
 
-    # Plot imbalance ratios
     plt.subplot(3, 1, 3)
     plt.bar(range(len(datasets)), imbalance_ratios, color="green")
     plt.title("Imbalance Ratio (IR) for Each Emotion Dataset")
     plt.ylabel("Imbalance Ratio (IR)")
     plt.xticks(range(len(datasets)), ["Anger", "Joy", "Sadness", "Fear"])
 
     plt.tight_layout()
```

### Comparing `emotion_analysis-0.1.1/emotion_analysis/frnn.py` & `emotion_analysis-0.1.2/emotion_analysis/frnn.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.1/emotion_analysis/tweets_embedding.py` & `emotion_analysis-0.1.2/emotion_analysis/tweets_embedding.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.1/setup.py` & `emotion_analysis-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="emotion_analysis",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "pandas",
         "beautifulsoup4",
         "emoji",
         "nltk",
         "wordcloud",
```

### Comparing `emotion_analysis-0.1.1/tests/test.py` & `emotion_analysis-0.1.2/tests/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # Get the parent directory (root directory of the project)
 parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
 
 # Add the parent directory to sys.path
 sys.path.append(parent_dir)
 
 from emotion_analysis.data_preprocessing import *
-from emotion_analysis.dataset_upload import *
 from emotion_analysis.tweets_embedding import *
 from emotion_analysis.frnn import *
 from emotion_analysis.bert_pcc_score_emotions import *
 from emotion_analysis.roberta_pcc_score_emotions import *
 
 anger_train, anger_dev, anger_data, anger_test = upload_datasets(
     "/home/ahsan-pmylsp/Desktop/frnn_emotion_detection-main/update/Frnn_Emotion/emotion_analysis/dataset/2018-EI-oc-En-anger-dev.txt",
@@ -85,14 +84,135 @@
 plot_ngrams_frequency(
     fear_train, n=3, top_n=10, title="Trigram Frequency in Fear Train Data"
 )
 
 
 plot_dataset_statistics([anger_data, joy_data, sad_data, fear_data])
 
+
+anger_data["Vector_bert"] = anger_data["Tweet"].apply(get_vector_bert)
+anger_test["Vector_bert"] = anger_test["Tweet"].apply(get_vector_bert)
+
+joy_data["Vector_bert"] = joy_data["Tweet"].apply(get_vector_bert)
+joy_test["Vector_bert"] = joy_test["Tweet"].apply(get_vector_bert)
+
+sad_data["Vector_bert"] = sad_data["Tweet"].apply(get_vector_bert)
+sad_test["Vector_bert"] = sad_test["Tweet"].apply(get_vector_bert)
+
+fear_data["Vector_bert"] = fear_data["Tweet"].apply(get_vector_bert)
+fear_test["Vector_bert"] = fear_test["Tweet"].apply(get_vector_bert)
+
+print("1st done")
+
+anger_data["Vector_bert_cl"] = anger_data["Cleaned_tweet"].apply(get_vector_bert)
+anger_test["Vector_bert_cl"] = anger_test["Cleaned_tweet"].apply(get_vector_bert)
+
+joy_data["Vector_bert_cl"] = joy_data["Cleaned_tweet"].apply(get_vector_bert)
+joy_test["Vector_bert_cl"] = joy_test["Cleaned_tweet"].apply(get_vector_bert)
+
+sad_data["Vector_bert_cl"] = sad_data["Cleaned_tweet"].apply(get_vector_bert)
+sad_test["Vector_bert_cl"] = sad_test["Cleaned_tweet"].apply(get_vector_bert)
+
+fear_data["Vector_bert_cl"] = fear_data["Cleaned_tweet"].apply(get_vector_bert)
+fear_test["Vector_bert_cl"] = fear_test["Cleaned_tweet"].apply(get_vector_bert)
+
+print("2nd done")
+
+# BERT
+# With raw tweets
+
+anger_data["Vector_bert_cl_ws"] = anger_data["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_bert
+)
+anger_test["Vector_bert_cl_ws"] = anger_test["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_bert
+)
+
+joy_data["Vector_bert_cl_ws"] = joy_data["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_bert
+)
+joy_test["Vector_bert_cl_ws"] = joy_test["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_bert
+)
+
+sad_data["Vector_bert_cl_ws"] = sad_data["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_bert
+)
+sad_test["Vector_bert_cl_ws"] = sad_test["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_bert
+)
+
+fear_data["Vector_bert_cl_ws"] = fear_data["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_bert
+)
+fear_test["Vector_bert_cl_ws"] = fear_test["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_bert
+)
+
+
+anger_data["Vector_roberta"] = anger_data["Tweet"].apply(get_vector_roberta)
+anger_test["Vector_roberta"] = anger_test["Tweet"].apply(get_vector_roberta)
+
+joy_data["Vector_roberta"] = joy_data["Tweet"].apply(get_vector_roberta)
+joy_test["Vector_roberta"] = joy_test["Tweet"].apply(get_vector_roberta)
+
+sad_data["Vector_roberta"] = sad_data["Tweet"].apply(get_vector_roberta)
+sad_test["Vector_roberta"] = sad_test["Tweet"].apply(get_vector_roberta)
+
+fear_data["Vector_roberta"] = fear_data["Tweet"].apply(get_vector_roberta)
+fear_test["Vector_roberta"] = fear_test["Tweet"].apply(get_vector_roberta)
+
+print("1st done")
+
+anger_data["Vector_roberta_cl"] = anger_data["Cleaned_tweet"].apply(get_vector_roberta)
+anger_test["Vector_roberta_cl"] = anger_test["Cleaned_tweet"].apply(get_vector_roberta)
+
+joy_data["Vector_roberta_cl"] = joy_data["Cleaned_tweet"].apply(get_vector_roberta)
+joy_test["Vector_roberta_cl"] = joy_test["Cleaned_tweet"].apply(get_vector_roberta)
+
+sad_data["Vector_roberta_cl"] = sad_data["Cleaned_tweet"].apply(get_vector_roberta)
+sad_test["Vector_roberta_cl"] = sad_test["Cleaned_tweet"].apply(get_vector_roberta)
+
+fear_data["Vector_roberta_cl"] = fear_data["Cleaned_tweet"].apply(get_vector_roberta)
+fear_test["Vector_roberta_cl"] = fear_test["Cleaned_tweet"].apply(get_vector_roberta)
+
+print("2nd done")
+
+# roberta
+# With raw tweets
+
+anger_data["Vector_roberta_cl_ws"] = anger_data["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_roberta
+)
+anger_test["Vector_roberta_cl_ws"] = anger_test["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_roberta
+)
+
+joy_data["Vector_roberta_cl_ws"] = joy_data["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_roberta
+)
+joy_test["Vector_roberta_cl_ws"] = joy_test["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_roberta
+)
+
+sad_data["Vector_roberta_cl_ws"] = sad_data["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_roberta
+)
+sad_test["Vector_roberta_cl_ws"] = sad_test["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_roberta
+)
+
+fear_data["Vector_roberta_cl_ws"] = fear_data["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_roberta
+)
+fear_test["Vector_roberta_cl_ws"] = fear_test["Cleaned_tweet_wt_stopwords"].apply(
+    get_vector_roberta
+)
+
+
 anger_pcc_scores = cross_validation_ensemble_owa(
     anger_data.head(10),
     vector_names=["Vector_roberta_cl", "Vector_roberta", "Vector_roberta_cl_ws"],
     NNeighbours=[5, 5],
     lower=[1, 1],
     upper=[1, 1],
     alpha=0.5,
```

