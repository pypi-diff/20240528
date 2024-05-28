# Comparing `tmp/PymoNNto-3.0.2.tar.gz` & `tmp/PymoNNto-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PymoNNto-3.0.2.tar", last modified: Thu Jan 18 13:14:45 2024, max compression
+gzip compressed data, was "PymoNNto-3.0.3.tar", last modified: Tue May 28 08:40:19 2024, max compression
```

## Comparing `PymoNNto-3.0.2.tar` & `PymoNNto-3.0.3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:45.102507 PymoNNto-3.0.2/
--rw-rw-rw-   0        0        0     1073 2020-12-02 18:45:09.000000 PymoNNto-3.0.2/LICENSE
--rw-rw-rw-   0        0        0      678 2024-01-18 13:14:45.101487 PymoNNto-3.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.239560 PymoNNto-3.0.2/PymoNNto/
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.295972 PymoNNto-3.0.2/PymoNNto/Exploration/
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.321174 PymoNNto-3.0.2/PymoNNto/Exploration/AnalysisModules/
--rw-rw-rw-   0        0        0      548 2023-02-24 14:24:06.000000 PymoNNto-3.0.2/PymoNNto/Exploration/AnalysisModules/Static_Classification.py
--rw-rw-rw-   0        0        0     3571 2023-03-09 20:27:54.000000 PymoNNto-3.0.2/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Base.py
--rw-rw-rw-   0        0        0      289 2023-02-24 14:24:06.000000 PymoNNto-3.0.2/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Post.py
--rw-rw-rw-   0        0        0      288 2023-02-24 14:24:06.000000 PymoNNto-3.0.2/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Pre.py
--rw-rw-rw-   0        0        0      221 2022-07-29 10:15:40.000000 PymoNNto-3.0.2/PymoNNto/Exploration/AnalysisModules/__init__.py
--rw-rw-rw-   0        0        0    10819 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Behaviour_UI.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.440983 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/
--rw-rw-rw-   0        0        0     5032 2023-02-15 19:37:04.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Breed_And_Selection_Module.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.470423 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/
--rw-rw-rw-   0        0        0     2471 2023-03-07 13:25:34.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/Evolution_Device.py
--rw-rw-rw-   0        0        0     2205 2022-09-21 18:37:13.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Multi_Thread.py
--rw-rw-rw-   0        0        0     2514 2022-12-08 02:47:35.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_SSH.py
--rw-rw-rw-   0        0        0      796 2022-09-21 17:40:35.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Single_Thread.py
--rw-rw-rw-   0        0        0        0 2021-04-24 18:29:07.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/__init__.py
--rw-rw-rw-   0        0        0    11655 2023-01-15 20:43:33.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Evolution.py
--rw-rw-rw-   0        0        0     9323 2022-09-22 13:04:38.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/EvolutionPlots.py
--rw-rw-rw-   0        0        0     1498 2022-09-22 17:48:30.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Evolution_Individual.py
--rw-rw-rw-   0        0        0    21064 2023-03-08 16:39:15.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Evolution_UI.py
--rw-rw-rw-   0        0        0     8026 2023-03-07 13:25:34.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Interface_Functions.py
--rw-rw-rw-   0        0        0    15128 2023-02-26 19:43:49.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/PlotQTObjects.py
--rw-rw-rw-   0        0        0     9012 2023-03-08 16:36:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/SSH_Functions.py
--rw-rw-rw-   0        0        0     1974 2023-01-15 20:43:33.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Single_Evolution_UI.py
--rw-rw-rw-   0        0        0     1237 2023-02-26 19:16:16.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/TxtHighlighter.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/__init__.py
--rw-rw-rw-   0        0        0    23680 2023-03-10 16:51:47.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/common_UI.py
--rw-rw-rw-   0        0        0     2156 2022-09-22 21:32:55.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/communication.py
--rw-rw-rw-   0        0        0      748 2022-09-22 20:08:23.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/example_master.py
--rw-rw-rw-   0        0        0      281 2022-09-22 20:20:34.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/example_slave.py
--rw-rw-rw-   0        0        0      906 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/example_slave_2.py
--rw-rw-rw-   0        0        0      970 2022-09-22 21:43:43.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/genome_exchange_com.py
--rw-rw-rw-   0        0        0     7250 2023-03-11 23:57:28.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Execute_UI.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.507845 PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/
--rw-rw-rw-   0        0        0     3671 2023-03-12 21:59:55.000000 PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/IteratorFunctions.py
--rw-rw-rw-   0        0        0     2550 2023-02-24 14:22:23.000000 PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/Reconstruction.py
--rw-rw-rw-   0        0        0     4163 2023-03-09 17:40:13.000000 PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/Save_Load.py
--rw-rw-rw-   0        0        0     5061 2023-04-27 08:20:12.000000 PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/Synapses_And_Weights.py
--rw-rw-rw-   0        0        0      428 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/Testing.py
--rw-rw-rw-   0        0        0      198 2021-10-07 21:32:07.000000 PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.532930 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.577457 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.591289 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/
--rw-rw-rw-   0        0        0     1990 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WP_testing.py
--rw-rw-rw-   0        0        0     8743 2022-04-26 14:19:19.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WiltingPriesemann.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/__init__.py
--rw-rw-rw-   0        0        0      795 2022-07-31 17:28:29.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/__init__.py
--rw-rw-rw-   0        0        0     2245 2023-04-27 08:23:13.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/afferent_syn_attr_plot_tab.py
--rw-rw-rw-   0        0        0     2192 2021-03-02 21:33:38.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/buffer_tab.py
--rw-rw-rw-   0        0        0     9817 2023-02-24 14:03:22.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/criticality_tab.py
--rw-rw-rw-   0        0        0     1533 2023-03-09 00:40:54.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/scatter_tab.py
--rw-rw-rw-   0        0        0     3675 2022-10-31 19:59:10.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/similarity_matrix_tab.py
--rw-rw-rw-   0        0        0     7537 2023-04-27 08:19:21.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/stdp_buffer_tab.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.751361 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/
--rw-rw-rw-   0        0        0     3093 2022-09-05 20:47:16.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/Analysis_Module_tab.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.774165 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/
--rw-rw-rw-   0        0        0      777 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/PCA.py
--rw-rw-rw-   0        0        0        0 2022-07-29 09:15:28.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/__init__.py
--rw-rw-rw-   0        0        0     7050 2023-01-14 13:41:06.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/syntax.py
--rw-rw-rw-   0        0        0     2507 2023-03-01 10:32:49.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/PCA_tab.py
--rw-rw-rw-   0        0        0     3426 2023-03-08 20:40:16.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-02-20 19:37:56.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/classifier_bar_tab.py
--rw-rw-rw-   0        0        0     6977 2023-04-27 08:20:12.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/code_execution_tab.py
--rw-rw-rw-   0        0        0     2201 2022-09-05 20:47:16.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/event_tab.py
--rw-rw-rw-   0        0        0     5013 2023-02-24 14:07:48.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/fourier_tab.py
--rw-rw-rw-   0        0        0     4807 2023-04-27 08:25:37.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/hist_tab.py
--rw-rw-rw-   0        0        0     4329 2023-04-27 08:23:13.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/individual_weight_tab.py
--rw-rw-rw-   0        0        0     5844 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/info_tabs.py
--rw-rw-rw-   0        0        0     5731 2023-02-24 14:07:49.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/isi_tab.py
--rw-rw-rw-   0        0        0     5901 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/module_visualizer_tab.py
--rw-rw-rw-   0        0        0     5995 2023-03-09 13:04:34.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/multi_group_plot_tab.py
--rw-rw-rw-   0        0        0     4728 2023-04-27 08:25:37.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/partition_tab.py
--rw-rw-rw-   0        0        0     5531 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_fast_forward_module.py
--rw-rw-rw-   0        0        0     1175 2023-03-22 16:39:47.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_module_quick_access.py
--rw-rw-rw-   0        0        0    14977 2023-03-09 13:18:07.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_network_selector.py
--rw-rw-rw-   0        0        0     6429 2023-03-09 00:06:00.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_neuron_grid.py
--rw-rw-rw-   0        0        0     2219 2023-03-09 23:11:53.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_save_load_module.py
--rw-rw-rw-   0        0        0     4715 2023-03-07 17:46:14.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/single_group_plot_tab.py
--rw-rw-rw-   0        0        0     1728 2023-03-09 01:03:08.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/spiketrain_tab.py
--rw-rw-rw-   0        0        0     2479 2023-03-09 00:40:54.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/stability_tab.py
--rw-rw-rw-   0        0        0     3962 2023-07-23 15:55:59.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab.py
--rw-rw-rw-   0        0        0     4559 2023-04-27 08:25:37.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab_old.py
--rw-rw-rw-   0        0        0    11308 2023-04-27 08:19:21.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Network_UI.py
--rw-rw-rw-   0        0        0     2376 2022-07-29 08:17:09.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Neuron_Classification_Colorizer.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.836125 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/
--rw-rw-rw-   0        0        0     1020 2021-06-10 09:16:56.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/__init__.py
--rw-rw-rw-   0        0        0     5668 2021-11-01 17:39:29.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/chain_tab.py
--rw-rw-rw-   0        0        0     3296 2023-02-24 14:50:37.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/character_activation_tab.py
--rw-rw-rw-   0        0        0     9285 2023-02-24 14:22:23.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/reconstruction_tab.py
--rw-rw-rw-   0        0        0     1949 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_drumbeat_module.py
--rw-rw-rw-   0        0        0    14649 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_grammar_module.py
--rw-rw-rw-   0        0        0     3952 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_image_module.py
--rw-rw-rw-   0        0        0     3360 2023-03-22 16:39:46.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_music_module.py
--rw-rw-rw-   0        0        0    24060 2023-04-27 08:16:20.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sun_gravity_plot_tab.py
--rw-rw-rw-   0        0        0      791 2023-02-24 14:36:01.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/TabBase.py
--rw-rw-rw-   0        0        0      116 2021-03-02 21:33:38.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/__init__.py
--rw-rw-rw-   0        0        0     4861 2023-01-15 20:43:33.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Overview_UI.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.866320 PymoNNto-3.0.2/PymoNNto/Exploration/StorageManager/
--rw-rw-rw-   0        0        0     4333 2023-03-29 10:48:53.000000 PymoNNto-3.0.2/PymoNNto/Exploration/StorageManager/SM2.py
--rw-rw-rw-   0        0        0    18314 2023-03-29 10:48:17.000000 PymoNNto-3.0.2/PymoNNto/Exploration/StorageManager/StorageManager.py
--rw-rw-rw-   0        0        0     2665 2021-05-17 22:04:21.000000 PymoNNto-3.0.2/PymoNNto/Exploration/StorageManager/Storage_Manager_Dir_Select_Dialog.py
--rw-rw-rw-   0        0        0      506 2021-06-24 17:39:58.000000 PymoNNto-3.0.2/PymoNNto/Exploration/StorageManager/User_Input_SM_Writer.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/StorageManager/__init__.py
--rw-rw-rw-   0        0        0    27589 2023-03-09 11:16:10.000000 PymoNNto-3.0.2/PymoNNto/Exploration/UI_Base.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.912950 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/
--rw-rw-rw-   0        0        0     1329 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Analysis_Plots.py
--rw-rw-rw-   0        0        0    28252 2023-04-27 08:28:05.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Module_visualizer.py
--rw-rw-rw-   0        0        0    14565 2023-03-22 16:39:47.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Pyplot_visualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.939058 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/
--rw-rw-rw-   0        0        0     2228 2023-02-24 13:11:58.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_Synapse_Transition_scatter.py
--rw-rw-rw-   0        0        0     2451 2021-03-02 21:33:38.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_weights.py
--rw-rw-rw-   0        0        0    27400 2023-05-04 13:11:42.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Reconstruct_Analyze_Label.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/__init__.py
--rw-rw-rw-   0        0        0    38124 2021-05-17 22:04:21.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/SORN_visualization.py
--rw-rw-rw-   0        0        0    12752 2023-04-27 08:22:49.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Visualization_Helper.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/__init__.py
--rw-rw-rw-   0        0        0     1916 2023-02-24 14:22:23.000000 PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/read_write_np_experiment.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/Exploration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.940058 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.981553 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/
--rw-rw-rw-   0        0        0     4658 2023-03-22 16:38:01.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/BasicHomeostasis.py
--rw-rw-rw-   0        0        0      838 2023-08-09 22:38:11.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Behavior_Weight_Initialization.py
--rw-rw-rw-   0        0        0     2229 2023-05-04 13:41:26.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Normalization.py
--rw-rw-rw-   0        0        0      901 2023-05-04 13:41:26.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Normalization_Sparse.py
--rw-rw-rw-   0        0        0     1411 2023-05-04 13:41:26.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Normalization_Tensorflow.py
--rw-rw-rw-   0        0        0     1221 2023-08-09 23:18:12.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Nox_diffusion.py
--rw-rw-rw-   0        0        0      523 2023-08-09 23:18:12.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Refractory.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:45.013523 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/
--rw-rw-rw-   0        0        0     1334 2023-03-22 16:38:59.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/Equation.py
--rw-rw-rw-   0        0        0      874 2023-03-22 16:38:00.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/EulerClock.py
--rw-rw-rw-   0        0        0     1084 2020-11-11 00:49:45.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/Helper.py
--rw-rw-rw-   0        0        0     1665 2023-03-22 16:39:00.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/VariableInitializer.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:45.021593 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Recorder/
--rw-rw-rw-   0        0        0     5905 2023-07-20 01:29:36.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Recorder/Recorder.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Recorder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:45.042486 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Structure/
--rw-rw-rw-   0        0        0     2793 2023-03-22 16:38:01.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Structure/Partition.py
--rw-rw-rw-   0        0        0     3751 2023-03-22 16:39:00.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Structure/Receptive_Fields.py
--rw-rw-rw-   0        0        0     6616 2023-03-22 16:38:01.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Structure/Structure.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Structure/__init__.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/NetworkBehavior/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:45.091569 PymoNNto-3.0.2/PymoNNto/NetworkCore/
--rw-rw-rw-   0        0        0     5305 2023-03-25 09:00:49.000000 PymoNNto-3.0.2/PymoNNto/NetworkCore/Analysis_Module.py
--rw-rw-rw-   0        0        0     9709 2023-07-31 15:54:21.000000 PymoNNto-3.0.2/PymoNNto/NetworkCore/Base_Attachable_Modules.py
--rw-rw-rw-   0        0        0     2392 2023-03-25 08:56:09.000000 PymoNNto-3.0.2/PymoNNto/NetworkCore/Base_Tagable_Object.py
--rw-rw-rw-   0        0        0     6863 2023-08-14 09:15:33.000000 PymoNNto-3.0.2/PymoNNto/NetworkCore/Behavior.py
--rw-rw-rw-   0        0        0    12586 2023-08-01 10:56:33.000000 PymoNNto-3.0.2/PymoNNto/NetworkCore/Network.py
--rw-rw-rw-   0        0        0    10839 2023-05-04 09:09:31.000000 PymoNNto-3.0.2/PymoNNto/NetworkCore/Neuron_Group.py
--rw-rw-rw-   0        0        0     6843 2023-05-04 08:17:05.000000 PymoNNto-3.0.2/PymoNNto/NetworkCore/Synapse_Group.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.2/PymoNNto/NetworkCore/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:45.099955 PymoNNto-3.0.2/PymoNNto/UI/
--rw-rw-rw-   0        0        0      448 2023-03-22 16:38:59.000000 PymoNNto-3.0.2/PymoNNto/UI/CLI.py
--rw-rw-rw-   0        0        0        2 2023-01-15 20:43:33.000000 PymoNNto-3.0.2/PymoNNto/UI/__init__.py
--rw-rw-rw-   0        0        0      836 2023-03-22 16:39:00.000000 PymoNNto-3.0.2/PymoNNto/__init__.py
--rw-rw-rw-   0        0        0     9015 2023-05-04 13:35:29.000000 PymoNNto-3.0.2/PymoNNto/test_pymoNNto.py
-drwxrwxrwx   0        0        0        0 2024-01-18 13:14:44.263941 PymoNNto-3.0.2/PymoNNto.egg-info/
--rw-rw-rw-   0        0        0      678 2024-01-18 13:14:44.000000 PymoNNto-3.0.2/PymoNNto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7890 2024-01-18 13:14:44.000000 PymoNNto-3.0.2/PymoNNto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-18 13:14:44.000000 PymoNNto-3.0.2/PymoNNto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      190 2024-01-18 13:14:44.000000 PymoNNto-3.0.2/PymoNNto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       87 2024-01-18 13:14:44.000000 PymoNNto-3.0.2/PymoNNto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-18 13:14:44.000000 PymoNNto-3.0.2/PymoNNto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2021-03-04 15:34:19.000000 PymoNNto-3.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-01-18 13:14:45.102507 PymoNNto-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1110 2024-01-18 13:14:16.000000 PymoNNto-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.811823 PymoNNto-3.0.3/
+-rw-rw-rw-   0        0        0     1073 2020-12-02 18:45:09.000000 PymoNNto-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0      678 2024-05-28 08:40:19.810802 PymoNNto-3.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:18.843158 PymoNNto-3.0.3/PymoNNto/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:18.911252 PymoNNto-3.0.3/PymoNNto/Exploration/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:18.945882 PymoNNto-3.0.3/PymoNNto/Exploration/AnalysisModules/
+-rw-rw-rw-   0        0        0      548 2023-02-24 14:24:06.000000 PymoNNto-3.0.3/PymoNNto/Exploration/AnalysisModules/Static_Classification.py
+-rw-rw-rw-   0        0        0     3571 2024-04-26 11:35:50.000000 PymoNNto-3.0.3/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Base.py
+-rw-rw-rw-   0        0        0      289 2023-02-24 14:24:06.000000 PymoNNto-3.0.3/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Post.py
+-rw-rw-rw-   0        0        0      288 2023-02-24 14:24:06.000000 PymoNNto-3.0.3/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Pre.py
+-rw-rw-rw-   0        0        0      221 2022-07-29 10:15:40.000000 PymoNNto-3.0.3/PymoNNto/Exploration/AnalysisModules/__init__.py
+-rw-rw-rw-   0        0        0    10819 2023-03-22 16:39:46.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Behavior_UI.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.078038 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/
+-rw-rw-rw-   0        0        0     5032 2023-02-15 19:37:04.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Breed_And_Selection_Module.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.110553 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/
+-rw-rw-rw-   0        0        0     2471 2023-03-07 13:25:34.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/Evolution_Device.py
+-rw-rw-rw-   0        0        0     2205 2022-09-21 18:37:13.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Multi_Thread.py
+-rw-rw-rw-   0        0        0     2514 2022-12-08 02:47:35.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_SSH.py
+-rw-rw-rw-   0        0        0      796 2022-09-21 17:40:35.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Single_Thread.py
+-rw-rw-rw-   0        0        0        0 2021-04-24 18:29:07.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/__init__.py
+-rw-rw-rw-   0        0        0    11655 2023-01-15 20:43:33.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Evolution.py
+-rw-rw-rw-   0        0        0     9323 2022-09-22 13:04:38.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/EvolutionPlots.py
+-rw-rw-rw-   0        0        0     1498 2022-09-22 17:48:30.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Evolution_Individual.py
+-rw-rw-rw-   0        0        0    21064 2023-03-08 16:39:15.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Evolution_UI.py
+-rw-rw-rw-   0        0        0     8026 2023-03-07 13:25:34.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Interface_Functions.py
+-rw-rw-rw-   0        0        0    15128 2023-02-26 19:43:49.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/PlotQTObjects.py
+-rw-rw-rw-   0        0        0     9012 2023-03-08 16:36:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/SSH_Functions.py
+-rw-rw-rw-   0        0        0     1974 2023-01-15 20:43:33.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Single_Evolution_UI.py
+-rw-rw-rw-   0        0        0     1237 2023-02-26 19:16:16.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/TxtHighlighter.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/__init__.py
+-rw-rw-rw-   0        0        0    23680 2023-03-10 16:51:47.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/common_UI.py
+-rw-rw-rw-   0        0        0     2156 2022-09-22 21:32:55.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/communication.py
+-rw-rw-rw-   0        0        0      748 2022-09-22 20:08:23.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/example_master.py
+-rw-rw-rw-   0        0        0      281 2022-09-22 20:20:34.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/example_slave.py
+-rw-rw-rw-   0        0        0      906 2023-03-22 16:39:46.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/example_slave_2.py
+-rw-rw-rw-   0        0        0      970 2022-09-22 21:43:43.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/genome_exchange_com.py
+-rw-rw-rw-   0        0        0     7250 2023-03-11 23:57:28.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Execute_UI.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.152258 PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/
+-rw-rw-rw-   0        0        0     3671 2023-03-12 21:59:55.000000 PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/IteratorFunctions.py
+-rw-rw-rw-   0        0        0     2550 2023-02-24 14:22:23.000000 PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/Reconstruction.py
+-rw-rw-rw-   0        0        0     4163 2023-03-09 17:40:13.000000 PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/Save_Load.py
+-rw-rw-rw-   0        0        0     5061 2023-04-27 08:20:12.000000 PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/Synapses_And_Weights.py
+-rw-rw-rw-   0        0        0      428 2023-03-22 16:39:46.000000 PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/Testing.py
+-rw-rw-rw-   0        0        0      198 2021-10-07 21:32:07.000000 PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.177970 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.227095 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.244061 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/
+-rw-rw-rw-   0        0        0     1990 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WP_testing.py
+-rw-rw-rw-   0        0        0     8743 2022-04-26 14:19:19.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WiltingPriesemann.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/__init__.py
+-rw-rw-rw-   0        0        0      795 2022-07-31 17:28:29.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/__init__.py
+-rw-rw-rw-   0        0        0     2245 2023-04-27 08:23:13.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/afferent_syn_attr_plot_tab.py
+-rw-rw-rw-   0        0        0     2192 2021-03-02 21:33:38.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/buffer_tab.py
+-rw-rw-rw-   0        0        0     9817 2023-02-24 14:03:22.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/criticality_tab.py
+-rw-rw-rw-   0        0        0     1533 2023-03-09 00:40:54.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/scatter_tab.py
+-rw-rw-rw-   0        0        0     3675 2022-10-31 19:59:10.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/similarity_matrix_tab.py
+-rw-rw-rw-   0        0        0     7537 2023-04-27 08:19:21.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/stdp_buffer_tab.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.422160 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/
+-rw-rw-rw-   0        0        0     3093 2022-09-05 20:47:16.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/Analysis_Module_tab.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.437760 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/
+-rw-rw-rw-   0        0        0      777 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/PCA.py
+-rw-rw-rw-   0        0        0        0 2022-07-29 09:15:28.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/__init__.py
+-rw-rw-rw-   0        0        0     7050 2023-01-14 13:41:06.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/syntax.py
+-rw-rw-rw-   0        0        0     2507 2023-03-01 10:32:49.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/PCA_tab.py
+-rw-rw-rw-   0        0        0     3426 2023-03-08 20:40:16.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-02-20 19:37:56.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/classifier_bar_tab.py
+-rw-rw-rw-   0        0        0     6977 2023-04-27 08:20:12.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/code_execution_tab.py
+-rw-rw-rw-   0        0        0     2201 2022-09-05 20:47:16.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/event_tab.py
+-rw-rw-rw-   0        0        0     5013 2023-02-24 14:07:48.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/fourier_tab.py
+-rw-rw-rw-   0        0        0     4807 2023-04-27 08:25:37.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/hist_tab.py
+-rw-rw-rw-   0        0        0     4329 2023-04-27 08:23:13.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/individual_weight_tab.py
+-rw-rw-rw-   0        0        0     5844 2023-03-22 16:39:46.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/info_tabs.py
+-rw-rw-rw-   0        0        0     5731 2023-02-24 14:07:49.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/isi_tab.py
+-rw-rw-rw-   0        0        0     5901 2023-03-22 16:39:46.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/module_visualizer_tab.py
+-rw-rw-rw-   0        0        0     5995 2023-03-09 13:04:34.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/multi_group_plot_tab.py
+-rw-rw-rw-   0        0        0     4728 2023-04-27 08:25:37.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/partition_tab.py
+-rw-rw-rw-   0        0        0     5531 2023-03-22 16:39:46.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_fast_forward_module.py
+-rw-rw-rw-   0        0        0     1175 2023-03-22 16:39:47.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_module_quick_access.py
+-rw-rw-rw-   0        0        0    14977 2023-03-09 13:18:07.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_network_selector.py
+-rw-rw-rw-   0        0        0     6429 2023-03-09 00:06:00.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_neuron_grid.py
+-rw-rw-rw-   0        0        0     2219 2023-03-09 23:11:53.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_save_load_module.py
+-rw-rw-rw-   0        0        0     4715 2023-03-07 17:46:14.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/single_group_plot_tab.py
+-rw-rw-rw-   0        0        0     1728 2023-03-09 01:03:08.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/spiketrain_tab.py
+-rw-rw-rw-   0        0        0     2479 2023-03-09 00:40:54.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/stability_tab.py
+-rw-rw-rw-   0        0        0     3962 2023-07-23 15:55:59.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab.py
+-rw-rw-rw-   0        0        0     4559 2023-04-27 08:25:37.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab_old.py
+-rw-rw-rw-   0        0        0    11308 2023-04-27 08:19:21.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Network_UI.py
+-rw-rw-rw-   0        0        0     2376 2022-07-29 08:17:09.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Neuron_Classification_Colorizer.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.504257 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/
+-rw-rw-rw-   0        0        0     1020 2021-06-10 09:16:56.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/__init__.py
+-rw-rw-rw-   0        0        0     5668 2021-11-01 17:39:29.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/chain_tab.py
+-rw-rw-rw-   0        0        0     3296 2023-02-24 14:50:37.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/character_activation_tab.py
+-rw-rw-rw-   0        0        0     9334 2024-05-07 13:39:15.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/reconstruction_tab.py
+-rw-rw-rw-   0        0        0     1949 2023-03-22 16:39:46.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_drumbeat_module.py
+-rw-rw-rw-   0        0        0    14835 2024-05-07 14:25:50.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_grammar_module.py
+-rw-rw-rw-   0        0        0     3952 2023-03-22 16:39:46.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_image_module.py
+-rw-rw-rw-   0        0        0     3360 2023-03-22 16:39:46.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_music_module.py
+-rw-rw-rw-   0        0        0    24059 2024-05-07 14:30:43.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sun_gravity_plot_tab.py
+-rw-rw-rw-   0        0        0      791 2023-02-24 14:36:01.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/TabBase.py
+-rw-rw-rw-   0        0        0      116 2021-03-02 21:33:38.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/__init__.py
+-rw-rw-rw-   0        0        0     4861 2023-01-15 20:43:33.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Overview_UI.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.539225 PymoNNto-3.0.3/PymoNNto/Exploration/StorageManager/
+-rw-rw-rw-   0        0        0     4333 2023-03-29 10:48:53.000000 PymoNNto-3.0.3/PymoNNto/Exploration/StorageManager/SM2.py
+-rw-rw-rw-   0        0        0    18327 2024-01-31 15:01:57.000000 PymoNNto-3.0.3/PymoNNto/Exploration/StorageManager/StorageManager.py
+-rw-rw-rw-   0        0        0     2665 2021-05-17 22:04:21.000000 PymoNNto-3.0.3/PymoNNto/Exploration/StorageManager/Storage_Manager_Dir_Select_Dialog.py
+-rw-rw-rw-   0        0        0      506 2021-06-24 17:39:58.000000 PymoNNto-3.0.3/PymoNNto/Exploration/StorageManager/User_Input_SM_Writer.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/StorageManager/__init__.py
+-rw-rw-rw-   0        0        0    27589 2023-03-09 11:16:10.000000 PymoNNto-3.0.3/PymoNNto/Exploration/UI_Base.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.590772 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/
+-rw-rw-rw-   0        0        0     1329 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Analysis_Plots.py
+-rw-rw-rw-   0        0        0    28252 2023-04-27 08:28:05.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Module_visualizer.py
+-rw-rw-rw-   0        0        0    14565 2023-03-22 16:39:47.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Pyplot_visualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.614999 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/
+-rw-rw-rw-   0        0        0     2228 2023-02-24 13:11:58.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_Synapse_Transition_scatter.py
+-rw-rw-rw-   0        0        0     2451 2021-03-02 21:33:38.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_weights.py
+-rw-rw-rw-   0        0        0    27400 2023-05-04 13:11:42.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Reconstruct_Analyze_Label.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/__init__.py
+-rw-rw-rw-   0        0        0    38124 2021-05-17 22:04:21.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/SORN_visualization.py
+-rw-rw-rw-   0        0        0    12752 2023-04-27 08:22:49.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Visualization_Helper.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/__init__.py
+-rw-rw-rw-   0        0        0     1916 2023-02-24 14:22:23.000000 PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/read_write_np_experiment.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/Exploration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.618004 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.671008 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/
+-rw-rw-rw-   0        0        0     4658 2023-03-22 16:38:01.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/BasicHomeostasis.py
+-rw-rw-rw-   0        0        0      838 2023-08-09 22:38:11.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Behavior_Weight_Initialization.py
+-rw-rw-rw-   0        0        0     2229 2023-05-04 13:41:26.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Normalization.py
+-rw-rw-rw-   0        0        0      901 2023-05-04 13:41:26.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Normalization_Sparse.py
+-rw-rw-rw-   0        0        0     1411 2023-05-04 13:41:26.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Normalization_Tensorflow.py
+-rw-rw-rw-   0        0        0     1221 2023-08-09 23:18:12.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Nox_diffusion.py
+-rw-rw-rw-   0        0        0      523 2023-08-09 23:18:12.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Refractory.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.706519 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/
+-rw-rw-rw-   0        0        0     1334 2023-03-22 16:38:59.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/Equation.py
+-rw-rw-rw-   0        0        0      874 2023-03-22 16:38:00.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/EulerClock.py
+-rw-rw-rw-   0        0        0     1084 2020-11-11 00:49:45.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/Helper.py
+-rw-rw-rw-   0        0        0     1665 2023-03-22 16:39:00.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/VariableInitializer.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.718521 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Recorder/
+-rw-rw-rw-   0        0        0     5905 2023-07-20 01:29:36.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Recorder/Recorder.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Recorder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.745519 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Structure/
+-rw-rw-rw-   0        0        0     2793 2023-03-22 16:38:01.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Structure/Partition.py
+-rw-rw-rw-   0        0        0     3751 2023-03-22 16:39:00.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Structure/Receptive_Fields.py
+-rw-rw-rw-   0        0        0     6616 2023-03-22 16:38:01.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Structure/Structure.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Structure/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/NetworkBehavior/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.802799 PymoNNto-3.0.3/PymoNNto/NetworkCore/
+-rw-rw-rw-   0        0        0     5305 2023-03-25 09:00:49.000000 PymoNNto-3.0.3/PymoNNto/NetworkCore/Analysis_Module.py
+-rw-rw-rw-   0        0        0     9419 2024-01-19 02:32:57.000000 PymoNNto-3.0.3/PymoNNto/NetworkCore/Base_Attachable_Modules.py
+-rw-rw-rw-   0        0        0     2392 2023-03-25 08:56:09.000000 PymoNNto-3.0.3/PymoNNto/NetworkCore/Base_Tagable_Object.py
+-rw-rw-rw-   0        0        0     6863 2023-08-14 09:15:33.000000 PymoNNto-3.0.3/PymoNNto/NetworkCore/Behavior.py
+-rw-rw-rw-   0        0        0    12780 2024-01-19 02:22:59.000000 PymoNNto-3.0.3/PymoNNto/NetworkCore/Network.py
+-rw-rw-rw-   0        0        0    10839 2023-05-04 09:09:31.000000 PymoNNto-3.0.3/PymoNNto/NetworkCore/Neuron_Group.py
+-rw-rw-rw-   0        0        0     6843 2023-05-04 08:17:05.000000 PymoNNto-3.0.3/PymoNNto/NetworkCore/Synapse_Group.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.3/PymoNNto/NetworkCore/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:19.809801 PymoNNto-3.0.3/PymoNNto/UI/
+-rw-rw-rw-   0        0        0      448 2023-03-22 16:38:59.000000 PymoNNto-3.0.3/PymoNNto/UI/CLI.py
+-rw-rw-rw-   0        0        0        2 2023-01-15 20:43:33.000000 PymoNNto-3.0.3/PymoNNto/UI/__init__.py
+-rw-rw-rw-   0        0        0      836 2023-03-22 16:39:00.000000 PymoNNto-3.0.3/PymoNNto/__init__.py
+-rw-rw-rw-   0        0        0     9015 2023-05-04 13:35:29.000000 PymoNNto-3.0.3/PymoNNto/test_pymoNNto.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:40:18.871698 PymoNNto-3.0.3/PymoNNto.egg-info/
+-rw-rw-rw-   0        0        0      678 2024-05-28 08:40:18.000000 PymoNNto-3.0.3/PymoNNto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7889 2024-05-28 08:40:18.000000 PymoNNto-3.0.3/PymoNNto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:40:18.000000 PymoNNto-3.0.3/PymoNNto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      190 2024-05-28 08:40:18.000000 PymoNNto-3.0.3/PymoNNto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       87 2024-05-28 08:40:18.000000 PymoNNto-3.0.3/PymoNNto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-28 08:40:18.000000 PymoNNto-3.0.3/PymoNNto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2021-03-04 15:34:19.000000 PymoNNto-3.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:40:19.811823 PymoNNto-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2024-05-28 08:39:45.000000 PymoNNto-3.0.3/setup.py
```

### Comparing `PymoNNto-3.0.2/LICENSE` & `PymoNNto-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PKG-INFO` & `PymoNNto-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PymoNNto
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python Modular Neural Network Toolbox
 Home-page: https://github.com/trieschlab/PymoNNto
 Author: Marius Vieth
 Author-email: mv15go@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/AnalysisModules/Static_Classification.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/AnalysisModules/Static_Classification.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Base.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Base.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Behaviour_UI.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Behavior_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Breed_And_Selection_Module.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Breed_And_Selection_Module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/Evolution_Device.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/Evolution_Device.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Multi_Thread.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Multi_Thread.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_SSH.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_SSH.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Single_Thread.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Single_Thread.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Evolution.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Evolution.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/EvolutionPlots.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/EvolutionPlots.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Evolution_Individual.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Evolution_Individual.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Evolution_UI.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Evolution_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Interface_Functions.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Interface_Functions.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/PlotQTObjects.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/PlotQTObjects.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/SSH_Functions.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/SSH_Functions.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/Single_Evolution_UI.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/Single_Evolution_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/TxtHighlighter.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/TxtHighlighter.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/common_UI.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/common_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/communication.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/communication.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/example_master.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/example_master.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/example_slave_2.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/example_slave_2.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Evolution/genome_exchange_com.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Evolution/genome_exchange_com.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Execute_UI.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Execute_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/IteratorFunctions.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/IteratorFunctions.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/Reconstruction.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/Reconstruction.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/Save_Load.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/Save_Load.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/HelperFunctions/Synapses_And_Weights.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/HelperFunctions/Synapses_And_Weights.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WP_testing.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WP_testing.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WiltingPriesemann.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WiltingPriesemann.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/__init__.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/afferent_syn_attr_plot_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/afferent_syn_attr_plot_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/buffer_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/buffer_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/criticality_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/criticality_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/scatter_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/scatter_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/similarity_matrix_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/similarity_matrix_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Advanced_Tabs/stdp_buffer_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Advanced_Tabs/stdp_buffer_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/Analysis_Module_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/Analysis_Module_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/PCA.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/PCA.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/syntax.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/syntax.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/PCA_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/PCA_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/__init__.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/classifier_bar_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/classifier_bar_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/code_execution_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/code_execution_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/event_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/event_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/fourier_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/fourier_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/hist_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/hist_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/individual_weight_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/individual_weight_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/info_tabs.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/info_tabs.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/isi_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/isi_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/module_visualizer_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/module_visualizer_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/multi_group_plot_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/multi_group_plot_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/partition_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/partition_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_fast_forward_module.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_fast_forward_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_module_quick_access.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_module_quick_access.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_network_selector.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_network_selector.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_neuron_grid.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_neuron_grid.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_save_load_module.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_save_load_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/single_group_plot_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/single_group_plot_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/spiketrain_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/spiketrain_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/stability_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/stability_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab_old.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab_old.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Network_UI.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Network_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Neuron_Classification_Colorizer.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Neuron_Classification_Colorizer.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/__init__.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/chain_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/chain_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/character_activation_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/character_activation_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/reconstruction_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/reconstruction_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         super().__init__(title)
         self.recon_groups_tag = recon_groups_tag
 
     def add_recorder_variables(self, neuron_group, Network_UI):
         return
 
     def initialize(self, Network_UI):
