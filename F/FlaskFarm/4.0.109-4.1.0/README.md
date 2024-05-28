# Comparing `tmp/FlaskFarm-4.0.109.tar.gz` & `tmp/FlaskFarm-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlaskFarm-4.0.109.tar", last modified: Mon May 27 16:26:56 2024, max compression
+gzip compressed data, was "FlaskFarm-4.1.0.tar", last modified: Tue May 28 16:43:27 2024, max compression
```

## Comparing `FlaskFarm-4.0.109.tar` & `FlaskFarm-4.1.0.tar`

### file list

```diff
@@ -1,179 +1,178 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.777889 FlaskFarm-4.0.109/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.729889 FlaskFarm-4.0.109/FlaskFarm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/FlaskFarm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7097 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/FlaskFarm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/FlaskFarm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/FlaskFarm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/FlaskFarm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-27 16:26:56.777889 FlaskFarm-4.0.109/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.729889 FlaskFarm-4.0.109/flaskfarm/
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.729889 FlaskFarm-4.0.109/flaskfarm/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      910 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/cli/chage_ui.py
--rw-r--r--   0 root         (0) root         (0)     4087 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/cli/code_encode.log
--rw-r--r--   0 root         (0) root         (0)     1649 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/cli/code_encode.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/cli/encode.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.733889 FlaskFarm-4.0.109/flaskfarm/files/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/files/config.yaml.template
--rw-r--r--   0 root         (0) root         (0)      818 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/files/menu.yaml.template
--rw-r--r--   0 root         (0) root         (0)      514 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/files/notify.yaml.template
--rw-r--r--   0 root         (0) root         (0)      319 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/files/requirements_mini.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/files/requirements_normal.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/files/requirements_useful.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.729889 FlaskFarm-4.0.109/flaskfarm/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.733889 FlaskFarm-4.0.109/flaskfarm/lib/framework/
--rw-r--r--   0 root         (0) root         (0)      680 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3710 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/init_declare.py
--rw-r--r--   0 root         (0) root         (0)    22703 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/init_main.py
--rw-r--r--   0 root         (0) root         (0)     4481 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/init_menu.py
--rw-r--r--   0 root         (0) root         (0)    17282 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/init_plugin.py
--rw-r--r--   0 root         (0) root         (0)     4491 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/init_route.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/init_web.py
--rw-r--r--   0 root         (0) root         (0)     4588 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/log_viewer.py
--rw-r--r--   0 root         (0) root         (0)    10318 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.729889 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.733889 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/
--rw-r--r--   0 root         (0) root         (0)    57995 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/animate.min.css
--rw-r--r--   0 root         (0) root         (0)   140891 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)     2256 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/custom.css
--rw-r--r--   0 root         (0) root         (0)     2527 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/showdown.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.753889 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/
--rw-r--r--   0 root         (0) root         (0)   180115 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Cerulean_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   170032 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Cosmo_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   180336 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Cyborg_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   180001 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Darkly_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   141027 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Default_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   180322 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Flatly_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   177197 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Journal_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   181004 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Litera_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   183229 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Lumen_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   178152 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Lux_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   215695 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Materia_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   181453 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Minty_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   193200 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Morph_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   172097 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Pulse_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   183373 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Quartz_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   179079 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Sandstone_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   179819 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Simplex_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   182175 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Sketchy_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   189545 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Slate_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   189936 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Solar_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   182721 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Spacelab_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   180331 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Superhero_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   176871 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/United_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   175809 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Vapor_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   184168 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Yeti_bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   175809 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Zephyr_bootstrap.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.753889 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/file/
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/file/robots.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.753889 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/img/
--rw-r--r--   0 root         (0) root         (0)      318 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/img/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    20700 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/img/loading.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.753889 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/
--rw-r--r--   0 root         (0) root         (0)   131074 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/Sortable.js
--rw-r--r--   0 root         (0) root         (0)     8976 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/bootstrap-notify.min.js
--rw-r--r--   0 root         (0) root         (0)    50998 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/bootstrap.min.js
--rw-r--r--   0 root         (0) root         (0)     6563 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/ff_common1.js
--rw-r--r--   0 root         (0) root         (0)    19497 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/ff_global1.js
--rw-r--r--   0 root         (0) root         (0)      371 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/ff_global_plugin.js
--rw-r--r--   0 root         (0) root         (0)     7527 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/ff_ui1.js
--rw-r--r--   0 root         (0) root         (0)   790932 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/hls.js
--rw-r--r--   0 root         (0) root         (0)    21004 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/popper.min.js
--rw-r--r--   0 root         (0) root         (0)      915 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/showdown-prettify.js
--rw-r--r--   0 root         (0) root         (0)    75208 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/showdown_2.1.0.js
--rw-r--r--   0 root         (0) root         (0)     6322 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/sjva_global1.js
--rw-r--r--   0 root         (0) root         (0)     2616 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/sjva_ui14.js
--rw-r--r--   0 root         (0) root         (0)   281485 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/video.min.js
--rw-r--r--   0 root         (0) root         (0)   498279 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/videojs-contrib-hls.js
--rw-r--r--   0 root         (0) root         (0)   170306 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/videojs-contrib-hls.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.757889 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/
--rw-r--r--   0 root         (0) root         (0)     3360 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/base.html
--rw-r--r--   0 root         (0) root         (0)     2594 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/log.html
--rw-r--r--   0 root         (0) root         (0)    24500 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/macro.html
--rw-r--r--   0 root         (0) root         (0)     4474 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/macro_include.html
--rw-r--r--   0 root         (0) root         (0)     7395 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/macro_menu.html
--rw-r--r--   0 root         (0) root         (0)     1033 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/manual.html
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/manual_old.html
--rw-r--r--   0 root         (0) root         (0)      109 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/sample.html
--rw-r--r--   0 root         (0) root         (0)     1520 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/videojs.html
--rw-r--r--   0 root         (0) root         (0)     3547 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/videojs_discord.html
--rw-r--r--   0 root         (0) root         (0)     3668 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/util.py
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/framework/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.757889 FlaskFarm-4.0.109/flaskfarm/lib/plugin/
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10463 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/plugin/_ffmpeg_queue.py
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/plugin/common.py
--rw-r--r--   0 root         (0) root         (0)     3541 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/plugin/create_plugin.py
--rw-r--r--   0 root         (0) root         (0)    12172 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/plugin/logic.py
--rw-r--r--   0 root         (0) root         (0)     7991 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/plugin/logic_module_base.py
--rw-r--r--   0 root         (0) root         (0)     6675 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/plugin/model_base.py
--rw-r--r--   0 root         (0) root         (0)     5707 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/plugin/model_setting.py
--rw-r--r--   0 root         (0) root         (0)    16538 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/plugin/route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.757889 FlaskFarm-4.0.109/flaskfarm/lib/support/
--rw-r--r--   0 root         (0) root         (0)      803 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.761889 FlaskFarm-4.0.109/flaskfarm/lib/support/base/
--rw-r--r--   0 root         (0) root         (0)     2099 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/__ffmpeg.py
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/aes.py
--rw-r--r--   0 root         (0) root         (0)    13030 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/discord.py
--rw-r--r--   0 root         (0) root         (0)    11016 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/file.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/image.py
--rw-r--r--   0 root         (0) root         (0)     1511 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/os_command.py
--rw-r--r--   0 root         (0) root         (0)      887 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/slack.py
--rw-r--r--   0 root         (0) root         (0)     2267 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/string.py
--rw-r--r--   0 root         (0) root         (0)    12123 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/sub_process.py
--rw-r--r--   0 root         (0) root         (0)     2040 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/support_sc.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/telegram.py
--rw-r--r--   0 root         (0) root         (0)     3143 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/util.py
--rw-r--r--   0 root         (0) root         (0)     2049 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/base/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.761889 FlaskFarm-4.0.109/flaskfarm/lib/support/expand/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/expand/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20129 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/expand/ffmpeg.py
--rw-r--r--   0 root         (0) root         (0)      893 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/expand/ffprobe.py
--rw-r--r--   0 root         (0) root         (0)     7822 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/expand/gsheet_base.py
--rw-r--r--   0 root         (0) root         (0)     7527 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/expand/rclone.py
--rw-r--r--   0 root         (0) root         (0)     4303 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/expand/simple_selenium.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.765889 FlaskFarm-4.0.109/flaskfarm/lib/support/libsc/
--rw-r--r--   0 root         (0) root         (0)    20480 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/libsc/sc.cp310-win_amd64.pyd
--rw-r--r--   0 root         (0) root         (0)    67168 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/libsc/sc.cpython-310-aarch64-linux-gnu.so
--rwxr-xr-x   0 root         (0) root         (0)    74584 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/libsc/sc.cpython-310-x86_64-linux-gnu.so
--rw-r--r--   0 root         (0) root         (0)    70640 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/libsc/sc.cpython-310.so
--rw-r--r--   0 root         (0) root         (0)     3540 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/support/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.765889 FlaskFarm-4.0.109/flaskfarm/lib/system/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4681 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/mod_home.py
--rw-r--r--   0 root         (0) root         (0)     3475 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/mod_log.py
--rw-r--r--   0 root         (0) root         (0)     3064 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/mod_plugin.py
--rw-r--r--   0 root         (0) root         (0)     2978 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/mod_route.py
--rw-r--r--   0 root         (0) root         (0)    12714 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/mod_setting.py
--rw-r--r--   0 root         (0) root         (0)     2165 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/mod_tool.py
--rw-r--r--   0 root         (0) root         (0)    11529 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/page_command.py
--rw-r--r--   0 root         (0) root         (0)     2448 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.773889 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/
--rw-r--r--   0 root         (0) root         (0)     3800 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_all_log.html
--rw-r--r--   0 root         (0) root         (0)     7554 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_home.html
--rw-r--r--   0 root         (0) root         (0)     2242 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_login.html
--rw-r--r--   0 root         (0) root         (0)     3791 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_plugin_list.html
--rw-r--r--   0 root         (0) root         (0)      806 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_restart.html
--rw-r--r--   0 root         (0) root         (0)     1511 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_auth.html
--rw-r--r--   0 root         (0) root         (0)     2014 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_basic.html
--rw-r--r--   0 root         (0) root         (0)     2210 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_celery.html
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_config.html
--rw-r--r--   0 root         (0) root         (0)     1324 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_export.html
--rw-r--r--   0 root         (0) root         (0)      912 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_menu.html
--rw-r--r--   0 root         (0) root         (0)     5006 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_notify.html
--rw-r--r--   0 root         (0) root         (0)     1191 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_web.html
--rw-r--r--   0 root         (0) root         (0)    11465 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_tool_command.html
--rw-r--r--   0 root         (0) root         (0)     2972 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_tool_crypt.html
--rw-r--r--   0 root         (0) root         (0)     2850 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_tool_python.html
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_tool_upload.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:26:56.777889 FlaskFarm-4.0.109/flaskfarm/lib/tool/
--rw-r--r--   0 root         (0) root         (0)      169 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/tool/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20353 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/tool/fp_entity_ktv.py
--rw-r--r--   0 root         (0) root         (0)     4570 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/tool/modal_command.py
--rw-r--r--   0 root         (0) root         (0)     2839 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/tool/notify.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/lib/tool/util.py
--rw-r--r--   0 root         (0) root         (0)      661 2024-05-27 16:26:56.000000 FlaskFarm-4.0.109/flaskfarm/main.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 16:26:56.777889 FlaskFarm-4.0.109/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3420 2024-05-27 04:54:25.000000 FlaskFarm-4.0.109/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.919525 FlaskFarm-4.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.851525 FlaskFarm-4.1.0/FlaskFarm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/FlaskFarm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7067 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/FlaskFarm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/FlaskFarm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/FlaskFarm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/FlaskFarm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-28 16:43:27.919525 FlaskFarm-4.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.851525 FlaskFarm-4.1.0/flaskfarm/
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.855525 FlaskFarm-4.1.0/flaskfarm/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      910 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/cli/chage_ui.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/cli/code_encode.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/cli/encode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.867525 FlaskFarm-4.1.0/flaskfarm/files/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/files/config.yaml.template
+-rw-r--r--   0 root         (0) root         (0)      818 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/files/menu.yaml.template
+-rw-r--r--   0 root         (0) root         (0)      514 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/files/notify.yaml.template
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/files/requirements_mini.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/files/requirements_normal.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/files/requirements_useful.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.843525 FlaskFarm-4.1.0/flaskfarm/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.875525 FlaskFarm-4.1.0/flaskfarm/lib/framework/
+-rw-r--r--   0 root         (0) root         (0)      680 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/init_declare.py
+-rw-r--r--   0 root         (0) root         (0)    22703 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/init_main.py
+-rw-r--r--   0 root         (0) root         (0)     4729 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/init_menu.py
+-rw-r--r--   0 root         (0) root         (0)    17282 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/init_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     4491 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/init_route.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/init_web.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/log_viewer.py
+-rw-r--r--   0 root         (0) root         (0)    10318 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.839525 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.875525 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/
+-rw-r--r--   0 root         (0) root         (0)    57995 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/animate.min.css
+-rw-r--r--   0 root         (0) root         (0)   140891 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/custom.css
+-rw-r--r--   0 root         (0) root         (0)     2527 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/showdown.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.891525 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/
+-rw-r--r--   0 root         (0) root         (0)   180115 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Cerulean_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   170032 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Cosmo_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   180336 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Cyborg_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   180001 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Darkly_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   141027 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Default_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   180322 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Flatly_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   177197 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Journal_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   181004 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Litera_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   183229 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Lumen_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   178152 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Lux_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   215695 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Materia_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   181453 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Minty_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   193200 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Morph_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   172097 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Pulse_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   183373 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Quartz_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   179079 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Sandstone_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   179819 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Simplex_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   182175 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Sketchy_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   189545 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Slate_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   189936 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Solar_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   182721 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Spacelab_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   180331 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Superhero_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   176871 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/United_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   175809 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Vapor_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   184168 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Yeti_bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   175809 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Zephyr_bootstrap.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.891525 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/file/
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/file/robots.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.895525 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/img/
+-rw-r--r--   0 root         (0) root         (0)      318 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/img/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    20700 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/img/loading.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.903525 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/
+-rw-r--r--   0 root         (0) root         (0)   131074 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/Sortable.js
+-rw-r--r--   0 root         (0) root         (0)     8976 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/bootstrap-notify.min.js
+-rw-r--r--   0 root         (0) root         (0)    50998 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/bootstrap.min.js
+-rw-r--r--   0 root         (0) root         (0)     6563 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/ff_common1.js
+-rw-r--r--   0 root         (0) root         (0)    19497 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/ff_global1.js
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/ff_global_plugin.js
+-rw-r--r--   0 root         (0) root         (0)     7527 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/ff_ui1.js
+-rw-r--r--   0 root         (0) root         (0)   790932 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/hls.js
+-rw-r--r--   0 root         (0) root         (0)    21004 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/popper.min.js
+-rw-r--r--   0 root         (0) root         (0)      915 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/showdown-prettify.js
+-rw-r--r--   0 root         (0) root         (0)    75208 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/showdown_2.1.0.js
+-rw-r--r--   0 root         (0) root         (0)     6322 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/sjva_global1.js
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/sjva_ui14.js
+-rw-r--r--   0 root         (0) root         (0)   281485 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/video.min.js
+-rw-r--r--   0 root         (0) root         (0)   498279 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/videojs-contrib-hls.js
+-rw-r--r--   0 root         (0) root         (0)   170306 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/videojs-contrib-hls.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.907525 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/
+-rw-r--r--   0 root         (0) root         (0)     3360 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     2594 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/log.html
+-rw-r--r--   0 root         (0) root         (0)    24500 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/macro.html
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/macro_include.html
+-rw-r--r--   0 root         (0) root         (0)     7548 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/macro_menu.html
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/manual.html
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/manual_old.html
+-rw-r--r--   0 root         (0) root         (0)      109 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/sample.html
+-rw-r--r--   0 root         (0) root         (0)     1520 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/videojs.html
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/videojs_discord.html
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/util.py
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/framework/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.907525 FlaskFarm-4.1.0/flaskfarm/lib/plugin/
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/plugin/_ffmpeg_queue.py
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/plugin/common.py
+-rw-r--r--   0 root         (0) root         (0)     3541 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/plugin/create_plugin.py
+-rw-r--r--   0 root         (0) root         (0)    12172 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/plugin/logic.py
+-rw-r--r--   0 root         (0) root         (0)     7991 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/plugin/logic_module_base.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/plugin/model_base.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/plugin/model_setting.py
+-rw-r--r--   0 root         (0) root         (0)    16538 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/plugin/route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.907525 FlaskFarm-4.1.0/flaskfarm/lib/support/
+-rw-r--r--   0 root         (0) root         (0)      803 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.911525 FlaskFarm-4.1.0/flaskfarm/lib/support/base/
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/__ffmpeg.py
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/aes.py
+-rw-r--r--   0 root         (0) root         (0)    13030 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/discord.py
+-rw-r--r--   0 root         (0) root         (0)    11016 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/file.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/image.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/os_command.py
+-rw-r--r--   0 root         (0) root         (0)      887 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/slack.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/string.py
+-rw-r--r--   0 root         (0) root         (0)    12123 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/sub_process.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/support_sc.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/telegram.py
+-rw-r--r--   0 root         (0) root         (0)     3143 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/util.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/base/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.911525 FlaskFarm-4.1.0/flaskfarm/lib/support/expand/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/expand/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20129 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/expand/ffmpeg.py
+-rw-r--r--   0 root         (0) root         (0)      893 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/expand/ffprobe.py
+-rw-r--r--   0 root         (0) root         (0)     7822 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/expand/gsheet_base.py
+-rw-r--r--   0 root         (0) root         (0)     7527 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/expand/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4303 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/expand/simple_selenium.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.911525 FlaskFarm-4.1.0/flaskfarm/lib/support/libsc/
+-rw-r--r--   0 root         (0) root         (0)    20480 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/libsc/sc.cp310-win_amd64.pyd
+-rw-r--r--   0 root         (0) root         (0)    67168 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/libsc/sc.cpython-310-aarch64-linux-gnu.so
+-rwxr-xr-x   0 root         (0) root         (0)    74584 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/libsc/sc.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0 root         (0) root         (0)    70640 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/libsc/sc.cpython-310.so
+-rw-r--r--   0 root         (0) root         (0)     3540 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/support/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.911525 FlaskFarm-4.1.0/flaskfarm/lib/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/mod_home.py
+-rw-r--r--   0 root         (0) root         (0)     3475 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/mod_log.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/mod_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/mod_route.py
+-rw-r--r--   0 root         (0) root         (0)    12714 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/mod_setting.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/mod_tool.py
+-rw-r--r--   0 root         (0) root         (0)    11529 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/page_command.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.915525 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/
+-rw-r--r--   0 root         (0) root         (0)     3800 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_all_log.html
+-rw-r--r--   0 root         (0) root         (0)     7554 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_home.html
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_login.html
+-rw-r--r--   0 root         (0) root         (0)     3791 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_plugin_list.html
+-rw-r--r--   0 root         (0) root         (0)      806 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_restart.html
+-rw-r--r--   0 root         (0) root         (0)     1511 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_auth.html
+-rw-r--r--   0 root         (0) root         (0)     2014 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_basic.html
+-rw-r--r--   0 root         (0) root         (0)     2210 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_celery.html
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_config.html
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_export.html
+-rw-r--r--   0 root         (0) root         (0)      912 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_menu.html
+-rw-r--r--   0 root         (0) root         (0)     5006 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_notify.html
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_web.html
+-rw-r--r--   0 root         (0) root         (0)    11465 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_tool_command.html
+-rw-r--r--   0 root         (0) root         (0)     2972 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_tool_crypt.html
+-rw-r--r--   0 root         (0) root         (0)     2850 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_tool_python.html
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_tool_upload.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:43:27.919525 FlaskFarm-4.1.0/flaskfarm/lib/tool/
+-rw-r--r--   0 root         (0) root         (0)      169 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/tool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20353 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/tool/fp_entity_ktv.py
+-rw-r--r--   0 root         (0) root         (0)     4570 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/tool/modal_command.py
+-rw-r--r--   0 root         (0) root         (0)     2839 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/tool/notify.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/lib/tool/util.py
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-28 16:43:27.000000 FlaskFarm-4.1.0/flaskfarm/main.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 16:43:27.919525 FlaskFarm-4.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3420 2024-05-27 04:54:25.000000 FlaskFarm-4.1.0/setup.py
```

### Comparing `FlaskFarm-4.0.109/FlaskFarm.egg-info/SOURCES.txt` & `FlaskFarm-4.1.0/FlaskFarm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 FlaskFarm.egg-info/dependency_links.txt
 FlaskFarm.egg-info/requires.txt
 FlaskFarm.egg-info/top_level.txt
 flaskfarm/__init__.py
 flaskfarm/main.py
 flaskfarm/cli/__init__.py
 flaskfarm/cli/chage_ui.py
