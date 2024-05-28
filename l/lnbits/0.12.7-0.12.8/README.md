# Comparing `tmp/lnbits-0.12.7.tar.gz` & `tmp/lnbits-0.12.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnbits-0.12.7.tar", max compression
+gzip compressed data, was "lnbits-0.12.8.tar", max compression
```

## Comparing `lnbits-0.12.7.tar` & `lnbits-0.12.8.tar`

### file list

```diff
@@ -1,206 +1,206 @@
--rw-r--r--   0        0        0     1060 2024-05-22 09:10:58.845615 lnbits-0.12.7/LICENSE
--rw-r--r--   0        0        0     4154 2024-05-22 09:10:58.845615 lnbits-0.12.7/README.md
--rw-r--r--   0        0        0        0 2024-05-22 09:10:58.845615 lnbits-0.12.7/lnbits/__init__.py
--rw-r--r--   0        0        0       48 2024-05-22 09:10:58.845615 lnbits-0.12.7/lnbits/__main__.py
--rw-r--r--   0        0        0    13866 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/app.py
--rw-r--r--   0        0        0      135 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/bolt11.py
--rw-r--r--   0        0        0    23130 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/commands.py
--rw-r--r--   0        0        0     1483 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/__init__.py
--rw-r--r--   0        0        0    36141 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/crud.py
--rw-r--r--   0        0        0      148 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/db.py
--rw-r--r--   0        0        0     4355 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/helpers.py
--rw-r--r--   0        0        0    15292 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/migrations.py
--rw-r--r--   0        0        0    12136 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/models.py
--rw-r--r--   0        0        0    28061 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/services.py
--rw-r--r--   0        0        0     1156 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/sso/keycloak.py
--rw-r--r--   0        0        0     5918 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/tasks.py
--rw-r--r--   0        0        0     3030 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/admin/_tab_funding.html
--rw-r--r--   0        0        0    12921 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/admin/_tab_security.html
--rw-r--r--   0        0        0     2187 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/admin/_tab_security_notifications.html
--rw-r--r--   0        0        0     6048 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/admin/_tab_server.html
--rw-r--r--   0        0        0     4766 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/admin/_tab_theme.html
--rw-r--r--   0        0        0     2238 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/admin/_tab_users.html
--rw-r--r--   0        0        0     2951 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/admin/index.html
--rw-r--r--   0        0        0     5530 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/core/_api_docs.html
--rw-r--r--   0        0        0    17024 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/core/account.html
--rw-r--r--   0        0        0    33218 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/core/extensions.html
--rw-r--r--   0        0        0     4037 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/core/first_install.html
--rw-r--r--   0        0        0    18777 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/core/index.html
--rw-r--r--   0        0        0    25092 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/core/wallet.html
--rw-r--r--   0        0        0    10041 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/node/_tab_channels.html
--rw-r--r--   0        0        0     2435 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/node/_tab_dashboard.html
--rw-r--r--   0        0        0    12171 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/node/_tab_transactions.html
--rw-r--r--   0        0        0    10706 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/node/index.html
--rw-r--r--   0        0        0     3719 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/node/public.html
--rw-r--r--   0        0        0     2429 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/service-worker.js
--rw-r--r--   0        0        0      716 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/users/_createUserDialog.html
--rw-r--r--   0        0        0      724 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/users/_createWalletDialog.html
--rw-r--r--   0        0        0     1088 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/users/_topupDialog.html
--rw-r--r--   0        0        0     3328 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/users/_walletDialog.html
--rw-r--r--   0        0        0     4005 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/templates/users/index.html
--rw-r--r--   0        0        0        0 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/__init__.py
--rw-r--r--   0        0        0     3826 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/admin_api.py
--rw-r--r--   0        0        0     8151 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/api.py
--rw-r--r--   0        0        0    12341 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/auth_api.py
--rw-r--r--   0        0        0     8743 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/extension_api.py
--rw-r--r--   0        0        0    14781 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/generic.py
--rw-r--r--   0        0        0     5896 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/node_api.py
--rw-r--r--   0        0        0    15146 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/payment_api.py
--rw-r--r--   0        0        0     1724 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/public_api.py
--rw-r--r--   0        0        0     2845 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/tinyurl_api.py
--rw-r--r--   0        0        0     5275 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/user_api.py
--rw-r--r--   0        0        0     1894 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/wallet_api.py
--rw-r--r--   0        0        0     1568 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/webpush_api.py
--rw-r--r--   0        0        0     1131 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/core/views/websocket_api.py
--rw-r--r--   0        0        0    15893 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/db.py
--rw-r--r--   0        0        0     8132 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/decorators.py
--rw-r--r--   0        0        0     3574 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/exceptions.py
--rw-r--r--   0        0        0    23809 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/extension_manager.py
--rw-r--r--   0        0        0     8177 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/helpers.py
--rw-r--r--   0        0        0     1073 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/jinja2_templating.py
--rw-r--r--   0        0        0       75 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/lnurl.py
--rw-r--r--   0        0        0     8386 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/middleware.py
--rw-r--r--   0        0        0      206 2024-05-22 09:10:58.849615 lnbits-0.12.7/lnbits/nodes/__init__.py
--rw-r--r--   0        0        0     5561 2024-05-22 09:10:58.853615 lnbits-0.12.7/lnbits/nodes/base.py
--rw-r--r--   0        0        0    11840 2024-05-22 09:10:58.853615 lnbits-0.12.7/lnbits/nodes/cln.py
--rw-r--r--   0        0        0    13247 2024-05-22 09:10:58.853615 lnbits-0.12.7/lnbits/nodes/lndrest.py
--rw-r--r--   0        0        0       26 2024-05-22 09:10:58.853615 lnbits-0.12.7/lnbits/py.typed
--rw-r--r--   0        0        0      198 2024-05-22 09:10:58.853615 lnbits-0.12.7/lnbits/requestvars.py
--rw-r--r--   0        0        0     2415 2024-05-22 09:10:58.853615 lnbits-0.12.7/lnbits/server.py
--rw-r--r--   0        0        0    18915 2024-05-22 09:10:58.853615 lnbits-0.12.7/lnbits/settings.py
--rw-r--r--   0        0        0   209450 2024-05-22 09:10:58.853615 lnbits-0.12.7/lnbits/static/bundle.min.css
--rw-r--r--   0        0        0  1599776 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/bundle.min.js
--rw-r--r--   0        0        0    12767 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/css/base.css
--rw-r--r--   0        0        0     4286 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/favicon.ico
--rw-r--r--   0        0        0   104948 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/fonts/material-icons-v50.woff2
--rw-r--r--   0        0        0    12057 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/br.js
--rw-r--r--   0        0        0    10482 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/cn.js
--rw-r--r--   0        0        0    11898 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/cs.js
--rw-r--r--   0        0        0    12422 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/de.js
--rw-r--r--   0        0        0    11082 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/en.js
--rw-r--r--   0        0        0    12374 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/es.js
--rw-r--r--   0        0        0    12462 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/fi.js
--rw-r--r--   0        0        0    12901 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/fr.js
--rw-r--r--   0        0        0       25 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/i18n.js
--rw-r--r--   0        0        0    12255 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/it.js
--rw-r--r--   0        0        0    13880 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/jp.js
--rw-r--r--   0        0        0    13119 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/kr.js
--rw-r--r--   0        0        0    11993 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/nl.js
--rw-r--r--   0        0        0    12372 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/pi.js
--rw-r--r--   0        0        0    12006 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/pl.js
--rw-r--r--   0        0        0    12015 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/pt.js
--rw-r--r--   0        0        0    12059 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/sk.js
--rw-r--r--   0        0        0    11470 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/i18n/we.js
--rw-r--r--   0        0        0     1620 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/images/alby.png
--rw-r--r--   0        0        0     1620 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/images/albyl.png
--rw-r--r--   0        0        0    16651 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/images/bitcoin-hardware-wallet.png
--rw-r--r--   0        0        0    56349 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/images/bitcoin-shop-banner.png
--rw-r--r--   0        0        0     3493 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/images/blitz.png
--rw-r--r--   0        0        0    13998 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/images/blitzl.png
--rw-r--r--   0        0        0     2465 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/images/cln.png
--rw-r--r--   0        0        0    12787 2024-05-22 09:10:58.861615 lnbits-0.12.7/lnbits/static/images/clnl.png
--rw-r--r--   0        0        0   181365 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/default_voucher.png
--rw-r--r--   0        0        0     1692 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/github-logo.png
--rw-r--r--   0        0        0      982 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/google-logo.png
--rw-r--r--   0        0        0     1887 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/keycloak-logo.png
--rw-r--r--   0        0        0    11564 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/lnbits-shop-dark.png
--rw-r--r--   0        0        0    13698 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/lnbits-shop-light.png
--rw-r--r--   0        0        0     2290 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/lnd.png
--rw-r--r--   0        0        0     3587 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/lnpay.png
--rw-r--r--   0        0        0    12415 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/lnpayl.png
--rw-r--r--   0        0        0    14906 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/logos/lnbits.png
--rw-r--r--   0        0        0      290 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/logos/lnbits.svg
--rw-r--r--   0        0        0    15727 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/maskable_icon.png
--rw-r--r--   0        0        0     2383 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/maskable_icon_x192.png
--rw-r--r--   0        0        0     6144 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/maskable_icon_x512.png
--rw-r--r--   0        0        0     1231 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/maskable_icon_x96.png
--rw-r--r--   0        0        0    13511 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/mynode.png
--rw-r--r--   0        0        0     8846 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/mynodel.png
--rw-r--r--   0        0        0    15961 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/open-sats.png
--rw-r--r--   0        0        0     3551 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/opennode.png
--rw-r--r--   0        0        0    14197 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/opennodel.png
--rw-r--r--   0        0        0     7751 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/phoenixd.png
--rw-r--r--   0        0        0     4592 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/phoenixdl.png
--rw-r--r--   0        0        0    98187 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/screenshot_desktop.png
--rw-r--r--   0        0        0   120332 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/screenshot_phone.png
--rw-r--r--   0        0        0     4401 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/spark.png
--rw-r--r--   0        0        0    15565 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/sparkl.png
--rw-r--r--   0        0        0     1233 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/start9.png
--rw-r--r--   0        0        0     1233 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/start9l.png
--rw-r--r--   0        0        0     3065 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/templatead.png
--rw-r--r--   0        0        0     3503 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/umbrel.png
--rw-r--r--   0        0        0    15335 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/umbrell.png
--rw-r--r--   0        0        0     2522 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/voltage.png
--rw-r--r--   0        0        0     2584 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/voltagel.png
--rw-r--r--   0        0        0      985 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/voucher_template.svg
--rw-r--r--   0        0        0     1937 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/zbd.png
--rw-r--r--   0        0        0     2003 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/images/zbdl.png
--rw-r--r--   0        0        0     3172 2024-05-22 09:10:58.865615 lnbits-0.12.7/lnbits/static/js/account.js
--rw-r--r--   0        0        0     8674 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/admin.js
--rw-r--r--   0        0        0    16664 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/base.js
--rw-r--r--   0        0        0     9730 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/bolt11-decoder.js
--rw-r--r--   0        0        0     2732 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/components/extension-settings.js
--rw-r--r--   0        0        0     4887 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/components/lnbits-funding-sources.js
--rw-r--r--   0        0        0     4087 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/components/payment-chart.js
--rw-r--r--   0        0        0    13203 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/components/payment-list.js
--rw-r--r--   0        0        0    23863 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/components.js
--rw-r--r--   0        0        0    16879 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/event-reactions.js
--rw-r--r--   0        0        0     2494 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/index.js
--rw-r--r--   0        0        0     6824 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/node.js
--rw-r--r--   0        0        0     9661 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/users.js
--rw-r--r--   0        0        0    18977 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/js/wallet.js
--rw-r--r--   0        0        0     4419 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/scss/base.scss
--rwxr-xr-x   0        0        0   593984 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/vendor/Chart.bundle.js
--rwxr-xr-x   0        0        0      858 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/vendor/Chart.css
--rw-r--r--   0        0        0   372118 2024-05-22 09:10:58.873615 lnbits-0.12.7/lnbits/static/vendor/VueQrcodeReader.umd.js
--rw-r--r--   0        0        0    97321 2024-05-22 09:10:58.873615 lnbits-0.12.7/lnbits/static/vendor/axios.js
--rw-r--r--   0        0        0   174604 2024-05-22 09:10:58.873615 lnbits-0.12.7/lnbits/static/vendor/moment.js
--rw-r--r--   0        0        0   242385 2024-05-22 09:10:58.873615 lnbits-0.12.7/lnbits/static/vendor/quasar.css
--rw-r--r--   0        0        0     9375 2024-05-22 09:10:58.873615 lnbits-0.12.7/lnbits/static/vendor/quasar.ie.polyfills.umd.min.js
--rw-r--r--   0        0        0  1066966 2024-05-22 09:10:58.877615 lnbits-0.12.7/lnbits/static/vendor/quasar.umd.js
--rw-r--r--   0        0        0   159755 2024-05-22 09:10:58.877615 lnbits-0.12.7/lnbits/static/vendor/showdown.js
--rw-r--r--   0        0        0    68416 2024-05-22 09:10:58.877615 lnbits-0.12.7/lnbits/static/vendor/underscore.js
--rw-r--r--   0        0        0    68299 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/static/vendor/vue-i18n.js
--rw-r--r--   0        0        0   157254 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/static/vendor/vue-qrcode.js
--rw-r--r--   0        0        0    84010 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/static/vendor/vue-router.js
--rw-r--r--   0        0        0   342147 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/static/vendor/vue.js
--rw-r--r--   0        0        0    38178 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/static/vendor/vuex.js
--rw-r--r--   0        0        0     1077 2024-05-22 09:10:58.869615 lnbits-0.12.7/lnbits/static/vendor.json
--rw-r--r--   0        0        0     6972 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/tasks.py
--rw-r--r--   0        0        0     9396 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/templates/base.html
--rw-r--r--   0        0        0     1476 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/templates/error.html
--rw-r--r--   0        0        0      406 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/templates/macros.jinja
--rw-r--r--   0        0        0     1194 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/templates/print.html
--rw-r--r--   0        0        0      635 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/templates/public.html
--rw-r--r--   0        0        0        0 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/utils/__init__.py
--rw-r--r--   0        0        0     1914 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/utils/cache.py
--rw-r--r--   0        0        0     2510 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/utils/crypto.py
--rw-r--r--   0        0        0     9000 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/utils/exchange_rates.py
--rw-r--r--   0        0        0     3990 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/utils/logger.py
--rw-r--r--   0        0        0     1568 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/wallets/__init__.py
--rw-r--r--   0        0        0     6870 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/wallets/alby.py
--rw-r--r--   0        0        0     3406 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/wallets/base.py
--rw-r--r--   0        0        0     6397 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/wallets/cliche.py
--rw-r--r--   0        0        0    10608 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/wallets/corelightning.py
--rw-r--r--   0        0        0    12191 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/wallets/corelightningrest.py
--rw-r--r--   0        0        0     8388 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/wallets/eclair.py
--rw-r--r--   0        0        0     4020 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/wallets/fake.py
--rw-r--r--   0        0        0     8516 2024-05-22 09:10:58.881615 lnbits-0.12.7/lnbits/wallets/lnbits.py
--rw-r--r--   0        0        0        0 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/lnd_grpc_files/__init__.py
--rw-r--r--   0        0        0   181468 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/lnd_grpc_files/lightning_pb2.py
--rw-r--r--   0        0        0   124188 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/lnd_grpc_files/lightning_pb2_grpc.py
--rw-r--r--   0        0        0    35071 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/lnd_grpc_files/router_pb2.py
--rw-r--r--   0        0        0    31107 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/lnd_grpc_files/router_pb2_grpc.py
--rw-r--r--   0        0        0     9951 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/lndgrpc.py
--rw-r--r--   0        0        0    10879 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/lndrest.py
--rw-r--r--   0        0        0     4764 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/lnpay.py
--rw-r--r--   0        0        0     6001 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/lntips.py
--rw-r--r--   0        0        0       36 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/macaroon/__init__.py
--rw-r--r--   0        0        0     1345 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/macaroon/macaroon.py
--rw-r--r--   0        0        0     4688 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/opennode.py
--rw-r--r--   0        0        0     8363 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/phoenixd.py
--rw-r--r--   0        0        0     9038 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/spark.py
--rw-r--r--   0        0        0     1246 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/void.py
--rw-r--r--   0        0        0     4913 2024-05-22 09:10:58.885615 lnbits-0.12.7/lnbits/wallets/zbd.py
--rw-r--r--   0        0        0     4759 2024-05-22 09:10:58.885615 lnbits-0.12.7/pyproject.toml
--rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 lnbits-0.12.7/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-28 12:03:30.945273 lnbits-0.12.8/LICENSE
+-rw-r--r--   0        0        0     4154 2024-05-28 12:03:30.945273 lnbits-0.12.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/__main__.py
+-rw-r--r--   0        0        0    13859 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/app.py
+-rw-r--r--   0        0        0      135 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/bolt11.py
+-rw-r--r--   0        0        0    23181 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/commands.py
+-rw-r--r--   0        0        0     1460 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/__init__.py
+-rw-r--r--   0        0        0    38012 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/crud.py
+-rw-r--r--   0        0        0      148 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/db.py
+-rw-r--r--   0        0        0     4405 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/helpers.py
+-rw-r--r--   0        0        0    15500 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/migrations.py
+-rw-r--r--   0        0        0    12204 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/models.py
+-rw-r--r--   0        0        0    28619 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/services.py
+-rw-r--r--   0        0        0     1156 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/sso/keycloak.py
+-rw-r--r--   0        0        0     5918 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/tasks.py
+-rw-r--r--   0        0        0     3030 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/admin/_tab_funding.html
+-rw-r--r--   0        0        0    12921 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/admin/_tab_security.html
+-rw-r--r--   0        0        0     2187 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/admin/_tab_security_notifications.html
+-rw-r--r--   0        0        0     6048 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/admin/_tab_server.html
+-rw-r--r--   0        0        0     4766 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/admin/_tab_theme.html
+-rw-r--r--   0        0        0     2238 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/admin/_tab_users.html
+-rw-r--r--   0        0        0     2951 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/admin/index.html
+-rw-r--r--   0        0        0     5530 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/core/_api_docs.html
+-rw-r--r--   0        0        0    17024 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/core/account.html
+-rw-r--r--   0        0        0    43399 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/core/extensions.html
+-rw-r--r--   0        0        0     4037 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/core/first_install.html
+-rw-r--r--   0        0        0    18777 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/core/index.html
+-rw-r--r--   0        0        0    25092 2024-05-28 12:03:30.945273 lnbits-0.12.8/lnbits/core/templates/core/wallet.html
+-rw-r--r--   0        0        0    10041 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/node/_tab_channels.html
+-rw-r--r--   0        0        0     2435 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/node/_tab_dashboard.html
+-rw-r--r--   0        0        0    12171 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/node/_tab_transactions.html
+-rw-r--r--   0        0        0    10706 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/node/index.html
+-rw-r--r--   0        0        0     3719 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/node/public.html
+-rw-r--r--   0        0        0     2429 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/service-worker.js
+-rw-r--r--   0        0        0      716 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/users/_createUserDialog.html
+-rw-r--r--   0        0        0      724 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/users/_createWalletDialog.html
+-rw-r--r--   0        0        0     1088 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/users/_topupDialog.html
+-rw-r--r--   0        0        0     3328 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/users/_walletDialog.html
+-rw-r--r--   0        0        0     4005 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/templates/users/index.html
+-rw-r--r--   0        0        0        0 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/__init__.py
+-rw-r--r--   0        0        0     3826 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/admin_api.py
+-rw-r--r--   0        0        0     8151 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/api.py
+-rw-r--r--   0        0        0    12341 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/auth_api.py
+-rw-r--r--   0        0        0    17278 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/extension_api.py
+-rw-r--r--   0        0        0    12872 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/generic.py
+-rw-r--r--   0        0        0     5896 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/node_api.py
+-rw-r--r--   0        0        0    15146 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/payment_api.py
+-rw-r--r--   0        0        0     1724 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/public_api.py
+-rw-r--r--   0        0        0     2845 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/tinyurl_api.py
+-rw-r--r--   0        0        0     5275 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/user_api.py
+-rw-r--r--   0        0        0     1894 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/wallet_api.py
+-rw-r--r--   0        0        0     2137 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/webpush_api.py
+-rw-r--r--   0        0        0     1131 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/core/views/websocket_api.py
+-rw-r--r--   0        0        0    15893 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/db.py
+-rw-r--r--   0        0        0     8649 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/decorators.py
+-rw-r--r--   0        0        0     3751 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/exceptions.py
+-rw-r--r--   0        0        0    24909 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/extension_manager.py
+-rw-r--r--   0        0        0     8177 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/helpers.py
+-rw-r--r--   0        0        0     1073 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/jinja2_templating.py
+-rw-r--r--   0        0        0       75 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/lnurl.py
+-rw-r--r--   0        0        0     8386 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/middleware.py
+-rw-r--r--   0        0        0      206 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/nodes/__init__.py
+-rw-r--r--   0        0        0     5561 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/nodes/base.py
+-rw-r--r--   0        0        0    11840 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/nodes/cln.py
+-rw-r--r--   0        0        0    13247 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/nodes/lndrest.py
+-rw-r--r--   0        0        0       26 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/py.typed
+-rw-r--r--   0        0        0      198 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/requestvars.py
+-rw-r--r--   0        0        0     2415 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/server.py
+-rw-r--r--   0        0        0    19415 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/settings.py
+-rw-r--r--   0        0        0   209450 2024-05-28 12:03:30.949273 lnbits-0.12.8/lnbits/static/bundle.min.css
+-rw-r--r--   0        0        0  1604902 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/bundle.min.js
+-rw-r--r--   0        0        0    12767 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/css/base.css
+-rw-r--r--   0        0        0     4286 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/favicon.ico
+-rw-r--r--   0        0        0   104948 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/fonts/material-icons-v50.woff2
+-rw-r--r--   0        0        0    12328 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/i18n/br.js
+-rw-r--r--   0        0        0    10705 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/i18n/cn.js
+-rw-r--r--   0        0        0    12205 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/i18n/cs.js
+-rw-r--r--   0        0        0    12724 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/i18n/de.js
+-rw-r--r--   0        0        0    11453 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/i18n/en.js
+-rw-r--r--   0        0        0    12652 2024-05-28 12:03:30.957273 lnbits-0.12.8/lnbits/static/i18n/es.js
+-rw-r--r--   0        0        0    12730 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/fi.js
+-rw-r--r--   0        0        0    13202 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/fr.js
+-rw-r--r--   0        0        0       25 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/i18n.js
+-rw-r--r--   0        0        0    12547 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/it.js
+-rw-r--r--   0        0        0    14211 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/jp.js
+-rw-r--r--   0        0        0    13412 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/kr.js
+-rw-r--r--   0        0        0    12293 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/nl.js
+-rw-r--r--   0        0        0    12608 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/pi.js
+-rw-r--r--   0        0        0    12300 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/pl.js
+-rw-r--r--   0        0        0    12289 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/pt.js
+-rw-r--r--   0        0        0    12365 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/sk.js
+-rw-r--r--   0        0        0    11748 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/i18n/we.js
+-rw-r--r--   0        0        0     1620 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/images/alby.png
+-rw-r--r--   0        0        0     1620 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/images/albyl.png
+-rw-r--r--   0        0        0    16651 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/images/bitcoin-hardware-wallet.png
+-rw-r--r--   0        0        0    56349 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/images/bitcoin-shop-banner.png
+-rw-r--r--   0        0        0     3493 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/images/blitz.png
+-rw-r--r--   0        0        0    13998 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/images/blitzl.png
+-rw-r--r--   0        0        0     2465 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/images/cln.png
+-rw-r--r--   0        0        0    12787 2024-05-28 12:03:30.961273 lnbits-0.12.8/lnbits/static/images/clnl.png
+-rw-r--r--   0        0        0   181365 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/default_voucher.png
+-rw-r--r--   0        0        0     1692 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/github-logo.png
+-rw-r--r--   0        0        0      982 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/google-logo.png
+-rw-r--r--   0        0        0     1887 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/keycloak-logo.png
+-rw-r--r--   0        0        0    11564 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/lnbits-shop-dark.png
+-rw-r--r--   0        0        0    13698 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/lnbits-shop-light.png
+-rw-r--r--   0        0        0     2290 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/lnd.png
+-rw-r--r--   0        0        0     3587 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/lnpay.png
+-rw-r--r--   0        0        0    12415 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/lnpayl.png
+-rw-r--r--   0        0        0    14906 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/logos/lnbits.png
+-rw-r--r--   0        0        0      290 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/logos/lnbits.svg
+-rw-r--r--   0        0        0    15727 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/maskable_icon.png
+-rw-r--r--   0        0        0     2383 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/maskable_icon_x192.png
+-rw-r--r--   0        0        0     6144 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/maskable_icon_x512.png
+-rw-r--r--   0        0        0     1231 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/maskable_icon_x96.png
+-rw-r--r--   0        0        0    13511 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/mynode.png
+-rw-r--r--   0        0        0     8846 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/mynodel.png
+-rw-r--r--   0        0        0    15961 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/open-sats.png
+-rw-r--r--   0        0        0     3551 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/opennode.png
+-rw-r--r--   0        0        0    14197 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/opennodel.png
+-rw-r--r--   0        0        0     7751 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/phoenixd.png
+-rw-r--r--   0        0        0     4592 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/phoenixdl.png
+-rw-r--r--   0        0        0    98187 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/screenshot_desktop.png
+-rw-r--r--   0        0        0   120332 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/screenshot_phone.png
+-rw-r--r--   0        0        0     4401 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/spark.png
+-rw-r--r--   0        0        0    15565 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/sparkl.png
+-rw-r--r--   0        0        0     1233 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/start9.png
+-rw-r--r--   0        0        0     1233 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/start9l.png
+-rw-r--r--   0        0        0     3065 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/templatead.png
+-rw-r--r--   0        0        0     3503 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/umbrel.png
+-rw-r--r--   0        0        0    15335 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/umbrell.png
+-rw-r--r--   0        0        0     2522 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/voltage.png
+-rw-r--r--   0        0        0     2584 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/voltagel.png
+-rw-r--r--   0        0        0      985 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/voucher_template.svg
+-rw-r--r--   0        0        0     1937 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/zbd.png
+-rw-r--r--   0        0        0     2003 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/images/zbdl.png
+-rw-r--r--   0        0        0     3172 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/account.js
+-rw-r--r--   0        0        0     8674 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/admin.js
+-rw-r--r--   0        0        0    16664 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/base.js
+-rw-r--r--   0        0        0     9730 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/bolt11-decoder.js
+-rw-r--r--   0        0        0     2732 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/components/extension-settings.js
+-rw-r--r--   0        0        0     4887 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/components/lnbits-funding-sources.js
+-rw-r--r--   0        0        0     4087 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/components/payment-chart.js
+-rw-r--r--   0        0        0    13203 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/components/payment-list.js
+-rw-r--r--   0        0        0    23863 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/components.js
+-rw-r--r--   0        0        0    16879 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/event-reactions.js
+-rw-r--r--   0        0        0     2494 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/index.js
+-rw-r--r--   0        0        0     6824 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/node.js
+-rw-r--r--   0        0        0     9661 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/users.js
+-rw-r--r--   0        0        0    19006 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/js/wallet.js
+-rw-r--r--   0        0        0     4419 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/scss/base.scss
+-rwxr-xr-x   0        0        0   593984 2024-05-28 12:03:30.969273 lnbits-0.12.8/lnbits/static/vendor/Chart.bundle.js
+-rwxr-xr-x   0        0        0      858 2024-05-28 12:03:30.969273 lnbits-0.12.8/lnbits/static/vendor/Chart.css
+-rw-r--r--   0        0        0   372118 2024-05-28 12:03:30.969273 lnbits-0.12.8/lnbits/static/vendor/VueQrcodeReader.umd.js
+-rw-r--r--   0        0        0    97321 2024-05-28 12:03:30.969273 lnbits-0.12.8/lnbits/static/vendor/axios.js
+-rw-r--r--   0        0        0   174604 2024-05-28 12:03:30.973273 lnbits-0.12.8/lnbits/static/vendor/moment.js
+-rw-r--r--   0        0        0   242385 2024-05-28 12:03:30.973273 lnbits-0.12.8/lnbits/static/vendor/quasar.css
+-rw-r--r--   0        0        0     9375 2024-05-28 12:03:30.973273 lnbits-0.12.8/lnbits/static/vendor/quasar.ie.polyfills.umd.min.js
+-rw-r--r--   0        0        0  1066966 2024-05-28 12:03:30.977273 lnbits-0.12.8/lnbits/static/vendor/quasar.umd.js
+-rw-r--r--   0        0        0   159755 2024-05-28 12:03:30.977273 lnbits-0.12.8/lnbits/static/vendor/showdown.js
+-rw-r--r--   0        0        0    68416 2024-05-28 12:03:30.977273 lnbits-0.12.8/lnbits/static/vendor/underscore.js
+-rw-r--r--   0        0        0    68299 2024-05-28 12:03:30.977273 lnbits-0.12.8/lnbits/static/vendor/vue-i18n.js
+-rw-r--r--   0        0        0   157254 2024-05-28 12:03:30.977273 lnbits-0.12.8/lnbits/static/vendor/vue-qrcode.js
+-rw-r--r--   0        0        0    84010 2024-05-28 12:03:30.977273 lnbits-0.12.8/lnbits/static/vendor/vue-router.js
+-rw-r--r--   0        0        0   342147 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/static/vendor/vue.js
+-rw-r--r--   0        0        0    38178 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/static/vendor/vuex.js
+-rw-r--r--   0        0        0     1077 2024-05-28 12:03:30.965273 lnbits-0.12.8/lnbits/static/vendor.json
+-rw-r--r--   0        0        0     7081 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/tasks.py
+-rw-r--r--   0        0        0     9396 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/templates/base.html
+-rw-r--r--   0        0        0     1476 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/templates/error.html
+-rw-r--r--   0        0        0      406 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/templates/macros.jinja
+-rw-r--r--   0        0        0     1194 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/templates/print.html
+-rw-r--r--   0        0        0      635 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/templates/public.html
+-rw-r--r--   0        0        0        0 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/utils/__init__.py
+-rw-r--r--   0        0        0     1914 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/utils/cache.py
+-rw-r--r--   0        0        0     2510 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/utils/crypto.py
+-rw-r--r--   0        0        0     9000 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/utils/exchange_rates.py
+-rw-r--r--   0        0        0     3990 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/utils/logger.py
+-rw-r--r--   0        0        0     1568 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/__init__.py
+-rw-r--r--   0        0        0     6870 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/alby.py
+-rw-r--r--   0        0        0     3406 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/base.py
+-rw-r--r--   0        0        0     6397 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/cliche.py
+-rw-r--r--   0        0        0    10608 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/corelightning.py
+-rw-r--r--   0        0        0    12191 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/corelightningrest.py
+-rw-r--r--   0        0        0     8388 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/eclair.py
+-rw-r--r--   0        0        0     4020 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/fake.py
+-rw-r--r--   0        0        0     8516 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lnbits.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lnd_grpc_files/__init__.py
+-rw-r--r--   0        0        0   181468 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lnd_grpc_files/lightning_pb2.py
+-rw-r--r--   0        0        0   124188 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lnd_grpc_files/lightning_pb2_grpc.py
+-rw-r--r--   0        0        0    35071 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lnd_grpc_files/router_pb2.py
+-rw-r--r--   0        0        0    31107 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lnd_grpc_files/router_pb2_grpc.py
+-rw-r--r--   0        0        0     9951 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lndgrpc.py
+-rw-r--r--   0        0        0    10879 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lndrest.py
+-rw-r--r--   0        0        0     4764 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lnpay.py
+-rw-r--r--   0        0        0     6001 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/lntips.py
+-rw-r--r--   0        0        0       36 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/macaroon/__init__.py
+-rw-r--r--   0        0        0     1345 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/macaroon/macaroon.py
+-rw-r--r--   0        0        0     4688 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/opennode.py
+-rw-r--r--   0        0        0     8363 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/phoenixd.py
+-rw-r--r--   0        0        0     9038 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/spark.py
+-rw-r--r--   0        0        0     1246 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/void.py
+-rw-r--r--   0        0        0     4913 2024-05-28 12:03:30.981273 lnbits-0.12.8/lnbits/wallets/zbd.py
+-rw-r--r--   0        0        0     4759 2024-05-28 12:03:30.985273 lnbits-0.12.8/pyproject.toml
+-rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 lnbits-0.12.8/PKG-INFO
```

### Comparing `lnbits-0.12.7/LICENSE` & `lnbits-0.12.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/README.md` & `lnbits-0.12.8/README.md`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/app.py` & `lnbits-0.12.8/lnbits/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.staticfiles import StaticFiles
 from loguru import logger
 from slowapi import Limiter
 from slowapi.util import get_remote_address
 from starlette.middleware.sessions import SessionMiddleware
 
-from lnbits.core.crud import get_dbversions, get_installed_extensions
+from lnbits.core.crud import (
+    get_dbversions,
+    get_installed_extensions,
+    update_installed_extension_state,
+)
 from lnbits.core.helpers import migrate_extension_database
 from lnbits.core.tasks import (  # watchdog_task
     killswitch_task,
     wait_for_paid_invoices,
 )
 from lnbits.exceptions import register_exception_handlers
 from lnbits.settings import settings
@@ -38,15 +42,14 @@
 from lnbits.wallets import get_funding_source, set_funding_source
 
 from .commands import migrate_databases
 from .core import init_core_routers
 from .core.db import core_app_extra
 from .core.services import check_admin_settings, check_webpush_settings
 from .core.views.extension_api import add_installed_extension
-from .core.views.generic import update_installed_extension_state
 from .extension_manager import (
     Extension,
     InstallableExtension,
     get_valid_extensions,
     version_parse,
 )
 from .middleware import (
@@ -257,18 +260,18 @@
     include_deactivated: Optional[bool] = True,
 ) -> List[InstallableExtension]:
     """
     Returns a list of all the installed extensions plus the extensions that
     MUST be installed by default (see LNBITS_EXTENSIONS_DEFAULT_INSTALL).
     """
     installed_extensions = await get_installed_extensions()
+    settings.lnbits_all_extensions_ids = {e.id for e in installed_extensions}
 
-    installed_extensions_ids = [e.id for e in installed_extensions]
     for ext_id in settings.lnbits_extensions_default_install:
-        if ext_id in installed_extensions_ids:
+        if ext_id in settings.lnbits_all_extensions_ids:
             continue
 
         ext_releases = await InstallableExtension.get_extension_releases(ext_id)
         ext_releases = sorted(
             ext_releases, key=lambda r: version_parse(r.version), reverse=True
         )
 
@@ -314,16 +317,15 @@
     register_ext_routes(app, extension)
 
     current_version = (await get_dbversions()).get(ext.id, 0)
     await migrate_extension_database(extension, current_version)
 
     # mount routes for the new version
     core_app_extra.register_new_ext_routes(extension)
-    if extension.upgrade_hash:
-        ext.notify_upgrade()
+    ext.notify_upgrade(extension.upgrade_hash)
 
 
 def register_custom_extensions_path():
     if settings.has_default_extension_path:
         return
     default_ext_path = os.path.join("lnbits", "extensions")
     if os.path.isdir(default_ext_path) and len(os.listdir(default_ext_path)) != 0:
```

### Comparing `lnbits-0.12.7/lnbits/commands.py` & `lnbits-0.12.8/lnbits/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from .core import migrations as core_migrations
 from .core.crud import (
     delete_accounts_no_wallets,
     delete_unused_wallets,
     delete_wallet_by_id,
     delete_wallet_payment,
     get_dbversions,
-    get_inactive_extensions,
     get_installed_extension,
     get_installed_extensions,
     get_payments,
     remove_deleted_wallets,
     update_payment_status,
 )
 from .core.helpers import migrate_extension_database, run_migration
@@ -150,14 +149,15 @@
         core_version = current_versions.get("core", 0)
         await run_migration(conn, core_migrations, "core", core_version)
 
     # here is the first place we can be sure that the
     # `installed_extensions` table has been created
     await load_disabled_extension_list()
 
+    # todo: revisit, use installed extensions
     for ext in get_valid_extensions(False):
         current_version = current_versions.get(ext.code, 0)
         try:
             await migrate_extension_database(ext, current_version)
         except Exception as e:
             logger.exception(f"Error migrating extension {ext.code}: {e}")
 
@@ -311,16 +311,16 @@
     for w in invalid_wallets:
         data = invalid_wallets[f"{w}"]
         click.echo(" ".join([w, str(data[0]), str(data[1] / 1000).ljust(10)]))
 
 
 async def load_disabled_extension_list() -> None:
     """Update list of extensions that have been explicitly disabled"""
-    inactive_extensions = await get_inactive_extensions()
-    settings.lnbits_deactivated_extensions += inactive_extensions
+    inactive_extensions = await get_installed_extensions(active=False)
+    settings.lnbits_deactivated_extensions.update([e.id for e in inactive_extensions])
 
 
 @extensions.command("list")
 @coro
 async def extensions_list():
     """Show currently installed extensions"""
     click.echo("Installed extensions:")
```

### Comparing `lnbits-0.12.7/lnbits/core/__init__.py` & `lnbits-0.12.8/lnbits/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .db import core_app_extra, db
 from .views.admin_api import admin_router
 from .views.api import api_router
 from .views.auth_api import auth_router
 from .views.extension_api import extension_router
 
 # this compat is needed for usermanager extension
-from .views.generic import generic_router, update_user_extension
+from .views.generic import generic_router
 from .views.node_api import node_router, public_node_router, super_node_router
 from .views.payment_api import payment_router
 from .views.public_api import public_router
 from .views.tinyurl_api import tinyurl_router
 from .views.user_api import users_router
 from .views.wallet_api import wallet_router
 from .views.webpush_api import webpush_router
```

### Comparing `lnbits-0.12.7/lnbits/core/crud.py` & `lnbits-0.12.8/lnbits/core/crud.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 from uuid import UUID, uuid4
 
 import shortuuid
 from passlib.context import CryptContext
 
 from lnbits.core.db import db
 from lnbits.db import DB_TYPE, SQLITE, Connection, Database, Filters, Page
-from lnbits.extension_manager import InstallableExtension
+from lnbits.extension_manager import (
+    InstallableExtension,
+    PayToEnableInfo,
+    UserExtension,
+    UserExtensionInfo,
+)
 from lnbits.settings import (
     AdminSettings,
     EditableSettings,
     SuperSettings,
     WebPushSettings,
     settings,
 )
@@ -318,18 +323,15 @@
         SELECT id, email, username, pass, extra, created_at, updated_at
         FROM accounts WHERE id = ?
         """,
         (user_id,),
     )
 
     if user:
-        extensions = await (conn or db).fetchall(
-            """SELECT extension FROM extensions WHERE "user" = ? AND active""",
-            (user_id,),
-        )
+        extensions = await get_user_active_extensions_ids(user_id, conn)
         wallets = await (conn or db).fetchall(
             """
             SELECT *, COALESCE((
                 SELECT balance FROM balances WHERE wallet = wallets.id
             ), 0) AS balance_msat
             FROM wallets
             WHERE "user" = ? and wallets.deleted = false
@@ -340,15 +342,15 @@
         return None
 
     return User(
         id=user["id"],
         email=user["email"],
         username=user["username"],
         extensions=[
-            e[0] for e in extensions if User.is_extension_for_user(e[0], user["id"])
+            e for e in extensions if User.is_extension_for_user(e[0], user["id"])
         ],
         wallets=[Wallet(**w) for w in wallets],
         admin=user["id"] == settings.super_user
         or user["id"] in settings.lnbits_admin_users,
         super_user=user["id"] == settings.super_user,
         has_password=True if user["pass"] else False,
         config=UserConfig(**json.loads(user["extra"])) if user["extra"] else None,
@@ -363,39 +365,41 @@
     ext: InstallableExtension,
     conn: Optional[Connection] = None,
 ) -> None:
     meta = {
         "installed_release": (
             dict(ext.installed_release) if ext.installed_release else None
         ),
+        "pay_to_enable": (dict(ext.pay_to_enable) if ext.pay_to_enable else None),
         "dependencies": ext.dependencies,
         "payments": [dict(p) for p in ext.payments] if ext.payments else None,
     }
 
     version = ext.installed_release.version if ext.installed_release else ""
 
     await (conn or db).execute(
         """
         INSERT INTO installed_extensions
-        (id, version, name, short_description, icon, stars, meta)
-        VALUES (?, ?, ?, ?, ?, ?, ?) ON CONFLICT (id) DO UPDATE SET
+        (id, version, name, active, short_description, icon, stars, meta)
+        VALUES (?, ?, ?, ?, ?, ?, ?, ?) ON CONFLICT (id) DO UPDATE SET
         (version, name, active, short_description, icon, stars, meta) =
         (?, ?, ?, ?, ?, ?, ?)
         """,
         (
             ext.id,
             version,
             ext.name,
+            ext.active,
             ext.short_description,
             ext.icon,
             ext.stars,
             json.dumps(meta),
             version,
             ext.name,
-            False,
+            ext.active,
             ext.short_description,
             ext.icon,
             ext.stars,
             json.dumps(meta),
         ),
     )
 
@@ -407,14 +411,25 @@
         """
         UPDATE installed_extensions SET active = ? WHERE id = ?
         """,
         (active, ext_id),
     )
 
 
+async def update_extension_pay_to_enable(
+    ext_id: str, payment_info: PayToEnableInfo, conn: Optional[Connection] = None
+) -> None:
+    ext = await get_installed_extension(ext_id, conn)
+    if not ext:
+        return
+    ext.pay_to_enable = payment_info
+
+    await add_installed_extension(ext, conn)
+
+
 async def delete_installed_extension(
     *, ext_id: str, conn: Optional[Connection] = None
 ) -> None:
     await (conn or db).execute(
         """
         DELETE from installed_extensions  WHERE id = ?
         """,
@@ -449,43 +464,92 @@
         (ext_id,),
     )
 
     return InstallableExtension.from_row(row) if row else None
 
 
 async def get_installed_extensions(
+    active: Optional[bool] = None,
     conn: Optional[Connection] = None,
 ) -> List["InstallableExtension"]:
     rows = await (conn or db).fetchall(
         "SELECT * FROM installed_extensions",
         (),
     )
-    return [InstallableExtension.from_row(row) for row in rows]
+    all_extensions = [InstallableExtension.from_row(row) for row in rows]
+    if active is None:
+        return all_extensions
 
+    return [e for e in all_extensions if e.active == active]
 
-async def get_inactive_extensions(*, conn: Optional[Connection] = None) -> List[str]:
-    inactive_extensions = await (conn or db).fetchall(
-        """SELECT id FROM installed_extensions WHERE NOT active""",
-        (),
+
+async def get_user_extension(
+    user_id: str, extension: str, conn: Optional[Connection] = None
+) -> Optional[UserExtension]:
+    row = await (conn or db).fetchone(
+        """
+            SELECT extension, active, extra as _extra FROM extensions
+            WHERE "user" = ? AND extension = ?
+        """,
+        (user_id, extension),
+    )
+    return UserExtension.from_row(row) if row else None
+
+
+async def get_user_extensions(
+    user_id: str, conn: Optional[Connection] = None
+) -> List[UserExtension]:
+    rows = await (conn or db).fetchall(
+        """
+            SELECT extension, active, extra as _extra FROM extensions
+            WHERE "user" = ?
+        """,
+        (user_id,),
     )
-    return [ext[0] for ext in inactive_extensions]
+    return [UserExtension.from_row(row) for row in rows]
 
 
 async def update_user_extension(
     *, user_id: str, extension: str, active: bool, conn: Optional[Connection] = None
 ) -> None:
     await (conn or db).execute(
         """
         INSERT INTO extensions ("user", extension, active) VALUES (?, ?, ?)
         ON CONFLICT ("user", extension) DO UPDATE SET active = ?
         """,
         (user_id, extension, active, active),
     )
 
 
+async def get_user_active_extensions_ids(
+    user_id: str, conn: Optional[Connection] = None
+) -> List[str]:
+    rows = await (conn or db).fetchall(
+        """SELECT extension FROM extensions WHERE "user" = ? AND active""",
+        (user_id,),
+    )
+    return [e[0] for e in rows]
+
+
+async def update_user_extension_extra(
+    user_id: str,
+    extension: str,
+    extra: UserExtensionInfo,
+    conn: Optional[Connection] = None,
+) -> None:
+    extra_json = json.dumps(dict(extra))
+    await (conn or db).execute(
+        """
+        INSERT INTO extensions ("user", extension, extra) VALUES (?, ?, ?)
+        ON CONFLICT ("user", extension) DO UPDATE SET extra = ?
+        """,
+        (user_id, extension, extra_json, extra_json),
+    )
+
+
 # wallets
 # -------
 
 
 async def create_wallet(
     *,
     user_id: str,
@@ -1252,60 +1316,62 @@
     return await get_webpush_settings()
 
 
 async def get_webpush_subscription(
     endpoint: str, user: str
 ) -> Optional[WebPushSubscription]:
     row = await db.fetchone(
-        "SELECT * FROM webpush_subscriptions WHERE endpoint = ? AND user = ?",
+        """SELECT * FROM webpush_subscriptions WHERE endpoint = ? AND "user" = ?""",
         (
             endpoint,
             user,
         ),
     )
     return WebPushSubscription(**dict(row)) if row else None
 
 
 async def get_webpush_subscriptions_for_user(
     user: str,
 ) -> List[WebPushSubscription]:
     rows = await db.fetchall(
-        "SELECT * FROM webpush_subscriptions WHERE user = ?",
+        """SELECT * FROM webpush_subscriptions WHERE "user" = ?""",
         (user,),
     )
     return [WebPushSubscription(**dict(row)) for row in rows]
 
 
 async def create_webpush_subscription(
     endpoint: str, user: str, data: str, host: str
 ) -> WebPushSubscription:
     await db.execute(
         """
-        INSERT INTO webpush_subscriptions (endpoint, user, data, host)
+        INSERT INTO webpush_subscriptions (endpoint, "user", data, host)
         VALUES (?, ?, ?, ?)
         """,
         (
             endpoint,
             user,
             data,
             host,
         ),
     )
     subscription = await get_webpush_subscription(endpoint, user)
     assert subscription, "Newly created webpush subscription couldn't be retrieved"
     return subscription
 
 
-async def delete_webpush_subscription(endpoint: str, user: str) -> None:
-    await db.execute(
-        "DELETE FROM webpush_subscriptions WHERE endpoint = ? AND user = ?",
+async def delete_webpush_subscription(endpoint: str, user: str) -> int:
+    resp = await db.execute(
+        """DELETE FROM webpush_subscriptions WHERE endpoint = ? AND "user" = ?""",
         (
             endpoint,
             user,
         ),
     )
+    return resp.rowcount
 
 
-async def delete_webpush_subscriptions(endpoint: str) -> None:
-    await db.execute(
+async def delete_webpush_subscriptions(endpoint: str) -> int:
+    resp = await db.execute(
         "DELETE FROM webpush_subscriptions WHERE endpoint = ?", (endpoint,)
     )
+    return resp.rowcount
```

### Comparing `lnbits-0.12.7/lnbits/core/helpers.py` & `lnbits-0.12.8/lnbits/core/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,17 @@
 
         # Extensions must expose an `{ext_id}_stop()` function at the module level
         # The `api_stop()` function is for backwards compatibility (will be deprecated)
         stop_fns = [f"{ext_id}_stop", "api_stop"]
         stop_fn_name = next((fn for fn in stop_fns if hasattr(old_module, fn)), None)
         assert stop_fn_name, "No stop function found for '{ext.module_name}'"
 
-        await getattr(old_module, stop_fn_name)()
+        stop_fn = getattr(old_module, stop_fn_name)
+        if stop_fn:
+            await stop_fn()
 
         logger.info(f"Stopped background work for extension '{ext.module_name}'.")
     except Exception as ex:
         logger.warning(f"Failed to stop background work for '{ext.module_name}'.")
         logger.warning(ex)
         return False
```

### Comparing `lnbits-0.12.7/lnbits/core/migrations.py` & `lnbits-0.12.8/lnbits/core/migrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,16 @@
         for row in rows:
             try:
                 user = row[2].split(":")[1]
                 adminkey = row[3].split(":")[1]
                 inkey = row[4].split(":")[1]
                 await db.execute(
                     """
-                    UPDATE wallets SET user = ?, adminkey = ?, inkey = ?, deleted = true
+                    UPDATE wallets SET
+                    "user" = ?, adminkey = ?, inkey = ?, deleted = true
                     WHERE id = ?
                     """,
                     (user, adminkey, inkey, row[0]),
                 )
             except Exception:
                 continue
     except OperationalError:
@@ -508,7 +509,14 @@
         LEFT JOIN apipayments ON apipayments.wallet = wallets.id
         WHERE (wallets.deleted = false OR wallets.deleted is NULL)
               AND ((apipayments.pending = false AND apipayments.amount > 0)
               OR apipayments.amount < 0)
         GROUP BY apipayments.wallet
     """
     )
+
+
+async def m020_add_column_column_to_user_extensions(db):
+    """
+    Adds extra column to user extensions.
+    """
+    await db.execute("ALTER TABLE extensions ADD COLUMN extra TEXT")
```

### Comparing `lnbits-0.12.7/lnbits/core/models.py` & `lnbits-0.12.8/lnbits/core/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -449,7 +449,12 @@
 class BalanceDelta(BaseModel):
     lnbits_balance_msats: int
     node_balance_msats: int
 
     @property
     def delta_msats(self):
         return self.node_balance_msats - self.lnbits_balance_msats
+
+
+class SimpleStatus(BaseModel):
+    success: bool
+    message: str
```

### Comparing `lnbits-0.12.7/lnbits/core/services.py` & `lnbits-0.12.8/lnbits/core/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 from fastapi import Depends, WebSocket
 from loguru import logger
 from py_vapid import Vapid
 from py_vapid.utils import b64urlencode
 
 from lnbits.core.db import db
 from lnbits.db import Connection
-from lnbits.decorators import WalletTypeInfo, require_admin_key
+from lnbits.decorators import (
+    WalletTypeInfo,
+    check_user_extension_access,
+    require_admin_key,
+)
 from lnbits.helpers import url_for
 from lnbits.lnurl import LnurlErrorResponse
 from lnbits.lnurl import decode as decode_lnurl
 from lnbits.settings import (
     EditableSettings,
     SuperSettings,
     readonly_variables,
@@ -296,26 +300,21 @@
                 logger.error(f"could not create temporary payment: {exc}")
                 # happens if the same wallet tries to pay an invoice twice
                 raise PaymentError("Could not make payment.", status="failed") from exc
 
         # do the balance check
         wallet = await get_wallet(wallet_id, conn=conn)
         assert wallet, "Wallet for balancecheck could not be fetched"
-        if wallet.balance_msat < 0:
-            logger.debug("balance is too low, deleting temporary payment")
-            if (
-                not internal_checking_id
-                and wallet.balance_msat > -fee_reserve_total_msat
-            ):
-                raise PaymentError(
-                    f"You must reserve at least ({round(fee_reserve_total_msat/1000)}"
-                    "  sat) to cover potential routing fees.",
-                    status="failed",
-                )
-            raise PaymentError("Insufficient balance.", status="failed")
+        _check_wallet_balance(wallet, fee_reserve_total_msat, internal_checking_id)
+
+    if extra and "tag" in extra:
+        # check if the payment is made for an extension that the user disabled
+        status = await check_user_extension_access(wallet.user, extra["tag"])
+        if not status.success:
+            raise PaymentError(status.message)
 
     if internal_checking_id:
         service_fee_msat = service_fee(invoice.amount_msat, internal=True)
         logger.debug(f"marking temporary payment as not pending {internal_checking_id}")
         # mark the invoice from the other side as not pending anymore
         # so the other side only has access to his new money when we are sure
         # the payer has enough to deduct from
@@ -398,14 +397,30 @@
             payment_request=payment_request,
             payment_hash=invoice.payment_hash,
             pending=False,
         )
     return invoice.payment_hash
 
 
+def _check_wallet_balance(
+    wallet: Wallet,
+    fee_reserve_total_msat: int,
+    internal_checking_id: Optional[str] = None,
+):
+    if wallet.balance_msat < 0:
+        logger.debug("balance is too low, deleting temporary payment")
+        if not internal_checking_id and wallet.balance_msat > -fee_reserve_total_msat:
+            raise PaymentError(
+                f"You must reserve at least ({round(fee_reserve_total_msat/1000)}"
+                "  sat) to cover potential routing fees.",
+                status="failed",
+            )
+        raise PaymentError("Insufficient balance.", status="failed")
+
+
 async def check_wallet_limits(wallet_id, conn, amount_msat):
     await check_time_limit_between_transactions(conn, wallet_id)
     await check_wallet_daily_withdraw_limit(conn, wallet_id, amount_msat)
 
 
 async def check_time_limit_between_transactions(conn, wallet_id):
     limit = settings.lnbits_wallet_limit_secs_between_trans
@@ -632,23 +647,27 @@
 
 def fee_reserve_total(amount_msat: int, internal: bool = False) -> int:
     return fee_reserve(amount_msat, internal) + service_fee(amount_msat, internal)
 
 
 async def send_payment_notification(wallet: Wallet, payment: Payment):
     await websocket_updater(
-        wallet.id,
+        wallet.inkey,
         json.dumps(
             {
                 "wallet_balance": wallet.balance,
                 "payment": payment.dict(),
             }
         ),
     )
 
+    await websocket_updater(
+        payment.payment_hash, json.dumps({"pending": payment.pending})
+    )
+
 
 async def update_wallet_balance(wallet_id: str, amount: int):
     payment_hash, _ = await create_invoice(
         wallet_id=wallet_id,
         amount=amount,
         memo="Admin top up",
         internal=True,
```

### Comparing `lnbits-0.12.7/lnbits/core/sso/keycloak.py` & `lnbits-0.12.8/lnbits/core/sso/keycloak.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/tasks.py` & `lnbits-0.12.8/lnbits/core/tasks.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/admin/_tab_funding.html` & `lnbits-0.12.8/lnbits/core/templates/admin/_tab_funding.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/admin/_tab_security.html` & `lnbits-0.12.8/lnbits/core/templates/admin/_tab_security.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/admin/_tab_security_notifications.html` & `lnbits-0.12.8/lnbits/core/templates/admin/_tab_security_notifications.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/admin/_tab_server.html` & `lnbits-0.12.8/lnbits/core/templates/admin/_tab_server.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/admin/_tab_theme.html` & `lnbits-0.12.8/lnbits/core/templates/admin/_tab_theme.html`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
             label="Site tagline"
           ></q-input>
           <br />
         </div>
         <div class="col-12 col-md-2 q-mt-xl">
           <q-toggle
             tip="Remove homepage elements like 'runs on' etc"
-            v-model="formData.LNBITS_SHOW_HOME_PAGE_ELEMENTS"
-            :label="formData.LNBITS_SHOW_HOME_PAGE_ELEMENTS ? 'Enable elements on homepage' : 'Disable elements on homepage'"
+            v-model="formData.lnbits_show_home_page_elements"
+            :label="formData.lnbits_show_home_page_elements ? 'Enable elements on homepage' : 'Disable elements on homepage'"
           ></q-toggle>
         </div>
       </div>
 
       <div>
         <p>Site Description</p>
         <q-input
```

### Comparing `lnbits-0.12.7/lnbits/core/templates/admin/_tab_users.html` & `lnbits-0.12.8/lnbits/core/templates/admin/_tab_users.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/admin/index.html` & `lnbits-0.12.8/lnbits/core/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/core/_api_docs.html` & `lnbits-0.12.8/lnbits/core/templates/core/_api_docs.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/core/account.html` & `lnbits-0.12.8/lnbits/core/templates/core/account.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/core/extensions.html` & `lnbits-0.12.8/lnbits/core/templates/core/extensions.html`

 * *Files 20% similar despite different names*

```diff
@@ -184,42 +184,37 @@
               :href="extension.id + '/'"
               :label="$t('open')"
             ></q-btn>
             <q-btn
               v-if="user.extensions.includes(extension.id) && extension.isActive && extension.isInstalled"
               flat
               color="grey-5"
-              type="a"
-              :href="['{{
-                url_for('install.extensions')
-              }}', '?disable=', extension.id].join('')"
+              @click="disableExtension(extension)"
               :label="$t('disable')"
             ></q-btn>
             <q-badge
               v-if="extension.isAdminOnly && !user.admin"
               v-text="$t('admin_only')"
             >
             </q-badge>
+
             <q-btn
               v-else-if="extension.isInstalled && extension.isActive && !user.extensions.includes(extension.id)"
               flat
               color="primary"
-              type="a"
-              :href="['{{
-                url_for('install.extensions')
-              }}', '?enable=', extension.id].join('')"
-              :label="$t('enable')"
+              @click="enableExtensionForUser(extension)"
+              :label="$t(extension.isPaymentRequired ? 'pay_to_enable': 'enable')"
             >
               <q-tooltip>
                 <span v-text="$t('enable_extension_details')">
                 </span> </q-tooltip
             ></q-btn>
 
             <q-btn
-              @click="showUpgrade(extension)"
+              @click="showManageExtension(extension)"
               flat
               color="primary"
               v-if="g.user.admin"
               :label="$t('manage')"
               ><q-tooltip
                 ><span v-text="$t('manage_extension_details')"></span
               ></q-tooltip>
@@ -309,15 +304,15 @@
           class="q-ml-auto"
           v-text="$t('cancel')"
         ></q-btn>
       </div>
     </q-card>
   </q-dialog>
 
-  <q-dialog v-model="showUpgradeDialog">
+  <q-dialog v-model="showManageExtensionDialog">
     <q-card v-if="selectedRelease" class="q-pa-lg lnbits__dialog-card">
       <q-card-section>
         <div v-if="selectedRelease.paymentRequest">
           <a :href="'lightning:' + selectedRelease.paymentRequest">
             <q-responsive :ratio="1" class="q-mx-xl">
               <lnbits-qrcode
                 :value="'lightning:' + selectedRelease.paymentRequest.toUpperCase()"
@@ -348,18 +343,38 @@
             class="float-right q-ml-lg"
             v-text="$t('close')"
           ></q-btn>
         </div>
       </div>
     </q-card>
     <q-card v-else class="q-pa-lg lnbits__dialog-card">
-      <q-card-section>
-        <div class="text-h6" v-text="selectedExtension?.name"></div>
-      </q-card-section>
-      <div class="col-12 col-md-5 q-gutter-y-md" v-if="selectedExtensionRepos">
+      <q-tabs
+        v-model="manageExtensionTab"
+        active-color="primary"
+        align="justify"
+      >
+        <q-tab
+          name="releases"
+          :label="$t('releases')"
+          @update="val => manageExtensionTab = val.name"
+        ></q-tab>
+
+        <q-tab
+          v-if="selectedExtension && selectedExtension.isInstalled"
+          name="sell"
+          :label="$t('sell')"
+          @update="val => manageExtensionTab = val.name"
+        ></q-tab>
+      </q-tabs>
+
+      <div
+        v-show="manageExtensionTab === 'releases'"
+        class="col-12 col-md-5 q-gutter-y-md q-mt-md"
+        v-if="selectedExtensionRepos"
+      >
         <q-card
           flat
           bordered
           class="my-card"
           v-for="repoName of Object.keys(selectedExtensionRepos)"
           :key="repoName"
         >
@@ -459,15 +474,15 @@
                           </q-input>
                           <q-select
                             filled
                             dense
                             emit-value
                             v-model="release.wallet"
                             :options="g.user.walletOptions"
-                            label="Wallet *"
+                            :label="$t('wallet_required')"
                             class="q-mt-sm"
                           >
                           </q-select>
                           <q-btn
                             unelevated
                             color="primary"
                             @click="payAndInstall(release)"
@@ -475,15 +490,15 @@
                             class="q-mt-sm"
                             :label="$t('pay_from_wallet')"
                           ></q-btn>
 
                           <q-btn
                             unelevated
                             color="primary"
-                            @click="showQRCode(release)"
+                            @click="showInstallQRCode(release)"
                             class="q-mt-sm float-right"
                             :label="$t('show_qr')"
                           ></q-btn>
                         </div>
                         <div v-else>
                           <br />
                           <span
@@ -552,54 +567,212 @@
 
                     <q-separator></q-separator> </q-card
                 ></q-expansion-item>
               </q-list>
             </q-card-section>
           </q-expansion-item>
         </q-card>
+        <div class="row q-mt-lg">
+          <q-btn
+            v-if="selectedExtension?.isInstalled"
+            @click="showUninstall()"
+            flat
+            color="red"
+            v-text="$t('uninstall')"
+          ></q-btn>
+          <q-btn
+            v-else-if="selectedExtension?.hasDatabaseTables"
+            @click="showDropDb()"
+            flat
+            color="red"
+            :label="$t('drop_db')"
+          ></q-btn>
+          <q-btn
+            v-close-popup
+            flat
+            color="grey"
+            class="q-ml-auto"
+            v-text="$t('close')"
+          ></q-btn>
+        </div>
       </div>
       <q-spinner v-else color="primary" size="2.55em"></q-spinner>
-      <div class="row q-mt-lg">
-        <q-btn
-          v-if="selectedExtension?.isInstalled"
-          @click="showUninstall()"
-          flat
-          color="red"
-          v-text="$t('uninstall')"
-        ></q-btn>
-        <q-btn
-          v-else-if="selectedExtension?.hasDatabaseTables"
-          @click="showDropDb()"
-          flat
-          color="red"
-          :label="$t('drop_db')"
-        ></q-btn>
-        <q-btn
-          v-close-popup
-          flat
-          color="grey"
-          class="q-ml-auto"
-          v-text="$t('close')"
-        ></q-btn>
+      <div
+        v-if="selectedExtension"
+        v-show="manageExtensionTab === 'sell'"
+        class="col-12 col-md-5 q-gutter-y-md q-mt-md"
+      >
+        <q-toggle
+          v-model="selectedExtension.payToEnable.required"
+          :label="$t('sell_require')"
+          color="secondary"
+          style="max-height: 21px"
+        ></q-toggle>
+        <q-select
+          v-if="selectedExtension.payToEnable.required"
+          filled
+          dense
+          emit-value
+          v-model="selectedExtension.payToEnable.wallet"
+          :options="g.user.walletOptions"
+          label="Wallet *"
+          class="q-mt-md"
+        ></q-select>
+        <q-input
+          v-if="selectedExtension.payToEnable.required"
+          filled
+          dense
+          v-model.number="selectedExtension.payToEnable.amount"
+          :label="$t('amount_sats')"
+          type="number"
+          min="1"
+          class="q-mt-md"
+        >
+        </q-input>
+        <div class="row q-mt-lg">
+          <q-btn
+            @click="updatePayToInstallData(selectedExtension)"
+            flat
+            color="green"
+            v-text="$t('update_payment')"
+          ></q-btn>
+
+          <q-btn
+            v-close-popup
+            flat
+            color="grey"
+            class="q-ml-auto"
+            v-text="$t('close')"
+          ></q-btn>
+        </div>
       </div>
     </q-card>
   </q-dialog>
+
+  <q-dialog v-model="showPayToEnableDialog">
+    <q-card v-if="selectedExtension" class="q-pa-md">
+      <q-card-section>
+        <p>
+          <span
+            v-text="$t('sell_info', {name: selectedExtension.name, amount: selectedExtension.payToEnable.amount})"
+          ></span>
+        </p>
+        <p>
+          <span v-text="$t('already_paid_question')"></span>
+          <q-badge
+            @click="enableExtension(selectedExtension)"
+            color="primary"
+            class="cursor-pointer"
+            rounded
+          >
+            <strong> <span v-text="$t('recheck')"></span> </strong
+          ></q-badge>
+        </p>
+      </q-card-section>
+      <q-card-section v-if="selectedExtension.payToEnable.showQRCode">
+        <div class="row q-mt-lg">
+          <div v-if="selectedExtension.payToEnable.paymentRequest" class="col">
+            <a
+              :href="'lightning:' + selectedExtension.payToEnable.paymentRequest"
+            >
+              <q-responsive :ratio="1" class="q-mx-xl">
+                <lnbits-qrcode
+                  :value="'lightning:' + selectedExtension.payToEnable.paymentRequest.toUpperCase()"
+                ></lnbits-qrcode>
+              </q-responsive>
+            </a>
+          </div>
+          <div v-else class="col">
+            <q-spinner color="primary" size="2.55em"></q-spinner>
+          </div>
+        </div>
+        <div class="row q-mt-lg">
+          <div class="col">
+            <q-btn
+              v-if="selectedExtension.payToEnable.paymentRequest"
+              outline
+              color="grey"
+              @click="copyText(selectedExtension.payToEnable.paymentRequest)"
+              :label="$t('copy_invoice')"
+            ></q-btn>
+          </div>
+          <div class="col">
+            <q-btn
+              v-close-popup
+              flat
+              color="grey"
+              class="float-right q-ml-lg"
+              v-text="$t('close')"
+            ></q-btn>
+          </div>
+        </div>
+      </q-card-section>
+
+      <q-card-section v-else>
+        <div class="row q-mt-lg">
+          <div class="col">
+            <div>
+              <q-input
+                filled
+                dense
+                type="number"
+                v-model.number="selectedExtension.payToEnable.paidAmount"
+                :min="selectedExtension.payToEnable.amount"
+                suffix="sat"
+                class="q-mt-sm"
+              >
+              </q-input>
+              <q-select
+                filled
+                dense
+                v-model="selectedExtension.payToEnable.paymentWallet"
+                emit-value
+                :options="g.user.walletOptions"
+                :label="$t('wallet_required')"
+                class="q-mt-sm"
+              >
+              </q-select>
+              <q-separator class="q-mb-lg"></q-separator>
+              <q-btn
+                unelevated
+                color="primary"
+                class="q-mt-sm"
+                @click="payAndEnable(selectedExtension)"
+                :disabled="!selectedExtension.payToEnable.paymentWallet"
+                :label="$t('pay_from_wallet')"
+              ></q-btn>
+
+              <q-btn
+                unelevated
+                @click="showEnableQRCode(selectedExtension)"
+                color="primary"
+                class="q-mt-sm float-right"
+                :label="$t('show_qr')"
+              ></q-btn>
+            </div>
+          </div>
+        </div>
+      </q-card-section>
+    </q-card>
+  </q-dialog>
 </div>
 {% endblock %} {% block scripts %} {{ window_vars(user) }}
 <script>
   new Vue({
     el: '#vue',
     data: function () {
       return {
         searchTerm: '',
         tab: 'all',
+        manageExtensionTab: 'releases',
         filteredExtensions: null,
         showUninstallDialog: false,
-        showUpgradeDialog: false,
+        showManageExtensionDialog: false,
         showDropDbDialog: false,
+        showPayToEnableDialog: false,
         dropDbExtensionId: '',
         selectedExtension: null,
         selectedExtensionRepos: null,
         selectedRelease: null,
         uninstallAndDropDb: false,
         maxStars: 5,
         paylinkWebsocket: null,
@@ -645,15 +818,15 @@
       installExtension: async function (release) {
         // no longer required to check if the invoice was paid
         // the install logic has been triggered one way or another
         this.unsubscribeFromPaylinkWs()
 
         const extension = this.selectedExtension
         extension.inProgress = true
-        this.showUpgradeDialog = false
+        this.showManageExtensionDialog = false
         release.payment_hash =
           release.payment_hash || this.getPaylinkHash(release.pay_link)
 
         LNbits.api
           .request(
             'POST',
             `/api/v1/extension`,
@@ -680,15 +853,15 @@
             console.warn(err)
             extension.inProgress = false
             LNbits.utils.notifyApiError(err)
           })
       },
       uninstallExtension: async function () {
         const extension = this.selectedExtension
-        this.showUpgradeDialog = false
+        this.showManageExtensionDialog = false
         this.showUninstallDialog = false
         extension.inProgress = true
         LNbits.api
           .request(
             'DELETE',
             `/api/v1/extension/${extension.id}`,
             this.g.user.wallets[0].adminkey
@@ -713,15 +886,15 @@
             LNbits.utils.notifyApiError(err)
             extension.inProgress = false
           })
       },
 
       dropExtensionDb: async function () {
         const extension = this.selectedExtension
-        this.showUpgradeDialog = false
+        this.showManageExtensionDialog = false
         this.showDropDbDialog = false
         this.dropDbExtensionId = ''
         extension.inProgress = true
         LNbits.api
           .request(
             'DELETE',
             `/api/v1/extension/${extension.id}/db`,
@@ -741,43 +914,126 @@
             extension.inProgress = false
           })
       },
       toggleExtension: function (extension) {
         const action = extension.isActive ? 'activate' : 'deactivate'
         LNbits.api
           .request(
-            'GET',
-            "{{ url_for('install.extensions') }}" +
-              '?' +
-              action +
-              '=' +
-              extension.id
+            'PUT',
+            `/api/v1/extension/${extension.id}/${action}`,
+            this.g.user.wallets[0].adminkey
+          )
+          .then(response => {
+            this.$q.notify({
+              type: 'positive',
+              message: `Extension '${extension.id}' ${action}d!`
+            })
+          })
+          .catch(err => {
+            LNbits.utils.notifyApiError(err)
+            extension.inProgress = false
+          })
+      },
+      enableExtensionForUser: function (extension) {
+        if (extension.isPaymentRequired) {
+          this.showPayToEnable(extension)
+          return
+        }
+        this.enableExtension(extension)
+      },
+      enableExtension: function (extension) {
+        LNbits.api
+          .request(
+            'PUT',
+            `/api/v1/extension/${extension.id}/enable`,
+            this.g.user.wallets[0].adminkey
           )
-          .then(response => {})
+          .then(response => {
+            this.$q.notify({
+              type: 'positive',
+              message: 'Extension enabled!'
+            })
+            setTimeout(() => {
+              window.location.reload()
+            }, 300)
+          })
+          .catch(err => {
+            console.warn(err)
+            LNbits.utils.notifyApiError(err)
+          })
+      },
+      disableExtension: function (extension) {
+        LNbits.api
+          .request(
+            'PUT',
+            `/api/v1/extension/${extension.id}/disable`,
+            this.g.user.wallets[0].adminkey
+          )
+          .then(response => {
+            this.$q.notify({
+              type: 'positive',
+              message: 'Extension disabled!'
+            })
+            setTimeout(() => {
+              window.location.reload()
+            }, 300)
+          })
+          .catch(err => {
+            console.warn(error)
+            LNbits.utils.notifyApiError(err)
+          })
+      },
+      showPayToEnable: function (extension) {
+        this.selectedExtension = extension
+        this.selectedExtension.payToEnable.paidAmount =
+          extension.payToEnable.amount
+        this.selectedExtension.payToEnable.showQRCode = false
+        this.showPayToEnableDialog = true
+      },
+      updatePayToInstallData: function (extension) {
+        LNbits.api
+          .request(
+            'PUT',
+            `/api/v1/extension/${extension.id}/sell`,
+            this.g.user.wallets[0].adminkey,
+            {
+              required: extension.payToEnable.required,
+              amount: extension.payToEnable.amount,
+              wallet: extension.payToEnable.wallet
+            }
+          )
+          .then(response => {
+            this.$q.notify({
+              type: 'positive',
+              message: 'Payment info updated!'
+            })
+            this.showManageExtensionDialog = false
+          })
           .catch(err => {
             LNbits.utils.notifyApiError(err)
             extension.inProgress = false
           })
       },
 
       showUninstall: function () {
-        this.showUpgradeDialog = false
+        this.showManageExtensionDialog = false
         this.showUninstallDialog = true
         this.uninstallAndDropDb = false
       },
 
       showDropDb: function () {
         this.showDropDbDialog = true
       },
 
-      showUpgrade: async function (extension) {
+      showManageExtension: async function (extension) {
         this.selectedExtension = extension
         this.selectedRelease = null
         this.selectedExtensionRepos = null
-        this.showUpgradeDialog = true
+        this.manageExtensionTab = 'releases'
+        this.showManageExtensionDialog = true
 
         try {
           const {data} = await LNbits.api.request(
             'GET',
             `/api/v1/extension/${extension.id}/releases`,
             this.g.user.wallets[0].adminkey
           )
@@ -812,16 +1068,16 @@
           extension.inProgress = false
         }
       },
 
       async payAndInstall(release) {
         try {
           this.selectedExtension.inProgress = true
-          this.showUpgradeDialog = false
-          const paymentInfo = await this.requestPayment(
+          this.showManageExtensionDialog = false
+          const paymentInfo = await this.requestPaymentForInstall(
             this.selectedExtension.id,
             release
           )
           this.rememberPaylinkHash(release.pay_link, paymentInfo.payment_hash)
           const wallet = this.g.user.wallets.find(w => w.id === release.wallet)
           const {data} = await LNbits.api.payInvoice(
             wallet,
@@ -834,19 +1090,40 @@
         } catch (err) {
           console.warn(err)
           LNbits.utils.notifyApiError(err)
         } finally {
           this.selectedExtension.inProgress = false
         }
       },
-      async showQRCode(release) {
+      async payAndEnable(extension) {
+        try {
+          const paymentInfo = await this.requestPaymentForEnable(
+            extension.id,
+            extension.payToEnable.paidAmount
+          )
+
+          const wallet = this.g.user.wallets.find(
+            w => w.id === extension.payToEnable.paymentWallet
+          )
+          const {data} = await LNbits.api.payInvoice(
+            wallet,
+            paymentInfo.payment_request
+          )
+          this.enableExtension(extension)
+          this.showPayToEnableDialog = false
+        } catch (err) {
+          console.warn(err)
+          LNbits.utils.notifyApiError(err)
+        }
+      },
+      async showInstallQRCode(release) {
         this.selectedRelease = release
 
         try {
-          const data = await this.requestPayment(
+          const data = await this.requestPaymentForInstall(
             this.selectedExtension.id,
             release
           )
 
           this.selectedRelease.paymentRequest = data.payment_request
           this.selectedRelease.payment_hash = data.payment_hash
           this.selectedRelease = _.clone(this.selectedRelease)
@@ -861,30 +1138,76 @@
           )
         } catch (err) {
           console.warn(err)
           LNbits.utils.notifyApiError(err)
         }
       },
 
-      async requestPayment(extId, release) {
+      async showEnableQRCode(extension) {
+        try {
+          extension.payToEnable.showQRCode = true
+          this.selectedExtension = _.clone(extension)
+
+          const data = await this.requestPaymentForEnable(
+            extension.id,
+            extension.payToEnable.paidAmount
+          )
+          extension.payToEnable.paymentRequest = data.payment_request
+          this.selectedExtension = _.clone(extension)
+
+          const url = new URL(window.location)
+          url.protocol = url.protocol === 'https:' ? 'wss' : 'ws'
+          url.pathname = `/api/v1/ws/${data.payment_hash}`
+          const ws = new WebSocket(url)
+          ws.addEventListener('message', async ({data}) => {
+            const payment = JSON.parse(data)
+            if (payment.pending === false) {
+              this.$q.notify({
+                type: 'positive',
+                message: 'Invoice Paid!'
+              })
+
+              this.enableExtension(extension)
+              ws.close()
+            }
+          })
+        } catch (err) {
+          console.warn(err)
+          LNbits.utils.notifyApiError(err)
+        }
+      },
+
+      async requestPaymentForInstall(extId, release) {
         const {data} = await LNbits.api.request(
           'PUT',
-          `/api/v1/extension/invoice`,
+          `/api/v1/extension/${extId}/invoice/install`,
           this.g.user.wallets[0].adminkey,
           {
             ext_id: extId,
             archive: release.archive,
             source_repo: release.source_repo,
             cost_sats: release.paidAmount,
             version: release.version
           }
         )
         return data
       },
 
+      async requestPaymentForEnable(extId, amount) {
+        const {data} = await LNbits.api.request(
+          'PUT',
+          `/api/v1/extension/${extId}/invoice/enable`,
+          this.g.user.wallets[0].adminkey,
+          {
+            amount
+          }
+        )
+        return data
+      },
+
       clearHangingInvoice(release) {
         this.forgetPaylinkHash(release.pay_link)
         release.payment_hash = null
       },
 
       rememberPaylinkHash(pay_link, payment_hash) {
         this.$q.localStorage.set(
```

### Comparing `lnbits-0.12.7/lnbits/core/templates/core/first_install.html` & `lnbits-0.12.8/lnbits/core/templates/core/first_install.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/core/index.html` & `lnbits-0.12.8/lnbits/core/templates/core/index.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/core/wallet.html` & `lnbits-0.12.8/lnbits/core/templates/core/wallet.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/node/_tab_channels.html` & `lnbits-0.12.8/lnbits/core/templates/node/_tab_channels.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/node/_tab_dashboard.html` & `lnbits-0.12.8/lnbits/core/templates/node/_tab_dashboard.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/node/_tab_transactions.html` & `lnbits-0.12.8/lnbits/core/templates/node/_tab_transactions.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/node/index.html` & `lnbits-0.12.8/lnbits/core/templates/node/index.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/node/public.html` & `lnbits-0.12.8/lnbits/core/templates/node/public.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/service-worker.js` & `lnbits-0.12.8/lnbits/core/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/users/_createUserDialog.html` & `lnbits-0.12.8/lnbits/core/templates/users/_createUserDialog.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/users/_createWalletDialog.html` & `lnbits-0.12.8/lnbits/core/templates/users/_createWalletDialog.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/users/_topupDialog.html` & `lnbits-0.12.8/lnbits/core/templates/users/_topupDialog.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/users/_walletDialog.html` & `lnbits-0.12.8/lnbits/core/templates/users/_walletDialog.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/templates/users/index.html` & `lnbits-0.12.8/lnbits/core/templates/users/index.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/admin_api.py` & `lnbits-0.12.8/lnbits/core/views/admin_api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/api.py` & `lnbits-0.12.8/lnbits/core/views/api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/auth_api.py` & `lnbits-0.12.8/lnbits/core/views/auth_api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/generic.py` & `lnbits-0.12.8/lnbits/core/views/generic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-import sys
 from http import HTTPStatus
 from pathlib import Path
 from typing import Annotated, List, Optional, Union
 from urllib.parse import urlparse
 
 from fastapi import Cookie, Depends, Query, Request
 from fastapi.exceptions import HTTPException
 from fastapi.responses import FileResponse, HTMLResponse, RedirectResponse
 from fastapi.routing import APIRouter
 from loguru import logger
 from pydantic.types import UUID4
 
-from lnbits.core.db import core_app_extra
 from lnbits.core.helpers import to_valid_user_id
 from lnbits.core.models import User
 from lnbits.decorators import check_admin, check_user_exists
 from lnbits.helpers import template_renderer
 from lnbits.settings import settings
 from lnbits.wallets import get_funding_source
 
 from ...extension_manager import InstallableExtension, get_valid_extensions
 from ...utils.exchange_rates import allowed_currencies, currencies
 from ..crud import (
     create_wallet,
     get_dbversions,
-    get_inactive_extensions,
     get_installed_extensions,
     get_user,
-    update_installed_extension_state,
-    update_user_extension,
 )
 
 generic_router = APIRouter(
     tags=["Core NON-API Website Routes"], include_in_schema=False
 )
 
 
@@ -69,76 +64,50 @@
     data = """
     User-agent: *
     Disallow: /
     """
     return HTMLResponse(content=data, media_type="text/plain")
 
 
-@generic_router.get(
-    "/extensions", name="install.extensions", response_class=HTMLResponse
-)
-async def extensions_install(
-    request: Request,
-    user: User = Depends(check_user_exists),
-    activate: str = Query(None),
-    deactivate: str = Query(None),
-    enable: str = Query(None),
-    disable: str = Query(None),
-):
-    await toggle_extension(enable, disable, user.id)
-
+@generic_router.get("/extensions", name="extensions", response_class=HTMLResponse)
+async def extensions(request: Request, user: User = Depends(check_user_exists)):
     try:
         installed_exts: List["InstallableExtension"] = await get_installed_extensions()
         installed_exts_ids = [e.id for e in installed_exts]
 
         installable_exts = await InstallableExtension.get_installable_extensions()
         installable_exts_ids = [e.id for e in installable_exts]
         installable_exts += [
             e for e in installed_exts if e.id not in installable_exts_ids
         ]
 
         for e in installable_exts:
             installed_ext = next((ie for ie in installed_exts if e.id == ie.id), None)
             if installed_ext:
                 e.installed_release = installed_ext.installed_release
+                if installed_ext.pay_to_enable and not user.admin:
+                    # not a security leak, but better not to share the wallet id
+                    installed_ext.pay_to_enable.wallet = None
+                e.pay_to_enable = installed_ext.pay_to_enable
+
                 # use the installed extension values
                 e.name = installed_ext.name
                 e.short_description = installed_ext.short_description
                 e.icon = installed_ext.icon
 
     except Exception as ex:
         logger.warning(ex)
         installable_exts = []
         installed_exts_ids = []
 
     try:
-        ext_id = activate or deactivate
-        all_extensions = get_valid_extensions()
-        ext = next((e for e in all_extensions if e.code == ext_id), None)
-        if ext_id and user.admin:
-            if deactivate and deactivate not in settings.lnbits_deactivated_extensions:
-                settings.lnbits_deactivated_extensions += [deactivate]
-            elif activate:
-                # if extension never loaded (was deactivated on server startup)
-                if ext_id not in sys.modules.keys():
-                    # run extension start-up routine
-                    core_app_extra.register_new_ext_routes(ext)
-
-                settings.lnbits_deactivated_extensions = list(
-                    filter(
-                        lambda e: e != activate, settings.lnbits_deactivated_extensions
-                    )
-                )
-
-            await update_installed_extension_state(
-                ext_id=ext_id, active=activate is not None
-            )
-
-        all_ext_ids = [ext.code for ext in all_extensions]
-        inactive_extensions = await get_inactive_extensions()
+        all_ext_ids = [ext.code for ext in get_valid_extensions()]
+        inactive_extensions = [
+            e.id for e in await get_installed_extensions(active=False)
+        ]
         db_version = await get_dbversions()
         extensions = [
             {
                 "id": ext.id,
                 "name": ext.name,
                 "icon": ext.icon,
                 "shortDescription": ext.short_description,
@@ -152,14 +121,16 @@
                 "isActive": ext.id not in inactive_extensions,
                 "latestRelease": (
                     dict(ext.latest_release) if ext.latest_release else None
                 ),
                 "installedRelease": (
                     dict(ext.installed_release) if ext.installed_release else None
                 ),
+                "payToEnable": (dict(ext.pay_to_enable) if ext.pay_to_enable else {}),
+                "isPaymentRequired": ext.requires_payment,
             }
             for ext in installable_exts
         ]
 
         # refresh user state. Eg: enabled extensions.
         user = await get_user(user.id) or user
 
@@ -199,15 +170,15 @@
         wallet_id = lnbits_last_active_wallet
     else:
         wallet_id = user.wallets[0].id
 
     user_wallet = user.get_wallet(wallet_id)
     if not user_wallet or user_wallet.deleted:
         return template_renderer().TemplateResponse(
-            request, "error.html", {"err": "Wallet not found"}
+            request, "error.html", {"err": "Wallet not found"}, HTTPStatus.NOT_FOUND
         )
 
     resp = template_renderer().TemplateResponse(
         request,
         "core/wallet.html",
         {
             "user": user.dict(),
@@ -414,33 +385,7 @@
     try:
         user_id = to_valid_user_id(hex_value).hex
         return RedirectResponse(url=f"/wallet?usr={user_id}")
     except Exception as exc:
         raise HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=str(exc)
         ) from exc
-
-
-async def toggle_extension(extension_to_enable, extension_to_disable, user_id):
-    if extension_to_enable and extension_to_disable:
-        raise HTTPException(
-            HTTPStatus.BAD_REQUEST, "You can either `enable` or `disable` an extension."
-        )
-
-    # check if extension exists
-    if extension_to_enable or extension_to_disable:
-        ext = extension_to_enable or extension_to_disable
-        if ext not in [e.code for e in get_valid_extensions()]:
-            raise HTTPException(
-                HTTPStatus.BAD_REQUEST, f"Extension '{ext}' doesn't exist."
-            )
-
-    if extension_to_enable:
-        logger.info(f"Enabling extension: {extension_to_enable} for user {user_id}")
-        await update_user_extension(
-            user_id=user_id, extension=extension_to_enable, active=True
-        )
-    elif extension_to_disable:
-        logger.info(f"Disabling extension: {extension_to_disable} for user {user_id}")
-        await update_user_extension(
-            user_id=user_id, extension=extension_to_disable, active=False
-        )
```

### Comparing `lnbits-0.12.7/lnbits/core/views/node_api.py` & `lnbits-0.12.8/lnbits/core/views/node_api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/payment_api.py` & `lnbits-0.12.8/lnbits/core/views/payment_api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/public_api.py` & `lnbits-0.12.8/lnbits/core/views/public_api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/tinyurl_api.py` & `lnbits-0.12.8/lnbits/core/views/tinyurl_api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/user_api.py` & `lnbits-0.12.8/lnbits/core/views/user_api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/wallet_api.py` & `lnbits-0.12.8/lnbits/core/views/wallet_api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/core/views/webpush_api.py` & `lnbits-0.12.8/lnbits/core/views/webpush_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import json
 from http import HTTPStatus
 from urllib.parse import unquote, urlparse
 
 from fastapi import (
     APIRouter,
     Depends,
+    HTTPException,
     Request,
 )
+from loguru import logger
 
 from lnbits.core.models import (
     CreateWebPushSubscription,
     WebPushSubscription,
 )
 from lnbits.decorators import (
     WalletTypeInfo,
@@ -29,32 +31,47 @@
 
 @webpush_router.post("", status_code=HTTPStatus.CREATED)
 async def api_create_webpush_subscription(
     request: Request,
     data: CreateWebPushSubscription,
     wallet: WalletTypeInfo = Depends(require_admin_key),
 ) -> WebPushSubscription:
-    subscription = json.loads(data.subscription)
-    endpoint = subscription["endpoint"]
-    host = urlparse(str(request.url)).netloc
-
-    subscription = await get_webpush_subscription(endpoint, wallet.wallet.user)
-    if subscription:
-        return subscription
-    else:
-        return await create_webpush_subscription(
-            endpoint,
-            wallet.wallet.user,
-            data.subscription,
-            host,
-        )
+    try:
+        subscription = json.loads(data.subscription)
+        endpoint = subscription["endpoint"]
+        host = urlparse(str(request.url)).netloc
+
+        subscription = await get_webpush_subscription(endpoint, wallet.wallet.user)
+        if subscription:
+            return subscription
+        else:
+            return await create_webpush_subscription(
+                endpoint,
+                wallet.wallet.user,
+                data.subscription,
+                host,
+            )
+    except Exception as exc:
+        logger.debug(exc)
+        raise HTTPException(
+            HTTPStatus.INTERNAL_SERVER_ERROR,
+            "Cannot create webpush notification",
+        ) from exc
 
 
 @webpush_router.delete("", status_code=HTTPStatus.OK)
 async def api_delete_webpush_subscription(
     request: Request,
     wallet: WalletTypeInfo = Depends(require_admin_key),
 ):
-    endpoint = unquote(
-        base64.b64decode(str(request.query_params.get("endpoint"))).decode("utf-8")
-    )
-    await delete_webpush_subscription(endpoint, wallet.wallet.user)
+    try:
+        endpoint = unquote(
+            base64.b64decode(str(request.query_params.get("endpoint"))).decode("utf-8")
+        )
+        count = await delete_webpush_subscription(endpoint, wallet.wallet.user)
+        return {"count": count}
+    except Exception as exc:
+        logger.debug(exc)
+        raise HTTPException(
+            HTTPStatus.INTERNAL_SERVER_ERROR,
+            "Cannot delete webpush notification",
+        ) from exc
```

### Comparing `lnbits-0.12.7/lnbits/core/views/websocket_api.py` & `lnbits-0.12.8/lnbits/core/views/websocket_api.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/db.py` & `lnbits-0.12.8/lnbits/db.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/decorators.py` & `lnbits-0.12.8/lnbits/decorators.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 from pydantic.types import UUID4
 
 from lnbits.core.crud import (
     get_account,
     get_account_by_email,
     get_account_by_username,
     get_user,
+    get_user_active_extensions_ids,
     get_wallet_for_key,
 )
-from lnbits.core.models import KeyType, User, WalletTypeInfo
+from lnbits.core.models import KeyType, SimpleStatus, User, WalletTypeInfo
 from lnbits.db import Filter, Filters, TFilterModel
 from lnbits.settings import AuthMethods, settings
 
 oauth2_scheme = OAuth2PasswordBearer(tokenUrl="api/v1/auth", auto_error=False)
 
 api_key_header = APIKeyHeader(
     name="X-API-KEY",
@@ -84,24 +85,15 @@
 
         if self.expected_key_type is KeyType.admin and wallet.adminkey != key_value:
             raise HTTPException(
                 status_code=HTTPStatus.UNAUTHORIZED,
                 detail="Invalid adminkey.",
             )
 
-        if (
-            wallet.user != settings.super_user
-            and wallet.user not in settings.lnbits_admin_users
-            and settings.lnbits_admin_extensions
-            and request["path"].split("/")[1] in settings.lnbits_admin_extensions
-        ):
-            raise HTTPException(
-                status_code=HTTPStatus.FORBIDDEN,
-                detail="User not authorized for this extension.",
-            )
+        await _check_user_extension_access(wallet.user, request["path"])
 
         key_type = KeyType.admin if wallet.adminkey == key_value else KeyType.invoice
         return WalletTypeInfo(key_type, wallet)
 
 
 async def get_key_type(
     request: Request,
@@ -157,23 +149,15 @@
 
     if not account or not settings.is_user_allowed(account.id):
         raise HTTPException(HTTPStatus.UNAUTHORIZED, "User not allowed.")
 
     user = await get_user(account.id)
     assert user, "User not found for account."
 
-    if (
-        user.id != settings.super_user
-        and user.id not in settings.lnbits_admin_users
-        and settings.lnbits_admin_extensions
-        and r["path"].split("/")[1] in settings.lnbits_admin_extensions
-    ):
-        raise HTTPException(
-            HTTPStatus.UNAUTHORIZED, "User not authorized for extension."
-        )
+    await _check_user_extension_access(user.id, r["path"])
 
     return user
 
 
 async def check_admin(user: Annotated[User, Depends(check_user_exists)]) -> User:
     if user.id != settings.super_user and user.id not in settings.lnbits_admin_users:
         raise HTTPException(
@@ -222,14 +206,45 @@
             search=search,
             model=model,
         )
 
     return dependency
 
 
+async def check_user_extension_access(user_id: str, ext_id: str) -> SimpleStatus:
+    """
+    Check if the user has access to a particular extension.
+    Raises HTTP Forbidden if the user is not allowed.
+    """
+    if settings.is_admin_extension(ext_id) and not settings.is_admin_user(user_id):
+        return SimpleStatus(
+            success=False, message=f"User not authorized for extension '{ext_id}'."
+        )
+
+    if settings.is_extension_id(ext_id):
+        ext_ids = await get_user_active_extensions_ids(user_id)
+        if ext_id not in ext_ids:
+            return SimpleStatus(
+                success=False, message=f"User extension '{ext_id}' not enabled."
+            )
+
+    return SimpleStatus(success=True, message="OK")
+
+
+async def _check_user_extension_access(user_id: str, current_path: str):
+    path = current_path.split("/")
+    ext_id = path[3] if path[1] == "upgrades" else path[1]
+    status = await check_user_extension_access(user_id, ext_id)
+    if not status.success:
+        raise HTTPException(
+            HTTPStatus.FORBIDDEN,
+            status.message,
+        )
+
+
 async def _get_account_from_token(access_token):
     try:
         payload = jwt.decode(access_token, settings.auth_secret_key, "HS256")
         if "sub" in payload and payload.get("sub"):
             return await get_account_by_username(str(payload.get("sub")))
         if "usr" in payload and payload.get("usr"):
             return await get_account(str(payload.get("usr")))
```

### Comparing `lnbits-0.12.7/lnbits/exceptions.py` & `lnbits-0.12.8/lnbits/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,22 @@
         ):
             response = RedirectResponse("/")
             response.delete_cookie("cookie_access_token")
             response.delete_cookie("is_lnbits_user_authorized")
             response.set_cookie("is_access_token_expired", "true")
             return response
 
+        status_code: int = (
+            exc.status_code
+            if isinstance(exc, HTTPException)
+            else HTTPStatus.INTERNAL_SERVER_ERROR
+        )
+
         return template_renderer().TemplateResponse(
-            request, "error.html", {"err": f"Error: {exc!s}"}
+            request, "error.html", {"err": f"Error: {exc!s}"}, status_code
         )
 
     return None
 
 
 def register_exception_handler(app: FastAPI):
     @app.exception_handler(Exception)
```

### Comparing `lnbits-0.12.7/lnbits/extension_manager.py` & `lnbits-0.12.8/lnbits/extension_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,47 @@
 class ReleasePaymentInfo(BaseModel):
     amount: Optional[int] = None
     pay_link: Optional[str] = None
     payment_hash: Optional[str] = None
     payment_request: Optional[str] = None
 
 
+class PayToEnableInfo(BaseModel):
+    required: Optional[bool] = False
+    amount: Optional[int] = None
+    wallet: Optional[str] = None
+
+
+class UserExtensionInfo(BaseModel):
+    paid_to_enable: Optional[bool] = False
+    payment_hash_to_enable: Optional[str] = None
+
+
+class UserExtension(BaseModel):
+    extension: str
+    active: bool
+    extra: Optional[UserExtensionInfo] = None
+
+    @property
+    def is_paid(self) -> bool:
+        if not self.extra:
+            return False
+        return self.extra.paid_to_enable is True
+
+    @classmethod
+    def from_row(cls, data: dict) -> "UserExtension":
+        ext = UserExtension(**data)
+        ext.extra = (
+            UserExtensionInfo(**json.loads(data["_extra"] or "{}"))
+            if "_extra" in data
+            else None
+        )
+        return ext
+
+
 def download_url(url, save_path):
     with request.urlopen(url, timeout=60) as dl_file:
         with open(save_path, "wb") as out_file:
             out_file.write(dl_file.read())
 
 
 def file_hash(filename):
@@ -231,14 +264,15 @@
     def __init__(self) -> None:
         p = Path(settings.lnbits_extensions_path, "extensions")
         Path(p).mkdir(parents=True, exist_ok=True)
         self._extension_folders: List[Path] = [f for f in p.iterdir() if f.is_dir()]
 
     @property
     def extensions(self) -> List[Extension]:
+        # todo: remove this property somehow, it is too expensive
         output: List[Extension] = []
 
         for extension_folder in self._extension_folders:
             extension_code = extension_folder.parts[-1]
             try:
                 with open(extension_folder / "config.json") as json_file:
                     config = json.load(json_file)
@@ -349,23 +383,25 @@
             logger.warning(e)
             return []
 
 
 class InstallableExtension(BaseModel):
     id: str
     name: str
+    active: Optional[bool] = False
     short_description: Optional[str] = None
     icon: Optional[str] = None
     dependencies: List[str] = []
     is_admin_only: bool = False
     stars: int = 0
     featured = False
     latest_release: Optional[ExtensionRelease] = None
     installed_release: Optional[ExtensionRelease] = None
     payments: List[ReleasePaymentInfo] = []
+    pay_to_enable: Optional[PayToEnableInfo] = None
     archive: Optional[str] = None
 
     @property
     def hash(self) -> str:
         if self.installed_release:
             if self.installed_release.hash:
                 return self.installed_release.hash
@@ -408,14 +444,20 @@
 
     @property
     def installed_version(self) -> str:
         if self.installed_release:
             return self.installed_release.version
         return ""
 
+    @property
+    def requires_payment(self) -> bool:
+        if not self.pay_to_enable:
+            return False
+        return self.pay_to_enable.required is True
+
     async def download_archive(self):
         logger.info(f"Downloading extension {self.name} ({self.installed_version}).")
         ext_zip_file = self.zip_path
         if ext_zip_file.is_file():
             os.remove(ext_zip_file)
         try:
             assert self.installed_release, "installed_release is none."
@@ -475,30 +517,23 @@
                     self.installed_release.source_repo, config_json.get("tile")
                 )
 
         shutil.rmtree(self.ext_dir, True)
         shutil.copytree(Path(self.ext_upgrade_dir), Path(self.ext_dir))
         logger.success(f"Extension {self.name} ({self.installed_version}) installed.")
 
-    def notify_upgrade(self) -> None:
+    def notify_upgrade(self, upgrade_hash: Optional[str]) -> None:
         """
         Update the list of upgraded extensions. The middleware will perform
         redirects based on this
         """
+        if upgrade_hash:
+            settings.lnbits_upgraded_extensions.add(f"{self.hash}/{self.id}")
 
-        clean_upgraded_exts = list(
-            filter(
-                lambda old_ext: not old_ext.endswith(f"/{self.id}"),
-                settings.lnbits_upgraded_extensions,
-            )
-        )
-        settings.lnbits_upgraded_extensions = [
-            *clean_upgraded_exts,
-            f"{self.hash}/{self.id}",
-        ]
+        settings.lnbits_all_extensions_ids.add(self.id)
 
     def clean_extension_files(self):
         # remove downloaded archive
         if self.zip_path.is_file():
             os.remove(self.zip_path)
 
         # remove module from extensions
@@ -551,16 +586,19 @@
 
     @classmethod
     def from_row(cls, data: dict) -> "InstallableExtension":
         meta = json.loads(data["meta"])
         ext = InstallableExtension(**data)
         if "installed_release" in meta:
             ext.installed_release = ExtensionRelease(**meta["installed_release"])
+        if meta.get("pay_to_enable"):
+            ext.pay_to_enable = PayToEnableInfo(**meta["pay_to_enable"])
         if meta.get("payments"):
             ext.payments = [ReleasePaymentInfo(**p) for p in meta["payments"]]
+
         return ext
 
     @classmethod
     def from_rows(
         cls, rows: Optional[List[Any]] = None
     ) -> List["InstallableExtension"]:
         if rows is None:
```

### Comparing `lnbits-0.12.7/lnbits/helpers.py` & `lnbits-0.12.8/lnbits/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     t.env.globals["VOIDWALLET"] = settings.lnbits_backend_wallet_class == "VoidWallet"
     t.env.globals["HIDE_API"] = settings.lnbits_hide_api
     t.env.globals["SITE_TITLE"] = settings.lnbits_site_title
     t.env.globals["LNBITS_DENOMINATION"] = settings.lnbits_denomination
     t.env.globals["SITE_TAGLINE"] = settings.lnbits_site_tagline
     t.env.globals["SITE_DESCRIPTION"] = settings.lnbits_site_description
     t.env.globals["LNBITS_SHOW_HOME_PAGE_ELEMENTS"] = (
-        settings.LNBITS_SHOW_HOME_PAGE_ELEMENTS
+        settings.lnbits_show_home_page_elements
     )
     t.env.globals["LNBITS_CUSTOM_BADGE"] = settings.lnbits_custom_badge
     t.env.globals["LNBITS_CUSTOM_BADGE_COLOR"] = settings.lnbits_custom_badge_color
     t.env.globals["LNBITS_THEME_OPTIONS"] = settings.lnbits_theme_options
     t.env.globals["LNBITS_QR_LOGO"] = settings.lnbits_qr_logo
     t.env.globals["LNBITS_VERSION"] = settings.version
     t.env.globals["LNBITS_NEW_ACCOUNTS_ALLOWED"] = settings.new_accounts_allowed
```

### Comparing `lnbits-0.12.7/lnbits/jinja2_templating.py` & `lnbits-0.12.8/lnbits/jinja2_templating.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/middleware.py` & `lnbits-0.12.8/lnbits/middleware.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/nodes/base.py` & `lnbits-0.12.8/lnbits/nodes/base.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/nodes/cln.py` & `lnbits-0.12.8/lnbits/nodes/cln.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/nodes/lndrest.py` & `lnbits-0.12.8/lnbits/nodes/lndrest.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/server.py` & `lnbits-0.12.8/lnbits/server.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/settings.py` & `lnbits-0.12.8/lnbits/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,20 +59,23 @@
     lnbits_extensions_default_install: list[str] = Field(default=[])
     # required due to GitHUb rate-limit
     lnbits_ext_github_token: str = Field(default="")
 
 
 class InstalledExtensionsSettings(LNbitsSettings):
     # installed extensions that have been deactivated
-    lnbits_deactivated_extensions: list[str] = Field(default=[])
+    lnbits_deactivated_extensions: set[str] = Field(default=[])
     # upgraded extensions that require API redirects
-    lnbits_upgraded_extensions: list[str] = Field(default=[])
+    lnbits_upgraded_extensions: set[str] = Field(default=[])
     # list of redirects that extensions want to perform
     lnbits_extensions_redirects: list[Any] = Field(default=[])
 
+    # list of all extension ids
+    lnbits_all_extensions_ids: set[Any] = Field(default=[])
+
     def extension_upgrade_path(self, ext_id: str) -> Optional[str]:
         return next(
             (e for e in self.lnbits_upgraded_extensions if e.endswith(f"/{ext_id}")),
             None,
         )
 
     def extension_upgrade_hash(self, ext_id: str) -> Optional[str]:
@@ -82,30 +85,30 @@
 
 class ThemesSettings(LNbitsSettings):
     lnbits_site_title: str = Field(default="LNbits")
     lnbits_site_tagline: str = Field(default="free and open-source lightning wallet")
     lnbits_site_description: Optional[str] = Field(
         default="The world's most powerful suite of bitcoin tools."
     )
-    LNBITS_SHOW_HOME_PAGE_ELEMENTS: bool = Field(default=True)
+    lnbits_show_home_page_elements: bool = Field(default=True)
     lnbits_default_wallet_name: str = Field(default="LNbits wallet")
-    lnbits_custom_badge: str = Field(default=None)
+    lnbits_custom_badge: Optional[str] = Field(default=None)
     lnbits_custom_badge_color: str = Field(default="warning")
     lnbits_theme_options: list[str] = Field(
         default=[
             "classic",
             "freedom",
             "mint",
             "salvador",
             "monochrome",
             "autumn",
             "cyber",
         ]
     )
-    lnbits_custom_logo: str = Field(default=None)
+    lnbits_custom_logo: Optional[str] = Field(default=None)
     lnbits_ad_space_title: str = Field(default="Supported by")
     lnbits_ad_space: str = Field(
         default="https://shop.lnbits.com/;/static/images/bitcoin-shop-banner.png;/static/images/bitcoin-shop-banner.png,https://affil.trezor.io/aff_c?offer_id=169&aff_id=33845;/static/images/bitcoin-hardware-wallet.png;/static/images/bitcoin-hardware-wallet.png,https://opensats.org/;/static/images/open-sats.png;/static/images/open-sats.png"
     )  # sneaky sneaky
     lnbits_ad_space_enabled: bool = Field(default=False)
     lnbits_allowed_currencies: list[str] = Field(default=[])
     lnbits_default_accounting_currency: Optional[str] = Field(default=None)
@@ -115,15 +118,15 @@
 class OpsSettings(LNbitsSettings):
     lnbits_baseurl: str = Field(default="http://127.0.0.1:5000/")
     lnbits_reserve_fee_min: int = Field(default=2000)
     lnbits_reserve_fee_percent: float = Field(default=1.0)
     lnbits_service_fee: float = Field(default=0)
     lnbits_service_fee_ignore_internal: bool = Field(default=True)
     lnbits_service_fee_max: int = Field(default=0)
-    lnbits_service_fee_wallet: str = Field(default=None)
+    lnbits_service_fee_wallet: Optional[str] = Field(default=None)
     lnbits_hide_api: bool = Field(default=False)
     lnbits_denomination: str = Field(default="sats")
 
 
 class SecuritySettings(LNbitsSettings):
     lnbits_rate_limit_no: str = Field(default="200")
     lnbits_rate_limit_unit: str = Field(default="minute")
@@ -269,16 +272,16 @@
     SparkFundingSource,
     LnTipsFundingSource,
 ):
     lnbits_backend_wallet_class: str = Field(default="VoidWallet")
 
 
 class WebPushSettings(LNbitsSettings):
-    lnbits_webpush_pubkey: str = Field(default=None)
-    lnbits_webpush_privkey: str = Field(default=None)
+    lnbits_webpush_pubkey: Optional[str] = Field(default=None)
+    lnbits_webpush_privkey: Optional[str] = Field(default=None)
 
 
 class NodeUISettings(LNbitsSettings):
     # on-off switch for node ui
     lnbits_node_ui: bool = Field(default=False)
     # whether to display the public node ui (only if lnbits_node_ui is True)
     lnbits_public_node_ui: bool = Field(default=False)
@@ -477,22 +480,31 @@
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
         case_sensitive = False
         json_loads = list_parse_fallback
 
-    def is_user_allowed(self, user_id: str):
+    def is_user_allowed(self, user_id: str) -> bool:
         return (
             len(self.lnbits_allowed_users) == 0
             or user_id in self.lnbits_allowed_users
             or user_id in self.lnbits_admin_users
             or user_id == self.super_user
         )
 
+    def is_admin_user(self, user_id: str) -> bool:
+        return user_id in self.lnbits_admin_users or user_id == self.super_user
+
+    def is_admin_extension(self, ext_id: str) -> bool:
+        return ext_id in self.lnbits_admin_extensions
+
+    def is_extension_id(self, ext_id: str) -> bool:
+        return ext_id in self.lnbits_all_extensions_ids
+
 
 class SuperSettings(EditableSettings):
     super_user: str
 
 
 class AdminSettings(EditableSettings):
     is_super_user: bool
```

### Comparing `lnbits-0.12.7/lnbits/static/bundle.min.css` & `lnbits-0.12.8/lnbits/static/bundle.min.css`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/bundle.min.js` & `lnbits-0.12.8/lnbits/static/bundle.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -552,23 +552,23 @@
         j[n] = j[n + "s"] = j[t] = e
     }
 
     function I(e) {
         return "string" == typeof e ? j[e] || j[e.toLowerCase()] : void 0
     }
 
-    function F(e) {
+    function B(e) {
         var t, n, i = {};
         for (n in e) a(e, n) && (t = I(n)) && (i[t] = e[n]);
         return i
     }
-    var $ = {};
+    var F = {};
 
-    function B(e, t) {
-        $[e] = t
+    function $(e, t) {
+        F[e] = t
     }
 
     function V(e) {
         return e % 4 == 0 && e % 100 != 0 || e % 400 == 0
     }
 
     function H(e) {
@@ -667,15 +667,15 @@
         return -1
     }, D("M", ["MM", 2], "Mo", (function() {
         return this.month() + 1
     })), D("MMM", 0, 0, (function(e) {
         return this.localeData().monthsShort(this, e)
     })), D("MMMM", 0, 0, (function(e) {
         return this.localeData().months(this, e)
-    })), R("month", "M"), B("month", 8), he("M", te), he("MM", te, Z), he("MMM", (function(e, t) {
+    })), R("month", "M"), $("month", 8), he("M", te), he("MM", te, Z), he("MMM", (function(e, t) {
         return t.monthsShortRegex(e)
     })), he("MMMM", (function(e, t) {
         return t.monthsRegex(e)
     })), ve(["M", "MM"], (function(e, t) {
         t[we] = U(e) - 1
     })), ve(["MMM", "MMMM"], (function(e, t, n, i) {
         var r = n._locale.monthsParse(e, i, n._strict);
@@ -724,38 +724,38 @@
         return V(e) ? 366 : 365
     }
     D("Y", 0, 0, (function() {
         var e = this.year();
         return e <= 9999 ? P(e, 4) : "+" + e
     })), D(0, ["YY", 2], 0, (function() {
         return this.year() % 100
-    })), D(0, ["YYYY", 4], 0, "year"), D(0, ["YYYYY", 5], 0, "year"), D(0, ["YYYYYY", 6, !0], 0, "year"), R("year", "y"), B("year", 1), he("Y", le), he("YY", te, Z), he("YYYY", ae, X), he("YYYYY", oe, ee), he("YYYYYY", oe, ee), ve(["YYYYY", "YYYYYY"], ye), ve("YYYY", (function(e, t) {
+    })), D(0, ["YYYY", 4], 0, "year"), D(0, ["YYYYY", 5], 0, "year"), D(0, ["YYYYYY", 6, !0], 0, "year"), R("year", "y"), $("year", 1), he("Y", le), he("YY", te, Z), he("YYYY", ae, X), he("YYYYY", oe, ee), he("YYYYYY", oe, ee), ve(["YYYYY", "YYYYYY"], ye), ve("YYYY", (function(e, t) {
         t[ye] = 2 === e.length ? n.parseTwoDigitYear(e) : U(e)
     })), ve("YY", (function(e, t) {
         t[ye] = n.parseTwoDigitYear(e)
     })), ve("Y", (function(e, t) {
         t[ye] = parseInt(e, 10)
     })), n.parseTwoDigitYear = function(e) {
         return U(e) + (U(e) > 68 ? 1900 : 2e3)
     };
-    var Fe = W("FullYear", !0);
+    var Be = W("FullYear", !0);
 
-    function $e(e, t, n, i, r, a, o) {
+    function Fe(e, t, n, i, r, a, o) {
         var s;
         return e < 100 && e >= 0 ? (s = new Date(e + 400, t, n, i, r, a, o), isFinite(s.getFullYear()) && s.setFullYear(e)) : s = new Date(e, t, n, i, r, a, o), s
     }
 
-    function Be(e) {
+    function $e(e) {
         var t, n;
         return e < 100 && e >= 0 ? ((n = Array.prototype.slice.call(arguments))[0] = e + 400, t = new Date(Date.UTC.apply(null, n)), isFinite(t.getUTCFullYear()) && t.setUTCFullYear(e)) : t = new Date(Date.UTC.apply(null, arguments)), t
     }
 
     function Ve(e, t, n) {
         var i = 7 + t - n;
-        return -((7 + Be(e, 0, i).getUTCDay() - t) % 7) + i - 1
+        return -((7 + $e(e, 0, i).getUTCDay() - t) % 7) + i - 1
     }
 
     function He(e, t, n, i, r) {
         var a, o, s = 1 + 7 * (t - 1) + (7 + n - i) % 7 + Ve(e, i, r);
         return s <= 0 ? o = Ie(a = e - 1) + s : s > Ie(e) ? (a = e + 1, o = s - Ie(e)) : (a = e, o = s), {
             year: a,
             dayOfYear: o
@@ -772,28 +772,28 @@
     }
 
     function We(e, t, n) {
         var i = Ve(e, t, n),
             r = Ve(e + 1, t, n);
         return (Ie(e) - i + r) / 7
     }
-    D("w", ["ww", 2], "wo", "week"), D("W", ["WW", 2], "Wo", "isoWeek"), R("week", "w"), R("isoWeek", "W"), B("week", 5), B("isoWeek", 5), he("w", te), he("ww", te, Z), he("W", te), he("WW", te, Z), ge(["w", "ww", "W", "WW"], (function(e, t, n, i) {
+    D("w", ["ww", 2], "wo", "week"), D("W", ["WW", 2], "Wo", "isoWeek"), R("week", "w"), R("isoWeek", "W"), $("week", 5), $("isoWeek", 5), he("w", te), he("ww", te, Z), he("W", te), he("WW", te, Z), ge(["w", "ww", "W", "WW"], (function(e, t, n, i) {
         t[i.substr(0, 1)] = U(e)
     }));
 
     function Ye(e, t) {
         return e.slice(t, 7).concat(e.slice(0, t))
     }
     D("d", 0, "do", "day"), D("dd", 0, 0, (function(e) {
         return this.localeData().weekdaysMin(this, e)
     })), D("ddd", 0, 0, (function(e) {
         return this.localeData().weekdaysShort(this, e)
     })), D("dddd", 0, 0, (function(e) {
         return this.localeData().weekdays(this, e)
-    })), D("e", 0, 0, "weekday"), D("E", 0, 0, "isoWeekday"), R("day", "d"), R("weekday", "e"), R("isoWeekday", "E"), B("day", 11), B("weekday", 11), B("isoWeekday", 11), he("d", te), he("e", te), he("E", te), he("dd", (function(e, t) {
+    })), D("e", 0, 0, "weekday"), D("E", 0, 0, "isoWeekday"), R("day", "d"), R("weekday", "e"), R("isoWeekday", "E"), $("day", 11), $("weekday", 11), $("isoWeekday", 11), he("d", te), he("e", te), he("E", te), he("dd", (function(e, t) {
         return t.weekdaysMinRegex(e)
     })), he("ddd", (function(e, t) {
         return t.weekdaysShortRegex(e)
     })), he("dddd", (function(e, t) {
         return t.weekdaysRegex(e)
     })), ge(["dd", "ddd", "dddd"], (function(e, t, n, i) {
         var r = n._locale.weekdaysParse(e, i, n._strict);
@@ -846,15 +846,15 @@
         return "" + nt.apply(this) + P(this.minutes(), 2)
     })), D("hmmss", 0, 0, (function() {
         return "" + nt.apply(this) + P(this.minutes(), 2) + P(this.seconds(), 2)
     })), D("Hmm", 0, 0, (function() {
         return "" + this.hours() + P(this.minutes(), 2)
     })), D("Hmmss", 0, 0, (function() {
         return "" + this.hours() + P(this.minutes(), 2) + P(this.seconds(), 2)
-    })), it("a", !0), it("A", !1), R("hour", "h"), B("hour", 13), he("a", rt), he("A", rt), he("H", te), he("h", te), he("k", te), he("HH", te, Z), he("hh", te, Z), he("kk", te, Z), he("hmm", ne), he("hmmss", ie), he("Hmm", ne), he("Hmmss", ie), ve(["H", "HH"], xe), ve(["k", "kk"], (function(e, t, n) {
+    })), it("a", !0), it("A", !1), R("hour", "h"), $("hour", 13), he("a", rt), he("A", rt), he("H", te), he("h", te), he("k", te), he("HH", te, Z), he("hh", te, Z), he("kk", te, Z), he("hmm", ne), he("hmmss", ie), he("Hmm", ne), he("Hmmss", ie), ve(["H", "HH"], xe), ve(["k", "kk"], (function(e, t, n) {
         var i = U(e);
         t[xe] = 24 === i ? 0 : i
     })), ve(["a", "A"], (function(e, t, n) {
         n._isPm = n._locale.isPM(e), n._meridiem = e
     })), ve(["h", "hh"], (function(e, t, n) {
         t[xe] = U(e), f(n).bigHour = !0
     })), ve("hmm", (function(e, t, n) {
@@ -1080,15 +1080,15 @@
                 }(c[1], t, e)) return;
             e._a = t, e._tzm = function(e, t, n) {
                 if (e) return St[e];
                 if (t) return 0;
                 var i = parseInt(n, 10),
                     r = i % 100;
                 return (i - r) / 100 * 60 + r
-            }(c[8], c[9], c[10]), e._d = Be.apply(null, e._a), e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), f(e).rfc2822 = !0
+            }(c[8], c[9], c[10]), e._d = $e.apply(null, e._a), e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), f(e).rfc2822 = !0
         } else e._isValid = !1
     }
 
     function At(e, t, n) {
         return null != e ? e : null != t ? t : n
     }
 
@@ -1098,17 +1098,17 @@
             for (r = function(e) {
                     var t = new Date(n.now());
                     return e._useUTC ? [t.getUTCFullYear(), t.getUTCMonth(), t.getUTCDate()] : [t.getFullYear(), t.getMonth(), t.getDate()]
                 }(e), e._w && null == e._a[ke] && null == e._a[we] && function(e) {
                     var t, n, i, r, a, o, s, l, c;
                     t = e._w, null != t.GG || null != t.W || null != t.E ? (a = 1, o = 4, n = At(t.GG, e._a[ye], Ue(Et(), 1, 4).year), i = At(t.W, 1), ((r = At(t.E, 1)) < 1 || r > 7) && (l = !0)) : (a = e._locale._week.dow, o = e._locale._week.doy, c = Ue(Et(), a, o), n = At(t.gg, e._a[ye], c.year), i = At(t.w, c.week), null != t.d ? ((r = t.d) < 0 || r > 6) && (l = !0) : null != t.e ? (r = t.e + a, (t.e < 0 || t.e > 6) && (l = !0)) : r = a);
                     i < 1 || i > We(n, a, o) ? f(e)._overflowWeeks = !0 : null != l ? f(e)._overflowWeekday = !0 : (s = He(n, i, r, a, o), e._a[ye] = s.year, e._dayOfYear = s.dayOfYear)
-                }(e), null != e._dayOfYear && (o = At(e._a[ye], r[ye]), (e._dayOfYear > Ie(o) || 0 === e._dayOfYear) && (f(e)._overflowDayOfYear = !0), i = Be(o, 0, e._dayOfYear), e._a[we] = i.getUTCMonth(), e._a[ke] = i.getUTCDate()), t = 0; t < 3 && null == e._a[t]; ++t) e._a[t] = s[t] = r[t];
+                }(e), null != e._dayOfYear && (o = At(e._a[ye], r[ye]), (e._dayOfYear > Ie(o) || 0 === e._dayOfYear) && (f(e)._overflowDayOfYear = !0), i = $e(o, 0, e._dayOfYear), e._a[we] = i.getUTCMonth(), e._a[ke] = i.getUTCDate()), t = 0; t < 3 && null == e._a[t]; ++t) e._a[t] = s[t] = r[t];
             for (; t < 7; t++) e._a[t] = s[t] = null == e._a[t] ? 2 === t ? 1 : 0 : e._a[t];
-            24 === e._a[xe] && 0 === e._a[Se] && 0 === e._a[Ce] && 0 === e._a[Me] && (e._nextDay = !0, e._a[xe] = 0), e._d = (e._useUTC ? Be : $e).apply(null, s), a = e._useUTC ? e._d.getUTCDay() : e._d.getDay(), null != e._tzm && e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), e._nextDay && (e._a[xe] = 24), e._w && void 0 !== e._w.d && e._w.d !== a && (f(e).weekdayMismatch = !0)
+            24 === e._a[xe] && 0 === e._a[Se] && 0 === e._a[Ce] && 0 === e._a[Me] && (e._nextDay = !0, e._a[xe] = 0), e._d = (e._useUTC ? $e : Fe).apply(null, s), a = e._useUTC ? e._d.getUTCDay() : e._d.getDay(), null != e._tzm && e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), e._nextDay && (e._a[xe] = 24), e._w && void 0 !== e._w.d && e._w.d !== a && (f(e).weekdayMismatch = !0)
         }
     }
 
     function Lt(e) {
         if (e._f !== n.ISO_8601)
             if (e._f !== n.RFC_2822) {
                 e._a = [], f(e).empty = !0;
@@ -1141,15 +1141,15 @@
             s(t) ? e._d = new Date(n.now()) : c(t) ? e._d = new Date(t.valueOf()) : "string" == typeof t ? function(e) {
                 var t = kt.exec(e._i);
                 null === t ? (Ct(e), !1 === e._isValid && (delete e._isValid, Tt(e), !1 === e._isValid && (delete e._isValid, e._strict ? e._isValid = !1 : n.createFromInputFallback(e)))) : e._d = new Date(+t[1])
             }(e) : i(t) ? (e._a = u(t.slice(0), (function(e) {
                 return parseInt(e, 10)
             })), Pt(e)) : r(t) ? function(e) {
                 if (!e._d) {
-                    var t = F(e._i),
+                    var t = B(e._i),
                         n = void 0 === t.day ? t.date : t.day;
                     e._a = u([t.year, t.month, n, t.hour, t.minute, t.second, t.millisecond], (function(e) {
                         return e && parseInt(e, 10)
                     })), Pt(e)
                 }
             }(e) : l(t) ? e._d = new Date(t) : n.createFromInputFallback(e)
         }(e), p(e) || (e._d = null), e))
@@ -1180,15 +1180,15 @@
         if (1 === t.length && i(t[0]) && (t = t[0]), !t.length) return Et();
         for (n = t[0], r = 1; r < t.length; ++r) t[r].isValid() && !t[r][e](n) || (n = t[r]);
         return n
     }
     var jt = ["year", "quarter", "month", "week", "day", "hour", "minute", "second", "millisecond"];
 
     function Rt(e) {
-        var t = F(e),
+        var t = B(e),
             n = t.year || 0,
             i = t.quarter || 0,
             r = t.month || 0,
             o = t.week || t.isoWeek || 0,
             s = t.day || 0,
             l = t.hour || 0,
             c = t.minute || 0,
@@ -1207,33 +1207,33 @@
         }(t), this._milliseconds = +d + 1e3 * u + 6e4 * c + 1e3 * l * 60 * 60, this._days = +s + 7 * o, this._months = +r + 3 * i + 12 * n, this._data = {}, this._locale = mt(), this._bubble()
     }
 
     function It(e) {
         return e instanceof Rt
     }
 
-    function Ft(e) {
+    function Bt(e) {
         return e < 0 ? -1 * Math.round(-1 * e) : Math.round(e)
     }
 
-    function $t(e, t) {
+    function Ft(e, t) {
         D(e, 0, 0, (function() {
             var e = this.utcOffset(),
                 n = "+";
             return e < 0 && (e = -e, n = "-"), n + P(~~(e / 60), 2) + t + P(~~e % 60, 2)
         }))
     }
-    $t("Z", ":"), $t("ZZ", ""), he("Z", ue), he("ZZ", ue), ve(["Z", "ZZ"], (function(e, t, n) {
+    Ft("Z", ":"), Ft("ZZ", ""), he("Z", ue), he("ZZ", ue), ve(["Z", "ZZ"], (function(e, t, n) {
         n._useUTC = !0, n._tzm = Vt(ue, e)
     }));
-    var Bt = /([\+\-]|\d\d)/gi;
+    var $t = /([\+\-]|\d\d)/gi;
 
     function Vt(e, t) {
         var n, i, r = (t || "").match(e);
-        return null === r ? null : 0 === (i = 60 * (n = ((r[r.length - 1] || []) + "").match(Bt) || ["-", 0, 0])[1] + U(n[2])) ? 0 : "+" === n[0] ? i : -i
+        return null === r ? null : 0 === (i = 60 * (n = ((r[r.length - 1] || []) + "").match($t) || ["-", 0, 0])[1] + U(n[2])) ? 0 : "+" === n[0] ? i : -i
     }
 
     function Ht(e, t) {
         var i, r;
         return t._isUTC ? (i = t.clone(), r = (y(e) || c(e) ? e.valueOf() : Et(e).valueOf()) - i.valueOf(), i._d.setTime(i._d.valueOf() + r), n.updateOffset(i, !1), i) : Et(e).local()
     }
 
@@ -1257,15 +1257,15 @@
             M: e._months
         } : l(e) || !isNaN(+e) ? (o = {}, t ? o[t] = +e : o.milliseconds = +e) : (s = Yt.exec(e)) ? (n = "-" === s[1] ? -1 : 1, o = {
             y: 0,
             d: U(s[ke]) * n,
             h: U(s[xe]) * n,
             m: U(s[Se]) * n,
             s: U(s[Ce]) * n,
-            ms: U(Ft(1e3 * s[Me])) * n
+            ms: U(Bt(1e3 * s[Me])) * n
         }) : (s = Qt.exec(e)) ? (n = "-" === s[1] ? -1 : 1, o = {
             y: Kt(s[2], n),
             M: Kt(s[3], n),
             w: Kt(s[4], n),
             d: Kt(s[5], n),
             h: Kt(s[6], n),
             m: Kt(s[7], n),
@@ -1296,16 +1296,16 @@
             var r;
             return null === i || isNaN(+i) || (C(t, "moment()." + t + "(period, number) is deprecated. Please use moment()." + t + "(number, period). See http://momentjs.com/guides/#/warnings/add-inverted-param/ for more info."), r = n, n = i, i = r), Xt(this, Gt(n, i), e), this
         }
     }
 
     function Xt(e, t, i, r) {
         var a = t._milliseconds,
-            o = Ft(t._days),
-            s = Ft(t._months);
+            o = Bt(t._days),
+            s = Bt(t._months);
         e.isValid() && (r = null == r || r, s && Ne(e, Y(e, "Month") + s * i), o && Q(e, "Date", Y(e, "Date") + o * i), a && e._d.setTime(e._d.valueOf() + a * i), r && n.updateOffset(e, o || s))
     }
     Gt.fn = Rt.prototype, Gt.invalid = function() {
         return Gt(NaN)
     };
     var en = Jt(1, "add"),
         tn = Jt(-1, "subtract");
@@ -1389,15 +1389,15 @@
     function bn(e, t, n, i, r) {
         var a;
         return null == e ? Ue(this, i, r).year : (t > (a = We(e, i, r)) && (t = a), yn.call(this, e, t, n, i, r))
     }
 
     function yn(e, t, n, i, r) {
         var a = He(e, t, n, i, r),
-            o = Be(a.year, 0, a.dayOfYear);
+            o = $e(a.year, 0, a.dayOfYear);
         return this.year(o.getUTCFullYear()), this.month(o.getUTCMonth()), this.date(o.getUTCDate()), this
     }
     D("N", 0, 0, "eraAbbr"), D("NN", 0, 0, "eraAbbr"), D("NNN", 0, 0, "eraAbbr"), D("NNNN", 0, 0, "eraName"), D("NNNNN", 0, 0, "eraNarrow"), D("y", ["y", 1], "yo", "eraYear"), D("y", ["yy", 2], 0, "eraYear"), D("y", ["yyy", 3], 0, "eraYear"), D("y", ["yyyy", 4], 0, "eraYear"), he("N", vn), he("NN", vn), he("NNN", vn), he("NNNN", (function(e, t) {
         return t.erasNameRegex(e)
     })), he("NNNNN", (function(e, t) {
         return t.erasNarrowRegex(e)
     })), ve(["N", "NN", "NNN", "NNNN", "NNNNN"], (function(e, t, n, i) {
@@ -1408,31 +1408,31 @@
     })), ve(["y", "yy", "yyy", "yyyy"], ye), ve(["yo"], (function(e, t, n, i) {
         var r;
         n._locale._eraYearOrdinalRegex && (r = e.match(n._locale._eraYearOrdinalRegex)), n._locale.eraYearOrdinalParse ? t[ye] = n._locale.eraYearOrdinalParse(e, r) : t[ye] = parseInt(e, 10)
     })), D(0, ["gg", 2], 0, (function() {
         return this.weekYear() % 100
     })), D(0, ["GG", 2], 0, (function() {
         return this.isoWeekYear() % 100
-    })), _n("gggg", "weekYear"), _n("ggggg", "weekYear"), _n("GGGG", "isoWeekYear"), _n("GGGGG", "isoWeekYear"), R("weekYear", "gg"), R("isoWeekYear", "GG"), B("weekYear", 1), B("isoWeekYear", 1), he("G", le), he("g", le), he("GG", te, Z), he("gg", te, Z), he("GGGG", ae, X), he("gggg", ae, X), he("GGGGG", oe, ee), he("ggggg", oe, ee), ge(["gggg", "ggggg", "GGGG", "GGGGG"], (function(e, t, n, i) {
+    })), _n("gggg", "weekYear"), _n("ggggg", "weekYear"), _n("GGGG", "isoWeekYear"), _n("GGGGG", "isoWeekYear"), R("weekYear", "gg"), R("isoWeekYear", "GG"), $("weekYear", 1), $("isoWeekYear", 1), he("G", le), he("g", le), he("GG", te, Z), he("gg", te, Z), he("GGGG", ae, X), he("gggg", ae, X), he("GGGGG", oe, ee), he("ggggg", oe, ee), ge(["gggg", "ggggg", "GGGG", "GGGGG"], (function(e, t, n, i) {
         t[i.substr(0, 2)] = U(e)
     })), ge(["gg", "GG"], (function(e, t, i, r) {
         t[r] = n.parseTwoDigitYear(e)
-    })), D("Q", 0, "Qo", "quarter"), R("quarter", "Q"), B("quarter", 7), he("Q", K), ve("Q", (function(e, t) {
+    })), D("Q", 0, "Qo", "quarter"), R("quarter", "Q"), $("quarter", 7), he("Q", K), ve("Q", (function(e, t) {
         t[we] = 3 * (U(e) - 1)
-    })), D("D", ["DD", 2], "Do", "date"), R("date", "D"), B("date", 9), he("D", te), he("DD", te, Z), he("Do", (function(e, t) {
+    })), D("D", ["DD", 2], "Do", "date"), R("date", "D"), $("date", 9), he("D", te), he("DD", te, Z), he("Do", (function(e, t) {
         return e ? t._dayOfMonthOrdinalParse || t._ordinalParse : t._dayOfMonthOrdinalParseLenient
     })), ve(["D", "DD"], ke), ve("Do", (function(e, t) {
         t[ke] = U(e.match(te)[0])
     }));
     var wn = W("Date", !0);
-    D("DDD", ["DDDD", 3], "DDDo", "dayOfYear"), R("dayOfYear", "DDD"), B("dayOfYear", 4), he("DDD", re), he("DDDD", J), ve(["DDD", "DDDD"], (function(e, t, n) {
+    D("DDD", ["DDDD", 3], "DDDo", "dayOfYear"), R("dayOfYear", "DDD"), $("dayOfYear", 4), he("DDD", re), he("DDDD", J), ve(["DDD", "DDDD"], (function(e, t, n) {
         n._dayOfYear = U(e)
-    })), D("m", ["mm", 2], 0, "minute"), R("minute", "m"), B("minute", 14), he("m", te), he("mm", te, Z), ve(["m", "mm"], Se);
+    })), D("m", ["mm", 2], 0, "minute"), R("minute", "m"), $("minute", 14), he("m", te), he("mm", te, Z), ve(["m", "mm"], Se);
     var kn = W("Minutes", !1);
-    D("s", ["ss", 2], 0, "second"), R("second", "s"), B("second", 15), he("s", te), he("ss", te, Z), ve(["s", "ss"], Ce);
+    D("s", ["ss", 2], 0, "second"), R("second", "s"), $("second", 15), he("s", te), he("ss", te, Z), ve(["s", "ss"], Ce);
     var xn, Sn, Cn = W("Seconds", !1);
     for (D("S", 0, 0, (function() {
             return ~~(this.millisecond() / 100)
         })), D(0, ["SS", 2], 0, (function() {
             return ~~(this.millisecond() / 10)
         })), D(0, ["SSS", 3], 0, "millisecond"), D(0, ["SSSS", 4], 0, (function() {
             return 10 * this.millisecond()
@@ -1442,15 +1442,15 @@
             return 1e3 * this.millisecond()
         })), D(0, ["SSSSSSS", 7], 0, (function() {
             return 1e4 * this.millisecond()
         })), D(0, ["SSSSSSSS", 8], 0, (function() {
             return 1e5 * this.millisecond()
         })), D(0, ["SSSSSSSSS", 9], 0, (function() {
             return 1e6 * this.millisecond()
-        })), R("millisecond", "ms"), B("millisecond", 16), he("S", re, K), he("SS", re, Z), he("SSS", re, J), xn = "SSSS"; xn.length <= 9; xn += "S") he(xn, se);
+        })), R("millisecond", "ms"), $("millisecond", 16), he("S", re, K), he("SS", re, Z), he("SSS", re, J), xn = "SSSS"; xn.length <= 9; xn += "S") he(xn, se);
 
     function Mn(e, t) {
         t[Me] = U(1e3 * ("0." + e))
     }
     for (xn = "S"; xn.length <= 9; xn += "S") ve(xn, Mn);
     Sn = W("Milliseconds", !1), D("z", 0, 0, "zoneAbbr"), D("zz", 0, 0, "zoneName");
     var Tn = b.prototype;
@@ -1584,20 +1584,20 @@
         return d({}, f(this))
     }, Tn.set = function(e, t) {
         if ("object" == typeof e) {
             var n, i = function(e) {
                     var t, n = [];
                     for (t in e) a(e, t) && n.push({
                         unit: t,
-                        priority: $[t]
+                        priority: F[t]
                     });
                     return n.sort((function(e, t) {
                         return e.priority - t.priority
                     })), n
-                }(e = F(e)),
+                }(e = B(e)),
                 r = i.length;
             for (n = 0; n < r; n++) this[i[n].unit](e[i[n].unit])
         } else if (M(this[e = I(e)])) return this[e](t);
         return this
     }, Tn.startOf = function(e) {
         var t, i;
         if (void 0 === (e = I(e)) || "millisecond" === e || !this.isValid()) return this;
@@ -1697,15 +1697,15 @@
         }
         return ""
     }, Tn.eraYear = function() {
         var e, t, i, r, a = this.localeData().eras();
         for (e = 0, t = a.length; e < t; ++e)
             if (i = a[e].since <= a[e].until ? 1 : -1, r = this.clone().startOf("day").valueOf(), a[e].since <= r && r <= a[e].until || a[e].until <= r && r <= a[e].since) return (this.year() - n(a[e].since).year()) * i + a[e].offset;
         return this.year()
-    }, Tn.year = Fe, Tn.isLeapYear = function() {
+    }, Tn.year = Be, Tn.isLeapYear = function() {
         return V(this.year())
     }, Tn.weekYear = function(e) {
         return bn.call(this, e, this.week(), this.weekday(), this.localeData()._week.dow, this.localeData()._week.doy)
     }, Tn.isoWeekYear = function(e) {
         return bn.call(this, e, this.isoWeek(), this.isoWeekday(), 1, 4)
     }, Tn.quarter = Tn.quarters = function(e) {
         return null == e ? Math.ceil((this.month() + 1) / 3) : this.month(3 * (e - 1) + this.month() % 3)
@@ -1778,15 +1778,15 @@
         return !!this.isValid() && !this._isUTC
     }, Tn.isUtcOffset = function() {
         return !!this.isValid() && this._isUTC
     }, Tn.isUtc = Wt, Tn.isUTC = Wt, Tn.zoneAbbr = function() {
         return this._isUTC ? "UTC" : ""
     }, Tn.zoneName = function() {
         return this._isUTC ? "Coordinated Universal Time" : ""
-    }, Tn.dates = k("dates accessor is deprecated. Use date instead.", wn), Tn.months = k("months accessor is deprecated. Use month instead", je), Tn.years = k("years accessor is deprecated. Use year instead", Fe), Tn.zone = k("moment().zone is deprecated, use moment().utcOffset instead. http://momentjs.com/guides/#/warnings/zone/", (function(e, t) {
+    }, Tn.dates = k("dates accessor is deprecated. Use date instead.", wn), Tn.months = k("months accessor is deprecated. Use month instead", je), Tn.years = k("years accessor is deprecated. Use year instead", Be), Tn.zone = k("moment().zone is deprecated, use moment().utcOffset instead. http://momentjs.com/guides/#/warnings/zone/", (function(e, t) {
         return null != e ? ("string" != typeof e && (e = -e), this.utcOffset(e, t), this) : -this.utcOffset()
     })), Tn.isDSTShifted = k("isDSTShifted is deprecated. See http://momentjs.com/guides/#/warnings/dst-shifted/ for more information", (function() {
         if (!s(this._isDSTShifted)) return this._isDSTShifted;
         var e, t = {};
         return _(t, this), (t = qt(t))._a ? (e = t._isUTC ? h(t._a) : Et(t._a), this._isDSTShifted = this.isValid() && function(e, t, n) {
             var i, r = Math.min(e.length, t.length),
                 a = Math.abs(e.length - t.length),
@@ -1970,17 +1970,17 @@
 
     function Rn(e) {
         return function() {
             return this.as(e)
         }
     }
     var In = Rn("ms"),
-        Fn = Rn("s"),
-        $n = Rn("m"),
-        Bn = Rn("h"),
+        Bn = Rn("s"),
+        Fn = Rn("m"),
+        $n = Rn("h"),
         Vn = Rn("d"),
         Hn = Rn("w"),
         Un = Rn("M"),
         Wn = Rn("Q"),
         Yn = Rn("y");
 
     function Qn(e) {
@@ -2055,15 +2055,15 @@
                 case "second":
                     return 86400 * t + i / 1e3;
                 case "millisecond":
                     return Math.floor(864e5 * t) + i;
                 default:
                     throw new Error("Unknown unit " + e)
             }
-        }, li.asMilliseconds = In, li.asSeconds = Fn, li.asMinutes = $n, li.asHours = Bn, li.asDays = Vn, li.asWeeks = Hn, li.asMonths = Un, li.asQuarters = Wn, li.asYears = Yn, li.valueOf = function() {
+        }, li.asMilliseconds = In, li.asSeconds = Bn, li.asMinutes = Fn, li.asHours = $n, li.asDays = Vn, li.asWeeks = Hn, li.asMonths = Un, li.asQuarters = Wn, li.asYears = Yn, li.valueOf = function() {
             return this.isValid() ? this._milliseconds + 864e5 * this._days + this._months % 12 * 2592e6 + 31536e6 * U(this._months / 12) : NaN
         }, li._bubble = function() {
             var e, t, n, i, r, a = this._milliseconds,
                 o = this._days,
                 s = this._months,
                 l = this._data;
             return a >= 0 && o >= 0 && s >= 0 || a <= 0 && o <= 0 && s <= 0 || (a += 864e5 * zn(jn(s) + o), o = 0, s = 0), l.milliseconds = a % 1e3, e = H(a / 1e3), l.seconds = e % 60, t = H(e / 60), l.minutes = t % 60, n = H(t / 60), l.hours = n % 24, o += H(n / 24), s += r = H(Nn(o)), o -= zn(jn(r)), i = H(s / 12), s %= 12, l.days = o, l.months = s, l.years = i, this
@@ -2227,26 +2227,26 @@
         z = S("Object"),
         N = u && z(new DataView(new ArrayBuffer(8))),
         j = "undefined" != typeof Map && z(new Map),
         R = S("DataView");
     var I = N ? function(e) {
             return null != e && D(e.getInt8) && q(e.buffer)
         } : R,
-        F = d || S("Array");
+        B = d || S("Array");
 
-    function $(e, t) {
+    function F(e, t) {
         return null != e && l.call(e, t)
     }
-    var B = S("Arguments");
+    var $ = S("Arguments");
     ! function() {
-        B(arguments) || (B = function(e) {
-            return $(e, "callee")
+        $(arguments) || ($ = function(e) {
+            return F(e, "callee")
         })
     }();
-    var V = B;
+    var V = $;
 
     function H(e) {
         return M(e) && m(e)
     }
 
     function U(e) {
         return function() {
@@ -2286,22 +2286,22 @@
                 }
             }
         }(t);
         var n = _.length,
             r = e.constructor,
             a = D(r) && r.prototype || i,
             o = "constructor";
-        for ($(e, o) && !t.contains(o) && t.push(o); n--;)(o = _[n]) in e && e[o] !== a[o] && !t.contains(o) && t.push(o)
+        for (F(e, o) && !t.contains(o) && t.push(o); n--;)(o = _[n]) in e && e[o] !== a[o] && !t.contains(o) && t.push(o)
     }
 
     function ee(e) {
         if (!w(e)) return [];
         if (h) return h(e);
         var t = [];
-        for (var n in e) $(e, n) && t.push(n);
+        for (var n in e) F(e, n) && t.push(n);
         return g && X(e, t), t
     }
 
     function te(e, t) {
         var n = ee(t),
             i = n.length;
         if (null == e) return !i;
@@ -2376,15 +2376,15 @@
             if ((u = e.length) !== t.length) return !1;
             for (; u--;)
                 if (!ae(e[u], t[u], n, i)) return !1
         } else {
             var d, h = ee(e);
             if (u = h.length, ee(t).length !== u) return !1;
             for (; u--;)
-                if (!$(t, d = h[u]) || !ae(e[d], t[d], n, i)) return !1
+                if (!F(t, d = h[u]) || !ae(e[d], t[d], n, i)) return !1
         }
         return n.pop(), i.pop(), !0
     }
 
     function se(e) {
         if (!w(e)) return [];
         var t = [];
@@ -2452,15 +2452,15 @@
         var t = function() {};
         t.prototype = e;
         var n = new t;
         return t.prototype = null, n
     }
 
     function Te(e) {
-        return F(e) ? e : [e]
+        return B(e) ? e : [e]
     }
 
     function Ae(e) {
         return ne.toPath(e)
     }
 
     function Pe(e, t) {
@@ -2512,15 +2512,15 @@
         }
         return function() {
             return e.apply(t, arguments)
         }
     }
 
     function ze(e, t, n) {
-        return null == e ? qe : D(e) ? De(e, t, n) : w(e) && !F(e) ? Oe(e) : Ee(e)
+        return null == e ? qe : D(e) ? De(e, t, n) : w(e) && !B(e) ? Oe(e) : Ee(e)
     }
 
     function Ne(e, t) {
         return ze(e, t, 1 / 0)
     }
 
     function je(e, t, n) {
@@ -2529,39 +2529,39 @@
 
     function Re() {}
 
     function Ie(e, t) {
         return null == t && (t = e, e = 0), e + Math.floor(Math.random() * (t - e + 1))
     }
     ne.toPath = Te, ne.iteratee = Ne;
-    var Fe = Date.now || function() {
+    var Be = Date.now || function() {
         return (new Date).getTime()
     };
 
-    function $e(e) {
+    function Fe(e) {
         var t = function(t) {
                 return e[t]
             },
             n = "(?:" + ee(e).join("|") + ")",
             i = RegExp(n),
             r = RegExp(n, "g");
         return function(e) {
             return e = null == e ? "" : "" + e, i.test(e) ? e.replace(r, t) : e
         }
     }
-    var Be = {
+    var $e = {
             "&": "&amp;",
             "<": "&lt;",
             ">": "&gt;",
             '"': "&quot;",
             "'": "&#x27;",
             "`": "&#x60;"
         },
-        Ve = $e(Be),
-        He = $e(ye(Be)),
+        Ve = Fe($e),
+        He = Fe(ye($e)),
         Ue = ne.templateSettings = {
             evaluate: /<%([\s\S]+?)%>/g,
             interpolate: /<%=([\s\S]+?)%>/g,
             escape: /<%-([\s\S]+?)%>/g
         },
         We = /(.)^/,
         Ye = {
@@ -2607,15 +2607,15 @@
 
     function nt(e, t, n, i) {
         if (i = i || [], t || 0 === t) {
             if (t <= 0) return i.concat(e)
         } else t = 1 / 0;
         for (var r = i.length, a = 0, o = J(e); a < o; a++) {
             var s = e[a];
-            if (tt(s) && (F(s) || V(s)))
+            if (tt(s) && (B(s) || V(s)))
                 if (t > 1) nt(s, t - 1, n, i), r = i.length;
                 else
                     for (var l = 0, c = s.length; l < c;) i[r++] = s[l++];
             else n || (i[r++] = s)
         }
         return i
     }
@@ -2785,15 +2785,15 @@
             ((r = t(e, n, i)) > o || r === -1 / 0 && a === -1 / 0) && (a = e, o = r)
         }));
         return a
     }
     var Lt = /[^\ud800-\udfff]|[\ud800-\udbff][\udc00-\udfff]|[\ud800-\udfff]/g;
 
     function qt(e) {
-        return e ? F(e) ? o.call(e) : C(e) ? e.match(Lt) : tt(e) ? bt(e, qe) : be(e) : []
+        return e ? B(e) ? o.call(e) : C(e) ? e.match(Lt) : tt(e) ? bt(e, qe) : be(e) : []
     }
 
     function Ot(e, t, n) {
         if (null == t || n) return tt(e) || (e = be(e)), e[Ie(e.length - 1)];
         var i = qt(e),
             r = J(i);
         t = Math.max(Math.min(t, r), 0);
@@ -2814,21 +2814,21 @@
             return i = je(i, r), _t(n, (function(t, r) {
                 var o = i(t, r, n);
                 e(a, t, o)
             })), a
         }
     }
     var Dt = Et((function(e, t, n) {
-            $(e, n) ? e[n].push(t) : e[n] = [t]
+            F(e, n) ? e[n].push(t) : e[n] = [t]
         })),
         zt = Et((function(e, t, n) {
             e[n] = t
         })),
         Nt = Et((function(e, t, n) {
-            $(e, n) ? e[n]++ : e[n] = 1
+            F(e, n) ? e[n]++ : e[n] = 1
         })),
         jt = Et((function(e, t, n) {
             e[n ? 0 : 1].push(t)
         }), !0);
 
     function Rt(e, t, n) {
         return t in n
@@ -2841,27 +2841,27 @@
             for (var r = 0, a = t.length; r < a; r++) {
                 var o = t[r],
                     s = e[o];
                 i(s, o, e) && (n[o] = s)
             }
             return n
         })),
-        Ft = y((function(e, t) {
+        Bt = y((function(e, t) {
             var n, i = t[0];
             return D(i) ? (i = ot(i), t.length > 1 && (n = t[1])) : (t = bt(nt(t, !1, !1), String), i = function(e, n) {
                 return !Mt(t, n)
             }), It(e, i, n)
         }));
 
-    function $t(e, t, n) {
+    function Ft(e, t, n) {
         return o.call(e, 0, Math.max(0, e.length - (null == t || n ? 1 : t)))
     }
 
-    function Bt(e, t, n) {
-        return null == e || e.length < 1 ? null == t || n ? void 0 : [] : null == t || n ? e[0] : $t(e, e.length - t)
+    function $t(e, t, n) {
+        return null == e || e.length < 1 ? null == t || n ? void 0 : [] : null == t || n ? e[0] : Ft(e, e.length - t)
     }
 
     function Vt(e, t, n) {
         return o.call(e, null == t || n ? 1 : t)
     }
     var Ht = y((function(e, t) {
             return t = nt(t, !0, !0), xt(e, (function(e) {
@@ -2934,26 +2934,26 @@
             isNumber: M,
             isDate: T,
             isRegExp: A,
             isError: P,
             isSymbol: L,
             isArrayBuffer: q,
             isDataView: I,
-            isArray: F,
+            isArray: B,
             isFunction: D,
             isArguments: V,
             isFinite: function(e) {
                 return !L(e) && v(e) && !isNaN(parseFloat(e))
             },
             isNaN: H,
             isTypedArray: Z,
             isEmpty: function(e) {
                 if (null == e) return !0;
                 var t = J(e);
-                return "number" == typeof t && (F(e) || C(e) || V(e)) ? 0 === t : 0 === J(ee(e))
+                return "number" == typeof t && (B(e) || C(e) || V(e)) ? 0 === t : 0 === J(ee(e))
             },
             isMatch: te,
             isEqual: function(e, t) {
                 return ae(e, t)
             },
             isMap: me,
             isWeakMap: ve,
@@ -2974,24 +2974,24 @@
             assign: Se,
             defaults: Ce,
             create: function(e, t) {
                 var n = Me(e);
                 return t && Se(n, t), n
             },
             clone: function(e) {
-                return w(e) ? F(e) ? e.slice() : xe({}, e) : e
+                return w(e) ? B(e) ? e.slice() : xe({}, e) : e
             },
             tap: function(e, t) {
                 return t(e), e
             },
             get: Le,
             has: function(e, t) {
                 for (var n = (t = Ae(t)).length, i = 0; i < n; i++) {
                     var r = t[i];
-                    if (!$(e, r)) return !1;
+                    if (!F(e, r)) return !1;
                     e = e[r]
                 }
                 return !!n
             },
             mapObject: function(e, t, n) {
                 t = je(t, n);
                 for (var i = ee(e), r = i.length, a = {}, o = 0; o < r; o++) {
@@ -3015,15 +3015,15 @@
             times: function(e, t, n) {
                 var i = Array(Math.max(0, e));
                 t = De(t, n, 1);
                 for (var r = 0; r < e; r++) i[r] = t(r);
                 return i
             },
             random: Ie,
-            now: Fe,
+            now: Be,
             escape: Ve,
             unescape: He,
             templateSettings: Ue,
             template: function(e, t, n) {
                 !t && n && (t = n), t = Ce({}, t, ne.templateSettings);
                 var i = RegExp([(t.escape || We).source, (t.interpolate || We).source, (t.evaluate || We).source].join("|") + "|$", "g"),
                     r = 0,
@@ -3067,43 +3067,43 @@
             partial: Xe,
             bind: et,
             bindAll: it,
             memoize: function(e, t) {
                 var n = function(i) {
                     var r = n.cache,
                         a = "" + (t ? t.apply(this, arguments) : i);
-                    return $(r, a) || (r[a] = e.apply(this, arguments)), r[a]
+                    return F(r, a) || (r[a] = e.apply(this, arguments)), r[a]
                 };
                 return n.cache = {}, n
             },
             delay: rt,
             defer: at,
             throttle: function(e, t, n) {
                 var i, r, a, o, s = 0;
                 n || (n = {});
                 var l = function() {
-                        s = !1 === n.leading ? 0 : Fe(), i = null, o = e.apply(r, a), i || (r = a = null)
+                        s = !1 === n.leading ? 0 : Be(), i = null, o = e.apply(r, a), i || (r = a = null)
                     },
                     c = function() {
-                        var c = Fe();
+                        var c = Be();
                         s || !1 !== n.leading || (s = c);
                         var u = t - (c - s);
                         return r = this, a = arguments, u <= 0 || u > t ? (i && (clearTimeout(i), i = null), s = c, o = e.apply(r, a), i || (r = a = null)) : i || !1 === n.trailing || (i = setTimeout(l, u)), o
                     };
                 return c.cancel = function() {
                     clearTimeout(i), s = 0, i = r = a = null
                 }, c
             },
             debounce: function(e, t, n) {
                 var i, r, a, o, s, l = function() {
-                        var c = Fe() - r;
+                        var c = Be() - r;
                         t > c ? i = setTimeout(l, t - c) : (i = null, n || (o = e.apply(s, a)), i || (a = s = null))
                     },
                     c = y((function(c) {
-                        return s = this, a = c, r = Fe(), i || (i = setTimeout(l, t), n && (o = e.apply(s, a))), o
+                        return s = this, a = c, r = Be(), i || (i = setTimeout(l, t), n && (o = e.apply(s, a))), o
                     }));
                 return c.cancel = function() {
                     clearTimeout(i), i = a = s = null
                 }, c
             },
             wrap: function(e, t) {
                 return Xe(t, e)
@@ -3199,19 +3199,19 @@
             countBy: Nt,
             partition: jt,
             toArray: qt,
             size: function(e) {
                 return null == e ? 0 : tt(e) ? e.length : ee(e).length
             },
             pick: It,
-            omit: Ft,
-            first: Bt,
-            head: Bt,
-            take: Bt,
-            initial: $t,
+            omit: Bt,
+            first: $t,
+            head: $t,
+            take: $t,
+            initial: Ft,
             last: function(e, t, n) {
                 return null == e || e.length < 1 ? null == t || n ? void 0 : [] : null == t || n ? e[e.length - 1] : Vt(e, Math.max(0, e.length - t))
             },
             rest: Vt,
             tail: Vt,
             drop: Vt,
             compact: function(e) {
@@ -3416,15 +3416,15 @@
         j = "0123456789",
         R = {
             DIGIT: j,
             ALPHA: N,
             ALPHA_DIGIT: N + N.toUpperCase() + j
         };
     var I = d("AsyncFunction"),
-        F = {
+        B = {
             isArray: f,
             isArrayBuffer: m,
             isBuffer: function(e) {
                 return null !== e && !p(e) && null !== e.constructor && !p(e.constructor) && g(e.constructor.isBuffer) && e.constructor.isBuffer(e)
             },
             isFormData: function(e) {
                 var t;
@@ -3574,114 +3574,114 @@
             },
             isAsyncFn: I,
             isThenable: function(e) {
                 return e && (b(e) || g(e)) && g(e.then) && g(e.catch)
             }
         };
 
-    function $(e, t, n, i, r) {
+    function F(e, t, n, i, r) {
         Error.call(this), Error.captureStackTrace ? Error.captureStackTrace(this, this.constructor) : this.stack = (new Error).stack, this.message = e, this.name = "AxiosError", t && (this.code = t), n && (this.config = n), i && (this.request = i), r && (this.response = r)
     }
-    F.inherits($, Error, {
+    B.inherits(F, Error, {
         toJSON: function() {
             return {
                 message: this.message,
                 name: this.name,
                 description: this.description,
                 number: this.number,
                 fileName: this.fileName,
                 lineNumber: this.lineNumber,
                 columnNumber: this.columnNumber,
                 stack: this.stack,
-                config: F.toJSONObject(this.config),
+                config: B.toJSONObject(this.config),
                 code: this.code,
                 status: this.response && this.response.status ? this.response.status : null
             }
         }
     });
-    var B = $.prototype,
+    var $ = F.prototype,
         V = {};
     ["ERR_BAD_OPTION_VALUE", "ERR_BAD_OPTION", "ECONNABORTED", "ETIMEDOUT", "ERR_NETWORK", "ERR_FR_TOO_MANY_REDIRECTS", "ERR_DEPRECATED", "ERR_BAD_RESPONSE", "ERR_BAD_REQUEST", "ERR_CANCELED", "ERR_NOT_SUPPORT", "ERR_INVALID_URL"].forEach((function(e) {
         V[e] = {
             value: e
         }
-    })), Object.defineProperties($, V), Object.defineProperty(B, "isAxiosError", {
+    })), Object.defineProperties(F, V), Object.defineProperty($, "isAxiosError", {
         value: !0
-    }), $.from = function(e, t, n, i, r, a) {
-        var o = Object.create(B);
-        return F.toFlatObject(e, o, (function(e) {
+    }), F.from = function(e, t, n, i, r, a) {
+        var o = Object.create($);
+        return B.toFlatObject(e, o, (function(e) {
             return e !== Error.prototype
         }), (function(e) {
             return "isAxiosError" !== e
-        })), $.call(o, e.message, t, n, i, r), o.cause = e, o.name = e.name, a && Object.assign(o, a), o
+        })), F.call(o, e.message, t, n, i, r), o.cause = e, o.name = e.name, a && Object.assign(o, a), o
     };
 
     function H(e) {
-        return F.isPlainObject(e) || F.isArray(e)
+        return B.isPlainObject(e) || B.isArray(e)
     }
 
     function U(e) {
-        return F.endsWith(e, "[]") ? e.slice(0, -2) : e
+        return B.endsWith(e, "[]") ? e.slice(0, -2) : e
     }
 
     function W(e, t, n) {
         return e ? e.concat(t).map((function(e, t) {
             return e = U(e), !n && t ? "[" + e + "]" : e
         })).join(n ? "." : "") : t
     }
-    var Y = F.toFlatObject(F, {}, null, (function(e) {
+    var Y = B.toFlatObject(B, {}, null, (function(e) {
         return /^is[A-Z]/.test(e)
     }));
 
     function Q(t, n, i) {
-        if (!F.isObject(t)) throw new TypeError("target must be an object");
+        if (!B.isObject(t)) throw new TypeError("target must be an object");
         n = n || new FormData;
-        var r = (i = F.toFlatObject(i, {
+        var r = (i = B.toFlatObject(i, {
                 metaTokens: !0,
                 dots: !1,
                 indexes: !1
             }, !1, (function(e, t) {
-                return !F.isUndefined(t[e])
+                return !B.isUndefined(t[e])
             }))).metaTokens,
             a = i.visitor || u,
             o = i.dots,
             s = i.indexes,
-            l = (i.Blob || "undefined" != typeof Blob && Blob) && F.isSpecCompliantForm(n);
-        if (!F.isFunction(a)) throw new TypeError("visitor must be a function");
+            l = (i.Blob || "undefined" != typeof Blob && Blob) && B.isSpecCompliantForm(n);
+        if (!B.isFunction(a)) throw new TypeError("visitor must be a function");
 
         function c(e) {
             if (null === e) return "";
-            if (F.isDate(e)) return e.toISOString();
-            if (!l && F.isBlob(e)) throw new $("Blob is not supported. Use a Buffer instead.");
-            return F.isArrayBuffer(e) || F.isTypedArray(e) ? l && "function" == typeof Blob ? new Blob([e]) : Buffer.from(e) : e
+            if (B.isDate(e)) return e.toISOString();
+            if (!l && B.isBlob(e)) throw new F("Blob is not supported. Use a Buffer instead.");
+            return B.isArrayBuffer(e) || B.isTypedArray(e) ? l && "function" == typeof Blob ? new Blob([e]) : Buffer.from(e) : e
         }
 
         function u(t, i, a) {
             var l = t;
             if (t && !a && "object" === e(t))
-                if (F.endsWith(i, "{}")) i = r ? i : i.slice(0, -2), t = JSON.stringify(t);
-                else if (F.isArray(t) && function(e) {
-                    return F.isArray(e) && !e.some(H)
-                }(t) || (F.isFileList(t) || F.endsWith(i, "[]")) && (l = F.toArray(t))) return i = U(i), l.forEach((function(e, t) {
-                !F.isUndefined(e) && null !== e && n.append(!0 === s ? W([i], t, o) : null === s ? i : i + "[]", c(e))
+                if (B.endsWith(i, "{}")) i = r ? i : i.slice(0, -2), t = JSON.stringify(t);
+                else if (B.isArray(t) && function(e) {
+                    return B.isArray(e) && !e.some(H)
+                }(t) || (B.isFileList(t) || B.endsWith(i, "[]")) && (l = B.toArray(t))) return i = U(i), l.forEach((function(e, t) {
+                !B.isUndefined(e) && null !== e && n.append(!0 === s ? W([i], t, o) : null === s ? i : i + "[]", c(e))
             })), !1;
             return !!H(t) || (n.append(W(a, i, o), c(t)), !1)
         }
         var d = [],
             h = Object.assign(Y, {
                 defaultVisitor: u,
                 convertValue: c,
                 isVisitable: H
             });
-        if (!F.isObject(t)) throw new TypeError("data must be an object");
+        if (!B.isObject(t)) throw new TypeError("data must be an object");
         return function e(t, i) {
-            if (!F.isUndefined(t)) {
+            if (!B.isUndefined(t)) {
                 if (-1 !== d.indexOf(t)) throw Error("Circular reference detected in " + i.join("."));
-                d.push(t), F.forEach(t, (function(t, r) {
-                    !0 === (!(F.isUndefined(t) || null === t) && a.call(n, t, F.isString(r) ? r.trim() : r, i, h)) && e(t, i ? i.concat(r) : [r])
+                d.push(t), B.forEach(t, (function(t, r) {
+                    !0 === (!(B.isUndefined(t) || null === t) && a.call(n, t, B.isString(r) ? r.trim() : r, i, h)) && e(t, i ? i.concat(r) : [r])
                 })), d.pop()
             }
         }(t), n
     }
 
     function G(e) {
         var t = {
@@ -3707,15 +3707,15 @@
         return encodeURIComponent(e).replace(/%3A/gi, ":").replace(/%24/g, "$").replace(/%2C/gi, ",").replace(/%20/g, "+").replace(/%5B/gi, "[").replace(/%5D/gi, "]")
     }
 
     function X(e, t, n) {
         if (!t) return e;
         var i, r = n && n.encode || J,
             a = n && n.serialize;
-        if (i = a ? a(t, n) : F.isURLSearchParams(t) ? t.toString() : new K(t, n).toString(r)) {
+        if (i = a ? a(t, n) : B.isURLSearchParams(t) ? t.toString() : new K(t, n).toString(r)) {
             var o = e.indexOf("#"); - 1 !== o && (e = e.slice(0, o)), e += (-1 === e.indexOf("?") ? "?" : "&") + i
         }
         return e
     }
     Z.append = function(e, t) {
         this._pairs.push([e, t])
     }, Z.toString = function(e) {
@@ -3749,15 +3749,15 @@
                 key: "clear",
                 value: function() {
                     this.handlers && (this.handlers = [])
                 }
             }, {
                 key: "forEach",
                 value: function(e) {
-                    F.forEach(this.handlers, (function(t) {
+                    B.forEach(this.handlers, (function(t) {
                         null !== t && e(t)
                     }))
                 }
             }]), e
         }(),
         ne = {
             silentJSONParsing: !0,
@@ -3777,80 +3777,80 @@
         };
 
     function re(e) {
         function t(e, n, i, r) {
             var a = e[r++],
                 o = Number.isFinite(+a),
                 s = r >= e.length;
-            return a = !a && F.isArray(i) ? i.length : a, s ? (F.hasOwnProp(i, a) ? i[a] = [i[a], n] : i[a] = n, !o) : (i[a] && F.isObject(i[a]) || (i[a] = []), t(e, n, i[a], r) && F.isArray(i[a]) && (i[a] = function(e) {
+            return a = !a && B.isArray(i) ? i.length : a, s ? (B.hasOwnProp(i, a) ? i[a] = [i[a], n] : i[a] = n, !o) : (i[a] && B.isObject(i[a]) || (i[a] = []), t(e, n, i[a], r) && B.isArray(i[a]) && (i[a] = function(e) {
                 var t, n, i = {},
                     r = Object.keys(e),
                     a = r.length;
                 for (t = 0; t < a; t++) i[n = r[t]] = e[n];
                 return i
             }(i[a])), !o)
         }
-        if (F.isFormData(e) && F.isFunction(e.entries)) {
+        if (B.isFormData(e) && B.isFunction(e.entries)) {
             var n = {};
-            return F.forEachEntry(e, (function(e, i) {
+            return B.forEachEntry(e, (function(e, i) {
                 t(function(e) {
-                    return F.matchAll(/\w+|\[(\w*)]/g, e).map((function(e) {
+                    return B.matchAll(/\w+|\[(\w*)]/g, e).map((function(e) {
                         return "[]" === e[0] ? "" : e[1] || e[0]
                     }))
                 }(e), i, n, 0)
             })), n
         }
         return null
     }
     var ae = {
         transitional: ne,
         adapter: ["xhr", "http"],
         transformRequest: [function(e, t) {
             var n, i = t.getContentType() || "",
                 r = i.indexOf("application/json") > -1,
-                a = F.isObject(e);
-            if (a && F.isHTMLForm(e) && (e = new FormData(e)), F.isFormData(e)) return r && r ? JSON.stringify(re(e)) : e;
-            if (F.isArrayBuffer(e) || F.isBuffer(e) || F.isStream(e) || F.isFile(e) || F.isBlob(e)) return e;
-            if (F.isArrayBufferView(e)) return e.buffer;
-            if (F.isURLSearchParams(e)) return t.setContentType("application/x-www-form-urlencoded;charset=utf-8", !1), e.toString();
+                a = B.isObject(e);
+            if (a && B.isHTMLForm(e) && (e = new FormData(e)), B.isFormData(e)) return r && r ? JSON.stringify(re(e)) : e;
+            if (B.isArrayBuffer(e) || B.isBuffer(e) || B.isStream(e) || B.isFile(e) || B.isBlob(e)) return e;
+            if (B.isArrayBufferView(e)) return e.buffer;
+            if (B.isURLSearchParams(e)) return t.setContentType("application/x-www-form-urlencoded;charset=utf-8", !1), e.toString();
             if (a) {
                 if (i.indexOf("application/x-www-form-urlencoded") > -1) return function(e, t) {
                     return Q(e, new ie.classes.URLSearchParams, Object.assign({
                         visitor: function(e, t, n, i) {
-                            return ie.isNode && F.isBuffer(e) ? (this.append(t, e.toString("base64")), !1) : i.defaultVisitor.apply(this, arguments)
+                            return ie.isNode && B.isBuffer(e) ? (this.append(t, e.toString("base64")), !1) : i.defaultVisitor.apply(this, arguments)
                         }
                     }, t))
                 }(e, this.formSerializer).toString();
-                if ((n = F.isFileList(e)) || i.indexOf("multipart/form-data") > -1) {
+                if ((n = B.isFileList(e)) || i.indexOf("multipart/form-data") > -1) {
                     var o = this.env && this.env.FormData;
                     return Q(n ? {
                         "files[]": e
                     } : e, o && new o, this.formSerializer)
                 }
             }
             return a || r ? (t.setContentType("application/json", !1), function(e, t, n) {
-                if (F.isString(e)) try {
-                    return (t || JSON.parse)(e), F.trim(e)
+                if (B.isString(e)) try {
+                    return (t || JSON.parse)(e), B.trim(e)
                 } catch (e) {
                     if ("SyntaxError" !== e.name) throw e
                 }
                 return (n || JSON.stringify)(e)
             }(e)) : e
         }],
         transformResponse: [function(e) {
             var t = this.transitional || ae.transitional,
                 n = t && t.forcedJSONParsing,
                 i = "json" === this.responseType;
-            if (e && F.isString(e) && (n && !this.responseType || i)) {
+            if (e && B.isString(e) && (n && !this.responseType || i)) {
                 var r = !(t && t.silentJSONParsing) && i;
                 try {
                     return JSON.parse(e)
                 } catch (e) {
                     if (r) {
-                        if ("SyntaxError" === e.name) throw $.from(e, $.ERR_BAD_RESPONSE, this, null, this.response);
+                        if ("SyntaxError" === e.name) throw F.from(e, F.ERR_BAD_RESPONSE, this, null, this.response);
                         throw e
                     }
                 }
             }
             return e
         }],
         timeout: 0,
@@ -3868,96 +3868,96 @@
         headers: {
             common: {
                 Accept: "application/json, text/plain, */*",
                 "Content-Type": void 0
             }
         }
     };
-    F.forEach(["delete", "get", "head", "post", "put", "patch"], (function(e) {
+    B.forEach(["delete", "get", "head", "post", "put", "patch"], (function(e) {
         ae.headers[e] = {}
     }));
     var oe = ae,
-        se = F.toObjectSet(["age", "authorization", "content-length", "content-type", "etag", "expires", "from", "host", "if-modified-since", "if-unmodified-since", "last-modified", "location", "max-forwards", "proxy-authorization", "referer", "retry-after", "user-agent"]),
+        se = B.toObjectSet(["age", "authorization", "content-length", "content-type", "etag", "expires", "from", "host", "if-modified-since", "if-unmodified-since", "last-modified", "location", "max-forwards", "proxy-authorization", "referer", "retry-after", "user-agent"]),
         le = Symbol("internals");
 
     function ce(e) {
         return e && String(e).trim().toLowerCase()
     }
 
     function ue(e) {
-        return !1 === e || null == e ? e : F.isArray(e) ? e.map(ue) : String(e)
+        return !1 === e || null == e ? e : B.isArray(e) ? e.map(ue) : String(e)
     }
 
     function de(e, t, n, i, r) {
-        return F.isFunction(i) ? i.call(this, t, n) : (r && (t = n), F.isString(t) ? F.isString(i) ? -1 !== t.indexOf(i) : F.isRegExp(i) ? i.test(t) : void 0 : void 0)
+        return B.isFunction(i) ? i.call(this, t, n) : (r && (t = n), B.isString(t) ? B.isString(i) ? -1 !== t.indexOf(i) : B.isRegExp(i) ? i.test(t) : void 0 : void 0)
     }
     var he = function(e, n) {
         function a(e) {
             t(this, a), e && this.set(e)
         }
         return i(a, [{
             key: "set",
             value: function(e, t, n) {
                 var i = this;
 
                 function r(e, t, n) {
                     var r = ce(t);
                     if (!r) throw new Error("header name must be a non-empty string");
-                    var a = F.findKey(i, r);
+                    var a = B.findKey(i, r);
                     (!a || void 0 === i[a] || !0 === n || void 0 === n && !1 !== i[a]) && (i[a || t] = ue(e))
                 }
                 var a, o, s, l, c, u = function(e, t) {
-                    return F.forEach(e, (function(e, n) {
+                    return B.forEach(e, (function(e, n) {
                         return r(e, n, t)
                     }))
                 };
-                return F.isPlainObject(e) || e instanceof this.constructor ? u(e, t) : F.isString(e) && (e = e.trim()) && !/^[-_a-zA-Z0-9^`|~,!#$%&'*+.]+$/.test(e.trim()) ? u((c = {}, (a = e) && a.split("\n").forEach((function(e) {
+                return B.isPlainObject(e) || e instanceof this.constructor ? u(e, t) : B.isString(e) && (e = e.trim()) && !/^[-_a-zA-Z0-9^`|~,!#$%&'*+.]+$/.test(e.trim()) ? u((c = {}, (a = e) && a.split("\n").forEach((function(e) {
                     l = e.indexOf(":"), o = e.substring(0, l).trim().toLowerCase(), s = e.substring(l + 1).trim(), !o || c[o] && se[o] || ("set-cookie" === o ? c[o] ? c[o].push(s) : c[o] = [s] : c[o] = c[o] ? c[o] + ", " + s : s)
                 })), c), t) : null != e && r(t, e, n), this
             }
         }, {
             key: "get",
             value: function(e, t) {
                 if (e = ce(e)) {
-                    var n = F.findKey(this, e);
+                    var n = B.findKey(this, e);
                     if (n) {
                         var i = this[n];
                         if (!t) return i;
                         if (!0 === t) return function(e) {
                             for (var t, n = Object.create(null), i = /([^\s,;=]+)\s*(?:=\s*([^,;]+))?/g; t = i.exec(e);) n[t[1]] = t[2];
                             return n
                         }(i);
-                        if (F.isFunction(t)) return t.call(this, i, n);
-                        if (F.isRegExp(t)) return t.exec(i);
+                        if (B.isFunction(t)) return t.call(this, i, n);
+                        if (B.isRegExp(t)) return t.exec(i);
                         throw new TypeError("parser must be boolean|regexp|function")
                     }
                 }
             }
         }, {
             key: "has",
             value: function(e, t) {
                 if (e = ce(e)) {
-                    var n = F.findKey(this, e);
+                    var n = B.findKey(this, e);
                     return !(!n || void 0 === this[n] || t && !de(0, this[n], n, t))
                 }
                 return !1
             }
         }, {
             key: "delete",
             value: function(e, t) {
                 var n = this,
                     i = !1;
 
                 function r(e) {
                     if (e = ce(e)) {
-                        var r = F.findKey(n, e);
+                        var r = B.findKey(n, e);
                         !r || t && !de(0, n[r], r, t) || (delete n[r], i = !0)
                     }
                 }
-                return F.isArray(e) ? e.forEach(r) : r(e), i
+                return B.isArray(e) ? e.forEach(r) : r(e), i
             }
         }, {
             key: "clear",
             value: function(e) {
                 for (var t = Object.keys(this), n = t.length, i = !1; n--;) {
                     var r = t[n];
                     e && !de(0, this[r], r, e, !0) || (delete this[r], i = !0)
@@ -3965,16 +3965,16 @@
                 return i
             }
         }, {
             key: "normalize",
             value: function(e) {
                 var t = this,
                     n = {};
-                return F.forEach(this, (function(i, r) {
-                    var a = F.findKey(n, r);
+                return B.forEach(this, (function(i, r) {
+                    var a = B.findKey(n, r);
                     if (a) return t[a] = ue(i), void delete t[r];
                     var o = e ? function(e) {
                         return e.trim().toLowerCase().replace(/([a-z\d])(\w*)/g, (function(e, t, n) {
                             return t.toUpperCase() + n
                         }))
                     }(r) : String(r).trim();
                     o !== r && delete t[r], t[o] = ue(i), n[o] = !0
@@ -3986,16 +3986,16 @@
                 for (var e, t = arguments.length, n = new Array(t), i = 0; i < t; i++) n[i] = arguments[i];
                 return (e = this.constructor).concat.apply(e, [this].concat(n))
             }
         }, {
             key: "toJSON",
             value: function(e) {
                 var t = Object.create(null);
-                return F.forEach(this, (function(n, i) {
-                    null != n && !1 !== n && (t[i] = e && F.isArray(n) ? n.join(", ") : n)
+                return B.forEach(this, (function(n, i) {
+                    null != n && !1 !== n && (t[i] = e && B.isArray(n) ? n.join(", ") : n)
                 })), t
             }
         }, {
             key: Symbol.iterator,
             value: function() {
                 return Object.entries(this.toJSON())[Symbol.iterator]()
             }
@@ -4032,67 +4032,67 @@
                         accessors: {}
                     }).accessors,
                     n = this.prototype;
 
                 function i(e) {
                     var i = ce(e);
                     t[i] || (! function(e, t) {
-                        var n = F.toCamelCase(" " + t);
+                        var n = B.toCamelCase(" " + t);
                         ["get", "set", "has"].forEach((function(i) {
                             Object.defineProperty(e, i + n, {
                                 value: function(e, n, r) {
                                     return this[i].call(this, t, e, n, r)
                                 },
                                 configurable: !0
                             })
                         }))
                     }(n, e), t[i] = !0)
                 }
-                return F.isArray(e) ? e.forEach(i) : i(e), this
+                return B.isArray(e) ? e.forEach(i) : i(e), this
             }
         }]), a
     }();
-    he.accessor(["Content-Type", "Content-Length", "Accept", "Accept-Encoding", "User-Agent", "Authorization"]), F.reduceDescriptors(he.prototype, (function(e, t) {
+    he.accessor(["Content-Type", "Content-Length", "Accept", "Accept-Encoding", "User-Agent", "Authorization"]), B.reduceDescriptors(he.prototype, (function(e, t) {
         var n = e.value,
             i = t[0].toUpperCase() + t.slice(1);
         return {
             get: function() {
                 return n
             },
             set: function(e) {
                 this[i] = e
             }
         }
-    })), F.freezeMethods(he);
+    })), B.freezeMethods(he);
     var fe = he;
 
     function pe(e, t) {
         var n = this || oe,
             i = t || n,
             r = fe.from(i.headers),
             a = i.data;
-        return F.forEach(e, (function(e) {
+        return B.forEach(e, (function(e) {
             a = e.call(n, a, r.normalize(), t ? t.status : void 0)
         })), r.normalize(), a
     }
 
     function me(e) {
         return !(!e || !e.__CANCEL__)
     }
 
     function ve(e, t, n) {
-        $.call(this, null == e ? "canceled" : e, $.ERR_CANCELED, t, n), this.name = "CanceledError"
+        F.call(this, null == e ? "canceled" : e, F.ERR_CANCELED, t, n), this.name = "CanceledError"
     }
-    F.inherits(ve, $, {
+    B.inherits(ve, F, {
         __CANCEL__: !0
     });
     var ge = ie.isStandardBrowserEnv ? {
         write: function(e, t, n, i, r, a) {
             var o = [];
-            o.push(e + "=" + encodeURIComponent(t)), F.isNumber(n) && o.push("expires=" + new Date(n).toGMTString()), F.isString(i) && o.push("path=" + i), F.isString(r) && o.push("domain=" + r), !0 === a && o.push("secure"), document.cookie = o.join("; ")
+            o.push(e + "=" + encodeURIComponent(t)), B.isNumber(n) && o.push("expires=" + new Date(n).toGMTString()), B.isString(i) && o.push("path=" + i), B.isString(r) && o.push("domain=" + r), !0 === a && o.push("secure"), document.cookie = o.join("; ")
         },
         read: function(e) {
             var t = document.cookie.match(new RegExp("(^|;\\s*)(" + e + ")=([^;]*)"));
             return t ? decodeURIComponent(t[3]) : null
         },
         remove: function(e) {
             this.write(e, "", Date.now() - 864e5)
@@ -4125,15 +4125,15 @@
                 hostname: n.hostname,
                 port: n.port,
                 pathname: "/" === n.pathname.charAt(0) ? n.pathname : "/" + n.pathname
             }
         }
         return e = i(window.location.href),
             function(t) {
-                var n = F.isString(t) ? i(t) : t;
+                var n = B.isString(t) ? i(t) : t;
                 return n.protocol === e.protocol && n.host === e.host
             }
     }() : function() {
         return !0
     };
 
     function ye(e, t) {
@@ -4181,29 +4181,29 @@
                 var i, r, a = e.data,
                     o = fe.from(e.headers).normalize(),
                     s = e.responseType;
 
                 function l() {
                     e.cancelToken && e.cancelToken.unsubscribe(i), e.signal && e.signal.removeEventListener("abort", i)
                 }
-                F.isFormData(a) && (ie.isStandardBrowserEnv || ie.isStandardBrowserWebWorkerEnv ? o.setContentType(!1) : o.getContentType(/^\s*multipart\/form-data/) ? F.isString(r = o.getContentType()) && o.setContentType(r.replace(/^\s*(multipart\/form-data);+/, "$1")) : o.setContentType("multipart/form-data"));
+                B.isFormData(a) && (ie.isStandardBrowserEnv || ie.isStandardBrowserWebWorkerEnv ? o.setContentType(!1) : o.getContentType(/^\s*multipart\/form-data/) ? B.isString(r = o.getContentType()) && o.setContentType(r.replace(/^\s*(multipart\/form-data);+/, "$1")) : o.setContentType("multipart/form-data"));
                 var c = new XMLHttpRequest;
                 if (e.auth) {
                     var u = e.auth.username || "",
                         d = e.auth.password ? unescape(encodeURIComponent(e.auth.password)) : "";
                     o.set("Authorization", "Basic " + btoa(u + ":" + d))
                 }
                 var h = _e(e.baseURL, e.url);
 
                 function f() {
                     if (c) {
                         var i = fe.from("getAllResponseHeaders" in c && c.getAllResponseHeaders());
                         ! function(e, t, n) {
                             var i = n.config.validateStatus;
-                            n.status && i && !i(n.status) ? t(new $("Request failed with status code " + n.status, [$.ERR_BAD_REQUEST, $.ERR_BAD_RESPONSE][Math.floor(n.status / 100) - 4], n.config, n.request, n)) : e(n)
+                            n.status && i && !i(n.status) ? t(new F("Request failed with status code " + n.status, [F.ERR_BAD_REQUEST, F.ERR_BAD_RESPONSE][Math.floor(n.status / 100) - 4], n.config, n.request, n)) : e(n)
                         }((function(e) {
                             t(e), l()
                         }), (function(e) {
                             n(e), l()
                         }), {
                             data: s && "text" !== s && "json" !== s ? c.response : c.responseText,
                             status: c.status,
@@ -4213,36 +4213,36 @@
                             request: c
                         }), c = null
                     }
                 }
                 if (c.open(e.method.toUpperCase(), X(h, e.params, e.paramsSerializer), !0), c.timeout = e.timeout, "onloadend" in c ? c.onloadend = f : c.onreadystatechange = function() {
                         c && 4 === c.readyState && (0 !== c.status || c.responseURL && 0 === c.responseURL.indexOf("file:")) && setTimeout(f)
                     }, c.onabort = function() {
-                        c && (n(new $("Request aborted", $.ECONNABORTED, e, c)), c = null)
+                        c && (n(new F("Request aborted", F.ECONNABORTED, e, c)), c = null)
                     }, c.onerror = function() {
-                        n(new $("Network Error", $.ERR_NETWORK, e, c)), c = null
+                        n(new F("Network Error", F.ERR_NETWORK, e, c)), c = null
                     }, c.ontimeout = function() {
                         var t = e.timeout ? "timeout of " + e.timeout + "ms exceeded" : "timeout exceeded",
                             i = e.transitional || ne;
-                        e.timeoutErrorMessage && (t = e.timeoutErrorMessage), n(new $(t, i.clarifyTimeoutError ? $.ETIMEDOUT : $.ECONNABORTED, e, c)), c = null
+                        e.timeoutErrorMessage && (t = e.timeoutErrorMessage), n(new F(t, i.clarifyTimeoutError ? F.ETIMEDOUT : F.ECONNABORTED, e, c)), c = null
                     }, ie.isStandardBrowserEnv) {
                     var p = be(h) && e.xsrfCookieName && ge.read(e.xsrfCookieName);
                     p && o.set(e.xsrfHeaderName, p)
                 }
-                void 0 === a && o.setContentType(null), "setRequestHeader" in c && F.forEach(o.toJSON(), (function(e, t) {
+                void 0 === a && o.setContentType(null), "setRequestHeader" in c && B.forEach(o.toJSON(), (function(e, t) {
                     c.setRequestHeader(t, e)
-                })), F.isUndefined(e.withCredentials) || (c.withCredentials = !!e.withCredentials), s && "json" !== s && (c.responseType = e.responseType), "function" == typeof e.onDownloadProgress && c.addEventListener("progress", ye(e.onDownloadProgress, !0)), "function" == typeof e.onUploadProgress && c.upload && c.upload.addEventListener("progress", ye(e.onUploadProgress)), (e.cancelToken || e.signal) && (i = function(t) {
+                })), B.isUndefined(e.withCredentials) || (c.withCredentials = !!e.withCredentials), s && "json" !== s && (c.responseType = e.responseType), "function" == typeof e.onDownloadProgress && c.addEventListener("progress", ye(e.onDownloadProgress, !0)), "function" == typeof e.onUploadProgress && c.upload && c.upload.addEventListener("progress", ye(e.onUploadProgress)), (e.cancelToken || e.signal) && (i = function(t) {
                     c && (n(!t || t.type ? new ve(null, e, c) : t), c.abort(), c = null)
                 }, e.cancelToken && e.cancelToken.subscribe(i), e.signal && (e.signal.aborted ? i() : e.signal.addEventListener("abort", i)));
                 var m, v = (m = /^([-+\w]{1,25})(:?\/\/|:)/.exec(h)) && m[1] || "";
-                v && -1 === ie.protocols.indexOf(v) ? n(new $("Unsupported protocol " + v + ":", $.ERR_BAD_REQUEST, e)) : c.send(a || null)
+                v && -1 === ie.protocols.indexOf(v) ? n(new F("Unsupported protocol " + v + ":", F.ERR_BAD_REQUEST, e)) : c.send(a || null)
             }))
         }
     };
-    F.forEach(we, (function(e, t) {
+    B.forEach(we, (function(e, t) {
         if (e) {
             try {
                 Object.defineProperty(e, "name", {
                     value: t
                 })
             } catch (e) {}
             Object.defineProperty(e, "adapterName", {
@@ -4250,31 +4250,31 @@
             })
         }
     }));
     var ke = function(e) {
             return "- ".concat(e)
         },
         xe = function(e) {
-            return F.isFunction(e) || null === e || !1 === e
+            return B.isFunction(e) || null === e || !1 === e
         },
         Se = function(e) {
-            for (var t, n, i = (e = F.isArray(e) ? e : [e]).length, a = {}, o = 0; o < i; o++) {
+            for (var t, n, i = (e = B.isArray(e) ? e : [e]).length, a = {}, o = 0; o < i; o++) {
                 var s = void 0;
-                if (n = t = e[o], !xe(t) && void 0 === (n = we[(s = String(t)).toLowerCase()])) throw new $("Unknown adapter '".concat(s, "'"));
+                if (n = t = e[o], !xe(t) && void 0 === (n = we[(s = String(t)).toLowerCase()])) throw new F("Unknown adapter '".concat(s, "'"));
                 if (n) break;
                 a[s || "#" + o] = n
             }
             if (!n) {
                 var l = Object.entries(a).map((function(e) {
                     var t = r(e, 2),
                         n = t[0],
                         i = t[1];
                     return "adapter ".concat(n, " ") + (!1 === i ? "is not supported by the environment" : "is not available in the build")
                 }));
-                throw new $("There is no suitable adapter to dispatch the request " + (i ? l.length > 1 ? "since :\n" + l.map(ke).join("\n") : " " + ke(l[0]) : "as no adapter specified"), "ERR_NOT_SUPPORT")
+                throw new F("There is no suitable adapter to dispatch the request " + (i ? l.length > 1 ? "since :\n" + l.map(ke).join("\n") : " " + ke(l[0]) : "as no adapter specified"), "ERR_NOT_SUPPORT")
             }
             return n
         };
 
     function Ce(e) {
         if (e.cancelToken && e.cancelToken.throwIfRequested(), e.signal && e.signal.aborted) throw new ve(null, e)
     }
@@ -4291,29 +4291,29 @@
     };
 
     function Ae(e, t) {
         t = t || {};
         var n = {};
 
         function i(e, t, n) {
-            return F.isPlainObject(e) && F.isPlainObject(t) ? F.merge.call({
+            return B.isPlainObject(e) && B.isPlainObject(t) ? B.merge.call({
                 caseless: n
-            }, e, t) : F.isPlainObject(t) ? F.merge({}, t) : F.isArray(t) ? t.slice() : t
+            }, e, t) : B.isPlainObject(t) ? B.merge({}, t) : B.isArray(t) ? t.slice() : t
         }
 
         function r(e, t, n) {
-            return F.isUndefined(t) ? F.isUndefined(e) ? void 0 : i(void 0, e, n) : i(e, t, n)
+            return B.isUndefined(t) ? B.isUndefined(e) ? void 0 : i(void 0, e, n) : i(e, t, n)
         }
 
         function a(e, t) {
-            if (!F.isUndefined(t)) return i(void 0, t)
+            if (!B.isUndefined(t)) return i(void 0, t)
         }
 
         function o(e, t) {
-            return F.isUndefined(t) ? F.isUndefined(e) ? void 0 : i(void 0, e) : i(void 0, t)
+            return B.isUndefined(t) ? B.isUndefined(e) ? void 0 : i(void 0, e) : i(void 0, t)
         }
 
         function s(n, r, a) {
             return a in t ? i(n, r) : a in e ? i(void 0, n) : void 0
         }
         var l = {
             url: a,
@@ -4343,18 +4343,18 @@
             socketPath: o,
             responseEncoding: o,
             validateStatus: s,
             headers: function(e, t) {
                 return r(Te(e), Te(t), !0)
             }
         };
-        return F.forEach(Object.keys(Object.assign({}, e, t)), (function(i) {
+        return B.forEach(Object.keys(Object.assign({}, e, t)), (function(i) {
             var a = l[i] || r,
                 o = a(e[i], t[i], i);
-            F.isUndefined(o) && a !== s || (n[i] = o)
+            B.isUndefined(o) && a !== s || (n[i] = o)
         })), n
     }
     var Pe = "1.6.0",
         Le = {};
     ["object", "boolean", "number", "function", "string", "symbol"].forEach((function(t, n) {
         Le[t] = function(i) {
             return e(i) === t || "a" + (n < 1 ? "n " : " ") + t
@@ -4362,29 +4362,29 @@
     }));
     var qe = {};
     Le.transitional = function(e, t, n) {
         function i(e, t) {
             return "[Axios v1.6.0] Transitional option '" + e + "'" + t + (n ? ". " + n : "")
         }
         return function(n, r, a) {
-            if (!1 === e) throw new $(i(r, " has been removed" + (t ? " in " + t : "")), $.ERR_DEPRECATED);
+            if (!1 === e) throw new F(i(r, " has been removed" + (t ? " in " + t : "")), F.ERR_DEPRECATED);
             return t && !qe[r] && (qe[r] = !0, console.warn(i(r, " has been deprecated since v" + t + " and will be removed in the near future"))), !e || e(n, r, a)
         }
     };
     var Oe = {
             assertOptions: function(t, n, i) {
-                if ("object" !== e(t)) throw new $("options must be an object", $.ERR_BAD_OPTION_VALUE);
+                if ("object" !== e(t)) throw new F("options must be an object", F.ERR_BAD_OPTION_VALUE);
                 for (var r = Object.keys(t), a = r.length; a-- > 0;) {
                     var o = r[a],
                         s = n[o];
                     if (s) {
                         var l = t[o],
                             c = void 0 === l || s(l, o, t);
-                        if (!0 !== c) throw new $("option " + o + " must be " + c, $.ERR_BAD_OPTION_VALUE)
-                    } else if (!0 !== i) throw new $("Unknown option " + o, $.ERR_BAD_OPTION)
+                        if (!0 !== c) throw new F("option " + o + " must be " + c, F.ERR_BAD_OPTION_VALUE)
+                    } else if (!0 !== i) throw new F("Unknown option " + o, F.ERR_BAD_OPTION)
                 }
             },
             validators: Le
         },
         Ee = Oe.validators,
         De = function() {
             function e(n) {
@@ -4401,22 +4401,22 @@
                         i = n.transitional,
                         r = n.paramsSerializer,
                         a = n.headers;
                     void 0 !== i && Oe.assertOptions(i, {
                         silentJSONParsing: Ee.transitional(Ee.boolean),
                         forcedJSONParsing: Ee.transitional(Ee.boolean),
                         clarifyTimeoutError: Ee.transitional(Ee.boolean)
-                    }, !1), null != r && (F.isFunction(r) ? t.paramsSerializer = {
+                    }, !1), null != r && (B.isFunction(r) ? t.paramsSerializer = {
                         serialize: r
                     } : Oe.assertOptions(r, {
                         encode: Ee.function,
                         serialize: Ee.function
                     }, !0)), t.method = (t.method || this.defaults.method || "get").toLowerCase();
-                    var o = a && F.merge(a.common, a[t.method]);
-                    a && F.forEach(["delete", "get", "head", "post", "put", "patch", "common"], (function(e) {
+                    var o = a && B.merge(a.common, a[t.method]);
+                    a && B.forEach(["delete", "get", "head", "post", "put", "patch", "common"], (function(e) {
                         delete a[e]
                     })), t.headers = fe.concat(o, a);
                     var s = [],
                         l = !0;
                     this.interceptors.request.forEach((function(e) {
                         "function" == typeof e.runWhen && !1 === e.runWhen(t) || (l = l && e.synchronous, s.unshift(e.fulfilled, e.rejected))
                     }));
@@ -4453,23 +4453,23 @@
             }, {
                 key: "getUri",
                 value: function(e) {
                     return X(_e((e = Ae(this.defaults, e)).baseURL, e.url), e.params, e.paramsSerializer)
                 }
             }]), e
         }();
-    F.forEach(["delete", "get", "head", "options"], (function(e) {
+    B.forEach(["delete", "get", "head", "options"], (function(e) {
         De.prototype[e] = function(t, n) {
             return this.request(Ae(n || {}, {
                 method: e,
                 url: t,
                 data: (n || {}).data
             }))
         }
-    })), F.forEach(["post", "put", "patch"], (function(e) {
+    })), B.forEach(["post", "put", "patch"], (function(e) {
         function t(t) {
             return function(n, i, r) {
                 return this.request(Ae(r || {}, {
                     method: e,
                     headers: t ? {
                         "Content-Type": "multipart/form-data"
                     } : {},
@@ -4606,32 +4606,32 @@
             i = t[1];
         je[i] = n
     }));
     var Re = je;
     var Ie = function e(t) {
         var n = new ze(t),
             i = o(ze.prototype.request, n);
-        return F.extend(i, ze.prototype, n, {
+        return B.extend(i, ze.prototype, n, {
             allOwnKeys: !0
-        }), F.extend(i, n, null, {
+        }), B.extend(i, n, null, {
             allOwnKeys: !0
         }), i.create = function(n) {
             return e(Ae(t, n))
         }, i
     }(oe);
-    return Ie.Axios = ze, Ie.CanceledError = ve, Ie.CancelToken = Ne, Ie.isCancel = me, Ie.VERSION = Pe, Ie.toFormData = Q, Ie.AxiosError = $, Ie.Cancel = Ie.CanceledError, Ie.all = function(e) {
+    return Ie.Axios = ze, Ie.CanceledError = ve, Ie.CancelToken = Ne, Ie.isCancel = me, Ie.VERSION = Pe, Ie.toFormData = Q, Ie.AxiosError = F, Ie.Cancel = Ie.CanceledError, Ie.all = function(e) {
         return Promise.all(e)
     }, Ie.spread = function(e) {
         return function(t) {
             return e.apply(null, t)
         }
     }, Ie.isAxiosError = function(e) {
-        return F.isObject(e) && !0 === e.isAxiosError
+        return B.isObject(e) && !0 === e.isAxiosError
     }, Ie.mergeConfig = Ae, Ie.AxiosHeaders = fe, Ie.formToJSON = function(e) {
-        return re(F.isHTMLForm(e) ? new FormData(e) : e)
+        return re(B.isHTMLForm(e) ? new FormData(e) : e)
     }, Ie.getAdapter = Se, Ie.HttpStatusCode = Re, Ie.default = Ie, Ie
 })),
 /*!
  * Vue.js v2.6.12
  * (c) 2014-2020 Evan You
  * Released under the MIT License.
  */
@@ -4821,30 +4821,30 @@
             isUnknownElement: q,
             getTagNamespace: L,
             parsePlatformTagName: O,
             mustUseProp: q,
             async: !0,
             _lifecycleHooks: R
         },
-        F = /a-zA-Z\u00B7\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u037D\u037F-\u1FFF\u200C-\u200D\u203F-\u2040\u2070-\u218F\u2C00-\u2FEF\u3001-\uD7FF\uF900-\uFDCF\uFDF0-\uFFFD/;
+        B = /a-zA-Z\u00B7\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u037D\u037F-\u1FFF\u200C-\u200D\u203F-\u2040\u2070-\u218F\u2C00-\u2FEF\u3001-\uD7FF\uF900-\uFDCF\uFDF0-\uFFFD/;
 
-    function $(e) {
+    function F(e) {
         var t = (e + "").charCodeAt(0);
         return 36 === t || 95 === t
     }
 
-    function B(e, t, n, i) {
+    function $(e, t, n, i) {
         Object.defineProperty(e, t, {
             value: n,
             enumerable: !!i,
             writable: !0,
             configurable: !0
         })
     }
-    var V = new RegExp("[^" + F.source + ".$_\\d]");
+    var V = new RegExp("[^" + B.source + ".$_\\d]");
     var H, U = "__proto__" in {},
         W = "undefined" != typeof window,
         Y = "undefined" != typeof WXEnvironment && !!WXEnvironment.platform,
         Q = Y && WXEnvironment.platform.toLowerCase(),
         G = W && window.navigator.userAgent.toLowerCase(),
         K = G && /msie|trident/.test(G),
         Z = G && G.indexOf("msie 9.0") > 0,
@@ -4981,15 +4981,15 @@
         var t = new ye(e.tag, e.data, e.children && e.children.slice(), e.text, e.elm, e.context, e.componentOptions, e.asyncFactory);
         return t.ns = e.ns, t.isStatic = e.isStatic, t.key = e.key, t.isComment = e.isComment, t.fnContext = e.fnContext, t.fnOptions = e.fnOptions, t.fnScopeId = e.fnScopeId, t.asyncMeta = e.asyncMeta, t.isCloned = !0, t
     }
     var Ce = Array.prototype,
         Me = Object.create(Ce);
     ["push", "pop", "shift", "unshift", "splice", "sort", "reverse"].forEach((function(e) {
         var t = Ce[e];
-        B(Me, e, (function() {
+        $(Me, e, (function() {
             for (var n = [], i = arguments.length; i--;) n[i] = arguments[i];
             var r, a = t.apply(this, n),
                 o = this.__ob__;
             switch (e) {
                 case "push":
                 case "unshift":
                     r = n;
@@ -5003,20 +5003,20 @@
     var Te = Object.getOwnPropertyNames(Me),
         Ae = !0;
 
     function Pe(e) {
         Ae = e
     }
     var Le = function(e) {
-        this.value = e, this.dep = new ve, this.vmCount = 0, B(e, "__ob__", this), Array.isArray(e) ? (U ? function(e, t) {
+        this.value = e, this.dep = new ve, this.vmCount = 0, $(e, "__ob__", this), Array.isArray(e) ? (U ? function(e, t) {
             e.__proto__ = t
         }(e, Me) : function(e, t, n) {
             for (var i = 0, r = n.length; i < r; i++) {
                 var a = n[i];
-                B(e, a, t[a])
+                $(e, a, t[a])
             }
         }(e, Me, Te), this.observeArray(e)) : this.walk(e)
     };
 
     function qe(e, t) {
         var n;
         if (a(e) && !(e instanceof ye)) return b(e, "__ob__") && e.__ob__ instanceof Le ? n = e.__ob__ : Ae && !re() && (Array.isArray(e) || l(e)) && Object.isExtensible(e) && !e._isVue && (n = new Le(e)), t && n && n.vmCount++, n
@@ -5090,26 +5090,26 @@
         var n = t ? e ? e.concat(t) : Array.isArray(t) ? t : [t] : e;
         return n ? function(e) {
             for (var t = [], n = 0; n < e.length; n++) - 1 === t.indexOf(e[n]) && t.push(e[n]);
             return t
         }(n) : n
     }
 
-    function Fe(e, t, n, i) {
+    function Be(e, t, n, i) {
         var r = Object.create(e || null);
         return t ? (Ve(i, t, n), A(r, t)) : r
     }
     Ne.el = Ne.propsData = function(e, t, n, i) {
-        return n || ce('option "' + i + '" can only be used during instance creation with the `new` keyword.'), $e(e, t)
+        return n || ce('option "' + i + '" can only be used during instance creation with the `new` keyword.'), Fe(e, t)
     }, Ne.data = function(e, t, n) {
         return n ? Re(e, t, n) : t && "function" != typeof t ? (ce('The "data" option should be a function that returns a per-instance value in component definitions.', n), e) : Re(e, t)
     }, R.forEach((function(e) {
         Ne[e] = Ie
     })), j.forEach((function(e) {
-        Ne[e + "s"] = Fe
+        Ne[e + "s"] = Be
     })), Ne.watch = function(e, t, n, i) {
         if (e === te && (e = void 0), t === te && (t = void 0), !t) return Object.create(e || null);
         if (Ve(i, t, n), !e) return t;
         var r = {};
         for (var a in A(r, e), t) {
             var o = r[a],
                 s = t[a];
@@ -5117,29 +5117,29 @@
         }
         return r
     }, Ne.props = Ne.methods = Ne.inject = Ne.computed = function(e, t, n, i) {
         if (t && Ve(i, t, n), !e) return t;
         var r = Object.create(null);
         return A(r, e), t && A(r, t), r
     }, Ne.provide = Re;
-    var $e = function(e, t) {
+    var Fe = function(e, t) {
         return void 0 === t ? e : t
     };
 
-    function Be(e) {
-        new RegExp("^[a-zA-Z][\\-\\.0-9_" + F.source + "]*$").test(e) || ce('Invalid component name: "' + e + '". Component names should conform to valid custom element name in html5 specification.'), (m(e) || I.isReservedTag(e)) && ce("Do not use built-in or reserved HTML elements as component id: " + e)
+    function $e(e) {
+        new RegExp("^[a-zA-Z][\\-\\.0-9_" + B.source + "]*$").test(e) || ce('Invalid component name: "' + e + '". Component names should conform to valid custom element name in html5 specification.'), (m(e) || I.isReservedTag(e)) && ce("Do not use built-in or reserved HTML elements as component id: " + e)
     }
 
     function Ve(e, t, n) {
         l(t) || ce('Invalid value for option "' + e + '": expected an Object, but got ' + s(t) + ".", n)
     }
 
     function He(e, t, n) {
         if (function(e) {
-                for (var t in e.components) Be(t)
+                for (var t in e.components) $e(t)
             }(t), "function" == typeof t && (t = t.options), function(e, t) {
                 var n = e.props;
                 if (n) {
                     var i, r, a = {};
                     if (Array.isArray(n))
                         for (i = n.length; i--;) "string" == typeof(r = n[i]) ? a[k(r)] = {
                             type: null
@@ -5182,15 +5182,15 @@
             }(t), !t._base && (t.extends && (e = He(e, t.extends, n)), t.mixins))
             for (var i = 0, r = t.mixins.length; i < r; i++) e = He(e, t.mixins[i], n);
         var a, o = {};
         for (a in e) c(a);
         for (a in t) b(e, a) || c(a);
 
         function c(i) {
-            var r = Ne[i] || $e;
+            var r = Ne[i] || Fe;
             o[i] = r(e[i], t[i], n, i)
         }
         return o
     }
 
     function Ue(e, t, n, i) {
         if ("string" == typeof n) {
@@ -5556,39 +5556,39 @@
     function It(t, n, i) {
         var r, a = Object.keys(n).length > 0,
             o = t ? !!t.$stable : !a,
             s = t && t.$key;
         if (t) {
             if (t._normalized) return t._normalized;
             if (o && i && i !== e && s === i.$key && !a && !i.$hasNormal) return i;
-            for (var l in r = {}, t) t[l] && "$" !== l[0] && (r[l] = Ft(n, l, t[l]))
+            for (var l in r = {}, t) t[l] && "$" !== l[0] && (r[l] = Bt(n, l, t[l]))
         } else r = {};
-        for (var c in n) c in r || (r[c] = $t(n, c));
-        return t && Object.isExtensible(t) && (t._normalized = r), B(r, "$stable", o), B(r, "$key", s), B(r, "$hasNormal", a), r
+        for (var c in n) c in r || (r[c] = Ft(n, c));
+        return t && Object.isExtensible(t) && (t._normalized = r), $(r, "$stable", o), $(r, "$key", s), $(r, "$hasNormal", a), r
     }
 
-    function Ft(e, t, n) {
+    function Bt(e, t, n) {
         var i = function() {
             var e = arguments.length ? n.apply(null, arguments) : n({});
             return (e = e && "object" == typeof e && !Array.isArray(e) ? [e] : Et(e)) && (0 === e.length || 1 === e.length && e[0].isComment) ? void 0 : e
         };
         return n.proxy && Object.defineProperty(e, t, {
             get: i,
             enumerable: !0,
             configurable: !0
         }), i
     }
 
-    function $t(e, t) {
+    function Ft(e, t) {
         return function() {
             return e[t]
         }
     }
 
-    function Bt(e, t) {
+    function $t(e, t) {
         var i, r, o, s, l;
         if (Array.isArray(e) || "string" == typeof e)
             for (i = new Array(e.length), r = 0, o = e.length; r < o; r++) i[r] = t(e[r], r);
         else if ("number" == typeof e)
             for (i = new Array(e), r = 0; r < e; r++) i[r] = t(r + 1, r);
         else if (a(e))
             if (le && e[Symbol.iterator]) {
@@ -5696,15 +5696,15 @@
     }
 
     function tn(e, t) {
         return "string" == typeof e ? t + e : e
     }
 
     function nn(e) {
-        e._o = Gt, e._n = f, e._s = h, e._l = Bt, e._t = Vt, e._q = E, e._i = D, e._m = Qt, e._f = Ht, e._k = Wt, e._b = Yt, e._v = xe, e._e = ke, e._u = Xt, e._g = Jt, e._d = en, e._p = tn
+        e._o = Gt, e._n = f, e._s = h, e._l = $t, e._t = Vt, e._q = E, e._i = D, e._m = Qt, e._f = Ht, e._k = Wt, e._b = Yt, e._v = xe, e._e = ke, e._u = Xt, e._g = Jt, e._d = en, e._p = tn
     }
 
     function rn(t, n, r, a, o) {
         var s, l = this,
             c = o.options;
         b(a, "_uid") ? (s = Object.create(a))._original = a : (s = a, a = a._original);
         var u = i(c._compiled),
@@ -6024,25 +6024,25 @@
         En = [],
         Dn = {},
         zn = {},
         Nn = !1,
         jn = !1,
         Rn = 0;
     var In = 0,
-        Fn = Date.now;
+        Bn = Date.now;
     if (W && !K) {
-        var $n = window.performance;
-        $n && "function" == typeof $n.now && Fn() > document.createEvent("Event").timeStamp && (Fn = function() {
-            return $n.now()
+        var Fn = window.performance;
+        Fn && "function" == typeof Fn.now && Bn() > document.createEvent("Event").timeStamp && (Bn = function() {
+            return Fn.now()
         })
     }
 
-    function Bn() {
+    function $n() {
         var e, t;
-        for (In = Fn(), jn = !0, On.sort((function(e, t) {
+        for (In = Bn(), jn = !0, On.sort((function(e, t) {
                 return e.id - t.id
             })), Rn = 0; Rn < On.length; Rn++)
             if ((e = On[Rn]).before && e.before(), t = e.id, Dn[t] = null, e.run(), null != Dn[t] && (zn[t] = (zn[t] || 0) + 1, zn[t] > qn)) {
                 ce("You may have an infinite update loop " + (e.user ? 'in watcher with expression "' + e.expression + '"' : "in a component render function."), e.vm);
                 break
             } var n = En.slice(),
             i = On.slice();
@@ -6102,16 +6102,16 @@
             var t = e.id;
             if (null == Dn[t]) {
                 if (Dn[t] = !0, jn) {
                     for (var n = On.length - 1; n > Rn && On[n].id > e.id;) n--;
                     On.splice(n + 1, 0, e)
                 } else On.push(e);
                 if (!Nn) {
-                    if (Nn = !0, !I.async) return void Bn();
-                    mt(Bn)
+                    if (Nn = !0, !I.async) return void $n();
+                    mt($n)
                 }
             }
         }(this)
     }, Hn.prototype.run = function() {
         if (this.active) {
             var e = this.get();
             if (e !== this.value || a(e) || this.deep) {
@@ -6166,15 +6166,15 @@
                     a || Cn || ce("Avoid mutating a prop directly since the value will be overwritten whenever the parent component re-renders. Instead, use a data or computed property based on the prop's value. Prop being mutated: \"" + o + '"', e)
                 })), o in e || Wn(e, "_props", o)
             };
             for (var s in t) o(s);
             Pe(!0)
         }(e, t.props), t.methods && function(e, t) {
             var n = e.$options.props;
-            for (var i in t) "function" != typeof t[i] && ce('Method "' + i + '" has type "' + typeof t[i] + '" in the component definition. Did you reference the function correctly?', e), n && b(n, i) && ce('Method "' + i + '" has already been defined as a prop.', e), i in e && $(i) && ce('Method "' + i + '" conflicts with an existing Vue instance method. Avoid defining component methods that start with _ or $.'), e[i] = "function" != typeof t[i] ? L : M(t[i], e)
+            for (var i in t) "function" != typeof t[i] && ce('Method "' + i + '" has type "' + typeof t[i] + '" in the component definition. Did you reference the function correctly?', e), n && b(n, i) && ce('Method "' + i + '" has already been defined as a prop.', e), i in e && F(i) && ce('Method "' + i + '" conflicts with an existing Vue instance method. Avoid defining component methods that start with _ or $.'), e[i] = "function" != typeof t[i] ? L : M(t[i], e)
         }(e, t.methods), t.data ? function(e) {
             var t = e.$options.data;
             t = e._data = "function" == typeof t ? function(e, t) {
                 _e();
                 try {
                     return e.call(t, t)
                 } catch (e) {
@@ -6185,15 +6185,15 @@
             }(t, e) : t || {}, l(t) || (t = {}, ce("data functions should return an object:\nhttps://vuejs.org/v2/guide/components.html#data-Must-Be-a-Function", e));
             var n = Object.keys(t),
                 i = e.$options.props,
                 r = e.$options.methods,
                 a = n.length;
             for (; a--;) {
                 var o = n[a];
-                r && b(r, o) && ce('Method "' + o + '" has already been defined as a data property.', e), i && b(i, o) ? ce('The data property "' + o + '" is already declared as a prop. Use prop default value instead.', e) : $(o) || Wn(e, "_data", o)
+                r && b(r, o) && ce('Method "' + o + '" has already been defined as a data property.', e), i && b(i, o) ? ce('The data property "' + o + '" is already declared as a prop. Use prop default value instead.', e) : F(o) || Wn(e, "_data", o)
             }
             qe(t, !0)
         }(e) : qe(e._data = {}, !0), t.computed && function(e, t) {
             var n = e._computedWatchers = Object.create(null),
                 i = re();
             for (var r in t) {
                 var a = t[r],
@@ -6266,15 +6266,15 @@
         e.extend = function(e) {
             e = e || {};
             var n = this,
                 i = n.cid,
                 r = e._Ctor || (e._Ctor = {});
             if (r[i]) return r[i];
             var a = e.name || n.options.name;
-            a && Be(a);
+            a && $e(a);
             var o = function(e) {
                 this._init(e)
             };
             return (o.prototype = Object.create(n.prototype)).constructor = o, o.cid = t++, o.options = He(n.options, e), o.super = n, o.options.props && function(e) {
                 var t = e.options.props;
                 for (var n in t) Wn(e.prototype, "_props", n)
             }(o), o.options.computed && function(e) {
@@ -6557,15 +6557,15 @@
                 e.mixin = function(e) {
                     return this.options = He(this.options, e), this
                 }
             }(e), ni(e),
             function(e) {
                 j.forEach((function(t) {
                     e[t] = function(e, n) {
-                        return n ? ("component" === t && Be(e), "component" === t && l(n) && (n.name = n.name || e, n = this.options._base.extend(n)), "directive" === t && "function" == typeof n && (n = {
+                        return n ? ("component" === t && $e(e), "component" === t && l(n) && (n.name = n.name || e, n = this.options._base.extend(n)), "directive" === t && "function" == typeof n && (n = {
                             bind: n,
                             update: n
                         }), this.options[t + "s"][e] = n, n) : this.options[t + "s"][e]
                     }
                 }))
             }(e)
     }(ti), Object.defineProperty(ti.prototype, "$isServer", {
@@ -6726,27 +6726,27 @@
 
     function Ri(e, t, i) {
         var r, a, o = {};
         for (r = t; r <= i; ++r) n(a = e[r].key) && (o[a] = r);
         return o
     }
     var Ii = {
-        create: Fi,
-        update: Fi,
+        create: Bi,
+        update: Bi,
         destroy: function(e) {
-            Fi(e, zi)
+            Bi(e, zi)
         }
     };
 
-    function Fi(e, t) {
+    function Bi(e, t) {
         (e.data.directives || t.data.directives) && function(e, t) {
             var n, i, r, a = e === zi,
                 o = t === zi,
-                s = Bi(e.data.directives, e.context),
-                l = Bi(t.data.directives, t.context),
+                s = $i(e.data.directives, e.context),
+                l = $i(t.data.directives, t.context),
                 c = [],
                 u = [];
             for (n in l) i = s[n], r = l[n], i ? (r.oldValue = i.value, r.oldArg = i.arg, Hi(r, "update", t, e), r.def && r.def.componentUpdated && u.push(r)) : (Hi(r, "bind", t, e), r.def && r.def.inserted && c.push(r));
             if (c.length) {
                 var d = function() {
                     for (var n = 0; n < c.length; n++) Hi(c[n], "inserted", t, e)
                 };
@@ -6755,20 +6755,20 @@
             u.length && qt(t, "postpatch", (function() {
                 for (var n = 0; n < u.length; n++) Hi(u[n], "componentUpdated", t, e)
             }));
             if (!a)
                 for (n in s) l[n] || Hi(s[n], "unbind", e, e, o)
         }(e, t)
     }
-    var $i = Object.create(null);
+    var Fi = Object.create(null);
 
-    function Bi(e, t) {
+    function $i(e, t) {
         var n, i, r = Object.create(null);
         if (!e) return r;
-        for (n = 0; n < e.length; n++)(i = e[n]).modifiers || (i.modifiers = $i), r[Vi(i)] = i, i.def = Ue(t.$options, "directives", i.name, !0);
+        for (n = 0; n < e.length; n++)(i = e[n]).modifiers || (i.modifiers = Fi), r[Vi(i)] = i, i.def = Ue(t.$options, "directives", i.name, !0);
         return r
     }
 
     function Vi(e) {
         return e.rawName || e.name + "." + Object.keys(e.modifiers || {}).join(".")
     }
 
@@ -7136,36 +7136,36 @@
             if (n(r)) {
                 if (r.number) return f(i) !== f(t);
                 if (r.trim) return i.trim() !== t.trim()
             }
             return i !== t
         }(e, t))
     }
-    var Fr = {
+    var Br = {
             create: Rr,
             update: Rr
         },
-        $r = y((function(e) {
+        Fr = y((function(e) {
             var t = {},
                 n = /:(.+)/;
             return e.split(/;(?![^(]*\))/g).forEach((function(e) {
                 if (e) {
                     var i = e.split(n);
                     i.length > 1 && (t[i[0].trim()] = i[1].trim())
                 }
             })), t
         }));
 
-    function Br(e) {
+    function $r(e) {
         var t = Vr(e.style);
         return e.staticStyle ? A(e.staticStyle, t) : t
     }
 
     function Vr(e) {
-        return Array.isArray(e) ? P(e) : "string" == typeof e ? $r(e) : e
+        return Array.isArray(e) ? P(e) : "string" == typeof e ? Fr(e) : e
     }
     var Hr, Ur = /^--/,
         Wr = /\s*!important$/,
         Yr = function(e, t, n) {
             if (Ur.test(t)) e.style.setProperty(t, n);
             else if (Wr.test(n)) e.style.setProperty(C(t), n.replace(Wr, ""), "important");
             else {
@@ -7193,17 +7193,17 @@
                 u = a.normalizedStyle || a.style || {},
                 d = c || u,
                 h = Vr(i.data.style) || {};
             i.data.normalizedStyle = n(h.__ob__) ? A({}, h) : h;
             var f = function(e, t) {
                 var n, i = {};
                 if (t)
-                    for (var r = e; r.componentInstance;)(r = r.componentInstance._vnode) && r.data && (n = Br(r.data)) && A(i, n);
-                (n = Br(e.data)) && A(i, n);
-                for (var a = e; a = a.parent;) a.data && (n = Br(a.data)) && A(i, n);
+                    for (var r = e; r.componentInstance;)(r = r.componentInstance._vnode) && r.data && (n = $r(r.data)) && A(i, n);
+                (n = $r(e.data)) && A(i, n);
+                for (var a = e; a = a.parent;) a.data && (n = $r(a.data)) && A(i, n);
                 return i
             }(i, !0);
             for (s in d) t(f[s]) && Yr(l, s, "");
             for (s in f)(o = f[s]) !== d[s] && Yr(l, s, null == o ? "" : o)
         }
     }
     var Zr = {
@@ -7645,15 +7645,15 @@
                 }
                 return P(r, d, c), r.elm
             }
             n(e) && x(e)
         }
     }({
         nodeOps: Oi,
-        modules: [Gi, rr, jr, Fr, Zr, W ? {
+        modules: [Gi, rr, jr, Br, Zr, W ? {
             create: Sa,
             activate: Sa,
             remove: function(e, t) {
                 !0 !== e.data.show ? ya(e, t) : t()
             }
         } : {}].concat(Ui)
     });
@@ -7777,56 +7777,56 @@
             n = e.$options;
         for (var i in n.propsData) t[i] = e[i];
         var r = n._parentListeners;
         for (var a in r) t[k(a)] = r[a];
         return t
     }
 
-    function Fa(e, t) {
+    function Ba(e, t) {
         if (/\d-keep-alive$/.test(t.tag)) return e("keep-alive", {
             props: t.componentOptions.propsData
         })
     }
-    var $a = function(e) {
+    var Fa = function(e) {
             return e.tag || _n(e)
         },
-        Ba = function(e) {
+        $a = function(e) {
             return "show" === e.name
         },
         Va = {
             name: "transition",
             props: ja,
             abstract: !0,
             render: function(e) {
                 var t = this,
                     n = this.$slots.default;
-                if (n && (n = n.filter($a)).length) {
+                if (n && (n = n.filter(Fa)).length) {
                     n.length > 1 && ce("<transition> can only be used on a single element. Use <transition-group> for lists.", this.$parent);
                     var i = this.mode;
                     i && "in-out" !== i && "out-in" !== i && ce("invalid <transition> mode: " + i, this.$parent);
                     var a = n[0];
                     if (function(e) {
                             for (; e = e.parent;)
                                 if (e.data.transition) return !0
                         }(this.$vnode)) return a;
                     var o = Ra(a);
                     if (!o) return a;
-                    if (this._leaving) return Fa(e, a);
+                    if (this._leaving) return Ba(e, a);
                     var s = "__transition-" + this._uid + "-";
                     o.key = null == o.key ? o.isComment ? s + "comment" : s + o.tag : r(o.key) ? 0 === String(o.key).indexOf(s) ? o.key : s + o.key : o.key;
                     var l = (o.data || (o.data = {})).transition = Ia(this),
                         c = this._vnode,
                         u = Ra(c);
-                    if (o.data.directives && o.data.directives.some(Ba) && (o.data.show = !0), u && u.data && ! function(e, t) {
+                    if (o.data.directives && o.data.directives.some($a) && (o.data.show = !0), u && u.data && ! function(e, t) {
                             return t.key === e.key && t.tag === e.tag
                         }(o, u) && !_n(u) && (!u.componentInstance || !u.componentInstance._vnode.isComment)) {
                         var d = u.data.transition = A({}, l);
                         if ("out-in" === i) return this._leaving = !0, qt(d, "afterLeave", (function() {
                             t._leaving = !1, t.$forceUpdate()
-                        })), Fa(e, a);
+                        })), Ba(e, a);
                         if ("in-out" === i) {
                             if (_n(o)) return c;
                             var h, f = function() {
                                 h()
                             };
                             qt(l, "afterEnter", f), qt(l, "enterCancelled", f), qt(d, "delayLeave", (function(e) {
                                 h = e
@@ -7989,15 +7989,15 @@
         }
     };
     var to, no = {
             staticKeys: ["staticStyle"],
             transformNode: function(e, t) {
                 var n = t.warn || lr,
                     i = _r(e, "style");
-                i && (Xa(i, t.delimiters) && n('style="' + i + '": Interpolation inside attributes has been removed. Use v-bind or the colon shorthand instead. For example, instead of <div style="{{ val }}">, use <div :style="val">.', e.rawAttrsMap.style), e.staticStyle = JSON.stringify($r(i)));
+                i && (Xa(i, t.delimiters) && n('style="' + i + '": Interpolation inside attributes has been removed. Use v-bind or the colon shorthand instead. For example, instead of <div style="{{ val }}">, use <div :style="val">.', e.rawAttrsMap.style), e.staticStyle = JSON.stringify(Fr(i)));
                 var r = gr(e, "style", !1);
                 r && (e.styleBinding = r)
             },
             genData: function(e) {
                 var t = "";
                 return e.staticStyle && (t += "staticStyle:" + e.staticStyle + ","), e.styleBinding && (t += "style:(" + e.styleBinding + "),"), t
             }
@@ -8006,15 +8006,15 @@
             return (to = to || document.createElement("div")).innerHTML = e, to.textContent
         },
         ro = p("area,base,br,col,embed,frame,hr,img,input,isindex,keygen,link,meta,param,source,track,wbr"),
         ao = p("colgroup,dd,dt,li,options,p,td,tfoot,th,thead,tr,source"),
         oo = p("address,article,aside,base,blockquote,body,caption,col,colgroup,dd,details,dialog,div,dl,dt,fieldset,figcaption,figure,footer,form,h1,h2,h3,h4,h5,h6,head,header,hgroup,hr,html,legend,li,menuitem,meta,optgroup,option,param,rp,rt,source,style,summary,tbody,td,tfoot,th,thead,title,tr,track"),
         so = /^\s*([^\s"'<>\/=]+)(?:\s*(=)\s*(?:"([^"]*)"+|'([^']*)'+|([^\s"'=<>`]+)))?/,
         lo = /^\s*((?:v-[\w-]+:|@|:|#)\[[^=]+\][^\s"'<>\/=]*)(?:\s*(=)\s*(?:"([^"]*)"+|'([^']*)'+|([^\s"'=<>`]+)))?/,
-        co = "[a-zA-Z_][\\-\\.0-9_a-zA-Z" + F.source + "]*",
+        co = "[a-zA-Z_][\\-\\.0-9_a-zA-Z" + B.source + "]*",
         uo = "((?:" + co + "\\:)?" + co + ")",
         ho = new RegExp("^<" + uo),
         fo = /^\s*(\/?)>/,
         po = new RegExp("^<\\/" + uo + "[^>]*>"),
         mo = /^<!DOCTYPE [^>]+>/i,
         vo = /^<!\--/,
         go = /^<!\[/,
@@ -8043,17 +8043,17 @@
         }))
     }
     var Mo, To, Ao, Po, Lo, qo, Oo, Eo, Do, zo = /^@|^v-on:/,
         No = /^v-|^@|^:|^#/,
         jo = /([\s\S]*?)\s+(?:in|of)\s+([\s\S]*)/,
         Ro = /,([^,\}\]]*)(?:,([^,\}\]]*))?$/,
         Io = /^\(|\)$/g,
-        Fo = /^\[.*\]$/,
-        $o = /:(.*)$/,
-        Bo = /^:|^\.|^v-bind:/,
+        Bo = /^\[.*\]$/,
+        Fo = /:(.*)$/,
+        $o = /^:|^\.|^v-bind:/,
         Vo = /\.[^.\]]+(?=[^\]]*$)/g,
         Ho = /^v-slot(:|$)|^#/,
         Uo = /[\r\n]/,
         Wo = /\s+/g,
         Yo = /[\s"'<>\/=]/,
         Qo = y(io),
         Go = "_empty_";
@@ -8394,20 +8394,20 @@
                 null != _r(e, "inline-template") && (e.inlineTemplate = !0)
             }(e);
         for (var i = 0; i < Ao.length; i++) e = Ao[i](e, t) || e;
         return function(e) {
             var t, n, i, r, a, o, s, l, c = e.attrsList;
             for (t = 0, n = c.length; t < n; t++) {
                 if (i = r = c[t].name, a = c[t].value, No.test(i))
-                    if (e.hasBindings = !0, (o = ns(i.replace(No, ""))) && (i = i.replace(Vo, "")), Bo.test(i)) i = i.replace(Bo, ""), a = or(a), (l = Fo.test(i)) && (i = i.slice(1, -1)), 0 === a.trim().length && Mo('The value for a v-bind expression cannot be empty. Found in "v-bind:' + i + '"'), o && (o.prop && !l && "innerHtml" === (i = k(i)) && (i = "innerHTML"), o.camel && !l && (i = k(i)), o.sync && (s = kr(a, "$event"), l ? mr(e, '"update:"+(' + i + ")", s, null, !1, Mo, c[t], !0) : (mr(e, "update:" + k(i), s, null, !1, Mo, c[t]), C(i) !== k(i) && mr(e, "update:" + C(i), s, null, !1, Mo, c[t])))), o && o.prop || !e.component && Oo(e.tag, e.attrsMap.type, i) ? ur(e, i, a, c[t], l) : dr(e, i, a, c[t], l);
-                    else if (zo.test(i)) i = i.replace(zo, ""), (l = Fo.test(i)) && (i = i.slice(1, -1)), mr(e, i, a, o, !1, Mo, c[t], l);
+                    if (e.hasBindings = !0, (o = ns(i.replace(No, ""))) && (i = i.replace(Vo, "")), $o.test(i)) i = i.replace($o, ""), a = or(a), (l = Bo.test(i)) && (i = i.slice(1, -1)), 0 === a.trim().length && Mo('The value for a v-bind expression cannot be empty. Found in "v-bind:' + i + '"'), o && (o.prop && !l && "innerHtml" === (i = k(i)) && (i = "innerHTML"), o.camel && !l && (i = k(i)), o.sync && (s = kr(a, "$event"), l ? mr(e, '"update:"+(' + i + ")", s, null, !1, Mo, c[t], !0) : (mr(e, "update:" + k(i), s, null, !1, Mo, c[t]), C(i) !== k(i) && mr(e, "update:" + C(i), s, null, !1, Mo, c[t])))), o && o.prop || !e.component && Oo(e.tag, e.attrsMap.type, i) ? ur(e, i, a, c[t], l) : dr(e, i, a, c[t], l);
+                    else if (zo.test(i)) i = i.replace(zo, ""), (l = Bo.test(i)) && (i = i.slice(1, -1)), mr(e, i, a, o, !1, Mo, c[t], l);
                 else {
-                    var u = (i = i.replace(No, "")).match($o),
+                    var u = (i = i.replace(No, "")).match(Fo),
                         d = u && u[1];
-                    l = !1, d && (i = i.slice(0, -(d.length + 1)), Fo.test(d) && (d = d.slice(1, -1), l = !0)), fr(e, i, r, a, d, l, o, c[t]), "model" === i && os(e, a)
+                    l = !1, d && (i = i.slice(0, -(d.length + 1)), Bo.test(d) && (d = d.slice(1, -1), l = !0)), fr(e, i, r, a, d, l, o, c[t]), "model" === i && os(e, a)
                 } else Xa(a, To) && Mo(i + '="' + a + '": Interpolation inside attributes has been removed. Use v-bind or the colon shorthand instead. For example, instead of <div id="{{ val }}">, use <div :id="val">.', c[t]), dr(e, i, JSON.stringify(a), c[t]), !e.component && "muted" === i && Oo(e.tag, e.attrsMap.type, i) && ur(e, i, "true", c[t])
             }
         }(e), e
     }
 
     function Xo(e) {
         var t;
@@ -8428,15 +8428,15 @@
 
     function es(e, t) {
         e.ifConditions || (e.ifConditions = []), e.ifConditions.push(t)
     }
 
     function ts(e) {
         var t = e.name.replace(Ho, "");
-        return t || ("#" !== e.name[0] ? t = "default" : Mo("v-slot shorthand syntax requires a slot name.", e)), Fo.test(t) ? {
+        return t || ("#" !== e.name[0] ? t = "default" : Mo("v-slot shorthand syntax requires a slot name.", e)), Bo.test(t) ? {
             name: t.slice(1, -1),
             dynamic: !0
         } : {
             name: '"' + t + '"',
             dynamic: !1
         }
     }
@@ -8736,15 +8736,15 @@
         if (e.for && !e.forProcessed) return zs(e, t);
         if (e.if && !e.ifProcessed) return Es(e, t);
         if ("template" !== e.tag || e.slotTarget || t.pre) {
             if ("slot" === e.tag) return function(e, t) {
                 var n = e.slotName || '"default"',
                     i = Is(e, t),
                     r = "_t(" + n + (i ? "," + i : ""),
-                    a = e.attrs || e.dynamicAttrs ? Bs((e.attrs || []).concat(e.dynamicAttrs || []).map((function(e) {
+                    a = e.attrs || e.dynamicAttrs ? $s((e.attrs || []).concat(e.dynamicAttrs || []).map((function(e) {
                         return {
                             name: k(e.name),
                             value: e.value,
                             dynamic: e.dynamic
                         }
                     }))) : null,
                     o = e.attrsMap["v-bind"];
@@ -8825,15 +8825,15 @@
                     var c = t.directives[a.name];
                     c && (o = !!c(e, a, t.warn)), o && (l = !0, s += '{name:"' + a.name + '",rawName:"' + a.rawName + '"' + (a.value ? ",value:(" + a.value + "),expression:" + JSON.stringify(a.value) : "") + (a.arg ? ",arg:" + (a.isDynamicArg ? a.arg : '"' + a.arg + '"') : "") + (a.modifiers ? ",modifiers:" + JSON.stringify(a.modifiers) : "") + "},")
                 }
                 if (l) return s.slice(0, -1) + "]"
             }(e, t);
         i && (n += i + ","), e.key && (n += "key:" + e.key + ","), e.ref && (n += "ref:" + e.ref + ","), e.refInFor && (n += "refInFor:true,"), e.pre && (n += "pre:true,"), e.component && (n += 'tag:"' + e.tag + '",');
         for (var r = 0; r < t.dataGenFns.length; r++) n += t.dataGenFns[r](e);
-        if (e.attrs && (n += "attrs:" + Bs(e.attrs) + ","), e.props && (n += "domProps:" + Bs(e.props) + ","), e.events && (n += Ss(e.events, !1) + ","), e.nativeEvents && (n += Ss(e.nativeEvents, !0) + ","), e.slotTarget && !e.slotScope && (n += "slot:" + e.slotTarget + ","), e.scopedSlots && (n += function(e, t, n) {
+        if (e.attrs && (n += "attrs:" + $s(e.attrs) + ","), e.props && (n += "domProps:" + $s(e.props) + ","), e.events && (n += Ss(e.events, !1) + ","), e.nativeEvents && (n += Ss(e.nativeEvents, !0) + ","), e.slotTarget && !e.slotScope && (n += "slot:" + e.slotTarget + ","), e.scopedSlots && (n += function(e, t, n) {
                 var i = e.for || Object.keys(t).some((function(e) {
                         var n = t[e];
                         return n.slotTargetDynamic || n.if || n.for || js(n)
                     })),
                     r = !!e.if;
                 if (!i)
                     for (var a = e.parent; a;) {
@@ -8863,15 +8863,15 @@
                     return "inlineTemplate:{render:function(){" + i.render + "},staticRenderFns:[" + i.staticRenderFns.map((function(e) {
                         return "function(){" + e + "}"
                     })).join(",") + "]}"
                 }
             }(e, t);
             a && (n += a + ",")
         }
-        return n = n.replace(/,$/, "") + "}", e.dynamicAttrs && (n = "_b(" + n + ',"' + e.tag + '",' + Bs(e.dynamicAttrs) + ")"), e.wrapData && (n = e.wrapData(n)), e.wrapListeners && (n = e.wrapListeners(n)), n
+        return n = n.replace(/,$/, "") + "}", e.dynamicAttrs && (n = "_b(" + n + ',"' + e.tag + '",' + $s(e.dynamicAttrs) + ")"), e.wrapData && (n = e.wrapData(n)), e.wrapListeners && (n = e.wrapListeners(n)), n
     }
 
     function js(e) {
         return 1 === e.type && ("slot" === e.tag || e.children.some(js))
     }
 
     function Rs(e, t) {
@@ -8892,46 +8892,46 @@
                 var s = n ? t.maybeComponent(o) ? ",1" : ",0" : "";
                 return "" + (i || Ls)(o, t) + s
             }
             var l = n ? function(e, t) {
                     for (var n = 0, i = 0; i < e.length; i++) {
                         var r = e[i];
                         if (1 === r.type) {
-                            if (Fs(r) || r.ifConditions && r.ifConditions.some((function(e) {
-                                    return Fs(e.block)
+                            if (Bs(r) || r.ifConditions && r.ifConditions.some((function(e) {
+                                    return Bs(e.block)
                                 }))) {
                                 n = 2;
                                 break
                             }(t(r) || r.ifConditions && r.ifConditions.some((function(e) {
                                 return t(e.block)
                             }))) && (n = 1)
                         }
                     }
                     return n
                 }(a, t.maybeComponent) : 0,
-                c = r || $s;
+                c = r || Fs;
             return "[" + a.map((function(e) {
                 return c(e, t)
             })).join(",") + "]" + (l ? "," + l : "")
         }
     }
 
-    function Fs(e) {
+    function Bs(e) {
         return void 0 !== e.for || "template" === e.tag || "slot" === e.tag
     }
 
-    function $s(e, t) {
+    function Fs(e, t) {
         return 1 === e.type ? Ls(e, t) : 3 === e.type && e.isComment ? function(e) {
             return "_e(" + JSON.stringify(e.text) + ")"
         }(e) : function(e) {
             return "_v(" + (2 === e.type ? e.expression : Vs(JSON.stringify(e.text))) + ")"
         }(e)
     }
 
-    function Bs(e) {
+    function $s(e) {
         for (var t = "", n = "", i = 0; i < e.length; i++) {
             var r = e[i],
                 a = Vs(r.value);
             r.dynamic ? n += r.name + "," + a + "," : t += '"' + r.name + '":' + a + ","
         }
         return t = "{" + t.slice(0, -1) + "}", n ? "_d(" + t + ",[" + n.slice(0, -1) + "])" : t
     }
@@ -9501,44 +9501,44 @@
         }(e, t, n) : function(e, t, n) {
             return j(L(e, n), t, n)
         }(e, t, n)
     }
     S.parse = C, S.compile = M, S.tokensToFunction = T, S.tokensToRegExp = A;
     var I = Object.create(null);
 
-    function F(e, n, i) {
+    function B(e, n, i) {
         n = n || {};
         try {
             var r = I[e] || (I[e] = S.compile(e));
             return "string" == typeof n.pathMatch && (n[0] = n.pathMatch), r(n, {
                 pretty: !0
             })
         } catch (e) {
             return t("string" == typeof n.pathMatch, "missing param for " + i + ": " + e.message), ""
         } finally {
             delete n[0]
         }
     }
 
-    function $(e, i, r, a) {
+    function F(e, i, r, a) {
         var o = "string" == typeof e ? {
             path: e
         } : e;
         if (o._normalized) return o;
         if (o.name) {
             var s = (o = n({}, e)).params;
             return s && "object" == typeof s && (o.params = n({}, s)), o
         }
         if (!o.path && o.params && i) {
             (o = n({}, o))._normalized = !0;
             var l = n(n({}, i.params), o.params);
             if (i.name) o.name = i.name, o.params = l;
             else if (i.matched.length) {
                 var c = i.matched[i.matched.length - 1].path;
-                o.path = F(c, l, "path " + i.path)
+                o.path = B(c, l, "path " + i.path)
             } else t(!1, "relative params navigation requires a current route.");
             return o
         }
         var h = function(e) {
                 var t = "",
                     n = "",
                     i = e.indexOf("#");
@@ -9570,15 +9570,15 @@
         return v && "#" !== v.charAt(0) && (v = "#" + v), {
             _normalized: !0,
             path: p,
             query: m,
             hash: v
         }
     }
-    var B, V = function() {},
+    var $, V = function() {},
         H = {
             name: "RouterLink",
             props: {
                 to: {
                     type: [String, Object],
                     required: !0
                 },
@@ -9611,15 +9611,15 @@
                     u = {},
                     d = r.options.linkActiveClass,
                     h = r.options.linkExactActiveClass,
                     m = null == d ? "router-link-active" : d,
                     v = null == h ? "router-link-exact-active" : h,
                     g = null == this.activeClass ? m : this.activeClass,
                     _ = null == this.exactActiveClass ? v : this.exactActiveClass,
-                    y = l.redirectedFrom ? p(null, $(l.redirectedFrom), null, r) : l;
+                    y = l.redirectedFrom ? p(null, F(l.redirectedFrom), null, r) : l;
                 u[_] = b(a, y), u[g] = this.exact ? u[_] : function(e, t) {
                     return 0 === e.path.replace(f, "/").indexOf(t.path.replace(f, "/")) && (!t.hash || e.hash === t.hash) && function(e, t) {
                         for (var n in t)
                             if (!(n in e)) return !1;
                         return !0
                     }(e.query, t.query)
                 }(a, y);
@@ -9684,16 +9684,16 @@
             for (var t, n = 0; n < e.length; n++) {
                 if ("a" === (t = e[n]).tag) return t;
                 if (t.children && (t = W(t.children))) return t
             }
     }
 
     function Y(e) {
-        if (!Y.installed || B !== e) {
-            Y.installed = !0, B = e;
+        if (!Y.installed || $ !== e) {
+            Y.installed = !0, $ = e;
             var t = function(e) {
                     return void 0 !== e
                 },
                 n = function(e, n) {
                     var i = e.$options._parentVnode;
                     t(i) && t(i = i.data) && t(i = i.registerRouteInstance) && i(e, n)
                 };
@@ -9799,27 +9799,27 @@
     function J(n, i) {
         var r = G(n),
             a = r.pathList,
             o = r.pathMap,
             s = r.nameMap;
 
         function l(e, n, r) {
-            var l = $(e, n, !1, i),
+            var l = F(e, n, !1, i),
                 c = l.name;
             if (c) {
                 var d = s[c];
                 if (t(d, "Route with name '" + c + "' does not exist"), !d) return u(null, l);
                 var h = d.regex.keys.filter((function(e) {
                     return !e.optional
                 })).map((function(e) {
                     return e.name
                 }));
                 if ("object" != typeof l.params && (l.params = {}), n && "object" == typeof n.params)
                     for (var f in n.params) !(f in l.params) && h.indexOf(f) > -1 && (l.params[f] = n.params[f]);
-                return l.path = F(d.path, l.params, 'named route "' + c + '"'), u(d, l, r)
+                return l.path = B(d.path, l.params, 'named route "' + c + '"'), u(d, l, r)
             }
             if (l.path) {
                 l.params = {};
                 for (var p = 0; p < a.length; p++) {
                     var m = a[p],
                         v = o[m];
                     if (X(v.regex, l.path, l.params)) return u(v, l, r)
@@ -9849,27 +9849,27 @@
             }, void 0, r);
             if (h) {
                 var g = function(e, t) {
                     return w(e, t.parent ? t.parent.path : "/", !0)
                 }(h, n);
                 return l({
                     _normalized: !0,
-                    path: F(g, v, 'redirect route with path "' + g + '"'),
+                    path: B(g, v, 'redirect route with path "' + g + '"'),
                     query: f,
                     hash: m
                 }, void 0, r)
             }
             return t(!1, "invalid redirect option: " + JSON.stringify(o)), u(null, r)
         }
 
         function u(e, t, n) {
             return e && e.redirect ? c(e, n || t) : e && e.matchAs ? function(e, t, n) {
                 var i = l({
                     _normalized: !0,
-                    path: F(n, t.params, 'aliased route with path "' + n + '"')
+                    path: B(n, t.params, 'aliased route with path "' + n + '"')
                 });
                 if (i) {
                     var r = i.matched,
                         a = r[r.length - 1];
                     return t.params = i.params, u(a, t)
                 }
                 return u(null, t)
@@ -10062,15 +10062,15 @@
                 s = null;
             Ae(e, (function(e, n, i, l) {
                 if ("function" == typeof e && void 0 === e.cid) {
                     a = !0, o++;
                     var c, u = qe((function(t) {
                             (function(e) {
                                 return e.__esModule || Le && "Module" === e[Symbol.toStringTag]
-                            })(t) && (t = t.default), e.resolved = "function" == typeof t ? t : B.extend(t), i.components[l] = t, --o <= 0 && r()
+                            })(t) && (t = t.default), e.resolved = "function" == typeof t ? t : $.extend(t), i.components[l] = t, --o <= 0 && r()
                         })),
                         d = qe((function(e) {
                             var n = "Failed to resolve async component " + l + ": " + e;
                             t(!1, n), s || (s = Ce(e) ? e : new Error(n), r(s))
                         }));
                     try {
                         c = e(u, d)
@@ -10119,15 +10119,15 @@
             return e.replace(/\/$/, "")
         }(t), this.current = v, this.pending = null, this.ready = !1, this.readyCbs = [], this.readyErrorCbs = [], this.errorCbs = [], this.listeners = []
     };
 
     function Ee(e, t, n, i) {
         var r = Ae(e, (function(e, i, r, a) {
             var o = function(e, t) {
-                "function" != typeof e && (e = B.extend(e));
+                "function" != typeof e && (e = $.extend(e));
                 return e.options[t]
             }(e, t);
             if (o) return Array.isArray(o) ? o.map((function(e) {
                 return n(e, i, r, a)
             })) : n(o, i, r, a)
         }));
         return Pe(i ? r.reverse() : r)
@@ -10310,74 +10310,74 @@
             var e = this;
             if (!(this.listeners.length > 0)) {
                 var t = this.router.options.scrollBehavior,
                     n = ve && t;
                 n && this.listeners.push(oe());
                 var i = function() {
                         var t = e.current;
-                        Ie() && e.transitionTo(Fe(), (function(i) {
+                        Ie() && e.transitionTo(Be(), (function(i) {
                             n && se(e.router, i, t, !0), ve || Ve(i.fullPath)
                         }))
                     },
                     r = ve ? "popstate" : "hashchange";
                 window.addEventListener(r, i), this.listeners.push((function() {
                     window.removeEventListener(r, i)
                 }))
             }
         }, t.prototype.push = function(e, t, n) {
             var i = this,
                 r = this.current;
             this.transitionTo(e, (function(e) {
-                Be(e.fullPath), se(i.router, e, r, !1), t && t(e)
+                $e(e.fullPath), se(i.router, e, r, !1), t && t(e)
             }), n)
         }, t.prototype.replace = function(e, t, n) {
             var i = this,
                 r = this.current;
             this.transitionTo(e, (function(e) {
                 Ve(e.fullPath), se(i.router, e, r, !1), t && t(e)
             }), n)
         }, t.prototype.go = function(e) {
             window.history.go(e)
         }, t.prototype.ensureURL = function(e) {
             var t = this.current.fullPath;
-            Fe() !== t && (e ? Be(t) : Ve(t))
+            Be() !== t && (e ? $e(t) : Ve(t))
         }, t.prototype.getCurrentLocation = function() {
-            return Fe()
+            return Be()
         }, t
     }(Oe);
 
     function Ie() {
-        var e = Fe();
+        var e = Be();
         return "/" === e.charAt(0) || (Ve("/" + e), !1)
     }
 
-    function Fe() {
+    function Be() {
         var e = window.location.href,
             t = e.indexOf("#");
         if (t < 0) return "";
         var n = (e = e.slice(t + 1)).indexOf("?");
         if (n < 0) {
             var i = e.indexOf("#");
             e = i > -1 ? decodeURI(e.slice(0, i)) + e.slice(i) : decodeURI(e)
         } else e = decodeURI(e.slice(0, n)) + e.slice(n);
         return e
     }
 
-    function $e(e) {
+    function Fe(e) {
         var t = window.location.href,
             n = t.indexOf("#");
         return (n >= 0 ? t.slice(0, n) : t) + "#" + e
     }
 
-    function Be(e) {
-        ve ? ge($e(e)) : window.location.hash = e
+    function $e(e) {
+        ve ? ge(Fe(e)) : window.location.hash = e
     }
 
     function Ve(e) {
-        ve ? _e($e(e)) : window.location.replace($e(e))
+        ve ? _e(Fe(e)) : window.location.replace(Fe(e))
     }
     var He = function(e) {
             function t(t, n) {
                 e.call(this, t, n), this.stack = [], this.index = -1
             }
             return e && (t.__proto__ = e), t.prototype = Object.create(e && e.prototype), t.prototype.constructor = t, t.prototype.push = function(e, t, n) {
                 var i = this;
@@ -10496,15 +10496,15 @@
         var t = e ? e.matched ? e : this.resolve(e).route : this.currentRoute;
         return t ? [].concat.apply([], t.matched.map((function(e) {
             return Object.keys(e.components).map((function(t) {
                 return e.components[t]
             }))
         }))) : []
     }, Ue.prototype.resolve = function(e, t, n) {
-        var i = $(e, t = t || this.history.current, n, this),
+        var i = F(e, t = t || this.history.current, n, this),
             r = this.match(i, t),
             a = r.redirectedFrom || r.fullPath,
             o = function(e, t, n) {
                 var i = "hash" === n ? "#" + t : t;
                 return e ? k(e + "/" + i) : i
             }(this.history.base, a, this.mode);
         return {
@@ -11961,31 +11961,31 @@
                 E = /^[0-7]+$/,
                 D = /^\d+$/,
                 z = /^[\dA-Fa-f]+$/,
                 N = /[\u0000\u0009\u000A\u000D #%/:?@[\\]]/,
                 j = /[\u0000\u0009\u000A\u000D #/:?@[\\]]/,
                 R = /^[\u0000-\u001F ]+|[\u0000-\u001F ]+$/g,
                 I = /[\u0009\u000A\u000D]/g,
-                F = function(e, t) {
+                B = function(e, t) {
                     var n, i, r;
                     if ("[" == t.charAt(0)) {
                         if ("]" != t.charAt(t.length - 1)) return T;
-                        if (!(n = B(t.slice(1, -1)))) return T;
+                        if (!(n = $(t.slice(1, -1)))) return T;
                         e.host = n
                     } else if (K(e)) {
                         if (t = m(t), N.test(t)) return T;
-                        if (null === (n = $(t))) return T;
+                        if (null === (n = F(t))) return T;
                         e.host = n
                     } else {
                         if (j.test(t)) return T;
                         for (n = "", i = f(t), r = 0; r < i.length; r++) n += Q(i[r], H);
                         e.host = n
                     }
                 },
-                $ = function(e) {
+                F = function(e) {
                     var t, n, i, r, a, o, s, l = e.split(".");
                     if (l.length && "" == l[l.length - 1] && l.pop(), (t = l.length) > 4) return e;
                     for (n = [], i = 0; i < t; i++) {
                         if ("" == (r = l[i])) return e;
                         if (a = 10, r.length > 1 && "0" == r.charAt(0) && (a = O.test(r) ? 16 : 8, r = r.slice(8 == a ? 1 : 2)), "" === r) o = 0;
                         else {
                             if (!(10 == a ? D : 8 == a ? E : z).test(r)) return e;
@@ -11996,15 +11996,15 @@
                     for (i = 0; i < t; i++)
                         if (o = n[i], i == t - 1) {
                             if (o >= C(256, 5 - t)) return null
                         } else if (o > 255) return null;
                     for (s = n.pop(), i = 0; i < n.length; i++) s += n[i] * C(256, 3 - i);
                     return s
                 },
-                B = function(e) {
+                $ = function(e) {
                     var t, n, i, r, a, o, s, l = [0, 0, 0, 0, 0, 0, 0, 0],
                         c = 0,
                         u = null,
                         d = 0,
                         h = function() {
                             return e.charAt(d)
                         };
@@ -12257,22 +12257,22 @@
                                     u = _e;
                                     continue
                                 }
                                 if (":" != o || v) {
                                     if (o == i || "/" == o || "?" == o || "#" == o || "\\" == o && K(e)) {
                                         if (K(e) && "" == p) return T;
                                         if (n && "" == p && (Z(e) || null !== e.port)) return;
-                                        if (l = F(e, p)) return l;
+                                        if (l = B(e, p)) return l;
                                         if (p = "", u = be, n) return;
                                         continue
                                     }
                                     "[" == o ? v = !0 : "]" == o && (v = !1), p += o
                                 } else {
                                     if ("" == p) return T;
-                                    if (l = F(e, p)) return l;
+                                    if (l = B(e, p)) return l;
                                     if (p = "", u = me, n == pe) return
                                 }
                                 break;
                             case me:
                                 if (!q.test(o)) {
                                     if (o == i || "/" == o || "?" == o || "#" == o || "\\" == o && K(e) || n) {
                                         if ("" != p) {
@@ -12316,15 +12316,15 @@
                             case _e:
                                 if (o == i || "/" == o || "\\" == o || "?" == o || "#" == o) {
                                     if (!n && X(p)) u = ye;
                                     else if ("" == p) {
                                         if (e.host = "", n) return;
                                         u = be
                                     } else {
-                                        if (l = F(e, p)) return l;
+                                        if (l = B(e, p)) return l;
                                         if ("localhost" == e.host && (e.host = ""), n) return;
                                         p = "", u = be
                                     }
                                     continue
                                 }
                                 p += o;
                                 break;
@@ -12504,20 +12504,20 @@
                 }), {
                     enumerable: !0
                 }), c(Me, "toString", (function() {
                     return Te.call(this)
                 }), {
                     enumerable: !0
                 }), b) {
-                var Fe = b.createObjectURL,
-                    $e = b.revokeObjectURL;
-                Fe && c(Ce, "createObjectURL", (function(e) {
+                var Be = b.createObjectURL,
+                    Fe = b.revokeObjectURL;
+                Be && c(Ce, "createObjectURL", (function(e) {
+                    return Be.apply(b, arguments)
+                })), Fe && c(Ce, "revokeObjectURL", (function(e) {
                     return Fe.apply(b, arguments)
-                })), $e && c(Ce, "revokeObjectURL", (function(e) {
-                    return $e.apply(b, arguments)
                 }))
             }
             v(Ce, "URL"), r({
                 global: !0,
                 forced: !o,
                 sham: !a
             }, {
@@ -14322,21 +14322,21 @@
                 I = function(e, t) {
                     if (t)
                         for (var n, i, r = t.split("&"), a = 0; a < r.length;)(n = r[a++]).length && (i = n.split("="), e.push({
                             key: D(i.shift()),
                             value: D(i.join("="))
                         }))
                 },
-                F = function(e) {
+                B = function(e) {
                     this.entries.length = 0, I(this.entries, e)
                 },
-                $ = function(e, t) {
+                F = function(e, t) {
                     if (e < t) throw TypeError("Not enough arguments")
                 },
-                B = c((function(e, t) {
+                $ = c((function(e, t) {
                     T(this, {
                         type: M,
                         iterator: b(A(e).entries),
                         kind: t
                     })
                 }), "Iterator", (function() {
                     var e = P(this),
@@ -14349,15 +14349,15 @@
                     d(this, V, C);
                     var e, t, n, i, r, a, o, s, l, c = arguments.length > 0 ? arguments[0] : void 0,
                         u = [];
                     if (T(this, {
                             type: C,
                             entries: u,
                             updateURL: function() {},
-                            updateSearchParams: F
+                            updateSearchParams: B
                         }), void 0 !== c)
                         if (v(c))
                             if ("function" == typeof(e = y(c)))
                                 for (n = (t = e.call(c)).next; !(i = n.call(t)).done;) {
                                     if ((o = (a = (r = b(m(i.value))).next).call(r)).done || (s = a.call(r)).done || !a.call(r).done) throw TypeError("Expected sequence with length 2");
                                     u.push({
                                         key: o.value + "",
@@ -14369,45 +14369,45 @@
                                         value: c[l] + ""
                                     });
                             else I(u, "string" == typeof c ? "?" === c.charAt(0) ? c.slice(1) : c : c + "")
                 },
                 H = V.prototype;
             s(H, {
                 append: function(e, t) {
-                    $(arguments.length, 2);
+                    F(arguments.length, 2);
                     var n = A(this);
                     n.entries.push({
                         key: e + "",
                         value: t + ""
                     }), n.updateURL()
                 },
                 delete: function(e) {
-                    $(arguments.length, 1);
+                    F(arguments.length, 1);
                     for (var t = A(this), n = t.entries, i = e + "", r = 0; r < n.length;) n[r].key === i ? n.splice(r, 1) : r++;
                     t.updateURL()
                 },
                 get: function(e) {
-                    $(arguments.length, 1);
+                    F(arguments.length, 1);
                     for (var t = A(this).entries, n = e + "", i = 0; i < t.length; i++)
                         if (t[i].key === n) return t[i].value;
                     return null
                 },
                 getAll: function(e) {
-                    $(arguments.length, 1);
+                    F(arguments.length, 1);
                     for (var t = A(this).entries, n = e + "", i = [], r = 0; r < t.length; r++) t[r].key === n && i.push(t[r].value);
                     return i
                 },
                 has: function(e) {
-                    $(arguments.length, 1);
+                    F(arguments.length, 1);
                     for (var t = A(this).entries, n = e + "", i = 0; i < t.length;)
                         if (t[i++].key === n) return !0;
                     return !1
                 },
                 set: function(e, t) {
-                    $(arguments.length, 1);
+                    F(arguments.length, 1);
                     for (var n, i = A(this), r = i.entries, a = !1, o = e + "", s = t + "", l = 0; l < r.length; l++)(n = r[l]).key === o && (a ? r.splice(l--, 1) : (a = !0, n.value = s));
                     a || r.push({
                         key: o,
                         value: s
                     }), i.updateURL()
                 },
                 sort: function() {
@@ -14423,21 +14423,21 @@
                     }
                     i.updateURL()
                 },
                 forEach: function(e) {
                     for (var t, n = A(this).entries, i = f(e, arguments.length > 1 ? arguments[1] : void 0, 3), r = 0; r < n.length;) i((t = n[r++]).value, t.key, this)
                 },
                 keys: function() {
-                    return new B(this, "keys")
+                    return new $(this, "keys")
                 },
                 values: function() {
-                    return new B(this, "values")
+                    return new $(this, "values")
                 },
                 entries: function() {
-                    return new B(this, "entries")
+                    return new $(this, "entries")
                 }
             }, {
                 enumerable: !0
             }), o(H, S, H.entries), o(H, "toString", (function() {
                 for (var e, t = A(this).entries, n = [], i = 0; i < t.length;) e = t[i++], n.push(R(e.key) + "=" + R(e.value));
                 return n.join("&")
             }), {
@@ -14712,49 +14712,49 @@
                 E = n("b622"),
                 D = n("e538"),
                 z = n("746f"),
                 N = n("d44e"),
                 j = n("69f3"),
                 R = n("b727").forEach,
                 I = L("hidden"),
-                F = "Symbol",
-                $ = "prototype",
-                B = E("toPrimitive"),
+                B = "Symbol",
+                F = "prototype",
+                $ = E("toPrimitive"),
                 V = j.set,
-                H = j.getterFor(F),
-                U = Object[$],
+                H = j.getterFor(B),
+                U = Object[F],
                 W = r.Symbol,
                 Y = a("JSON", "stringify"),
                 Q = S.f,
                 G = C.f,
                 K = k.f,
                 Z = M.f,
                 J = P("symbols"),
                 X = P("op-symbols"),
                 ee = P("string-to-symbol-registry"),
                 te = P("symbol-to-string-registry"),
                 ne = P("wks"),
                 ie = r.QObject,
-                re = !ie || !ie[$] || !ie[$].findChild,
+                re = !ie || !ie[F] || !ie[F].findChild,
                 ae = s && u((function() {
                     return 7 != b(G({}, "a", {
                         get: function() {
                             return G(this, "a", {
                                 value: 7
                             }).a
                         }
                     })).a
                 })) ? function(e, t, n) {
                     var i = Q(U, t);
                     i && delete U[t], G(e, t, n), i && e !== U && G(U, t, i)
                 } : G,
                 oe = function(e, t) {
-                    var n = J[e] = b(W[$]);
+                    var n = J[e] = b(W[F]);
                     return V(n, {
-                        type: F,
+                        type: B,
                         tag: e,
                         description: t
                     }), s || (n.description = t), n
                 },
                 se = c ? function(e) {
                     return "symbol" == typeof e
                 } : function(e) {
@@ -14810,21 +14810,21 @@
                     n = function(e) {
                         this === U && n.call(X, e), d(this, I) && d(this[I], t) && (this[I][t] = !1), ae(this, t, _(1, e))
                     };
                 return s && re && ae(U, t, {
                     configurable: !0,
                     set: n
                 }), oe(t, e)
-            }, A(W[$], "toString", (function() {
+            }, A(W[F], "toString", (function() {
                 return H(this).tag
             })), A(W, "withoutSetter", (function(e) {
                 return oe(O(e), e)
             })), M.f = ue, C.f = le, S.f = de, w.f = k.f = he, x.f = fe, D.f = function(e) {
                 return oe(E(e), e)
-            }, s && (G(W[$], "description", {
+            }, s && (G(W[F], "description", {
                 configurable: !0,
                 get: function() {
                     return H(this).description
                 }
             }), o || A(U, "propertyIsEnumerable", ue, {
                 unsafe: !0
             }))), i({
@@ -14833,15 +14833,15 @@
                 forced: !l,
                 sham: !l
             }, {
                 Symbol: W
             }), R(y(ne), (function(e) {
                 z(e)
             })), i({
-                target: F,
+                target: B,
                 stat: !0,
                 forced: !l
             }, {
                 for: function(e) {
                     var t = String(e);
                     if (d(ee, t)) return ee[t];
                     var n = W(t);
@@ -14899,15 +14899,15 @@
                 stringify: function(e, t, n) {
                     for (var i, r = [e], a = 1; arguments.length > a;) r.push(arguments[a++]);
                     if (i = t, (f(t) || void 0 !== e) && !se(e)) return h(t) || (t = function(e, t) {
                         if ("function" == typeof i && (t = i.call(this, e, t)), !se(t)) return t
                     }), r[1] = t, Y.apply(null, r)
                 }
             });
-            W[$][B] || T(W[$], B, W[$].valueOf), N(W, F), q[I] = !0
+            W[F][$] || T(W[F], $, W[F].valueOf), N(W, B), q[I] = !0
         },
         a630: function(e, t, n) {
             var i = n("23e7"),
                 r = n("4df4");
             i({
                 target: "Array",
                 stat: !0,
@@ -15834,22 +15834,22 @@
                 E = n("2d00"),
                 D = O("species"),
                 z = "Promise",
                 N = L.get,
                 j = L.set,
                 R = L.getterFor(z),
                 I = d,
-                F = c.TypeError,
-                $ = c.document,
-                B = c.process,
+                B = c.TypeError,
+                F = c.document,
+                $ = c.process,
                 V = u("fetch"),
                 H = A.f,
                 U = H,
-                W = "process" == b(B),
-                Y = !!($ && $.createEvent && c.dispatchEvent),
+                W = "process" == b($),
+                Y = !!(F && F.createEvent && c.dispatchEvent),
                 Q = "unhandledrejection",
                 G = q(z, (function() {
                     if (!(y(I) !== String(I))) {
                         if (66 === E) return !0;
                         if (!W && "function" != typeof PromiseRejectionEvent) return !0
                     }
                     if (l && !I.prototype.finally) return !0;
@@ -15875,59 +15875,59 @@
                             for (var r = t.value, a = 1 == t.state, o = 0; i.length > o;) {
                                 var s, l, c, u = i[o++],
                                     d = a ? u.ok : u.fail,
                                     h = u.resolve,
                                     f = u.reject,
                                     p = u.domain;
                                 try {
-                                    d ? (a || (2 === t.rejection && ne(e, t), t.rejection = 1), !0 === d ? s = r : (p && p.enter(), s = d(r), p && (p.exit(), c = !0)), s === u.promise ? f(F("Promise-chain cycle")) : (l = Z(s)) ? l.call(s, h, f) : h(s)) : f(r)
+                                    d ? (a || (2 === t.rejection && ne(e, t), t.rejection = 1), !0 === d ? s = r : (p && p.enter(), s = d(r), p && (p.exit(), c = !0)), s === u.promise ? f(B("Promise-chain cycle")) : (l = Z(s)) ? l.call(s, h, f) : h(s)) : f(r)
                                 } catch (e) {
                                     p && !c && p.exit(), f(e)
                                 }
                             }
                             t.reactions = [], t.notified = !1, n && !t.rejection && ee(e, t)
                         }))
                     }
                 },
                 X = function(e, t, n) {
                     var i, r;
-                    Y ? ((i = $.createEvent("Event")).promise = t, i.reason = n, i.initEvent(e, !1, !0), c.dispatchEvent(i)) : i = {
+                    Y ? ((i = F.createEvent("Event")).promise = t, i.reason = n, i.initEvent(e, !1, !0), c.dispatchEvent(i)) : i = {
                         promise: t,
                         reason: n
                     }, (r = c["on" + e]) ? r(i) : e === Q && T("Unhandled promise rejection", n)
                 },
                 ee = function(e, t) {
                     S.call(c, (function() {
                         var n, i = t.value;
                         if (te(t) && (n = P((function() {
-                                W ? B.emit("unhandledRejection", i, e) : X(Q, e, i)
+                                W ? $.emit("unhandledRejection", i, e) : X(Q, e, i)
                             })), t.rejection = W || te(t) ? 2 : 1, n.error)) throw n.value
                     }))
                 },
                 te = function(e) {
                     return 1 !== e.rejection && !e.parent
                 },
                 ne = function(e, t) {
                     S.call(c, (function() {
-                        W ? B.emit("rejectionHandled", e) : X("rejectionhandled", e, t.value)
+                        W ? $.emit("rejectionHandled", e) : X("rejectionhandled", e, t.value)
                     }))
                 },
                 ie = function(e, t, n, i) {
                     return function(r) {
                         e(t, n, r, i)
                     }
                 },
                 re = function(e, t, n, i) {
                     t.done || (t.done = !0, i && (t = i), t.value = n, t.state = 2, J(e, t, !0))
                 },
                 ae = function(e, t, n, i) {
                     if (!t.done) {
                         t.done = !0, i && (t = i);
                         try {
-                            if (e === n) throw F("Promise can't be resolved itself");
+                            if (e === n) throw B("Promise can't be resolved itself");
                             var r = Z(n);
                             r ? C((function() {
                                 var i = {
                                     done: !1
                                 };
                                 try {
                                     r.call(n, ie(ae, e, i, t), ie(re, e, i, t))
@@ -15961,15 +15961,15 @@
                     state: 0,
                     value: void 0
                 })
             }).prototype = f(I.prototype, {
                 then: function(e, t) {
                     var n = R(this),
                         i = H(x(this, I));
-                    return i.ok = "function" != typeof e || e, i.fail = "function" == typeof t && t, i.domain = W ? B.domain : void 0, n.parent = !0, n.reactions.push(i), 0 != n.state && J(this, n, !1), i.promise
+                    return i.ok = "function" != typeof e || e, i.fail = "function" == typeof t && t, i.domain = W ? $.domain : void 0, n.parent = !0, n.reactions.push(i), 0 != n.state && J(this, n, !1), i.promise
                 },
                 catch: function(e) {
                     return this.then(void 0, e)
                 }
             }), r = function() {
                 var e = new i,
                     t = N(e);
@@ -18233,31 +18233,31 @@
                 }
 
                 function I(e, t, n) {
                     if (e % 1 != 0 || e < 0) throw new RangeError("offset is not uint");
                     if (e + t > n) throw new RangeError("Trying to access beyond buffer length")
                 }
 
-                function F(e, t, n, i, r, a) {
+                function B(e, t, n, i, r, a) {
                     if (!c.isBuffer(e)) throw new TypeError('"buffer" argument must be a Buffer instance');
                     if (t > r || t < a) throw new RangeError('"value" argument is out of bounds');
                     if (n + i > e.length) throw new RangeError("Index out of range")
                 }
 
-                function $(e, t, n, i, r, a) {
+                function F(e, t, n, i, r, a) {
                     if (n + i > e.length) throw new RangeError("Index out of range");
                     if (n < 0) throw new RangeError("Index out of range")
                 }
 
-                function B(e, t, n, i, a) {
-                    return t = +t, n >>>= 0, a || $(e, t, n, 4), r.write(e, t, n, i, 23, 4), n + 4
+                function $(e, t, n, i, a) {
+                    return t = +t, n >>>= 0, a || F(e, t, n, 4), r.write(e, t, n, i, 23, 4), n + 4
                 }
 
                 function V(e, t, n, i, a) {
-                    return t = +t, n >>>= 0, a || $(e, t, n, 8), r.write(e, t, n, i, 52, 8), n + 8
+                    return t = +t, n >>>= 0, a || F(e, t, n, 8), r.write(e, t, n, i, 52, 8), n + 8
                 }
                 c.prototype.slice = function(e, t) {
                     var n = this.length;
                     (e = ~~e) < 0 ? (e += n) < 0 && (e = 0) : e > n && (e = n), (t = void 0 === t ? n : ~~t) < 0 ? (t += n) < 0 && (t = 0) : t > n && (t = n), t < e && (t = e);
                     var i = this.subarray(e, t);
                     return Object.setPrototypeOf(i, c.prototype), i
                 }, c.prototype.readUIntLE = function(e, t, n) {
@@ -18305,69 +18305,69 @@
                 }, c.prototype.readFloatBE = function(e, t) {
                     return e >>>= 0, t || I(e, 4, this.length), r.read(this, e, !1, 23, 4)
                 }, c.prototype.readDoubleLE = function(e, t) {
                     return e >>>= 0, t || I(e, 8, this.length), r.read(this, e, !0, 52, 8)
                 }, c.prototype.readDoubleBE = function(e, t) {
                     return e >>>= 0, t || I(e, 8, this.length), r.read(this, e, !1, 52, 8)
                 }, c.prototype.writeUIntLE = function(e, t, n, i) {
-                    e = +e, t >>>= 0, n >>>= 0, i || F(this, e, t, n, Math.pow(2, 8 * n) - 1, 0);
+                    e = +e, t >>>= 0, n >>>= 0, i || B(this, e, t, n, Math.pow(2, 8 * n) - 1, 0);
                     var r = 1,
                         a = 0;
                     for (this[t] = 255 & e; ++a < n && (r *= 256);) this[t + a] = e / r & 255;
                     return t + n
                 }, c.prototype.writeUIntBE = function(e, t, n, i) {
-                    e = +e, t >>>= 0, n >>>= 0, i || F(this, e, t, n, Math.pow(2, 8 * n) - 1, 0);
+                    e = +e, t >>>= 0, n >>>= 0, i || B(this, e, t, n, Math.pow(2, 8 * n) - 1, 0);
                     var r = n - 1,
                         a = 1;
                     for (this[t + r] = 255 & e; --r >= 0 && (a *= 256);) this[t + r] = e / a & 255;
                     return t + n
                 }, c.prototype.writeUInt8 = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 1, 255, 0), this[t] = 255 & e, t + 1
+                    return e = +e, t >>>= 0, n || B(this, e, t, 1, 255, 0), this[t] = 255 & e, t + 1
                 }, c.prototype.writeUInt16LE = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 2, 65535, 0), this[t] = 255 & e, this[t + 1] = e >>> 8, t + 2
+                    return e = +e, t >>>= 0, n || B(this, e, t, 2, 65535, 0), this[t] = 255 & e, this[t + 1] = e >>> 8, t + 2
                 }, c.prototype.writeUInt16BE = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 2, 65535, 0), this[t] = e >>> 8, this[t + 1] = 255 & e, t + 2
+                    return e = +e, t >>>= 0, n || B(this, e, t, 2, 65535, 0), this[t] = e >>> 8, this[t + 1] = 255 & e, t + 2
                 }, c.prototype.writeUInt32LE = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 4, 4294967295, 0), this[t + 3] = e >>> 24, this[t + 2] = e >>> 16, this[t + 1] = e >>> 8, this[t] = 255 & e, t + 4
+                    return e = +e, t >>>= 0, n || B(this, e, t, 4, 4294967295, 0), this[t + 3] = e >>> 24, this[t + 2] = e >>> 16, this[t + 1] = e >>> 8, this[t] = 255 & e, t + 4
                 }, c.prototype.writeUInt32BE = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 4, 4294967295, 0), this[t] = e >>> 24, this[t + 1] = e >>> 16, this[t + 2] = e >>> 8, this[t + 3] = 255 & e, t + 4
+                    return e = +e, t >>>= 0, n || B(this, e, t, 4, 4294967295, 0), this[t] = e >>> 24, this[t + 1] = e >>> 16, this[t + 2] = e >>> 8, this[t + 3] = 255 & e, t + 4
                 }, c.prototype.writeIntLE = function(e, t, n, i) {
                     if (e = +e, t >>>= 0, !i) {
                         var r = Math.pow(2, 8 * n - 1);
-                        F(this, e, t, n, r - 1, -r)
+                        B(this, e, t, n, r - 1, -r)
                     }
                     var a = 0,
                         o = 1,
                         s = 0;
                     for (this[t] = 255 & e; ++a < n && (o *= 256);) e < 0 && 0 === s && 0 !== this[t + a - 1] && (s = 1), this[t + a] = (e / o >> 0) - s & 255;
                     return t + n
                 }, c.prototype.writeIntBE = function(e, t, n, i) {
                     if (e = +e, t >>>= 0, !i) {
                         var r = Math.pow(2, 8 * n - 1);
-                        F(this, e, t, n, r - 1, -r)
+                        B(this, e, t, n, r - 1, -r)
                     }
                     var a = n - 1,
                         o = 1,
                         s = 0;
                     for (this[t + a] = 255 & e; --a >= 0 && (o *= 256);) e < 0 && 0 === s && 0 !== this[t + a + 1] && (s = 1), this[t + a] = (e / o >> 0) - s & 255;
                     return t + n
                 }, c.prototype.writeInt8 = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 1, 127, -128), e < 0 && (e = 255 + e + 1), this[t] = 255 & e, t + 1
+                    return e = +e, t >>>= 0, n || B(this, e, t, 1, 127, -128), e < 0 && (e = 255 + e + 1), this[t] = 255 & e, t + 1
                 }, c.prototype.writeInt16LE = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 2, 32767, -32768), this[t] = 255 & e, this[t + 1] = e >>> 8, t + 2
+                    return e = +e, t >>>= 0, n || B(this, e, t, 2, 32767, -32768), this[t] = 255 & e, this[t + 1] = e >>> 8, t + 2
                 }, c.prototype.writeInt16BE = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 2, 32767, -32768), this[t] = e >>> 8, this[t + 1] = 255 & e, t + 2
+                    return e = +e, t >>>= 0, n || B(this, e, t, 2, 32767, -32768), this[t] = e >>> 8, this[t + 1] = 255 & e, t + 2
                 }, c.prototype.writeInt32LE = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 4, 2147483647, -2147483648), this[t] = 255 & e, this[t + 1] = e >>> 8, this[t + 2] = e >>> 16, this[t + 3] = e >>> 24, t + 4
+                    return e = +e, t >>>= 0, n || B(this, e, t, 4, 2147483647, -2147483648), this[t] = 255 & e, this[t + 1] = e >>> 8, this[t + 2] = e >>> 16, this[t + 3] = e >>> 24, t + 4
                 }, c.prototype.writeInt32BE = function(e, t, n) {
-                    return e = +e, t >>>= 0, n || F(this, e, t, 4, 2147483647, -2147483648), e < 0 && (e = 4294967295 + e + 1), this[t] = e >>> 24, this[t + 1] = e >>> 16, this[t + 2] = e >>> 8, this[t + 3] = 255 & e, t + 4
+                    return e = +e, t >>>= 0, n || B(this, e, t, 4, 2147483647, -2147483648), e < 0 && (e = 4294967295 + e + 1), this[t] = e >>> 24, this[t + 1] = e >>> 16, this[t + 2] = e >>> 8, this[t + 3] = 255 & e, t + 4
                 }, c.prototype.writeFloatLE = function(e, t, n) {
-                    return B(this, e, t, !0, n)
+                    return $(this, e, t, !0, n)
                 }, c.prototype.writeFloatBE = function(e, t, n) {
-                    return B(this, e, t, !1, n)
+                    return $(this, e, t, !1, n)
                 }, c.prototype.writeDoubleLE = function(e, t, n) {
                     return V(this, e, t, !0, n)
                 }, c.prototype.writeDoubleBE = function(e, t, n) {
                     return V(this, e, t, !1, n)
                 }, c.prototype.copy = function(e, t, n, i) {
                     if (!c.isBuffer(e)) throw new TypeError("argument should be a Buffer");
                     if (n || (n = 0), i || 0 === i || (i = this.length), t >= e.length && (t = e.length), t || (t = 0), i > 0 && i < n && (i = n), i === n) return 0;
@@ -20177,33 +20177,33 @@
                         o.set(e, t.ssr)
                     }, e.lang.set(s)
                 })), this.isoName = s.isoName, this.nativeName = s.nativeName, this.props = s) : (e.util.defineReactive(t, "lang", {}), this.set(s))
             }
         },
         I = /^rgb(a)?\((\d{1,3}),(\d{1,3}),(\d{1,3}),?([01]?\.?\d*?)?\)$/;
 
-    function F(e) {
+    function B(e) {
         var t = e.r,
             n = e.g,
             i = e.b,
             r = e.a,
             a = void 0 !== r;
         if (t = Math.round(t), n = Math.round(n), i = Math.round(i), t > 255 || n > 255 || i > 255 || a && r > 100) throw new TypeError("Expected 3 numbers below 256 (and optionally one below 100)");
         return r = a ? (256 | Math.round(255 * r / 100)).toString(16).slice(1) : "", "#" + (i | n << 8 | t << 16 | 1 << 24).toString(16).slice(1) + r
     }
 
-    function $(e) {
+    function F(e) {
         var t = e.r,
             n = e.g,
             i = e.b,
             r = e.a;
         return "rgb" + (void 0 !== r ? "a" : "") + "(" + t + "," + n + "," + i + (void 0 !== r ? "," + r / 100 : "") + ")"
     }
 
-    function B(e) {
+    function $(e) {
         if ("string" != typeof e) throw new TypeError("Expected a string");
         3 === (e = e.replace(/^#/, "")).length ? e = e[0] + e[0] + e[1] + e[1] + e[2] + e[2] : 4 === e.length && (e = e[0] + e[0] + e[1] + e[1] + e[2] + e[2] + e[3] + e[3]);
         var t = parseInt(e, 16);
         return e.length > 6 ? {
             r: t >> 24 & 255,
             g: t >> 16 & 255,
             b: t >> 8 & 255,
@@ -20284,15 +20284,15 @@
         }
     }
 
     function U(e) {
         if ("string" != typeof e) throw new TypeError("Expected a string");
         var t = e.replace(/ /g, ""),
             n = I.exec(t);
-        if (null === n) return B(t);
+        if (null === n) return $(t);
         var i = {
             r: Math.min(255, parseInt(n[2], 10)),
             g: Math.min(255, parseInt(n[3], 10)),
             b: Math.min(255, parseInt(n[4], 10))
         };
         if (n[1]) {
             var r = parseFloat(n[5]);
@@ -20319,16 +20319,16 @@
 
     function Q(e, t) {
         if (void 0 === t && (t = document.body), "string" != typeof e) throw new TypeError("Expected a string as color");
         if (!(t instanceof Element)) throw new TypeError("Expected a DOM element");
         return getComputedStyle(t).getPropertyValue("--q-color-" + e).trim() || null
     }
     var G = {
-            rgbToHex: F,
-            hexToRgb: B,
+            rgbToHex: B,
+            hexToRgb: $,
             hsvToRgb: V,
             rgbToHsv: H,
             textToRgb: U,
             lighten: function(e, t) {
                 if ("string" != typeof e) throw new TypeError("Expected a string as color");
                 if ("number" != typeof t) throw new TypeError("Expected a numeric percent");
                 var n = U(e),
@@ -20361,40 +20361,40 @@
                     h = o + d * (1 - o),
                     f = {
                         r: Math.round((i * o + l * d * (1 - o)) / h * 255),
                         g: Math.round((r * o + c * d * (1 - o)) / h * 255),
                         b: Math.round((a * o + u * d * (1 - o)) / h * 255),
                         a: Math.round(100 * h)
                     };
-                return "string" == typeof e ? F(f) : f
+                return "string" == typeof e ? B(f) : f
             },
             changeAlpha: function(e, t) {
                 if ("string" != typeof e) throw new TypeError("Expected a string as color");
                 if (void 0 === t || t < -1 || t > 1) throw new TypeError("Expected offset to be between -1 and 1");
                 var n = U(e),
                     i = n.r,
                     r = n.g,
                     a = n.b,
                     o = n.a,
                     s = void 0 !== o ? o / 100 : 0;
-                return F({
+                return B({
                     r: i,
                     g: r,
                     b: a,
                     a: Math.round(100 * Math.min(1, Math.max(0, s + t)))
                 })
             },
             setBrand: Y,
             getBrand: Q,
             getPaletteColor: function(e) {
                 if ("string" != typeof e) throw new TypeError("Expected a string as color");
                 var t = document.createElement("div");
                 t.className = "text-" + e + " invisible fixed no-pointer-events", document.body.appendChild(t);
                 var n = getComputedStyle(t).getPropertyValue("color");
-                return t.remove(), F(U(n))
+                return t.remove(), B(U(n))
             }
         },
         K = !1;
 
     function Z(e) {
         K = !0 === e.isComposing
     }
@@ -21073,60 +21073,60 @@
                         "rounded-borders": this.rounded
                     },
                     attrs: Re,
                     on: Object.assign({}, this.qListeners)
                 }, n)
             }
         }),
-        Fe = {
+        Be = {
             role: "toolbar"
         },
-        $e = e.extend({
+        Fe = e.extend({
             name: "QBar",
             mixins: [Pe, je],
             props: {
                 dense: Boolean
             },
             computed: {
                 classes: function() {
                     return "q-bar--" + (!0 === this.dense ? "dense" : "standard") + " q-bar--" + (!0 === this.isDark ? "dark" : "light")
                 }
             },
             render: function(e) {
                 return e("div", {
                     staticClass: "q-bar row no-wrap items-center",
                     class: this.classes,
-                    attrs: Fe,
+                    attrs: Be,
                     on: Object.assign({}, this.qListeners)
                 }, Le(this, "default"))
             }
         }),
-        Be = {
+        $e = {
             left: "start",
             center: "center",
             right: "end",
             between: "between",
             around: "around",
             evenly: "evenly",
             stretch: "stretch"
         },
-        Ve = Object.keys(Be),
+        Ve = Object.keys($e),
         He = {
             props: {
                 align: {
                     type: String,
                     validator: function(e) {
                         return Ve.includes(e)
                     }
                 }
             },
             computed: {
                 alignClass: function() {
                     var e = void 0 === this.align ? !0 === this.vertical ? "stretch" : "left" : this.align;
-                    return (!0 === this.vertical ? "items" : "justify") + "-" + Be[e]
+                    return (!0 === this.vertical ? "items" : "justify") + "-" + $e[e]
                 }
             }
         },
         Ue = e.extend({
             name: "QBreadcrumbs",
             mixins: [Pe, He],
             props: {
@@ -22144,50 +22144,50 @@
         return (e === window ? document.body : e).scrollHeight
     }
 
     function It(e) {
         return e === window ? window.pageYOffset || window.scrollY || document.body.scrollTop || 0 : e.scrollTop
     }
 
-    function Ft(e) {
+    function Bt(e) {
         return e === window ? window.pageXOffset || window.scrollX || document.body.scrollLeft || 0 : e.scrollLeft
     }
 
-    function $t(e, t, n) {
+    function Ft(e, t, n) {
         void 0 === n && (n = 0);
         var i = It(e);
         n <= 0 ? i !== t && Vt(e, t) : requestAnimationFrame((function() {
             var r = i + (t - i) / Math.max(16, n) * 16;
-            Vt(e, r), r !== t && $t(e, t, n - 16)
+            Vt(e, r), r !== t && Ft(e, t, n - 16)
         }))
     }
 
-    function Bt(e, t, n) {
+    function $t(e, t, n) {
         void 0 === n && (n = 0);
-        var i = Ft(e);
+        var i = Bt(e);
         n <= 0 ? i !== t && Ht(e, t) : requestAnimationFrame((function() {
             var r = i + (t - i) / Math.max(16, n) * 16;
-            Ht(e, r), r !== t && Bt(e, t, n - 16)
+            Ht(e, r), r !== t && $t(e, t, n - 16)
         }))
     }
 
     function Vt(e, t) {
         e !== window ? e.scrollTop = t : window.scrollTo(window.pageXOffset || window.scrollX || document.body.scrollLeft || 0, t)
     }
 
     function Ht(e, t) {
         e !== window ? e.scrollLeft = t : window.scrollTo(t, window.pageYOffset || window.scrollY || document.body.scrollTop || 0)
     }
 
     function Ut(e, t, n) {
-        n ? $t(e, t, n) : Vt(e, t)
+        n ? Ft(e, t, n) : Vt(e, t)
     }
 
     function Wt(e, t, n) {
-        n ? Bt(e, t, n) : Ht(e, t)
+        n ? $t(e, t, n) : Ht(e, t)
     }
 
     function Yt() {
         if (void 0 !== Dt) return Dt;
         var e = document.createElement("p"),
             t = document.createElement("div");
         Je(e, {
@@ -22214,17 +22214,17 @@
     var Gt, Kt, Zt = {
             getScrollTarget: jt,
             getScrollHeight: Rt,
             getScrollWidth: function(e) {
                 return (e === window ? document.body : e).scrollWidth
             },
             getScrollPosition: It,
-            getHorizontalScrollPosition: Ft,
-            animScrollTo: $t,
-            animHorizontalScrollTo: Bt,
+            getHorizontalScrollPosition: Bt,
+            animScrollTo: Ft,
+            animHorizontalScrollTo: $t,
             setScrollPosition: Ut,
             setHorizontalScrollPosition: Wt,
             getScrollbarWidth: Yt,
             hasScrollbar: Qt
         },
         Jt = [],
         Xt = !1,
@@ -24068,17 +24068,17 @@
                     style: this.sizeStyle,
                     on: Object.assign({}, this.qListeners),
                     attrs: this.attrs
                 }, Ee(n, this, "internal"))
             }
         }),
         In = /^#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?$/,
-        Fn = /^#[0-9a-fA-F]{4}([0-9a-fA-F]{4})?$/,
-        $n = /^#([0-9a-fA-F]{3}|[0-9a-fA-F]{4}|[0-9a-fA-F]{6}|[0-9a-fA-F]{8})$/,
-        Bn = /^rgb\(((0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5]),){2}(0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5])\)$/,
+        Bn = /^#[0-9a-fA-F]{4}([0-9a-fA-F]{4})?$/,
+        Fn = /^#([0-9a-fA-F]{3}|[0-9a-fA-F]{4}|[0-9a-fA-F]{6}|[0-9a-fA-F]{8})$/,
+        $n = /^rgb\(((0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5]),){2}(0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5])\)$/,
         Vn = /^rgba\(((0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5]),){2}(0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5]),(0|0\.[0-9]+[1-9]|0\.[1-9]+|1)\)$/,
         Hn = {
             date: function(e) {
                 return /^-?[\d]+\/[0-1]\d\/[0-3]\d$/.test(e)
             },
             time: function(e) {
                 return /^([0-1]?\d|2[0-3]):[0-5]\d$/.test(e)
@@ -24089,36 +24089,36 @@
             timeOrFulltime: function(e) {
                 return /^([0-1]?\d|2[0-3]):[0-5]\d(:[0-5]\d)?$/.test(e)
             },
             hexColor: function(e) {
                 return In.test(e)
             },
             hexaColor: function(e) {
-                return Fn.test(e)
+                return Bn.test(e)
             },
             hexOrHexaColor: function(e) {
-                return $n.test(e)
+                return Fn.test(e)
             },
             rgbColor: function(e) {
-                return Bn.test(e)
+                return $n.test(e)
             },
             rgbaColor: function(e) {
                 return Vn.test(e)
             },
             rgbOrRgbaColor: function(e) {
-                return Bn.test(e) || Vn.test(e)
+                return $n.test(e) || Vn.test(e)
             },
             hexOrRgbColor: function(e) {
-                return In.test(e) || Bn.test(e)
+                return In.test(e) || $n.test(e)
             },
             hexaOrRgbaColor: function(e) {
-                return Fn.test(e) || Vn.test(e)
+                return Bn.test(e) || Vn.test(e)
             },
             anyColor: function(e) {
-                return $n.test(e) || Bn.test(e) || Vn.test(e)
+                return Fn.test(e) || $n.test(e) || Vn.test(e)
             }
         },
         Un = {
             testPattern: Hn
         };
 
     function Wn(e, t, n) {
@@ -25666,15 +25666,15 @@
                         }
                     } else r && this.$forceUpdate()
                 },
                 __onEditorChange: function(e, t) {
                     var n, i = e.target.value;
                     if (b(e), "hex" === this.topView) {
                         if (i.length !== (!0 === this.hasAlpha ? 9 : 7) || !/^#[0-9A-Fa-f]+$/.test(i)) return !0;
-                        n = B(i)
+                        n = $(i)
                     } else {
                         var r;
                         if (!i.endsWith(")")) return !0;
                         if (!0 !== this.hasAlpha && i.startsWith("rgb(")) {
                             if (3 !== (r = i.substring(4, i.length - 1).split(",").map((function(e) {
                                     return parseInt(e, 10)
                                 }))).length || !/^rgb\([0-9]{1,3},[0-9]{1,3},[0-9]{1,3}\)$/.test(i)) return !0
@@ -25713,15 +25713,15 @@
                             g: t.g,
                             b: t.b,
                             a: t.a
                         };
                     void 0 === n.a && (n.a = this.model.a), this.model.h = t.h, this.model.s = t.s, this.model.v = t.v, this.__update(n, !0)
                 },
                 __update: function(e, t) {
-                    this.model.hex = F(e), this.model.rgb = $(e), this.model.r = e.r, this.model.g = e.g, this.model.b = e.b, this.model.a = e.a;
+                    this.model.hex = B(e), this.model.rgb = F(e), this.model.r = e.r, this.model.g = e.g, this.model.b = e.b, this.model.a = e.a;
                     var n = this.model[!0 === this.isOutputHex ? "hex" : "rgb"];
                     this.$emit("input", n), !0 === t && this.$emit("change", n)
                 },
                 __updateErrorIcon: function(e) {
                     void 0 !== this.$refs.errorIcon && (this.$refs.errorIcon.$el.style.opacity = e ? 1 : 0)
                 },
                 __parseModel: function(e) {
@@ -25734,15 +25734,15 @@
                         g: 0,
                         b: 0,
                         a: !0 === t ? 100 : void 0,
                         hex: void 0,
                         rgb: void 0
                     };
                     var n = U(e);
-                    return !0 === t && void 0 === n.a && (n.a = 100), n.hex = F(n), n.rgb = $(n), Object.assign(n, H(n))
+                    return !0 === t && void 0 === n.a && (n.a = 100), n.hex = B(n), n.rgb = F(n), Object.assign(n, H(n))
                 },
                 __spectrumPan: function(e) {
                     e.isFinal ? this.__onSpectrumChange(e.position.left, e.position.top, !0) : this.__spectrumChange(e)
                 },
                 __spectrumChange: function(e) {
                     this.__onSpectrumChange(e.position.left, e.position.top)
                 },
@@ -26113,26 +26113,26 @@
     function Ii(e, t) {
         var n = new Date(e);
         return !0 === t ? function(e) {
             return 1e4 * e.getFullYear() + 100 * e.getMonth() + e.getDate()
         }(n) : n.getTime()
     }
 
-    function Fi(e, t, n) {
+    function Bi(e, t, n) {
         var i = new Date(e),
             r = "set" + (n ? "UTC" : "");
         return Object.keys(t).forEach((function(e) {
             if ("month" !== e) {
                 var n = "year" === e ? "FullYear" : e.charAt(0).toUpperCase() + e.slice(1);
                 i["" + r + n](t[e])
             } else Ni(i, t.month)
         })), i
     }
 
-    function $i(e, t) {
+    function Fi(e, t) {
         var n = new Date(e);
         switch (t) {
             case "year":
                 n.setMonth(0);
             case "month":
                 n.setDate(1);
             case "day":
@@ -26143,40 +26143,40 @@
                 n.setSeconds(0);
             case "second":
                 n.setMilliseconds(0)
         }
         return n
     }
 
-    function Bi(e, t, n) {
+    function $i(e, t, n) {
         return (e.getTime() - e.getTimezoneOffset() * Pi - (t.getTime() - t.getTimezoneOffset() * Pi)) / n
     }
 
     function Vi(e, t, n) {
         void 0 === n && (n = "days");
         var i = new Date(e),
             r = new Date(t);
         switch (n) {
             case "years":
                 return i.getFullYear() - r.getFullYear();
             case "months":
                 return 12 * (i.getFullYear() - r.getFullYear()) + i.getMonth() - r.getMonth();
             case "days":
-                return Bi($i(i, "day"), $i(r, "day"), Ti);
+                return $i(Fi(i, "day"), Fi(r, "day"), Ti);
             case "hours":
-                return Bi($i(i, "hour"), $i(r, "hour"), Ai);
+                return $i(Fi(i, "hour"), Fi(r, "hour"), Ai);
             case "minutes":
-                return Bi($i(i, "minute"), $i(r, "minute"), Pi);
+                return $i(Fi(i, "minute"), Fi(r, "minute"), Pi);
             case "seconds":
-                return Bi($i(i, "second"), $i(r, "second"), 1e3)
+                return $i(Fi(i, "second"), Fi(r, "second"), 1e3)
         }
     }
 
     function Hi(e) {
-        return Vi(e, $i(e, "year"), "days") + 1
+        return Vi(e, Fi(e, "year"), "days") + 1
     }
 
     function Ui(e) {
         return new Date(e.getFullYear(), e.getMonth() + 1, 0).getDate()
     }
 
     function Wi(e) {
@@ -26331,15 +26331,15 @@
                     r = new Date(i.year, null === i.month ? null : i.month - 1, i.day, i.hour, i.minute, i.second, i.millisecond),
                     a = r.getTimezoneOffset();
                 return null === i.timezoneOffset || i.timezoneOffset === a ? r : ji(r, {
                     minutes: i.timezoneOffset - a
                 }, !0)
             },
             buildDate: function(e, t) {
-                return Fi(new Date, e, t)
+                return Bi(new Date, e, t)
             },
             getDayOfWeek: function(e) {
                 var t = new Date(e).getDay();
                 return 0 === t ? 7 : t
             },
             getWeekOfYear: Ri,
             isBetweenDates: function(e, t, n, i) {
@@ -26351,16 +26351,16 @@
             },
             addToDate: function(e, t) {
                 return ji(e, t, !0)
             },
             subtractFromDate: function(e, t) {
                 return ji(e, t, !1)
             },
-            adjustDate: Fi,
-            startOfDate: $i,
+            adjustDate: Bi,
+            startOfDate: Fi,
             endOfDate: function(e, t) {
                 var n = new Date(e);
                 switch (t) {
                     case "year":
                         n.setMonth(11);
                     case "month":
                         n.setDate(Ui(n));
@@ -27488,15 +27488,15 @@
     }
 
     function pr(e) {
         var t = document.body,
             n = void 0 !== window.visualViewport;
         if ("add" === e) {
             var i = window.getComputedStyle(t).overflowY;
-            Gi = Ft(window), Ki = It(window), Ji = t.style.left, Xi = t.style.top, t.style.left = "-" + Gi + "px", t.style.top = "-" + Ki + "px", "hidden" !== i && ("scroll" === i || t.scrollHeight > window.innerHeight) && t.classList.add("q-body--force-scrollbar"), t.classList.add("q-body--prevent-scroll"), document.qScrollPrevented = !0, !0 === d.is.ios && (!0 === n ? (window.scrollTo(0, 0), window.visualViewport.addEventListener("resize", fr, f.passiveCapture), window.visualViewport.addEventListener("scroll", fr, f.passiveCapture), window.scrollTo(0, 0)) : window.addEventListener("scroll", hr, f.passiveCapture))
+            Gi = Bt(window), Ki = It(window), Ji = t.style.left, Xi = t.style.top, t.style.left = "-" + Gi + "px", t.style.top = "-" + Ki + "px", "hidden" !== i && ("scroll" === i || t.scrollHeight > window.innerHeight) && t.classList.add("q-body--force-scrollbar"), t.classList.add("q-body--prevent-scroll"), document.qScrollPrevented = !0, !0 === d.is.ios && (!0 === n ? (window.scrollTo(0, 0), window.visualViewport.addEventListener("resize", fr, f.passiveCapture), window.visualViewport.addEventListener("scroll", fr, f.passiveCapture), window.scrollTo(0, 0)) : window.addEventListener("scroll", hr, f.passiveCapture))
         }!0 === d.is.desktop && !0 === d.is.mac && window[e + "EventListener"]("wheel", dr, f.notPassive), "remove" === e && (!0 === d.is.ios && (!0 === n ? (window.visualViewport.removeEventListener("resize", fr, f.passiveCapture), window.visualViewport.removeEventListener("scroll", fr, f.passiveCapture)) : window.removeEventListener("scroll", hr, f.passiveCapture)), t.classList.remove("q-body--prevent-scroll"), t.classList.remove("q-body--force-scrollbar"), document.qScrollPrevented = !1, t.style.left = Ji, t.style.top = Xi, window.scrollTo(Gi, Ki), Zi = void 0)
     }
 
     function mr(e) {
         var t = "add";
         if (!0 === e) {
             if (cr++, void 0 !== er) return clearTimeout(er), void(er = void 0);
@@ -28618,17 +28618,17 @@
                 }
             }
         },
         Ir = Object.keys(Rr);
     Ir.forEach((function(e) {
         Rr[e].regex = new RegExp(Rr[e].pattern)
     }));
-    var Fr = new RegExp("\\\\([^.*+?^${}()|([\\]])|([.*+?^${}()|[\\]])|([" + Ir.join("") + "])|(.)", "g"),
-        $r = /[.*+?^${}()|[\]\\]/g,
-        Br = String.fromCharCode(1),
+    var Br = new RegExp("\\\\([^.*+?^${}()|([\\]])|([.*+?^${}()|[\\]])|([" + Ir.join("") + "])|(.)", "g"),
+        Fr = /[.*+?^${}()|[\]\\]/g,
+        $r = String.fromCharCode(1),
         Vr = {
             props: {
                 mask: String,
                 reverseFillMask: Boolean,
                 fillMask: [Boolean, String],
                 unmaskedValue: Boolean
             },
@@ -28661,41 +28661,41 @@
                     }
                     return this.value
                 },
                 __getPaddedMaskMarked: function(e) {
                     if (e < this.maskMarked.length) return this.maskMarked.slice(-e);
                     var t = this.maskMarked,
                         n = "",
-                        i = t.indexOf(Br);
+                        i = t.indexOf($r);
                     if (i > -1) {
-                        for (var r = e - t.length; r > 0; r--) n += Br;
+                        for (var r = e - t.length; r > 0; r--) n += $r;
                         t = t.slice(0, i) + n + t.slice(i)
                     }
                     return t
                 },
                 __updateMaskInternals: function() {
                     var e = this;
                     if (this.hasMask = void 0 !== this.mask && this.mask.length > 0 && ["text", "search", "url", "tel", "password"].includes(this.type), !1 === this.hasMask) return this.computedUnmask = void 0, this.maskMarked = "", void(this.maskReplaced = "");
                     var t = void 0 === jr[this.mask] ? this.mask : jr[this.mask],
                         n = "string" == typeof this.fillMask && this.fillMask.length > 0 ? this.fillMask.slice(0, 1) : "_",
-                        i = n.replace($r, "\\$&"),
+                        i = n.replace(Fr, "\\$&"),
                         r = [],
                         a = [],
                         o = [],
                         s = !0 === this.reverseFillMask,
                         l = "",
                         c = "";
-                    t.replace(Fr, (function(e, t, n, i, u) {
+                    t.replace(Br, (function(e, t, n, i, u) {
                         if (void 0 !== i) {
                             var d = Rr[i];
                             o.push(d), c = d.negate, !0 === s && (a.push("(?:" + c + "+)?(" + d.pattern + "+)?(?:" + c + "+)?(" + d.pattern + "+)?"), s = !1), a.push("(?:" + c + "+)?(" + d.pattern + ")?")
                         } else if (void 0 !== n) l = "\\" + ("\\" === n ? "" : n), o.push(n), r.push("([^" + l + "]+)?" + l + "?");
                         else {
                             var h = void 0 !== t ? t : u;
-                            l = "\\" === h ? "\\\\\\\\" : h.replace($r, "\\\\$&"), o.push(h), r.push("([^" + l + "]+)?" + l + "?")
+                            l = "\\" === h ? "\\\\\\\\" : h.replace(Fr, "\\\\$&"), o.push(h), r.push("([^" + l + "]+)?" + l + "?")
                         }
                     }));
                     var u = new RegExp("^" + r.join("") + "(" + ("" === l ? "." : "[^" + l + "]") + "+)?$"),
                         d = a.length - 1,
                         h = a.map((function(t, n) {
                             return 0 === n && !0 === e.reverseFillMask ? new RegExp("^" + i + "*" + t) : n === d ? new RegExp("^" + t + "(" + ("" === c ? "." : c) + "+)?" + (!0 === e.reverseFillMask ? "$" : i + "*")) : new RegExp("^" + t)
                         }));
@@ -28705,16 +28705,16 @@
                         for (var n = [], i = h.length, r = 0, a = e; r < i; r++) {
                             var o = h[r].exec(a);
                             if (null === o) break;
                             a = a.slice(o.shift().length), n.push.apply(n, o)
                         }
                         return n.length > 0 ? n.join("") : e
                     }, this.maskMarked = o.map((function(e) {
-                        return "string" == typeof e ? e : Br
-                    })).join(""), this.maskReplaced = this.maskMarked.split(Br).join(n)
+                        return "string" == typeof e ? e : $r
+                    })).join(""), this.maskReplaced = this.maskMarked.split($r).join(n)
                 },
                 __updateMaskValue: function(e, t, n) {
                     var i = this,
                         r = this.$refs.input,
                         a = r.selectionEnd,
                         o = r.value.length - a,
                         s = this.__unmask(e);
@@ -28733,15 +28733,15 @@
                                 var t = Math.max(0, c.length - (c === i.maskReplaced ? 0 : Math.min(l.length, o + 1)));
                                 i.__moveCursorRightReverse(r, t, t)
                             } else {
                                 var s = c.length - o;
                                 r.setSelectionRange(s, s, "backward")
                             }
                         else if (!0 === u) {
-                            var d = Math.max(0, i.maskMarked.indexOf(Br), Math.min(l.length, a) - 1);
+                            var d = Math.max(0, i.maskMarked.indexOf($r), Math.min(l.length, a) - 1);
                             i.__moveCursorRight(r, d, d)
                         } else {
                             var h = a - 1;
                             i.__moveCursorRight(r, h, h)
                         } else {
                             var f = a - 1;
                             i.__moveCursorRight(r, f, f)
@@ -28751,52 +28751,52 @@
                         }
                     }));
                     var d = !0 === this.unmaskedValue ? this.__unmask(c) : c;
                     this.value !== d && this.__emitValue(d, !0)
                 },
                 __moveCursorForPaste: function(e, t, n) {
                     var i = this.__mask(this.__unmask(e.value));
-                    t = Math.max(0, this.maskMarked.indexOf(Br), Math.min(i.length, t)), e.setSelectionRange(t, n, "forward")
+                    t = Math.max(0, this.maskMarked.indexOf($r), Math.min(i.length, t)), e.setSelectionRange(t, n, "forward")
                 },
                 __moveCursorLeft: function(e, t, n, i) {
-                    for (var r = -1 === this.maskMarked.slice(t - 1).indexOf(Br), a = Math.max(0, t - 1); a >= 0; a--)
-                        if (this.maskMarked[a] === Br) {
+                    for (var r = -1 === this.maskMarked.slice(t - 1).indexOf($r), a = Math.max(0, t - 1); a >= 0; a--)
+                        if (this.maskMarked[a] === $r) {
                             t = a, !0 === r && t++;
                             break
-                        } if (a < 0 && void 0 !== this.maskMarked[t] && this.maskMarked[t] !== Br) return this.__moveCursorRight(e, 0, 0);
+                        } if (a < 0 && void 0 !== this.maskMarked[t] && this.maskMarked[t] !== $r) return this.__moveCursorRight(e, 0, 0);
                     t >= 0 && e.setSelectionRange(t, !0 === i ? n : t, "backward")
                 },
                 __moveCursorRight: function(e, t, n, i) {
                     for (var r = e.value.length, a = Math.min(r, n + 1); a <= r; a++) {
-                        if (this.maskMarked[a] === Br) {
+                        if (this.maskMarked[a] === $r) {
                             n = a;
                             break
                         }
-                        this.maskMarked[a - 1] === Br && (n = a)
+                        this.maskMarked[a - 1] === $r && (n = a)
                     }
-                    if (a > r && void 0 !== this.maskMarked[n - 1] && this.maskMarked[n - 1] !== Br) return this.__moveCursorLeft(e, r, r);
+                    if (a > r && void 0 !== this.maskMarked[n - 1] && this.maskMarked[n - 1] !== $r) return this.__moveCursorLeft(e, r, r);
                     e.setSelectionRange(i ? t : n, n, "forward")
                 },
                 __moveCursorLeftReverse: function(e, t, n, i) {
                     for (var r = this.__getPaddedMaskMarked(e.value.length), a = Math.max(0, t - 1); a >= 0; a--) {
-                        if (r[a - 1] === Br) {
+                        if (r[a - 1] === $r) {
                             t = a;
                             break
                         }
-                        if (r[a] === Br && (t = a, 0 === a)) break
+                        if (r[a] === $r && (t = a, 0 === a)) break
                     }
-                    if (a < 0 && void 0 !== r[t] && r[t] !== Br) return this.__moveCursorRightReverse(e, 0, 0);
+                    if (a < 0 && void 0 !== r[t] && r[t] !== $r) return this.__moveCursorRightReverse(e, 0, 0);
                     t >= 0 && e.setSelectionRange(t, !0 === i ? n : t, "backward")
                 },
                 __moveCursorRightReverse: function(e, t, n, i) {
-                    for (var r = e.value.length, a = this.__getPaddedMaskMarked(r), o = -1 === a.slice(0, n + 1).indexOf(Br), s = Math.min(r, n + 1); s <= r; s++)
-                        if (a[s - 1] === Br) {
+                    for (var r = e.value.length, a = this.__getPaddedMaskMarked(r), o = -1 === a.slice(0, n + 1).indexOf($r), s = Math.min(r, n + 1); s <= r; s++)
+                        if (a[s - 1] === $r) {
                             (n = s) > 0 && !0 === o && n--;
                             break
-                        } if (s > r && void 0 !== a[n - 1] && a[n - 1] !== Br) return this.__moveCursorLeftReverse(e, r, r);
+                        } if (s > r && void 0 !== a[n - 1] && a[n - 1] !== $r) return this.__moveCursorLeftReverse(e, r, r);
                     e.setSelectionRange(!0 === i ? t : n, n, "forward")
                 },
                 __onMaskedKeydown: function(e) {
                     if (!0 !== J(e)) {
                         var t = this.$refs.input,
                             n = t.selectionStart,
                             i = t.selectionEnd;
@@ -28818,15 +28818,15 @@
                             if (void 0 === a || !o.regex.test(a)) return i;
                             i += void 0 !== o.transform ? o.transform(a) : a, n++
                         }
                     }
                     return i
                 },
                 __maskReverse: function(e) {
-                    for (var t = this.computedMask, n = this.maskMarked.indexOf(Br), i = e.length - 1, r = "", a = t.length - 1; a >= 0; a--) {
+                    for (var t = this.computedMask, n = this.maskMarked.indexOf($r), i = e.length - 1, r = "", a = t.length - 1; a >= 0; a--) {
                         var o = t[a],
                             s = e[i];
                         if ("string" == typeof o) r = o + r, s === o && i--;
                         else {
                             if (void 0 === s || !o.regex.test(s)) return r;
                             do {
                                 r = (void 0 !== o.transform ? o.transform(s) : s) + r, s = e[--i]
@@ -31630,53 +31630,53 @@
         }),
         Ia = {
             threshold: 0,
             root: null,
             rootMargin: "0px"
         };
 
-    function Fa(e, t, n) {
+    function Ba(e, t, n) {
         var i, r, a;
         "function" == typeof n ? (i = n, r = Ia, a = void 0 === t.cfg) : (i = n.handler, r = Object.assign({}, Ia, n.cfg), a = void 0 === t.cfg || !1 === Sn(t.cfg, r)), t.handler !== i && (t.handler = i), !0 === a && (t.cfg = r, void 0 !== t.observer && t.observer.unobserve(e), t.observer = new IntersectionObserver((function(n) {
             var i = n[0];
             if ("function" == typeof t.handler) {
                 if (null === i.rootBounds && (void 0 !== e.__vue__ ? !0 !== e.__vue__._inactive : !0 === document.body.contains(e))) return t.observer.unobserve(e), void t.observer.observe(e);
-                (!1 === t.handler(i, t.observer) || !0 === t.once && !0 === i.isIntersecting) && $a(e)
+                (!1 === t.handler(i, t.observer) || !0 === t.once && !0 === i.isIntersecting) && Fa(e)
             }
         }), r), t.observer.observe(e))
     }
 
-    function $a(e) {
+    function Fa(e) {
         var t = e.__qvisible;
         void 0 !== t && (void 0 !== t.observer && t.observer.unobserve(e), delete e.__qvisible)
     }
-    var Ba = {
+    var $a = {
             name: "intersection",
             inserted: function(e, t) {
                 var n = t.modifiers,
                     i = t.value;
-                void 0 !== e.__qvisible && ($a(e), e.__qvisible_destroyed = !0);
+                void 0 !== e.__qvisible && (Fa(e), e.__qvisible_destroyed = !0);
                 var r = {
                     once: !0 === n.once
                 };
-                Fa(e, r, i), e.__qvisible = r
+                Ba(e, r, i), e.__qvisible = r
             },
             update: function(e, t) {
                 var n = e.__qvisible;
-                void 0 !== n && Fa(e, n, t.value)
+                void 0 !== n && Ba(e, n, t.value)
             },
             unbind: function(e) {
-                void 0 === e.__qvisible_destroyed ? $a(e) : delete e.__qvisible_destroyed
+                void 0 === e.__qvisible_destroyed ? Fa(e) : delete e.__qvisible_destroyed
             }
         },
         Va = e.extend({
             name: "QIntersection",
             mixins: [Ae, Pe],
             directives: {
-                Intersection: Ba
+                Intersection: $a
             },
             props: {
                 once: Boolean,
                 transition: String,
                 ssrPrerender: Boolean,
                 margin: String,
                 threshold: [Number, Array],
@@ -31914,15 +31914,15 @@
                         inflexionPosition: this.dirChangePos
                     }
                 },
                 trigger: function(e) {
                     !0 === e || 0 === this.debounce || "0" === this.debounce ? this.__emit() : this.timer || (this.timer = this.debounce ? setTimeout(this.__emit, this.debounce) : requestAnimationFrame(this.__emit))
                 },
                 __emit: function() {
-                    var e = !0 === this.horizontal ? Ft : It,
+                    var e = !0 === this.horizontal ? Bt : It,
                         t = Math.max(0, e(this.__scrollTarget)),
                         n = t - this.pos,
                         i = !0 === this.horizontal ? n < 0 ? "left" : "right" : n < 0 ? "up" : "down";
                     this.dirChanged = this.dir !== i, this.dirChanged && (this.dir = i, this.dirChangePos = this.pos), this.timer = null, this.pos = t, this.$emit("scroll", this.getPosition())
                 },
                 __configureScrollTarget: function() {
                     this.__scrollTarget = jt(this.$el.parentNode, this.scrollTarget), this.__scrollTarget.addEventListener("scroll", this.trigger, Wa), this.trigger(!0)
@@ -35155,21 +35155,21 @@
                     staticClass: "q-skeleton",
                     class: this.classes,
                     style: this.style,
                     on: Object.assign({}, this.qListeners)
                 }, Le(this, "default"))
             }
         }),
-        Fo = [
+        Bo = [
             ["left", "center", "start", "width"],
             ["right", "center", "end", "width"],
             ["top", "start", "center", "height"],
             ["bottom", "end", "center", "height"]
         ],
-        $o = e.extend({
+        Fo = e.extend({
             name: "QSlideItem",
             mixins: [je, Pe],
             props: {
                 leftColor: String,
                 rightColor: String,
                 topColor: String,
                 bottomColor: String
@@ -35196,15 +35196,15 @@
                     var t, n, i, r = this,
                         a = this.$refs.content;
                     if (e.isFirst) this.__dir = null, this.__size = {
                         left: 0,
                         right: 0,
                         top: 0,
                         bottom: 0
-                    }, this.__scale = 0, a.classList.add("no-transition"), Fo.forEach((function(e) {
+                    }, this.__scale = 0, a.classList.add("no-transition"), Bo.forEach((function(e) {
                         if (void 0 !== r.$scopedSlots[e[0]]) {
                             var t = r.$refs[e[0] + "Content"];
                             t.style.transform = "scale(1)", r.__size[e[0]] = t.getBoundingClientRect()[e[3]]
                         }
                     })), this.__axis = "up" === e.direction || "down" === e.direction ? "Y" : "X";
                     else {
                         if (e.isFinal) return a.classList.remove("no-transition"), void(1 === this.__scale ? (a.style.transform = "translate" + this.__axis + "(" + 100 * this.__dir + "%)", this.timer = setTimeout((function() {
@@ -35230,15 +35230,15 @@
                         right: void 0 !== this.$scopedSlots[this.langDir.left],
                         up: void 0 !== this.$scopedSlots.bottom,
                         down: void 0 !== this.$scopedSlots.top
                     },
                     r = Object.keys(i).filter((function(e) {
                         return !0 === i[e]
                     }));
-                return Fo.forEach((function(i) {
+                return Bo.forEach((function(i) {
                     var r = i[0];
                     void 0 !== t.$scopedSlots[r] && n.push(e("div", {
                         ref: r,
                         class: "q-slide-item__" + r + " absolute-full row no-wrap items-" + i[1] + " justify-" + i[2] + (void 0 !== t[r + "Color"] ? " bg-" + t[r + "Color"] : "")
                     }, [e("div", {
                         ref: r + "Content"
                     }, t.$scopedSlots[r]())]))
@@ -35266,15 +35266,15 @@
                     on: Object.assign({}, this.qListeners)
                 }, n)
             },
             beforeDestroy: function() {
                 clearTimeout(this.timer)
             }
         }),
-        Bo = e.extend({
+        $o = e.extend({
             name: "QSpace",
             mixins: [Pe],
             render: function(e) {
                 return e("div", {
                     staticClass: "q-space",
                     on: Object.assign({}, this.qListeners)
                 })
@@ -39180,15 +39180,15 @@
                         tabindex: -1
                     }
                 }, [this.__getHeader(e), e("div", {
                     staticClass: "q-time__main col overflow-auto"
                 }, t)])
             }
         }),
-        Fs = e.extend({
+        Bs = e.extend({
             name: "QTimeline",
             mixins: [je, Pe],
             provide: function() {
                 return {
                     __timeline: this
                 }
             },
@@ -39221,15 +39221,15 @@
                 return e("ul", {
                     staticClass: "q-timeline",
                     class: this.classes,
                     on: Object.assign({}, this.qListeners)
                 }, Le(this, "default"))
             }
         }),
-        $s = e.extend({
+        Fs = e.extend({
             name: "QTimelineEntry",
             inject: {
                 __timeline: {
                     default: function() {
                         console.error("QTimelineEntry needs to be child of QTimeline")
                     }
                 }
@@ -39301,15 +39301,15 @@
                 return e("li", {
                     staticClass: "q-timeline__entry",
                     class: this.classes,
                     on: Object.assign({}, this.qListeners)
                 }, !0 === this.reverse ? r.reverse() : r)
             }
         }),
-        Bs = e.extend({
+        $s = e.extend({
             name: "QToolbar",
             mixins: [Pe],
             props: {
                 inset: Boolean
             },
             render: function(e) {
                 return e("div", {
@@ -40219,15 +40219,15 @@
         }),
         Zs = Object.freeze({
             __proto__: null,
             QAjaxBar: Se,
             QAvatar: ze,
             QBadge: Ne,
             QBanner: Ie,
-            QBar: $e,
+            QBar: Fe,
             QBreadcrumbs: Ue,
             QBreadcrumbsEl: Ye,
             QBtn: bt,
             QBtnDropdown: sn,
             QBtnGroup: yt,
             QBtnToggle: un,
             QCard: dn,
@@ -40285,18 +40285,18 @@
             QResizeObserver: ni,
             QResponsive: xo,
             QScrollArea: So,
             QScrollObserver: Ya,
             QSelect: No,
             QSeparator: ya,
             QSkeleton: Io,
-            QSlideItem: $o,
+            QSlideItem: Fo,
             QSlideTransition: ga,
             QSlider: ei,
-            QSpace: Bo,
+            QSpace: $o,
             QSpinner: Ge,
             QSpinnerAudio: Vo,
             QSpinnerBall: Ho,
             QSpinnerBars: Uo,
             QSpinnerComment: Wo,
             QSpinnerCube: Yo,
             QSpinnerDots: Qo,
@@ -40323,18 +40323,18 @@
             QTh: ps,
             QTr: Es,
             QTd: Ds,
             QTabs: li,
             QTab: ui,
             QRouteTab: Rs,
             QTime: Is,
-            QTimeline: Fs,
-            QTimelineEntry: $s,
+            QTimeline: Bs,
+            QTimelineEntry: Fs,
             QToggle: Ja,
-            QToolbar: Bs,
+            QToolbar: $s,
             QToolbarTitle: Vs,
             QTooltip: Gr,
             QTree: Hs,
             QUploader: Qs,
             QUploaderBase: Us,
             QUploaderAddTrigger: Gs,
             QVideo: Ks,
@@ -40580,17 +40580,17 @@
                             D.setAttribute("aria-hidden", "true"), !0 !== a.keepToClone && (D.style.left = 0, D.style.right = "unset", D.style.top = 0, D.style.bottom = "unset", D.style.transform = "none", D.style.pointerEvents = "none"), D.classList.add("q-morph--internal");
                             var z = e === o && d === r ? A : e.nextElementSibling;
                             r.insertBefore(D, z);
                             var N = cl(e, ["borderWidth", "borderStyle", "borderColor", "borderRadius", "backgroundColor", "transform", "position", "cssText"]),
                                 j = N.borderWidth,
                                 R = N.borderStyle,
                                 I = N.borderColor,
-                                F = N.borderRadius,
-                                $ = N.backgroundColor,
-                                B = N.transform,
+                                B = N.borderRadius,
+                                F = N.backgroundColor,
+                                $ = N.transform,
                                 V = N.position,
                                 H = N.cssText,
                                 U = e.classList.toString(),
                                 W = e.style.cssText;
                             e.style.cssText = H, e.style.transform = "none", e.style.animation = "none", e.style.transition = "none", e.className = U.split(" ").filter((function(e) {
                                 return !1 === /^bg-/.test(e)
                             })).join(" ");
@@ -40635,31 +40635,31 @@
                                         opacity: a.tweenToOpacity
                                     } : {
                                         backgroundColor: k
                                     },
                                     ge = void 0 !== P ? {
                                         opacity: 1
                                     } : {
-                                        backgroundColor: $
+                                        backgroundColor: F
                                     };
                                 u = e.animate([Object.assign({}, {
                                     margin: 0,
                                     borderWidth: _,
                                     borderStyle: b,
                                     borderColor: y,
                                     borderRadius: w,
                                     transformOrigin: "0 0"
                                 }, he, ve), Object.assign({}, {
                                     margin: 0,
                                     borderWidth: j,
                                     borderStyle: R,
                                     borderColor: I,
-                                    borderRadius: F,
+                                    borderRadius: B,
                                     transformOrigin: "0 0",
-                                    transform: B
+                                    transform: $
                                 }, fe, ge)], {
                                     duration: a.duration,
                                     easing: a.easing,
                                     fill: a.fill,
                                     delay: a.delay
                                 }), l = void 0 === P ? void 0 : P.animate([Object.assign({}, {
                                     opacity: a.tweenFromOpacity,
@@ -40672,15 +40672,15 @@
                                     transform: x
                                 }, pe), Object.assign({}, {
                                     opacity: 0,
                                     margin: 0,
                                     borderWidth: j,
                                     borderStyle: R,
                                     borderColor: I,
-                                    borderRadius: F,
+                                    borderRadius: B,
                                     transformOrigin: "0 0"
                                 }, me)], {
                                     duration: a.duration,
                                     easing: a.easing,
                                     fill: a.fill,
                                     delay: a.delay
                                 }), s = !0 === a.hideFromClone || !0 === oe ? void 0 : A.animate([{
@@ -40728,20 +40728,20 @@
                                 var be = "q-morph-anim-" + ++il,
                                     ye = document.createElement("style"),
                                     we = !0 === a.resize ? "\n            transform: translate(" + Q + "px, " + G + "px);\n            width: " + ne + "px;\n            height: " + ie + "px;\n          " : "transform: translate(" + Q + "px, " + G + "px) scale(" + K + ", " + Z + ");",
                                     ke = !0 === a.resize ? "\n            width: " + re + "px;\n            height: " + ae + "px;\n          " : "",
                                     xe = !0 === a.resize ? "\n            width: " + ne + "px;\n            height: " + ie + "px;\n          " : "",
                                     Se = !0 === a.resize ? "\n            transform: translate(" + -1 * Q + "px, " + -1 * G + "px);\n            width: " + re + "px;\n            height: " + ae + "px;\n          " : "transform: translate(" + -1 * Q + "px, " + -1 * G + "px) scale(" + 1 / K + ", " + 1 / Z + ");",
                                     Ce = void 0 !== P ? "opacity: " + a.tweenToOpacity + ";" : "background-color: " + k + ";",
-                                    Me = void 0 !== P ? "opacity: 1;" : "background-color: " + $ + ";",
-                                    Te = void 0 === P ? "" : "\n            @keyframes " + be + "-from-tween {\n              0% {\n                opacity: " + a.tweenFromOpacity + ";\n                margin: 0;\n                border-width: " + _ + ";\n                border-style: " + b + ";\n                border-color: " + y + ";\n                border-radius: " + w + ";\n                transform-origin: 0 0;\n                transform: " + x + ";\n                " + xe + "\n              }\n\n              100% {\n                opacity: 0;\n                margin: 0;\n                border-width: " + j + ";\n                border-style: " + R + ";\n                border-color: " + I + ";\n                border-radius: " + F + ";\n                transform-origin: 0 0;\n                " + Se + "\n              }\n            }\n          ",
+                                    Me = void 0 !== P ? "opacity: 1;" : "background-color: " + F + ";",
+                                    Te = void 0 === P ? "" : "\n            @keyframes " + be + "-from-tween {\n              0% {\n                opacity: " + a.tweenFromOpacity + ";\n                margin: 0;\n                border-width: " + _ + ";\n                border-style: " + b + ";\n                border-color: " + y + ";\n                border-radius: " + w + ";\n                transform-origin: 0 0;\n                transform: " + x + ";\n                " + xe + "\n              }\n\n              100% {\n                opacity: 0;\n                margin: 0;\n                border-width: " + j + ";\n                border-style: " + R + ";\n                border-color: " + I + ";\n                border-radius: " + B + ";\n                transform-origin: 0 0;\n                " + Se + "\n              }\n            }\n          ",
                                     Ae = !0 === a.hideFromClone || !0 === oe ? "" : "\n            @keyframes " + be + "-from {\n              0% {\n                margin: " + (X < 0 ? X / 2 : 0) + "px " + (J < 0 ? J / 2 : 0) + "px;\n                width: " + (ne + f.marginH) + "px;\n                height: " + (ie + f.marginV) + "px;\n              }\n\n              100% {\n                margin: 0;\n                width: 0;\n                height: 0;\n              }\n            }\n          ",
                                     Pe = !0 === oe ? "\n            margin: " + (X < 0 ? X / 2 : 0) + "px " + (J < 0 ? J / 2 : 0) + "px;\n            width: " + (ne + f.marginH) + "px;\n            height: " + (ie + f.marginV) + "px;\n          " : "\n            margin: 0;\n            width: 0;\n            height: 0;\n          ",
                                     Le = !0 === a.keepToClone ? "" : "\n            @keyframes " + be + "-to {\n              0% {\n                " + Pe + "\n              }\n\n              100% {\n                margin: " + (te < 0 ? te / 2 : 0) + "px " + (ee < 0 ? ee / 2 : 0) + "px;\n                width: " + (re + Y.marginH) + "px;\n                height: " + (ae + Y.marginV) + "px;\n              }\n            }\n          ";
-                                ye.innerHTML = "\n          @keyframes " + be + " {\n            0% {\n              margin: 0;\n              border-width: " + _ + ";\n              border-style: " + b + ";\n              border-color: " + y + ";\n              border-radius: " + w + ";\n              background-color: " + k + ";\n              transform-origin: 0 0;\n              " + we + "\n              " + Ce + "\n            }\n\n            100% {\n              margin: 0;\n              border-width: " + j + ";\n              border-style: " + R + ";\n              border-color: " + I + ";\n              border-radius: " + F + ";\n              background-color: " + $ + ";\n              transform-origin: 0 0;\n              transform: " + B + ";\n              " + ke + "\n              " + Me + "\n            }\n          }\n\n          " + Ae + "\n\n          " + Te + "\n\n          " + Le + "\n        ", document.head.appendChild(ye);
+                                ye.innerHTML = "\n          @keyframes " + be + " {\n            0% {\n              margin: 0;\n              border-width: " + _ + ";\n              border-style: " + b + ";\n              border-color: " + y + ";\n              border-radius: " + w + ";\n              background-color: " + k + ";\n              transform-origin: 0 0;\n              " + we + "\n              " + Ce + "\n            }\n\n            100% {\n              margin: 0;\n              border-width: " + j + ";\n              border-style: " + R + ";\n              border-color: " + I + ";\n              border-radius: " + B + ";\n              background-color: " + F + ";\n              transform-origin: 0 0;\n              transform: " + $ + ";\n              " + ke + "\n              " + Me + "\n            }\n          }\n\n          " + Ae + "\n\n          " + Te + "\n\n          " + Le + "\n        ", document.head.appendChild(ye);
                                 var qe = "normal";
                                 A.style.animation = a.duration + "ms " + a.easing + " " + a.delay + "ms " + qe + " " + a.fill + " " + be + "-from", void 0 !== P && (P.style.animation = a.duration + "ms " + a.easing + " " + a.delay + "ms " + qe + " " + a.fill + " " + be + "-from-tween"), D.style.animation = a.duration + "ms " + a.easing + " " + a.delay + "ms " + qe + " " + a.fill + " " + be + "-to", e.style.animation = a.duration + "ms " + a.easing + " " + a.delay + "ms " + qe + " " + a.fill + " " + be;
                                 var Oe = function(t) {
                                     t === Object(t) && t.animationName !== be || (e.removeEventListener("animationend", Oe), e.removeEventListener("animationcancel", Oe), de(), ye.remove())
                                 };
                                 o.qMorphCancel = function() {
                                     o.qMorphCancel = void 0, n = !0, Oe()
@@ -40965,15 +40965,15 @@
     var Ol = {
         name: "scroll",
         inserted: function(e, t) {
             void 0 !== e.__qscroll && (ql(e), e.__qscroll_destroyed = !0);
             var n = {
                 scrollTarget: jt(e),
                 scroll: function() {
-                    n.handler(It(n.scrollTarget), Ft(n.scrollTarget))
+                    n.handler(It(n.scrollTarget), Bt(n.scrollTarget))
                 }
             };
             Ll(n, t), e.__qscroll = n
         },
         update: function(e, t) {
             void 0 !== e.__qscroll && t.oldValue !== t.value && Ll(e.__qscroll, t)
         },
@@ -41177,47 +41177,47 @@
                     r = e.__qtouchrepeat;
                 void 0 !== r && n !== i && ("function" != typeof i && r.end(), r.handler = i)
             },
             unbind: function(e) {
                 void 0 === e.__qtouchrepeat_destroyed ? jl(e) : delete e.__qtouchrepeat_destroyed
             }
         },
-        Fl = Object.freeze({
+        Bl = Object.freeze({
             __proto__: null,
             ClosePopup: el,
             GoBack: nl,
-            Intersection: Ba,
+            Intersection: $a,
             Morph: kl,
             Mutation: Ml,
             Ripple: at,
             ScrollFire: Pl,
             Scroll: Ol,
             TouchHold: Dl,
             TouchPan: Gn,
             TouchRepeat: Il,
             TouchSwipe: vn
         });
 
-    function $l(e) {
+    function Fl(e) {
         void 0 === Rl && (Rl = h.is.winphone ? "msapplication-navbutton-color" : h.is.safari ? "apple-mobile-web-app-status-bar-style" : "theme-color");
         var t = function(e) {
                 var t = document.getElementsByTagName("META");
                 for (var n in t)
                     if (t[n].name === e) return t[n]
             }(Rl),
             n = void 0 === t;
         n && (t = document.createElement("meta")).setAttribute("name", Rl), t.setAttribute("content", e), n && document.head.appendChild(t)
     }
-    var Bl = {
+    var $l = {
             install: function(e) {
                 var t = e.$q,
                     n = e.cfg;
                 this.set = !1 !== i || !0 !== h.is.mobile || !0 !== h.is.nativeMobile && !0 !== h.is.winphone && !0 !== h.is.safari && !0 !== h.is.webkit && !0 !== h.is.vivaldi ? m : function(e) {
                     var t = e || Q("primary");
-                    !0 === h.is.nativeMobile && window.StatusBar ? window.StatusBar.backgroundColorByHexString(t) : $l(t)
+                    !0 === h.is.nativeMobile && window.StatusBar ? window.StatusBar.backgroundColorByHexString(t) : Fl(t)
                 }, t.addressbarColor = this, n.addressbarColor && this.set(n.addressbarColor)
             }
         },
         Vl = {};
 
     function Hl(e, t) {
         try {
@@ -42406,45 +42406,45 @@
                 t.clear()
             },
             isEmpty: function() {
                 return 0 === t.length
             }
         }
     }
-    var Fc = {
+    var Bc = {
             install: function(e) {
                 var t = e.$q,
                     n = !0 === i || !1 === d.has.webStorage ? Rc() : Ic("local");
                 t.localStorage = n, Object.assign(this, n)
             }
         },
-        $c = {
+        Fc = {
             install: function(e) {
                 var t = e.$q,
                     n = !0 === i || !1 === d.has.webStorage ? Rc() : Ic("session");
                 t.sessionStorage = n, Object.assign(this, n)
             }
         },
-        Bc = Object.freeze({
+        $c = Object.freeze({
             __proto__: null,
-            AddressbarColor: Bl,
+            AddressbarColor: $l,
             AppFullscreen: Ul,
             AppVisibility: Wl,
             BottomSheet: Kl,
             Cookies: lc,
             Dark: q,
             Dialog: uc,
             LoadingBar: dc,
             Loading: vc,
             Meta: Ac,
             Notify: jc,
             Platform: h,
             Screen: L,
-            LocalStorage: Fc,
-            SessionStorage: $c
+            LocalStorage: Bc,
+            SessionStorage: Fc
         });
 
     function Vc(e) {
         setTimeout((function() {
             window.URL.revokeObjectURL(e.href)
         }), 1e4), e.remove()
     }
@@ -42541,26 +42541,26 @@
                         "function" == typeof n.install && !1 === re.includes(n) && n.install(r)
                     }))
                 }
             }
         }
     }, {
         components: Zs,
-        directives: Fl,
-        plugins: Bc,
+        directives: Bl,
+        plugins: $c,
         config: window.quasarConfig || {}
     }), Object.assign({}, {
         version: n,
         lang: R,
         iconSet: ie,
         components: Zs,
-        directives: Fl,
-        plugins: Bc,
+        directives: Bl,
+        plugins: $c,
         utils: Uc
-    }, Zs, Fl, Bc, Uc)
+    }, Zs, Bl, $c, Uc)
 })),
 /*!
  * Chart.js v2.9.4
  * https://www.chartjs.org
  * (c) 2020 Chart.js Contributors
  * Released under the MIT License
  */
@@ -44049,32 +44049,32 @@
             },
             resolve: function(e, t, n, i) {
                 var r, a, o, s = !0;
                 for (r = 0, a = e.length; r < a; ++r)
                     if (void 0 !== (o = e[r]) && (void 0 !== t && "function" == typeof o && (o = o(t), s = !1), void 0 !== n && C.isArray(o) && (o = o[n], s = !1), void 0 !== o)) return i && !s && (i.cacheable = !1), o
             }
         },
-        F = {
+        B = {
             _factorize: function(e) {
                 var t, n = [],
                     i = Math.sqrt(e);
                 for (t = 1; t < i; t++) e % t == 0 && (n.push(t), n.push(e / t));
                 return i === (0 | i) && n.push(i), n.sort((function(e, t) {
                     return e - t
                 })).pop(), n
             },
             log10: Math.log10 || function(e) {
                 var t = Math.log(e) * Math.LOG10E,
                     n = Math.round(t);
                 return e === Math.pow(10, n) ? n : t
             }
         },
-        $ = F;
-    C.log10 = F.log10;
-    var B = {
+        F = B;
+    C.log10 = B.log10;
+    var $ = {
             getRtlAdapter: function(e, t, n) {
                 return e ? function(e, t) {
                     return {
                         x: function(n) {
                             return e + e + t - n
                         },
                         setWidth: function(e) {
@@ -44115,16 +44115,16 @@
                 void 0 !== t && (delete e.prevTextDirection, e.canvas.style.setProperty("direction", t[0], t[1]))
             }
         },
         V = C,
         H = T,
         U = z,
         W = I,
-        Y = $,
-        Q = B;
+        Y = F,
+        Q = $;
     V.easing = H, V.canvas = U, V.options = W, V.math = Y, V.rtl = Q;
     var G = function(e) {
         V.extend(this, e), this.initialize.apply(this, arguments)
     };
     V.extend(G.prototype, {
         _type: void 0,
         initialize: function() {
@@ -45280,24 +45280,24 @@
         datasets: {
             horizontalBar: {
                 categoryPercentage: .8,
                 barPercentage: .9
             }
         }
     });
-    var Fe = qe.extend({
+    var Be = qe.extend({
             _getValueScaleId: function() {
                 return this.getMeta().xAxisID
             },
             _getIndexScaleId: function() {
                 return this.getMeta().yAxisID
             }
         }),
-        $e = V.valueOrDefault,
-        Be = V.options.resolve,
+        Fe = V.valueOrDefault,
+        $e = V.options.resolve,
         Ve = V.canvas._isPointInArea;
 
     function He(e, t) {
         var n = e && e.options.ticks || {},
             i = n.reverse,
             r = void 0 === n.min ? t : 0,
             a = void 0 === n.max ? t : 0;
@@ -45343,15 +45343,15 @@
             update: function(e) {
                 var t, n, i = this,
                     r = i.getMeta(),
                     a = r.dataset,
                     o = r.data || [],
                     s = i.chart.options,
                     l = i._config,
-                    c = i._showLine = $e(l.showLine, s.showLines);
+                    c = i._showLine = Fe(l.showLine, s.showLines);
                 for (i._xScale = i.getScaleForId(r.xAxisID), i._yScale = i.getScaleForId(r.yAxisID), c && (void 0 !== l.tension && void 0 === l.lineTension && (l.lineTension = l.tension), a._scale = i._yScale, a._datasetIndex = i.index, a._children = o, a._model = i._resolveDatasetElementOptions(a), a.pivot()), t = 0, n = o.length; t < n; ++t) i.updateElement(o[t], t, e);
                 for (c && 0 !== a._model.tension && i.updateBezierControlPoints(), t = 0, n = o.length; t < n; ++t) o[t].pivot()
             },
             updateElement: function(e, t, n) {
                 var i, r, a = this,
                     o = a.getMeta(),
                     s = e.custom || {},
@@ -45368,27 +45368,27 @@
                     skip: s.skip || isNaN(i) || isNaN(r),
                     radius: p.radius,
                     pointStyle: p.pointStyle,
                     rotation: p.rotation,
                     backgroundColor: p.backgroundColor,
                     borderColor: p.borderColor,
                     borderWidth: p.borderWidth,
-                    tension: $e(s.tension, f ? f.tension : 0),
+                    tension: Fe(s.tension, f ? f.tension : 0),
                     steppedLine: !!f && f.steppedLine,
                     hitRadius: p.hitRadius
                 }
             },
             _resolveDatasetElementOptions: function(e) {
                 var t, n, i, r, a, o, s, l, c, u, d, h = this,
                     f = h._config,
                     p = e.custom || {},
                     m = h.chart.options,
                     v = m.elements.line,
                     g = re.prototype._resolveDatasetElementOptions.apply(h, arguments);
-                return g.spanGaps = $e(f.spanGaps, m.spanGaps), g.tension = $e(f.lineTension, v.tension), g.steppedLine = Be([p.steppedLine, f.steppedLine, v.stepped]), g.clip = (t = $e(f.clip, (o = h._xScale, s = h._yScale, l = g.borderWidth, u = He(o, c = l / 2), {
+                return g.spanGaps = Fe(f.spanGaps, m.spanGaps), g.tension = Fe(f.lineTension, v.tension), g.steppedLine = $e([p.steppedLine, f.steppedLine, v.stepped]), g.clip = (t = Fe(f.clip, (o = h._xScale, s = h._yScale, l = g.borderWidth, u = He(o, c = l / 2), {
                     top: (d = He(s, c)).end,
                     right: u.end,
                     bottom: d.start,
                     left: u.start
                 })), V.isObject(t) ? (n = t.top, i = t.right, r = t.bottom, a = t.left) : n = i = r = a = t, {
                     top: n,
                     right: i,
@@ -45446,15 +45446,15 @@
                     n = e._options,
                     i = V.getHoverColor;
                 e.$previousStyle = {
                     backgroundColor: t.backgroundColor,
                     borderColor: t.borderColor,
                     borderWidth: t.borderWidth,
                     radius: t.radius
-                }, t.backgroundColor = $e(n.hoverBackgroundColor, i(n.backgroundColor)), t.borderColor = $e(n.hoverBorderColor, i(n.borderColor)), t.borderWidth = $e(n.hoverBorderWidth, n.borderWidth), t.radius = $e(n.hoverRadius, n.radius)
+                }, t.backgroundColor = Fe(n.hoverBackgroundColor, i(n.backgroundColor)), t.borderColor = Fe(n.hoverBorderColor, i(n.borderColor)), t.borderWidth = Fe(n.hoverBorderWidth, n.borderWidth), t.radius = Fe(n.hoverRadius, n.radius)
             }
         }),
         We = V.options.resolve;
     j._set("polarArea", {
         scale: {
             type: "radialLinear",
             angleLines: {
@@ -45757,15 +45757,15 @@
             }
         }
     });
     var Ze = {
         bar: qe,
         bubble: De,
         doughnut: Ie,
-        horizontalBar: Fe,
+        horizontalBar: Be,
         line: Ue,
         polarArea: Ye,
         pie: Qe,
         radar: Ke,
         scatter: Ue
     };
 
@@ -46430,23 +46430,23 @@
             return {
                 x: a,
                 y: o
             }
         }
     };
 
-    function Ft(e, t) {
+    function Bt(e, t) {
         return t && (V.isArray(t) ? Array.prototype.push.apply(e, t) : e.push(t)), e
     }
 
-    function $t(e) {
+    function Ft(e) {
         return ("string" == typeof e || e instanceof String) && e.indexOf("\n") > -1 ? e.split("\n") : e
     }
 
-    function Bt(e) {
+    function $t(e) {
         var t = j.global;
         return {
             xPadding: e.xPadding,
             yPadding: e.yPadding,
             xAlign: e.xAlign,
             yAlign: e.yAlign,
             rtl: e.rtl,
@@ -46483,62 +46483,62 @@
     }
 
     function Vt(e, t) {
         return "center" === t ? e.x + e.width / 2 : "right" === t ? e.x + e.width - e.xPadding : e.x + e.xPadding
     }
 
     function Ht(e) {
-        return Ft([], $t(e))
+        return Bt([], Ft(e))
     }
     var Ut = K.extend({
             initialize: function() {
-                this._model = Bt(this._options), this._lastActive = []
+                this._model = $t(this._options), this._lastActive = []
             },
             getTitle: function() {
                 var e = this,
                     t = e._options.callbacks,
                     n = t.beforeTitle.apply(e, arguments),
                     i = t.title.apply(e, arguments),
                     r = t.afterTitle.apply(e, arguments),
                     a = [];
-                return a = Ft(a, $t(n)), a = Ft(a, $t(i)), a = Ft(a, $t(r))
+                return a = Bt(a, Ft(n)), a = Bt(a, Ft(i)), a = Bt(a, Ft(r))
             },
             getBeforeBody: function() {
                 return Ht(this._options.callbacks.beforeBody.apply(this, arguments))
             },
             getBody: function(e, t) {
                 var n = this,
                     i = n._options.callbacks,
                     r = [];
                 return V.each(e, (function(e) {
                     var a = {
                         before: [],
                         lines: [],
                         after: []
                     };
-                    Ft(a.before, $t(i.beforeLabel.call(n, e, t))), Ft(a.lines, i.label.call(n, e, t)), Ft(a.after, $t(i.afterLabel.call(n, e, t))), r.push(a)
+                    Bt(a.before, Ft(i.beforeLabel.call(n, e, t))), Bt(a.lines, i.label.call(n, e, t)), Bt(a.after, Ft(i.afterLabel.call(n, e, t))), r.push(a)
                 })), r
             },
             getAfterBody: function() {
                 return Ht(this._options.callbacks.afterBody.apply(this, arguments))
             },
             getFooter: function() {
                 var e = this,
                     t = e._options.callbacks,
                     n = t.beforeFooter.apply(e, arguments),
                     i = t.footer.apply(e, arguments),
                     r = t.afterFooter.apply(e, arguments),
                     a = [];
-                return a = Ft(a, $t(n)), a = Ft(a, $t(i)), a = Ft(a, $t(r))
+                return a = Bt(a, Ft(n)), a = Bt(a, Ft(i)), a = Bt(a, Ft(r))
             },
             update: function(e) {
                 var t, n, i, r, a, o, s, l, c, u, d = this,
                     h = d._options,
                     f = d._model,
-                    p = d._model = Bt(h),
+                    p = d._model = $t(h),
                     m = d._active,
                     v = d._data,
                     g = {
                         xAlign: f.xAlign,
                         yAlign: f.yAlign
                     },
                     _ = {
@@ -48109,16 +48109,16 @@
                 return 0 === n && 0 === t.min ? 0 : Math.pow(10, t._startValue + (n - t._valueOffset) * t._valueRange)
             }
         }),
         jn = Dn;
     Nn._defaults = jn;
     var Rn = V.valueOrDefault,
         In = V.valueAtIndexOrDefault,
-        Fn = V.options.resolve,
-        $n = {
+        Bn = V.options.resolve,
+        Fn = {
             display: !0,
             animate: !0,
             position: "chartArea",
             angleLines: {
                 display: !0,
                 color: "rgba(0,0,0,0.1)",
                 lineWidth: 1,
@@ -48140,15 +48140,15 @@
                 fontSize: 10,
                 callback: function(e) {
                     return e
                 }
             }
         };
 
-    function Bn(e) {
+    function $n(e) {
         var t = e.ticks;
         return t.display && e.display ? Rn(t.fontSize, j.global.defaultFontSize) + 2 * t.backdropPaddingY : 0
     }
 
     function Vn(e, t, n, i, r) {
         return e === i || e === r ? {
             start: t - n / 2,
@@ -48179,15 +48179,15 @@
 
     function Yn(e) {
         return V.isNumber(e) ? e : 0
     }
     var Qn = Mn.extend({
             setDimensions: function() {
                 var e = this;
-                e.width = e.maxWidth, e.height = e.maxHeight, e.paddingTop = Bn(e.options) / 2, e.xCenter = Math.floor(e.width / 2), e.yCenter = Math.floor((e.height - e.paddingTop) / 2), e.drawingArea = Math.min(e.height - e.paddingTop, e.width) / 2
+                e.width = e.maxWidth, e.height = e.maxHeight, e.paddingTop = $n(e.options) / 2, e.xCenter = Math.floor(e.width / 2), e.yCenter = Math.floor((e.height - e.paddingTop) / 2), e.drawingArea = Math.min(e.height - e.paddingTop, e.width) / 2
             },
             determineDataLimits: function() {
                 var e = this,
                     t = e.chart,
                     n = Number.POSITIVE_INFINITY,
                     i = Number.NEGATIVE_INFINITY;
                 V.each(t.data.datasets, (function(r, a) {
@@ -48197,15 +48197,15 @@
                             var a = +e.getRightValue(t);
                             isNaN(a) || o.data[r].hidden || (n = Math.min(a, n), i = Math.max(a, i))
                         }))
                     }
                 })), e.min = n === Number.POSITIVE_INFINITY ? 0 : n, e.max = i === Number.NEGATIVE_INFINITY ? 0 : i, e.handleTickRangeOptions()
             },
             _computeTickLimit: function() {
-                return Math.ceil(this.drawingArea / Bn(this.options))
+                return Math.ceil(this.drawingArea / $n(this.options))
             },
             convertTicksToLabels: function() {
                 var e = this;
                 Mn.prototype.convertTicksToLabels.call(e), e.pointLabels = e.chart.data.labels.map((function() {
                     var t = V.callback(e.options.pointLabels.callback, arguments, e);
                     return t || 0 === t ? t : ""
                 }))
@@ -48296,15 +48296,15 @@
                     s = a.angleLines,
                     l = Rn(s.lineWidth, o.lineWidth),
                     c = Rn(s.color, o.color);
                 if (a.pointLabels.display && function(e) {
                         var t = e.ctx,
                             n = e.options,
                             i = n.pointLabels,
-                            r = Bn(n),
+                            r = $n(n),
                             a = e.getDistanceFromCenterForValue(n.ticks.reverse ? e.min : e.max),
                             o = V.options._parseFont(i);
                         t.save(), t.font = o.string, t.textBaseline = "middle";
                         for (var s = e.chart.data.labels.length - 1; s >= 0; s--) {
                             var l = 0 === s ? r / 2 : 0,
                                 c = e.getPointPosition(s, a + l + 5),
                                 u = In(i.fontColor, s, j.global.defaultFontColor);
@@ -48327,15 +48327,15 @@
                                     r = e.getPointPosition(0, n), a.moveTo(r.x, r.y);
                                     for (var u = 1; u < s; u++) r = e.getPointPosition(u, n), a.lineTo(r.x, r.y)
                                 }
                                 a.closePath(), a.stroke(), a.restore()
                             }
                         }(i, o, t, n))
                     })), s.display && l && c) {
-                    for (r.save(), r.lineWidth = l, r.strokeStyle = c, r.setLineDash && (r.setLineDash(Fn([s.borderDash, o.borderDash, []])), r.lineDashOffset = Fn([s.borderDashOffset, o.borderDashOffset, 0])), e = i.chart.data.labels.length - 1; e >= 0; e--) t = i.getDistanceFromCenterForValue(a.ticks.reverse ? i.min : i.max), n = i.getPointPosition(e, t), r.beginPath(), r.moveTo(i.xCenter, i.yCenter), r.lineTo(n.x, n.y), r.stroke();
+                    for (r.save(), r.lineWidth = l, r.strokeStyle = c, r.setLineDash && (r.setLineDash(Bn([s.borderDash, o.borderDash, []])), r.lineDashOffset = Bn([s.borderDashOffset, o.borderDashOffset, 0])), e = i.chart.data.labels.length - 1; e >= 0; e--) t = i.getDistanceFromCenterForValue(a.ticks.reverse ? i.min : i.max), n = i.getPointPosition(e, t), r.beginPath(), r.moveTo(i.xCenter, i.yCenter), r.lineTo(n.x, n.y), r.stroke();
                     r.restore()
                 }
             },
             _drawLabels: function() {
                 var e = this,
                     t = e.ctx,
                     n = e.options.ticks;
@@ -48346,15 +48346,15 @@
                     t.save(), t.font = o.string, t.translate(e.xCenter, e.yCenter), t.rotate(a), t.textAlign = "center", t.textBaseline = "middle", V.each(e.ticks, (function(a, l) {
                         (0 !== l || n.reverse) && (i = e.getDistanceFromCenterForValue(e.ticksAsNumbers[l]), n.showLabelBackdrop && (r = t.measureText(a).width, t.fillStyle = n.backdropColor, t.fillRect(-r / 2 - n.backdropPaddingX, -i - o.size / 2 - n.backdropPaddingY, r + 2 * n.backdropPaddingX, o.size + 2 * n.backdropPaddingY)), t.fillStyle = s, t.fillText(a, 0, -i))
                     })), t.restore()
                 }
             },
             _drawTitle: V.noop
         }),
-        Gn = $n;
+        Gn = Fn;
     Qn._defaults = Gn;
     var Kn = V._deprecated,
         Zn = V.options.resolve,
         Jn = V.valueOrDefault,
         Xn = Number.MIN_SAFE_INTEGER || -9007199254740991,
         ei = Number.MAX_SAFE_INTEGER || 9007199254740991,
         ti = {
@@ -48906,24 +48906,24 @@
                     LT: "h:mm A",
                     L: "MM/DD/YYYY",
                     LL: "MMMM D, YYYY",
                     LLL: "MMMM D, YYYY h:mm A",
                     LLLL: "dddd, MMMM D, YYYY h:mm A"
                 };
 
-                function F(e) {
+                function B(e) {
                     var t = this._longDateFormat[e],
                         n = this._longDateFormat[e.toUpperCase()];
                     return t || !n ? t : (this._longDateFormat[e] = n.replace(/MMMM|MM|DD|dddd/g, (function(e) {
                         return e.slice(1)
                     })), this._longDateFormat[e])
                 }
-                var $ = "Invalid date";
+                var F = "Invalid date";
 
-                function B() {
+                function $() {
                     return this._invalidDate
                 }
                 var V = "%d",
                     H = /\d{1,2}/;
 
                 function U(e) {
                     return this._ordinal.replace("%d", e)
@@ -49089,17 +49089,17 @@
                 }
 
                 function je(e, t, n) {
                     null != t && f(De, e) && De[e](t, n._a, n, e)
                 }
                 var Re = 0,
                     Ie = 1,
-                    Fe = 2,
-                    $e = 3,
-                    Be = 4,
+                    Be = 2,
+                    Fe = 3,
+                    $e = 4,
                     Ve = 5,
                     He = 6,
                     Ue = 7,
                     We = 8;
 
                 function Ye(e) {
                     return Qe(e) ? 366 : 365
@@ -49361,28 +49361,28 @@
                 var jt = "Sun_Mon_Tue_Wed_Thu_Fri_Sat".split("_");
 
                 function Rt(e) {
                     return !0 === e ? Dt(this._weekdaysShort, this._week.dow) : e ? this._weekdaysShort[e.day()] : this._weekdaysShort
                 }
                 var It = "Su_Mo_Tu_We_Th_Fr_Sa".split("_");
 
-                function Ft(e) {
+                function Bt(e) {
                     return !0 === e ? Dt(this._weekdaysMin, this._week.dow) : e ? this._weekdaysMin[e.day()] : this._weekdaysMin
                 }
 
-                function $t(e, t, n) {
+                function Ft(e, t, n) {
                     var i, r, a, o = e.toLocaleLowerCase();
                     if (!this._weekdaysParse)
                         for (this._weekdaysParse = [], this._shortWeekdaysParse = [], this._minWeekdaysParse = [], i = 0; i < 7; ++i) a = m([2e3, 1]).day(i), this._minWeekdaysParse[i] = this.weekdaysMin(a, "").toLocaleLowerCase(), this._shortWeekdaysParse[i] = this.weekdaysShort(a, "").toLocaleLowerCase(), this._weekdaysParse[i] = this.weekdays(a, "").toLocaleLowerCase();
                     return n ? "dddd" === t ? -1 !== (r = Ge.call(this._weekdaysParse, o)) ? r : null : "ddd" === t ? -1 !== (r = Ge.call(this._shortWeekdaysParse, o)) ? r : null : -1 !== (r = Ge.call(this._minWeekdaysParse, o)) ? r : null : "dddd" === t ? -1 !== (r = Ge.call(this._weekdaysParse, o)) || -1 !== (r = Ge.call(this._shortWeekdaysParse, o)) || -1 !== (r = Ge.call(this._minWeekdaysParse, o)) ? r : null : "ddd" === t ? -1 !== (r = Ge.call(this._shortWeekdaysParse, o)) || -1 !== (r = Ge.call(this._weekdaysParse, o)) || -1 !== (r = Ge.call(this._minWeekdaysParse, o)) ? r : null : -1 !== (r = Ge.call(this._minWeekdaysParse, o)) || -1 !== (r = Ge.call(this._weekdaysParse, o)) || -1 !== (r = Ge.call(this._shortWeekdaysParse, o)) ? r : null
                 }
 
-                function Bt(e, t, n) {
+                function $t(e, t, n) {
                     var i, r, a;
-                    if (this._weekdaysParseExact) return $t.call(this, e, t, n);
+                    if (this._weekdaysParseExact) return Ft.call(this, e, t, n);
                     for (this._weekdaysParse || (this._weekdaysParse = [], this._minWeekdaysParse = [], this._shortWeekdaysParse = [], this._fullWeekdaysParse = []), i = 0; i < 7; i++) {
                         if (r = m([2e3, 1]).day(i), n && !this._fullWeekdaysParse[i] && (this._fullWeekdaysParse[i] = new RegExp("^" + this.weekdays(r, "").replace(".", "\\.?") + "$", "i"), this._shortWeekdaysParse[i] = new RegExp("^" + this.weekdaysShort(r, "").replace(".", "\\.?") + "$", "i"), this._minWeekdaysParse[i] = new RegExp("^" + this.weekdaysMin(r, "").replace(".", "\\.?") + "$", "i")), this._weekdaysParse[i] || (a = "^" + this.weekdays(r, "") + "|^" + this.weekdaysShort(r, "") + "|^" + this.weekdaysMin(r, ""), this._weekdaysParse[i] = new RegExp(a.replace(".", ""), "i")), n && "dddd" === t && this._fullWeekdaysParse[i].test(e)) return i;
                         if (n && "ddd" === t && this._shortWeekdaysParse[i].test(e)) return i;
                         if (n && "dd" === t && this._minWeekdaysParse[i].test(e)) return i;
                         if (!n && this._weekdaysParse[i].test(e)) return i
                     }
                 }
@@ -49461,46 +49461,46 @@
                     return "" + Xt.apply(this) + ne(this.minutes(), 2)
                 })), se("hmmss", 0, 0, (function() {
                     return "" + Xt.apply(this) + ne(this.minutes(), 2) + ne(this.seconds(), 2)
                 })), se("Hmm", 0, 0, (function() {
                     return "" + this.hours() + ne(this.minutes(), 2)
                 })), se("Hmmss", 0, 0, (function() {
                     return "" + this.hours() + ne(this.minutes(), 2) + ne(this.seconds(), 2)
-                })), tn("a", !0), tn("A", !1), K("hour", "h"), ee("hour", 13), Le("a", nn), Le("A", nn), Le("H", ge), Le("h", ge), Le("k", ge), Le("HH", ge, fe), Le("hh", ge, fe), Le("kk", ge, fe), Le("hmm", _e), Le("hmmss", be), Le("Hmm", _e), Le("Hmmss", be), ze(["H", "HH"], $e), ze(["k", "kk"], (function(e, t, n) {
+                })), tn("a", !0), tn("A", !1), K("hour", "h"), ee("hour", 13), Le("a", nn), Le("A", nn), Le("H", ge), Le("h", ge), Le("k", ge), Le("HH", ge, fe), Le("hh", ge, fe), Le("kk", ge, fe), Le("hmm", _e), Le("hmmss", be), Le("Hmm", _e), Le("Hmmss", be), ze(["H", "HH"], Fe), ze(["k", "kk"], (function(e, t, n) {
                     var i = M(e);
-                    t[$e] = 24 === i ? 0 : i
+                    t[Fe] = 24 === i ? 0 : i
                 })), ze(["a", "A"], (function(e, t, n) {
                     n._isPm = n._locale.isPM(e), n._meridiem = e
                 })), ze(["h", "hh"], (function(e, t, n) {
-                    t[$e] = M(e), g(n).bigHour = !0
+                    t[Fe] = M(e), g(n).bigHour = !0
                 })), ze("hmm", (function(e, t, n) {
                     var i = e.length - 2;
-                    t[$e] = M(e.substr(0, i)), t[Be] = M(e.substr(i)), g(n).bigHour = !0
+                    t[Fe] = M(e.substr(0, i)), t[$e] = M(e.substr(i)), g(n).bigHour = !0
                 })), ze("hmmss", (function(e, t, n) {
                     var i = e.length - 4,
                         r = e.length - 2;
-                    t[$e] = M(e.substr(0, i)), t[Be] = M(e.substr(i, 2)), t[Ve] = M(e.substr(r)), g(n).bigHour = !0
+                    t[Fe] = M(e.substr(0, i)), t[$e] = M(e.substr(i, 2)), t[Ve] = M(e.substr(r)), g(n).bigHour = !0
                 })), ze("Hmm", (function(e, t, n) {
                     var i = e.length - 2;
-                    t[$e] = M(e.substr(0, i)), t[Be] = M(e.substr(i))
+                    t[Fe] = M(e.substr(0, i)), t[$e] = M(e.substr(i))
                 })), ze("Hmmss", (function(e, t, n) {
                     var i = e.length - 4,
                         r = e.length - 2;
-                    t[$e] = M(e.substr(0, i)), t[Be] = M(e.substr(i, 2)), t[Ve] = M(e.substr(r))
+                    t[Fe] = M(e.substr(0, i)), t[$e] = M(e.substr(i, 2)), t[Ve] = M(e.substr(r))
                 }));
                 var an = /[ap]\.?m?\.?/i;
 
                 function on(e, t, n) {
                     return e > 11 ? n ? "pm" : "PM" : n ? "am" : "AM"
                 }
                 var sn, ln = Je("Hours", !0),
                     cn = {
                         calendar: j,
                         longDateFormat: I,
-                        invalidDate: $,
+                        invalidDate: F,
                         ordinal: V,
                         dayOfMonthOrdinalParse: H,
                         relativeTime: W,
                         months: ot,
                         monthsShort: lt,
                         week: Tt,
                         weekdays: zt,
@@ -49579,32 +49579,32 @@
 
                 function bn() {
                     return L(un)
                 }
 
                 function yn(e) {
                     var t, n = e._a;
-                    return n && -2 === g(e).overflow && (t = n[Ie] < 0 || n[Ie] > 11 ? Ie : n[Fe] < 1 || n[Fe] > rt(n[Re], n[Ie]) ? Fe : n[$e] < 0 || n[$e] > 24 || 24 === n[$e] && (0 !== n[Be] || 0 !== n[Ve] || 0 !== n[He]) ? $e : n[Be] < 0 || n[Be] > 59 ? Be : n[Ve] < 0 || n[Ve] > 59 ? Ve : n[He] < 0 || n[He] > 999 ? He : -1, g(e)._overflowDayOfYear && (t < Re || t > Fe) && (t = Fe), g(e)._overflowWeeks && -1 === t && (t = Ue), g(e)._overflowWeekday && -1 === t && (t = We), g(e).overflow = t), e
+                    return n && -2 === g(e).overflow && (t = n[Ie] < 0 || n[Ie] > 11 ? Ie : n[Be] < 1 || n[Be] > rt(n[Re], n[Ie]) ? Be : n[Fe] < 0 || n[Fe] > 24 || 24 === n[Fe] && (0 !== n[$e] || 0 !== n[Ve] || 0 !== n[He]) ? Fe : n[$e] < 0 || n[$e] > 59 ? $e : n[Ve] < 0 || n[Ve] > 59 ? Ve : n[He] < 0 || n[He] > 999 ? He : -1, g(e)._overflowDayOfYear && (t < Re || t > Be) && (t = Be), g(e)._overflowWeeks && -1 === t && (t = Ue), g(e)._overflowWeekday && -1 === t && (t = We), g(e).overflow = t), e
                 }
 
                 function wn(e, t, n) {
                     return null != e ? e : null != t ? t : n
                 }
 
                 function kn(e) {
                     var t = new Date(r.now());
                     return e._useUTC ? [t.getUTCFullYear(), t.getUTCMonth(), t.getUTCDate()] : [t.getFullYear(), t.getMonth(), t.getDate()]
                 }
 
                 function xn(e) {
                     var t, n, i, r, a, o = [];
                     if (!e._d) {
-                        for (i = kn(e), e._w && null == e._a[Fe] && null == e._a[Ie] && Sn(e), null != e._dayOfYear && (a = wn(e._a[Re], i[Re]), (e._dayOfYear > Ye(a) || 0 === e._dayOfYear) && (g(e)._overflowDayOfYear = !0), n = wt(a, 0, e._dayOfYear), e._a[Ie] = n.getUTCMonth(), e._a[Fe] = n.getUTCDate()), t = 0; t < 3 && null == e._a[t]; ++t) e._a[t] = o[t] = i[t];
+                        for (i = kn(e), e._w && null == e._a[Be] && null == e._a[Ie] && Sn(e), null != e._dayOfYear && (a = wn(e._a[Re], i[Re]), (e._dayOfYear > Ye(a) || 0 === e._dayOfYear) && (g(e)._overflowDayOfYear = !0), n = wt(a, 0, e._dayOfYear), e._a[Ie] = n.getUTCMonth(), e._a[Be] = n.getUTCDate()), t = 0; t < 3 && null == e._a[t]; ++t) e._a[t] = o[t] = i[t];
                         for (; t < 7; t++) e._a[t] = o[t] = null == e._a[t] ? 2 === t ? 1 : 0 : e._a[t];
-                        24 === e._a[$e] && 0 === e._a[Be] && 0 === e._a[Ve] && 0 === e._a[He] && (e._nextDay = !0, e._a[$e] = 0), e._d = (e._useUTC ? wt : yt).apply(null, o), r = e._useUTC ? e._d.getUTCDay() : e._d.getDay(), null != e._tzm && e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), e._nextDay && (e._a[$e] = 24), e._w && void 0 !== e._w.d && e._w.d !== r && (g(e).weekdayMismatch = !0)
+                        24 === e._a[Fe] && 0 === e._a[$e] && 0 === e._a[Ve] && 0 === e._a[He] && (e._nextDay = !0, e._a[Fe] = 0), e._d = (e._useUTC ? wt : yt).apply(null, o), r = e._useUTC ? e._d.getUTCDay() : e._d.getDay(), null != e._tzm && e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), e._nextDay && (e._a[Fe] = 24), e._w && void 0 !== e._w.d && e._w.d !== r && (g(e).weekdayMismatch = !0)
                     }
                 }
 
                 function Sn(e) {
                     var t, n, i, r, a, o, s, l;
                     if (null != (t = e._w).GG || null != t.W || null != t.E) a = 1, o = 4, n = wn(t.GG, e._a[Re], St(Gn(), 1, 4).year), i = wn(t.W, 1), ((r = wn(t.E, 1)) < 1 || r > 7) && (l = !0);
                     else {
@@ -49660,15 +49660,15 @@
                                 } if (null == a) return void(e._isValid = !1)
                         }
                         if (!i && null != a) return void(e._isValid = !1);
                         if (l[4]) {
                             if (!Tn.exec(l[4])) return void(e._isValid = !1);
                             o = "Z"
                         }
-                        e._f = r + (a || "") + (o || ""), $n(e)
+                        e._f = r + (a || "") + (o || ""), Fn(e)
                     } else e._isValid = !1
                 }
                 var On = /^(?:(Mon|Tue|Wed|Thu|Fri|Sat|Sun),?\s)?(\d{1,2})\s(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s(\d{2,4})\s(\d\d):(\d\d)(?::(\d\d))?\s(?:(UT|GMT|[ECMP][SD]T)|([Zz])|([+-]\d{4}))$/;
 
                 function En(e, t, n, i, r, a) {
                     var o = [Dn(e), lt.indexOf(t), parseInt(n, 10), parseInt(i, 10), parseInt(r, 10)];
                     return a && o.push(parseInt(a, 10)), o
@@ -49712,41 +49712,41 @@
                     if (t) {
                         var n = En(t[4], t[3], t[2], t[5], t[6], t[7]);
                         if (!Nn(t[1], n, e)) return;
                         e._a = n, e._tzm = Rn(t[8], t[9], t[10]), e._d = wt.apply(null, e._a), e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), g(e).rfc2822 = !0
                     } else e._isValid = !1
                 }
 
-                function Fn(e) {
+                function Bn(e) {
                     var t = Ln.exec(e._i);
                     null === t ? (qn(e), !1 === e._isValid && (delete e._isValid, In(e), !1 === e._isValid && (delete e._isValid, r.createFromInputFallback(e)))) : e._d = new Date(+t[1])
                 }
 
-                function $n(e) {
+                function Fn(e) {
                     if (e._f !== r.ISO_8601)
                         if (e._f !== r.RFC_2822) {
                             e._a = [], g(e).empty = !0;
                             var t, n, i, a, o, s = "" + e._i,
                                 l = s.length,
                                 c = 0;
                             for (i = de(e._f, e._locale).match(ie) || [], t = 0; t < i.length; t++) a = i[t], (n = (s.match(qe(a, e)) || [])[0]) && ((o = s.substr(0, s.indexOf(n))).length > 0 && g(e).unusedInput.push(o), s = s.slice(s.indexOf(n) + n.length), c += n.length), oe[a] ? (n ? g(e).empty = !1 : g(e).unusedTokens.push(a), je(a, n, e)) : e._strict && !n && g(e).unusedTokens.push(a);
-                            g(e).charsLeftOver = l - c, s.length > 0 && g(e).unusedInput.push(s), e._a[$e] <= 12 && !0 === g(e).bigHour && e._a[$e] > 0 && (g(e).bigHour = void 0), g(e).parsedDateParts = e._a.slice(0), g(e).meridiem = e._meridiem, e._a[$e] = Bn(e._locale, e._a[$e], e._meridiem), xn(e), yn(e)
+                            g(e).charsLeftOver = l - c, s.length > 0 && g(e).unusedInput.push(s), e._a[Fe] <= 12 && !0 === g(e).bigHour && e._a[Fe] > 0 && (g(e).bigHour = void 0), g(e).parsedDateParts = e._a.slice(0), g(e).meridiem = e._meridiem, e._a[Fe] = $n(e._locale, e._a[Fe], e._meridiem), xn(e), yn(e)
                         } else In(e);
                     else qn(e)
                 }
 
-                function Bn(e, t, n) {
+                function $n(e, t, n) {
                     var i;
                     return null == n ? t : null != e.meridiemHour ? e.meridiemHour(t, n) : null != e.isPM ? ((i = e.isPM(n)) && t < 12 && (t += 12), i || 12 !== t || (t = 0), t) : t
                 }
 
                 function Vn(e) {
                     var t, n, i, r, a;
                     if (0 === e._f.length) return g(e).invalidFormat = !0, void(e._d = new Date(NaN));
-                    for (r = 0; r < e._f.length; r++) a = 0, t = w({}, e), null != e._useUTC && (t._useUTC = e._useUTC), t._f = e._f[r], $n(t), _(t) && (a += g(t).charsLeftOver, a += 10 * g(t).unusedTokens.length, g(t).score = a, (null == i || a < i) && (i = a, n = t));
+                    for (r = 0; r < e._f.length; r++) a = 0, t = w({}, e), null != e._useUTC && (t._useUTC = e._useUTC), t._f = e._f[r], Fn(t), _(t) && (a += g(t).charsLeftOver, a += 10 * g(t).unusedTokens.length, g(t).score = a, (null == i || a < i) && (i = a, n = t));
                     p(e, n || t)
                 }
 
                 function Hn(e) {
                     if (!e._d) {
                         var t = J(e._i);
                         e._a = h([t.year, t.month, t.day || t.date, t.hour, t.minute, t.second, t.millisecond], (function(e) {
@@ -49761,20 +49761,20 @@
                 }
 
                 function Wn(e) {
                     var t = e._i,
                         n = e._f;
                     return e._locale = e._locale || _n(e._l), null === t || void 0 === n && "" === t ? b({
                         nullInput: !0
-                    }) : ("string" == typeof t && (e._i = t = e._locale.preparse(t)), S(t) ? new x(yn(t)) : (d(t) ? e._d = t : o(n) ? Vn(e) : n ? $n(e) : Yn(e), _(e) || (e._d = null), e))
+                    }) : ("string" == typeof t && (e._i = t = e._locale.preparse(t)), S(t) ? new x(yn(t)) : (d(t) ? e._d = t : o(n) ? Vn(e) : n ? Fn(e) : Yn(e), _(e) || (e._d = null), e))
                 }
 
                 function Yn(e) {
                     var t = e._i;
-                    c(t) ? e._d = new Date(r.now()) : d(t) ? e._d = new Date(t.valueOf()) : "string" == typeof t ? Fn(e) : o(t) ? (e._a = h(t.slice(0), (function(e) {
+                    c(t) ? e._d = new Date(r.now()) : d(t) ? e._d = new Date(t.valueOf()) : "string" == typeof t ? Bn(e) : o(t) ? (e._a = h(t.slice(0), (function(e) {
                         return parseInt(e, 10)
                     })), xn(e)) : s(t) ? Hn(e) : u(t) ? e._d = new Date(t) : r.createFromInputFallback(e)
                 }
 
                 function Qn(e, t, n, i, r) {
                     var a = {};
                     return !0 !== n && !1 !== n || (i = n, n = void 0), (s(e) && l(e) || o(e) && 0 === e.length) && (e = void 0), a._isAMomentObject = !0, a._useUTC = a._isUTC = r, a._l = n, a._i = e, a._f = t, a._strict = i, Un(a)
@@ -49954,17 +49954,17 @@
                         o = null;
                     return si(e) ? a = {
                         ms: e._milliseconds,
                         d: e._days,
                         M: e._months
                     } : u(e) ? (a = {}, t ? a[t] = e : a.milliseconds = e) : (o = Ci.exec(e)) ? (n = "-" === o[1] ? -1 : 1, a = {
                         y: 0,
-                        d: M(o[Fe]) * n,
-                        h: M(o[$e]) * n,
-                        m: M(o[Be]) * n,
+                        d: M(o[Be]) * n,
+                        h: M(o[Fe]) * n,
+                        m: M(o[$e]) * n,
                         s: M(o[Ve]) * n,
                         ms: M(li(1e3 * o[He])) * n
                     }) : (o = Mi.exec(e)) ? (n = "-" === o[1] ? -1 : 1, a = {
                         y: Ai(o[2], n),
                         M: Ai(o[3], n),
                         w: Ai(o[4], n),
                         d: Ai(o[5], n),
@@ -50032,26 +50032,26 @@
                 }
 
                 function Ii(e, t) {
                     var n = S(e) ? e : Gn(e);
                     return !(!this.isValid() || !n.isValid()) && ("millisecond" === (t = Z(t) || "millisecond") ? this.valueOf() < n.valueOf() : this.clone().endOf(t).valueOf() < n.valueOf())
                 }
 
-                function Fi(e, t, n, i) {
+                function Bi(e, t, n, i) {
                     var r = S(e) ? e : Gn(e),
                         a = S(t) ? t : Gn(t);
                     return !!(this.isValid() && r.isValid() && a.isValid()) && ("(" === (i = i || "()")[0] ? this.isAfter(r, n) : !this.isBefore(r, n)) && (")" === i[1] ? this.isBefore(a, n) : !this.isAfter(a, n))
                 }
 
-                function $i(e, t) {
+                function Fi(e, t) {
                     var n, i = S(e) ? e : Gn(e);
                     return !(!this.isValid() || !i.isValid()) && ("millisecond" === (t = Z(t) || "millisecond") ? this.valueOf() === i.valueOf() : (n = i.valueOf(), this.clone().startOf(t).valueOf() <= n && n <= this.clone().endOf(t).valueOf()))
                 }
 
-                function Bi(e, t) {
+                function $i(e, t) {
                     return this.isSame(e, t) || this.isAfter(e, t)
                 }
 
                 function Vi(e, t) {
                     return this.isSame(e, t) || this.isBefore(e, t)
                 }
 
@@ -50347,26 +50347,26 @@
                     t[i.substr(0, 2)] = M(e)
                 })), Ne(["gg", "GG"], (function(e, t, n, i) {
                     t[i] = r.parseTwoDigitYear(e)
                 })), se("Q", 0, "Qo", "quarter"), K("quarter", "Q"), ee("quarter", 7), Le("Q", he), ze("Q", (function(e, t) {
                     t[Ie] = 3 * (M(e) - 1)
                 })), se("D", ["DD", 2], "Do", "date"), K("date", "D"), ee("date", 9), Le("D", ge), Le("DD", ge, fe), Le("Do", (function(e, t) {
                     return e ? t._dayOfMonthOrdinalParse || t._ordinalParse : t._dayOfMonthOrdinalParseLenient
-                })), ze(["D", "DD"], Fe), ze("Do", (function(e, t) {
-                    t[Fe] = M(e.match(ge)[0])
+                })), ze(["D", "DD"], Be), ze("Do", (function(e, t) {
+                    t[Be] = M(e.match(ge)[0])
                 }));
                 var Lr = Je("Date", !0);
 
                 function qr(e) {
                     var t = Math.round((this.clone().startOf("day") - this.clone().startOf("year")) / 864e5) + 1;
                     return null == e ? t : this.add(e - t, "d")
                 }
                 se("DDD", ["DDDD", 3], "DDDo", "dayOfYear"), K("dayOfYear", "DDD"), ee("dayOfYear", 4), Le("DDD", ye), Le("DDDD", pe), ze(["DDD", "DDDD"], (function(e, t, n) {
                     n._dayOfYear = M(e)
-                })), se("m", ["mm", 2], 0, "minute"), K("minute", "m"), ee("minute", 14), Le("m", ge), Le("mm", ge, fe), ze(["m", "mm"], Be);
+                })), se("m", ["mm", 2], 0, "minute"), K("minute", "m"), ee("minute", 14), Le("m", ge), Le("mm", ge, fe), ze(["m", "mm"], $e);
                 var Or = Je("Minutes", !1);
                 se("s", ["ss", 2], 0, "second"), K("second", "s"), ee("second", 15), Le("s", ge), Le("ss", ge, fe), ze(["s", "ss"], Ve);
                 var Er, Dr = Je("Seconds", !1);
                 for (se("S", 0, 0, (function() {
                         return ~~(this.millisecond() / 100)
                     })), se(0, ["SS", 2], 0, (function() {
                         return ~~(this.millisecond() / 10)
@@ -50396,26 +50396,26 @@
 
                 function Rr() {
                     return this._isUTC ? "Coordinated Universal Time" : ""
                 }
                 se("z", 0, 0, "zoneAbbr"), se("zz", 0, 0, "zoneName");
                 var Ir = x.prototype;
 
-                function Fr(e) {
+                function Br(e) {
                     return Gn(1e3 * e)
                 }
 
-                function $r() {
+                function Fr() {
                     return Gn.apply(null, arguments).parseZone()
                 }
 
-                function Br(e) {
+                function $r(e) {
                     return e
                 }
-                Ir.add = Ei, Ir.calendar = Ni, Ir.clone = ji, Ir.diff = Hi, Ir.endOf = dr, Ir.format = Gi, Ir.from = Ki, Ir.fromNow = Zi, Ir.to = Ji, Ir.toNow = Xi, Ir.get = tt, Ir.invalidAt = yr, Ir.isAfter = Ri, Ir.isBefore = Ii, Ir.isBetween = Fi, Ir.isSame = $i, Ir.isSameOrAfter = Bi, Ir.isSameOrBefore = Vi, Ir.isValid = _r, Ir.lang = tr, Ir.locale = er, Ir.localeData = nr, Ir.max = Zn, Ir.min = Kn, Ir.parsingFlags = br, Ir.set = nt, Ir.startOf = ur, Ir.subtract = Di, Ir.toArray = mr, Ir.toObject = vr, Ir.toDate = pr, Ir.toISOString = Yi, Ir.inspect = Qi, Ir.toJSON = gr, Ir.toString = Wi, Ir.unix = fr, Ir.valueOf = hr, Ir.creationData = wr, Ir.year = Ke, Ir.isLeapYear = Ze, Ir.weekYear = xr, Ir.isoWeekYear = Sr, Ir.quarter = Ir.quarters = Pr, Ir.month = ft, Ir.daysInMonth = pt, Ir.week = Ir.weeks = Lt, Ir.isoWeek = Ir.isoWeeks = qt, Ir.weeksInYear = Mr, Ir.isoWeeksInYear = Cr, Ir.date = Lr, Ir.day = Ir.days = Vt, Ir.weekday = Ht, Ir.isoWeekday = Ut, Ir.dayOfYear = qr, Ir.hour = Ir.hours = ln, Ir.minute = Ir.minutes = Or, Ir.second = Ir.seconds = Dr, Ir.millisecond = Ir.milliseconds = Nr, Ir.utcOffset = pi, Ir.utc = vi, Ir.local = gi, Ir.parseZone = _i, Ir.hasAlignedHourOffset = bi, Ir.isDST = yi, Ir.isLocal = ki, Ir.isUtcOffset = xi, Ir.isUtc = Si, Ir.isUTC = Si, Ir.zoneAbbr = jr, Ir.zoneName = Rr, Ir.dates = P("dates accessor is deprecated. Use date instead.", Lr), Ir.months = P("months accessor is deprecated. Use month instead", ft), Ir.years = P("years accessor is deprecated. Use year instead", Ke), Ir.zone = P("moment().zone is deprecated, use moment().utcOffset instead. http://momentjs.com/guides/#/warnings/zone/", mi), Ir.isDSTShifted = P("isDSTShifted is deprecated. See http://momentjs.com/guides/#/warnings/dst-shifted/ for more information", wi);
+                Ir.add = Ei, Ir.calendar = Ni, Ir.clone = ji, Ir.diff = Hi, Ir.endOf = dr, Ir.format = Gi, Ir.from = Ki, Ir.fromNow = Zi, Ir.to = Ji, Ir.toNow = Xi, Ir.get = tt, Ir.invalidAt = yr, Ir.isAfter = Ri, Ir.isBefore = Ii, Ir.isBetween = Bi, Ir.isSame = Fi, Ir.isSameOrAfter = $i, Ir.isSameOrBefore = Vi, Ir.isValid = _r, Ir.lang = tr, Ir.locale = er, Ir.localeData = nr, Ir.max = Zn, Ir.min = Kn, Ir.parsingFlags = br, Ir.set = nt, Ir.startOf = ur, Ir.subtract = Di, Ir.toArray = mr, Ir.toObject = vr, Ir.toDate = pr, Ir.toISOString = Yi, Ir.inspect = Qi, Ir.toJSON = gr, Ir.toString = Wi, Ir.unix = fr, Ir.valueOf = hr, Ir.creationData = wr, Ir.year = Ke, Ir.isLeapYear = Ze, Ir.weekYear = xr, Ir.isoWeekYear = Sr, Ir.quarter = Ir.quarters = Pr, Ir.month = ft, Ir.daysInMonth = pt, Ir.week = Ir.weeks = Lt, Ir.isoWeek = Ir.isoWeeks = qt, Ir.weeksInYear = Mr, Ir.isoWeeksInYear = Cr, Ir.date = Lr, Ir.day = Ir.days = Vt, Ir.weekday = Ht, Ir.isoWeekday = Ut, Ir.dayOfYear = qr, Ir.hour = Ir.hours = ln, Ir.minute = Ir.minutes = Or, Ir.second = Ir.seconds = Dr, Ir.millisecond = Ir.milliseconds = Nr, Ir.utcOffset = pi, Ir.utc = vi, Ir.local = gi, Ir.parseZone = _i, Ir.hasAlignedHourOffset = bi, Ir.isDST = yi, Ir.isLocal = ki, Ir.isUtcOffset = xi, Ir.isUtc = Si, Ir.isUTC = Si, Ir.zoneAbbr = jr, Ir.zoneName = Rr, Ir.dates = P("dates accessor is deprecated. Use date instead.", Lr), Ir.months = P("months accessor is deprecated. Use month instead", ft), Ir.years = P("years accessor is deprecated. Use year instead", Ke), Ir.zone = P("moment().zone is deprecated, use moment().utcOffset instead. http://momentjs.com/guides/#/warnings/zone/", mi), Ir.isDSTShifted = P("isDSTShifted is deprecated. See http://momentjs.com/guides/#/warnings/dst-shifted/ for more information", wi);
                 var Vr = N.prototype;
 
                 function Hr(e, t, n, i) {
                     var r = _n(),
                         a = m().set(i, t);
                     return r[n](a, e)
                 }
@@ -50452,15 +50452,15 @@
                 function Kr(e, t, n) {
                     return Wr(e, t, n, "weekdaysShort")
                 }
 
                 function Zr(e, t, n) {
                     return Wr(e, t, n, "weekdaysMin")
                 }
-                Vr.calendar = R, Vr.longDateFormat = F, Vr.invalidDate = B, Vr.ordinal = U, Vr.preparse = Br, Vr.postformat = Br, Vr.relativeTime = Y, Vr.pastFuture = Q, Vr.set = D, Vr.months = st, Vr.monthsShort = ct, Vr.monthsParse = dt, Vr.monthsRegex = _t, Vr.monthsShortRegex = vt, Vr.week = Mt, Vr.firstDayOfYear = Pt, Vr.firstDayOfWeek = At, Vr.weekdays = Nt, Vr.weekdaysMin = Ft, Vr.weekdaysShort = Rt, Vr.weekdaysParse = Bt, Vr.weekdaysRegex = Yt, Vr.weekdaysShortRegex = Gt, Vr.weekdaysMinRegex = Zt, Vr.isPM = rn, Vr.meridiem = on, mn("en", {
+                Vr.calendar = R, Vr.longDateFormat = B, Vr.invalidDate = $, Vr.ordinal = U, Vr.preparse = $r, Vr.postformat = $r, Vr.relativeTime = Y, Vr.pastFuture = Q, Vr.set = D, Vr.months = st, Vr.monthsShort = ct, Vr.monthsParse = dt, Vr.monthsRegex = _t, Vr.monthsShortRegex = vt, Vr.week = Mt, Vr.firstDayOfYear = Pt, Vr.firstDayOfWeek = At, Vr.weekdays = Nt, Vr.weekdaysMin = Bt, Vr.weekdaysShort = Rt, Vr.weekdaysParse = $t, Vr.weekdaysRegex = Yt, Vr.weekdaysShortRegex = Gt, Vr.weekdaysMinRegex = Zt, Vr.isPM = rn, Vr.meridiem = on, mn("en", {
                     dayOfMonthOrdinalParse: /\d{1,2}(th|st|nd|rd)/,
                     ordinal: function(e) {
                         var t = e % 10;
                         return e + (1 === M(e % 100 / 10) ? "th" : 1 === t ? "st" : 2 === t ? "nd" : 3 === t ? "rd" : "th")
                     }
                 }), r.lang = P("moment.lang is deprecated. Use moment.locale instead.", mn), r.langData = P("moment.langData is deprecated. Use moment.localeData instead.", _n);
                 var Jr = Math.abs;
@@ -50636,20 +50636,20 @@
                     if (!d) return "P0D";
                     var h = d < 0 ? "-" : "",
                         f = Ra(this._months) !== Ra(d) ? "-" : "",
                         p = Ra(this._days) !== Ra(d) ? "-" : "",
                         m = Ra(this._milliseconds) !== Ra(d) ? "-" : "";
                     return h + "P" + (a ? f + a + "Y" : "") + (o ? f + o + "M" : "") + (s ? p + s + "D" : "") + (l || c || u ? "T" : "") + (l ? m + l + "H" : "") + (c ? m + c + "M" : "") + (u ? m + u + "S" : "")
                 }
-                var Fa = oi.prototype;
-                return Fa.isValid = ri, Fa.abs = Xr, Fa.add = ta, Fa.subtract = na, Fa.as = sa, Fa.asMilliseconds = ua, Fa.asSeconds = da, Fa.asMinutes = ha, Fa.asHours = fa, Fa.asDays = pa, Fa.asWeeks = ma, Fa.asMonths = va, Fa.asQuarters = ga, Fa.asYears = _a, Fa.valueOf = la, Fa._bubble = ra, Fa.clone = ba, Fa.get = ya, Fa.milliseconds = ka, Fa.seconds = xa, Fa.minutes = Sa, Fa.hours = Ca, Fa.days = Ma, Fa.weeks = Pa, Fa.months = Ta, Fa.years = Aa, Fa.humanize = Na, Fa.toISOString = Ia, Fa.toString = Ia, Fa.toJSON = Ia, Fa.locale = er, Fa.localeData = nr, Fa.toIsoString = P("toIsoString() is deprecated. Please use toISOString() instead (notice the capitals)", Ia), Fa.lang = tr, se("X", 0, 0, "unix"), se("x", 0, 0, "valueOf"), Le("x", Se), Le("X", Te), ze("X", (function(e, t, n) {
+                var Ba = oi.prototype;
+                return Ba.isValid = ri, Ba.abs = Xr, Ba.add = ta, Ba.subtract = na, Ba.as = sa, Ba.asMilliseconds = ua, Ba.asSeconds = da, Ba.asMinutes = ha, Ba.asHours = fa, Ba.asDays = pa, Ba.asWeeks = ma, Ba.asMonths = va, Ba.asQuarters = ga, Ba.asYears = _a, Ba.valueOf = la, Ba._bubble = ra, Ba.clone = ba, Ba.get = ya, Ba.milliseconds = ka, Ba.seconds = xa, Ba.minutes = Sa, Ba.hours = Ca, Ba.days = Ma, Ba.weeks = Pa, Ba.months = Ta, Ba.years = Aa, Ba.humanize = Na, Ba.toISOString = Ia, Ba.toString = Ia, Ba.toJSON = Ia, Ba.locale = er, Ba.localeData = nr, Ba.toIsoString = P("toIsoString() is deprecated. Please use toISOString() instead (notice the capitals)", Ia), Ba.lang = tr, se("X", 0, 0, "unix"), se("x", 0, 0, "valueOf"), Le("x", Se), Le("X", Te), ze("X", (function(e, t, n) {
                     n._d = new Date(1e3 * parseFloat(e, 10))
                 })), ze("x", (function(e, t, n) {
                     n._d = new Date(M(e))
-                })), r.version = "2.24.0", a(Gn), r.fn = Ir, r.min = Xn, r.max = ei, r.now = ti, r.utc = m, r.unix = Fr, r.months = Yr, r.isDate = d, r.locale = mn, r.invalid = b, r.duration = Ti, r.isMoment = S, r.weekdays = Gr, r.parseZone = $r, r.localeData = _n, r.isDuration = si, r.monthsShort = Qr, r.weekdaysMin = Zr, r.defineLocale = vn, r.updateLocale = gn, r.locales = bn, r.weekdaysShort = Kr, r.normalizeUnits = Z, r.relativeTimeRounding = Da, r.relativeTimeThreshold = za, r.calendarFormat = zi, r.prototype = Ir, r.HTML5_FMT = {
+                })), r.version = "2.24.0", a(Gn), r.fn = Ir, r.min = Xn, r.max = ei, r.now = ti, r.utc = m, r.unix = Br, r.months = Yr, r.isDate = d, r.locale = mn, r.invalid = b, r.duration = Ti, r.isMoment = S, r.weekdays = Gr, r.parseZone = Fr, r.localeData = _n, r.isDuration = si, r.monthsShort = Qr, r.weekdaysMin = Zr, r.defineLocale = vn, r.updateLocale = gn, r.locales = bn, r.weekdaysShort = Kr, r.normalizeUnits = Z, r.relativeTimeRounding = Da, r.relativeTimeThreshold = za, r.calendarFormat = zi, r.prototype = Ir, r.HTML5_FMT = {
                     DATETIME_LOCAL: "YYYY-MM-DDTHH:mm",
                     DATETIME_LOCAL_SECONDS: "YYYY-MM-DDTHH:mm:ss",
                     DATETIME_LOCAL_MS: "YYYY-MM-DDTHH:mm:ss.SSS",
                     DATE: "YYYY-MM-DD",
                     TIME: "HH:mm",
                     TIME_SECONDS: "HH:mm:ss",
                     TIME_MS: "HH:mm:ss.SSS",
@@ -51410,22 +51410,22 @@
                 }, V.getHoverColor = function(e) {
                     return e instanceof CanvasPattern || e instanceof CanvasGradient ? e : V.color(e).saturate(.5).darken(.1).rgbString()
                 }
             }(), tn._adapters = an, tn.Animation = J, tn.animationService = X, tn.controllers = Ze, tn.DatasetController = re, tn.defaults = j, tn.Element = K, tn.elements = xe, tn.Interaction = rt, tn.layouts = pt, tn.platform = Dt, tn.plugins = zt, tn.Scale = yn, tn.scaleService = Nt, tn.Ticks = on, tn.Tooltip = Yt, tn.helpers.each(fi, (function(e, t) {
                 tn.scaleService.registerScaleType(t, e, e._defaults)
             })), zi) zi.hasOwnProperty(Ii) && tn.plugins.register(zi[Ii]);
     tn.platform.initialize();
-    var Fi = tn;
+    var Bi = tn;
     return "undefined" != typeof window && (window.Chart = tn), tn.Chart = tn, tn.Legend = zi.legend._element, tn.Title = zi.title._element, tn.pluginService = tn.plugins, tn.PluginBase = tn.Element.extend({}), tn.canvasHelpers = tn.helpers.canvas, tn.layoutService = tn.layouts, tn.LinearScaleBase = Mn, tn.helpers.each(["Bar", "Bubble", "Doughnut", "Line", "PolarArea", "Radar", "Scatter"], (function(e) {
         tn[e] = function(t, n) {
             return new tn(t, tn.helpers.merge(n || {}, {
                 type: e.charAt(0).toLowerCase() + e.slice(1)
             }))
         }
-    })), Fi
+    })), Bi
 })),
 /*!
  * vue-i18n v8.28.2 
  * (c) 2022 kazuya kawaguchi
  * Released under the MIT License.
  */
 function(e, t) {
@@ -51944,16 +51944,16 @@
         for (var i = n.length, r = e, o = 0; o < i;) {
             var s = r[n[o]];
             if (null == s) return null;
             r = s, o++
         }
         return r
     };
-    var F, $ = /<\/?[\w\s="/.':;#-\/]+>/,
-        B = /(?:@(?:\.[a-zA-Z]+)?:(?:[\w\-_|./]+|\([\w\-_:|./]+\)))/g,
+    var B, F = /<\/?[\w\s="/.':;#-\/]+>/,
+        $ = /(?:@(?:\.[a-zA-Z]+)?:(?:[\w\-_|./]+|\([\w\-_:|./]+\)))/g,
         V = /^@(?:\.([a-zA-Z]+))?:/,
         H = /[()]/g,
         U = {
             upper: function(e) {
                 return e.toLocaleUpperCase()
             },
             lower: function(e) {
@@ -52045,15 +52045,15 @@
                 var i = a[n];
                 c(i) ? (l.push(n), l.push("."), s(e, t, i, l), l.pop(), l.pop()) : (l.push(n), s(e, t, i, l), l.pop())
             }));
             else if (r(a)) a.forEach((function(n, i) {
                 c(n) ? (l.push("[" + i + "]"), l.push("."), s(e, t, n, l), l.pop(), l.pop()) : (l.push("[" + i + "]"), s(e, t, n, l), l.pop())
             }));
             else if (o(a)) {
-                if ($.test(a)) {
+                if (F.test(a)) {
                     var u = "Detected HTML in message '" + a + "' of keypath '" + l.join("") + "' at '" + t + "'. Consider component interpolation with '<i18n>' to avoid XSS. See https://bit.ly/2ZqJzkp";
                     "warn" === e ? n(u) : "error" === e && i(u)
                 }
             }
         };
         s(t, e, a, [])
     }, Y.prototype._initVM = function(e) {
@@ -52197,15 +52197,15 @@
         } else {
             if (!o(p) && !d(p)) return this._isSilentTranslationWarn(i) || this._isSilentFallback(e, i) || n("Value of key '" + i + "' is not a string or function!"), null;
             f = p
         }
         return o(f) && (f.indexOf("@:") >= 0 || f.indexOf("@.") >= 0) && (f = this._link(e, t, f, a, "raw", l, h)), this._render(f, s, l, i)
     }, Y.prototype._link = function(e, t, i, a, o, s, l) {
         var c = i,
-            u = c.match(B);
+            u = c.match($);
         for (var d in u)
             if (u.hasOwnProperty(d)) {
                 var h = u[d],
                     f = h.match(V),
                     m = f[0],
                     v = f[1],
                     g = h.replace(m, "").replace(H, "");
@@ -52432,22 +52432,22 @@
         if (this._isFallbackRoot(o)) {
             if (this._isSilentTranslationWarn(i) || n("Fall back to format number to parts of root: key '" + i + "' ."), !this._root) throw Error("unexpected error");
             return this._root.$i18n._ntp(e, t, i, r)
         }
         return o || []
     }, Object.defineProperties(Y.prototype, Q), Object.defineProperty(Y, "availabilities", {
         get: function() {
-            if (!F) {
+            if (!B) {
                 var e = "undefined" != typeof Intl;
-                F = {
+                B = {
                     dateTimeFormat: e && void 0 !== Intl.DateTimeFormat,
                     numberFormat: e && void 0 !== Intl.NumberFormat
                 }
             }
-            return F
+            return B
         }
     }), Y.install = q, Y.version = "8.28.2", Y
 })), /*! showdown v 2.1.0 - 21-04-2022 */
 function() {
     function e(e) {
         "use strict";
         var t = {
@@ -54974,14 +54974,16 @@
         funding: "Funding",
         users: "Benutzer",
         apps: "Apps",
         channels: "Kanäle",
         transactions: "Transaktionen",
         dashboard: "Armaturenbrett",
         node: "Knoten",
+        export_users: "Benutzer exportieren",
+        no_users: "Keine Benutzer gefunden",
         total_capacity: "Gesamtkapazität",
         avg_channel_size: "Durchschn. Kanalgröße",
         biggest_channel_size: "Größte Kanalgröße",
         smallest_channel_size: "Kleinste Kanalgröße",
         number_of_channels: "Anzahl der Kanäle",
         active_channels: "Aktive Kanäle",
         connect_peer: "Peer verbinden",
@@ -54998,14 +55000,15 @@
         topup_hint: "Nutze die Wallet-ID, um eine beliebige Wallet aufzuladen",
         restart_tooltip: "Starte den Server neu, um die Änderungen zu übernehmen",
         add_funds_tooltip: "Füge Geld zu einer Wallet hinzu.",
         reset_defaults: "Zurücksetzen",
         reset_defaults_tooltip: "Alle Einstellungen auf die Standardeinstellungen zurücksetzen.",
         download_backup: "Datenbank-Backup herunterladen",
         name_your_wallet: "Vergib deiner %{name} Wallet einen Namen",
+        wallet_topup_ok: "Erfolg beim Erstellen von virtuellen Mitteln (%{amount} Satoshis). Zahlungen hängen von den tatsächlichen Mitteln der Finanzierungsquelle ab.",
         paste_invoice_label: "Füge eine Rechnung, Zahlungsanforderung oder LNURL ein *",
         lnbits_description: "Einfach zu installieren und kompakt, LNbits kann auf jeder Funding-Quelle im Lightning Netzwerk aufsetzen und sogar LNbits selbst! Du kannst LNbits für dich selbst betreiben oder anderen die Verwaltung durch dich anbieten. Jede Wallet hat ihre eigenen API-Schlüssel und die Anzahl der Wallets ist unbegrenzt. Die Möglichkeit, Gelder auf verschiedene Accounts mit unterschiedlicher Logik aufteilen zu können macht LNbits zu einem nützlichen Werkzeug für deine Buchhaltung - aber auch als Entwicklungswerkzeug. Erweiterungen bereichern LNbits Accounts um zusätzliche Funktionalität, so dass du mit einer Reihe von neuartigen Technologien auf dem Lightning-Netzwerk experimentieren kannst. Wir haben es so einfach wie möglich gemacht, Erweiterungen zu entwickeln, und als freies und Open-Source-Projekt möchten wir Menschen ermutigen, sich selbst hieran zu versuchen und gemeinsam mit uns neue Funktionalitäten zu entwickeln.",
         export_to_phone: "Auf dem Telefon öffnen",
         export_to_phone_desc: "Dieser QR-Code beinhaltet vollständige Rechte auf deine Wallet. Du kannst den QR-Code mit Deinem Telefon scannen, um deine Wallet dort zu öffnen.",
         wallets: "Wallets",
         add_wallet: "Wallet hinzufügen",
         delete_wallet: "Wallet löschen",
@@ -55190,15 +55193,16 @@
         color_scheme: "Farbschema",
         extension_cost: "Diese Version erfordert eine Zahlung von mindestens %{cost} Sats.",
         extension_paid_sats: "Sie haben bereits %{paid_sats} Sats bezahlt.",
         release_details_error: "Kann die Details zur Veröffentlichung nicht abrufen.",
         pay_from_wallet: "Zahlen aus dem Geldbeutel",
         show_qr: "QR anzeigen",
         retry_install: "Installieren erneut versuchen",
-        new_payment: "Neue Zahlung vornehmen"
+        new_payment: "Neue Zahlung vornehmen",
+        hide_empty_wallets: "Leere Geldbörsen verbergen"
     }, window.localisation.en = {
         confirm: "Yes",
         server: "Server",
         theme: "Theme",
         funding: "Funding",
         users: "Users",
         apps: "Apps",
@@ -55304,14 +55308,15 @@
         repository: "Repository",
         confirm_continue: "Are you sure you want to continue?",
         manage_extension_details: "Install/uninstall extension",
         install: "Install",
         uninstall: "Uninstall",
         drop_db: "Remove Data",
         enable: "Enable",
+        pay_to_enable: "Pay To Enable",
         enable_extension_details: "Enable extension for current user",
         disable: "Disable",
         installed: "Installed",
         activated: "Activated",
         deactivated: "Deactivated",
         release_notes: "Release Notes",
         activate_extension_details: "Make extension available/unavailable for users",
@@ -55327,14 +55332,15 @@
         uninstall_confirm: "Yes, Uninstall",
         extension_db_drop_info: "All data for the extension will be permanently deleted. There is no way to undo this operation!",
         extension_db_drop_warning: "You are about to remove all data for the extension. Please type the extension name to continue:",
         extension_min_lnbits_version: "This release requires at least LNbits version",
         payment_hash: "Payment Hash",
         fee: "Fee",
         amount: "Amount",
+        amount_sats: "Amount (sats)",
         tag: "Tag",
         unit: "Unit",
         description: "Description",
         expiry: "Expiry",
         webhook: "Webhook",
         payment_proof: "Payment Proof",
         update_available: "Update %{version} available!",
@@ -55419,29 +55425,38 @@
         look_and_feel: "Look and Feel",
         language: "Language",
         color_scheme: "Color Scheme",
         extension_cost: "This release requires a payment of minimum %{cost} sats.",
         extension_paid_sats: "You have already paid %{paid_sats} sats.",
         release_details_error: "Cannot get the release details.",
         pay_from_wallet: "Pay from Wallet",
+        wallet_required: "Wallet *",
         show_qr: "Show QR",
         retry_install: "Retry Install",
         new_payment: "Make New Payment",
-        hide_empty_wallets: "Hide empty wallets"
+        update_payment: "Update Payment",
+        already_paid_question: "Have you already paid?",
+        sell: "Sell",
+        sell_require: "Ask payment to enable extension",
+        sell_info: "The %{name} extension requires a payment of minimum %{amount} sats to enable.",
+        hide_empty_wallets: "Hide empty wallets",
+        recheck: "Recheck"
     }, window.localisation.es = {
         confirm: "Sí",
         server: "Servidor",
         theme: "Tema",
         funding: "Financiación",
         users: "Usuarios",
         apps: "Aplicaciones",
         channels: "Canales",
         transactions: "Transacciones",
         dashboard: "Tablero de instrumentos",
         node: "Nodo",
+        export_users: "Exportar Usuarios",
+        no_users: "No se encontraron usuarios",
         total_capacity: "Capacidad Total",
         avg_channel_size: "Tamaño Medio del Canal",
         biggest_channel_size: "Tamaño del Canal Más Grande",
         smallest_channel_size: "Tamaño de canal más pequeño",
         number_of_channels: "Número de canales",
         active_channels: "Canales activos",
         connect_peer: "Conectar Par",
@@ -55458,14 +55473,15 @@
         topup_hint: "Utilice el ID de billetera para recargar cualquier billetera",
         restart_tooltip: "Reinicie el servidor para aplicar los cambios",
         add_funds_tooltip: "Agregue fondos a una billetera.",
         reset_defaults: "Restablecer",
         reset_defaults_tooltip: "Borrar todas las configuraciones y restablecer a los valores predeterminados.",
         download_backup: "Descargar copia de seguridad de la base de datos",
         name_your_wallet: "Nombre de su billetera %{name}",
+        wallet_topup_ok: "Éxito creando fondos virtuales (%{amount} sats). Los pagos dependen de los fondos reales en la fuente de financiación.",
         paste_invoice_label: "Pegue la factura aquí",
         lnbits_description: "Fácil de instalar y liviano, LNbits puede ejecutarse en cualquier fuente de financiación de la red Lightning y hasta LNbits mismo! Puede ejecutar LNbits para usted mismo o ofrecer una solución competente a otros. Cada billetera tiene su propia clave API y no hay límite para la cantidad de billeteras que puede crear. La capacidad de particionar fondos hace de LNbits una herramienta útil para la administración de fondos y como herramienta de desarrollo. Las extensiones agregan funcionalidad adicional a LNbits, por lo que puede experimentar con una variedad de tecnologías de vanguardia en la red Lightning. Lo hemos hecho lo más simple posible para desarrollar extensiones y, como un proyecto gratuito y de código abierto, animamos a las personas a que se desarrollen a sí mismas y envíen sus propios contribuciones.",
         export_to_phone: "Exportar a teléfono con código QR",
         export_to_phone_desc: "Este código QR contiene su URL de billetera con acceso completo. Puede escanearlo desde su teléfono para abrir su billetera allí.",
         wallets: "Billeteras",
         add_wallet: "Agregar nueva billetera",
         delete_wallet: "Eliminar billetera",
@@ -55650,26 +55666,29 @@
         color_scheme: "Esquema de colores",
         extension_cost: "Esta versión requiere un pago mínimo de %{cost} sats.",
         extension_paid_sats: "Ya has pagado %{paid_sats} sats.",
         release_details_error: "No se pueden obtener los detalles de la versión.",
         pay_from_wallet: "Pagar desde la billetera",
         show_qr: "Mostrar QR",
         retry_install: "Reintentar Instalación",
-        new_payment: "Realizar nuevo pago"
+        new_payment: "Realizar nuevo pago",
+        hide_empty_wallets: "Ocultar billeteras vacías"
     }, window.localisation.fr = {
         confirm: "Oui",
         server: "Serveur",
         theme: "Thème",
         funding: "Financement",
         users: "Utilisateurs",
         apps: "Applications",
         channels: "Canaux",
         transactions: "Transactions",
         dashboard: "Tableau de bord",
         node: "Noeud",
+        export_users: "Exporter les utilisateurs",
+        no_users: "Aucun utilisateur trouvé",
         total_capacity: "Capacité totale",
         avg_channel_size: "Taille moyenne du canal",
         biggest_channel_size: "Taille de canal maximale",
         smallest_channel_size: "Taille de canal la plus petite",
         number_of_channels: "Nombre de canaux",
         active_channels: "Canaux actifs",
         connect_peer: "Connecter un pair",
@@ -55686,14 +55705,15 @@
         topup_hint: "Utilisez l'ID du portefeuille pour recharger n'importe quel portefeuille",
         restart_tooltip: "Redémarrez le serveur pour que les changements prennent effet",
         add_funds_tooltip: "Ajouter des fonds à un portefeuille.",
         reset_defaults: "Réinitialiser aux valeurs par défaut",
         reset_defaults_tooltip: "Supprimer tous les paramètres et les réinitialiser aux valeurs par défaut.",
         download_backup: "Télécharger la sauvegarde de la base de données",
         name_your_wallet: "Nommez votre portefeuille %{name}",
+        wallet_topup_ok: "Succès de la création de fonds virtuels (%{amount} sats). Les paiements dépendent des fonds réels sur la source de financement.",
         paste_invoice_label: "Coller une facture, une demande de paiement ou un code lnurl *",
         lnbits_description: "Facile à installer et léger, LNbits peut fonctionner sur n'importe quelle source de financement du réseau Lightning et même LNbits lui-même! Vous pouvez exécuter LNbits pour vous-même ou offrir facilement une solution de gardien pour les autres. Chaque portefeuille a ses propres clés API et il n'y a pas de limite au nombre de portefeuilles que vous pouvez créer. La capacité de partitionner les fonds rend LNbits un outil utile pour la gestion de l'argent et comme outil de développement. Les extensions ajoutent une fonctionnalité supplémentaire à LNbits afin que vous puissiez expérimenter une gamme de technologies de pointe sur le réseau Lightning. Nous avons rendu le développement d'extensions aussi simple que possible et, en tant que projet gratuit et open source, nous encourageons les gens à développer et à soumettre les leurs.",
         export_to_phone: "Exporter vers le téléphone avec un code QR",
         export_to_phone_desc: "Ce code QR contient l'URL de votre portefeuille avec un accès complet. Vous pouvez le scanner depuis votre téléphone pour ouvrir votre portefeuille depuis là-bas.",
         wallets: "Portefeuilles",
         add_wallet: "Ajouter un nouveau portefeuille",
         delete_wallet: "Supprimer le portefeuille",
@@ -55878,26 +55898,29 @@
         color_scheme: "Schéma de couleurs",
         extension_cost: "Cette version nécessite un paiement minimum de %{cost} sats.",
         extension_paid_sats: "Vous avez déjà payé %{paid_sats} sats.",
         release_details_error: "Impossible d'obtenir les détails de la version.",
         pay_from_wallet: "Payer depuis le portefeuille",
         show_qr: "Afficher le QR",
         retry_install: "Réessayer l'installation",
-        new_payment: "Effectuer un nouveau paiement"
+        new_payment: "Effectuer un nouveau paiement",
+        hide_empty_wallets: "Masquer les portefeuilles vides"
     }, window.localisation.it = {
         confirm: "Sì",
         server: "Server",
         theme: "Tema",
         funding: "Funding",
         users: "Utenti",
         apps: "Applicazioni",
         channels: "Canali",
         transactions: "Transazioni",
         dashboard: "Pannello di controllo",
         node: "Interruttore",
+        export_users: "Esporta utenti",
+        no_users: "Nessun utente trovato",
         total_capacity: "Capacità Totale",
         avg_channel_size: "Dimensione media del canale",
         biggest_channel_size: "Dimensione del canale più grande",
         smallest_channel_size: "Dimensione Più Piccola del Canale",
         number_of_channels: "Numero di Canali",
         active_channels: "Canali Attivi",
         connect_peer: "Connetti Peer",
@@ -55914,14 +55937,15 @@
         topup_hint: "Usa l'ID del portafoglio per ricaricare qualsiasi portafoglio",
         restart_tooltip: "Riavvia il server affinché le modifiche abbiano effetto",
         add_funds_tooltip: "Aggiungere fondi a un portafoglio",
         reset_defaults: "Ripristina le impostazioni predefinite",
         reset_defaults_tooltip: "Cancella tutte le impostazioni e ripristina i valori predefiniti",
         download_backup: "Scarica il backup del database",
         name_your_wallet: "Dai un nome al tuo portafoglio %{name}",
+        wallet_topup_ok: "Operazione riuscita nella creazione di fondi virtuali (%{amount} sats). I pagamenti dipendono dai fondi effettivi sulla fonte di finanziamento.",
         paste_invoice_label: "Incolla una fattura, una richiesta di pagamento o un codice lnurl *",
         lnbits_description: "Leggero e facile da configurare, LNbits può funzionare su qualsiasi fonte di finanziamento Lightning Network e persino LNbits stesso! Potete gestire LNbits per conto vostro o offrire facilmente una soluzione di custodia per altri. Ogni portafoglio ha le proprie chiavi API e non c'è limite al numero di portafogli che si possono creare. La possibilità di suddividere i fondi rende LNbits uno strumento utile per la gestione del denaro e come strumento di sviluppo. Le estensioni aggiungono ulteriori funzionalità a LNbits, consentendo di sperimentare una serie di tecnologie all'avanguardia sulla rete Lightning. Abbiamo reso lo sviluppo delle estensioni il più semplice possibile e, in quanto progetto libero e open-source, incoraggiamo le persone a sviluppare e inviare le proprie",
         export_to_phone: "Esportazione su telefono con codice QR",
         export_to_phone_desc: "Questo codice QR contiene l'URL del portafoglio con accesso da amministratore. È possibile scansionarlo dal telefono per aprire il portafoglio da lì.",
         wallets: "Portafogli",
         add_wallet: "Aggiungi un nuovo portafoglio",
         delete_wallet: "Elimina il portafoglio",
@@ -56106,26 +56130,29 @@
         color_scheme: "Schema dei colori",
         extension_cost: "Questa versione richiede un pagamento minimo di %{cost} satoshi.",
         extension_paid_sats: "Hai già pagato %{paid_sats} sats.",
         release_details_error: "Impossibile ottenere i dettagli della versione.",
         pay_from_wallet: "Paga dal Portafoglio",
         show_qr: "Mostra QR",
         retry_install: "Riprova Installazione",
-        new_payment: "Effettua Nuovo Pagamento"
+        new_payment: "Effettua Nuovo Pagamento",
+        hide_empty_wallets: "Nascondi portafogli vuoti"
     }, window.localisation.jp = {
         confirm: "はい",
         server: "サーバー",
         theme: "テーマ",
         funding: "資金調達",
         users: "ユーザー",
         apps: "アプリ",
         channels: "チャンネル",
         transactions: "トランザクション",
         dashboard: "ダッシュボード",
         node: "ノード",
+        export_users: "ユーザーのエクスポート",
+        no_users: "ユーザーが見つかりません",
         total_capacity: "合計容量",
         avg_channel_size: "平均チャンネルサイズ",
         biggest_channel_size: "最大チャネルサイズ",
         smallest_channel_size: "最小チャンネルサイズ",
         number_of_channels: "チャンネル数",
         active_channels: "アクティブチャンネル",
         connect_peer: "ピアを接続",
@@ -56142,14 +56169,15 @@
         topup_hint: "ウォレットIDを使用して、任意のウォレットをトップアップできます",
         restart_tooltip: "サーバーを再起動して変更を適用します",
         add_funds_tooltip: "ウォレットに資金を追加します。",
         reset_defaults: "リセット",
         reset_defaults_tooltip: "すべての設定を削除してデフォルトに戻します。",
         download_backup: "データベースのバックアップをダウンロードする",
         name_your_wallet: "あなたのウォレットの名前 %{name}",
+        wallet_topup_ok: "仮想資金の作成に成功しました（%{amount} sats）。支払いは資金ソースの実際の資金に依存します。",
         paste_invoice_label: "請求書を貼り付けてください",
         lnbits_description: "簡単にインストールでき、軽量なLNbitsは、あらゆるライトニングネットワークの資金源と、LNbits自身でさえも実行できます！LNbitsを個人で実行することも、他人に対してカストディアンソリューションをで実行できます！ LNbitsを自分で実行することも、他の人に優れたソリューションを提供することもできます。各ウォレットには独自のAPIキーがあり、作成できるウォレットの数に制限はありません。資金を分割する機能は、LNbitsを資金管理ツールとして使用したり、開発ツールとして使用したりするための便利なツールです。拡張機能は、LNbitsに追加の機能を追加します。そのため、LNbitsは最先端の技術をネットワークLightningで試すことができます。拡張機能を開発するのは簡単で、無料でオープンソースのプロジェクトであるため、人々が自分で開発し、自分の貢献を送信することを奨励しています。",
         export_to_phone: "電話にエクスポート",
         export_to_phone_desc: "ウォレットを電話にエクスポートすると、ウォレットを削除する前にウォレットを復元できます。ウォレットを削除すると、ウォレットの秘密鍵が削除され、ウォレットを復元することはできません。",
         wallets: "ウォレット",
         add_wallet: "ウォレットを追加",
         delete_wallet: "ウォレットを削除",
@@ -56334,26 +56362,29 @@
         color_scheme: "カラースキーム",
         extension_cost: "このリリースには最低 %{cost} サトシの支払いが必要です。",
         extension_paid_sats: "すでに%{paid_sats} satsを支払いました。",
         release_details_error: "リリースの詳細を取得できません。",
         pay_from_wallet: "ウォレットから支払う",
         show_qr: "QRを表示",
         retry_install: "再試行インストール",
-        new_payment: "新しい支払いを作成する"
+        new_payment: "新しい支払いを作成する",
+        hide_empty_wallets: "空のウォレットを非表示にする"
     }, window.localisation.cn = {
         confirm: "确定",
         server: "服务器",
         theme: "主题",
         funding: "资金",
         users: "用户",
         apps: "应用程序",
         channels: "频道",
         transactions: "交易记录",
         dashboard: "控制面板",
         node: "节点",
+        export_users: "导出用户",
+        no_users: "未找到用户",
         total_capacity: "总容量",
         avg_channel_size: "平均频道大小",
         biggest_channel_size: "最大通道大小",
         smallest_channel_size: "最小频道尺寸",
         number_of_channels: "频道数量",
         active_channels: "活跃频道",
         connect_peer: "连接对等",
@@ -56370,14 +56401,15 @@
         topup_hint: "使用钱包ID为任何钱包充值",
         restart_tooltip: "重新启动服务器以使更改生效",
         add_funds_tooltip: "为钱包添加资金",
         reset_defaults: "重置为默认设置",
         reset_defaults_tooltip: "删除所有设置并重置为默认设置",
         download_backup: "下载数据库备份",
         name_your_wallet: "给你的 %{name}钱包起个名字",
+        wallet_topup_ok: "成功创建虚拟资金（%{amount} sats）。付款取决于资金来源的实际资金。",
         paste_invoice_label: "粘贴发票，付款请求或lnurl*",
         lnbits_description: "LNbits 设置简单、轻量级，可以在任何闪电网络的资金来源上运行，甚至可以在LNbits自身上运行！您可以为自己运行LNbits，或者轻松为他人提供托管解决方案。每个钱包都有自己的 API 密钥，你可以创建的钱包数量没有限制。能够把资金分开管理使 LNbits 成为一款有用的资金管理和开发工具。扩展程序增加了 LNbits 的额外功能，所以你可以在闪电网络上尝试各种尖端技术。我们已经尽可能简化了开发扩展程序的过程，作为一个免费和开源的项目，我们鼓励人们开发并提交自己的扩展程序。",
         export_to_phone: "通过二维码导出到手机",
         export_to_phone_desc: "这个二维码包含您钱包的URL。您可以使用手机扫描的方式打开您的钱包。",
         wallets: "钱包",
         add_wallet: "添加新钱包",
         delete_wallet: "删除钱包",
@@ -56562,26 +56594,29 @@
         color_scheme: "配色方案",
         extension_cost: "此版本需要支付最低 %{cost} sats。",
         extension_paid_sats: "您已经支付了%{paid_sats} sats。",
         release_details_error: "无法获取发布详情。",
         pay_from_wallet: "从钱包支付",
         show_qr: "显示QR码",
         retry_install: "重试安装",
-        new_payment: "创建新支付"
+        new_payment: "创建新支付",
+        hide_empty_wallets: "隐藏空钱包"
     }, window.localisation.nl = {
         confirm: "Ja",
         server: "Server",
         theme: "Thema",
         funding: "Financiering",
         users: "Gebruikers",
         apps: "Apps",
         channels: "Kanalen",
         transactions: "Transacties",
         dashboard: "Dashboard",
         node: "Knooppunt",
+        export_users: "Gebruikers exporteren",
+        no_users: "Geen gebruikers gevonden",
         total_capacity: "Totale capaciteit",
         avg_channel_size: "Gem. Kanaalgrootte",
         biggest_channel_size: "Grootste Kanaalgrootte",
         smallest_channel_size: "Kleinste Kanaalgrootte",
         number_of_channels: "Aantal kanalen",
         active_channels: "Actieve Kanalen",
         connect_peer: "Peer verbinden",
@@ -56598,14 +56633,15 @@
         topup_hint: "Gebruik de portemonnee-ID om elke portemonnee bij te vullen",
         restart_tooltip: "Start de server opnieuw op zodat wijzigingen van kracht worden",
         add_funds_tooltip: "Voeg geld toe aan een portemonnee.",
         reset_defaults: "Standaardinstellingen herstellen",
         reset_defaults_tooltip: "Wis alle instellingen en herstel de standaardinstellingen.",
         download_backup: "Databaseback-up downloaden",
         name_your_wallet: "Geef je %{name} portemonnee een naam",
+        wallet_topup_ok: "Succes met het aanmaken van virtuele fondsen (%{amount} sats). Betalingen zijn afhankelijk van de werkelijke fondsen op de financieringsbron.",
         paste_invoice_label: "Plak een factuur, betalingsverzoek of lnurl-code*",
         lnbits_description: "Gemakkelijk in te stellen en lichtgewicht, LNbits kan op elke lightning-netwerkfinancieringsbron draaien en zelfs LNbits zelf! U kunt LNbits voor uzelf laten draaien of gemakkelijk een bewaardersoplossing voor anderen bieden. Elke portemonnee heeft zijn eigen API-sleutels en er is geen limiet aan het aantal portemonnees dat u kunt maken. Het kunnen partitioneren van fondsen maakt LNbits een nuttige tool voor geldbeheer en als ontwikkelingstool. Extensies voegen extra functionaliteit toe aan LNbits, zodat u kunt experimenteren met een reeks toonaangevende technologieën op het bliksemschichtnetwerk. We hebben het ontwikkelen van extensies zo eenvoudig mogelijk gemaakt en als een gratis en opensource-project moedigen we mensen aan om hun eigen ontwikkelingen in te dienen.",
         export_to_phone: "Exporteren naar telefoon met QR-code",
         export_to_phone_desc: "Deze QR-code bevat uw portemonnee-URL met volledige toegang. U kunt het vanaf uw telefoon scannen om uw portemonnee van daaruit te openen.",
         wallets: "Portemonnees",
         add_wallet: "Een nieuwe portemonnee toevoegen",
         delete_wallet: "Portemonnee verwijderen",
@@ -56790,26 +56826,29 @@
         color_scheme: "Kleurenschema",
         extension_cost: "Deze release vereist een betaling van minimaal %{cost} sats.",
         extension_paid_sats: "U heeft al %{paid_sats} sats betaald.",
         release_details_error: "Kan de gegevens van de release niet ophalen.",
         pay_from_wallet: "Betalen vanuit Portemonnee",
         show_qr: "Toon QR",
         retry_install: "Opnieuw installeren",
-        new_payment: "Nieuwe betaling maken"
+        new_payment: "Nieuwe betaling maken",
+        hide_empty_wallets: "Verberg lege portemonnees"
     }, window.localisation.pi = {
         confirm: "Aye",
         server: "Cap`n",
         theme: "Theme",
         funding: "Funding",
         users: "Buccaneers",
         apps: "Arrrrplications",
         channels: "Channels",
         transactions: "Pirate Transactions and loot",
         dashboard: "Arrr-board",
         node: "Node",
+        export_users: "Export Mateys",
+        no_users: "No swabbies found",
         total_capacity: "Total Capacity",
         avg_channel_size: "Avg. Channel Size",
         biggest_channel_size: "Largest Bilge Size",
         smallest_channel_size: "Smallest Channel Size",
         number_of_channels: "Nummer o' Channels",
         active_channels: "Active Channels",
         connect_peer: "Connect Peer",
@@ -56826,14 +56865,15 @@
         topup_hint: "Use the chest ID to top up any chest",
         restart_tooltip: "Restart the Cap`n for changes to take effect, arr!",
         add_funds_tooltip: "Add doubloons to a chest and make it heavier",
         reset_defaults: "Reset to Davy Jones Locker",
         reset_defaults_tooltip: "Scuttle all settings and reset to Davy Jones Locker. Aye, start anew!",
         download_backup: "Download database booty",
         name_your_wallet: "Name yer %{name} treasure chest",
+        wallet_topup_ok: "Success creatin' virtual funds (%{amount} sats). Payments depend on actual funds on funding source.",
         paste_invoice_label: "Paste a booty, payment request or lnurl code, matey!",
         lnbits_description: "Arr, easy to set up and lightweight, LNbits can run on any Lightning Network funding source and even LNbits itself! Ye can run LNbits for yourself, or easily offer a custodian solution for others. Each chest has its own API keys and there be no limit to the number of chests ye can make. Being able to partition booty makes LNbits a useful tool for money management and as a development tool. Arr, extensions add extra functionality to LNbits so ye can experiment with a range of cutting-edge technologies on the lightning network. We have made developing extensions as easy as possible, and as a free and open-source project, we encourage scallywags to develop and submit their own.",
         export_to_phone: "Export to Phone with QR Code, me hearties",
         export_to_phone_desc: "This QR code contains yer chest URL with full access. Ye can scan it from yer phone to open yer chest from there, arr!",
         wallets: "Treasure Chests",
         add_wallet: "Add a new chest and fill it with doubloons!",
         delete_wallet: "Scuttle the Chest",
@@ -57018,26 +57058,29 @@
         color_scheme: "Colour Scheme",
         extension_cost: "This release be needin' a payment o' minimum %{cost} sats, arr.",
         extension_paid_sats: "Ye have already paid %{paid_sats} sats.",
         release_details_error: "Cannot get th' release details.",
         pay_from_wallet: "Pay from ye Wallet",
         show_qr: "Show QR",
         retry_install: "Try 'nstallin' Again",
-        new_payment: "Make New Payment"
+        new_payment: "Make New Payment",
+        hide_empty_wallets: "Stow empty wallets"
     }, window.localisation.pl = {
         confirm: "Tak",
         server: "Serwer",
         theme: "Motyw",
         funding: "Finansowanie",
         users: "Użytkownicy",
         apps: "Aplikacje",
         channels: "Kanały",
         transactions: "Transakcje",
         dashboard: "Panel kontrolny",
         node: "Węzeł",
+        export_users: "Eksportuj użytkowników",
+        no_users: "Nie znaleziono użytkowników",
         total_capacity: "Całkowita Pojemność",
         avg_channel_size: "Średni rozmiar kanału",
         biggest_channel_size: "Największy Rozmiar Kanału",
         smallest_channel_size: "Najmniejszy Rozmiar Kanału",
         number_of_channels: "Ilość kanałów",
         active_channels: "Aktywne kanały",
         connect_peer: "Połącz z węzłem równorzędnym",
@@ -57054,14 +57097,15 @@
         topup_hint: "Użyj ID portfela aby go doładować",
         restart_tooltip: "Zrestartuj serwer aby aktywować zmiany",
         add_funds_tooltip: "Dodaj środki do portfela.",
         reset_defaults: "Powrót do ustawień domyślnych",
         reset_defaults_tooltip: "Wymaż wszystkie ustawienia i ustaw domyślne.",
         download_backup: "Pobierz kopię zapasową bazy danych",
         name_your_wallet: "Nazwij swój portfel %{name}",
+        wallet_topup_ok: "Sukces w tworzeniu wirtualnych środków (%{amount} sats). Płatności zależą od rzeczywistych środków na źródle finansowania.",
         paste_invoice_label: "Wklej fakturę, żądanie zapłaty lub kod lnurl *",
         lnbits_description: "Łatwy i lekki w konfiguracji, LNbits może działać w oparciu o dowolne źródło finansowania w sieci lightning czy nawet inną instancję LNbits! Możesz uruchomić instancję LNbits dla siebie lub dla innych. Każdy portfel ma swoje klucze API i nie ma ograniczeń jeśli chodzi o ilość portfeli. LNbits umożliwia dzielenie środków w celu zarządzania nimi, jest również dobrym narzędziem deweloperskim. Rozszerzenia zwiększają funkcjonalność LNbits co umożliwia eksperymentowanie z nowym technologiami w sieci lightning. Tworzenie rozszerzeń jest proste dlatego zachęcamy innych deweloperów do tworzenia dodatkowych funkcjonalności i wysyłanie do nas PR",
         export_to_phone: "Eksport kodu QR na telefon",
         export_to_phone_desc: "Ten kod QR zawiera adres URL Twojego portfela z pełnym dostępem do niego. Możesz go zeskanować na swoim telefonie aby otworzyć na nim ten portfel.",
         wallets: "Portfele",
         add_wallet: "Dodaj portfel",
         delete_wallet: "Usuń portfel",
@@ -57246,26 +57290,29 @@
         color_scheme: "Schemat kolorów",
         extension_cost: "To niniejsze wydanie wymaga zapłaty minimalnej %{cost} satów.",
         extension_paid_sats: "Już zapłaciłeś %{paid_sats} satów.",
         release_details_error: "Nie można uzyskać szczegółów wydania.",
         pay_from_wallet: "Zapłać z portfela",
         show_qr: "Pokaż kod QR",
         retry_install: "Ponów instalację",
-        new_payment: "Dokonaj nowej płatności"
+        new_payment: "Dokonaj nowej płatności",
+        hide_empty_wallets: "Ukryj puste portfele"
     }, window.localisation.fr = {
         confirm: "Oui",
         server: "Serveur",
         theme: "Thème",
         funding: "Financement",
         users: "Utilisateurs",
         apps: "Applications",
         channels: "Canaux",
         transactions: "Transactions",
         dashboard: "Tableau de bord",
         node: "Noeud",
+        export_users: "Exporter les utilisateurs",
+        no_users: "Aucun utilisateur trouvé",
         total_capacity: "Capacité totale",
         avg_channel_size: "Taille moyenne du canal",
         biggest_channel_size: "Taille de canal maximale",
         smallest_channel_size: "Taille de canal la plus petite",
         number_of_channels: "Nombre de canaux",
         active_channels: "Canaux actifs",
         connect_peer: "Connecter un pair",
@@ -57282,14 +57329,15 @@
         topup_hint: "Utilisez l'ID du portefeuille pour recharger n'importe quel portefeuille",
         restart_tooltip: "Redémarrez le serveur pour que les changements prennent effet",
         add_funds_tooltip: "Ajouter des fonds à un portefeuille.",
         reset_defaults: "Réinitialiser aux valeurs par défaut",
         reset_defaults_tooltip: "Supprimer tous les paramètres et les réinitialiser aux valeurs par défaut.",
         download_backup: "Télécharger la sauvegarde de la base de données",
         name_your_wallet: "Nommez votre portefeuille %{name}",
+        wallet_topup_ok: "Succès de la création de fonds virtuels (%{amount} sats). Les paiements dépendent des fonds réels sur la source de financement.",
         paste_invoice_label: "Coller une facture, une demande de paiement ou un code lnurl *",
         lnbits_description: "Facile à installer et léger, LNbits peut fonctionner sur n'importe quelle source de financement du réseau Lightning et même LNbits lui-même! Vous pouvez exécuter LNbits pour vous-même ou offrir facilement une solution de gardien pour les autres. Chaque portefeuille a ses propres clés API et il n'y a pas de limite au nombre de portefeuilles que vous pouvez créer. La capacité de partitionner les fonds rend LNbits un outil utile pour la gestion de l'argent et comme outil de développement. Les extensions ajoutent une fonctionnalité supplémentaire à LNbits afin que vous puissiez expérimenter une gamme de technologies de pointe sur le réseau Lightning. Nous avons rendu le développement d'extensions aussi simple que possible et, en tant que projet gratuit et open source, nous encourageons les gens à développer et à soumettre les leurs.",
         export_to_phone: "Exporter vers le téléphone avec un code QR",
         export_to_phone_desc: "Ce code QR contient l'URL de votre portefeuille avec un accès complet. Vous pouvez le scanner depuis votre téléphone pour ouvrir votre portefeuille depuis là-bas.",
         wallets: "Portefeuilles",
         add_wallet: "Ajouter un nouveau portefeuille",
         delete_wallet: "Supprimer le portefeuille",
@@ -57474,26 +57522,29 @@
         color_scheme: "Schéma de couleurs",
         extension_cost: "Cette version nécessite un paiement minimum de %{cost} sats.",
         extension_paid_sats: "Vous avez déjà payé %{paid_sats} sats.",
         release_details_error: "Impossible d'obtenir les détails de la version.",
         pay_from_wallet: "Payer depuis le portefeuille",
         show_qr: "Afficher le QR",
         retry_install: "Réessayer l'installation",
-        new_payment: "Effectuer un nouveau paiement"
+        new_payment: "Effectuer un nouveau paiement",
+        hide_empty_wallets: "Masquer les portefeuilles vides"
     }, window.localisation.nl = {
         confirm: "Ja",
         server: "Server",
         theme: "Thema",
         funding: "Financiering",
         users: "Gebruikers",
         apps: "Apps",
         channels: "Kanalen",
         transactions: "Transacties",
         dashboard: "Dashboard",
         node: "Knooppunt",
+        export_users: "Gebruikers exporteren",
+        no_users: "Geen gebruikers gevonden",
         total_capacity: "Totale capaciteit",
         avg_channel_size: "Gem. Kanaalgrootte",
         biggest_channel_size: "Grootste Kanaalgrootte",
         smallest_channel_size: "Kleinste Kanaalgrootte",
         number_of_channels: "Aantal kanalen",
         active_channels: "Actieve Kanalen",
         connect_peer: "Peer verbinden",
@@ -57510,14 +57561,15 @@
         topup_hint: "Gebruik de portemonnee-ID om elke portemonnee bij te vullen",
         restart_tooltip: "Start de server opnieuw op zodat wijzigingen van kracht worden",
         add_funds_tooltip: "Voeg geld toe aan een portemonnee.",
         reset_defaults: "Standaardinstellingen herstellen",
         reset_defaults_tooltip: "Wis alle instellingen en herstel de standaardinstellingen.",
         download_backup: "Databaseback-up downloaden",
         name_your_wallet: "Geef je %{name} portemonnee een naam",
+        wallet_topup_ok: "Succes met het aanmaken van virtuele fondsen (%{amount} sats). Betalingen zijn afhankelijk van de werkelijke fondsen op de financieringsbron.",
         paste_invoice_label: "Plak een factuur, betalingsverzoek of lnurl-code*",
         lnbits_description: "Gemakkelijk in te stellen en lichtgewicht, LNbits kan op elke lightning-netwerkfinancieringsbron draaien en zelfs LNbits zelf! U kunt LNbits voor uzelf laten draaien of gemakkelijk een bewaardersoplossing voor anderen bieden. Elke portemonnee heeft zijn eigen API-sleutels en er is geen limiet aan het aantal portemonnees dat u kunt maken. Het kunnen partitioneren van fondsen maakt LNbits een nuttige tool voor geldbeheer en als ontwikkelingstool. Extensies voegen extra functionaliteit toe aan LNbits, zodat u kunt experimenteren met een reeks toonaangevende technologieën op het bliksemschichtnetwerk. We hebben het ontwikkelen van extensies zo eenvoudig mogelijk gemaakt en als een gratis en opensource-project moedigen we mensen aan om hun eigen ontwikkelingen in te dienen.",
         export_to_phone: "Exporteren naar telefoon met QR-code",
         export_to_phone_desc: "Deze QR-code bevat uw portemonnee-URL met volledige toegang. U kunt het vanaf uw telefoon scannen om uw portemonnee van daaruit te openen.",
         wallets: "Portemonnees",
         add_wallet: "Een nieuwe portemonnee toevoegen",
         delete_wallet: "Portemonnee verwijderen",
@@ -57702,26 +57754,29 @@
         color_scheme: "Kleurenschema",
         extension_cost: "Deze release vereist een betaling van minimaal %{cost} sats.",
         extension_paid_sats: "U heeft al %{paid_sats} sats betaald.",
         release_details_error: "Kan de gegevens van de release niet ophalen.",
         pay_from_wallet: "Betalen vanuit Portemonnee",
         show_qr: "Toon QR",
         retry_install: "Opnieuw installeren",
-        new_payment: "Nieuwe betaling maken"
+        new_payment: "Nieuwe betaling maken",
+        hide_empty_wallets: "Verberg lege portemonnees"
     }, window.localisation.we = {
         confirm: "Ydw",
         server: "Gweinydd",
         theme: "Thema",
         funding: "Arian fyndio",
         users: "Defnyddwyr",
         apps: "Apiau",
         channels: "Sianelau",
         transactions: "Trafodion",
         dashboard: "Panel Gweinyddol",
         node: "Nod",
+        export_users: "Allfor Defnyddwyr",
+        no_users: "Heb ganfod defnyddwyr",
         total_capacity: "Capasiti Cyfanswm",
         avg_channel_size: "Maint Sianel Cyf.",
         biggest_channel_size: "Maint Sianel Fwyaf",
         smallest_channel_size: "Maint Sianel Lleiaf",
         number_of_channels: "Nifer y Sianeli",
         active_channels: "Sianeli Gweithredol",
         connect_peer: "Cysylltu â Chymar",
@@ -57738,14 +57793,15 @@
         topup_hint: "Defnyddiwch ID y waled i ychwanegu at unrhyw waled",
         restart_tooltip: "Ailgychwyn y gweinydd er mwyn i newidiadau ddod i rym",
         add_funds_tooltip: "Ychwanegu arian at waled.",
         reset_defaults: "Ailosod i`r rhagosodiadau",
         reset_defaults_tooltip: "Dileu pob gosodiad ac ailosod i`r rhagosodiadau.",
         download_backup: "Lawrlwytho copi wrth gefn cronfa ddata",
         name_your_wallet: "Enwch eich waled %{name}",
+        wallet_topup_ok: "Llwyddiant wrth greu cronfeydd rhithwir (%{amount} sats). Mae taliadau'n dibynnu ar gronfeydd gwirioneddol ar y ffynhonnell cyllido.",
         paste_invoice_label: "Gludwch anfoneb, cais am daliad neu god lnurl *",
         lnbits_description: "Yn hawdd iw sefydlu ac yn ysgafn, gall LNbits redeg ar unrhyw ffynhonnell ariannu rhwydwaith mellt a hyd yn oed LNbits ei hun! Gallwch redeg LNbits i chi`ch hun, neu gynnig datrysiad ceidwad i eraill yn hawdd. Mae gan bob waled ei allweddi API ei hun ac nid oes cyfyngiad ar nifer y waledi y gallwch eu gwneud. Mae gallu rhannu cronfeydd yn gwneud LNbits yn arf defnyddiol ar gyfer rheoli arian ac fel offeryn datblygu. Mae estyniadau yn ychwanegu ymarferoldeb ychwanegol at LNbits fel y gallwch arbrofi gydag ystod o dechnolegau blaengar ar y rhwydwaith mellt. Rydym wedi gwneud datblygu estyniadau mor hawdd â phosibl, ac fel prosiect ffynhonnell agored am ddim, rydym yn annog pobl i ddatblygu a chyflwyno eu rhai eu hunain.",
         export_to_phone: "Allforio i Ffôn gyda chod QR",
         export_to_phone_desc: "Mae`r cod QR hwn yn cynnwys URL eich waled gyda mynediad llawn. Gallwch ei sganio o`ch ffôn i agor eich waled oddi yno.",
         wallets: "Waledi",
         add_wallet: "Ychwanegu waled newydd",
         delete_wallet: "Dileu waled",
@@ -57930,26 +57986,29 @@
         color_scheme: "Cynllun Lliw",
         extension_cost: "Mae'r rhyddhad hwn yn gofyn am daliad o leiaf %{cost} sats.",
         extension_paid_sats: "Rydych chi eisoes wedi talu %{paid_sats} sats.",
         release_details_error: "Methu cael manylion y rhyddhau.",
         pay_from_wallet: "Talu o'r Waled",
         show_qr: "Dangos QR",
         retry_install: "Ailgeisio Gosod",
-        new_payment: "Gwneud Taliad Newydd"
+        new_payment: "Gwneud Taliad Newydd",
+        hide_empty_wallets: "Cuddio waledau gwag"
     }, window.localisation.pt = {
         confirm: "Sim",
         server: "Servidor",
         theme: "Tema",
         funding: "Financiamento",
         users: "Usuários",
         apps: "Aplicativos",
         channels: "Canais",
         transactions: "Transações",
         dashboard: "Painel de Controle",
         node: "Nó",
+        export_users: "Exportar Usuários",
+        no_users: "Nenhum usuário encontrado",
         total_capacity: "Capacidade Total",
         avg_channel_size: "Tamanho Médio do Canal",
         biggest_channel_size: "Maior Tamanho do Canal",
         smallest_channel_size: "Menor Tamanho de Canal",
         number_of_channels: "Número de Canais",
         active_channels: "Canais Ativos",
         connect_peer: "Conectar Par",
@@ -57966,14 +58025,15 @@
         topup_hint: "Use o ID da carteira para recarregar qualquer carteira",
         restart_tooltip: "Reinicie o servidor para que as alterações tenham efeito",
         add_funds_tooltip: "Adicionar fundos a uma carteira.",
         reset_defaults: "Redefinir para padrões",
         reset_defaults_tooltip: "Apagar todas as configurações e redefinir para os padrões.",
         download_backup: "Fazer backup da base de dados",
         name_your_wallet: "Nomeie sua carteira %{name}",
+        wallet_topup_ok: "Sucesso ao criar fundos virtuais (%{amount} sats). Os pagamentos dependem dos fundos reais na fonte de financiamento.",
         paste_invoice_label: "Cole uma fatura, pedido de pagamento ou código lnurl *",
         lnbits_description: "Fácil de configurar e leve, o LNbits pode ser executado em qualquer fonte de financiamento da Lightning Network e até mesmo o LNbits em si! Você pode executar o LNbits para si mesmo ou oferecer facilmente uma solução de custódia para outros. Cada carteira tem suas próprias chaves de API e não há limite para o número de carteiras que você pode criar. Ser capaz de particionar fundos torna o LNbits uma ferramenta útil para gerenciamento de dinheiro e como uma ferramenta de desenvolvimento. As extensões adicionam funcionalidades extras ao LNbits para que você possa experimentar uma série de tecnologias de ponta na rede lightning. Nós tornamos o desenvolvimento de extensões o mais fácil possível e, como um projeto gratuito e de código aberto, incentivamos as pessoas a desenvolver e enviar as suas próprias.",
         export_to_phone: "Exportar para o telefone com código QR",
         export_to_phone_desc: "Este código QR contém a URL da sua carteira com acesso total. Você pode escaneá-lo do seu telefone para abrir sua carteira a partir dele.",
         wallets: "Carteiras",
         add_wallet: "Adicionar nova carteira",
         delete_wallet: "Excluir carteira",
@@ -58158,26 +58218,29 @@
         color_scheme: "Esquema de Cores",
         extension_cost: "Este lançamento requer um pagamento mínimo de %{cost} sats.",
         extension_paid_sats: "Você já pagou %{paid_sats} sats.",
         release_details_error: "Não é possível obter os detalhes da versão.",
         pay_from_wallet: "Pague da Carteira",
         show_qr: "Exibir QR",
         retry_install: "Reinstalar Tente Novamente",
-        new_payment: "Realizar Novo Pagamento"
+        new_payment: "Realizar Novo Pagamento",
+        hide_empty_wallets: "Ocultar carteiras vazias"
     }, window.localisation.br = {
         confirm: "Sim",
         server: "Servidor",
         theme: "Tema",
         funding: "Financiamento",
         users: "Usuários",
         apps: "Aplicativos",
         channels: "Canais",
         transactions: "Transações",
         dashboard: "Painel de Controle",
         node: "Nó",
+        export_users: "Exportar Usuários",
+        no_users: "Nenhum usuário encontrado",
         total_capacity: "Capacidade Total",
         avg_channel_size: "Tamanho médio do canal",
         biggest_channel_size: "Maior Tamanho de Canal",
         smallest_channel_size: "Tamanho Mínimo do Canal",
         number_of_channels: "Número de Canais",
         active_channels: "Canais Ativos",
         connect_peer: "Conectar Par",
@@ -58194,14 +58257,15 @@
         topup_hint: "Use o ID da carteira para recarregar qualquer carteira",
         restart_tooltip: "Reinicie o servidor para que as alterações tenham efeito",
         add_funds_tooltip: "Adicionar fundos a uma carteira.",
         reset_defaults: "Redefinir para padrões",
         reset_defaults_tooltip: "Apagar todas as configurações e redefinir para os padrões.",
         download_backup: "Fazer backup do banco de dados",
         name_your_wallet: "Nomeie sua carteira %{name}",
+        wallet_topup_ok: "Sucesso ao criar fundos virtuais (%{amount} sats). Pagamentos dependem dos fundos reais na fonte de financiamento.",
         paste_invoice_label: "Cole uma fatura, pedido de pagamento ou código lnurl *",
         lnbits_description: "Fácil de configurar e leve, o LNbits pode ser executado em qualquer fonte de financiamento da Lightning Network e até mesmo o LNbits em si! Você pode executar o LNbits para si mesmo ou oferecer facilmente uma solução de custódia para outros. Cada carteira tem suas próprias chaves de API e não há limite para o número de carteiras que você pode criar. Ser capaz de particionar fundos torna o LNbits uma ferramenta útil para gerenciamento de dinheiro e como uma ferramenta de desenvolvimento. As extensões adicionam funcionalidades extras ao LNbits para que você possa experimentar uma série de tecnologias de ponta na rede lightning. Nós tornamos o desenvolvimento de extensões o mais fácil possível e, como um projeto gratuito e de código aberto, incentivamos as pessoas a desenvolver e enviar as suas próprias.",
         export_to_phone: "Exportar para o telefone com código QR",
         export_to_phone_desc: "Este código QR contém a URL da sua carteira com acesso total. Você pode escaneá-lo do seu telefone para abrir sua carteira a partir dele.",
         wallets: "Carteiras",
         add_wallet: "Adicionar nova carteira",
         delete_wallet: "Excluir carteira",
@@ -58386,26 +58450,29 @@
         color_scheme: "Esquema de Cores",
         extension_cost: "Este lançamento requer um pagamento mínimo de %{cost} sats.",
         extension_paid_sats: "Você já pagou %{paid_sats} sats.",
         release_details_error: "Não é possível obter os detalhes da versão.",
         pay_from_wallet: "Pagar com a Carteira",
         show_qr: "Exibir QR",
         retry_install: "Repetir Instalação",
-        new_payment: "Efetuar Novo Pagamento"
+        new_payment: "Efetuar Novo Pagamento",
+        hide_empty_wallets: "Ocultar carteiras vazias"
     }, window.localisation.cs = {
         confirm: "Ano",
         server: "Server",
         theme: "Téma",
         funding: "Financování",
         users: "Uživatelé",
         apps: "Aplikace",
         channels: "Kanály",
         transactions: "Transakce",
         dashboard: "Přehled",
         node: "Uzel",
+        export_users: "Exportovat uživatele",
+        no_users: "Nebyli nalezeni žádní uživatelé",
         total_capacity: "Celková kapacita",
         avg_channel_size: "Průmerná velikost kanálu",
         biggest_channel_size: "Největší velikost kanálu",
         smallest_channel_size: "Nejmenší velikost kanálu",
         number_of_channels: "Počet kanálů",
         active_channels: "Aktivní kanály",
         connect_peer: "Připojit peer",
@@ -58422,14 +58489,15 @@
         topup_hint: "Použijte ID peněženky pro dobíjení jakékoliv peněženky",
         restart_tooltip: "Restartujte server pro aplikaci změn",
         add_funds_tooltip: "Přidat prostředky do peněženky.",
         reset_defaults: "Obnovit výchozí",
         reset_defaults_tooltip: "Smazat všechna nastavení a obnovit výchozí.",
         download_backup: "Stáhnout zálohu databáze",
         name_your_wallet: "Pojmenujte svou %{name} peněženku",
+        wallet_topup_ok: "Úspěšně vytvořeny virtuální prostředky (%{amount} sats). Platby závisí na skutečných prostředcích na zdrojovém účtu.",
         paste_invoice_label: "Vložte fakturu, platební požadavek nebo lnurl kód *",
         lnbits_description: "Snadno nastavitelný a lehkotonážní, LNbits může běžet na jakémkoliv zdroji financování Lightning Network a dokonce LNbits samotné! LNbits můžete provozovat pro sebe, nebo snadno nabízet správu peněženek pro ostatní. Každá peněženka má své vlastní API klíče a není omezen počet peněženek, které můžete vytvořit. Možnost rozdělení prostředků dělá z LNbits užitečný nástroj pro správu peněz a jako vývojový nástroj. Rozšíření přidávají extra funkčnost k LNbits, takže můžete experimentovat s řadou špičkových technologií na lightning network. Vývoj rozšíření jsme učinili co nejjednodušší a jako svobodný a open-source projekt podporujeme lidi ve vývoji a zasílání vlastních rozšíření.",
         export_to_phone: "Exportovat do telefonu pomocí QR kódu",
         export_to_phone_desc: "Tento QR kód obsahuje URL vaší peněženky s plným přístupem. Můžete jej naskenovat z telefonu a otevřít peněženku odtamtud.",
         wallets: "Peněženky",
         add_wallet: "Přidat novou peněženku",
         delete_wallet: "Smazat peněženku",
@@ -58614,26 +58682,29 @@
         color_scheme: "Barevné schéma",
         extension_cost: "Toto vydání vyžaduje minimální platbu %{cost} satoshi.",
         extension_paid_sats: "Již jste zaplatili %{paid_sats} sats.",
         release_details_error: "Nelze získat podrobnosti o vydání.",
         pay_from_wallet: "Platit z peněženky",
         show_qr: "Zobrazit QR",
         retry_install: "Zkusit znovu nainstalovat",
-        new_payment: "Vytvořit novou platbu"
+        new_payment: "Vytvořit novou platbu",
+        hide_empty_wallets: "Skrýt prázdné peněženky"
     }, window.localisation.sk = {
         confirm: "Áno",
         server: "Server",
         theme: "Téma",
         funding: "Financovanie",
         users: "Používatelia",
         apps: "Aplikácie",
         channels: "Kanály",
         transactions: "Transakcie",
         dashboard: "Prehľad",
         node: "Uzol",
+        export_users: "Exportovať používateľov",
+        no_users: "Nenašli sa žiadni používatelia",
         total_capacity: "Celková kapacita",
         avg_channel_size: "Priemerná veľkosť kanálu",
         biggest_channel_size: "Najväčší kanál",
         smallest_channel_size: "Najmenší kanál",
         number_of_channels: "Počet kanálov",
         active_channels: "Aktívne kanály",
         connect_peer: "Pripojiť peer",
@@ -58650,14 +58721,15 @@
         topup_hint: "Použite ID peňaženky na doplnenie ľubovoľnej peňaženky",
         restart_tooltip: "Pre prejavenie zmien reštartujte server",
         add_funds_tooltip: "Pridať prostriedky do peňaženky.",
         reset_defaults: "Obnoviť predvolené",
         reset_defaults_tooltip: "Odstrániť všetky nastavenia a obnoviť predvolené.",
         download_backup: "Stiahnuť zálohu databázy",
         name_your_wallet: "Pomenujte vašu %{name} peňaženku",
+        wallet_topup_ok: "Úspešne vytvorené virtuálne prostriedky (%{amount} sats). Platby závisia od skutočných prostriedkov v zdroji financovania.",
         paste_invoice_label: "Vložte faktúru, platobnú požiadavku alebo lnurl kód *",
         lnbits_description: "Ľahko nastaviteľný a ľahkotonážny, LNbits môže bežať na akomkoľvek zdroji financovania Lightning Network a dokonca LNbits samotný! LNbits môžete používať pre seba, alebo ľahko ponúknuť správcovské riešenie pre iných. Každá peňaženka má svoje vlastné API kľúče a nie je limit na počet peňaženiek, ktoré môžete vytvoriť. Schopnosť rozdeľovať finančné prostriedky robí z LNbits užitočný nástroj pre správu peňazí a ako vývojový nástroj. Rozšírenia pridávajú extra funkčnosť do LNbits, takže môžete experimentovať s radou najnovších technológií na lightning sieti. Vývoj rozšírení sme urobili čo najjednoduchší a ako voľný a open-source projekt, podporujeme ľudí vývoj a odovzdávanie vlastných rozšírení.",
         export_to_phone: "Exportovať do telefónu s QR kódom",
         export_to_phone_desc: "Tento QR kód obsahuje URL vašej peňaženky s plným prístupom. Môžete ho naskenovať z vášho telefónu a otvoriť vašu peňaženku odtiaľ.",
         wallets: "Peňaženky",
         add_wallet: "Pridať novú peňaženku",
         delete_wallet: "Zmazať peňaženku",
@@ -58842,26 +58914,29 @@
         color_scheme: "Farebná schéma",
         extension_cost: "Táto verzia vyžaduje minimálnu platbu %{cost} satoshi.",
         extension_paid_sats: "Už ste zaplatili %{paid_sats} sats.",
         release_details_error: "Nepodarilo sa získať podrobnosti o vydaní.",
         pay_from_wallet: "Zaplatiť z peňaženky",
         show_qr: "Zobraziť QR",
         retry_install: "Skúste inštaláciu znova",
-        new_payment: "Vytvoriť novú platbu"
+        new_payment: "Vytvoriť novú platbu",
+        hide_empty_wallets: "Skryť prázdne peňaženky"
     }, window.localisation.kr = {
         confirm: "확인",
         server: "서버",
         theme: "테마",
         funding: "자금",
         users: "사용자",
         apps: "앱",
         channels: "채널",
         transactions: "거래 내역",
         dashboard: "현황판",
         node: "노드",
+        export_users: "사용자 내보내기",
+        no_users: "사용자가 없습니다",
         total_capacity: "총 용량",
         avg_channel_size: "평균 채널 용량",
         biggest_channel_size: "가장 큰 채널 용량",
         smallest_channel_size: "가장 작은 채널 용량",
         number_of_channels: "채널 수",
         active_channels: "활성화된 채널",
         connect_peer: "피어 연결하기",
@@ -58878,14 +58953,15 @@
         topup_hint: "자금을 추가할 지갑의 ID를 넣어주세요",
         restart_tooltip: "변경 사항을 적용하려면 서버를 재시작해야 합니다.",
         add_funds_tooltip: "지갑에 자금을 추가합니다.",
         reset_defaults: "기본 설정으로 돌아가기",
         reset_defaults_tooltip: "설정했던 내용들을 모두 지우고, 기본 설정으로 돌아갑니다.",
         download_backup: "데이터베이스 백업 다운로드",
         name_your_wallet: "사용할 %{name}지갑의 이름을 정하세요",
+        wallet_topup_ok: "성공적으로 가상 자금을 생성했습니다 (%{amount} sats). 지급은 자금 원천의 실제 자금에 따라 달라집니다.",
         paste_invoice_label: "인보이스, 결제 요청, 혹은 lnurl 코드를 붙여넣으세요 *",
         lnbits_description: "설정이 쉽고 가벼운 LNBits는 어떤 라이트닝 네트워크의 예산 자원 위에서든 돌아갈 수 있습니다, 그리고 다른 LNBits 지갑들입니다. 스스로 사용하기 위해, 또는 다른 사람들에게 수탁형 솔루션을 제공하기 위해 LNBits를 운영할 수 있습니다. 각 지갑들은 자신만의 API key를 가지며, 생성 가능한 지갑의 수에는 제한이 없습니다. 자금을 분할할 수 있는 기능으로 인해, LNBits는 자금 운영 도구로써뿐만 아니라 개발 도구로써도 유용합니다. 확장 기능들은 LNBits에 여러분들이 라이트닝 네트워크의 다양한 최신 기술들을 수행해볼 수 있게 하는 추가 기능을 제공합니다. LNBits 개발진들은 확장 기능들의 개발 또한 가능한 쉽게 만들었으며, 무료 오픈 소스 프로젝트답게 사람들이 자신만의 확장 기능들을 개발하고 제출하기를 응원합니다.",
         export_to_phone: "QR 코드를 이용해 모바일 기기로 내보내기",
         export_to_phone_desc: "이 QR 코드는 선택된 지갑의 최대 접근 권한을 가진 전체 URL을 담고 있습니다. 스캔 후, 모바일 기기에서 지갑을 열 수 있습니다.",
         wallets: "지갑",
         add_wallet: "새로운 지갑을 추가합니다",
         delete_wallet: "지갑을 삭제합니다",
@@ -59070,26 +59146,29 @@
         color_scheme: "색상 구성",
         extension_cost: "이 버전은 최소 %{cost} sats의 지불이 필요합니다.",
         extension_paid_sats: "당신은 이미 %{paid_sats} sats를 지불했습니다.",
         release_details_error: "릴리스 세부 정보를 가져올 수 없습니다.",
         pay_from_wallet: "지갑에서 결제하다",
         show_qr: "QR 보기",
         retry_install: "다시 설치하세요",
-        new_payment: "새로운 결제하기"
+        new_payment: "새로운 결제하기",
+        hide_empty_wallets: "빈 지갑 숨기기"
     }, window.localisation.fi = {
         confirm: "Kyllä",
         server: "Palvelin",
         theme: "Teema",
         funding: "Rahoitus",
         users: "Käyttäjät",
         apps: "Sovellukset",
         channels: "Kanavat",
         transactions: "Tapahtumat",
         dashboard: "Ohjauspaneeli",
         node: "Solmu",
+        export_users: "Vie käyttäjät",
+        no_users: "Käyttäjiä ei löytynyt",
         total_capacity: "Kokonaiskapasiteetti",
         avg_channel_size: "Keskimääräisen kanavan kapasiteetti",
         biggest_channel_size: "Suurimman kanavan kapasiteetti",
         smallest_channel_size: "Pienimmän kanavan kapasiteetti",
         number_of_channels: "Kanavien lukumäärä",
         active_channels: "Aktiivisia kanavia",
         connect_peer: "Yhdistä naapuriin",
@@ -59106,14 +59185,15 @@
         topup_hint: "Lisää varoja lompakkoon sen ID:n perusteella",
         restart_tooltip: "Uudelleenkäynnistä palvelu muutosten käyttöönottamiseksi",
         add_funds_tooltip: "Lisää varoja lompakkoon",
         reset_defaults: "Peruuta muutokset",
         reset_defaults_tooltip: "Poista kaikki asetusten muutokset ja palauta järjestelmän oletusasetukset.",
         download_backup: "Lataa tietokannan varmuuskopio",
         name_your_wallet: "Anna %{name}-lompakollesi nimi",
+        wallet_topup_ok: "Virtuaalisten varojen luominen onnistui (%{amount} sats). Maksut riippuvat rahoituslähteen todellisista varoista.",
         paste_invoice_label: "Liitä lasku, maksupyyntö, lnurl-koodi tai Lightning Address *",
         lnbits_description: "Kevyt ja helppokäyttöinen LNbits voi käyttää rahoituslähteinään erilaisia palveluita, ja jopa LNbits itseään! Voit käyttää sitä itsenäisesti ja helposti tarjota erilaisia Lightning-palveluita. Pystyt luomaan sillä salamaverkkolompakoita eikä niiden määrää ole rajoitettu. Jokaiselle lompakolle saat yksilölliset API-avaimet. Varojen osittaminen tekee siitä erittäin kätevän varojen hallinnassa sekä myös ohjelmistokehityksen työkalun. Laajennukset lisäävät LNbits:in toiminnallisuuksia. Näinpä voit helposti testailla useita erilaisia ja viimeisimpiä salamaverkon teknologioita. Laajennuksien kehittämisen olemme pyrkineet tekemään mahdollisimman helpoksi pitämällä LNbits:in ilmaisena OpenSource-projektina. Kannustamme kaikkia kehittämään ja jakelemaan omia laajennuksia!",
         export_to_phone: "Käytä puhelimessa lukemalla QR-koodi",
         export_to_phone_desc: "Tämä QR-koodi sisältää URL-osoitteen, jolla saa lompakkoosi täydet valtuudet. Voi lukea sen puhelimellasi ja avata sillä lompakkosi. Voit myös lisätä lompakkosi selaimella käytettäväksi PWA-sovellukseksi puhelimen aloitusruudulle. ",
         wallets: "Lompakot",
         add_wallet: "Lisää lompakko",
         delete_wallet: "Poista lompakko",
@@ -59298,15 +59378,16 @@
         color_scheme: "Väriteema",
         extension_cost: "Tämä julkaisu edellyttää vähintään %{cost} satsin maksua.",
         extension_paid_sats: "Olet jo maksanut %{paid_sats} satsia.",
         release_details_error: "Ei voi hakea julkaisun tietoja.",
         pay_from_wallet: "Maksa lompakosta",
         show_qr: "Näytä QR",
         retry_install: "Yritä asennusta uudelleen",
-        new_payment: "Tee uusi maksu"
+        new_payment: "Tee uusi maksu",
+        hide_empty_wallets: "Piilota tyhjät lompakot"
     }, Vue.use(VueI18n), window.LOCALE = "en", window.i18n = new VueI18n({
         locale: window.LOCALE,
         fallbackLocale: window.LOCALE,
         messages: window.localisation
     }), window.EventHub = new Vue, window.LNbits = {
         api: {
             request: function(e, t, n, i) {
```

### Comparing `lnbits-0.12.7/lnbits/static/css/base.css` & `lnbits-0.12.8/lnbits/static/css/base.css`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/favicon.ico` & `lnbits-0.12.8/lnbits/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/fonts/material-icons-v50.woff2` & `lnbits-0.12.8/lnbits/static/fonts/material-icons-v50.woff2`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/i18n/br.js` & `lnbits-0.12.8/lnbits/static/i18n/br.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Financiamento',
     users: 'Usuários',
     apps: 'Aplicativos',
     channels: 'Canais',
     transactions: 'Transações',
     dashboard: 'Painel de Controle',
     node: 'Nó',
+    export_users: 'Exportar Usuários',
+    no_users: 'Nenhum usuário encontrado',
     total_capacity: 'Capacidade Total',
     avg_channel_size: 'Tamanho médio do canal',
     biggest_channel_size: 'Maior Tamanho de Canal',
     smallest_channel_size: 'Tamanho Mínimo do Canal',
     number_of_channels: 'Número de Canais',
     active_channels: 'Canais Ativos',
     connect_peer: 'Conectar Par',
@@ -29,14 +31,15 @@
     topup_hint: 'Use o ID da carteira para recarregar qualquer carteira',
     restart_tooltip: 'Reinicie o servidor para que as alterações tenham efeito',
     add_funds_tooltip: 'Adicionar fundos a uma carteira.',
     reset_defaults: 'Redefinir para padrões',
     reset_defaults_tooltip: 'Apagar todas as configurações e redefinir para os padrões.',
     download_backup: 'Fazer backup do banco de dados',
     name_your_wallet: 'Nomeie sua carteira %{name}',
+    wallet_topup_ok: 'Sucesso ao criar fundos virtuais (%{amount} sats). Pagamentos dependem dos fundos reais na fonte de financiamento.',
     paste_invoice_label: 'Cole uma fatura, pedido de pagamento ou código lnurl *',
     lnbits_description: 'Fácil de configurar e leve, o LNbits pode ser executado em qualquer fonte de financiamento da Lightning Network e até mesmo o LNbits em si! Você pode executar o LNbits para si mesmo ou oferecer facilmente uma solução de custódia para outros. Cada carteira tem suas próprias chaves de API e não há limite para o número de carteiras que você pode criar. Ser capaz de particionar fundos torna o LNbits uma ferramenta útil para gerenciamento de dinheiro e como uma ferramenta de desenvolvimento. As extensões adicionam funcionalidades extras ao LNbits para que você possa experimentar uma série de tecnologias de ponta na rede lightning. Nós tornamos o desenvolvimento de extensões o mais fácil possível e, como um projeto gratuito e de código aberto, incentivamos as pessoas a desenvolver e enviar as suas próprias.',
     export_to_phone: 'Exportar para o telefone com código QR',
     export_to_phone_desc: 'Este código QR contém a URL da sua carteira com acesso total. Você pode escaneá-lo do seu telefone para abrir sua carteira a partir dele.',
     wallets: 'Carteiras',
     add_wallet: 'Adicionar nova carteira',
     delete_wallet: 'Excluir carteira',
@@ -221,9 +224,10 @@
     color_scheme: 'Esquema de Cores',
     extension_cost: 'Este lançamento requer um pagamento mínimo de %{cost} sats.',
     extension_paid_sats: 'Você já pagou %{paid_sats} sats.',
     release_details_error: 'Não é possível obter os detalhes da versão.',
     pay_from_wallet: 'Pagar com a Carteira',
     show_qr: 'Exibir QR',
     retry_install: 'Repetir Instalação',
-    new_payment: 'Efetuar Novo Pagamento'
+    new_payment: 'Efetuar Novo Pagamento',
+    hide_empty_wallets: 'Ocultar carteiras vazias'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/cn.js` & `lnbits-0.12.8/lnbits/static/i18n/cn.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: '资金',
     users: '用户',
     apps: '应用程序',
     channels: '频道',
     transactions: '交易记录',
     dashboard: '控制面板',
     node: '节点',
+    export_users: '导出用户',
+    no_users: '未找到用户',
     total_capacity: '总容量',
     avg_channel_size: '平均频道大小',
     biggest_channel_size: '最大通道大小',
     smallest_channel_size: '最小频道尺寸',
     number_of_channels: '频道数量',
     active_channels: '活跃频道',
     connect_peer: '连接对等',
@@ -29,14 +31,15 @@
     topup_hint: '使用钱包ID为任何钱包充值',
     restart_tooltip: '重新启动服务器以使更改生效',
     add_funds_tooltip: '为钱包添加资金',
     reset_defaults: '重置为默认设置',
     reset_defaults_tooltip: '删除所有设置并重置为默认设置',
     download_backup: '下载数据库备份',
     name_your_wallet: '给你的 %{name}钱包起个名字',
+    wallet_topup_ok: '成功创建虚拟资金（%{amount} sats）。付款取决于资金来源的实际资金。',
     paste_invoice_label: '粘贴发票，付款请求或lnurl*',
     lnbits_description: 'LNbits 设置简单、轻量级，可以在任何闪电网络的资金来源上运行，甚至可以在LNbits自身上运行！您可以为自己运行LNbits，或者轻松为他人提供托管解决方案。每个钱包都有自己的 API 密钥，你可以创建的钱包数量没有限制。能够把资金分开管理使 LNbits 成为一款有用的资金管理和开发工具。扩展程序增加了 LNbits 的额外功能，所以你可以在闪电网络上尝试各种尖端技术。我们已经尽可能简化了开发扩展程序的过程，作为一个免费和开源的项目，我们鼓励人们开发并提交自己的扩展程序。',
     export_to_phone: '通过二维码导出到手机',
     export_to_phone_desc: '这个二维码包含您钱包的URL。您可以使用手机扫描的方式打开您的钱包。',
     wallets: '钱包',
     add_wallet: '添加新钱包',
     delete_wallet: '删除钱包',
@@ -221,9 +224,10 @@
     color_scheme: '配色方案',
     extension_cost: '此版本需要支付最低 %{cost} sats。',
     extension_paid_sats: '您已经支付了%{paid_sats} sats。',
     release_details_error: '无法获取发布详情。',
     pay_from_wallet: '从钱包支付',
     show_qr: '显示QR码',
     retry_install: '重试安装',
-    new_payment: '创建新支付'
+    new_payment: '创建新支付',
+    hide_empty_wallets: '隐藏空钱包'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/cs.js` & `lnbits-0.12.8/lnbits/static/i18n/cs.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Financování',
     users: 'Uživatelé',
     apps: 'Aplikace',
     channels: 'Kanály',
     transactions: 'Transakce',
     dashboard: 'Přehled',
     node: 'Uzel',
+    export_users: 'Exportovat uživatele',
+    no_users: 'Nebyli nalezeni žádní uživatelé',
     total_capacity: 'Celková kapacita',
     avg_channel_size: 'Průmerná velikost kanálu',
     biggest_channel_size: 'Největší velikost kanálu',
     smallest_channel_size: 'Nejmenší velikost kanálu',
     number_of_channels: 'Počet kanálů',
     active_channels: 'Aktivní kanály',
     connect_peer: 'Připojit peer',
@@ -29,14 +31,15 @@
     topup_hint: 'Použijte ID peněženky pro dobíjení jakékoliv peněženky',
     restart_tooltip: 'Restartujte server pro aplikaci změn',
     add_funds_tooltip: 'Přidat prostředky do peněženky.',
     reset_defaults: 'Obnovit výchozí',
     reset_defaults_tooltip: 'Smazat všechna nastavení a obnovit výchozí.',
     download_backup: 'Stáhnout zálohu databáze',
     name_your_wallet: 'Pojmenujte svou %{name} peněženku',
+    wallet_topup_ok: 'Úspěšně vytvořeny virtuální prostředky (%{amount} sats). Platby závisí na skutečných prostředcích na zdrojovém účtu.',
     paste_invoice_label: 'Vložte fakturu, platební požadavek nebo lnurl kód *',
     lnbits_description: 'Snadno nastavitelný a lehkotonážní, LNbits může běžet na jakémkoliv zdroji financování Lightning Network a dokonce LNbits samotné! LNbits můžete provozovat pro sebe, nebo snadno nabízet správu peněženek pro ostatní. Každá peněženka má své vlastní API klíče a není omezen počet peněženek, které můžete vytvořit. Možnost rozdělení prostředků dělá z LNbits užitečný nástroj pro správu peněz a jako vývojový nástroj. Rozšíření přidávají extra funkčnost k LNbits, takže můžete experimentovat s řadou špičkových technologií na lightning network. Vývoj rozšíření jsme učinili co nejjednodušší a jako svobodný a open-source projekt podporujeme lidi ve vývoji a zasílání vlastních rozšíření.',
     export_to_phone: 'Exportovat do telefonu pomocí QR kódu',
     export_to_phone_desc: 'Tento QR kód obsahuje URL vaší peněženky s plným přístupem. Můžete jej naskenovat z telefonu a otevřít peněženku odtamtud.',
     wallets: 'Peněženky',
     add_wallet: 'Přidat novou peněženku',
     delete_wallet: 'Smazat peněženku',
@@ -221,9 +224,10 @@
     color_scheme: 'Barevné schéma',
     extension_cost: 'Toto vydání vyžaduje minimální platbu %{cost} satoshi.',
     extension_paid_sats: 'Již jste zaplatili %{paid_sats} sats.',
     release_details_error: 'Nelze získat podrobnosti o vydání.',
     pay_from_wallet: 'Platit z peněženky',
     show_qr: 'Zobrazit QR',
     retry_install: 'Zkusit znovu nainstalovat',
-    new_payment: 'Vytvořit novou platbu'
+    new_payment: 'Vytvořit novou platbu',
+    hide_empty_wallets: 'Skrýt prázdné peněženky'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/de.js` & `lnbits-0.12.8/lnbits/static/i18n/de.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Funding',
     users: 'Benutzer',
     apps: 'Apps',
     channels: 'Kanäle',
     transactions: 'Transaktionen',
     dashboard: 'Armaturenbrett',
     node: 'Knoten',
+    export_users: 'Benutzer exportieren',
+    no_users: 'Keine Benutzer gefunden',
     total_capacity: 'Gesamtkapazität',
     avg_channel_size: 'Durchschn. Kanalgröße',
     biggest_channel_size: 'Größte Kanalgröße',
     smallest_channel_size: 'Kleinste Kanalgröße',
     number_of_channels: 'Anzahl der Kanäle',
     active_channels: 'Aktive Kanäle',
     connect_peer: 'Peer verbinden',
@@ -29,14 +31,15 @@
     topup_hint: 'Nutze die Wallet-ID, um eine beliebige Wallet aufzuladen',
     restart_tooltip: 'Starte den Server neu, um die Änderungen zu übernehmen',
     add_funds_tooltip: 'Füge Geld zu einer Wallet hinzu.',
     reset_defaults: 'Zurücksetzen',
     reset_defaults_tooltip: 'Alle Einstellungen auf die Standardeinstellungen zurücksetzen.',
     download_backup: 'Datenbank-Backup herunterladen',
     name_your_wallet: 'Vergib deiner %{name} Wallet einen Namen',
+    wallet_topup_ok: 'Erfolg beim Erstellen von virtuellen Mitteln (%{amount} Satoshis). Zahlungen hängen von den tatsächlichen Mitteln der Finanzierungsquelle ab.',
     paste_invoice_label: 'Füge eine Rechnung, Zahlungsanforderung oder LNURL ein *',
     lnbits_description: 'Einfach zu installieren und kompakt, LNbits kann auf jeder Funding-Quelle im Lightning Netzwerk aufsetzen und sogar LNbits selbst! Du kannst LNbits für dich selbst betreiben oder anderen die Verwaltung durch dich anbieten. Jede Wallet hat ihre eigenen API-Schlüssel und die Anzahl der Wallets ist unbegrenzt. Die Möglichkeit, Gelder auf verschiedene Accounts mit unterschiedlicher Logik aufteilen zu können macht LNbits zu einem nützlichen Werkzeug für deine Buchhaltung - aber auch als Entwicklungswerkzeug. Erweiterungen bereichern LNbits Accounts um zusätzliche Funktionalität, so dass du mit einer Reihe von neuartigen Technologien auf dem Lightning-Netzwerk experimentieren kannst. Wir haben es so einfach wie möglich gemacht, Erweiterungen zu entwickeln, und als freies und Open-Source-Projekt möchten wir Menschen ermutigen, sich selbst hieran zu versuchen und gemeinsam mit uns neue Funktionalitäten zu entwickeln.',
     export_to_phone: 'Auf dem Telefon öffnen',
     export_to_phone_desc: 'Dieser QR-Code beinhaltet vollständige Rechte auf deine Wallet. Du kannst den QR-Code mit Deinem Telefon scannen, um deine Wallet dort zu öffnen.',
     wallets: 'Wallets',
     add_wallet: 'Wallet hinzufügen',
     delete_wallet: 'Wallet löschen',
@@ -221,9 +224,10 @@
     color_scheme: 'Farbschema',
     extension_cost: 'Diese Version erfordert eine Zahlung von mindestens %{cost} Sats.',
     extension_paid_sats: 'Sie haben bereits %{paid_sats} Sats bezahlt.',
     release_details_error: 'Kann die Details zur Veröffentlichung nicht abrufen.',
     pay_from_wallet: 'Zahlen aus dem Geldbeutel',
     show_qr: 'QR anzeigen',
     retry_install: 'Installieren erneut versuchen',
-    new_payment: 'Neue Zahlung vornehmen'
+    new_payment: 'Neue Zahlung vornehmen',
+    hide_empty_wallets: 'Leere Geldbörsen verbergen'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/en.js` & `lnbits-0.12.8/lnbits/static/i18n/en.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -107,14 +107,15 @@
     repository: 'Repository',
     confirm_continue: 'Are you sure you want to continue?',
     manage_extension_details: 'Install/uninstall extension',
     install: 'Install',
     uninstall: 'Uninstall',
     drop_db: 'Remove Data',
     enable: 'Enable',
+    pay_to_enable: 'Pay To Enable',
     enable_extension_details: 'Enable extension for current user',
     disable: 'Disable',
     installed: 'Installed',
     activated: 'Activated',
     deactivated: 'Deactivated',
     release_notes: 'Release Notes',
     activate_extension_details: 'Make extension available/unavailable for users',
@@ -130,14 +131,15 @@
     uninstall_confirm: 'Yes, Uninstall',
     extension_db_drop_info: 'All data for the extension will be permanently deleted. There is no way to undo this operation!',
     extension_db_drop_warning: 'You are about to remove all data for the extension. Please type the extension name to continue:',
     extension_min_lnbits_version: 'This release requires at least LNbits version',
     payment_hash: 'Payment Hash',
     fee: 'Fee',
     amount: 'Amount',
+    amount_sats: 'Amount (sats)',
     tag: 'Tag',
     unit: 'Unit',
     description: 'Description',
     expiry: 'Expiry',
     webhook: 'Webhook',
     payment_proof: 'Payment Proof',
     update_available: 'Update %{version} available!',
@@ -222,12 +224,19 @@
     look_and_feel: 'Look and Feel',
     language: 'Language',
     color_scheme: 'Color Scheme',
     extension_cost: 'This release requires a payment of minimum %{cost} sats.',
     extension_paid_sats: 'You have already paid %{paid_sats} sats.',
     release_details_error: 'Cannot get the release details.',
     pay_from_wallet: 'Pay from Wallet',
+    wallet_required: 'Wallet *',
     show_qr: 'Show QR',
     retry_install: 'Retry Install',
     new_payment: 'Make New Payment',
-    hide_empty_wallets: 'Hide empty wallets'
+    update_payment: 'Update Payment',
+    already_paid_question: 'Have you already paid?',
+    sell: 'Sell',
+    sell_require: 'Ask payment to enable extension',
+    sell_info: 'The %{name} extension requires a payment of minimum %{amount} sats to enable.',
+    hide_empty_wallets: 'Hide empty wallets',
+    recheck: 'Recheck'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/es.js` & `lnbits-0.12.8/lnbits/static/i18n/es.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Financiación',
     users: 'Usuarios',
     apps: 'Aplicaciones',
     channels: 'Canales',
     transactions: 'Transacciones',
     dashboard: 'Tablero de instrumentos',
     node: 'Nodo',
+    export_users: 'Exportar Usuarios',
+    no_users: 'No se encontraron usuarios',
     total_capacity: 'Capacidad Total',
     avg_channel_size: 'Tamaño Medio del Canal',
     biggest_channel_size: 'Tamaño del Canal Más Grande',
     smallest_channel_size: 'Tamaño de canal más pequeño',
     number_of_channels: 'Número de canales',
     active_channels: 'Canales activos',
     connect_peer: 'Conectar Par',
@@ -29,14 +31,15 @@
     topup_hint: 'Utilice el ID de billetera para recargar cualquier billetera',
     restart_tooltip: 'Reinicie el servidor para aplicar los cambios',
     add_funds_tooltip: 'Agregue fondos a una billetera.',
     reset_defaults: 'Restablecer',
     reset_defaults_tooltip: 'Borrar todas las configuraciones y restablecer a los valores predeterminados.',
     download_backup: 'Descargar copia de seguridad de la base de datos',
     name_your_wallet: 'Nombre de su billetera %{name}',
+    wallet_topup_ok: 'Éxito creando fondos virtuales (%{amount} sats). Los pagos dependen de los fondos reales en la fuente de financiación.',
     paste_invoice_label: 'Pegue la factura aquí',
     lnbits_description: 'Fácil de instalar y liviano, LNbits puede ejecutarse en cualquier fuente de financiación de la red Lightning y hasta LNbits mismo! Puede ejecutar LNbits para usted mismo o ofrecer una solución competente a otros. Cada billetera tiene su propia clave API y no hay límite para la cantidad de billeteras que puede crear. La capacidad de particionar fondos hace de LNbits una herramienta útil para la administración de fondos y como herramienta de desarrollo. Las extensiones agregan funcionalidad adicional a LNbits, por lo que puede experimentar con una variedad de tecnologías de vanguardia en la red Lightning. Lo hemos hecho lo más simple posible para desarrollar extensiones y, como un proyecto gratuito y de código abierto, animamos a las personas a que se desarrollen a sí mismas y envíen sus propios contribuciones.',
     export_to_phone: 'Exportar a teléfono con código QR',
     export_to_phone_desc: 'Este código QR contiene su URL de billetera con acceso completo. Puede escanearlo desde su teléfono para abrir su billetera allí.',
     wallets: 'Billeteras',
     add_wallet: 'Agregar nueva billetera',
     delete_wallet: 'Eliminar billetera',
@@ -221,9 +224,10 @@
     color_scheme: 'Esquema de colores',
     extension_cost: 'Esta versión requiere un pago mínimo de %{cost} sats.',
     extension_paid_sats: 'Ya has pagado %{paid_sats} sats.',
     release_details_error: 'No se pueden obtener los detalles de la versión.',
     pay_from_wallet: 'Pagar desde la billetera',
     show_qr: 'Mostrar QR',
     retry_install: 'Reintentar Instalación',
-    new_payment: 'Realizar nuevo pago'
+    new_payment: 'Realizar nuevo pago',
+    hide_empty_wallets: 'Ocultar billeteras vacías'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/fi.js` & `lnbits-0.12.8/lnbits/static/i18n/fi.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Rahoitus',
     users: 'Käyttäjät',
     apps: 'Sovellukset',
     channels: 'Kanavat',
     transactions: 'Tapahtumat',
     dashboard: 'Ohjauspaneeli',
     node: 'Solmu',
+    export_users: 'Vie käyttäjät',
+    no_users: 'Käyttäjiä ei löytynyt',
     total_capacity: 'Kokonaiskapasiteetti',
     avg_channel_size: 'Keskimääräisen kanavan kapasiteetti',
     biggest_channel_size: 'Suurimman kanavan kapasiteetti',
     smallest_channel_size: 'Pienimmän kanavan kapasiteetti',
     number_of_channels: 'Kanavien lukumäärä',
     active_channels: 'Aktiivisia kanavia',
     connect_peer: 'Yhdistä naapuriin',
@@ -29,14 +31,15 @@
     topup_hint: 'Lisää varoja lompakkoon sen ID:n perusteella',
     restart_tooltip: 'Uudelleenkäynnistä palvelu muutosten käyttöönottamiseksi',
     add_funds_tooltip: 'Lisää varoja lompakkoon',
     reset_defaults: 'Peruuta muutokset',
     reset_defaults_tooltip: 'Poista kaikki asetusten muutokset ja palauta järjestelmän oletusasetukset.',
     download_backup: 'Lataa tietokannan varmuuskopio',
     name_your_wallet: 'Anna %{name}-lompakollesi nimi',
+    wallet_topup_ok: 'Virtuaalisten varojen luominen onnistui (%{amount} sats). Maksut riippuvat rahoituslähteen todellisista varoista.',
     paste_invoice_label: 'Liitä lasku, maksupyyntö, lnurl-koodi tai Lightning Address *',
     lnbits_description: 'Kevyt ja helppokäyttöinen LNbits voi käyttää rahoituslähteinään erilaisia palveluita, ja jopa LNbits itseään! Voit käyttää sitä itsenäisesti ja helposti tarjota erilaisia Lightning-palveluita. Pystyt luomaan sillä salamaverkkolompakoita eikä niiden määrää ole rajoitettu. Jokaiselle lompakolle saat yksilölliset API-avaimet. Varojen osittaminen tekee siitä erittäin kätevän varojen hallinnassa sekä myös ohjelmistokehityksen työkalun. Laajennukset lisäävät LNbits:in toiminnallisuuksia. Näinpä voit helposti testailla useita erilaisia ja viimeisimpiä salamaverkon teknologioita. Laajennuksien kehittämisen olemme pyrkineet tekemään mahdollisimman helpoksi pitämällä LNbits:in ilmaisena OpenSource-projektina. Kannustamme kaikkia kehittämään ja jakelemaan omia laajennuksia!',
     export_to_phone: 'Käytä puhelimessa lukemalla QR-koodi',
     export_to_phone_desc: 'Tämä QR-koodi sisältää URL-osoitteen, jolla saa lompakkoosi täydet valtuudet. Voi lukea sen puhelimellasi ja avata sillä lompakkosi. Voit myös lisätä lompakkosi selaimella käytettäväksi PWA-sovellukseksi puhelimen aloitusruudulle. ',
     wallets: 'Lompakot',
     add_wallet: 'Lisää lompakko',
     delete_wallet: 'Poista lompakko',
@@ -221,9 +224,10 @@
     color_scheme: 'Väriteema',
     extension_cost: 'Tämä julkaisu edellyttää vähintään %{cost} satsin maksua.',
     extension_paid_sats: 'Olet jo maksanut %{paid_sats} satsia.',
     release_details_error: 'Ei voi hakea julkaisun tietoja.',
     pay_from_wallet: 'Maksa lompakosta',
     show_qr: 'Näytä QR',
     retry_install: 'Yritä asennusta uudelleen',
-    new_payment: 'Tee uusi maksu'
+    new_payment: 'Tee uusi maksu',
+    hide_empty_wallets: 'Piilota tyhjät lompakot'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/fr.js` & `lnbits-0.12.8/lnbits/static/i18n/fr.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Financement',
     users: 'Utilisateurs',
     apps: 'Applications',
     channels: 'Canaux',
     transactions: 'Transactions',
     dashboard: 'Tableau de bord',
     node: 'Noeud',
+    export_users: 'Exporter les utilisateurs',
+    no_users: 'Aucun utilisateur trouvé',
     total_capacity: 'Capacité totale',
     avg_channel_size: 'Taille moyenne du canal',
     biggest_channel_size: 'Taille de canal maximale',
     smallest_channel_size: 'Taille de canal la plus petite',
     number_of_channels: 'Nombre de canaux',
     active_channels: 'Canaux actifs',
     connect_peer: 'Connecter un pair',
@@ -29,14 +31,15 @@
     topup_hint: "Utilisez l'ID du portefeuille pour recharger n'importe quel portefeuille",
     restart_tooltip: 'Redémarrez le serveur pour que les changements prennent effet',
     add_funds_tooltip: 'Ajouter des fonds à un portefeuille.',
     reset_defaults: 'Réinitialiser aux valeurs par défaut',
     reset_defaults_tooltip: 'Supprimer tous les paramètres et les réinitialiser aux valeurs par défaut.',
     download_backup: 'Télécharger la sauvegarde de la base de données',
     name_your_wallet: 'Nommez votre portefeuille %{name}',
+    wallet_topup_ok: 'Succès de la création de fonds virtuels (%{amount} sats). Les paiements dépendent des fonds réels sur la source de financement.',
     paste_invoice_label: 'Coller une facture, une demande de paiement ou un code lnurl *',
     lnbits_description: "Facile à installer et léger, LNbits peut fonctionner sur n'importe quelle source de financement du réseau Lightning et même LNbits lui-même! Vous pouvez exécuter LNbits pour vous-même ou offrir facilement une solution de gardien pour les autres. Chaque portefeuille a ses propres clés API et il n'y a pas de limite au nombre de portefeuilles que vous pouvez créer. La capacité de partitionner les fonds rend LNbits un outil utile pour la gestion de l'argent et comme outil de développement. Les extensions ajoutent une fonctionnalité supplémentaire à LNbits afin que vous puissiez expérimenter une gamme de technologies de pointe sur le réseau Lightning. Nous avons rendu le développement d'extensions aussi simple que possible et, en tant que projet gratuit et open source, nous encourageons les gens à développer et à soumettre les leurs.",
     export_to_phone: 'Exporter vers le téléphone avec un code QR',
     export_to_phone_desc: "Ce code QR contient l'URL de votre portefeuille avec un accès complet. Vous pouvez le scanner depuis votre téléphone pour ouvrir votre portefeuille depuis là-bas.",
     wallets: 'Portefeuilles',
     add_wallet: 'Ajouter un nouveau portefeuille',
     delete_wallet: 'Supprimer le portefeuille',
@@ -221,9 +224,10 @@
     color_scheme: 'Schéma de couleurs',
     extension_cost: 'Cette version nécessite un paiement minimum de %{cost} sats.',
     extension_paid_sats: 'Vous avez déjà payé %{paid_sats} sats.',
     release_details_error: "Impossible d'obtenir les détails de la version.",
     pay_from_wallet: 'Payer depuis le portefeuille',
     show_qr: 'Afficher le QR',
     retry_install: "Réessayer l'installation",
-    new_payment: 'Effectuer un nouveau paiement'
+    new_payment: 'Effectuer un nouveau paiement',
+    hide_empty_wallets: 'Masquer les portefeuilles vides'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/it.js` & `lnbits-0.12.8/lnbits/static/i18n/it.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Funding',
     users: 'Utenti',
     apps: 'Applicazioni',
     channels: 'Canali',
     transactions: 'Transazioni',
     dashboard: 'Pannello di controllo',
     node: 'Interruttore',
+    export_users: 'Esporta utenti',
+    no_users: 'Nessun utente trovato',
     total_capacity: 'Capacità Totale',
     avg_channel_size: 'Dimensione media del canale',
     biggest_channel_size: 'Dimensione del canale più grande',
     smallest_channel_size: 'Dimensione Più Piccola del Canale',
     number_of_channels: 'Numero di Canali',
     active_channels: 'Canali Attivi',
     connect_peer: 'Connetti Peer',
@@ -29,14 +31,15 @@
     topup_hint: "Usa l'ID del portafoglio per ricaricare qualsiasi portafoglio",
     restart_tooltip: 'Riavvia il server affinché le modifiche abbiano effetto',
     add_funds_tooltip: 'Aggiungere fondi a un portafoglio',
     reset_defaults: 'Ripristina le impostazioni predefinite',
     reset_defaults_tooltip: 'Cancella tutte le impostazioni e ripristina i valori predefiniti',
     download_backup: 'Scarica il backup del database',
     name_your_wallet: 'Dai un nome al tuo portafoglio %{name}',
+    wallet_topup_ok: 'Operazione riuscita nella creazione di fondi virtuali (%{amount} sats). I pagamenti dipendono dai fondi effettivi sulla fonte di finanziamento.',
     paste_invoice_label: 'Incolla una fattura, una richiesta di pagamento o un codice lnurl *',
     lnbits_description: "Leggero e facile da configurare, LNbits può funzionare su qualsiasi fonte di finanziamento Lightning Network e persino LNbits stesso! Potete gestire LNbits per conto vostro o offrire facilmente una soluzione di custodia per altri. Ogni portafoglio ha le proprie chiavi API e non c'è limite al numero di portafogli che si possono creare. La possibilità di suddividere i fondi rende LNbits uno strumento utile per la gestione del denaro e come strumento di sviluppo. Le estensioni aggiungono ulteriori funzionalità a LNbits, consentendo di sperimentare una serie di tecnologie all'avanguardia sulla rete Lightning. Abbiamo reso lo sviluppo delle estensioni il più semplice possibile e, in quanto progetto libero e open-source, incoraggiamo le persone a sviluppare e inviare le proprie",
     export_to_phone: 'Esportazione su telefono con codice QR',
     export_to_phone_desc: "Questo codice QR contiene l'URL del portafoglio con accesso da amministratore. È possibile scansionarlo dal telefono per aprire il portafoglio da lì.",
     wallets: 'Portafogli',
     add_wallet: 'Aggiungi un nuovo portafoglio',
     delete_wallet: 'Elimina il portafoglio',
@@ -221,9 +224,10 @@
     color_scheme: 'Schema dei colori',
     extension_cost: 'Questa versione richiede un pagamento minimo di %{cost} satoshi.',
     extension_paid_sats: 'Hai già pagato %{paid_sats} sats.',
     release_details_error: 'Impossibile ottenere i dettagli della versione.',
     pay_from_wallet: 'Paga dal Portafoglio',
     show_qr: 'Mostra QR',
     retry_install: 'Riprova Installazione',
-    new_payment: 'Effettua Nuovo Pagamento'
+    new_payment: 'Effettua Nuovo Pagamento',
+    hide_empty_wallets: 'Nascondi portafogli vuoti'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/jp.js` & `lnbits-0.12.8/lnbits/static/i18n/jp.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: '資金調達',
     users: 'ユーザー',
     apps: 'アプリ',
     channels: 'チャンネル',
     transactions: 'トランザクション',
     dashboard: 'ダッシュボード',
     node: 'ノード',
+    export_users: 'ユーザーのエクスポート',
+    no_users: 'ユーザーが見つかりません',
     total_capacity: '合計容量',
     avg_channel_size: '平均チャンネルサイズ',
     biggest_channel_size: '最大チャネルサイズ',
     smallest_channel_size: '最小チャンネルサイズ',
     number_of_channels: 'チャンネル数',
     active_channels: 'アクティブチャンネル',
     connect_peer: 'ピアを接続',
@@ -29,14 +31,15 @@
     topup_hint: 'ウォレットIDを使用して、任意のウォレットをトップアップできます',
     restart_tooltip: 'サーバーを再起動して変更を適用します',
     add_funds_tooltip: 'ウォレットに資金を追加します。',
     reset_defaults: 'リセット',
     reset_defaults_tooltip: 'すべての設定を削除してデフォルトに戻します。',
     download_backup: 'データベースのバックアップをダウンロードする',
     name_your_wallet: 'あなたのウォレットの名前 %{name}',
+    wallet_topup_ok: '仮想資金の作成に成功しました（%{amount} sats）。支払いは資金ソースの実際の資金に依存します。',
     paste_invoice_label: '請求書を貼り付けてください',
     lnbits_description: '簡単にインストールでき、軽量なLNbitsは、あらゆるライトニングネットワークの資金源と、LNbits自身でさえも実行できます！LNbitsを個人で実行することも、他人に対してカストディアンソリューションをで実行できます！ LNbitsを自分で実行することも、他の人に優れたソリューションを提供することもできます。各ウォレットには独自のAPIキーがあり、作成できるウォレットの数に制限はありません。資金を分割する機能は、LNbitsを資金管理ツールとして使用したり、開発ツールとして使用したりするための便利なツールです。拡張機能は、LNbitsに追加の機能を追加します。そのため、LNbitsは最先端の技術をネットワークLightningで試すことができます。拡張機能を開発するのは簡単で、無料でオープンソースのプロジェクトであるため、人々が自分で開発し、自分の貢献を送信することを奨励しています。',
     export_to_phone: '電話にエクスポート',
     export_to_phone_desc: 'ウォレットを電話にエクスポートすると、ウォレットを削除する前にウォレットを復元できます。ウォレットを削除すると、ウォレットの秘密鍵が削除され、ウォレットを復元することはできません。',
     wallets: 'ウォレット',
     add_wallet: 'ウォレットを追加',
     delete_wallet: 'ウォレットを削除',
@@ -221,9 +224,10 @@
     color_scheme: 'カラースキーム',
     extension_cost: 'このリリースには最低 %{cost} サトシの支払いが必要です。',
     extension_paid_sats: 'すでに%{paid_sats} satsを支払いました。',
     release_details_error: 'リリースの詳細を取得できません。',
     pay_from_wallet: 'ウォレットから支払う',
     show_qr: 'QRを表示',
     retry_install: '再試行インストール',
-    new_payment: '新しい支払いを作成する'
+    new_payment: '新しい支払いを作成する',
+    hide_empty_wallets: '空のウォレットを非表示にする'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/kr.js` & `lnbits-0.12.8/lnbits/static/i18n/kr.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: '자금',
     users: '사용자',
     apps: '앱',
     channels: '채널',
     transactions: '거래 내역',
     dashboard: '현황판',
     node: '노드',
+    export_users: '사용자 내보내기',
+    no_users: '사용자가 없습니다',
     total_capacity: '총 용량',
     avg_channel_size: '평균 채널 용량',
     biggest_channel_size: '가장 큰 채널 용량',
     smallest_channel_size: '가장 작은 채널 용량',
     number_of_channels: '채널 수',
     active_channels: '활성화된 채널',
     connect_peer: '피어 연결하기',
@@ -29,14 +31,15 @@
     topup_hint: '자금을 추가할 지갑의 ID를 넣어주세요',
     restart_tooltip: '변경 사항을 적용하려면 서버를 재시작해야 합니다.',
     add_funds_tooltip: '지갑에 자금을 추가합니다.',
     reset_defaults: '기본 설정으로 돌아가기',
     reset_defaults_tooltip: '설정했던 내용들을 모두 지우고, 기본 설정으로 돌아갑니다.',
     download_backup: '데이터베이스 백업 다운로드',
     name_your_wallet: '사용할 %{name}지갑의 이름을 정하세요',
+    wallet_topup_ok: '성공적으로 가상 자금을 생성했습니다 (%{amount} sats). 지급은 자금 원천의 실제 자금에 따라 달라집니다.',
     paste_invoice_label: '인보이스, 결제 요청, 혹은 lnurl 코드를 붙여넣으세요 *',
     lnbits_description: '설정이 쉽고 가벼운 LNBits는 어떤 라이트닝 네트워크의 예산 자원 위에서든 돌아갈 수 있습니다, 그리고 다른 LNBits 지갑들입니다. 스스로 사용하기 위해, 또는 다른 사람들에게 수탁형 솔루션을 제공하기 위해 LNBits를 운영할 수 있습니다. 각 지갑들은 자신만의 API key를 가지며, 생성 가능한 지갑의 수에는 제한이 없습니다. 자금을 분할할 수 있는 기능으로 인해, LNBits는 자금 운영 도구로써뿐만 아니라 개발 도구로써도 유용합니다. 확장 기능들은 LNBits에 여러분들이 라이트닝 네트워크의 다양한 최신 기술들을 수행해볼 수 있게 하는 추가 기능을 제공합니다. LNBits 개발진들은 확장 기능들의 개발 또한 가능한 쉽게 만들었으며, 무료 오픈 소스 프로젝트답게 사람들이 자신만의 확장 기능들을 개발하고 제출하기를 응원합니다.',
     export_to_phone: 'QR 코드를 이용해 모바일 기기로 내보내기',
     export_to_phone_desc: '이 QR 코드는 선택된 지갑의 최대 접근 권한을 가진 전체 URL을 담고 있습니다. 스캔 후, 모바일 기기에서 지갑을 열 수 있습니다.',
     wallets: '지갑',
     add_wallet: '새로운 지갑을 추가합니다',
     delete_wallet: '지갑을 삭제합니다',
@@ -221,9 +224,10 @@
     color_scheme: '색상 구성',
     extension_cost: '이 버전은 최소 %{cost} sats의 지불이 필요합니다.',
     extension_paid_sats: '당신은 이미 %{paid_sats} sats를 지불했습니다.',
     release_details_error: '릴리스 세부 정보를 가져올 수 없습니다.',
     pay_from_wallet: '지갑에서 결제하다',
     show_qr: 'QR 보기',
     retry_install: '다시 설치하세요',
-    new_payment: '새로운 결제하기'
+    new_payment: '새로운 결제하기',
+    hide_empty_wallets: '빈 지갑 숨기기'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/nl.js` & `lnbits-0.12.8/lnbits/static/i18n/nl.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Financiering',
     users: 'Gebruikers',
     apps: 'Apps',
     channels: 'Kanalen',
     transactions: 'Transacties',
     dashboard: 'Dashboard',
     node: 'Knooppunt',
+    export_users: 'Gebruikers exporteren',
+    no_users: 'Geen gebruikers gevonden',
     total_capacity: 'Totale capaciteit',
     avg_channel_size: 'Gem. Kanaalgrootte',
     biggest_channel_size: 'Grootste Kanaalgrootte',
     smallest_channel_size: 'Kleinste Kanaalgrootte',
     number_of_channels: 'Aantal kanalen',
     active_channels: 'Actieve Kanalen',
     connect_peer: 'Peer verbinden',
@@ -29,14 +31,15 @@
     topup_hint: 'Gebruik de portemonnee-ID om elke portemonnee bij te vullen',
     restart_tooltip: 'Start de server opnieuw op zodat wijzigingen van kracht worden',
     add_funds_tooltip: 'Voeg geld toe aan een portemonnee.',
     reset_defaults: 'Standaardinstellingen herstellen',
     reset_defaults_tooltip: 'Wis alle instellingen en herstel de standaardinstellingen.',
     download_backup: 'Databaseback-up downloaden',
     name_your_wallet: 'Geef je %{name} portemonnee een naam',
+    wallet_topup_ok: 'Succes met het aanmaken van virtuele fondsen (%{amount} sats). Betalingen zijn afhankelijk van de werkelijke fondsen op de financieringsbron.',
     paste_invoice_label: 'Plak een factuur, betalingsverzoek of lnurl-code*',
     lnbits_description: 'Gemakkelijk in te stellen en lichtgewicht, LNbits kan op elke lightning-netwerkfinancieringsbron draaien en zelfs LNbits zelf! U kunt LNbits voor uzelf laten draaien of gemakkelijk een bewaardersoplossing voor anderen bieden. Elke portemonnee heeft zijn eigen API-sleutels en er is geen limiet aan het aantal portemonnees dat u kunt maken. Het kunnen partitioneren van fondsen maakt LNbits een nuttige tool voor geldbeheer en als ontwikkelingstool. Extensies voegen extra functionaliteit toe aan LNbits, zodat u kunt experimenteren met een reeks toonaangevende technologieën op het bliksemschichtnetwerk. We hebben het ontwikkelen van extensies zo eenvoudig mogelijk gemaakt en als een gratis en opensource-project moedigen we mensen aan om hun eigen ontwikkelingen in te dienen.',
     export_to_phone: 'Exporteren naar telefoon met QR-code',
     export_to_phone_desc: 'Deze QR-code bevat uw portemonnee-URL met volledige toegang. U kunt het vanaf uw telefoon scannen om uw portemonnee van daaruit te openen.',
     wallets: 'Portemonnees',
     add_wallet: 'Een nieuwe portemonnee toevoegen',
     delete_wallet: 'Portemonnee verwijderen',
@@ -221,9 +224,10 @@
     color_scheme: 'Kleurenschema',
     extension_cost: 'Deze release vereist een betaling van minimaal %{cost} sats.',
     extension_paid_sats: 'U heeft al %{paid_sats} sats betaald.',
     release_details_error: 'Kan de gegevens van de release niet ophalen.',
     pay_from_wallet: 'Betalen vanuit Portemonnee',
     show_qr: 'Toon QR',
     retry_install: 'Opnieuw installeren',
-    new_payment: 'Nieuwe betaling maken'
+    new_payment: 'Nieuwe betaling maken',
+    hide_empty_wallets: 'Verberg lege portemonnees'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/pi.js` & `lnbits-0.12.8/lnbits/static/i18n/pi.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Funding',
     users: 'Buccaneers',
     apps: 'Arrrrplications',
     channels: 'Channels',
     transactions: 'Pirate Transactions and loot',
     dashboard: 'Arrr-board',
     node: 'Node',
+    export_users: 'Export Mateys',
+    no_users: 'No swabbies found',
     total_capacity: 'Total Capacity',
     avg_channel_size: 'Avg. Channel Size',
     biggest_channel_size: 'Largest Bilge Size',
     smallest_channel_size: 'Smallest Channel Size',
     number_of_channels: "Nummer o' Channels",
     active_channels: 'Active Channels',
     connect_peer: 'Connect Peer',
@@ -29,14 +31,15 @@
     topup_hint: 'Use the chest ID to top up any chest',
     restart_tooltip: 'Restart the Cap`n for changes to take effect, arr!',
     add_funds_tooltip: 'Add doubloons to a chest and make it heavier',
     reset_defaults: 'Reset to Davy Jones Locker',
     reset_defaults_tooltip: 'Scuttle all settings and reset to Davy Jones Locker. Aye, start anew!',
     download_backup: 'Download database booty',
     name_your_wallet: 'Name yer %{name} treasure chest',
+    wallet_topup_ok: "Success creatin' virtual funds (%{amount} sats). Payments depend on actual funds on funding source.",
     paste_invoice_label: 'Paste a booty, payment request or lnurl code, matey!',
     lnbits_description: 'Arr, easy to set up and lightweight, LNbits can run on any Lightning Network funding source and even LNbits itself! Ye can run LNbits for yourself, or easily offer a custodian solution for others. Each chest has its own API keys and there be no limit to the number of chests ye can make. Being able to partition booty makes LNbits a useful tool for money management and as a development tool. Arr, extensions add extra functionality to LNbits so ye can experiment with a range of cutting-edge technologies on the lightning network. We have made developing extensions as easy as possible, and as a free and open-source project, we encourage scallywags to develop and submit their own.',
     export_to_phone: 'Export to Phone with QR Code, me hearties',
     export_to_phone_desc: 'This QR code contains yer chest URL with full access. Ye can scan it from yer phone to open yer chest from there, arr!',
     wallets: 'Treasure Chests',
     add_wallet: 'Add a new chest and fill it with doubloons!',
     delete_wallet: 'Scuttle the Chest',
@@ -221,9 +224,10 @@
     color_scheme: 'Colour Scheme',
     extension_cost: "This release be needin' a payment o' minimum %{cost} sats, arr.",
     extension_paid_sats: 'Ye have already paid %{paid_sats} sats.',
     release_details_error: "Cannot get th' release details.",
     pay_from_wallet: 'Pay from ye Wallet',
     show_qr: 'Show QR',
     retry_install: "Try 'nstallin' Again",
-    new_payment: 'Make New Payment'
+    new_payment: 'Make New Payment',
+    hide_empty_wallets: 'Stow empty wallets'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/pl.js` & `lnbits-0.12.8/lnbits/static/i18n/pl.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Finansowanie',
     users: 'Użytkownicy',
     apps: 'Aplikacje',
     channels: 'Kanały',
     transactions: 'Transakcje',
     dashboard: 'Panel kontrolny',
     node: 'Węzeł',
+    export_users: 'Eksportuj użytkowników',
+    no_users: 'Nie znaleziono użytkowników',
     total_capacity: 'Całkowita Pojemność',
     avg_channel_size: 'Średni rozmiar kanału',
     biggest_channel_size: 'Największy Rozmiar Kanału',
     smallest_channel_size: 'Najmniejszy Rozmiar Kanału',
     number_of_channels: 'Ilość kanałów',
     active_channels: 'Aktywne kanały',
     connect_peer: 'Połącz z węzłem równorzędnym',
@@ -29,14 +31,15 @@
     topup_hint: 'Użyj ID portfela aby go doładować',
     restart_tooltip: 'Zrestartuj serwer aby aktywować zmiany',
     add_funds_tooltip: 'Dodaj środki do portfela.',
     reset_defaults: 'Powrót do ustawień domyślnych',
     reset_defaults_tooltip: 'Wymaż wszystkie ustawienia i ustaw domyślne.',
     download_backup: 'Pobierz kopię zapasową bazy danych',
     name_your_wallet: 'Nazwij swój portfel %{name}',
+    wallet_topup_ok: 'Sukces w tworzeniu wirtualnych środków (%{amount} sats). Płatności zależą od rzeczywistych środków na źródle finansowania.',
     paste_invoice_label: 'Wklej fakturę, żądanie zapłaty lub kod lnurl *',
     lnbits_description: 'Łatwy i lekki w konfiguracji, LNbits może działać w oparciu o dowolne źródło finansowania w sieci lightning czy nawet inną instancję LNbits! Możesz uruchomić instancję LNbits dla siebie lub dla innych. Każdy portfel ma swoje klucze API i nie ma ograniczeń jeśli chodzi o ilość portfeli. LNbits umożliwia dzielenie środków w celu zarządzania nimi, jest również dobrym narzędziem deweloperskim. Rozszerzenia zwiększają funkcjonalność LNbits co umożliwia eksperymentowanie z nowym technologiami w sieci lightning. Tworzenie rozszerzeń jest proste dlatego zachęcamy innych deweloperów do tworzenia dodatkowych funkcjonalności i wysyłanie do nas PR',
     export_to_phone: 'Eksport kodu QR na telefon',
     export_to_phone_desc: 'Ten kod QR zawiera adres URL Twojego portfela z pełnym dostępem do niego. Możesz go zeskanować na swoim telefonie aby otworzyć na nim ten portfel.',
     wallets: 'Portfele',
     add_wallet: 'Dodaj portfel',
     delete_wallet: 'Usuń portfel',
@@ -221,9 +224,10 @@
     color_scheme: 'Schemat kolorów',
     extension_cost: 'To niniejsze wydanie wymaga zapłaty minimalnej %{cost} satów.',
     extension_paid_sats: 'Już zapłaciłeś %{paid_sats} satów.',
     release_details_error: 'Nie można uzyskać szczegółów wydania.',
     pay_from_wallet: 'Zapłać z portfela',
     show_qr: 'Pokaż kod QR',
     retry_install: 'Ponów instalację',
-    new_payment: 'Dokonaj nowej płatności'
+    new_payment: 'Dokonaj nowej płatności',
+    hide_empty_wallets: 'Ukryj puste portfele'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/pt.js` & `lnbits-0.12.8/lnbits/static/i18n/pt.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Financiamento',
     users: 'Usuários',
     apps: 'Aplicativos',
     channels: 'Canais',
     transactions: 'Transações',
     dashboard: 'Painel de Controle',
     node: 'Nó',
+    export_users: 'Exportar Usuários',
+    no_users: 'Nenhum usuário encontrado',
     total_capacity: 'Capacidade Total',
     avg_channel_size: 'Tamanho Médio do Canal',
     biggest_channel_size: 'Maior Tamanho do Canal',
     smallest_channel_size: 'Menor Tamanho de Canal',
     number_of_channels: 'Número de Canais',
     active_channels: 'Canais Ativos',
     connect_peer: 'Conectar Par',
@@ -29,14 +31,15 @@
     topup_hint: 'Use o ID da carteira para recarregar qualquer carteira',
     restart_tooltip: 'Reinicie o servidor para que as alterações tenham efeito',
     add_funds_tooltip: 'Adicionar fundos a uma carteira.',
     reset_defaults: 'Redefinir para padrões',
     reset_defaults_tooltip: 'Apagar todas as configurações e redefinir para os padrões.',
     download_backup: 'Fazer backup da base de dados',
     name_your_wallet: 'Nomeie sua carteira %{name}',
+    wallet_topup_ok: 'Sucesso ao criar fundos virtuais (%{amount} sats). Os pagamentos dependem dos fundos reais na fonte de financiamento.',
     paste_invoice_label: 'Cole uma fatura, pedido de pagamento ou código lnurl *',
     lnbits_description: 'Fácil de configurar e leve, o LNbits pode ser executado em qualquer fonte de financiamento da Lightning Network e até mesmo o LNbits em si! Você pode executar o LNbits para si mesmo ou oferecer facilmente uma solução de custódia para outros. Cada carteira tem suas próprias chaves de API e não há limite para o número de carteiras que você pode criar. Ser capaz de particionar fundos torna o LNbits uma ferramenta útil para gerenciamento de dinheiro e como uma ferramenta de desenvolvimento. As extensões adicionam funcionalidades extras ao LNbits para que você possa experimentar uma série de tecnologias de ponta na rede lightning. Nós tornamos o desenvolvimento de extensões o mais fácil possível e, como um projeto gratuito e de código aberto, incentivamos as pessoas a desenvolver e enviar as suas próprias.',
     export_to_phone: 'Exportar para o telefone com código QR',
     export_to_phone_desc: 'Este código QR contém a URL da sua carteira com acesso total. Você pode escaneá-lo do seu telefone para abrir sua carteira a partir dele.',
     wallets: 'Carteiras',
     add_wallet: 'Adicionar nova carteira',
     delete_wallet: 'Excluir carteira',
@@ -221,9 +224,10 @@
     color_scheme: 'Esquema de Cores',
     extension_cost: 'Este lançamento requer um pagamento mínimo de %{cost} sats.',
     extension_paid_sats: 'Você já pagou %{paid_sats} sats.',
     release_details_error: 'Não é possível obter os detalhes da versão.',
     pay_from_wallet: 'Pague da Carteira',
     show_qr: 'Exibir QR',
     retry_install: 'Reinstalar Tente Novamente',
-    new_payment: 'Realizar Novo Pagamento'
+    new_payment: 'Realizar Novo Pagamento',
+    hide_empty_wallets: 'Ocultar carteiras vazias'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/sk.js` & `lnbits-0.12.8/lnbits/static/i18n/sk.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Financovanie',
     users: 'Používatelia',
     apps: 'Aplikácie',
     channels: 'Kanály',
     transactions: 'Transakcie',
     dashboard: 'Prehľad',
     node: 'Uzol',
+    export_users: 'Exportovať používateľov',
+    no_users: 'Nenašli sa žiadni používatelia',
     total_capacity: 'Celková kapacita',
     avg_channel_size: 'Priemerná veľkosť kanálu',
     biggest_channel_size: 'Najväčší kanál',
     smallest_channel_size: 'Najmenší kanál',
     number_of_channels: 'Počet kanálov',
     active_channels: 'Aktívne kanály',
     connect_peer: 'Pripojiť peer',
@@ -29,14 +31,15 @@
     topup_hint: 'Použite ID peňaženky na doplnenie ľubovoľnej peňaženky',
     restart_tooltip: 'Pre prejavenie zmien reštartujte server',
     add_funds_tooltip: 'Pridať prostriedky do peňaženky.',
     reset_defaults: 'Obnoviť predvolené',
     reset_defaults_tooltip: 'Odstrániť všetky nastavenia a obnoviť predvolené.',
     download_backup: 'Stiahnuť zálohu databázy',
     name_your_wallet: 'Pomenujte vašu %{name} peňaženku',
+    wallet_topup_ok: 'Úspešne vytvorené virtuálne prostriedky (%{amount} sats). Platby závisia od skutočných prostriedkov v zdroji financovania.',
     paste_invoice_label: 'Vložte faktúru, platobnú požiadavku alebo lnurl kód *',
     lnbits_description: 'Ľahko nastaviteľný a ľahkotonážny, LNbits môže bežať na akomkoľvek zdroji financovania Lightning Network a dokonca LNbits samotný! LNbits môžete používať pre seba, alebo ľahko ponúknuť správcovské riešenie pre iných. Každá peňaženka má svoje vlastné API kľúče a nie je limit na počet peňaženiek, ktoré môžete vytvoriť. Schopnosť rozdeľovať finančné prostriedky robí z LNbits užitočný nástroj pre správu peňazí a ako vývojový nástroj. Rozšírenia pridávajú extra funkčnosť do LNbits, takže môžete experimentovať s radou najnovších technológií na lightning sieti. Vývoj rozšírení sme urobili čo najjednoduchší a ako voľný a open-source projekt, podporujeme ľudí vývoj a odovzdávanie vlastných rozšírení.',
     export_to_phone: 'Exportovať do telefónu s QR kódom',
     export_to_phone_desc: 'Tento QR kód obsahuje URL vašej peňaženky s plným prístupom. Môžete ho naskenovať z vášho telefónu a otvoriť vašu peňaženku odtiaľ.',
     wallets: 'Peňaženky',
     add_wallet: 'Pridať novú peňaženku',
     delete_wallet: 'Zmazať peňaženku',
@@ -221,9 +224,10 @@
     color_scheme: 'Farebná schéma',
     extension_cost: 'Táto verzia vyžaduje minimálnu platbu %{cost} satoshi.',
     extension_paid_sats: 'Už ste zaplatili %{paid_sats} sats.',
     release_details_error: 'Nepodarilo sa získať podrobnosti o vydaní.',
     pay_from_wallet: 'Zaplatiť z peňaženky',
     show_qr: 'Zobraziť QR',
     retry_install: 'Skúste inštaláciu znova',
-    new_payment: 'Vytvoriť novú platbu'
+    new_payment: 'Vytvoriť novú platbu',
+    hide_empty_wallets: 'Skryť prázdne peňaženky'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/i18n/we.js` & `lnbits-0.12.8/lnbits/static/i18n/we.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,16 @@
     funding: 'Arian fyndio',
     users: 'Defnyddwyr',
     apps: 'Apiau',
     channels: 'Sianelau',
     transactions: 'Trafodion',
     dashboard: 'Panel Gweinyddol',
     node: 'Nod',
+    export_users: 'Allfor Defnyddwyr',
+    no_users: 'Heb ganfod defnyddwyr',
     total_capacity: 'Capasiti Cyfanswm',
     avg_channel_size: 'Maint Sianel Cyf.',
     biggest_channel_size: 'Maint Sianel Fwyaf',
     smallest_channel_size: 'Maint Sianel Lleiaf',
     number_of_channels: 'Nifer y Sianeli',
     active_channels: 'Sianeli Gweithredol',
     connect_peer: 'Cysylltu â Chymar',
@@ -29,14 +31,15 @@
     topup_hint: 'Defnyddiwch ID y waled i ychwanegu at unrhyw waled',
     restart_tooltip: 'Ailgychwyn y gweinydd er mwyn i newidiadau ddod i rym',
     add_funds_tooltip: 'Ychwanegu arian at waled.',
     reset_defaults: 'Ailosod i`r rhagosodiadau',
     reset_defaults_tooltip: 'Dileu pob gosodiad ac ailosod i`r rhagosodiadau.',
     download_backup: 'Lawrlwytho copi wrth gefn cronfa ddata',
     name_your_wallet: 'Enwch eich waled %{name}',
+    wallet_topup_ok: "Llwyddiant wrth greu cronfeydd rhithwir (%{amount} sats). Mae taliadau'n dibynnu ar gronfeydd gwirioneddol ar y ffynhonnell cyllido.",
     paste_invoice_label: 'Gludwch anfoneb, cais am daliad neu god lnurl *',
     lnbits_description: 'Yn hawdd iw sefydlu ac yn ysgafn, gall LNbits redeg ar unrhyw ffynhonnell ariannu rhwydwaith mellt a hyd yn oed LNbits ei hun! Gallwch redeg LNbits i chi`ch hun, neu gynnig datrysiad ceidwad i eraill yn hawdd. Mae gan bob waled ei allweddi API ei hun ac nid oes cyfyngiad ar nifer y waledi y gallwch eu gwneud. Mae gallu rhannu cronfeydd yn gwneud LNbits yn arf defnyddiol ar gyfer rheoli arian ac fel offeryn datblygu. Mae estyniadau yn ychwanegu ymarferoldeb ychwanegol at LNbits fel y gallwch arbrofi gydag ystod o dechnolegau blaengar ar y rhwydwaith mellt. Rydym wedi gwneud datblygu estyniadau mor hawdd â phosibl, ac fel prosiect ffynhonnell agored am ddim, rydym yn annog pobl i ddatblygu a chyflwyno eu rhai eu hunain.',
     export_to_phone: 'Allforio i Ffôn gyda chod QR',
     export_to_phone_desc: 'Mae`r cod QR hwn yn cynnwys URL eich waled gyda mynediad llawn. Gallwch ei sganio o`ch ffôn i agor eich waled oddi yno.',
     wallets: 'Waledi',
     add_wallet: 'Ychwanegu waled newydd',
     delete_wallet: 'Dileu waled',
@@ -221,9 +224,10 @@
     color_scheme: 'Cynllun Lliw',
     extension_cost: "Mae'r rhyddhad hwn yn gofyn am daliad o leiaf %{cost} sats.",
     extension_paid_sats: 'Rydych chi eisoes wedi talu %{paid_sats} sats.',
     release_details_error: 'Methu cael manylion y rhyddhau.',
     pay_from_wallet: "Talu o'r Waled",
     show_qr: 'Dangos QR',
     retry_install: 'Ailgeisio Gosod',
-    new_payment: 'Gwneud Taliad Newydd'
+    new_payment: 'Gwneud Taliad Newydd',
+    hide_empty_wallets: 'Cuddio waledau gwag'
 }
```

### Comparing `lnbits-0.12.7/lnbits/static/images/alby.png` & `lnbits-0.12.8/lnbits/static/images/alby.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/albyl.png` & `lnbits-0.12.8/lnbits/static/images/albyl.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/bitcoin-hardware-wallet.png` & `lnbits-0.12.8/lnbits/static/images/bitcoin-hardware-wallet.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/bitcoin-shop-banner.png` & `lnbits-0.12.8/lnbits/static/images/bitcoin-shop-banner.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/blitz.png` & `lnbits-0.12.8/lnbits/static/images/blitz.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/blitzl.png` & `lnbits-0.12.8/lnbits/static/images/blitzl.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/cln.png` & `lnbits-0.12.8/lnbits/static/images/cln.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/clnl.png` & `lnbits-0.12.8/lnbits/static/images/clnl.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/default_voucher.png` & `lnbits-0.12.8/lnbits/static/images/default_voucher.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/github-logo.png` & `lnbits-0.12.8/lnbits/static/images/github-logo.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/google-logo.png` & `lnbits-0.12.8/lnbits/static/images/google-logo.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/keycloak-logo.png` & `lnbits-0.12.8/lnbits/static/images/keycloak-logo.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/lnbits-shop-dark.png` & `lnbits-0.12.8/lnbits/static/images/lnbits-shop-dark.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/lnbits-shop-light.png` & `lnbits-0.12.8/lnbits/static/images/lnbits-shop-light.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/lnd.png` & `lnbits-0.12.8/lnbits/static/images/lnd.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/lnpay.png` & `lnbits-0.12.8/lnbits/static/images/lnpay.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/lnpayl.png` & `lnbits-0.12.8/lnbits/static/images/lnpayl.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/logos/lnbits.png` & `lnbits-0.12.8/lnbits/static/images/logos/lnbits.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/maskable_icon.png` & `lnbits-0.12.8/lnbits/static/images/maskable_icon.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/maskable_icon_x192.png` & `lnbits-0.12.8/lnbits/static/images/maskable_icon_x192.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/maskable_icon_x512.png` & `lnbits-0.12.8/lnbits/static/images/maskable_icon_x512.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/maskable_icon_x96.png` & `lnbits-0.12.8/lnbits/static/images/maskable_icon_x96.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/mynode.png` & `lnbits-0.12.8/lnbits/static/images/mynode.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/mynodel.png` & `lnbits-0.12.8/lnbits/static/images/mynodel.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/open-sats.png` & `lnbits-0.12.8/lnbits/static/images/open-sats.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/opennode.png` & `lnbits-0.12.8/lnbits/static/images/opennode.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/opennodel.png` & `lnbits-0.12.8/lnbits/static/images/opennodel.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/phoenixd.png` & `lnbits-0.12.8/lnbits/static/images/phoenixd.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/phoenixdl.png` & `lnbits-0.12.8/lnbits/static/images/phoenixdl.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/screenshot_desktop.png` & `lnbits-0.12.8/lnbits/static/images/screenshot_desktop.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/screenshot_phone.png` & `lnbits-0.12.8/lnbits/static/images/screenshot_phone.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/spark.png` & `lnbits-0.12.8/lnbits/static/images/spark.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/sparkl.png` & `lnbits-0.12.8/lnbits/static/images/sparkl.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/start9.png` & `lnbits-0.12.8/lnbits/static/images/start9.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/start9l.png` & `lnbits-0.12.8/lnbits/static/images/start9l.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/templatead.png` & `lnbits-0.12.8/lnbits/static/images/templatead.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/umbrel.png` & `lnbits-0.12.8/lnbits/static/images/umbrel.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/umbrell.png` & `lnbits-0.12.8/lnbits/static/images/umbrell.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/voltage.png` & `lnbits-0.12.8/lnbits/static/images/voltage.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/voltagel.png` & `lnbits-0.12.8/lnbits/static/images/voltagel.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/voucher_template.svg` & `lnbits-0.12.8/lnbits/static/images/voucher_template.svg`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/zbd.png` & `lnbits-0.12.8/lnbits/static/images/zbd.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/images/zbdl.png` & `lnbits-0.12.8/lnbits/static/images/zbdl.png`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/account.js` & `lnbits-0.12.8/lnbits/static/js/account.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/admin.js` & `lnbits-0.12.8/lnbits/static/js/admin.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/base.js` & `lnbits-0.12.8/lnbits/static/js/base.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/bolt11-decoder.js` & `lnbits-0.12.8/lnbits/static/js/bolt11-decoder.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/components/extension-settings.js` & `lnbits-0.12.8/lnbits/static/js/components/extension-settings.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/components/lnbits-funding-sources.js` & `lnbits-0.12.8/lnbits/static/js/components/lnbits-funding-sources.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/components/payment-chart.js` & `lnbits-0.12.8/lnbits/static/js/components/payment-chart.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/components/payment-list.js` & `lnbits-0.12.8/lnbits/static/js/components/payment-list.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/components.js` & `lnbits-0.12.8/lnbits/static/js/components.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/event-reactions.js` & `lnbits-0.12.8/lnbits/static/js/event-reactions.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/index.js` & `lnbits-0.12.8/lnbits/static/js/index.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/node.js` & `lnbits-0.12.8/lnbits/static/js/node.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/users.js` & `lnbits-0.12.8/lnbits/static/js/users.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/js/wallet.js` & `lnbits-0.12.8/lnbits/static/js/wallet.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -555,14 +555,15 @@
         }
         if (this.$q.screen.lt.md) {
             this.mobileSimple = true
         }
         this.update.name = this.g.wallet.name
         this.update.currency = this.g.wallet.currency
         this.receive.units = ['sat', ...window.currencies]
+        this.updateFiatBalance()
     },
     watch: {
         updatePayments: function() {
             this.fetchBalance()
         }
     },
     mounted: function() {
```

### Comparing `lnbits-0.12.7/lnbits/static/scss/base.scss` & `lnbits-0.12.8/lnbits/static/scss/base.scss`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/Chart.bundle.js` & `lnbits-0.12.8/lnbits/static/vendor/Chart.bundle.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/Chart.css` & `lnbits-0.12.8/lnbits/static/vendor/Chart.css`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/VueQrcodeReader.umd.js` & `lnbits-0.12.8/lnbits/static/vendor/VueQrcodeReader.umd.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/axios.js` & `lnbits-0.12.8/lnbits/static/vendor/axios.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/moment.js` & `lnbits-0.12.8/lnbits/static/vendor/moment.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/quasar.css` & `lnbits-0.12.8/lnbits/static/vendor/quasar.css`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/quasar.ie.polyfills.umd.min.js` & `lnbits-0.12.8/lnbits/static/vendor/quasar.ie.polyfills.umd.min.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/quasar.umd.js` & `lnbits-0.12.8/lnbits/static/vendor/quasar.umd.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/showdown.js` & `lnbits-0.12.8/lnbits/static/vendor/showdown.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/underscore.js` & `lnbits-0.12.8/lnbits/static/vendor/underscore.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/vue-i18n.js` & `lnbits-0.12.8/lnbits/static/vendor/vue-i18n.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/vue-qrcode.js` & `lnbits-0.12.8/lnbits/static/vendor/vue-qrcode.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/vue-router.js` & `lnbits-0.12.8/lnbits/static/vendor/vue-router.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/vue.js` & `lnbits-0.12.8/lnbits/static/vendor/vue.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor/vuex.js` & `lnbits-0.12.8/lnbits/static/vendor/vuex.js`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/static/vendor.json` & `lnbits-0.12.8/lnbits/static/vendor.json`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/tasks.py` & `lnbits-0.12.8/lnbits/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,19 @@
 async def send_push_notification(subscription, title, body, url=""):
     vapid = Vapid()
     try:
         logger.debug("sending push notification")
         webpush(
             json.loads(subscription.data),
             json.dumps({"title": title, "body": body, "url": url}),
-            vapid.from_pem(bytes(settings.lnbits_webpush_privkey, "utf-8")),
+            (
+                vapid.from_pem(bytes(settings.lnbits_webpush_privkey, "utf-8"))
+                if settings.lnbits_webpush_privkey
+                else None
+            ),
             {"aud": "", "sub": "mailto:alan@lnbits.com"},
         )
     except WebPushException as e:
         if e.response.status_code == HTTPStatus.GONE:
             # cleanup unsubscribed or expired push subscriptions
             await delete_webpush_subscriptions(subscription.endpoint)
         else:
```

### Comparing `lnbits-0.12.7/lnbits/templates/base.html` & `lnbits-0.12.8/lnbits/templates/base.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/templates/error.html` & `lnbits-0.12.8/lnbits/templates/error.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/templates/print.html` & `lnbits-0.12.8/lnbits/templates/print.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/templates/public.html` & `lnbits-0.12.8/lnbits/templates/public.html`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/utils/cache.py` & `lnbits-0.12.8/lnbits/utils/cache.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/utils/crypto.py` & `lnbits-0.12.8/lnbits/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/utils/exchange_rates.py` & `lnbits-0.12.8/lnbits/utils/exchange_rates.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/utils/logger.py` & `lnbits-0.12.8/lnbits/utils/logger.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/__init__.py` & `lnbits-0.12.8/lnbits/wallets/__init__.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/alby.py` & `lnbits-0.12.8/lnbits/wallets/alby.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/base.py` & `lnbits-0.12.8/lnbits/wallets/base.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/cliche.py` & `lnbits-0.12.8/lnbits/wallets/cliche.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/corelightning.py` & `lnbits-0.12.8/lnbits/wallets/corelightning.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/corelightningrest.py` & `lnbits-0.12.8/lnbits/wallets/corelightningrest.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/eclair.py` & `lnbits-0.12.8/lnbits/wallets/eclair.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/fake.py` & `lnbits-0.12.8/lnbits/wallets/fake.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/lnbits.py` & `lnbits-0.12.8/lnbits/wallets/lnbits.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/lnd_grpc_files/lightning_pb2.py` & `lnbits-0.12.8/lnbits/wallets/lnd_grpc_files/lightning_pb2.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/lnd_grpc_files/lightning_pb2_grpc.py` & `lnbits-0.12.8/lnbits/wallets/lnd_grpc_files/lightning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/lnd_grpc_files/router_pb2.py` & `lnbits-0.12.8/lnbits/wallets/lnd_grpc_files/router_pb2.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/lnd_grpc_files/router_pb2_grpc.py` & `lnbits-0.12.8/lnbits/wallets/lnd_grpc_files/router_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/lndgrpc.py` & `lnbits-0.12.8/lnbits/wallets/lndgrpc.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/lndrest.py` & `lnbits-0.12.8/lnbits/wallets/lndrest.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/lnpay.py` & `lnbits-0.12.8/lnbits/wallets/lnpay.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/lntips.py` & `lnbits-0.12.8/lnbits/wallets/lntips.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/macaroon/macaroon.py` & `lnbits-0.12.8/lnbits/wallets/macaroon/macaroon.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/opennode.py` & `lnbits-0.12.8/lnbits/wallets/opennode.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/phoenixd.py` & `lnbits-0.12.8/lnbits/wallets/phoenixd.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/spark.py` & `lnbits-0.12.8/lnbits/wallets/spark.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/void.py` & `lnbits-0.12.8/lnbits/wallets/void.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/lnbits/wallets/zbd.py` & `lnbits-0.12.8/lnbits/wallets/zbd.py`

 * *Files identical despite different names*

### Comparing `lnbits-0.12.7/pyproject.toml` & `lnbits-0.12.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lnbits"
-version = "0.12.7"
+version = "0.12.8"
 description = "LNbits, free and open-source Lightning wallet and accounts system."
 authors = ["Alan Bits <alan@lnbits.com>"]
 readme = "README.md"
 repository = "https://github.com/lnbits/lnbits"
 homepage = "https://lnbits.com"
 packages = [
   {include = "lnbits"},
```

### Comparing `lnbits-0.12.7/PKG-INFO` & `lnbits-0.12.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnbits
-Version: 0.12.7
+Version: 0.12.8
 Summary: LNbits, free and open-source Lightning wallet and accounts system.
 Home-page: https://lnbits.com
 Author: Alan Bits
 Author-email: alan@lnbits.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