-        if Network_UI.network['TextActivator', 0] and Network_UI.network['TextGenerator', 0] is not None:
-            self.reconstruction_tab = Network_UI.add_tab(title=self.title) #Network_UI.Next_Tab(self.title)
+        if Network_UI.network['TextActivator', 0] is not None and Network_UI.network['TextGenerator', 0] is not None:
+            self.recon_tab = Network_UI.add_tab(title=self.title) #Network_UI.Next_Tab(self.title)
 
             self.grid = QGridLayout()
             self.grid.setAlignment(Qt.AlignLeft)
             Network_UI.tab.get_layout().addLayout(self.grid)
             Network_UI.tab.get_layout().setAlignment(Qt.AlignTop)
 
             generator = Network_UI.network['TextGenerator', 0]
@@ -66,15 +66,15 @@
 
 
 
 
 
 
     def update(self, Network_UI):
-        if Network_UI.network['TextActivator', 0] is not None and self.reconstruction_tab.isVisible():
+        if Network_UI.network['TextActivator', 0] is not None and Network_UI.network['TextGenerator', 0] is not None and self.recon_tab.isVisible():
             group=Network_UI.selected_neuron_group()
 
             '''
             RALN = Reconstruct_Analyze_Label_Network(Network_UI.network)
             RALN.zero_recon()
             group.recon[Network_UI.selected_neuron_id()] = 1
             RALN.propagation('W', 10, 'backward', 'forget', 'all', temporal_recon_groups=Network_UI.network['prediction_source'], exponent=4, normalize=True, filter_weakest_percent=40.0)  # forget
```

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_drumbeat_module.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_drumbeat_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_grammar_module.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_grammar_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,24 @@
             self.recon_text_label.setText('')
             self.recon_text_label.setFont(QFont("Courier"))
             self.recon_text_label.setToolTip('simple reconstruction text')
 
     def update(self, Network_UI):
 
         if Network_UI.network['TextGenerator', 0] is not None and Network_UI.network['TextActivator', 0] is not None:
-            if Network_UI.network['TextActivator', 0].behavior_enabled:
-                inp_text = Network_UI.network['TextGenerator', 0].history[-self.text_length:]
+            if Network_UI.network['TextGenerator', 0].behavior_enabled and Network_UI.network['TextActivator', 0].behavior_enabled:
+                inp_text = Network_UI.network['TextGenerator', 0].get_str_history()[-self.text_length:]
             else:
                 inp_text = 'deactivated'
+            inp_text=inp_text.replace('\n', '<break>')
             self.inp_text_label.setText(inp_text)
 
         if Network_UI.network['TextReconstructor', 0] is not None:
             recon_text = Network_UI.network['TextReconstructor', 0].reconstruction_history[-self.text_length:]
+            recon_text=recon_text.replace('\n', '<break>')
             self.recon_text_label.setText(recon_text)
 '''
 
 class sidebar_grammar_module(TabBase):
 
     def __init__(self, next_p=True, simu_p=True, noc_p=True, text_length=35):
         self.next_p=next_p
