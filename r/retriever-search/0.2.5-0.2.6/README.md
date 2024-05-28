# Comparing `tmp/retriever_search-0.2.5.tar.gz` & `tmp/retriever_search-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.2.5.tar", last modified: Sun May 19 21:00:24 2024, max compression
+gzip compressed data, was "retriever_search-0.2.6.tar", last modified: Tue May 28 05:29:55 2024, max compression
```

## Comparing `retriever_search-0.2.5.tar` & `retriever_search-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 21:00:24.120120 retriever_search-0.2.5/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.5/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2286 2024-05-19 21:00:24.119756 retriever_search-0.2.5/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.5/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 21:00:24.093565 retriever_search-0.2.5/retriever_search/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.5/retriever_search/DocumentIngestion.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.5/retriever_search/QueryPipeline.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)   315320 2024-05-02 19:07:29.000000 retriever_search-0.2.5/retriever_search/TopicModellingInit.html
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.5/retriever_search/Utils.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      144 2024-05-19 21:00:18.000000 retriever_search-0.2.5/retriever_search/__init__.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9998 2024-05-19 17:40:04.000000 retriever_search-0.2.5/retriever_search/callbacks.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 21:00:24.103960 retriever_search-0.2.5/retriever_search/data/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)   337240 2024-05-02 19:07:29.000000 retriever_search-0.2.5/retriever_search/data/CountVectorizer.pkl
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)  6339926 2024-05-02 19:07:29.000000 retriever_search-0.2.5/retriever_search/data/EmbeddedVectors.pkl
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)  2102124 2024-05-02 19:07:29.000000 retriever_search-0.2.5/retriever_search/data/LDAModel.pkl
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3623 2024-05-19 19:45:03.000000 retriever_search-0.2.5/retriever_search/frontend_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.5/retriever_search/layout.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.5/retriever_search/search_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3491 2024-05-19 19:41:40.000000 retriever_search-0.2.5/retriever_search/search_server.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1174 2024-05-19 20:59:49.000000 retriever_search-0.2.5/retriever_search/viz_server.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 21:00:24.119270 retriever_search-0.2.5/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2286 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      698 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      255 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-19 21:00:24.120210 retriever_search-0.2.5/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1129 2024-05-19 19:01:43.000000 retriever_search-0.2.5/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-28 05:29:55.915404 retriever_search-0.2.6/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.6/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2490 2024-05-28 05:29:55.915009 retriever_search-0.2.6/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1716 2024-05-28 05:19:50.000000 retriever_search-0.2.6/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-28 05:29:55.895420 retriever_search-0.2.6/retriever_search/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.6/retriever_search/DocumentIngestion.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.6/retriever_search/QueryPipeline.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)   315320 2024-05-02 19:07:29.000000 retriever_search-0.2.6/retriever_search/TopicModellingInit.html
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.6/retriever_search/Utils.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      144 2024-05-28 05:29:52.000000 retriever_search-0.2.6/retriever_search/__init__.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9998 2024-05-19 17:40:04.000000 retriever_search-0.2.6/retriever_search/callbacks.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-28 05:29:55.905091 retriever_search-0.2.6/retriever_search/data/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)   337240 2024-05-02 19:07:29.000000 retriever_search-0.2.6/retriever_search/data/CountVectorizer.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)  6339926 2024-05-02 19:07:29.000000 retriever_search-0.2.6/retriever_search/data/EmbeddedVectors.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)  2102124 2024-05-02 19:07:29.000000 retriever_search-0.2.6/retriever_search/data/LDAModel.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     4301 2024-05-28 05:18:07.000000 retriever_search-0.2.6/retriever_search/frontend_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.6/retriever_search/layout.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.6/retriever_search/search_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3589 2024-05-28 05:27:12.000000 retriever_search-0.2.6/retriever_search/search_server.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1174 2024-05-19 20:59:49.000000 retriever_search-0.2.6/retriever_search/viz_server.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-28 05:29:55.914379 retriever_search-0.2.6/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2490 2024-05-28 05:29:55.000000 retriever_search-0.2.6/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      698 2024-05-28 05:29:55.000000 retriever_search-0.2.6/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-28 05:29:55.000000 retriever_search-0.2.6/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      255 2024-05-28 05:29:55.000000 retriever_search-0.2.6/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-28 05:29:55.000000 retriever_search-0.2.6/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-28 05:29:55.915500 retriever_search-0.2.6/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1128 2024-05-20 03:42:54.000000 retriever_search-0.2.6/setup.py
```

### Comparing `retriever_search-0.2.5/LICENSE` & `retriever_search-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/PKG-INFO` & `retriever_search-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.5
+Version: 0.2.6
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
@@ -78,7 +78,17 @@
 >>> vs.run_viz_server()
 ```
 
 ## Where to access the frontend 
 
 Access via the following URL - http://127.0.0.1:7860 
 This URL would work for your local setup only
+
+
+## Tickets
+
+1.0.0
+- [ ] Add lightweight embedding model support as flag in launcher
+- [ ] Remove HTML requirement for plotly visualization
+- [ ] Make LDA visualization update
+- [ ] Add model quantized
+
```