-flaskfarm/cli/code_encode.log
 flaskfarm/cli/code_encode.py
 flaskfarm/cli/encode.py
 flaskfarm/files/config.yaml.template
 flaskfarm/files/menu.yaml.template
 flaskfarm/files/notify.yaml.template
 flaskfarm/files/requirements_mini.txt
 flaskfarm/files/requirements_normal.txt
```

### Comparing `FlaskFarm-4.0.109/flaskfarm/cli/chage_ui.py` & `FlaskFarm-4.1.0/flaskfarm/cli/chage_ui.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/cli/code_encode.py` & `FlaskFarm-4.1.0/flaskfarm/cli/code_encode.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/cli/encode.py` & `FlaskFarm-4.1.0/flaskfarm/cli/encode.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/files/config.yaml.template` & `FlaskFarm-4.1.0/flaskfarm/files/config.yaml.template`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/files/menu.yaml.template` & `FlaskFarm-4.1.0/flaskfarm/files/menu.yaml.template`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/files/notify.yaml.template` & `FlaskFarm-4.1.0/flaskfarm/files/notify.yaml.template`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/__init__.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/init_declare.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/init_declare.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/init_main.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/init_main.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/init_menu.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/init_menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,7 +107,15 @@
         #F.logger.warning(d(cls.menu_map))
 
 
     @classmethod
     def get_menu_map(cls):
         #F.logger.warning(d(cls.menu_map))
         return cls.menu_map
+
+    @classmethod
+    def is_expand_setting(cls, uri):
+        from .init_plugin import PluginManager
+        for tmp in PluginManager.setting_menus:
+            if tmp['uri'].split('/',1)[0] == uri:
+                return True
+        return False
```

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/init_plugin.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/init_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                 try:
                     mod_menu = getattr(entity['P'], 'menu')
                     if mod_menu and cls.all_package_list[key]['loading'] != False:
                         cls.plugin_menus[key]=  {'menu':mod_menu, 'match':False}
 
                     setting_menu = getattr(entity['P'], 'setting_menu')
                     if setting_menu != None and cls.all_package_list[key]['loading'] != False:
