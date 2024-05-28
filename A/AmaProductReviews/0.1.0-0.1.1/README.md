# Comparing `tmp/amaproductreviews-0.1.0.tar.gz` & `tmp/amaproductreviews-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amaproductreviews-0.1.0.tar", max compression
+gzip compressed data, was "amaproductreviews-0.1.1.tar", max compression
```

## Comparing `amaproductreviews-0.1.0.tar` & `amaproductreviews-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     5185 2024-05-06 11:54:51.242932 amaproductreviews-0.1.0/amaproductreviews.py
--rw-r--r--   0        0        0      371 2024-05-11 16:29:41.129396 amaproductreviews-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2287 2024-05-11 16:27:49.731585 amaproductreviews-0.1.0/README.md
--rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 amaproductreviews-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5394 2024-05-28 12:13:15.188270 amaproductreviews-0.1.1/amaproductreviews.py
+-rw-r--r--   0        0        0      371 2024-05-28 12:14:13.893809 amaproductreviews-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2287 2024-05-11 16:27:49.731585 amaproductreviews-0.1.1/README.md
+-rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 amaproductreviews-0.1.1/PKG-INFO
```

### Comparing `amaproductreviews-0.1.0/amaproductreviews.py` & `amaproductreviews-0.1.1/amaproductreviews.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from nltk.corpus import stopwords
 from nltk.tokenize import word_tokenize
 import spacy
 from textblob import TextBlob
 import plotly.express as px
 from wordcloud import WordCloud
 from webdriver_manager.chrome import ChromeDriverManager
+import joblib
 nlp = spacy.load("en_core_web_sm")
 #subprocess.run(["python", "-m", "spacy", "download", "en_core_web_sm"])
 stop_words = set(stopwords.words('english'))
 chrome_options = Options()
 #chrome_options.add_argument("--headless")
 options = Options()
 options.add_argument('--disable-gpu')
@@ -110,8 +111,15 @@
 def get_reviews_images(UrlProduct):
     driver.get(UrlProduct)
     soup = BeautifulSoup(driver.page_source,'html.parser')
     image_reviews = soup.find_all('div', class_='_Y3Itb_media-thumbnail-container_2MRZY')
     image_reviews = str(image_reviews)
     image_reviews = re.findall(r'src="(https.*?jpg)',image_reviews)
     # Image_of_product = re.findall(r'src="https.*pg',str(Image_of_product))
-    return image_reviews
+    return image_reviews
+
+def model_log_reg():
+    model = joblib.load('logistic_regression_model.pkl')
+    return model
+def vec_text():
+    vectorizer = joblib.load('tfidf_vectorizer.pkl')
+    return vectorizer
```

### Comparing `amaproductreviews-0.1.0/README.md` & `amaproductreviews-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `amaproductreviews-0.1.0/PKG-INFO` & `amaproductreviews-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 416d 6150  : 2.1.Name: AmaP
 00000020: 726f 6475 6374 5265 7669 6577 730a 5665  roductReviews.Ve
-00000030: 7273 696f 6e3a 2030 2e31 2e30 0a53 756d  rsion: 0.1.0.Sum
+00000030: 7273 696f 6e3a 2030 2e31 2e31 0a53 756d  rsion: 0.1.1.Sum
 00000040: 6d61 7279 3a20 416e 616c 797a 6520 416d  mary: Analyze Am
 00000050: 617a 6f6e 2070 726f 6475 6374 2072 6576  azon product rev
 00000060: 6965 7773 0a41 7574 686f 723a 206f 6c61  iews.Author: ola
 00000070: 6d69 6e65 207a 616b 6172 6961 0a41 7574  mine zakaria.Aut
 00000080: 686f 722d 656d 6169 6c3a 206f 6c61 6d69  hor-email: olami
 00000090: 6e65 7a61 6b61 7269 6130 3340 676d 6169  nezakaria03@gmai
 000000a0: 6c2e 636f 6d0a 5265 7175 6972 6573 2d50  l.com.Requires-P
```

