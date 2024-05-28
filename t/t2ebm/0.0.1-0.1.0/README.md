# Comparing `tmp/t2ebm-0.0.1.tar.gz` & `tmp/t2ebm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2ebm-0.0.1.tar", last modified: Fri Jul 28 02:33:07 2023, max compression
+gzip compressed data, was "t2ebm-0.1.0.tar", last modified: Tue May 28 12:37:30 2024, max compression
```

## Comparing `t2ebm-0.0.1.tar` & `t2ebm-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 02:33:07.174860 t2ebm-0.0.1/
--rw-rw-rw-   0        0        0     1089 2023-07-28 02:30:09.000000 t2ebm-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     8997 2023-07-28 02:33:07.174860 t2ebm-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8482 2023-07-28 02:30:09.000000 t2ebm-0.0.1/README.md
--rw-rw-rw-   0        0        0      111 2023-07-28 02:30:09.000000 t2ebm-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 02:33:07.174860 t2ebm-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      963 2023-07-28 02:32:45.000000 t2ebm-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:33:07.142793 t2ebm-0.0.1/t2ebm/
--rw-rw-rw-   0        0        0      159 2023-07-28 02:30:09.000000 t2ebm-0.0.1/t2ebm/__init__.py
--rw-rw-rw-   0        0        0     5321 2023-07-28 02:30:09.000000 t2ebm-0.0.1/t2ebm/_llm.py
--rw-rw-rw-   0        0        0    13747 2023-07-28 02:30:09.000000 t2ebm-0.0.1/t2ebm/graphs.py
--rw-rw-rw-   0        0        0     7419 2023-07-28 02:30:09.000000 t2ebm-0.0.1/t2ebm/prompts.py
--rw-rw-rw-   0        0        0     3083 2023-07-28 02:30:09.000000 t2ebm-0.0.1/t2ebm/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:33:07.174860 t2ebm-0.0.1/t2ebm.egg-info/
--rw-rw-rw-   0        0        0     8997 2023-07-28 02:33:07.000000 t2ebm-0.0.1/t2ebm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-07-28 02:33:07.000000 t2ebm-0.0.1/t2ebm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 02:33:07.000000 t2ebm-0.0.1/t2ebm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-28 02:33:07.000000 t2ebm-0.0.1/t2ebm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-28 02:33:07.000000 t2ebm-0.0.1/t2ebm.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-05-28 12:37:30.314637 t2ebm-0.1.0/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1068 2024-05-15 10:13:16.000000 t2ebm-0.1.0/LICENSE
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)    12934 2024-05-28 12:37:30.314637 t2ebm-0.1.0/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12263 2024-05-28 12:35:55.000000 t2ebm-0.1.0/README.md
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      107 2024-05-15 10:13:16.000000 t2ebm-0.1.0/pyproject.toml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2024-05-28 12:37:30.314637 t2ebm-0.1.0/setup.cfg
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      957 2024-05-28 12:06:08.000000 t2ebm-0.1.0/setup.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-05-28 12:37:30.314637 t2ebm-0.1.0/t2ebm/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      226 2024-05-28 12:19:48.000000 t2ebm-0.1.0/t2ebm/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5597 2024-05-28 12:19:52.000000 t2ebm-0.1.0/t2ebm/functions.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    15705 2024-05-28 12:19:53.000000 t2ebm-0.1.0/t2ebm/graphs.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4814 2024-05-28 12:11:43.000000 t2ebm-0.1.0/t2ebm/llm.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5698 2024-05-27 12:53:49.000000 t2ebm-0.1.0/t2ebm/prompts.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2772 2024-05-28 12:19:50.000000 t2ebm-0.1.0/t2ebm/utils.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-05-28 12:37:30.314637 t2ebm-0.1.0/t2ebm.egg-info/
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)    12934 2024-05-28 12:37:30.000000 t2ebm-0.1.0/t2ebm.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      317 2024-05-28 12:37:30.000000 t2ebm-0.1.0/t2ebm.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2024-05-28 12:37:30.000000 t2ebm-0.1.0/t2ebm.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       65 2024-05-28 12:37:30.000000 t2ebm-0.1.0/t2ebm.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2024-05-28 12:37:30.000000 t2ebm-0.1.0/t2ebm.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-05-28 12:37:30.314637 t2ebm-0.1.0/tests/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      652 2024-05-28 12:19:46.000000 t2ebm-0.1.0/tests/test_package.py
```

### Comparing `t2ebm-0.0.1/PKG-INFO` & `t2ebm-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,197 +1,250 @@
-Metadata-Version: 2.1
-Name: t2ebm
-Version: 0.0.1
-Summary: A Natural Language Interface to Explainable Boosting Machines
-Home-page: https://github.com/interpretml/TalkToEBM
-Author: Sebastian Bordt, Ben Lengerich, Harsha Nori, Rich Caruana
-Author-email: sbordt@posteo.de
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# TalkToEBM
-
-> ### Did you ever want to talk to a model?
-
-<p align="center">
-  <img src="images/landing.png" alt="drawing" width="900"/>
-</p>
-
-TalkToEBM is an open-source package that provides a natural language interface to [Explainable Boosting Machines (EBMs)](https://github.com/interpretml/interpret). With this package, you can convert the graphs of Explainable Boosting Machines to text and generate prompts for LLMs. We also have higher-level functions that directly ask the LLM to describe entire models. This package is under active development, so the current API is not guaranteed to stay stable.
-
-
-
-# Installation
-
-Python 3.7+ | Linux, Mac, Windows
-```sh
-pip install t2ebm
-```
-
-# High-Level API: Pass the EBM to the LLM
-
-```python
-import t2ebm
-
-gpt4 = guidance.llms.OpenAI("gpt-4")
-```
-
-We have trained an ```ExplainableBoostingClassifier``` on the Kaggle [Spaceship Titanic Dataset](https://www.kaggle.com/competitions/spaceship-titanic/overview). This dataset is from 2022, so GPT-3.5 and GPT-4 have not seen it during training. 
-
-```python
-ebm = ExplainableBoostingClassifier(feature_names=feature_names)
-ebm.fit(X_train, y_train)
-```
-Getting the LLM to describe a graph from the model is as simple as this. Let's describe the graph for feature 0, 'Home Planet'.
-
-```python
-graph_desc = t2ebm.llm_describe_ebm_graph(gpt4, ebm, 0) 
-```
-
-> **GPT-4:** *The feature "HomePlanet" significantly influences the model's outcome. Being
-from "Europa" has the highest positive effect with a mean value of 0.87. The
-"Mars" category also has a positive effect, albeit much smaller, with a mean
-value of 0.098. On the contrary, being from "Earth" negatively impacts the
-prediction, with a mean value of -0.439. The 95% confidence intervals suggest
-that these effects are statistically significant and not due to random chance.
-However, without additional context, it's difficult to determine why these
-differences occur. Further investigation would be required for a deeper
-understanding.*
-
-We can give the LLM more context by providing a description of the dataset and the outcome. This allows the LLM to talk about the spacetime anomaly.
-
-```python
-dataset_description = """ The description of the dataset from Kaggle """
-
-y_axis_description = """The y-axis depicts contributions in log-odds towards the probability
-that the passenger was transported to another dimension."""
-```
-
-
-```python
-graph_desc = t2ebm.llm_describe_ebm_graph(gpt4, ebm, 0,
-                                          dataset_description=dataset_description,
-                                          y_axis_description=y_axis_description)     
-```
-
-> **GPT-4:** *The HomePlanet feature has a significant influence on the probability of a
-passenger being transported to an alternate dimension during the collision with
-the spacetime anomaly. Passengers from Europa have the highest positive effect,
-indicating a higher likelihood of being transported. On the other hand,
-passengers from Earth have a negative effect, suggesting a lower likelihood of
-being transported. Interestingly, passengers from Mars have a smaller positive
-effect compared to Europa, but still higher than Earth. This suggests that the
-planet of origin plays a role in determining the probability of being
-transported, with passengers from Europa having the highest likelihood. However,
-there may be confounding factors or interactions with other features that
-contribute to the observed pattern, and further analysis is needed to fully
-understand the influence of the HomePlanet feature on the outcome.*
-
-Instead of describing individual graphs, we can also ask the LLM to summarize the entire model. We can also ask for a summary in a given number of sentences.
-
-```python
-model_description = t2ebm.llm_describe_ebm(gpt4, ebm,
-                                           dataset_description=dataset_description, 
-                                           y_axis_description=y_axis_description) 
-```
-
-> **GPT-4:** *Based on the global feature importances and the summaries of the individual
-features, we can provide the following summary:  The most important features in
-the model are Spa, VRDeck, CryoSleep, and RoomService.   Passengers who spent
-more at the spa had a lower probability of being affected by the anomaly. Higher
-spending on the VRDeck also decreased the likelihood of being transported,
-although there was a surprising counterintuitive behavior within a specific
-spending range.   Choosing to be in cryosleep during the voyage increased the
-probability of being affected by the anomaly, which was unexpected.   Higher
-spending on room service corresponded to a higher probability of being affected,
-but extremely high spending was associated with a lower probability.   Other
-features had lower importances and may have less significant or less
-straightforward effects on the outcome.  In summary, Spa, VRDeck, CryoSleep, and
-RoomService were the most important features. The unexpected findings, such as
-the counterintuitive influence of cryosleep and the complex relationships
-observed in features like RoomService and VRDeck, warrant further investigation
-and analysis.*
-
-# Low-Level API: Extract Graphs from the EBM and perform custom prompts
-
-```python
-import t2ebm.graphs as graphs
-```
-We have a simple datastructure for graphs, and some useful operations on them
-
-```python
-graph = graphs.extract_graph(ebm, 9)  # feature 9, 'Spa'
-graphs.plot_graph(graph)
-```
-
-<img src="images/Spaceship%20Titanic_21_0.png" alt="drawing" width="400"/>
-
-The graphs learned by EBMs can contain many small details. We can simplify them to reduce the number of tokens. There is a parameter to control the degree of simplification.
-
-```python
-t2ebm.graphs.plot_graph(t2ebm.graphs.simplify_graph(graph, min_variation_per_cent=0.041))
-```
-
-<img src="images/Spaceship%20Titanic_24_0.png" alt="drawing" width="400"/>
-
-
-The package also supports categorical and boolean features
-
-```python
-graphs.plot_graph(graphs.extract_graph(ebm, 0)) # home planet
-```
-
-<img src="images/Spaceship%20Titanic_22_0.png" alt="drawing" width="400"/>
-
-We have to convert graphs to text before passing them to the LLM
-
-```python
-graph_as_text = graphs.graph_to_text(graph, max_tokens=1000)
-print(graph_as_text)
-```
-
->    This graph represents a continuous-valued feature. The keys are intervals that represent ranges where the function predicts the same value.
->    
->    Feature Name: Spa
->    Feature Type: continuous
->    Means: {"(0.0, 36.5)": 0.517, "(36.5, 117.5)": 0.212, ..., "(3978.0, 18572.0)": -5.917}
-> 
->    Lower Bounds (95%-Confidence Interval): {"(0.0, 36.5)": 0.068, "(36.5, 117.5)": 0.049, ..., "(3978.0, 18572.0)": -6.956}
-> > 
->    Upper Bounds (95%-Confidence Interval): {"(0.0, 36.5)": 0.966, "(36.5, 117.5)": 0.374, ..., "(3978.0, 18572.0)": -4.877}
-    
-
-Given the textual representation of the graph, you can start to write your own prompts. Usually, the first prompt will ask the LLM to describe the graph. We use [guidance](https://github.com/microsoft/guidance) in order to handle sequential execution and chain-of-thought prompting.
-
-```python
-prompt = t2ebm.prompts.describe_graph(graph_as_text,
-                                      expert_description="{some kind of expert that will help me.}",
-                                      y_axis_description="{The y-axis on the graph depicts how cool the graph is.}",
-                                      special_task_description="{Pay special attention to run 'pip install t2ebm'}",
-                                      dataset_description="{My dataset is great!}",
-                                      include_assistant_response=True)
-
-# our prompts use guidance, and this is a nice way to print them
-guidance(prompt, llm=gpt4)
-```
-
-<p align="left">
-  <img src="images/part_1.png" alt="drawing" width="800"/>
-  <img src="images/part_2.png" alt="drawing" width="800"/>
-</p>
-
-# Citation
-
-If you use this software in your research, please consider to cite our paper.
-
-```bib
-@inproceedings{lengerich2023llms,
-  author    = {Benjamin J. Lengerich, Sebastian Bordt, Harsha Nori, Mark E. Nunnally, Yin Aphinyanaphongs, Manolis Kellis, and Rich Caruana},
-  title     = {LLMs Understand Glass-Box Models, Discover Surprises, and Suggest Repairs},
-  booktitle = {arxiv},
-  year      = {2023}
- }
-```
+# TalkToEBM
+![License](https://img.shields.io/github/license/interpretml/TalkToEBM.svg?style=flat-square)
+![Python Version](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10-blue)
+![Package Version](https://img.shields.io/pypi/v/t2ebm.svg?style=flat-square)
+[![Downloads](https://pepy.tech/badge/t2ebm)](https://pepy.tech/project/t2ebm)
+<br/>
+
+> ### A Natural Language Interface to Explainable Boosting Machines
+
+<p align="center">
+  <img src="images/landing.png" alt="drawing" width="900"/>
+</p>
+
+TalkToEBM is an open-source package that provides a natural language interface to [Explainable Boosting Machines (EBMs)](https://github.com/interpretml/interpret). With this package, you can convert the graphs of Explainable Boosting Machines to text and generate prompts for LLMs. We also have higher-level functions that directly ask the LLM to describe entire models. This package is under active development, so the current API is not guaranteed to stay stable.
+
+Features:
+- [x] Convert EBMs and their graphs to text that can be understood by LLMs. Includes confidence intervals.
+- [x] Ask the LLM to describe and summarize individual graphs or entire models.
+- [x] Modular approach that allows to write custom prompts - ask the LLM to perform any desired task with the EBM.
+- [x] Automatic simplification of minor details in graphs to stay within the desired token limit.
+
+# Installation
+
+Python 3.7+ | Linux, Mac, Windows
+```sh
+pip install t2ebm
+```
+
+# High-Level API: Pass the EBM to the LLM
+
+We have trained an ```ExplainableBoostingClassifier``` on the Kaggle [Spaceship Titanic Dataset](https://www.kaggle.com/competitions/spaceship-titanic/overview).
+
+```python
+ebm = ExplainableBoostingClassifier(feature_names=feature_names)
+ebm.fit(X_train, y_train)
+```
+Getting the LLM to describe a graph from the model is as simple as this. Let's describe the graph for feature 0, 'Home Planet'.
+
+```python
+import t2ebm
+
+t2ebm.describe_graph('gpt-4-turbo-2024-04-09', ebm, 0)
+```
+
+> **GPT-4:** *The graph illustrates the effects of the categorical feature `HomePlanet` on a
+dependent variable, as modeled by a Generalized Additive Model (GAM). The
+feature `HomePlanet` includes three categories: "Earth," "Europa," and "Mars."
+Passengers from Europa exhibit a notably high positive mean effect of 0.5678 on
+the dependent variable, with a tight confidence interval ranging from 0.5116 to
+0.624, suggesting a strong and consistent positive impact. In contrast, Earth
+shows a negative mean effect of -0.3246 with the confidence interval from -0.354
+to -0.2952, indicating a robust negative association. Mars, while also positive,
+has a much milder effect of 0.1713, with its confidence interval spanning from
+0.1256 to 0.2171. This pronounced disparity in the effects, especially the
+negative impact associated with Earth, is surprising and could hint at
+underlying socio-economic or contextual factors influencing these outcomes.
+Understanding these patterns might require further investigation into the
+dataset's characteristics, including possible biases or the nature of the
+dependent variable.*
+
+We can give the LLM more context by providing a description of the dataset and the outcome. This allows the LLM to talk about the spacetime anomaly.
+
+```python
+dataset_description = """ The description of the dataset from Kaggle """
+
+y_axis_descripton = """The y-axis depicts contributions in log-odds towards the probability
+that the passenger was transported to another dimension."""
+```
+
+
+```python
+t2ebm.describe_graph('gpt-4-turbo-2024-04-09', 
+                      ebm,
+                      0, 
+                      graph_description=y_axis_descripton,
+                      dataset_description=dataset_description)  
+```
+
+> **GPT-4:** *The graph from the Generalized Additive Model (GAM) showcases the contributions
+of different home planets—Earth, Europa, and Mars—towards the log-odds of
+passengers being transported to another dimension on the Spaceship Titanic.
+Passengers from Europa exhibit a strong positive contribution to the likelihood
+of being transported, with a mean log-odds contribution of 0.5678, indicating a
+higher propensity for these individuals to experience the anomalous event.
+Conversely, Earth shows a negative contribution (-0.3246 mean log-odds),
+suggesting that passengers from Earth are less likely to be transported compared
+to the baseline. Mars, while also showing a positive contribution (0.1713 mean
+log-odds), has a lesser effect than Europa, but still indicates an increased
+likelihood over Earth. This pattern could suggest unique environmental,
+technological, or cultural factors on Europa and Mars that influence their
+inhabitants' interactions with the spacetime anomaly encountered during the
+voyage. The observed negative contribution from Earth might hint at more
+effective protective measures or less vulnerability to such spacetime
+disturbances. These findings highlight planet-based differences in
+susceptibility to extraordinary events, revealing insights into interplanetary
+travel and safety in this futuristic scenario.*
+
+Instead of describing individual graphs, we can also ask the LLM to summarize the entire model. We can also ask for a summary in a given number of sentences.
+
+```python
+t2ebm.llm_describe_ebm('gpt-4-turbo-2024-04-09',
+                       ebm,
+                       dataset_description=dataset_description, 
+                       y_axis_description=y_axis_descripton) 
+```
+
+> **GPT-4:** *The Generalized Additive Model (GAM) applied to the Spaceship Titanic dataset
+has uncovered significant relationships between passenger features and the
+likelihood of being transported to an alternate dimension during a spacetime
+anomaly. Here's a condensed summary of the key findings:  1. **CryoSleep**
+(Feature Importance: 0.56):    - Passengers in CryoSleep are significantly more
+likely to be transported (mean effect = 0.814) compared to those not in
+CryoSleep (mean effect = -0.447). This suggests unique interactions between the
+CryoSleep technology and the anomaly.  2. **Spa** (Feature Importance: 0.72):
+There is a strong negative correlation between spa spending and the likelihood
+of transportation, with a steep decline in likelihood as expenditures increase.
+This counterintuitive pattern points to complex, non-linear effects of luxury
+expenditures on outcomes.  3. **VRDeck** (Feature Importance: 0.63):    - Higher
+spending on the VRDeck is associated with a lower likelihood of being
+transported, with an increasing negative effect as expenditure rises.  4.
+**RoomService** (Feature Importance: 0.48):    - Minimal initial spending on
+room service slightly increases the likelihood of being transported, but as
+spending rises, the effect becomes negatively pronounced. This indicates complex
+interactions influenced by passenger behavior or security measures.  5.
+**HomePlanet** (Feature: 0.35):    - Europa passengers are notably more likely
+to be transported (mean = 0.5678) compared to those from Earth (mean = -0.3246)
+and Mars (mean = 0.1713), suggesting differences in technology or emergency
+responses among the planets.  6. **Cabin** (Feature: 0.39):    - Cabin location
+significantly affects transportation likelihood, with notable disparities
+between cabin sides (Port vs. Starboard) on the same deck, indicating uneven
+exposure to the anomaly or structural differences in the ship.  Surprising
+Patterns: - **Age**: There's a non-linear relationship with age, where both very
+young and older seniors show higher transportation probabilities, highlighting
+age-specific dynamics in anomaly interaction. - **Destination**: Passengers to
+"55 Cancri e" have a higher transportation likelihood compared to other
+destinations, indicating unique risks associated with this route.  This GAM
+analysis provides crucial insights into the dynamics of spacetime anomalies in
+interstellar travel, emphasizing the importance of considering complex and non-
+linear interactions between features and outcomes for safety and operational
+strategies.*
+
+# Low-Level API: Extract Graphs from the EBM and perform custom prompts
+
+```python
+import t2ebm.graphs as graphs
+```
+We have a simple datastructure for graphs, and some useful operations on them
+
+```python
+graph = graphs.extract_graph(ebm, 9)  # feature 9, 'Spa'
+graphs.plot_graph(graph)
+```
+
+<img src="images/Spaceship%20Titanic_21_0.png" alt="drawing" width="400"/>
+
+The graphs learned by EBMs can contain many small details. We can simplify them to reduce the number of tokens. There is a parameter to control the degree of simplification.
+
+```python
+t2ebm.graphs.plot_graph(t2ebm.graphs.simplify_graph(graph, min_variation_per_cent=0.041))
+```
+
+<img src="images/Spaceship%20Titanic_24_0.png" alt="drawing" width="400"/>
+
+
+The package also supports categorical and boolean features
+
+```python
+graphs.plot_graph(graphs.extract_graph(ebm, 0)) # home planet
+```
+
+<img src="images/Spaceship%20Titanic_22_0.png" alt="drawing" width="400"/>
+
+We have to convert graphs to text before passing them to the LLM
+
+```python
+graph_as_text = graphs.graph_to_text(graph, max_tokens=1000)
+print(graph_as_text)
+```
+
+>    This graph represents a continuous-valued feature. The keys are intervals that represent ranges where the function predicts the same value.
+>    
+>    Feature Name: Spa
+>    Feature Type: continuous
+>    Means: {"(0.0, 36.5)": 0.517, "(36.5, 117.5)": 0.212, ..., "(3978.0, 18572.0)": -5.917}
+> 
+>    Lower Bounds (95%-Confidence Interval): {"(0.0, 36.5)": 0.068, "(36.5, 117.5)": 0.049, ..., "(3978.0, 18572.0)": -6.956}
+> > 
+>    Upper Bounds (95%-Confidence Interval): {"(0.0, 36.5)": 0.966, "(36.5, 117.5)": 0.374, ..., "(3978.0, 18572.0)": -4.877}
+    
+
+Given the textual representation of the graph, you can start to write your own prompts. Usually, the first prompt will ask the LLM to describe the graph. 
+
+```python
+t2ebm.prompts.describe_graph(graph_as_text,
+                             graph_description="{The y-axis on the graph depicts how cool the graph is.}",
+                             dataset_description="{The dataset is great!}",
+                             task_description="{Please summarize the graph. Pay special attention to run 'pip install t2ebm'}",)
+```
+
+```
+Below is the graph of a Generalized Additive Model (GAM). The graph is presented as a JSON object with keys representing the x-axis and values representing the y-axis. For continuous features, the keys are intervals that represent ranges where the function predicts the same value. For categorical features, each key represents a possible value that the feature can take.
+    
+The graph is provided in the following format:
+    - The name of the feature depicted in the graph
+    - The type of the feature (continuous, categorical, or boolean)
+    - Mean values
+    - Lower bounds of confidence interval (optional)
+    - Upper bounds of confidence interval (optional)
+
+Here is the graph:
+
+This graph represents categorical feature. Each key represents a possible value that the feature can take.
+
+Feature Name: HomePlanet
+Feature Type: categorical
+Means: {"Earth": -0.3246, "Europa": 0.5678, "Mars": 0.1713}
+Lower Bounds (95%-Confidence Interval): {"Earth": -0.354, "Europa": 0.5116, "Mars": 0.1256}
+Upper Bounds (95%-Confidence Interval): {"Earth": -0.2952, "Europa": 0.624, "Mars": 0.2171}
+
+
+{The y-axis on the graph depicts how cool the graph is.}
+
+Here is a description of the dataset that the model was trained on:
+
+{The dataset is great!}
+
+{Please summarize the graph. Pay special attention to run 'pip install t2ebm'}
+```
+
+# Citation
+
+If you use this software in your research, please consider citing our research papers.
+
+```bib
+@inproceedings{bordt2024talktoebm,
+  author    = {Sebastian Bordt, Ben Lengerich, Harsha Nori, Rich Caruana},
+  title     = {Data Science with LLMs and Interpretable Models},
+  booktitle = {XAI4Sci Workshop at AAAI-24},
+  year      = {2024}
+ }
+```
+
+```bib
+@inproceedings{lengerich2023llms,
+  author    = {Benjamin J. Lengerich, Sebastian Bordt, Harsha Nori, Mark E. Nunnally, Yin Aphinyanaphongs, Manolis Kellis, and Rich Caruana},
+  title     = {LLMs Understand Glass-Box Models, Discover Surprises, and Suggest Repairs},
+  booktitle = {arxiv},
+  year      = {2023}
+ }
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `t2ebm-0.0.1/setup.py` & `t2ebm-0.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="t2ebm",
-    version="0.0.1",
-    author="Sebastian Bordt, Ben Lengerich, Harsha Nori, Rich Caruana",
-    author_email="sbordt@posteo.de",
-    description="A Natural Language Interface to Explainable Boosting Machines",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/interpretml/TalkToEBM",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    package_dir={"": "."},
-    packages=["t2ebm"],
-    python_requires=">=3.6",
-    install_requires=[
-        "numpy",
-        "matplotlib",
-        "tiktoken",
-        "guidance",
-        "openai",
-        "tenacity",
-        "scipy",
-        "interpret",
-    ],
-)
+"""
+TalkToEBM installation script.
+"""
+
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="t2ebm",
+    version="0.1.0",
+    author="Sebastian Bordt, Ben Lengerich, Harsha Nori, Rich Caruana",
+    author_email="sbordt@posteo.de",
+    description="A Natural Language Interface to Explainable Boosting Machines",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/interpretml/TalkToEBM",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    package_dir={"": "."},
+    packages=["t2ebm"],
+    python_requires=">=3.6",
+    install_requires=[
+        "numpy",
+        "matplotlib",
+        "tiktoken",
+        "openai>=1.8.0",
+        "tenacity",
+        "scipy",
+        "interpret",
+    ],
+)
```

### Comparing `t2ebm-0.0.1/t2ebm/_llm.py` & `t2ebm-0.1.0/t2ebm/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,128 +1,158 @@
-################################################################################################################
-# TalkToEBM: A Natural Language Interface to Explainable Boosting Machines
-################################################################################################################
-
-import numpy as np
-
-
-import inspect
-
-import guidance
-
-
-from t2ebm.graphs import extract_graph, graph_to_text
-
-import t2ebm.prompts as prompts
-
-################################################################################################################
-# Talk to the EBM about other things than graphs.
-################################################################################################################
-
-
-def feature_importances_to_text(ebm):
-    feature_importances = ""
-    for feature_idx, feature_name in enumerate(ebm.feature_names_in_):
-        feature_importances += (
-            f"{feature_name}: {ebm.term_importances()[feature_idx]:.2f}\n"
-        )
-    return feature_importances
-
-
-################################################################################################################
-# Ask the LLM to perform high-level tasks directly on the EBM.
-################################################################################################################
-
-
-def llm_describe_ebm_graph(llm, ebm, feature_index, num_sentences=7, **kwargs):
-    """Ask the LLM to describe a graph from an EBM, using chain-of-thought reasoning.
-
-    This function accepts arbitrary keyword arguments that are passed to the corresponding lower-level functions.
-
-    :param ebm:
-    :param feature_index:
-    :param kwargs: see llm_describe_graph
-    :return: A summary of the graph in at most num_sentences sentences.
-    """
-
-    # extract the graph from the EBM
-    extract_kwargs = list(inspect.signature(extract_graph).parameters)
-    extract_dict = {k: kwargs[k] for k in dict(kwargs) if k in extract_kwargs}
-    graph = extract_graph(ebm, feature_index, **extract_dict)
-
-    # convert the graph to text
-    to_text_kwargs = list(inspect.signature(graph_to_text).parameters)
-    to_text_dict = {k: kwargs[k] for k in dict(kwargs) if k in to_text_kwargs}
-    graph = graph_to_text(graph, **to_text_dict)
-
-    # ask the LLM to describe the graph and execute the prompt
-    llm_descripe_kwargs = list(inspect.signature(prompts.describe_graph_cot).parameters)
-    llm_descripe_kwargs.extend(
-        list(inspect.signature(prompts.describe_graph).parameters)
-    )
-    llm_descripe_dict = {k: kwargs[k] for k in dict(kwargs) if k in llm_descripe_kwargs}
-    prompt = prompts.describe_graph_cot(
-        graph, num_sentences=num_sentences, **llm_descripe_dict
-    )
-
-    return guidance(prompt, llm, silent=True)()["cot_graph_description"]
-
-
-def llm_describe_ebm(llm, ebm, num_sentences=30, **kwargs):
-    """Ask the LLM to describe the LLM in at most {num_sentences} sentences."""
-
-    # Note: We convert all objects to text before we prompt the LLM the first time.
-    # The idea is that if there is an error processing one of the graphs, we get it before we prompt the LLM.
-    feature_importances = feature_importances_to_text(ebm)
-
-    # extract the graphs from the EBM
-    extract_kwargs = list(inspect.signature(extract_graph).parameters)
-    extract_dict = {k: kwargs[k] for k in dict(kwargs) if k in extract_kwargs}
-    graphs = []
-    for feature_index in range(len(ebm.feature_names_in_)):
-        graphs.append(extract_graph(ebm, feature_index, **extract_dict))
-
-    # convert the graphs to text
-    to_text_kwargs = list(inspect.signature(graph_to_text).parameters)
-    to_text_dict = {k: kwargs[k] for k in dict(kwargs) if k in to_text_kwargs}
-    graphs = [graph_to_text(graph, **to_text_dict) for graph in graphs]
-
-    # construct guidance prompts that ask the LLM to describe the graphs
-    llm_descripe_kwargs = list(inspect.signature(prompts.describe_graph_cot).parameters)
-    llm_descripe_kwargs.extend(
-        list(inspect.signature(prompts.describe_graph).parameters)
-    )
-    llm_descripe_dict = {
-        k: kwargs[k]
-        for k in dict(kwargs)
-        if k in llm_descripe_kwargs and k != "num_sentences"
-    }
-    graph_prompts = [
-        prompts.describe_graph_cot(graph, num_sentences=7, **llm_descripe_dict)
-        for graph in graphs
-    ]
-
-    # execute the prompts
-    graph_descriptions = [
-        guidance(p, llm, silent=True)()["cot_graph_description"] for p in graph_prompts
-    ]
-
-    # combine the graph descriptions in a single string
-    graph_descriptions = "\n\n".join(
-        [
-            ebm.feature_names_in_[idx] + ": " + graph_description
-            for idx, graph_description in enumerate(graph_descriptions)
-        ]
-    )
-
-    # now, ask the llm to summarize the different descriptions
-    llm_summarize_kwargs = list(inspect.signature(prompts.summarize_ebm).parameters)
-    llm_summarize_dict = {
-        k: kwargs[k] for k in dict(kwargs) if k in llm_summarize_kwargs
-    }
-    prompt = prompts.summarize_ebm(
-        feature_importances,
-        graph_descriptions,
-        num_sentences=num_sentences,
-        **llm_summarize_dict,
-    )
-    return guidance(prompt, llm, silent=True)()["short_summary"]
+"""
+TalkToEBM: A Natural Language Interface to Explainable Boosting Machines
+"""
+
+import inspect
+
+from typing import Union
+
+import t2ebm
+import t2ebm.llm
+from t2ebm.llm import AbstractChatModel
+
+from t2ebm.graphs import extract_graph, graph_to_text
+
+import t2ebm.prompts as prompts
+
+from interpret.glassbox import (
+    ExplainableBoostingClassifier,
+    ExplainableBoostingRegressor,
+)
+
+###################################################################################################
+# Talk to the EBM about other things than graphs.
+###################################################################################################
+
+
+def feature_importances_to_text(ebm):
+    feature_importances = ""
+    for feature_idx, feature_name in enumerate(ebm.feature_names_in_):
+        feature_importances += (
+            f"{feature_name}: {ebm.term_importances()[feature_idx]:.2f}\n"
+        )
+    return feature_importances
+
+
+################################################################################################################
+# Ask the LLM to perform high-level tasks directly on the EBM.
+################################################################################################################
+
+
+def describe_graph(
+    llm: Union[AbstractChatModel, str],
+    ebm: Union[ExplainableBoostingClassifier, ExplainableBoostingRegressor],
+    feature_index: int,
+    num_sentences: int = 7,
+    **kwargs,
+):
+    """Ask the LLM to describe a graph from an EBM, using chain-of-thought reasoning.
+
+    This function accepts arbitrary keyword arguments that are passed to the corresponding lower-level functions.
+
+    :param ebm:
+    :param feature_index:
+    :param kwargs: see llm_describe_graph
+    :return: A summary of the graph in at most num_sentences sentences.
+    """
+
+    # llm setup
+    llm = t2ebm.llm.setup(llm)
+
+    # extract the graph from the EBM
+    extract_kwargs = list(inspect.signature(extract_graph).parameters)
+    extract_dict = {k: kwargs[k] for k in dict(kwargs) if k in extract_kwargs}
+    graph = extract_graph(ebm, feature_index, **extract_dict)
+
+    # convert the graph to text
+    to_text_kwargs = list(inspect.signature(graph_to_text).parameters)
+    to_text_dict = {k: kwargs[k] for k in dict(kwargs) if k in to_text_kwargs}
+    graph = graph_to_text(graph, **to_text_dict)
+
+    # get a cot sequence of messages to describe the graph
+    llm_descripe_kwargs = list(inspect.signature(prompts.describe_graph_cot).parameters)
+    llm_descripe_kwargs.extend(
+        list(inspect.signature(prompts.describe_graph).parameters)
+    )
+    llm_descripe_dict = {k: kwargs[k] for k in dict(kwargs) if k in llm_descripe_kwargs}
+    messages = prompts.describe_graph_cot(
+        graph, num_sentences=num_sentences, **llm_descripe_dict
+    )
+
+    # execute the prompt
+    messages = t2ebm.llm.chat_completion(llm, messages)
+
+    # the last message contains the summary
+    return messages[-1]["content"]
+
+
+def describe_ebm(
+    llm: Union[AbstractChatModel, str],
+    ebm: Union[ExplainableBoostingClassifier, ExplainableBoostingRegressor],
+    num_sentences: int = 30,
+    **kwargs,
+):
+    """Ask the LLM to describe the LLM in at most {num_sentences} sentences."""
+
+    # llm setup
+    llm = t2ebm.llm.setup(llm)
+
+    # Note: We convert all objects to text before we prompt the LLM the first time.
+    # The idea is that if there is an error processing one of the graphs, we get it before we prompt the LLM.
+    feature_importances = feature_importances_to_text(ebm)
+
+    # extract the graphs from the EBM
+    extract_kwargs = list(inspect.signature(extract_graph).parameters)
+    extract_dict = {k: kwargs[k] for k in dict(kwargs) if k in extract_kwargs}
+    graphs = []
+    for feature_index in range(len(ebm.feature_names_in_)):
+        graphs.append(extract_graph(ebm, feature_index, **extract_dict))
+
+    # convert the graphs to text
+    to_text_kwargs = list(inspect.signature(graph_to_text).parameters)
+    to_text_dict = {k: kwargs[k] for k in dict(kwargs) if k in to_text_kwargs}
+    graphs = [graph_to_text(graph, **to_text_dict) for graph in graphs]
+
+    # get a cot sequence of messages to describe the graph
+    llm_descripe_kwargs = list(inspect.signature(prompts.describe_graph_cot).parameters)
+    llm_descripe_kwargs.extend(
+        list(inspect.signature(prompts.describe_graph).parameters)
+    )
+    llm_descripe_dict = {
+        k: kwargs[k]
+        for k in dict(kwargs)
+        if k in llm_descripe_kwargs and k != "num_sentences"
+    }
+    messages = [
+        prompts.describe_graph_cot(graph, num_sentences=7, **llm_descripe_dict)
+        for graph in graphs
+    ]
+
+    # execute the prompts
+    graph_descriptions = [
+        t2ebm.llm.chat_completion(llm, msg)[-1]["content"] for msg in messages
+    ]
+
+    # combine the graph descriptions in a single string
+    graph_descriptions = "\n\n".join(
+        [
+            ebm.feature_names_in_[idx] + ": " + graph_description
+            for idx, graph_description in enumerate(graph_descriptions)
+        ]
+    )
+
+    # print(graph_descriptions)
+
+    # now, ask the llm to summarize the different descriptions
+    llm_summarize_kwargs = list(inspect.signature(prompts.summarize_ebm).parameters)
+    llm_summarize_dict = {
+        k: kwargs[k] for k in dict(kwargs) if k in llm_summarize_kwargs
+    }
+    messages = prompts.summarize_ebm(
+        feature_importances,
+        graph_descriptions,
+        num_sentences=num_sentences,
+        **llm_summarize_dict,
+    )
+
+    # execute the prompt and return the summary
+    return t2ebm.llm.chat_completion(llm, messages)[-1]["content"]
```

### Comparing `t2ebm-0.0.1/t2ebm/graphs.py` & `t2ebm-0.1.0/t2ebm/graphs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,320 +1,384 @@
-from interpret.glassbox._ebm._utils import convert_to_intervals
-
-import numpy as np
-
-from dataclasses import dataclass
-
-import matplotlib.pyplot as plt
-
-
-import typing
-
-
-import scipy
-
-from t2ebm.utils import num_tokens_from_string_
-
-
-################################################################################################################
-# Put individual graphs to text
-# Also has a datatype for graphs and various simple operations on this datatype.
-################################################################################################################
-
-
-# a low-level datastructure for the graphs of explainable boosting machines
-@dataclass
-class EBMGraph:
-    feature_name: str
-    feature_type: str
-    x_vals: typing.List[
-        typing.Tuple[float, float]
-    ]  # todo add union with categorical features
-    scores: typing.List[float]
-    stds: typing.List[float]
-
-
-def extract_graph(
-    ebm,
-    feature_index,
-    normalization="none",
-    use_feature_bounds=True,
-):
-    """Extract a graph from an Explainable Boosting Machine.
-
-    This is a low-level function. It does not return the final format in which the graph is presented to the LLM.
-
-    The purpose of this function is to extract the graph from the interals of the EBM and return it in a format that is easy to work with.
-
-    :param ebm:
-    :param feature_index:
-    :param normalization: how to normalize the graph. possible values are: 'mean', 'min', 'none'
-    :param use_feature_bounds: if True, the first and last bin are min and max value of the feature stored in the EBM. If false, the first and last value are -inf and inf, respectively.
-    :return: EBMGraph
-    """
-
-    # read the variables from the ebm
-    feature_name = ebm.feature_names_in_[feature_index]
-    feature_type = ebm.feature_types_in_[feature_index]
-    scores = ebm.term_scores_[feature_index][1:-1]  # Drop missing and unknown bins
-    stds = ebm.standard_deviations_[feature_index][1:-1]
-
-    # normalize the graph
-    normalization_constant = None
-    if normalization == "mean":
-        normalization_constant = np.mean(scores)
-    elif normalization == "min":
-        normalization_constant = np.min(scores)
-    elif normalization == "none":
-        normalization_constant = 0
-    else:
-        raise Exception(f"Unknown normalization {normalization}")
-    scores = scores - normalization_constant
-
-    # read the x-axis bins from the ebm
-    if feature_type == "continuous":
-        x_vals = convert_to_intervals(ebm.bins_[feature_index][0])
-        # feature bounds apply to continuous features only
-        if use_feature_bounds:
-            x_vals[0] = (ebm.feature_bounds_[feature_index][0], x_vals[0][1])
-            x_vals[-1] = (x_vals[-1][0], ebm.feature_bounds_[feature_index][1])
-    elif feature_type == "nominal":
-        x_vals = ebm.bins_[feature_index][
-            0
-        ]  # todo: check this transformation with Paul
-        x_vals = {v - 1: k for k, v in x_vals.items()}
-        x_vals = [x_vals[idx] for idx in range(len(x_vals.keys()))]
-    else:
-        raise Exception(
-            f"Feature {feature_index} is of unknown feature_type {feature_type}."
-        )
-    assert len(x_vals) == len(scores), "The number of bins and scores does not match."
-
-    return EBMGraph(feature_name, feature_type, x_vals, scores, stds)
-
-
-def simplify_graph(graph: EBMGraph, min_variation_per_cent: float = 0.0):
-    """Simplifies a graph. Removes redundant (flat) bins from the graph.
-
-    With min_variation_per_cent>0 (default 0.0), the function simplifies the graph by removing bins
-    that correspond to a less that min_variation_per_cent change in the score, considering the overal min/max difference of score for the feature as 100%.
-    this can be useful to keep a query within the context limit. Empirically, removing changes of less than 2% simplifies graphs a lot
-    in terms of the number of bins/tokens, but visually we can hardly see the difference.
-
-    :param bins:
-    :param scores:
-    :return: EBMGraph. A new simplified graph.
-    """
-    assert graph.feature_type == "continuous", "Can only simplify continuous graphs."
-    x_vals, scores, stds = graph.x_vals, graph.scores, graph.stds
-    total_variation = np.max(scores) - np.min(scores)
-    new_x_vals, new_scores, new_stds = [], [], []
-    for idx, (b0, b1) in enumerate(x_vals):
-        if idx == 0:
-            new_x_vals.append((b0, b1))
-            new_scores.append(scores[idx])
-            new_stds.append(stds[idx])
-        else:
-            score_prev = new_scores[-1]
-            if (
-                np.abs(float(score_prev) - float(scores[idx]))
-                <= total_variation * min_variation_per_cent
-            ):
-                # extend the previous bin to b1
-                new_x_vals[-1] = (new_x_vals[-1][0], b1)
-                # guarantee that the the confidence bands of the simplified graph cover the original graph as well as its confidence bands
-                new_stds[-1] = max(new_stds[-1], stds[idx])
-            else:
-                new_x_vals.append((b0, b1))
-                new_scores.append(scores[idx])
-                new_stds.append(stds[idx])
-    return EBMGraph(
-        graph.feature_name, graph.feature_type, new_x_vals, new_scores, new_stds
-    )
-
-
-def plot_graph(graph: EBMGraph):
-    x_vals, scores, stds = graph.x_vals, graph.scores, graph.stds
-    if graph.feature_type == "continuous":
-        x, y, y_lower, y_upper = [], [], [], []
-        for idx, bin in enumerate(x_vals):
-            if bin[0] == -np.inf or bin[1] == np.inf:
-                continue
-            # left part of the bin
-            x.append(bin[0] + 1e-12)
-            y.append(scores[idx])
-            y_lower.append(scores[idx] - stds[idx])
-            y_upper.append(scores[idx] + stds[idx])
-            # right part of the bin
-            x.append(bin[1])
-            y.append(scores[idx])
-            y_lower.append(scores[idx] - stds[idx])
-            y_upper.append(scores[idx] + stds[idx])
-        # plot
-        fig = plt.figure()
-        plt.plot(x, y)
-        plt.fill_between(x, y_lower, y_upper, alpha=0.2)
-    elif (
-        graph.feature_type == "nominal"
-        or graph.feature_type == "boolean"
-        or graph.feature_type == "categorical"
-    ):
-        # plot bins for the categorical features
-        fig = plt.figure()
-        plt.bar(x_vals, scores, yerr=stds)
-    else:
-        raise Exception(f"Unknown graph feature type {graph.feature_type}.")
-    plt.xlabel(graph.feature_name)
-    plt.title(f"{graph.feature_name} ({graph.feature_type})")
-
-
-def xy_to_json_(x_vals, y_vals):
-    """convert a sequence of x_vals and y_vals to a json string"""
-    # continuous features
-    if isinstance(x_vals[0], tuple):
-        return (
-            "{"
-            + ", ".join([f'"({x[0]}, {x[1]})": {y}' for x, y in zip(x_vals, y_vals)])
-            + "}"
-        )
-    # other features
-    return "{" + ", ".join([f'"{x}": {y}' for x, y in zip(x_vals, y_vals)]) + "}"
-
-
-def graph_to_text(
-    graph: EBMGraph,
-    include_description=True,
-    feature_format=None,
-    x_axis_precision=None,
-    y_axis_precision="auto",
-    confidence_bounds=True,
-    confidence_level=0.95,
-    max_tokens=3000,
-):
-    """Convert a graph to a textual representation that can be passed to a LLM.
-
-    This function takes care of all the different formatting issues that can arise in this process.
-
-    The user can explicitly specify the format of the feature (continuous, cateorical, boolean), as well as the precision of the values on the x-axis and y-axis. If the user does not specify these values, the function will try to infer them from the graph.
-
-    By default, this functions adds a short descriptive text that describes the graph to the LLM.
-
-    This function simplifies the graph so that the textual description length is at most {max_tokens} GPT-4 tokens.
-    """
-
-    # a simple auto-detect for boolean feautres
-    try:
-        if (
-            len(graph.x_vals) == 2
-            and graph.x_vals[0].upper() == "FALSE"
-            and graph.x_vals[1].upper() == "TRUE"
-        ):
-            feature_format = "boolean"
-    except:
-        pass
-
-    # determine the feature format
-    if feature_format is None:
-        feature_format = graph.feature_type
-    if feature_format == "nominal":
-        feature_format = "categorical"
-
-    # the description of the graph depends on the feature format
-    if feature_format == "continuous":
-        description_text = "This graph represents a continuous-valued feature. The keys are intervals that represent ranges where the function predicts the same value.\n\n"
-    elif feature_format == "categorical":
-        description_text = "This graph represents categorical feature. Each key represents a possible value that the feature can take.\n\n"
-    elif feature_format == "boolean":
-        description_text = "This graph represents a boolean feature. The keys are 'True' and 'False', the two possible values of the feature.\n\n"
-    else:
-        raise Exception(f"Unknown feature format {feature_format}")
-
-    # simplify the graph until it fits into the max_tokens limit
-    total_tokens = None
-    min_variation_per_cent = 0.0
-    while True:
-        # simplify the graph
-        simplified_graph = graph
-        if feature_format == "continuous":
-            simplified_graph = simplify_graph(
-                graph, min_variation_per_cent=min_variation_per_cent
-            )
-
-        # confidence bounds via normal approximation
-        scores = simplified_graph.scores
-        if confidence_bounds:
-            factor = scipy.stats.norm.interval(confidence_level, loc=0, scale=1)[1]
-            lower_bounds = [
-                scores[idx] - factor * simplified_graph.stds[idx]
-                for idx in range(len(scores))
-            ]
-            upper_bounds = [
-                scores[idx] + factor * simplified_graph.stds[idx]
-                for idx in range(len(scores))
-            ]
-
-        # adjust the precision on the x-axis. this can be dangerous if we don't know the distribution of the data (it can impact the accuracy).
-        # however, this is a necessary formatting feature because certain (old?) versions of EBMs introduce trailing digits for the xbins (e.g. age as a floating point number with 10 significant digits)
-        x_vals = simplified_graph.x_vals
-        if x_axis_precision is not None:
-            x_vals = [
-                (
-                    np.round(x[0], x_axis_precision).astype(str),
-                    np.round(x[1], x_axis_precision).astype(str),
-                )
-                for x in x_vals
-            ]
-
-        # adjust the precision on the y-axis
-        if y_axis_precision == "auto":  # at least 3 significant digits
-            total_variation = np.max(scores) - np.min(scores)
-            y_fraction = total_variation / 100.0
-            y_axis_precision = 1
-            while y_fraction < 1:
-                y_fraction *= 10
-                y_axis_precision += 1
-        scores = np.round(scores, y_axis_precision).astype(str)
-        if confidence_bounds:
-            lower_bounds = np.round(lower_bounds, y_axis_precision).astype(str)
-            upper_bounds = np.round(upper_bounds, y_axis_precision).astype(str)
-
-        # formatting for boolean features
-        if feature_format == "boolean":
-            assert (
-                len(x_vals) == 2
-            ), f"Requested a boolean format, but the feature has more than x-axis values: {x_vals}"
-            # we assume that the left key (the lower numer, typically -1 or 0), is 'False'
-            x_vals = ["False", "True"]
-
-        # create the textual representation of the graph
-        prompt = ""
-        if include_description:
-            prompt += description_text
-        prompt += f"Feature Name: {graph.feature_name}\n"
-        prompt += f"Feature Type: {feature_format}\n"
-        prompt += f"Means: {xy_to_json_(x_vals, scores)}\n"
-        if confidence_bounds:
-            prompt += f"Lower Bounds ({confidence_level*100:.0f}%-Confidence Interval): {xy_to_json_(x_vals, lower_bounds)}\n"
-            prompt += f"Upper Bounds ({confidence_level*100:.0f}%-Confidence Interval): {xy_to_json_(x_vals, upper_bounds)}\n"
-
-        # count the number of tokens
-        total_tokens = num_tokens_from_string_(prompt, "gpt-4")
-        if feature_format == "continuous":
-            if total_tokens > max_tokens:
-                if min_variation_per_cent > 0.1:
-                    raise Exception(
-                        f"The graph for feature {graph.feature_name} of type {graph.feature_type} requires {total_tokens} tokens even at a simplification level of 10\%. This graph is too complex to be passed to the LLM within the loken limit of {max_tokens} tokens."
-                    )
-                min_variation_per_cent += 0.001
-            else:
-                if min_variation_per_cent > 0:
-                    print(
-                        f"INFO: The graph of feature {graph.feature_name} was simplified by {min_variation_per_cent * 100:.1f}%."
-                    )
-                return prompt
-        else:
-            if total_tokens > max_tokens:
-                raise Exception(
-                    f"The graph for feature {graph.feature_name} of type {graph.feature_type} requires {total_tokens} tokens and exceeds the token limit of {max_tokens}."
-                )
-            else:
-                return prompt
+from dataclasses import dataclass
+import typing
+
+import matplotlib.pyplot as plt
+import numpy as np
+import scipy
+import json
+
+from interpret.glassbox._ebm._utils import convert_to_intervals
+
+from t2ebm.utils import num_tokens_from_string_
+
+###################################################################################################
+# Put individual graphs to text
+# Also has a datatype for graphs and various simple operations on this datatype.
+###################################################################################################
+
+
+# a low-level datastructure for the graphs of explainable boosting machines
+@dataclass
+class EBMGraph:
+    feature_name: str
+    feature_type: str
+    x_vals: typing.List[
+        typing.Tuple[float, float]
+    ]  # todo add union with categorical features
+    scores: typing.List[float]
+    stds: typing.List[float]
+
+
+def extract_graph(
+    ebm,
+    feature_index,
+    normalization="none",
+    use_feature_bounds=True,
+):
+    """Extract a graph from an Explainable Boosting Machine.
+
+    This is a low-level function. It does not return the final format in which the graph is presented to the LLM.
+
+    The purpose of this function is to extract the graph from the interals of the EBM and return it in a format that is easy to work with.
+
+    :param ebm:
+    :param feature_index:
+    :param normalization: how to normalize the graph. possible values are: 'mean', 'min', 'none'
+    :param use_feature_bounds: if True, the first and last bin are min and max value of the feature stored in the EBM. If false, the first and last value are -inf and inf, respectively.
+    :return: EBMGraph
+    """
+
+    # read the variables from the ebm
+    feature_name = ebm.feature_names_in_[feature_index]
+    feature_type = ebm.feature_types_in_[feature_index]
+    scores = ebm.term_scores_[feature_index][1:-1]  # Drop missing and unknown bins
+    stds = ebm.standard_deviations_[feature_index][1:-1]
+
+    # normalize the graph
+    normalization_constant = None
+    if normalization == "mean":
+        normalization_constant = np.mean(scores)
+    elif normalization == "min":
+        normalization_constant = np.min(scores)
+    elif normalization == "none":
+        normalization_constant = 0
+    else:
+        raise Exception(f"Unknown normalization {normalization}")
+    scores = scores - normalization_constant
+
+    # read the x-axis bins from the ebm
+    if feature_type == "continuous":
+        x_vals = convert_to_intervals(ebm.bins_[feature_index][0])
+        # feature bounds apply to continuous features only
+        if use_feature_bounds:
+            x_vals[0] = (ebm.feature_bounds_[feature_index][0], x_vals[0][1])
+            x_vals[-1] = (x_vals[-1][0], ebm.feature_bounds_[feature_index][1])
+    elif feature_type == "nominal":
+        x_vals = ebm.bins_[feature_index][
+            0
+        ]  # todo: check this transformation with Paul
+        x_vals = {v - 1: k for k, v in x_vals.items()}
+        x_vals = [x_vals[idx] for idx in range(len(x_vals.keys()))]
+    else:
+        raise Exception(
+            f"Feature {feature_index} is of unknown feature_type {feature_type}."
+        )
+    assert len(x_vals) == len(scores), "The number of bins and scores does not match."
+
+    return EBMGraph(feature_name, feature_type, x_vals, scores, stds)
+
+
+def simplify_graph(graph: EBMGraph, min_variation_per_cent: float = 0.0):
+    """Simplifies a graph. Removes redundant (flat) bins from the graph.
+
+    With min_variation_per_cent>0 (default 0.0), the function simplifies the graph by removing bins
+    that correspond to a less that min_variation_per_cent change in the score, considering the overal min/max difference of score for the feature as 100%.
+    this can be useful to keep a query within the context limit. Empirically, removing changes of less than 2% simplifies graphs a lot
+    in terms of the number of bins/tokens, but visually we can hardly see the difference.
+
+    :param bins:
+    :param scores:
+    :return: EBMGraph. A new simplified graph.
+    """
+    assert graph.feature_type == "continuous", "Can only simplify continuous graphs."
+    x_vals, scores, stds = graph.x_vals, graph.scores, graph.stds
+    total_variation = np.max(scores) - np.min(scores)
+    new_x_vals, new_scores, new_stds = [], [], []
+    for idx, (b0, b1) in enumerate(x_vals):
+        if idx == 0:
+            new_x_vals.append((b0, b1))
+            new_scores.append(scores[idx])
+            new_stds.append(stds[idx])
+        else:
+            score_prev = new_scores[-1]
+            if (
+                np.abs(float(score_prev) - float(scores[idx]))
+                <= total_variation * min_variation_per_cent
+            ):
+                # extend the previous bin to b1
+                new_x_vals[-1] = (new_x_vals[-1][0], b1)
+                # guarantee that the the confidence bands of the simplified graph cover the original graph as well as its confidence bands
+                new_stds[-1] = max(new_stds[-1], stds[idx])
+            else:
+                new_x_vals.append((b0, b1))
+                new_scores.append(scores[idx])
+                new_stds.append(stds[idx])
+    return EBMGraph(
+        graph.feature_name, graph.feature_type, new_x_vals, new_scores, new_stds
+    )
+
+
+def plot_graph(graph: EBMGraph):
+    x_vals, scores, stds = graph.x_vals, graph.scores, graph.stds
+    if graph.feature_type == "continuous":
+        x, y, y_lower, y_upper = [], [], [], []
+        for idx, bin in enumerate(x_vals):
+            if bin[0] == -np.inf or bin[1] == np.inf:
+                continue
+            # left part of the bin
+            x.append(bin[0] + 1e-12)
+            y.append(scores[idx])
+            y_lower.append(scores[idx] - stds[idx])
+            y_upper.append(scores[idx] + stds[idx])
+            # right part of the bin
+            x.append(bin[1])
+            y.append(scores[idx])
+            y_lower.append(scores[idx] - stds[idx])
+            y_upper.append(scores[idx] + stds[idx])
+        # plot
+        fig = plt.figure()
+        plt.plot(x, y)
+        plt.fill_between(x, y_lower, y_upper, alpha=0.2)
+    elif (
+        graph.feature_type == "nominal"
+        or graph.feature_type == "boolean"
+        or graph.feature_type == "categorical"
+    ):
+        # plot bins for the categorical features
+        fig = plt.figure()
+        plt.bar(x_vals, scores, yerr=stds)
+    else:
+        raise Exception(f"Unknown graph feature type {graph.feature_type}.")
+    plt.xlabel(graph.feature_name)
+    plt.title(f"{graph.feature_name} ({graph.feature_type})")
+
+
+def xy_to_json_(x_vals, y_vals):
+    """convert a sequence of x_vals and y_vals to a json string"""
+    # continuous features
+    if isinstance(x_vals[0], tuple):
+        return (
+            "{"
+            + ", ".join([f'"({x[0]}, {x[1]})": {y}' for x, y in zip(x_vals, y_vals)])
+            + "}"
+        )
+    # other features
+    return "{" + ", ".join([f'"{x}": {y}' for x, y in zip(x_vals, y_vals)]) + "}"
+
+
+def graph_to_text(
+    graph: EBMGraph,
+    include_description=True,
+    feature_format=None,
+    x_axis_precision=None,
+    y_axis_precision="auto",
+    confidence_bounds=True,
+    confidence_level=0.95,
+    max_tokens=3000,
+):
+    """Convert a graph to a textual representation that can be passed to a LLM.
+
+    This function takes care of all the different formatting issues that can arise in this process.
+
+    The user can explicitly specify the format of the feature (continuous, cateorical, boolean), as well as the precision of the values on the x-axis and y-axis. If the user does not specify these values, the function will try to infer them from the graph.
+
+    By default, this functions adds a short descriptive text that describes the graph to the LLM.
+
+    This function simplifies the graph so that the textual description length is at most {max_tokens} GPT-4 tokens.
+    """
+
+    # a simple auto-detect for boolean feautres
+    try:
+        if (
+            len(graph.x_vals) == 2
+            and graph.x_vals[0].upper() == "FALSE"
+            and graph.x_vals[1].upper() == "TRUE"
+        ):
+            feature_format = "boolean"
+    except:
+        pass
+
+    # determine the feature format
+    if feature_format is None:
+        feature_format = graph.feature_type
+    if feature_format == "nominal":
+        feature_format = "categorical"
+
+    # the description of the graph depends on the feature format
+    if feature_format == "continuous":
+        description_text = (
+            "This graph represents a continuous-valued feature. The keys are intervals"
+            " that represent ranges where the function predicts the same value.\n\n"
+        )
+    elif feature_format == "categorical":
+        description_text = (
+            "This graph represents categorical feature. Each key represents a possible"
+            " value that the feature can take.\n\n"
+        )
+    elif feature_format == "boolean":
+        description_text = (
+            "This graph represents a boolean feature. The keys are 'True' and 'False',"
+            " the two possible values of the feature.\n\n"
+        )
+    else:
+        raise Exception(f"Unknown feature format {feature_format}")
+
+    # simplify the graph until it fits into the max_tokens limit
+    total_tokens = None
+    min_variation_per_cent = 0.0
+    while True:
+        # simplify the graph
+        simplified_graph = graph
+        if feature_format == "continuous":
+            simplified_graph = simplify_graph(
+                graph, min_variation_per_cent=min_variation_per_cent
+            )
+
+        # confidence bounds via normal approximation
+        scores = simplified_graph.scores
+        if confidence_bounds:
+            factor = scipy.stats.norm.interval(confidence_level, loc=0, scale=1)[1]
+            lower_bounds = [
+                scores[idx] - factor * simplified_graph.stds[idx]
+                for idx in range(len(scores))
+            ]
+            upper_bounds = [
+                scores[idx] + factor * simplified_graph.stds[idx]
+                for idx in range(len(scores))
+            ]
+
+        # adjust the precision on the x-axis. this can be dangerous if we don't know the distribution of the data (it can impact the accuracy).
+        # however, this is a necessary formatting feature because certain (old?) versions of EBMs introduce trailing digits for the xbins (e.g. age as a floating point number with 10 significant digits)
+        x_vals = simplified_graph.x_vals
+        if x_axis_precision is not None:
+            x_vals = [
+                (
+                    np.round(x[0], x_axis_precision).astype(str),
+                    np.round(x[1], x_axis_precision).astype(str),
+                )
+                for x in x_vals
+            ]
+
+        # adjust the precision on the y-axis
+        if y_axis_precision == "auto":  # at least 3 significant digits
+            total_variation = np.max(scores) - np.min(scores)
+            y_fraction = total_variation / 100.0
+            y_axis_precision = 1
+            while y_fraction < 1:
+                y_fraction *= 10
+                y_axis_precision += 1
+        scores = np.round(scores, y_axis_precision).astype(str)
+        if confidence_bounds:
+            lower_bounds = np.round(lower_bounds, y_axis_precision).astype(str)
+            upper_bounds = np.round(upper_bounds, y_axis_precision).astype(str)
+
+        # formatting for boolean features
+        if feature_format == "boolean":
+            assert len(x_vals) == 2, (
+                "Requested a boolean format, but the feature has more than x-axis"
+                f" values: {x_vals}"
+            )
+            # we assume that the left key (the lower numer, typically -1 or 0), is 'False'
+            x_vals = ["False", "True"]
+
+        # create the textual representation of the graph
+        prompt = ""
+        if include_description:
+            prompt += description_text
+        prompt += f"Feature Name: {graph.feature_name}\n"
+        prompt += f"Feature Type: {feature_format}\n"
+        prompt += f"Means: {xy_to_json_(x_vals, scores)}\n"
+        if confidence_bounds:
+            prompt += (
+                f"Lower Bounds ({confidence_level*100:.0f}%-Confidence Interval):"
+                f" {xy_to_json_(x_vals, lower_bounds)}\n"
+            )
+            prompt += (
+                f"Upper Bounds ({confidence_level*100:.0f}%-Confidence Interval):"
+                f" {xy_to_json_(x_vals, upper_bounds)}\n"
+            )
+
+        # count the number of tokens
+        total_tokens = num_tokens_from_string_(prompt, "gpt-4")
+        if feature_format == "continuous":
+            if total_tokens > max_tokens:
+                if min_variation_per_cent > 0.1:
+                    raise Exception(
+                        f"The graph for feature {graph.feature_name} of type"
+                        f" {graph.feature_type} requires {total_tokens} tokens even at"
+                        " a simplification level of 10\%. This graph is too complex to"
+                        " be passed to the LLM within the loken limit of"
+                        f" {max_tokens} tokens."
+                    )
+                min_variation_per_cent += 0.001
+            else:
+                if min_variation_per_cent > 0:
+                    print(
+                        f"INFO: The graph of feature {graph.feature_name} was"
+                        f" simplified by {min_variation_per_cent * 100:.1f}%."
+                    )
+                return prompt
+        else:
+            if total_tokens > max_tokens:
+                raise Exception(
+                    f"The graph for feature {graph.feature_name} of type"
+                    f" {graph.feature_type} requires {total_tokens} tokens and exceeds"
+                    f" the token limit of {max_tokens}."
+                )
+            else:
+                return prompt
+
+
+def parse_str_tuple_to_float_tuple(str_tuple: str):
+    """Parse a string tuple to a float tuple"""
+    return tuple(float(x) for x in str_tuple[1:-1].split(","))
+
+
+def text_to_graph(graph: str):
+    """Convert  the textual representation of a graph back to an EBMGraph."""
+    split_graph = graph.split("\n")
+
+    # find the line that starts with "Feature Name:"
+    start_idx = 0
+    while not split_graph[start_idx].startswith("Feature Name:"):
+        start_idx = start_idx + 1
+
+    feature_name = split_graph[start_idx][13:].strip()
+    feature_type = split_graph[start_idx + 1][13:].strip()
+    assert (
+        feature_type == "continuous"
+    ), "currently only continuous features are supported to convert back to graph"
+
+    # parse json
+    means_json = split_graph[start_idx + 2][6:]
+    means_json = json.loads(means_json)
+
+    lower_bounds_json = split_graph[start_idx + 3]
+    lower_bounds_json = lower_bounds_json[lower_bounds_json.find("):") + 2 :]
+    lower_bounds_json = json.loads(lower_bounds_json)
+
+    upper_bounds_json = split_graph[start_idx + 4]
+    upper_bounds_json = upper_bounds_json[upper_bounds_json.find("):") + 2 :]
+    upper_bounds_json = json.loads(upper_bounds_json)
+
+    # json to EBMGraph format
+    x_vals = [parse_str_tuple_to_float_tuple(k) for k, _ in means_json.items()]
+    scores = [v for _, v in means_json.items()]
+    lower_bounds = [v for _, v in lower_bounds_json.items()]
+    upper_bounds = [v for _, v in upper_bounds_json.items()]
+
+    # heuristically determine the stds from the lower and upper bounds
+    confidence_level = 0.95  # assume 95% confidence interval TODO: infer from the text
+    factor = scipy.stats.norm.interval(confidence_level, loc=0, scale=1)[1]
+    stds = [(u - l) / 2 / factor for u, l in zip(upper_bounds, lower_bounds)]
+
+    return EBMGraph(feature_name, feature_type, x_vals, scores, stds)
```

### Comparing `t2ebm-0.0.1/t2ebm/utils.py` & `t2ebm-0.1.0/t2ebm/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,84 @@
-from tenacity import (
-    retry,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random_exponential,
-)
-
-import openai
-import tiktoken
-
-################################################################################################################
-#                                           Misc. helper functions
-################################################################################################################
-
-
-def num_tokens_from_string_(string: str, model_name: str) -> int:
-    """Returns the number of tokens in a text string."""
-    encoding = tiktoken.encoding_for_model(model_name)
-    num_tokens = len(encoding.encode(string))
-    return num_tokens
-
-
-@retry(
-    retry=retry_if_not_exception_type(openai.error.InvalidRequestError),
-    wait=wait_random_exponential(min=1, max=60),
-    stop=stop_after_attempt(10),
-)
-def openai_completion_query(model, messages, **kwargs):
-    """Catches exceptions and retries, good for deployment / running experiments"""
-    response = openai.ChatCompletion.create(model=model, messages=messages, **kwargs)
-    return response["choices"][0]["message"]["content"]
-
-
-def openai_debug_completion_query(model, messages, **kwargs):
-    """Does not catch exceptions, better for debugging"""
-    response = openai.ChatCompletion.create(model=model, messages=messages, **kwargs)
-    return response["choices"][0]["message"]["content"]
-
-
-def parse_guidance_query(query):
-    """This is a utility function that parses a guidance query string into a list of messages for the openai api.
-
-    It only works with the most simple types of queries.
-    """
-    messages = []
-    start_tokens = ["{{#system~}}", "{{#assistant~}}", "{{#user~}}"]
-    # find first occurence of any start toke in the query
-    position = -1
-    next_token = None
-    for token in start_tokens:
-        next_position = query.find(token)
-        if next_position != -1 and (position == -1 or next_position < position):
-            position = next_position
-            next_token = token
-    if next_token == start_tokens[0]:  # system
-        end_pos = query.find("{{~/system}}")
-        messages.append(
-            {
-                "role": "system",
-                "content": query[position + len(start_tokens[0]) : end_pos].strip(),
-            }
-        )
-    if next_token == start_tokens[1]:  # assistant
-        end_pos = query.find("{{~/assistant}}")
-        messages.append(
-            {
-                "role": "assistant",
-                "content": query[position + len(start_tokens[1]) : end_pos].strip(),
-            }
-        )
-    if next_token == start_tokens[2]:  # user
-        end_pos = query.find("{{~/user}}")
-        messages.append(
-            {
-                "role": "user",
-                "content": query[position + len(start_tokens[2]) : end_pos].strip(),
-            }
-        )
-    if next_token is not None and len(query[end_pos:]) > 15:
-        messages.extend(parse_guidance_query(query[end_pos:]))
-    return messages
+"""
+Misc. helper functions
+"""
+
+from tenacity import (
+    retry,
+    retry_if_not_exception_type,
+    stop_after_attempt,
+    wait_random_exponential,
+)
+
+import openai
+from openai import OpenAI
+
+client = OpenAI()
+import tiktoken
+
+
+def num_tokens_from_string_(string: str, model_name: str) -> int:
+    """Returns the number of tokens in a text string."""
+    encoding = tiktoken.encoding_for_model(model_name)
+    num_tokens = len(encoding.encode(string))
+    return num_tokens
+
+
+# @retry(
+#    retry=retry_if_not_exception_type(openai.InvalidRequestError),
+#    wait=wait_random_exponential(min=1, max=60),
+#    stop=stop_after_attempt(10),
+# )
+def openai_completion_query(model, messages, **kwargs):
+    """Catches exceptions and retries, good for deployment / running experiments"""
+    response = client.chat.completions.create(model=model, messages=messages, **kwargs)
+    return response.choices[0].message.content
+
+
+def openai_debug_completion_query(model, messages, **kwargs):
+    """Does not catch exceptions, better for debugging"""
+    response = client.chat.completions.create(model=model, messages=messages, **kwargs)
+    return response.choices[0].message.content
+
+
+def parse_guidance_query(query):
+    """This is a utility function that parses a guidance query string into a list of messages for the openai api.
+
+    It only works with the most simple types of queries.
+    """
+    messages = []
+    start_tokens = ["{{#system~}}", "{{#assistant~}}", "{{#user~}}"]
+    # find first occurence of any start toke in the query
+    position = -1
+    next_token = None
+    for token in start_tokens:
+        next_position = query.find(token)
+        if next_position != -1 and (position == -1 or next_position < position):
+            position = next_position
+            next_token = token
+    if next_token == start_tokens[0]:  # system
+        end_pos = query.find("{{~/system}}")
+        messages.append(
+            {
+                "role": "system",
+                "content": query[position + len(start_tokens[0]) : end_pos].strip(),
+            }
+        )
+    if next_token == start_tokens[1]:  # assistant
+        end_pos = query.find("{{~/assistant}}")
+        messages.append(
+            {
+                "role": "assistant",
+                "content": query[position + len(start_tokens[1]) : end_pos].strip(),
+            }
+        )
+    if next_token == start_tokens[2]:  # user
+        end_pos = query.find("{{~/user}}")
+        messages.append(
+            {
+                "role": "user",
+                "content": query[position + len(start_tokens[2]) : end_pos].strip(),
+            }
+        )
+    if next_token is not None and len(query[end_pos:]) > 15:
+        messages.extend(parse_guidance_query(query[end_pos:]))
+    return messages
```