```

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_image_module.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_image_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_music_module.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_music_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sun_gravity_plot_tab.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sun_gravity_plot_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     def draw_neurons(self, painter, group, neuron_size=1, selected_neurons=None):
 
         color = self.get_neuron_color(group)
 
         painter.setPen(0)
 
-        inactive = group.output <= 0
+        inactive = group.spike <= 0
         active = np.invert(inactive)
 
         for c in unique(color, axis=0):
             mask = np.all(color == c[None,:], axis=1) * inactive #(color == c) np.all(a == b, axis=1)
             painter.setBrush(pg.mkBrush(color=c))
             for x, y in zip(group.buffer_posx[mask], group.buffer_posy[mask]):
                 painter.drawEllipse(QtCore.QPointF(x, y), neuron_size, neuron_size)
```

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Network_UI/TabBase.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Network_UI/TabBase.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Overview_UI.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Overview_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/StorageManager/SM2.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/StorageManager/SM2.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/StorageManager/StorageManager.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/StorageManager/StorageManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,21 +244,20 @@
         return string
 
     def backup_execued_file(self):
         executed_file = sys.argv[0]
         self.backup(executed_file)
 
     def backup(self, file_or_folder):
-        file_or_folder.replace('\\','/')
+        file_or_folder=file_or_folder.replace('\\','/')
         if file_or_folder[-1]=='/':
             file_or_folder=file_or_folder[:-1]
         parts = file_or_folder.split('/')
         shutil.copy(file_or_folder, self.absolute_path+parts[-1])
 
