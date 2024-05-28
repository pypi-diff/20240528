# Comparing `tmp/gdm-concordia-1.4.0.tar.gz` & `tmp/gdm-concordia-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdm-concordia-1.4.0.tar", last modified: Thu May 16 11:41:17 2024, max compression
+gzip compressed data, was "gdm-concordia-1.5.0.tar", last modified: Tue May 28 10:58:46 2024, max compression
```

## Comparing `gdm-concordia-1.4.0.tar` & `gdm-concordia-1.5.0.tar`

### file list

```diff
@@ -1,115 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.285225 gdm-concordia-1.4.0/concordia/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.285225 gdm-concordia-1.4.0/concordia/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/agents/basic_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.285225 gdm-concordia-1.4.0/concordia/associative_memory/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/associative_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/blank_memories.py
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/formative_memories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/importance_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.285225 gdm-concordia-1.4.0/concordia/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/clocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/clocks/game_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/clocks/game_clock_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.289224 gdm-concordia-1.4.0/concordia/components/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.289224 gdm-concordia-1.4.0/concordia/components/agent/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/all_similar_memories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/creative_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/dialectical_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/justify_recent_voluntary_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/person_by_situation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/scheduled_hint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/self_perception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/situation_perception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/somatic_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/components/game_master/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/current_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/current_scene_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/direct_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/player_status_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/relevant_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/schelling_diagram_payoffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/time_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/report_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/document/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/document_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/interactive_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/interactive_document_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/game_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/game_master_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/environment/scenes/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/scenes/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/scenes/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/language_model/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/cloud_vertex_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/google_aistudio_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/gpt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/no_language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/ollama_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/retry_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/common_sense_morality.py
--rw-r--r--   0 runner    (1001) docker     (127)    17111 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/dass_questionnaire.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/goal_achievement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/opinion_of_others.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/uncertainty_scale_question.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/concordia/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/tests/concordia_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/tests/mock_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/concordia/thought_chains/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/thought_chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/thought_chains/thought_chains.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/concordia/typing/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/game_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/concordia/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/measurements_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/gdm_concordia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:46.000988 gdm-concordia-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 10:58:46.000988 gdm-concordia-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.988988 gdm-concordia-1.5.0/concordia/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.988988 gdm-concordia-1.5.0/concordia/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/agents/basic_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.988988 gdm-concordia-1.5.0/concordia/associative_memory/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/associative_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/associative_memory/associative_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/associative_memory/blank_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/associative_memory/formative_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/associative_memory/importance_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.988988 gdm-concordia-1.5.0/concordia/clocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/clocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/clocks/game_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/clocks/game_clock_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.988988 gdm-concordia-1.5.0/concordia/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.992988 gdm-concordia-1.5.0/concordia/components/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/all_similar_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/characteristic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.992988 gdm-concordia-1.5.0/concordia/components/agent/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/contrib/affect_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/contrib/illness_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/creative_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/dialectical_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/justify_recent_voluntary_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/person_by_situation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/scheduled_hint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/self_perception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/situation_perception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/agent/somatic_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.992988 gdm-concordia-1.5.0/concordia/components/game_master/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.992988 gdm-concordia-1.5.0/concordia/components/game_master/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/contrib/world_background_and_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/current_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/current_scene_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/direct_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/player_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/relevant_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/schelling_diagram_payoffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/game_master/time_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/report_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/components/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.996988 gdm-concordia-1.5.0/concordia/document/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/document/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/document/document_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/document/interactive_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/document/interactive_document_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.996988 gdm-concordia-1.5.0/concordia/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/environment/game_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/environment/game_master_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.996988 gdm-concordia-1.5.0/concordia/environment/scenes/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/environment/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/environment/scenes/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/environment/scenes/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.996988 gdm-concordia-1.5.0/concordia/language_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/language_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/language_model/cloud_vertex_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/language_model/google_aistudio_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/language_model/gpt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/language_model/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/language_model/no_language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/language_model/ollama_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/language_model/pytorch_gemma_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/language_model/retry_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:45.996988 gdm-concordia-1.5.0/concordia/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/metrics/common_sense_morality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17111 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/metrics/dass_questionnaire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/metrics/goal_achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/metrics/opinion_of_others.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/metrics/uncertainty_scale_question.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:46.000988 gdm-concordia-1.5.0/concordia/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/tests/concordia_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/tests/mock_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:46.000988 gdm-concordia-1.5.0/concordia/thought_chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/thought_chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/thought_chains/thought_chains.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:46.000988 gdm-concordia-1.5.0/concordia/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/typing/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/typing/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/typing/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/typing/game_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/typing/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:46.000988 gdm-concordia-1.5.0/concordia/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/utils/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/utils/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/utils/measurements_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/utils/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/concordia/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:58:46.000988 gdm-concordia-1.5.0/gdm_concordia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 10:58:45.000000 gdm-concordia-1.5.0/gdm_concordia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-28 10:58:45.000000 gdm-concordia-1.5.0/gdm_concordia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:58:45.000000 gdm-concordia-1.5.0/gdm_concordia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 10:58:45.000000 gdm-concordia-1.5.0/gdm_concordia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 10:58:45.000000 gdm-concordia-1.5.0/gdm_concordia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 10:58:46.000988 gdm-concordia-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-28 10:58:44.000000 gdm-concordia-1.5.0/setup.py
```

### Comparing `gdm-concordia-1.4.0/LICENSE` & `gdm-concordia-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/PKG-INFO` & `gdm-concordia-1.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdm-concordia
-Version: 1.4.0
+Version: 1.5.0
 Summary: A library for building a generative model of social interacions.
 Home-page: https://github.com/google-deepmind/concordia
 Author: DeepMind
 Author-email: noreply@google.com
 License: Apache 2.0
 Download-URL: https://github.com/google-deepmind/concordia/releases
 Keywords: multi-agent agent-based-simulation generative-agents python machine-learning
```

### Comparing `gdm-concordia-1.4.0/README.md` & `gdm-concordia-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/__init__.py` & `gdm-concordia-1.5.0/concordia/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/agents/__init__.py` & `gdm-concordia-1.5.0/concordia/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/agents/basic_agent.py` & `gdm-concordia-1.5.0/concordia/agents/basic_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,18 @@
 
 Park, J.S., O'Brien, J.C., Cai, C.J., Morris, M.R., Liang, P. and
 Bernstein, M.S., 2023. Generative agents: Interactive simulacra of human
 behavior. arXiv preprint arXiv:2304.03442.
 """
 from collections.abc import Callable, Sequence
 import concurrent
-import contextlib
 import copy
 import datetime
 import threading
 
-from concordia.associative_memory import associative_memory
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from concordia.typing import agent
 from concordia.typing import clock as game_clock
 from concordia.typing import component
 from concordia.utils import helper_functions
 from IPython import display
@@ -44,55 +42,48 @@
     agent.SpeakerGenerativeAgent,
 ):
   """A Generative agent."""
 
   def __init__(
       self,
       model: language_model.LanguageModel,
-      memory: associative_memory.AssociativeMemory,
       agent_name: str,
       clock: game_clock.GameClock,
       components: Sequence[component.Component] | None = None,
-      num_memories_retrieved: int = 10,
       update_interval: datetime.timedelta = datetime.timedelta(hours=1),
       verbose: bool = False,
       user_controlled: bool = False,
-      print_colour='green',
+      print_colour: str = 'green',
   ):
     """A generative agent.
 
     Args:
       model: a language model
-      memory: an associative memory
       agent_name: the name of the agent
       clock: the game clock is needed to know when is the current time
       components: components that contextualise the policies. The components
         state will be added to the agents state in the order they are passed
         here.