### Comparing `retriever_search-0.2.5/README.md` & `retriever_search-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -52,7 +52,17 @@
 >>> vs.run_viz_server()
 ```
 
 ## Where to access the frontend 
 
 Access via the following URL - http://127.0.0.1:7860 
 This URL would work for your local setup only
+
+
+## Tickets
+
+1.0.0
+- [ ] Add lightweight embedding model support as flag in launcher
+- [ ] Remove HTML requirement for plotly visualization
+- [ ] Make LDA visualization update
+- [ ] Add model quantized
+
```

### Comparing `retriever_search-0.2.5/retriever_search/DocumentIngestion.py` & `retriever_search-0.2.6/retriever_search/DocumentIngestion.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search/QueryPipeline.py` & `retriever_search-0.2.6/retriever_search/QueryPipeline.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search/TopicModellingInit.html` & `retriever_search-0.2.6/retriever_search/TopicModellingInit.html`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search/callbacks.py` & `retriever_search-0.2.6/retriever_search/callbacks.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search/data/CountVectorizer.pkl` & `retriever_search-0.2.6/retriever_search/data/CountVectorizer.pkl`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search/data/EmbeddedVectors.pkl` & `retriever_search-0.2.6/retriever_search/data/EmbeddedVectors.pkl`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search/data/LDAModel.pkl` & `retriever_search-0.2.6/retriever_search/data/LDAModel.pkl`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search/frontend_app.py` & `retriever_search-0.2.6/retriever_search/frontend_app.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 class gradio_app:
     def __init__(self, search_link, analysis_link):
         self.search_link = search_link
         self.analysis_link = analysis_link
         self.qa_answer_value = "### You havent asked any questions yet"
+        self.input_query = ''
 
     def load_example(self, example_id):
         global keyword
 
         data_values = { "query": str(keyword[example_id][0])}
         responses = requests.post(self.search_link + "/search_query", json=data_values)
         qa_answer = requests.get(self.search_link + "/get_qa_answer")
@@ -41,20 +42,27 @@
 
         #df, doc_ids = self.search_code_arxiv(responses)
         if [input_query] not in keyword:
             keyword.append([input_query])
 
         #file = open('./plotly_dash_viz/main.py', 'r')
         #file.close()
-        return df, keyword, gr.Markdown(self.qa_answer_value)
-
-    def export_data(self, df, query):
         if not os.path.isdir('./output/'):
             os.makedirs('./output/')
-        df.to_csv('./output/' + query + '.csv')
+        df.to_csv('./output/' + input_query.strip('?') + '.csv')
+        filepath = './output/' + input_query.strip('?') + '.csv'
+        name = input_query.strip('?') + '.csv'
+        self.input_query = input_query
+        return df, keyword, gr.Markdown(self.qa_answer_value), gr.DownloadButton(label=f"Download {name}", value=filepath, visible=True)
+
+    def export_data(self, df):
+        query = self.input_query.strip('?')
+        filepath = './output/' + query + '.csv'
+        os.remove(filepath)
+        return gr.DownloadButton(label=f"Download the file", visible=False)
 
 
     def gradio_launch(self):
         with gr.Blocks() as demo:
             with gr.Tabs() as tabs:
                 with gr.TabItem("SEARCH", id = 0):
                     gr.Markdown("# Let's Get You Started With Search")