-
     def save_np(self, key, obj):
         np.save(self.absolute_path + key + '.npy', arr=obj)
 
     def save_obj(self, key, obj):
         pickle.dump(obj, open(self.absolute_path + key + '.obj', 'wb'))
 
     def load_obj(self, key):
```

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/StorageManager/Storage_Manager_Dir_Select_Dialog.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/StorageManager/Storage_Manager_Dir_Select_Dialog.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/UI_Base.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/UI_Base.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Analysis_Plots.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Analysis_Plots.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Module_visualizer.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Module_visualizer.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Pyplot_visualizer.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Pyplot_visualizer.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_Synapse_Transition_scatter.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_Synapse_Transition_scatter.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_weights.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_weights.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Reconstruct_Analyze_Label.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Reconstruct_Analyze_Label.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/SORN_visualization.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/SORN_visualization.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/Visualization_Helper.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/Visualization_Helper.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/Exploration/Visualization/read_write_np_experiment.py` & `PymoNNto-3.0.3/PymoNNto/Exploration/Visualization/read_write_np_experiment.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/BasicHomeostasis.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/BasicHomeostasis.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Behavior_Weight_Initialization.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Behavior_Weight_Initialization.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Normalization.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Normalization.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Normalization_Sparse.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Normalization_Sparse.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Normalization_Tensorflow.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Normalization_Tensorflow.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Nox_diffusion.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Nox_diffusion.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Basics/Refractory.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Basics/Refractory.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/Equation.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/Equation.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/EulerClock.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/EulerClock.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/Helper.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/Helper.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/EulerEquationModules/VariableInitializer.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/EulerEquationModules/VariableInitializer.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Recorder/Recorder.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Recorder/Recorder.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Structure/Partition.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Structure/Partition.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Structure/Receptive_Fields.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Structure/Receptive_Fields.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkBehavior/Structure/Structure.py` & `PymoNNto-3.0.3/PymoNNto/NetworkBehavior/Structure/Structure.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkCore/Analysis_Module.py` & `PymoNNto-3.0.3/PymoNNto/NetworkCore/Analysis_Module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkCore/Base_Attachable_Modules.py` & `PymoNNto-3.0.3/PymoNNto/NetworkCore/Base_Attachable_Modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,14 +154,15 @@
             return result, modules
         else:
             return result
 
 
     def _get_mat(self, mode, dim, density=None, scale=None, plot=False):
         if mode not in self._mat_eval_dict:
+            '''
             ev_str = mode
 
             cast = True
 
             if ev_str == bool or ev_str == 'bool':
                 cast = False
                 ev_str = 'zeros(dtype=bool)'
@@ -187,32 +188,19 @@
             ev_str = ev_str.replace(')', ',' + a1 + ')')
             ev_str = ev_str.replace('(,', '(')
 
             if cast:
                 ev_str += '.astype(self.def_dtype)'
 
             self._mat_eval_dict[mode] = compile(ev_str, '<string>', 'eval')
+            '''
+            self._mat_eval_dict[mode] = compile(self.network.backend.evaluate_string(mode), '<string>', 'eval')
 
         result = eval(self._mat_eval_dict[mode])
-
-        if density is not None:
-            if type(density) == int or type(density) == float:
-                result = (result * (random_sample(dim) <= density))
-            elif type(density) is np.ndarray:
-                result = (result * (random_sample(dim) <= density[:, None]))
-
-        if scale is not None:
-            result *= scale
-
-        if plot:
-            import matplotlib.pyplot as plt
-            plt.hist(result.flatten(), bins=50)
-            plt.show()
-
-        return result
+        return self.network.backend.modulate(result, dim, density, scale, plot)
 
     def get_nparray(self, dim):
         return np.zeros(dim).astype(self.def_dtype)
 
     def get_buffer_mat(self, dim, size):
         return np.array([self.get_nparray(dim) for _ in range(size)])
```

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkCore/Base_Tagable_Object.py` & `PymoNNto-3.0.3/PymoNNto/NetworkCore/Base_Tagable_Object.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkCore/Behavior.py` & `PymoNNto-3.0.3/PymoNNto/NetworkCore/Behavior.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkCore/Network.py` & `PymoNNto-3.0.3/PymoNNto/NetworkCore/Network.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 from PymoNNto.NetworkCore.Base_Attachable_Modules import *
 from PymoNNto.NetworkCore.Synapse_Group import *
 from PymoNNto.Exploration.Evolution.Interface_Functions import *
 import copy
 import time
 import sys