-      num_memories_retrieved: number of memories to retrieve for acting,
-        speaking, testing
       update_interval: how often to update components. In game time according to
         the clock argument.
       verbose: whether to print chains of thought or not
       user_controlled: if True, would query user input for speech and action
       print_colour: which colour to use for printing
     """
     self._verbose = verbose
     self._print_colour = print_colour
 
     self._model = model
-    self._memory = memory
 
     self._agent_name = agent_name
     self._clock = clock
-    self._num_memories_retrieved = num_memories_retrieved
     self._user_controlled = user_controlled
     self._update_interval = update_interval
 
-    self._under_interrogation = False
+    self._conversation_prefix = ''
     self._state_lock = threading.Lock()
 
     self._components = {}
     for comp in components:
       self.add_component(comp)
 
     self._log = []
@@ -104,28 +95,23 @@
   def name(self) -> str:
     return self._agent_name
 
   def copy(self) -> 'BasicAgent':
     """Creates a copy of the agent."""
     new_sim = BasicAgent(
         model=self._model,
-        memory=self._memory,
         agent_name=self._agent_name,
         clock=self._clock,
         components=copy.copy(list(self._components.values())),
-        num_memories_retrieved=self._num_memories_retrieved,
         verbose=self._verbose,
         user_controlled=self._user_controlled,
         print_colour=self._print_colour,
     )
     return new_sim
 
-  def get_memory(self) -> associative_memory.AssociativeMemory:
-    return self._memory
-
   def _print(self, entry: str):
     print(termcolor.colored(entry, self._print_colour), end='')
 
   def add_component(self, comp: component.Component) -> None:
     """Add a component."""
     if comp.name() in self._components:
       raise ValueError(f'Duplicate component name: {comp.name()}')
@@ -135,36 +121,14 @@
   def remove_component(self, component_name: str) -> None:
     """Remove a component."""
     del self._components[component_name]
 
   def set_clock(self, clock: game_clock.GameClock):
     self._clock = clock
 
-  def enter_interrogation(self):
-    self._under_interrogation = True
-
-  def leave_interrogation(self):
-    self._under_interrogation = False
-
-  @contextlib.contextmanager
-  def interrogate(self):
-    """Context manager to interrogate the agent.
-
-    When in this context, agent makes no memories or observations and doesn't
-    update components.
-
-    Yields:
-      None
-    """
-    self.enter_interrogation()
-    try:
-      yield
-    finally:
-      self.leave_interrogation()
-
   def _ask_for_input(self, context: str, prompt: str) -> str:
     display.clear_output()
     print(context, flush=True)
     result = input(prompt)
     return result
 
   def get_last_log(self):
@@ -178,15 +142,15 @@
           f"{self._agent_name}'s " + (comp.name() + ':\n' + comp.state() + '\n')
           for comp in self._components.values()
           if comp.state()
       )
 
   def _maybe_update(self):
     next_update = self._last_update + self._update_interval
-    if self._clock.now() >= next_update and not self._under_interrogation:
+    if self._clock.now() >= next_update:
       self._update()
 
   def _update(self):
     self._last_update = self._clock.now()
 
     def _get_recursive_update_func(
         comp: component.Component,
@@ -196,23 +160,22 @@
       )
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
       for comp in self._components.values():
         executor.submit(_get_recursive_update_func(comp))
 
   def observe(self, observation: str):
-    if observation and not self._under_interrogation:
+    if observation:
       for comp in self._components.values():
         comp.observe(observation)
 
   def act(
       self,
       action_spec: agent.ActionSpec = agent.DEFAULT_ACTION_SPEC,
-      memorize: bool = False,
-  ):
+  ) -> str:
     if not action_spec:
       action_spec = agent.DEFAULT_ACTION_SPEC
     self._maybe_update()
     prompt = interactive_document.InteractiveDocument(self._model)
     context_of_action = '\n'.join([
         f'{self.state()}',
     ])
@@ -273,28 +236,32 @@
     if self._verbose:
       self._print(
           f'\n{self._agent_name} context of action:\n'
           + prompt.view().text()
           + '\n'
       )
 
-    if memorize and not self._under_interrogation:  # observe instead?
-      if action_spec.tag:
-        self._memory.add(
-            f'[{action_spec.tag}] {output}', tags=[action_spec.tag]
-        )
-      else:
-        self._memory.add(output)
-
     return output
 
-  def add_memory(self, memory: str, importance: float | None = None):
-    self._memory.add(memory, importance=importance)
+  def _observe_latest(self, conversation: str):
+    # If the prefix is not found then `find` returns -1.
+    prefix_start_index = conversation.find(self._conversation_prefix)
+    if prefix_start_index >= 0:
+      # Get the part of the conversation the agent heard since their last turn.
+      start_index = prefix_start_index + len(self._conversation_prefix)
+      conversation_suffix = conversation[start_index:]
+      # Replace newline characters with commas.
+      conversation_suffix = conversation_suffix.replace('\n', ', ')
+      # Observe the new part of the conversation.
+      self.observe(conversation_suffix)
+      # Store the whole conversation thus far as the new prefix.
+      self._conversation_prefix = conversation
 
   def say(self, conversation: str) -> str:
+    self._observe_latest(conversation)
     convo_context = (
         f'{self._agent_name} is in the following'
         f' conversation:\n{conversation}\n'
     )
     call_to_speech = agent.DEFAULT_CALL_TO_SPEECH.format(
         agent_name=self._agent_name,
     )
```

### Comparing `gdm-concordia-1.4.0/concordia/associative_memory/__init__.py` & `gdm-concordia-1.5.0/concordia/associative_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/associative_memory/associative_memory.py` & `gdm-concordia-1.5.0/concordia/associative_memory/associative_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 
 """An associative memory similar to the one in the following paper.
 
 Park, J.S., O'Brien, J.C., Cai, C.J., Morris, M.R., Liang, P. and Bernstein,
 M.S., 2023. Generative agents: Interactive simulacra of human behavior. arXiv
 preprint arXiv:2304.03442.
 """
+
 from collections.abc import Callable, Iterable
 import datetime
 import threading
 
+from concordia.associative_memory import importance_function
 import numpy as np
 import pandas as pd
 
 
 def _check_date_in_range(timestamp: datetime.datetime) -> None:
   if timestamp < pd.Timestamp.min:
     min_date = pd.Timestamp.min
@@ -38,30 +40,32 @@
 
 class AssociativeMemory:
   """Class that implements associative memory."""
 
   def __init__(
       self,
       sentence_embedder: Callable[[str], np.ndarray],
-      importance: Callable[[str], float],
+      importance: Callable[[str], float] | None = None,
       clock: Callable[[], datetime.datetime] = datetime.datetime.now,
       clock_step_size: datetime.timedelta | None = None,
   ):
     """Constructor.
 
     Args:
       sentence_embedder: text embedding model
-      importance: maps a sentence into [0,1] scale of importance
+      importance: maps a sentence into [0, 1] scale of importance, if None then
+        use a constant importance model that sets all memories to importance 1.0
       clock: a callable to get time when adding memories
       clock_step_size: sets the step size of the clock. If None, assumes precise
         time
     """
     self._memory_bank_lock = threading.Lock()
     self._embedder = sentence_embedder
-    self._importance = importance
+    self._importance = (
+        importance or importance_function.ConstantImportanceModel().importance)
 
     self._memory_bank = pd.DataFrame(
         columns=['text', 'time', 'tags', 'embedding', 'importance']
     )
     self._clock_now = clock
     self._interval = clock_step_size
     self._stored_hashes = set()
```

### Comparing `gdm-concordia-1.4.0/concordia/associative_memory/blank_memories.py` & `gdm-concordia-1.5.0/concordia/associative_memory/blank_memories.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,32 +15,44 @@
 
 """This is a factory for generating memories for generative agents."""
 
 from collections.abc import Callable
 import datetime
 
 from concordia.associative_memory import associative_memory
+from concordia.associative_memory import importance_function
 from concordia.language_model import language_model
 import numpy as np
 
 
 class MemoryFactory:
   """Generator of formative memories."""
 
   def __init__(
       self,
       model: language_model.LanguageModel,
       embedder: Callable[[str], np.ndarray],
-      importance: Callable[[str], float],
-      clock_now: Callable[[], datetime.datetime],
+      importance: Callable[[str], float] | None = None,
+      clock_now: Callable[[], datetime.datetime] | None = None,
   ):
+    """Initializes the memory factory.
+
+    Args:
+      model: The language model to use
+      embedder: The text embedder to use
+      importance: maps a sentence into [0, 1] scale of importance, if None then
+        use a constant importance model that sets all memories to importance 1.0
+      clock_now: a callable to get time when adding memories, if None then use
+        the current time.
+    """
     self._model = model
     self._embedder = embedder
-    self._importance = importance
-    self._clock_now = clock_now
+    self._importance = (
+        importance or importance_function.ConstantImportanceModel().importance)
+    self._clock_now = clock_now or datetime.datetime.now
 
   def make_blank_memory(
       self,
   ) -> associative_memory.AssociativeMemory:
     """Creates a blank memory.
 
     Returns a blank memory
```

### Comparing `gdm-concordia-1.4.0/concordia/associative_memory/formative_memories.py` & `gdm-concordia-1.5.0/concordia/associative_memory/formative_memories.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,19 +70,30 @@
   """Generator of formative memories."""
 
   def __init__(
       self,
       *,
       model: language_model.LanguageModel,
       shared_memories: Sequence[str] = (),
+      delimiter_symbol: str = '\n\n\n',
       blank_memory_factory_call: Callable[
           [], associative_memory.AssociativeMemory
       ],
   ):
+    """Initializes the formative memory factory.
+
+    Args:
+      model: the language model to use for generating memories
+      shared_memories: memories to be added to all agents
+      delimiter_symbol: the delimiter to use when splitting the generated
+        episodes
+      blank_memory_factory_call: a function that returns a new blank memory
+    """
     self._model = model
+    self._delimiter_symbol = delimiter_symbol
     self._blank_memory_factory_call = blank_memory_factory_call
     self._shared_memories = shared_memories
 
   def make_backstory(
       self, name: str, gender: str, traits_description: str, context: str | None
   ) -> str:
     """Creates a backstory of an agent based on traits.
@@ -188,16 +199,17 @@
         'important for establishing who they are as a person. They should '
         f'be consistent with {agent_config.name}\'s personality. '
         f'Describe each episode from {agent_config.name}\'s perspective '
         'and use third-person limited point of view. Each episode must '
         'mention their age at the time the event occurred using language such '
         f'as "When {agent_config.name} was 5 years old, they experienced..." . '
         'Use past tense. Write no more than three sentences per episode. '
-        'Separate episodes from one another by the delimiter "\n\n\n". Do not '
-        'apply any other special formatting besides these delimiters.'
+        'Separate episodes from one another by the delimiter '
+        f'"{self._delimiter_symbol}". Do not apply any other '
+        'special formatting besides these delimiters.'
     )
     if agent_config.traits:
       question += (
           '\nTaken as a whole, these formative episodes from the life of '
           f'{agent_config.name} should explain their personality, which has '
           f'been described as: "{agent_config.traits}".')
     if agent_config.context:
@@ -209,15 +221,15 @@
     aggregated_result = prompt.open_question(
         question=question,
         max_characters=8000,
         max_tokens=6000,
         terminators=[],
     )
 
-    episodes = aggregated_result.split('\n\n\n')
+    episodes = aggregated_result.split(self._delimiter_symbol)
 
     if len(episodes) != len(list(agent_config.formative_ages)):
       logger.warning(
           f'Number of generated formative episodes ({len(episodes)}) does ' +
           'not match number of formative ages ' +
           f'({len(list(agent_config.formative_ages))}).')
```

### Comparing `gdm-concordia-1.4.0/concordia/associative_memory/importance_function.py` & `gdm-concordia-1.5.0/concordia/associative_memory/importance_function.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/clocks/__init__.py` & `gdm-concordia-1.5.0/concordia/clocks/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/clocks/game_clock.py` & `gdm-concordia-1.5.0/concordia/clocks/game_clock.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/clocks/game_clock_test.py` & `gdm-concordia-1.5.0/concordia/clocks/game_clock_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/__init__.py` & `gdm-concordia-1.5.0/concordia/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/__init__.py` & `gdm-concordia-1.5.0/concordia/components/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/all_similar_memories.py` & `gdm-concordia-1.5.0/concordia/components/agent/self_perception.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,60 +8,63 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Return all memories similar to the prompt.
-"""
-
-from collections.abc import Callable, Sequence
+"""Agent component for representing what kind of person the agent is."""
 import datetime