@@ -67,19 +75,22 @@
                     examples = gr.Dataset(samples=keyword, components=[inp], type="index", label="Queries")
 
                     gr.Markdown("## Synthesized Results")
                     qa_answer_markdown = gr.Markdown(self.qa_answer_value)
 
                     gr.Markdown("## Other Relevant Papers")
                     out = gr.DataFrame(pd.DataFrame([], columns = ['Title']), wrap = True)
-                    examples.click(self.load_example, inputs=[examples], outputs=[inp, out, qa_answer_markdown])
-                    btn.click(fn=self.search_query, inputs=inp, outputs=[out, examples, qa_answer_markdown])
                     with gr.Row():
-                        btn1 = gr.Button("Export Results")
-                    btn1.click(fn=self.export_data, inputs=[out, inp], outputs=[])
+                        btn1 = gr.DownloadButton("Download the file", visible=False)
+                        #btn1 = gr.Button("Export Results")
+                    examples.click(self.load_example, inputs=[examples], outputs=[inp, out, qa_answer_markdown])
+                    btn.click(fn=self.search_query, inputs=inp, outputs=[out, examples, qa_answer_markdown, btn1])
+                    btn1.click(fn=self.export_data, inputs=[out], outputs=[btn1])
+                    #btn1.click(fn=self.export_data, inputs=[out, inp], outputs=[])
+                    #os.remove(filepath)
                 with gr.TabItem("ANALYSIS", id = 1):
                     gr.Markdown("# Analyse your searched data")
                     
                     src_val = self.analysis_link
                     html = ("<iframe id=\"iframeid\" src=" + src_val + "\ width=1200 height=2000>")
                     out1 = gr.HTML(html)
```

### Comparing `retriever_search-0.2.5/retriever_search/layout.py` & `retriever_search-0.2.6/retriever_search/layout.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search/search_app.py` & `retriever_search-0.2.6/retriever_search/search_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search/search_server.py` & `retriever_search-0.2.6/retriever_search/search_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,13 +90,13 @@
         embedding_2d.append({"doc_ids" : doc_id, "embeddings" : emb_2d})
         doc_ids.append(doc_id)
 
     df = pd.DataFrame(list(zip(titles, abstracts, arxiv_links)), columns = ['Title','Content','Link'])
     return df, doc_ids, embedding_2d, qa_answer
 
 
-def run_search_server(inputDirectory, json_save_path, device):
+def run_search_server(inputDirectory, json_save_path, hugging_face_model = 'sentence-transformers/allenai-specter', device = 'cpu'):
     global main_pipe
     print(device)
-    search_obj = search_app(inputDirectory, json_save_path, device = device)
+    search_obj = search_app(inputDirectory, json_save_path, model = hugging_face_model, device = device)
     main_pipe = search_obj.new_search_run()
     app.run(debug=False, host='127.0.0.1', threaded=True)
```

### Comparing `retriever_search-0.2.5/retriever_search/viz_server.py` & `retriever_search-0.2.6/retriever_search/viz_server.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/retriever_search.egg-info/PKG-INFO` & `retriever_search-0.2.6/retriever_search.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.5
+Version: 0.2.6
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
@@ -78,7 +78,17 @@
 >>> vs.run_viz_server()
 ```
 
 ## Where to access the frontend 
 
 Access via the following URL - http://127.0.0.1:7860 
 This URL would work for your local setup only
+
+
+## Tickets
+
+1.0.0
+- [ ] Add lightweight embedding model support as flag in launcher
+- [ ] Remove HTML requirement for plotly visualization
+- [ ] Make LDA visualization update
+- [ ] Add model quantized
+
```

### Comparing `retriever_search-0.2.5/retriever_search.egg-info/SOURCES.txt` & `retriever_search-0.2.6/retriever_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.5/setup.py` & `retriever_search-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,13 +25,13 @@
         'torch==2.2.1',
         'accelerate==0.27.2',
         'gradio==4.21.0',
         'dash==2.15.0',
         'plotly==5.10.0',
         'wordcloud',
         'pyLDAvis==3.4.1',
-        'nltk==3.7',
+        'nltk==3.7'
     ],
     packages=find_packages(),
     include_package_data=True,
     package_data={'retriever_search': ['data/CountVectorizer.pkl', 'data/EmbeddedVectors.pkl', 'data/LDAModel.pkl', 'TopicModellingInit.html']}
 )
```