+from PymoNNto.NetworkCore.NumPy_Backend.NumPy_Backend import *
 
 float32 = np.float32
 float64 = np.float64
 
 SxD = 0
 DxS = 1
 
@@ -26,14 +27,17 @@
         self.behavior_timesteps = []
         self.sorted_behavior_execution_list = [] #stores (key, beh_parent, behavior) triplets
         
         super().__init__(tag, self, behavior)
 
     # {'dtype':float32, 'syn_dim':DxS}
     def apply_settings(self, settings):
+        #backend_class = settings.get('backend', NumPy)
+        #self.backend = backend_class()
+        self.backend = NumPy()
         self.def_dtype = settings.get('dtype', float32)
         self.transposed_synapse_matrix_mode = settings.get('syn_dim', DxS)!=DxS
 
     def all_objects(self):
         return [self]+self.NeuronGroups+self.SynapseGroups
 
     def _add_key_to_sorted_behavior_timesteps(self, key):
```

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkCore/Neuron_Group.py` & `PymoNNto-3.0.3/PymoNNto/NetworkCore/Neuron_Group.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/NetworkCore/Synapse_Group.py` & `PymoNNto-3.0.3/PymoNNto/NetworkCore/Synapse_Group.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/__init__.py` & `PymoNNto-3.0.3/PymoNNto/__init__.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto/test_pymoNNto.py` & `PymoNNto-3.0.3/PymoNNto/test_pymoNNto.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.2/PymoNNto.egg-info/PKG-INFO` & `PymoNNto-3.0.3/PymoNNto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PymoNNto
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python Modular Neural Network Toolbox
 Home-page: https://github.com/trieschlab/PymoNNto
 Author: Marius Vieth
 Author-email: mv15go@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PymoNNto-3.0.2/PymoNNto.egg-info/SOURCES.txt` & `PymoNNto-3.0.3/PymoNNto.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PymoNNto/test_pymoNNto.py
 PymoNNto.egg-info/PKG-INFO
 PymoNNto.egg-info/SOURCES.txt
 PymoNNto.egg-info/dependency_links.txt
 PymoNNto.egg-info/entry_points.txt
 PymoNNto.egg-info/requires.txt
 PymoNNto.egg-info/top_level.txt
-PymoNNto/Exploration/Behaviour_UI.py
+PymoNNto/Exploration/Behavior_UI.py
 PymoNNto/Exploration/Execute_UI.py
 PymoNNto/Exploration/Overview_UI.py
 PymoNNto/Exploration/UI_Base.py
 PymoNNto/Exploration/__init__.py
 PymoNNto/Exploration/AnalysisModules/Static_Classification.py
 PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Base.py
 PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Post.py
```

### Comparing `PymoNNto-3.0.2/setup.py` & `PymoNNto-3.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PymoNNto",
-    version="3.0.2",
+    version="3.0.3",
     author="Marius Vieth",
     author_email="mv15go@gmail.com",
     description="Python Modular Neural Network Toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/trieschlab/PymoNNto",
     packages=setuptools.find_packages(),
```