+from typing import Callable, Sequence
+
 from concordia.associative_memory import associative_memory
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from concordia.typing import component
 import termcolor
 
 
-class AllSimilarMemories(component.Component):
-  """Get all memories similar to the state of the components."""
+class SelfPerception(component.Component):
+  """This component answers the question 'what kind of person is the agent?'."""
 
   def __init__(
       self,
       name: str,
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
       agent_name: str,
       components: Sequence[component.Component] | None = None,
       clock_now: Callable[[], datetime.datetime] | None = None,
-      num_memories_to_retrieve: int = 25,
+      num_memories_to_retrieve: int = 100,
       verbose: bool = False,
   ):
-    """Initializes the AllSimilarMemories component.
+    """Initializes the SelfPerception component.
 
     Args:
-      name: The name of the component.
-      model: The language model to use.
-      memory: The memory to use.
-      agent_name: The name of the agent.
+      name: Name of the component.
+      model: Language model.
+      memory: Associative memory.
+      agent_name: Name of the agent.
       components: The components to condition the answer on.
       clock_now: time callback to use for the state.
-      num_memories_to_retrieve: The number of memories to retrieve.
-      verbose: Whether to print the state of the component.
+      num_memories_to_retrieve: Number of memories to retrieve.
+      verbose: Whether to print the state.
     """
 
     self._verbose = verbose
     self._model = model
     self._memory = memory
     self._state = ''
     self._components = components or []
     self._agent_name = agent_name
+
     self._clock_now = clock_now
+    if clock_now is None:
+      self._clock_now = lambda: ''
+
     self._num_memories_to_retrieve = num_memories_to_retrieve
     self._name = name
     self._last_update = datetime.datetime.min
     self._history = []
 
   def name(self) -> str:
     return self._name
@@ -77,54 +80,53 @@
     return self._components
 
   def update(self) -> None:
     if self._clock_now() == self._last_update:
       return
     self._last_update = self._clock_now()
 
+    mems = '\n'.join(
+        self._memory.retrieve_recent(
+            self._num_memories_to_retrieve, add_time=True
+        )
+    )
+
     prompt = interactive_document.InteractiveDocument(self._model)
+    prompt.statement(f'Memories of {self._agent_name}:\n{mems}')
+
+    if self._clock_now is not None:
+      prompt.statement(f'Current time: {self._clock_now()}.\n')
 
     component_states = '\n'.join([
-        f"{self._agent_name}'s {comp.name()}:\n{comp.state()}"
+        f"{self._agent_name}'s "
+        + (comp.name() + ':\n' + comp.state())
         for comp in self._components
     ])
-    prompt.statement(f'Statements:\n{component_states}\n')
-    prompt_summary = prompt.open_question('Summarize the statements above.')
-
-    query = f'{self._agent_name}, {prompt_summary}'
-    if self._clock_now is not None:
-      query = f'[{self._clock_now()}] {query}'
-
-    mems = '\n'.join(
-        self._memory.retrieve_associative(
-            query, self._num_memories_to_retrieve, add_time=True
-        )
-    )
+    prompt.statement(component_states)
 
     question = (
-        'Select all the following statements that are important for '
-        f'{self._agent_name} to consider right now. Whenever statements '
-        'are not mutally consistent, then pick whichever one is the most '
-        'recent.'
+        f'Given the above, what kind of person is {self._agent_name}?'
     )
-    if self._clock_now is not None:
-      question = f'Current time: {self._clock_now()}.\n{question}'
-    new_prompt = prompt.new()
-    self._state = new_prompt.open_question(
-        f'{question}\nStatements:\n{mems}',
+    old_state = self._state
+    self._state = prompt.open_question(
+        question,
+        answer_prefix=f'{self._agent_name} is ',
         max_characters=3000,
-        max_tokens=2000,
+        max_tokens=1000,
     )
 
+    self._state = f'{self._agent_name} is {self._state}'
+
+    if old_state != self._state:
+      self._memory.add(f'[self reflection] {self._state}')
+
+    self._last_chain = prompt
     if self._verbose:
-      print(termcolor.colored(prompt.view().text(), 'green'), end='')
-      print(termcolor.colored(new_prompt.view().text(), 'green'), end='')
-      print(termcolor.colored(self._state, 'green'), end='')
+      print(termcolor.colored(self._last_chain.view().text(), 'green'), end='')
 
     update_log = {
         'date': self._clock_now(),
-        'Summary': self._name,
+        'Summary': question,
         'State': self._state,
-        'Initial chain of thought': prompt.view().text().splitlines(),
-        'Final chain of thought': new_prompt.view().text().splitlines(),
+        'Chain of thought': prompt.view().text().splitlines(),
     }
     self._history.append(update_log)
```

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/characteristic.py` & `gdm-concordia-1.5.0/concordia/components/agent/characteristic.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/creative_reflection.py` & `gdm-concordia-1.5.0/concordia/components/agent/creative_reflection.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/dialectical_reflection.py` & `gdm-concordia-1.5.0/concordia/components/agent/dialectical_reflection.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/identity.py` & `gdm-concordia-1.5.0/concordia/components/agent/identity.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Agent identity component."""
 import concurrent
 import datetime
-from typing import Callable
+from typing import Callable, Sequence
 from concordia.associative_memory import associative_memory
 from concordia.components.agent import characteristic
 from concordia.language_model import language_model
 from concordia.typing import component
 
 
 class SimIdentity(component.Component):
@@ -33,30 +33,34 @@
   """
 
   def __init__(
       self,
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
       agent_name: str,
+      name: str = 'identity',
       clock_now: Callable[[], datetime.datetime] | None = None,
   ):
     """Initialize an identity component.
 
     Args:
       model: a language model
       memory: an associative memory
       agent_name: the name of the agent
+      name: the name of the component
       clock_now: time callback to use for the state.
     """
     self._model = model
     self._memory = memory
     self._state = ''
     self._agent_name = agent_name
+    self._name = name
     self._clock_now = clock_now
     self._last_update = datetime.datetime.min
+    self._history = []
 
     self._identity_component_names = [
         'core characteristics',
         'current daily occupation',
         'feeling about recent progress in life',
     ]
 
@@ -69,37 +73,40 @@
               memory=self._memory,
               agent_name=self._agent_name,
               characteristic_name=component_name,
           )
       )
 
   def name(self) -> str:
-    return 'Identity'
+    return self._name
 
   def state(self):
     return self._state
 
   def get_last_log(self):
-    current_log = {
-        'Summary': f'identity of {self._agent_name}',
-        'state': self._state,
-    }
-    for comp in self._identity_components:
-      last_log = comp.get_last_log()
-      if last_log:
-        if 'date' in last_log.keys():
-          last_log.pop('date')
-        current_log[comp.name()] = last_log
-    return current_log
+    if self._history:
+      return self._history[-1].copy()
+
+  def get_components(self) -> Sequence[component.Component]:
+    # Since this component handles updating of its subcomponents itself, we
+    # therefore do not need to return them here.
+    return []
 
   def update(self):
     if self._clock_now() == self._last_update:
       return
     self._last_update = self._clock_now()
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
       for c in self._identity_components:
         executor.submit(c.update)
 
     self._state = '\n'.join(
         [f'{c.name()}: {c.state()}' for c in self._identity_components]
     )
+
+    update_log = {
+        'date': self._clock_now(),
+        'Summary': self._name,
+        'State': self._state,
+    }
+    self._history.append(update_log)
```

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/justify_recent_voluntary_actions.py` & `gdm-concordia-1.5.0/concordia/components/agent/justify_recent_voluntary_actions.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/observation.py` & `gdm-concordia-1.5.0/concordia/components/agent/observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     Args:
       agent_name: Name of the agent.
       model: Language model to summarise the observations.
       clock_now: Function that returns the current time.
       timeframe_delta_from: delta from the current moment to the begnning of the
         segment to summarise, e.g. 4h would summarise all observations that
-        happened from 4h ago intil clock_now minus timeframe_delta_until.
+        happened from 4h ago until clock_now minus timeframe_delta_until.
       timeframe_delta_until: delta from the current moment to the end of the
         segment to summarise.
       memory: Associative memory retrieve observations from.
       components: List of components to summarise.
       component_name: Name of the component.
       prompt: Language prompt for summarising memories and components.
       display_timeframe: Whether to display the time interval as text.
```

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/person_by_situation.py` & `gdm-concordia-1.5.0/concordia/components/agent/person_by_situation.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/plan.py` & `gdm-concordia-1.5.0/concordia/components/agent/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
   def __init__(
       self,
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
       agent_name: str,
       components: list[component.Component],
       clock_now: Callable[[], datetime.datetime],
+      name: str = 'plan',
       goal: component.Component | None = None,
       num_memories_to_retrieve: int = 5,
       timescale: str = 'the rest of the day',
       time_adverb: str = 'hourly',
       verbose: bool = False,
       log_color='green',
   ):
@@ -44,28 +45,30 @@
 
     Args:
       model: a language model
       memory: an associative memory
       agent_name: the name of the agent
       components: components to build the context of planning
       clock_now: time callback to use for the state.
+      name: name of the component
       goal: a component to represent the goal of planning
       num_memories_to_retrieve: how many memories to retrieve as conditioning
         for the planning chain of thought
       timescale: string describing how long the plan should last
       time_adverb: string describing the rate of steps in the plan
       verbose: whether or not to print intermediate reasoning steps
       log_color: color for debug logging
     """
     self._model = model
     self._memory = memory
     self._state = ''
     self._agent_name = agent_name
     self._log_color = log_color
     self._components = components