-                        F.logger.info(f"메뉴 포함 : {key}")
+                        F.logger.info(f"확장 설정 : {key}")
                         cls.setting_menus.append(setting_menu)
                 except Exception as exception:
                     F.logger.debug('no menu')
             F.logger.debug('### plugin_load threading all start.. : %s ', len(cls.plugin_list))
             # 모든 모듈을 로드한 이후에 app 등록, table 생성, start
 
         except Exception as e:
```

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/init_route.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/init_route.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/init_web.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/init_web.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,17 +48,19 @@
 
 def jinja_initialize(app):
     #from .init_menu import get_menu_map, get_plugin_menu
     from .init_menu import MenuManager
     app.jinja_env.globals.update(get_menu=get_menu)
     app.jinja_env.globals.update(get_theme=get_theme)
     app.jinja_env.globals.update(get_menu_map=MenuManager.get_menu_map)
+    app.jinja_env.globals.update(is_expand_setting=MenuManager.is_expand_setting)
     app.jinja_env.globals.update(get_web_title=get_web_title)
     app.jinja_env.globals.update(dropzone=F.dropzone)
 
     app.jinja_env.filters['get_menu'] = get_menu
     app.jinja_env.filters['get_theme'] = get_theme
     app.jinja_env.filters['get_menu_map'] = MenuManager.get_menu_map
+    app.jinja_env.filters['is_expand_setting'] = MenuManager.is_expand_setting
     app.jinja_env.filters['get_web_title'] = get_web_title
 
     app.jinja_env.auto_reload = True
     app.jinja_env.add_extension('jinja2.ext.loopcontrols')
```

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/log_viewer.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/log_viewer.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/scheduler.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/scheduler.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/animate.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/animate.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/custom.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/showdown.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/showdown.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Cerulean_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Cerulean_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Cosmo_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Cosmo_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Cyborg_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Cyborg_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Darkly_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Darkly_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Default_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Default_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Flatly_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Flatly_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Journal_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Journal_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Litera_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Litera_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Lumen_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Lumen_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Lux_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Lux_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Materia_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Materia_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Minty_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Minty_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Morph_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Morph_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Pulse_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Pulse_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Quartz_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Quartz_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Sandstone_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Sandstone_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Simplex_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Simplex_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Sketchy_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Sketchy_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Slate_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Slate_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Solar_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Solar_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Spacelab_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Spacelab_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Superhero_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Superhero_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/United_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/United_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Vapor_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Vapor_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Yeti_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Yeti_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/css/theme/Zephyr_bootstrap.min.css` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/css/theme/Zephyr_bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/img/loading.gif` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/Sortable.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/Sortable.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/bootstrap-notify.min.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/bootstrap-notify.min.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/bootstrap.min.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/ff_common1.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/ff_common1.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/ff_global1.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/ff_global1.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/ff_ui1.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/ff_ui1.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/hls.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/hls.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/popper.min.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/showdown-prettify.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/showdown-prettify.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/showdown_2.1.0.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/showdown_2.1.0.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/sjva_global1.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/sjva_global1.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/sjva_ui14.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/sjva_ui14.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/video.min.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/video.min.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/videojs-contrib-hls.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/videojs-contrib-hls.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/static/js/videojs-contrib-hls.min.js` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/static/js/videojs-contrib-hls.min.js`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/base.html` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/base.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/log.html` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/log.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/macro.html` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/macro.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/macro_include.html` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/macro_include.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/macro_menu.html` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/macro_menu.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,40 +22,42 @@
         <li class="nav-item"> <a class="nav-link" href="/{{ category['uri']}}">{{category['name']}}</a></li>
       {% else %}
         <!--{{ category }}-->
         <li class="nav-item dropdown">
           <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">{{category['name']}}</a>
           <ul class="dropdown-menu">
           {% for category_child in category['list'] %}
-            {% if category_child['uri'] == 'setting' %}
-              <li><a class="dropdown-item" href="#" style="font-size: .850rem; font-weight:bold">{{category_child['name']}}</a>
-                <ul class="submenu dropdown-menu">
-                {% for item in category_child['list'] %}
-                  <li><a class="dropdown-item" href="/{{item['uri']}}" style="font-size: .850rem; font-weight:bold">{{item['name']}}</a></li>
-                {% endfor %}
-                </ul>
-              </li>
-            {% elif category_child['uri'] == '-' %}
-              <div class="dropdown-divider"></div>
-            {% elif 'uri' in category_child and category_child['uri'].startswith('http') %}
-              {% if 'target' not in category_child or  category_child['target'] == '_blank' %}
-                <a class="dropdown-item" href="{{ category_child['uri'] }}" target="_blank" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
-              {% else %}
-              <a class="dropdown-item" href="{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
-              {% endif %}
-            {% elif 'uri' in category_child and category_child['uri'].startswith('javascript') %}
-              <a class="dropdown-item" href="{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
-            {% else %}
-              {% if category_child['uri'] == menu[0] %}
-                <a class="dropdown-item active" href="/{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
+            {% if is_expand_setting(category_child['uri']) == False %}
+              {% if category_child['uri'] == 'setting' %}
+                <li><a class="dropdown-item" href="#" style="font-size: .850rem; font-weight:bold">{{category_child['name']}}</a>
+                  <ul class="submenu dropdown-menu">
+                  {% for item in category_child['list'] %}
+                    <li><a class="dropdown-item" href="/{{item['uri']}}" style="font-size: .850rem; font-weight:bold">{{item['name']}}</a></li>
+                  {% endfor %}
+                  </ul>
+                </li>
+              {% elif category_child['uri'] == '-' %}
+                <div class="dropdown-divider"></div>
+              {% elif 'uri' in category_child and category_child['uri'].startswith('http') %}
+                {% if 'target' not in category_child or  category_child['target'] == '_blank' %}
+                  <a class="dropdown-item" href="{{ category_child['uri'] }}" target="_blank" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
+                {% else %}
+                <a class="dropdown-item" href="{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
+                {% endif %}
+              {% elif 'uri' in category_child and category_child['uri'].startswith('javascript') %}
+                <a class="dropdown-item" href="{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
               {% else %}
-                {% if 'target' in category_child %}
-                  <a class="dropdown-item" href="/{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold" target="{{category_child['target']}}">{{ category_child['name'] }}</a>
+                {% if category_child['uri'] == menu[0] %}
+                  <a class="dropdown-item active" href="/{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
                 {% else %}
-                  <a class="dropdown-item" href="/{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
+                  {% if 'target' in category_child %}
+                    <a class="dropdown-item" href="/{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold" target="{{category_child['target']}}">{{ category_child['name'] }}</a>
+                  {% else %}
+                    <a class="dropdown-item" href="/{{ category_child['uri'] }}" style="font-size: .850rem; font-weight:bold">{{ category_child['name'] }}</a>
+                  {% endif %}
                 {% endif %}
               {% endif %}
             {% endif %}
           {% endfor %} 
           </ul>
         </li> 
       {% endif %}
```

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/manual.html` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/manual.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/videojs.html` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/videojs.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/templates/videojs_discord.html` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/templates/videojs_discord.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/framework/util.py` & `FlaskFarm-4.1.0/flaskfarm/lib/framework/util.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/plugin/__init__.py` & `FlaskFarm-4.1.0/flaskfarm/lib/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/plugin/_ffmpeg_queue.py` & `FlaskFarm-4.1.0/flaskfarm/lib/plugin/_ffmpeg_queue.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/plugin/create_plugin.py` & `FlaskFarm-4.1.0/flaskfarm/lib/plugin/create_plugin.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/plugin/logic.py` & `FlaskFarm-4.1.0/flaskfarm/lib/plugin/logic.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/plugin/logic_module_base.py` & `FlaskFarm-4.1.0/flaskfarm/lib/plugin/logic_module_base.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/plugin/model_base.py` & `FlaskFarm-4.1.0/flaskfarm/lib/plugin/model_base.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/plugin/model_setting.py` & `FlaskFarm-4.1.0/flaskfarm/lib/plugin/model_setting.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/plugin/route.py` & `FlaskFarm-4.1.0/flaskfarm/lib/plugin/route.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/__init__.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/__init__.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/__ffmpeg.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/__ffmpeg.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/aes.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/aes.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/discord.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/discord.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/file.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/file.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/image.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/image.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/os_command.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/os_command.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/slack.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/slack.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/string.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/string.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/sub_process.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/sub_process.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/support_sc.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/support_sc.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/telegram.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/telegram.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/util.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/util.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/base/yaml.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/base/yaml.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/expand/ffmpeg.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/expand/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/expand/ffprobe.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/expand/ffprobe.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/expand/gsheet_base.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/expand/gsheet_base.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/expand/rclone.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/expand/rclone.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/expand/simple_selenium.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/expand/simple_selenium.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/libsc/sc.cpython-310-aarch64-linux-gnu.so` & `FlaskFarm-4.1.0/flaskfarm/lib/support/libsc/sc.cpython-310-aarch64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/libsc/sc.cpython-310-x86_64-linux-gnu.so` & `FlaskFarm-4.1.0/flaskfarm/lib/support/libsc/sc.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/libsc/sc.cpython-310.so` & `FlaskFarm-4.1.0/flaskfarm/lib/support/libsc/sc.cpython-310.so`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/support/logger.py` & `FlaskFarm-4.1.0/flaskfarm/lib/support/logger.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/mod_home.py` & `FlaskFarm-4.1.0/flaskfarm/lib/system/mod_home.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/mod_log.py` & `FlaskFarm-4.1.0/flaskfarm/lib/system/mod_log.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/mod_plugin.py` & `FlaskFarm-4.1.0/flaskfarm/lib/system/mod_plugin.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/mod_route.py` & `FlaskFarm-4.1.0/flaskfarm/lib/system/mod_route.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/mod_setting.py` & `FlaskFarm-4.1.0/flaskfarm/lib/system/mod_setting.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/mod_tool.py` & `FlaskFarm-4.1.0/flaskfarm/lib/system/mod_tool.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/page_command.py` & `FlaskFarm-4.1.0/flaskfarm/lib/system/page_command.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/setup.py` & `FlaskFarm-4.1.0/flaskfarm/lib/system/setup.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_all_log.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_all_log.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_home.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_home.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_login.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_login.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_plugin_list.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_plugin_list.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_restart.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_restart.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_auth.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_auth.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_basic.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_basic.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_celery.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_celery.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_config.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_config.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_export.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_export.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_menu.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_menu.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_notify.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_notify.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_setting_web.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_setting_web.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_tool_command.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_tool_command.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_tool_crypt.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_tool_crypt.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_tool_python.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_tool_python.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/system/templates/system_tool_upload.html` & `FlaskFarm-4.1.0/flaskfarm/lib/system/templates/system_tool_upload.html`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/tool/fp_entity_ktv.py` & `FlaskFarm-4.1.0/flaskfarm/lib/tool/fp_entity_ktv.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/tool/modal_command.py` & `FlaskFarm-4.1.0/flaskfarm/lib/tool/modal_command.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/tool/notify.py` & `FlaskFarm-4.1.0/flaskfarm/lib/tool/notify.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/lib/tool/util.py` & `FlaskFarm-4.1.0/flaskfarm/lib/tool/util.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/flaskfarm/main.py` & `FlaskFarm-4.1.0/flaskfarm/main.py`

 * *Files identical despite different names*

### Comparing `FlaskFarm-4.0.109/setup.py` & `FlaskFarm-4.1.0/setup.py`

 * *Files identical despite different names*