+    self._name = name
     self._num_memories_to_retrieve = num_memories_to_retrieve
     self._goal_component = goal
     self._timescale = timescale
     self._time_adverb = time_adverb
     self._clock_now = clock_now
     self._last_update = datetime.datetime.min
 
@@ -73,15 +76,15 @@
     self._last_observation = []
     self._current_plan = ''
     self._history = []
 
     self._verbose = verbose
 
   def name(self) -> str:
-    return 'Plan'
+    return self._name
 
   def state(self):
     return self._state
 
   def get_last_log(self):
     if self._history:
       return self._history[-1].copy()
```

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/reflection.py` & `gdm-concordia-1.5.0/concordia/components/agent/reflection.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/relationships.py` & `gdm-concordia-1.5.0/concordia/components/agent/relationships.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/scheduled_hint.py` & `gdm-concordia-1.5.0/concordia/components/agent/scheduled_hint.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/self_perception.py` & `gdm-concordia-1.5.0/concordia/components/agent/situation_perception.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,75 +8,76 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Agent component for self perception."""
+"""Agent component for situation perception."""
 import datetime
-from typing import Callable
+from typing import Callable, Sequence
 
 from concordia.associative_memory import associative_memory
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from concordia.typing import component
 import termcolor
 
 
-class SelfPerception(component.Component):
-  """This component answers the question 'what kind of person is the agent?'."""
+class SituationPerception(component.Component):
+  """This component answers the question 'what kind of situation is it?'."""
 
   def __init__(
       self,
       name: str,
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
       agent_name: str,
+      components: Sequence[component.Component] | None = None,
       clock_now: Callable[[], datetime.datetime] | None = None,
-      num_memories_to_retrieve: int = 100,
+      num_memories_to_retrieve: int = 25,
       verbose: bool = False,
   ):
-    """Initializes the SelfPerception component.
+    """Initializes the component.
 
     Args:
-      name: Name of the component.
-      model: Language model.
-      memory: Associative memory.
-      agent_name: Name of the agent.
+      name: The name of the component.
+      model: The language model to use.
+      memory: The memory to use.
+      agent_name: The name of the agent.
+      components: The components to condition the answer on.
       clock_now: time callback to use for the state.
-      num_memories_to_retrieve: Number of memories to retrieve.
-      verbose: Whether to print the state.
+      num_memories_to_retrieve: The number of memories to retrieve.
+      verbose: Whether to print the last chain.
     """
-
     self._verbose = verbose
     self._model = model
     self._memory = memory
     self._state = ''
+    self._components = components or []
     self._agent_name = agent_name
-
     self._clock_now = clock_now
-    if clock_now is None:
-      self._clock_now = lambda: ''
-
     self._num_memories_to_retrieve = num_memories_to_retrieve
     self._name = name
-    self._last_update = datetime.datetime.min
+    self._last_update = self._clock_now() - datetime.timedelta(days=365)
     self._history = []
 
   def name(self) -> str:
     return self._name
 
   def state(self) -> str:
     return self._state
 
   def get_last_log(self):
     if self._history:
       return self._history[-1].copy()
 
+  def get_components(self) -> Sequence[component.Component]:
+    return self._components
+
   def update(self) -> None:
     if self._clock_now() == self._last_update:
       return
     self._last_update = self._clock_now()
 
     mems = '\n'.join(
         self._memory.retrieve_recent(
@@ -86,29 +87,32 @@
 
     prompt = interactive_document.InteractiveDocument(self._model)
     prompt.statement(f'Memories of {self._agent_name}:\n{mems}')
 
     if self._clock_now is not None:
       prompt.statement(f'Current time: {self._clock_now()}.\n')
 
+    component_states = '\n'.join([
+        f"{self._agent_name}'s "
+        + (comp.name() + ':\n' + comp.state())
+        for comp in self._components
+    ])
+    prompt.statement(component_states)
+
     question = (
-        f'Given the memories above, what kind of person is {self._agent_name}?'
+        'Given the statements above, what kind of situation is'
+        f' {self._agent_name} in right now?'
     )
-    old_state = self._state
     self._state = prompt.open_question(
         question,
-        answer_prefix=f'{self._agent_name} is ',
+        answer_prefix=f'{self._agent_name} is currently ',
         max_characters=3000,
         max_tokens=1000,
     )
-
-    self._state = f'{self._agent_name} is {self._state}'
-
-    if old_state != self._state:
-      self._memory.add(f'[self reflection] {self._state}')
+    self._state = f'{self._agent_name} is currently {self._state}'
 
     self._last_chain = prompt
     if self._verbose:
       print(termcolor.colored(self._last_chain.view().text(), 'green'), end='')
 
     update_log = {
         'date': self._clock_now(),
```

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/situation_perception.py` & `gdm-concordia-1.5.0/concordia/components/game_master/player_status.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,116 +8,118 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Agent component for situation perception."""
+
+"""This construct track the status and location of players."""
+
+from collections.abc import Callable, Sequence
 import datetime
-from typing import Callable, Sequence
+import threading
 
 from concordia.associative_memory import associative_memory
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from concordia.typing import component
-import termcolor
 
 
-class SituationPerception(component.Component):
-  """This component answers the question 'what kind of situation is it?'."""
+class PlayerStatus(component.Component):
+  """Tracks the status of players."""
 
   def __init__(
       self,
-      name: str,
+      clock_now: Callable[[], datetime.datetime],
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
-      agent_name: str,
-      components: Sequence[component.Component] | None = None,
-      clock_now: Callable[[], datetime.datetime] | None = None,
-      num_memories_to_retrieve: int = 25,
+      player_names: Sequence[str],
+      num_memories_to_retrieve: int = 10,
       verbose: bool = False,
   ):
-    """Initializes the component.
+    """Constructs a PlayerStatus component.
 
     Args:
-      name: The name of the component.
-      model: The language model to use.
-      memory: The memory to use.
-      agent_name: The name of the agent.
-      components: The components to condition the answer on.
-      clock_now: time callback to use for the state.
-      num_memories_to_retrieve: The number of memories to retrieve.
-      verbose: Whether to print the last chain.
+      clock_now: A function that returns the current time.
+      model: A language model.
+      memory: An associative memory.
+      player_names: A list of player names to track.
+      num_memories_to_retrieve: The number of memories to retrieve (max).
+      verbose: Whether to print the prompt to the console.
     """
-    self._verbose = verbose
-    self._model = model
     self._memory = memory
+    self._model = model
     self._state = ''
-    self._components = components or []
-    self._agent_name = agent_name
-    self._clock_now = clock_now
+    self._player_names = player_names
     self._num_memories_to_retrieve = num_memories_to_retrieve
-    self._name = name
-    self._last_update = self._clock_now() - datetime.timedelta(days=365)
+    self._partial_states = {name: '' for name in self._player_names}
+    self._verbose = verbose
     self._history = []
+    self._clock_now = clock_now
+    self._last_memory_len = 0
+    self._state_lock = threading.Lock()
 
   def name(self) -> str:
-    return self._name
+    return 'Status of players'
 
   def state(self) -> str:
-    return self._state
+    with self._state_lock:
+      return self._state
+
+  def get_history(self):
+    with self._state_lock:
+      return self._history.copy()
 
   def get_last_log(self):
-    if self._history:
-      return self._history[-1].copy()
+    with self._state_lock:
+      if self._history:
+        return self._history[-1].copy()
 
-  def get_components(self) -> Sequence[component.Component]:
-    return self._components
+  def partial_state(
+      self,
+      player_name: str,
+  ) -> str:
+    """Return a player-specific view of the construct's state."""
+    with self._state_lock:
+      return self._partial_states[player_name]
 
   def update(self) -> None:
-    if self._clock_now() == self._last_update:
-      return
-    self._last_update = self._clock_now()
-
-    mems = '\n'.join(
-        self._memory.retrieve_recent(
-            self._num_memories_to_retrieve, add_time=True
+    with self._state_lock:
+      if self._last_memory_len == len(self._memory):
+        return
+      self._last_memory_len = len(self._memory)
+
+      self._state = ''
+      self._partial_states = {name: '' for name in self._player_names}
+      per_player_prompt = {}
+      for player_name in self._player_names:
+        memories = self._memory.retrieve_by_regex(player_name)
+        memories = memories[-self._num_memories_to_retrieve:]
+        prompt = interactive_document.InteractiveDocument(self._model)
+        prompt.statement('Events:\n' + '\n'.join(memories) + '\n')
+        time_now = self._clock_now().strftime('[%d %b %Y %H:%M:%S]')
+        prompt.statement(f'The current time is: {time_now}\n')
+        player_loc = (
+            prompt.open_question(
+                'Given the above events and their time, what is the latest'
+                f' location of {player_name} and what are they doing?',
+                answer_prefix=f'{player_name} is ',
+            )
+            + '\n'
         )
-    )
-
-    prompt = interactive_document.InteractiveDocument(self._model)
-    prompt.statement(f'Memories of {self._agent_name}:\n{mems}')
-
-    if self._clock_now is not None:
-      prompt.statement(f'Current time: {self._clock_now()}.\n')
-
-    component_states = '\n'.join([
-        f"{self._agent_name}'s "
-        + (comp.name() + ':\n' + comp.state())
-        for comp in self._components
-    ])
-    prompt.statement(component_states)
-
-    question = (
-        'Given the statements above, what kind of situation is'
-        f' {self._agent_name} in right now?'
-    )
-    self._state = prompt.open_question(
-        question,
-        answer_prefix=f'{self._agent_name} is currently ',
-        max_characters=3000,
-        max_tokens=1000,
-    )
-    self._state = f'{self._agent_name} is currently {self._state}'
-
-    self._last_chain = prompt
-    if self._verbose:
-      print(termcolor.colored(self._last_chain.view().text(), 'green'), end='')
-
-    update_log = {
-        'date': self._clock_now(),
-        'Summary': question,
-        'State': self._state,
-        'Chain of thought': prompt.view().text().splitlines(),
-    }
-    self._history.append(update_log)
+        per_player_prompt[player_name] = prompt.view().text().splitlines()
+        if self._verbose:
+          print(prompt.view().text())
+
+        # Indent player status outputs.
+        player_state_string = f'  {player_name} is ' + player_loc
+        self._partial_states[player_name] = player_state_string
+        self._state = self._state + player_state_string
+
+      update_log = {
+          'date': self._clock_now(),
+          'state': self._state,
+          'partial states': self._partial_states,
+          'per player prompts': per_player_prompt,
+      }
+      self._history.append(update_log)
```

### Comparing `gdm-concordia-1.4.0/concordia/components/agent/somatic_state.py` & `gdm-concordia-1.5.0/concordia/components/agent/somatic_state.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/constant.py` & `gdm-concordia-1.5.0/concordia/components/constant.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/__init__.py` & `gdm-concordia-1.5.0/concordia/components/game_master/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/conversation.py` & `gdm-concordia-1.5.0/concordia/components/game_master/conversation.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         f' following:\n{self._shared_context}'
     )
 
     mem = self._burner_memory_factory.make_blank_memory()
 
     npc = basic_agent.BasicAgent(
         model=self._model,
-        memory=mem,
         agent_name=name,
         clock=scene_clock,
         components=[
             generic_components.constant.ConstantComponent(
                 name='Instructions:', state=self._npc_instructions
             ),
             generic_components.constant.ConstantComponent(
```

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/current_scene.py` & `gdm-concordia-1.5.0/concordia/components/game_master/current_scene.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/current_scene_test.py` & `gdm-concordia-1.5.0/concordia/components/game_master/current_scene_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/direct_effect.py` & `gdm-concordia-1.5.0/concordia/components/game_master/direct_effect.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/inventory.py` & `gdm-concordia-1.5.0/concordia/components/game_master/inventory.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/player_status_test.py` & `gdm-concordia-1.5.0/concordia/components/game_master/player_status_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/relevant_events.py` & `gdm-concordia-1.5.0/concordia/components/game_master/relevant_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,24 +67,24 @@
   def get_history(self):
     return self._history.copy()
 
   def get_last_log(self):
     if self._history:
       return self._history[-1].copy()
 
-  def update_before_event(self, cause_statement: str) -> None:
+  def update_before_event(self, action_attempt: str) -> None:
     mem_retrieved = self._memory.retrieve_associative(
-        cause_statement,
+        action_attempt,
         use_recency=self._use_recency,
         add_time=self._add_time,
         k=self._num_memories_retrieved_for_update,
     )
 
     mems = '\n'.join(mem_retrieved)
     self._state = mems
 
     update_log = {
         'date': self._clock_now(),
         'state': self._state,
-        'cause_statement': cause_statement,
+        'action_attempt': action_attempt,
     }
     self._history.append(update_log)
```

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/schedule.py` & `gdm-concordia-1.5.0/concordia/components/game_master/schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,8 +84,8 @@
 
     for event_name in events_to_pop:
       self._schedule.pop(event_name)
 
     if events:
       self._state = '\n'.join(events)
     else:
-      self._state = 'None'
+      self._state = None
```

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/schelling_diagram_payoffs.py` & `gdm-concordia-1.5.0/concordia/components/game_master/schelling_diagram_payoffs.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,15 +85,14 @@
     self._outcome_summarization_fn = outcome_summarization_fn
     self._clock_now = clock_now
     self._name = name
     self._verbose = verbose
 
     self._history = []
     self._state = ''
-    self._last_update = self._clock_now() - datetime.timedelta(days=365)
     self._partial_states = {player.name: '' for player in self._players}
     self._player_scores = {player.name: 0 for player in self._players}
 
     self._resolution_scene = resolution_scene
     self._current_scene = current_scene.CurrentScene(
         name='current scene type',
         memory=self._memory,
@@ -103,17 +102,17 @@
 
     self.reset()
     # Set the initial state's string representation.
     self.update()
 
   def reset(self) -> None:
     self._stage_idx = 0
-    # Per stage, map each player's name to their component of the joint action.
-    self._stage_to_joint_action = [
-        {name: None for name in self._acting_player_names}]
+    # Map each player's name to their component of the joint action.
+    self._partial_joint_action = {
+        name: None for name in self._acting_player_names}
 
   def name(self) -> str:
     """Returns the name of this component."""
     return self._name
 
   def get_last_log(self):
     if self._history:
@@ -139,29 +138,28 @@
     for acting_player_name in self._acting_player_names:
       if joint_action[acting_player_name] is None:
         return False
     return True
 
   def _binarize_joint_action(
       self,
-      joint_action: Mapping[str, str]) -> Mapping[str, int]:
+      joint_action: Mapping[str, str]) -> Mapping[str, bool]:
     binary_joint_action = {name: act == self._cooperative_option
                            for name, act in joint_action.items()}
     return binary_joint_action
 
   def _get_rewards_from_joint_action(
-      self, binary_joint_action: Mapping[str, int]) -> Mapping[str, float]:
-    # For now, this only supports "Schelling style" (binary choice with
+      self, binary_joint_action: Mapping[str, bool]) -> Mapping[str, float]:
+    # This scoring function only supports "Schelling style" (binary choice with
     # externalities) type of game representations. This means the critical
     # factor is the number of players picking the cooperate option.
     num_cooperators = np.sum(list(binary_joint_action.values()))
 
     rewards = {}
-    for player_name, is_cooperator in zip(self._acting_player_names,
-                                          binary_joint_action):
+    for player_name, is_cooperator in binary_joint_action.items():
       if is_cooperator:
         rewards[player_name] = self._cooperator_reward_fn(num_cooperators)
       else:
         rewards[player_name] = self._defector_reward_fn(num_cooperators)
 
     return rewards
 
@@ -195,50 +193,60 @@
         player.observe(partial_states[player.name])
       else:
         player.observe(common_view_of_player_obs)
 
   def update_before_event(self, player_action_attempt: str) -> None:
     # `player_action_attempt` is formatted as "name: attempt".
     player_name, choice_str = player_action_attempt.split(': ')
-    self._stage_to_joint_action[self._stage_idx][player_name] = choice_str
+    self._partial_joint_action[player_name] = choice_str
+    self._state = ''
 
   def update_after_event(
       self,
       event_statement: str,
   ) -> None:
-    if self._clock_now() == self._last_update:
-      return
-    self._last_update = self._clock_now()
-
     current_scene_type = self._current_scene.state()
-    joint_action = []
+    payoffs_for_log = ''
+    joint_action_for_log = ''
+    finished = False
     if current_scene_type == self._resolution_scene:
       # Check if all players have acted so far in the current stage game.
-      joint_action = self._stage_to_joint_action[self._stage_idx]
+      joint_action = self._partial_joint_action.copy()
       if self._joint_action_is_complete(joint_action):
         # Map the joint action to rewards per player.
         binary_joint_action = self._binarize_joint_action(joint_action)
         rewards = self._get_rewards_from_joint_action(binary_joint_action)
 
         # Accumulate the rewards per player.
         for name in self._acting_player_names:
           self._player_scores[name] += rewards[name]
 
-        # Determine summary messages for each player and the GM.
+        # Use the outcome summarization function to get the state.
         self._set_outcome_messages(binary_joint_action, rewards)
+        self._memory.extend([self.state(),])
 
-        # Advance to the next stage.
-        self._stage_idx += 1
-        self._stage_to_joint_action.append(
-            {name: None for name in self._acting_player_names})
-
-      if self._verbose:
-        print(termcolor.colored(self.state(), 'yellow'))
-
+        joint_action_for_log = str(self._partial_joint_action)
+        payoffs_for_log = self.state()
+        finished = True
+
+        if self._verbose:
+          print(termcolor.colored(self.state(), 'yellow'))
+
+    num_players_already_acted = np.sum(
+        [value is not None for value in self._partial_joint_action.values()])
+    total_num_players_to_act = len(self._partial_joint_action)
     update_log = {
         'date': self._clock_now(),
         'Summary': self.name(),
-        'Schelling diagram payoffs': self.state(),
-        'Joint action': str(joint_action),
+        'Stage index': self._stage_idx,
+        'How many players acted so far this stage': (
+            f'{num_players_already_acted}/{total_num_players_to_act}'),
+        'Schelling diagram payoffs': payoffs_for_log,
+        'Joint action': joint_action_for_log,
     }
-    self._memory.extend([self._state,])
     self._history.append(update_log)
+
+    if finished:
+      # Advance to the next stage.
+      self._stage_idx += 1
+      self._partial_joint_action = {
+          name: None for name in self._acting_player_names}
```

### Comparing `gdm-concordia-1.4.0/concordia/components/game_master/time_display.py` & `gdm-concordia-1.5.0/concordia/components/game_master/time_display.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/report_function.py` & `gdm-concordia-1.5.0/concordia/components/report_function.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/components/sequential.py` & `gdm-concordia-1.5.0/concordia/components/sequential.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/document/__init__.py` & `gdm-concordia-1.5.0/concordia/document/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/document/document.py` & `gdm-concordia-1.5.0/concordia/document/document.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/document/document_test.py` & `gdm-concordia-1.5.0/concordia/document/document_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/document/interactive_document.py` & `gdm-concordia-1.5.0/concordia/document/interactive_document.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/document/interactive_document_test.py` & `gdm-concordia-1.5.0/concordia/document/interactive_document_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/environment/__init__.py` & `gdm-concordia-1.5.0/concordia/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/environment/game_master.py` & `gdm-concordia-1.5.0/concordia/environment/game_master.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A Generic Game Master."""
 
 from collections.abc import Callable, Sequence
 import concurrent.futures
+import dataclasses
+import datetime
 import random
 
 from concordia import components as generic_components
 from concordia.agents import basic_agent
 from concordia.associative_memory import associative_memory
 from concordia.document import interactive_document
 from concordia.language_model import language_model
@@ -51,14 +53,28 @@
     'take actions and change things in their world. Remember that this '
     'is a serious social science experiment. It is not just a game. It '
     'need not be fun for the participants. Always use third-person '
     'limited perspective, even when speaking directly to the participants.'
 )
 
 
+@dataclasses.dataclass
+class LogEntry:
+  """A log entry to be inserted into the game master's log at a given time.
+
+  Attributes:
+    date: the time associated with this log entry (in-game time)
+    event_statement: a statement of the event that occurred
+    summary: information about the event
+  """
+  date: datetime.datetime
+  event_statement: str
+  summary: str
+
+
 class GameMaster(simulacrum_game_master.GameMaster):
   """A generic game master."""
 
   def __init__(
       self,
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
@@ -154,14 +170,23 @@
   @property
   def name(self) -> str:
     return self._name
 
   def get_history(self):
     return self._log.copy()
 
+  def insert_history(self, log_entry: LogEntry):
+    """Insert a log entry into the game master's log, often used with scenes."""
+    update_log = {
+        'date': log_entry.date,
+        'Event statement': log_entry.event_statement,
+        'Summary': log_entry.summary,
+    }
+    self._log.append(update_log)
+
   def get_memory(self) -> associative_memory.AssociativeMemory:
     return self._memory
 
   def get_data_frame(self):
     return self._memory.get_data_frame()
 
   def _print(self, entry, color=None):
```

### Comparing `gdm-concordia-1.4.0/concordia/environment/game_master_test.py` & `gdm-concordia-1.5.0/concordia/environment/game_master_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 """Test the sequence of calls made by the game master to the components."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from concordia.agents import basic_agent
 from concordia.associative_memory import associative_memory
-from concordia.associative_memory import blank_memories
 from concordia.associative_memory import importance_function
 from concordia.clocks import game_clock
 from concordia.environment import game_master
 from concordia.tests import mock_model
 from concordia.typing import component
 import numpy as np
 
@@ -90,39 +89,28 @@
     gm_call_tracker = CallTrackingComponent()
 
     model = mock_model.MockModel()
 
     importance_model = importance_function.ConstantImportanceModel()
 
     clock = game_clock.FixedIntervalClock()
-    mem_factory = blank_memories.MemoryFactory(
-        model=model,
-        embedder=embedder,
-        importance=importance_model.importance,
-        clock_now=clock.now,
-    )
-
-    mem = mem_factory.make_blank_memory()
-
     alice_call_tracker = CallTrackingComponent()
 
     alice = basic_agent.BasicAgent(
         model,
-        mem,
         'Alice',
         clock,
         [alice_call_tracker],
         verbose=False,
     )
 
     bob_call_tracker = CallTrackingComponent()
 
     bob = basic_agent.BasicAgent(
         model,
-        mem,
         'Bob',
         clock,
         [bob_call_tracker],
         verbose=False,
     )
 
     game_master_memory = associative_memory.AssociativeMemory(
```

### Comparing `gdm-concordia-1.4.0/concordia/environment/scenes/__init__.py` & `gdm-concordia-1.5.0/concordia/environment/scenes/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/environment/scenes/conversation.py` & `gdm-concordia-1.5.0/concordia/environment/scenes/conversation.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/environment/scenes/runner.py` & `gdm-concordia-1.5.0/concordia/environment/scenes/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,26 +86,37 @@
     participant_names = [config.name for config in scene.participant_configs]
     if verbose:
       print(f'\n\n    Scene {scene_idx}    Participants: {participant_names}\n')
     participants = [players_by_name[name] for name in participant_names]
 
     # Prepare to run the scene
     clock.set(scene.start_time)
+
+    all_premises = ''
     for participant in participants:
       premise_messages = _get_interscene_messages(
           key='premise',
           agent_name=participant.name,
           scene_type_spec=scene.scene_type,
       )
       for message in premise_messages:
+        all_premises += f'{participant.name} -- premise: {message}      \n'
         if verbose:
           print(f'{participant.name} -- premise: {message}')
         participant.observe(message)
         this_scene_game_master_memory.add(message)
 
+    # Add the scene and its premise to the history
+    scene_update_log_entry = game_master.LogEntry(
+        date=clock.now(),
+        event_statement=all_premises,
+        summary=f'Scene {scene_idx} --- Participants: {participant_names}',
+    )
+    environment.insert_history(log_entry=scene_update_log_entry)
+
     # Run the scene
     for _ in range(scene.num_rounds):
       this_scene_game_master_memory.add(f'[scene type] {scene.scene_type.name}')
       this_scene_environment.step(active_players=participants,
                                   action_spec=scene.scene_type.action_spec)
 
     # Conclude the scene
```

### Comparing `gdm-concordia-1.4.0/concordia/language_model/__init__.py` & `gdm-concordia-1.5.0/concordia/language_model/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/language_model/cloud_vertex_model.py` & `gdm-concordia-1.5.0/concordia/language_model/cloud_vertex_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Google Cloud Vertex Language Model."""
 
 from collections.abc import Collection, Sequence
 import copy
-import re
 import time
 
 from concordia.language_model import language_model
 from concordia.utils import measurements as measurements_lib
+from concordia.utils import sampling
 from concordia.utils import text
 
 from typing_extensions import override
 
 from vertexai.preview.generative_models import Content
 from vertexai.preview.generative_models import GenerativeModel
 from vertexai.preview.generative_models import HarmBlockThreshold
@@ -58,23 +58,14 @@
     Content(
         role='model',
         parts=[Part.from_dict({
             'text': 'sleeping.'})]),
 )
 
 
-def extract_response(sample: str):
-  """Given text formatted as 'lorum(a)ipsum', return 'a'."""
-  match = re.search(r'\(?(\w)\)', sample)
-  if match:
-    return match.group(1)
-  else:
-    return None
-
-
 class VertexLanguageModel(language_model.LanguageModel):
   """Language model via the vertex API for Google Cloud."""
 
   def __init__(
       self,
       model_name: str = 'gemini-pro',
       harm_block_threshold: HarmBlockThreshold = HarmBlockThreshold.BLOCK_NONE,
@@ -159,50 +150,42 @@
   def sample_choice(
       self,
       prompt: str,
       responses: Sequence[str],
       *,
       seed: int | None = None,
   ) -> tuple[int, str, dict[str, float]]:
-    attempts = 1
-    for _ in range(MAX_MULTIPLE_CHOICE_ATTEMPTS):
+    sample = ''
+    answer = ''
+    for attempts in range(MAX_MULTIPLE_CHOICE_ATTEMPTS):
       # Increase temperature after the first failed attempt.
-      temperature = 0.0
-      if attempts > 1:
-        temperature = 0.5
+      temperature = sampling.dynamically_adjust_temperature(
+          attempts, MAX_MULTIPLE_CHOICE_ATTEMPTS)
 
       question = (
           'The following is a multiple choice question. Respond ' +
           'with one of the possible choices, such as (a) or (b). ' +
           f'Do not include reasoning.\n{prompt}')
       sample = self.sample_text(
           question,
           max_tokens=256,  # This is wasteful, but Gemini blocks lower values.
           temperature=temperature,
           seed=seed,
       )
-      if len(sample) == 1:
-        # i.e. this would be a sample such as "a"
-        answer = sample
-      elif len(sample) == 2:
-        # i.e. this would be a sample such as "a)"
-        answer = sample[0]
-      else:
-        # extract a substring like "(a)" wherever it may be in a longer string
-        answer = extract_response(sample)
+      answer = sampling.extract_choice_response(sample)
       try:
         idx = responses.index(answer)
       except ValueError:
-        attempts += 1
         print(f'Sample choice fail: {answer} extracted from {sample}.')
         continue
       else:
         if self._measurements is not None:
           self._measurements.publish_datum(
               self._channel,
               {'choices_calls': attempts})
         debug = {}
         return idx, responses[idx], debug
 
     raise language_model.InvalidResponseError(
-        'Too many multiple choice attempts.'
+        (f'Too many multiple choice attempts.\nLast attempt: {sample}, ' +
+         f'extracted: {answer}')
     )
```

### Comparing `gdm-concordia-1.4.0/concordia/language_model/google_aistudio_model.py` & `gdm-concordia-1.5.0/concordia/language_model/google_aistudio_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Google AI Studio Language Model API."""
 
 from collections.abc import Collection, Mapping, Sequence
 import copy
-import re
 import time
 
 from concordia.language_model import language_model
 from concordia.utils import measurements as measurements_lib
+from concordia.utils import sampling
 from concordia.utils import text
 import google.generativeai as genai
 
 from typing_extensions import override
 
 
 MAX_MULTIPLE_CHOICE_ATTEMPTS = 20
@@ -88,23 +88,14 @@
     {
         'category': 'HARM_CATEGORY_DANGEROUS_CONTENT',
         'threshold': 'BLOCK_MEDIUM_AND_ABOVE',
     },
 )
 
 
-def extract_response(sample: str):
-  """Given text formatted as 'lorum(a)ipsum', return 'a'."""
-  match = re.search(r'\(?(\w)\)', sample)
-  if match:
-    return match.group(1)
-  else:
-    return None
-
-
 class GoogleAIStudioLanguageModel(language_model.LanguageModel):
   """Language model API obtained via the Google AI Studio."""
 
   def __init__(
       self,
       api_key: str,
       model_name: str = 'gemini-1.5-pro-latest',
@@ -199,50 +190,42 @@
   def sample_choice(
       self,
       prompt: str,
       responses: Sequence[str],
       *,
       seed: int | None = None,
   ) -> tuple[int, str, dict[str, float]]:
-    attempts = 1
-    for _ in range(MAX_MULTIPLE_CHOICE_ATTEMPTS):
+    sample = ''
+    answer = ''
+    for attempts in range(MAX_MULTIPLE_CHOICE_ATTEMPTS):
       # Increase temperature after the first failed attempt.
-      temperature = 0.0
-      if attempts > 1:
-        temperature = 0.5
+      temperature = sampling.dynamically_adjust_temperature(
+          attempts, MAX_MULTIPLE_CHOICE_ATTEMPTS)
 
       question = (
           'The following is a multiple choice question. Respond ' +
           'with one of the possible choices, such as (a) or (b). ' +
           f'Do not include reasoning.\n{prompt}')
       sample = self.sample_text(
           question,
           max_tokens=256,  # This is wasteful, but Gemini blocks lower values.
           temperature=temperature,
           seed=seed,
       )
-      if len(sample) == 1:
-        # i.e. this would be a sample such as "a"
-        answer = sample
-      elif len(sample) == 2:
-        # i.e. this would be a sample such as "a)"
-        answer = sample[0]
-      else:
-        # extract a substring like "(a)" wherever it may be in a longer string
-        answer = extract_response(sample)
+      answer = sampling.extract_choice_response(sample)
       try:
         idx = responses.index(answer)
       except ValueError:
-        attempts += 1
         print(f'Sample choice fail: {answer} extracted from {sample}.')
         continue
       else:
         if self._measurements is not None:
           self._measurements.publish_datum(
               self._channel,
               {'choices_calls': attempts})
         debug = {}
         return idx, responses[idx], debug
 
     raise language_model.InvalidResponseError(
-        'Too many multiple choice attempts.'
+        (f'Too many multiple choice attempts.\nLast attempt: {sample}, ' +
+         f'extracted: {answer}')
     )
```

### Comparing `gdm-concordia-1.4.0/concordia/language_model/gpt_model.py` & `gdm-concordia-1.5.0/concordia/language_model/gpt_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,32 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Language Model that uses OpenAI's GPT models."""
 
 from collections.abc import Collection, Sequence
-import re
 from concordia.language_model import language_model
 from concordia.utils import measurements as measurements_lib
+from concordia.utils import sampling
 import openai
 from typing_extensions import override
 
 _MAX_MULTIPLE_CHOICE_ATTEMPTS = 20
 
 
-def extract_response(sample: str):
-  """Given text formatted as 'lorum(a)ipsum', return 'a'."""
-  match = re.search(r'\(?(\w)\)', sample)
-  if match:
-    return match.group(1)
-  else:
-    return None
-
-
 class GptLanguageModel(language_model.LanguageModel):
   """Language Model that uses OpenAI GPT models."""
 
   def __init__(
       self,
       api_key: str,
       model_name: str,
@@ -117,48 +108,36 @@
   def sample_choice(
       self,
       prompt: str,
       responses: Sequence[str],
       *,
       seed: int | None = None,
   ) -> tuple[int, str, dict[str, float]]:
-
-    attempts = 1
     prompt = (
         prompt
         + '\nRespond EXACTLY with one of the following strings:\n'
         + '\n'.join(responses) + '.'
     )
 
     sample = ''
     answer = ''
-    for _ in range(_MAX_MULTIPLE_CHOICE_ATTEMPTS):
+    for attempts in range(_MAX_MULTIPLE_CHOICE_ATTEMPTS):
       # Increase temperature after the first failed attempt.
-      temperature = 0.0
-      if attempts > 1:
-        temperature = 0.5
+      temperature = sampling.dynamically_adjust_temperature(
+          attempts, _MAX_MULTIPLE_CHOICE_ATTEMPTS)
 
       sample = self.sample_text(
           prompt,
           temperature=temperature,
           seed=seed,
       )
-      if len(sample) == 1:
-        # i.e. this would be a sample such as "a"
-        answer = sample
-      elif len(sample) == 2:
-        # i.e. this would be a sample such as "a)"
-        answer = sample[0]
-      else:
-        # extract a substring like "(a)" wherever it may be in a longer string
-        answer = extract_response(sample)
+      answer = sampling.extract_choice_response(sample)
       try:
         idx = responses.index(answer)
       except ValueError:
-        attempts += 1
         continue
       else:
         if self._measurements is not None:
           self._measurements.publish_datum(
               self._channel, {'choices_calls': attempts}
           )
         debug = {}
```

### Comparing `gdm-concordia-1.4.0/concordia/language_model/language_model.py` & `gdm-concordia-1.5.0/concordia/language_model/language_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/language_model/no_language_model.py` & `gdm-concordia-1.5.0/concordia/language_model/no_language_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/language_model/ollama_model.py` & `gdm-concordia-1.5.0/concordia/language_model/ollama_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,40 +8,43 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Ollama Language Model."""
+"""Ollama Language Model, a wrapper for models running on the local machine."""
 
 from collections.abc import Collection, Sequence
-import re
 
 from concordia.language_model import language_model
 from concordia.utils import measurements as measurements_lib
+from concordia.utils import sampling
 from langchain import llms
-from typing_extensions import override
 
+from typing_extensions import override
 
-def _extract_choices(text):
-  match = re.search(r"\(?(\w)\)", text)
-  if match:
-    return match.group(1)
-  return None
+_MAX_MULTIPLE_CHOICE_ATTEMPTS = 20
+_DEFAULT_TEMPERATURE = 0.5
+_DEFAULT_TERMINATORS = ()
+_DEFAULT_SYSTEM_MESSAGE = (
+    'Continue the user\'s sentences. Never repeat their starts. For example, '
+    'when you see \'Bob is\', you should continue the sentence after '
+    'the word \'is\'.'
+)
 
 
 class OllamaLanguageModel(language_model.LanguageModel):
   """Language Model that uses Ollama LLM models."""
 
   def __init__(
       self,
       model_name: str,
       *,
-      system_message: str = "",
+      system_message: str = _DEFAULT_SYSTEM_MESSAGE,
       measurements: measurements_lib.Measurements | None = None,
       channel: str = language_model.DEFAULT_STATS_CHANNEL,
   ) -> None:
     """Initializes the instance.
 
     Args:
         model_name: The language model to use. For more details, see
@@ -49,66 +52,96 @@
         system_message: System message to prefix to requests when prompting the
           model.
         measurements: The measurements object to log usage statistics to.
         channel: The channel to write the statistics to.
     """
     self._model_name = model_name
     self._system_message = system_message
+    self._terminators = []
+    if 'llama3' in self._model_name:
+      self._terminators.extend(['<|eot_id|>'])
+    self._client = llms.Ollama(model=model_name, stop=self._terminators)
+
     self._measurements = measurements
     self._channel = channel
-    self._client = llms.Ollama(model=model_name)
 
   @override
   def sample_text(
       self,
       prompt: str,
       *,
-      max_tokens: int = language_model.DEFAULT_MAX_TOKENS,
-      max_characters: int = language_model.DEFAULT_MAX_CHARACTERS,
-      terminators: Collection[str] = language_model.DEFAULT_TERMINATORS,
-      temperature: float = language_model.DEFAULT_TEMPERATURE,
-      timeout: float = language_model.DEFAULT_TIMEOUT_SECONDS,
+      max_tokens: int = -1,
+      max_characters: int = -1,
+      terminators: Collection[str] = _DEFAULT_TERMINATORS,
+      temperature: float = _DEFAULT_TEMPERATURE,
+      timeout: float = -1,
       seed: int | None = None,
   ) -> str:
-    prompt_with_system_message = f"{self._system_message}\n\n{prompt}"
+    if max_tokens != -1:
+      raise ValueError('max_tokens is not supported.')
+    if max_characters != -1:
+      raise ValueError('max_characters is not supported.')
+    if timeout != -1:
+      raise ValueError('timeout is not supported.')
+    if seed is not None:
+      raise ValueError('seed is not supported.')
+
+    del max_tokens, max_characters, timeout, seed  # Unused.
+
+    prompt_with_system_message = f'{self._system_message}\n\n{prompt}'
+
+    terminators = (self._terminators.extend(terminators)
+                   if terminators is not None else self._terminators)
 
     response = self._client(
         prompt_with_system_message,
         stop=terminators,
         temperature=temperature,
     )
 
     if self._measurements is not None:
       self._measurements.publish_datum(
-          self._channel, {"raw_text_length": len(response)}
-      )
+          self._channel,
+          {'raw_text_length': len(response)})
+
     return response
 
   @override
   def sample_choice(
       self,
       prompt: str,
       responses: Sequence[str],
       *,
       seed: int | None = None,
   ) -> tuple[int, str, dict[str, float]]:
     max_characters = len(max(responses, key=len))
-    prompt_with_system_message = f"{self._system_message}\n\n{prompt}"
-    sample = self.sample_text(
-        prompt_with_system_message,
-        max_characters=max_characters,
-        temperature=0.0,
-        seed=seed,
+    prompt_with_system_message = f'{self._system_message}\n\n{prompt}'
+    sample = ''
+    answer = ''
+    for attempts in range(_MAX_MULTIPLE_CHOICE_ATTEMPTS):
+      # Increase temperature after the first failed attempt.
+      temperature = sampling.dynamically_adjust_temperature(
+          attempts, _MAX_MULTIPLE_CHOICE_ATTEMPTS)
+
+      sample = self.sample_text(
+          prompt_with_system_message,
+          max_characters=max_characters,
+          temperature=temperature,
+          seed=seed,
+      )
+      answer = sampling.extract_choice_response(sample)
+      try:
+        idx = responses.index(answer)
+      except ValueError:
+        continue
+      else:
+        if self._measurements is not None:
+          self._measurements.publish_datum(
+              self._channel, {'choices_calls': attempts}
+          )
+        debug = {}
+        return idx, responses[idx], debug
+
+    raise language_model.InvalidResponseError(
+        (f'Too many multiple choice attempts.\nLast attempt: {sample}, ' +
+         f'extracted: {answer}')
     )
-    answer = _extract_choices(sample)
-    try:
-      idx = responses.index(answer)
-    except ValueError:
-      raise language_model.InvalidResponseError(
-          f"Invalid response: {answer}. "
-          f"LLM Input: {prompt}\nLLM Output: {sample}"
-      ) from None
-
-    if self._measurements is not None:
-      self._measurements.publish_datum(self._channel, {"choices_calls": 1})
-    debug = {}
-    return idx, responses[idx], debug
```

### Comparing `gdm-concordia-1.4.0/concordia/language_model/retry_wrapper.py` & `gdm-concordia-1.5.0/concordia/language_model/retry_wrapper.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/metrics/__init__.py` & `gdm-concordia-1.5.0/concordia/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/metrics/common_sense_morality.py` & `gdm-concordia-1.5.0/concordia/metrics/common_sense_morality.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/metrics/dass_questionnaire.py` & `gdm-concordia-1.5.0/concordia/metrics/dass_questionnaire.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/metrics/goal_achievement.py` & `gdm-concordia-1.5.0/concordia/metrics/goal_achievement.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/metrics/opinion_of_others.py` & `gdm-concordia-1.5.0/concordia/metrics/opinion_of_others.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/metrics/uncertainty_scale_question.py` & `gdm-concordia-1.5.0/concordia/metrics/uncertainty_scale_question.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/tests/__init__.py` & `gdm-concordia-1.5.0/concordia/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/tests/concordia_integration_test.py` & `gdm-concordia-1.5.0/concordia/tests/concordia_integration_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,14 @@
       timeframe_delta_until=datetime.timedelta(hours=1),
       components=[identity],
       component_name='summary of observations',
   )
 
   agent = basic_agent.BasicAgent(
       model,
-      mem,
       name,
       clock,
       [
           components.constant.ConstantComponent(
               'Instructions:', agent_instructions
           ),
           persona,
```

### Comparing `gdm-concordia-1.4.0/concordia/tests/mock_model.py` & `gdm-concordia-1.5.0/concordia/tests/mock_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/thought_chains/__init__.py` & `gdm-concordia-1.5.0/concordia/thought_chains/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/thought_chains/thought_chains.py` & `gdm-concordia-1.5.0/concordia/thought_chains/thought_chains.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/typing/__init__.py` & `gdm-concordia-1.5.0/concordia/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/typing/agent.py` & `gdm-concordia-1.5.0/concordia/typing/agent.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/typing/clock.py` & `gdm-concordia-1.5.0/concordia/typing/clock.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/typing/component.py` & `gdm-concordia-1.5.0/concordia/typing/component.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/typing/game_master.py` & `gdm-concordia-1.5.0/concordia/typing/game_master.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/typing/scene.py` & `gdm-concordia-1.5.0/concordia/typing/scene.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/utils/__init__.py` & `gdm-concordia-1.5.0/concordia/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/utils/helper_functions.py` & `gdm-concordia-1.5.0/concordia/utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/utils/html.py` & `gdm-concordia-1.5.0/concordia/utils/html.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/utils/measurements.py` & `gdm-concordia-1.5.0/concordia/utils/measurements.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/utils/measurements_test.py` & `gdm-concordia-1.5.0/concordia/utils/measurements_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/utils/plotting.py` & `gdm-concordia-1.5.0/concordia/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/concordia/utils/text.py` & `gdm-concordia-1.5.0/concordia/utils/text.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/gdm_concordia.egg-info/PKG-INFO` & `gdm-concordia-1.5.0/gdm_concordia.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdm-concordia
-Version: 1.4.0
+Version: 1.5.0
 Summary: A library for building a generative model of social interacions.
 Home-page: https://github.com/google-deepmind/concordia
 Author: DeepMind
 Author-email: noreply@google.com
 License: Apache 2.0
 Download-URL: https://github.com/google-deepmind/concordia/releases
 Keywords: multi-agent agent-based-simulation generative-agents python machine-learning
```

### Comparing `gdm-concordia-1.4.0/gdm_concordia.egg-info/SOURCES.txt` & `gdm-concordia-1.5.0/gdm_concordia.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,26 +29,31 @@
 concordia/components/agent/plan.py
 concordia/components/agent/reflection.py
 concordia/components/agent/relationships.py
 concordia/components/agent/scheduled_hint.py
 concordia/components/agent/self_perception.py
 concordia/components/agent/situation_perception.py
 concordia/components/agent/somatic_state.py
+concordia/components/agent/contrib/__init__.py
+concordia/components/agent/contrib/affect_reflection.py
+concordia/components/agent/contrib/illness_representation.py
 concordia/components/game_master/__init__.py
 concordia/components/game_master/conversation.py
 concordia/components/game_master/current_scene.py
 concordia/components/game_master/current_scene_test.py
 concordia/components/game_master/direct_effect.py
 concordia/components/game_master/inventory.py
 concordia/components/game_master/player_status.py
 concordia/components/game_master/player_status_test.py
 concordia/components/game_master/relevant_events.py
 concordia/components/game_master/schedule.py
 concordia/components/game_master/schelling_diagram_payoffs.py
 concordia/components/game_master/time_display.py
+concordia/components/game_master/contrib/__init__.py
+concordia/components/game_master/contrib/world_background_and_relevance.py
 concordia/document/__init__.py
 concordia/document/document.py
 concordia/document/document_test.py
 concordia/document/interactive_document.py
 concordia/document/interactive_document_test.py
 concordia/environment/__init__.py
 concordia/environment/game_master.py
@@ -59,14 +64,15 @@
 concordia/language_model/__init__.py
 concordia/language_model/cloud_vertex_model.py
 concordia/language_model/google_aistudio_model.py
 concordia/language_model/gpt_model.py
 concordia/language_model/language_model.py
 concordia/language_model/no_language_model.py
 concordia/language_model/ollama_model.py
+concordia/language_model/pytorch_gemma_model.py
 concordia/language_model/retry_wrapper.py
 concordia/metrics/__init__.py
 concordia/metrics/common_sense_morality.py
 concordia/metrics/dass_questionnaire.py
 concordia/metrics/goal_achievement.py
 concordia/metrics/opinion_of_others.py
 concordia/metrics/uncertainty_scale_question.py
@@ -83,13 +89,14 @@
 concordia/typing/scene.py
 concordia/utils/__init__.py
 concordia/utils/helper_functions.py
 concordia/utils/html.py
 concordia/utils/measurements.py
 concordia/utils/measurements_test.py
 concordia/utils/plotting.py
+concordia/utils/sampling.py
 concordia/utils/text.py
 gdm_concordia.egg-info/PKG-INFO
 gdm_concordia.egg-info/SOURCES.txt
 gdm_concordia.egg-info/dependency_links.txt
 gdm_concordia.egg-info/requires.txt
 gdm_concordia.egg-info/top_level.txt
```

### Comparing `gdm-concordia-1.4.0/pyproject.toml` & `gdm-concordia-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.4.0/setup.py` & `gdm-concordia-1.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """Install script for setuptools."""
 
 import setuptools
 
 setuptools.setup(
     name='gdm-concordia',
-    version='1.4.0',
+    version='1.5.0',
     license='Apache 2.0',
     license_files=['LICENSE'],
     url='https://github.com/google-deepmind/concordia',
     download_url='https://github.com/google-deepmind/concordia/releases',
     author='DeepMind',
     author_email='noreply@google.com',
     description=(
@@ -61,14 +61,15 @@
         'openai>=1.3.0',
         'pandas<=2.0.3',
         'python-dateutil',
         'reactivex',
         'retry',
         'scipy',
         'termcolor',
+        'transformers',
         'typing-extensions',
     ),
     extras_require={
         # Used in development.
         'dev': [
             'build',
             'isort',
```

