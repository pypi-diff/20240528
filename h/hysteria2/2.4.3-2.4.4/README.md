# Comparing `tmp/hysteria2-2.4.3.tar.gz` & `tmp/hysteria2-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hysteria2-2.4.3.tar", last modified: Mon Apr 29 09:33:20 2024, max compression
+gzip compressed data, was "dist/hysteria2-2.4.4.tar", last modified: Tue May 28 02:17:11 2024, max compression
```

## Comparing `hysteria2-2.4.3.tar` & `hysteria2-2.4.4.tar`

### file list

```diff
@@ -1,356 +1,355 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.919344 hysteria2-2.4.3/
--rw-r--r--   0 runner     (501) staff       (20)     1170 2024-04-29 09:32:26.000000 hysteria2-2.4.3/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1069 2024-04-29 09:32:26.000000 hysteria2-2.4.3/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      195 2024-04-29 09:32:26.000000 hysteria2-2.4.3/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     5476 2024-04-29 09:33:20.918952 hysteria2-2.4.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3772 2024-04-29 09:32:26.000000 hysteria2-2.4.3/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.715710 hysteria2-2.4.3/gobuild/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-29 09:32:26.000000 hysteria2-2.4.3/gobuild/.gitkeep
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.716029 hysteria2-2.4.3/hysteria2/
--rw-r--r--   0 runner     (501) staff       (20)       60 2024-04-29 09:32:37.000000 hysteria2-2.4.3/hysteria2/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.722065 hysteria2-2.4.3/hysteria2-go/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.723227 hysteria2-2.4.3/hysteria2-go/.github/
--rw-r--r--   0 runner     (501) staff       (20)       57 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/FUNDING.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.725498 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner     (501) staff       (20)      536 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner     (501) staff       (20)      511 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.zh.md
--rw-r--r--   0 runner     (501) staff       (20)      605 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner     (501) staff       (20)      597 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.zh.md
--rw-r--r--   0 runner     (501) staff       (20)      204 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/dependabot.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.727756 hysteria2-2.4.3/hysteria2-go/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1171 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/workflows/docker.yml
--rw-r--r--   0 runner     (501) staff       (20)     1188 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/.github/workflows/master.yml
--rw-r--r--   0 runner     (501) staff       (20)     1947 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/.github/workflows/release.yml
--rw-r--r--   0 runner     (501) staff       (20)      668 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/.github/workflows/scripts.yml
--rw-r--r--   0 runner     (501) staff       (20)     9265 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)       57 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/CHANGELOG.md
--rw-r--r--   0 runner     (501) staff       (20)     1257 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/Dockerfile
--rw-r--r--   0 runner     (501) staff       (20)     1052 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)     8028 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/PROTOCOL.md
--rw-r--r--   0 runner     (501) staff       (20)     2288 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.730018 hysteria2-2.4.3/hysteria2-go/app/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.737213 hysteria2-2.4.3/hysteria2-go/app/cmd/
--rw-r--r--   0 runner     (501) staff       (20)    32611 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/client.go
--rw-r--r--   0 runner     (501) staff       (20)     4790 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/client_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1386 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/client_test.yaml
--rw-r--r--   0 runner     (501) staff       (20)      245 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/errors.go
--rw-r--r--   0 runner     (501) staff       (20)     1574 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/ping.go
--rw-r--r--   0 runner     (501) staff       (20)     4779 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/root.go
--rw-r--r--   0 runner     (501) staff       (20)    29942 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/server.go
--rw-r--r--   0 runner     (501) staff       (20)     3860 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/server_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2091 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/server_test.yaml
--rw-r--r--   0 runner     (501) staff       (20)     4506 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/speedtest.go
--rw-r--r--   0 runner     (501) staff       (20)     2292 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/update.go
--rw-r--r--   0 runner     (501) staff       (20)      359 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/version.go
--rw-r--r--   0 runner     (501) staff       (20)     3167 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/go.mod
--rw-r--r--   0 runner     (501) staff       (20)    60261 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/go.sum
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.702829 hysteria2-2.4.3/hysteria2-go/app/internal/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.739497 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/
--rw-r--r--   0 runner     (501) staff       (20)     1047 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/tcp.go
--rw-r--r--   0 runner     (501) staff       (20)      743 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/tcp_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3633 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/udp.go
--rw-r--r--   0 runner     (501) staff       (20)      749 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/udp_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.742143 hysteria2-2.4.3/hysteria2-go/app/internal/http/
--rw-r--r--   0 runner     (501) staff       (20)     7744 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/server.go
--rw-r--r--   0 runner     (501) staff       (20)     1316 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/server_test.go
--rw-r--r--   0 runner     (501) staff       (20)      582 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/server_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1363 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/test.crt
--rw-r--r--   0 runner     (501) staff       (20)     1675 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/test.key
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.745287 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/
--rw-r--r--   0 runner     (501) staff       (20)      209 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/.mockery.yaml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.700842 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.746295 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/mocks/
--rw-r--r--   0 runner     (501) staff       (20)    10390 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Conn.go
--rw-r--r--   0 runner     (501) staff       (20)     4297 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Listener.go
--rw-r--r--   0 runner     (501) staff       (20)     1343 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/manager.go
--rw-r--r--   0 runner     (501) staff       (20)     1789 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/manager_test.go
--rw-r--r--   0 runner     (501) staff       (20)     5951 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/mux.go
--rw-r--r--   0 runner     (501) staff       (20)     3044 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/mux_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.749131 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/
--rw-r--r--   0 runner     (501) staff       (20)      328 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/getsockopt_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      551 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/getsockopt_linux_386.go
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/syscall_socketcall_linux_386.s
--rw-r--r--   0 runner     (501) staff       (20)     2734 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/tcp_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      424 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/tcp_others.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.751450 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/
--rw-r--r--   0 runner     (501) staff       (20)     1981 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/fd_control_unix_socket_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1900 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/sockopts.go
--rw-r--r--   0 runner     (501) staff       (20)     2300 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/sockopts_linux.go
--rw-r--r--   0 runner     (501) staff       (20)     1105 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/sockopts_linux_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.753401 hysteria2-2.4.3/hysteria2-go/app/internal/socks5/
--rw-r--r--   0 runner     (501) staff       (20)     7613 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server.go
--rw-r--r--   0 runner     (501) staff       (20)      578 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1423 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server_test.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.755880 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/
--rw-r--r--   0 runner     (501) staff       (20)     1408 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/tcp_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      418 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/tcp_others.go
--rw-r--r--   0 runner     (501) staff       (20)     3082 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/udp_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      453 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/udp_others.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.756954 hysteria2-2.4.3/hysteria2-go/app/internal/tun/
--rw-r--r--   0 runner     (501) staff       (20)     1450 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tun/log.go
--rw-r--r--   0 runner     (501) staff       (20)     5114 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tun/server.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.758160 hysteria2-2.4.3/hysteria2-go/app/internal/url/
--rw-r--r--   0 runner     (501) staff       (20)    35764 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/url/url.go
--rw-r--r--   0 runner     (501) staff       (20)     1760 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/url/url_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.760832 hysteria2-2.4.3/hysteria2-go/app/internal/utils/
--rw-r--r--   0 runner     (501) staff       (20)     1549 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/bpsconv.go
--rw-r--r--   0 runner     (501) staff       (20)     1088 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/bpsconv_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3887 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/geoloader.go
--rw-r--r--   0 runner     (501) staff       (20)      267 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/qr.go
--rw-r--r--   0 runner     (501) staff       (20)     2519 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/update.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.761353 hysteria2-2.4.3/hysteria2-go/app/internal/utils_test/
--rw-r--r--   0 runner     (501) staff       (20)     1823 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils_test/mock.go
--rw-r--r--   0 runner     (501) staff       (20)      225 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/main.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.761974 hysteria2-2.4.3/hysteria2-go/app/misc/
--rw-r--r--   0 runner     (501) staff       (20)     1405 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/misc/socks5_test.py
--rw-r--r--   0 runner     (501) staff       (20)      310 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/pprof.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.762907 hysteria2-2.4.3/hysteria2-go/core/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.766663 hysteria2-2.4.3/hysteria2-go/core/client/
--rw-r--r--   0 runner     (501) staff       (20)      171 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/.mockery.yaml
--rw-r--r--   0 runner     (501) staff       (20)     8098 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/client.go
--rw-r--r--   0 runner     (501) staff       (20)     4190 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/config.go
--rw-r--r--   0 runner     (501) staff       (20)     3613 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/mock_udpIO.go
--rw-r--r--   0 runner     (501) staff       (20)     3135 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/reconnect.go
--rw-r--r--   0 runner     (501) staff       (20)     3402 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/udp.go
--rw-r--r--   0 runner     (501) staff       (20)     2934 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/udp_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.767080 hysteria2-2.4.3/hysteria2-go/core/errors/
--rw-r--r--   0 runner     (501) staff       (20)     1590 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/errors/errors.go
--rw-r--r--   0 runner     (501) staff       (20)     1202 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/go.mod
--rw-r--r--   0 runner     (501) staff       (20)     6432 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/go.sum
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.706366 hysteria2-2.4.3/hysteria2-go/core/internal/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.767994 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.772033 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/
--rw-r--r--   0 runner     (501) staff       (20)      602 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bandwidth.go
--rw-r--r--   0 runner     (501) staff       (20)    31585 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bandwidth_sampler.go
--rw-r--r--   0 runner     (501) staff       (20)    32614 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bbr_sender.go
--rw-r--r--   0 runner     (501) staff       (20)      327 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/clock.go
--rw-r--r--   0 runner     (501) staff       (20)     5684 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/packet_number_indexed_queue.go
--rw-r--r--   0 runner     (501) staff       (20)     3225 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/ringbuffer.go
--rw-r--r--   0 runner     (501) staff       (20)     5609 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/windowed_filter.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.772724 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/brutal/
--rw-r--r--   0 runner     (501) staff       (20)     5432 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/brutal/brutal.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.773353 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/common/
--rw-r--r--   0 runner     (501) staff       (20)     2267 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/common/pacer.go
--rw-r--r--   0 runner     (501) staff       (20)      449 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/utils.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.774464 hysteria2-2.4.3/hysteria2-go/core/internal/frag/
--rw-r--r--   0 runner     (501) staff       (20)     1952 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/frag/frag.go
--rw-r--r--   0 runner     (501) staff       (20)     5867 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/frag/frag_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.779698 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/
--rw-r--r--   0 runner     (501) staff       (20)      543 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/.mockery.yaml
--rw-r--r--   0 runner     (501) staff       (20)     8156 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/close_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2558 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/masq_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.783108 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/
--rw-r--r--   0 runner     (501) staff       (20)     2675 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Authenticator.go
--rw-r--r--   0 runner     (501) staff       (20)     9787 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Conn.go
--rw-r--r--   0 runner     (501) staff       (20)     8645 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_EventLogger.go
--rw-r--r--   0 runner     (501) staff       (20)     3662 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Outbound.go
--rw-r--r--   0 runner     (501) staff       (20)     2168 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_TrafficLogger.go
--rw-r--r--   0 runner     (501) staff       (20)     4692 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_UDPConn.go
--rw-r--r--   0 runner     (501) staff       (20)     7704 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/smoke_test.go
--rw-r--r--   0 runner     (501) staff       (20)     6021 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/stress_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1363 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/test.crt
--rw-r--r--   0 runner     (501) staff       (20)     1675 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/test.key
--rw-r--r--   0 runner     (501) staff       (20)     5297 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/trafficlogger_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1611 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/utils_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.784264 hysteria2-2.4.3/hysteria2-go/core/internal/pmtud/
--rw-r--r--   0 runner     (501) staff       (20)       97 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/pmtud/avail.go
--rw-r--r--   0 runner     (501) staff       (20)      480 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/pmtud/unavail.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.786646 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/
--rw-r--r--   0 runner     (501) staff       (20)     1826 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/http.go
--rw-r--r--   0 runner     (501) staff       (20)      637 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/padding.go
--rw-r--r--   0 runner     (501) staff       (20)     6130 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/proxy.go
--rw-r--r--   0 runner     (501) staff       (20)    11136 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/proxy_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.787686 hysteria2-2.4.3/hysteria2-go/core/internal/utils/
--rw-r--r--   0 runner     (501) staff       (20)      316 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/utils/atomic.go
--rw-r--r--   0 runner     (501) staff       (20)     1517 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/utils/qstream.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.792560 hysteria2-2.4.3/hysteria2-go/core/server/
--rw-r--r--   0 runner     (501) staff       (20)      311 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/.mockery.yaml
--rw-r--r--   0 runner     (501) staff       (20)     7566 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/config.go
--rw-r--r--   0 runner     (501) staff       (20)     1512 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/copy.go
--rw-r--r--   0 runner     (501) staff       (20)     4693 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/mock_UDPConn.go
--rw-r--r--   0 runner     (501) staff       (20)     3130 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/mock_udpEventLogger.go
--rw-r--r--   0 runner     (501) staff       (20)     4943 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/mock_udpIO.go
--rw-r--r--   0 runner     (501) staff       (20)     9058 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/server.go
--rw-r--r--   0 runner     (501) staff       (20)     5871 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/udp.go
--rw-r--r--   0 runner     (501) staff       (20)     5208 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/udp_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.793861 hysteria2-2.4.3/hysteria2-go/extras/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.798274 hysteria2-2.4.3/hysteria2-go/extras/auth/
--rw-r--r--   0 runner     (501) staff       (20)      621 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/command.go
--rw-r--r--   0 runner     (501) staff       (20)     1756 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/http.go
--rw-r--r--   0 runner     (501) staff       (20)      760 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/http_test.go
--rw-r--r--   0 runner     (501) staff       (20)      547 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/http_test.py
--rw-r--r--   0 runner     (501) staff       (20)      477 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/password.go
--rw-r--r--   0 runner     (501) staff       (20)     1106 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/password_test.go
--rw-r--r--   0 runner     (501) staff       (20)      847 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/userpass.go
--rw-r--r--   0 runner     (501) staff       (20)     1729 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/userpass_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.798852 hysteria2-2.4.3/hysteria2-go/extras/correctnet/
--rw-r--r--   0 runner     (501) staff       (20)     2064 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/correctnet/correctnet.go
--rw-r--r--   0 runner     (501) staff       (20)     1436 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/go.mod
--rw-r--r--   0 runner     (501) staff       (20)    10610 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/go.sum
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.799347 hysteria2-2.4.3/hysteria2-go/extras/masq/
--rw-r--r--   0 runner     (501) staff       (20)     2865 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/masq/server.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.801087 hysteria2-2.4.3/hysteria2-go/extras/obfs/
--rw-r--r--   0 runner     (501) staff       (20)     2915 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/obfs/conn.go
--rw-r--r--   0 runner     (501) staff       (20)     1527 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/obfs/salamander.go
--rw-r--r--   0 runner     (501) staff       (20)     1048 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/obfs/salamander_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.811187 hysteria2-2.4.3/hysteria2-go/extras/outbounds/
--rw-r--r--   0 runner     (501) staff       (20)      263 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/.mockery.yaml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.815500 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/
--rw-r--r--   0 runner     (501) staff       (20)     7738 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/compile.go
--rw-r--r--   0 runner     (501) staff       (20)     6601 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/compile_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1468 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers.go
--rw-r--r--   0 runner     (501) staff       (20)     6123 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_test.go
--rw-r--r--   0 runner     (501) staff       (20)     4808 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_v2geo.go
--rw-r--r--   0 runner     (501) staff       (20)     2489 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_v2geo_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/parse.go
--rw-r--r--   0 runner     (501) staff       (20)     1611 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/parse_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.858627 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/
--rw-r--r--   0 runner     (501) staff       (20)  9640091 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/geoip.dat
--rw-r--r--   0 runner     (501) staff       (20)  4143750 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/geosite.dat
--rw-r--r--   0 runner     (501) staff       (20)     1080 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/load.go
--rw-r--r--   0 runner     (501) staff       (20)     1348 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/load_test.go
--rw-r--r--   0 runner     (501) staff       (20)    21809 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1561 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.proto
--rw-r--r--   0 runner     (501) staff       (20)     3266 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl.go
--rw-r--r--   0 runner     (501) staff       (20)     1675 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1956 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_https.go
--rw-r--r--   0 runner     (501) staff       (20)     5508 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_standard.go
--rw-r--r--   0 runner     (501) staff       (20)     1053 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_system.go
--rw-r--r--   0 runner     (501) staff       (20)     3913 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/interface.go
--rw-r--r--   0 runner     (501) staff       (20)     1225 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/interface_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3906 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/mock_PluggableOutbound.go
--rw-r--r--   0 runner     (501) staff       (20)     4741 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/mock_UDPConn.go
--rw-r--r--   0 runner     (501) staff       (20)    11736 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct.go
--rw-r--r--   0 runner     (501) staff       (20)     1287 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      628 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct_others.go
--rw-r--r--   0 runner     (501) staff       (20)     4596 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_http.go
--rw-r--r--   0 runner     (501) staff       (20)     6928 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_socks5.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.861763 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/
--rw-r--r--   0 runner     (501) staff       (20)     3031 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/client.go
--rw-r--r--   0 runner     (501) staff       (20)     3381 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/protocol.go
--rw-r--r--   0 runner     (501) staff       (20)     9544 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/protocol_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2163 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/server.go
--rw-r--r--   0 runner     (501) staff       (20)      796 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest.go
--rw-r--r--   0 runner     (501) staff       (20)      963 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/utils.go
--rw-r--r--   0 runner     (501) staff       (20)     1603 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/utils_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.862379 hysteria2-2.4.3/hysteria2-go/extras/trafficlogger/
--rw-r--r--   0 runner     (501) staff       (20)     3228 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/trafficlogger/http.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.709363 hysteria2-2.4.3/hysteria2-go/extras/transport/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.863968 hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/
--rw-r--r--   0 runner     (501) staff       (20)     1960 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/addr.go
--rw-r--r--   0 runner     (501) staff       (20)     2488 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/addr_test.go
--rw-r--r--   0 runner     (501) staff       (20)     6863 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/conn.go
--rw-r--r--   0 runner     (501) staff       (20)       42 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/go.work
--rw-r--r--   0 runner     (501) staff       (20)    33613 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/go.work.sum
--rw-r--r--   0 runner     (501) staff       (20)    14484 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/hyperbole.py
--rw-r--r--   0 runner     (501) staff       (20)     2490 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/logo.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.710123 hysteria2-2.4.3/hysteria2-go/media-kit/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.876350 hysteria2-2.4.3/hysteria2-go/media-kit/png/
--rw-r--r--   0 runner     (501) staff       (20)    18296 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/black 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    38595 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/black 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    19475 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/black 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    40667 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/black 4@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    17502 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    37286 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    18565 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    38855 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 4@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    18334 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    38791 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    19526 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    40734 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 4@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    12744 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    12395 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    12672 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    12013 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 4@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    17426 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/white 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    37014 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/white 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    18330 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/white 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    38461 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/white 4@2x.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.887123 hysteria2-2.4.3/hysteria2-go/media-kit/svg/
--rw-r--r--   0 runner     (501) staff       (20)     2126 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 1.svg
--rw-r--r--   0 runner     (501) staff       (20)    14333 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2427 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 3.svg
--rw-r--r--   0 runner     (501) staff       (20)    14626 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 4.svg
--rw-r--r--   0 runner     (501) staff       (20)     2347 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 1.svg
--rw-r--r--   0 runner     (501) staff       (20)    15086 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2662 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 3.svg
--rw-r--r--   0 runner     (501) staff       (20)    15393 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 4.svg
--rw-r--r--   0 runner     (501) staff       (20)     2189 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 1.svg
--rw-r--r--   0 runner     (501) staff       (20)    14396 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2490 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 3.svg
--rw-r--r--   0 runner     (501) staff       (20)    14689 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 4.svg
--rw-r--r--   0 runner     (501) staff       (20)      714 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 1.svg
--rw-r--r--   0 runner     (501) staff       (20)      788 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 2.svg
--rw-r--r--   0 runner     (501) staff       (20)      651 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 3.svg
--rw-r--r--   0 runner     (501) staff       (20)      767 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 4.svg
--rw-r--r--   0 runner     (501) staff       (20)     2326 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 1.svg
--rw-r--r--   0 runner     (501) staff       (20)    15065 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2641 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 3.svg
--rw-r--r--   0 runner     (501) staff       (20)    15372 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 4.svg
--rw-r--r--   0 runner     (501) staff       (20)      488 2024-04-29 09:32:37.000000 hysteria2-2.4.3/hysteria2-go/platforms.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.888224 hysteria2-2.4.3/hysteria2-go/scripts/
--rw-r--r--   0 runner     (501) staff       (20)       25 2024-04-29 09:32:37.000000 hysteria2-2.4.3/hysteria2-go/scripts/_redirects
--rw-r--r--   0 runner     (501) staff       (20)    26403 2024-04-29 09:32:37.000000 hysteria2-2.4.3/hysteria2-go/scripts/install_server.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.891002 hysteria2-2.4.3/hysteria2.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     5476 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    12021 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       10 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.892831 hysteria2-2.4.3/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    11911 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1684 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)        7 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/VERSION
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.711232 hysteria2-2.4.3/pybind11/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.904300 hysteria2-2.4.3/pybind11/include/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    23979 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner     (501) staff       (20)     7069 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner     (501) staff       (20)    65638 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner     (501) staff       (20)     8458 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner     (501) staff       (20)      120 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner     (501) staff       (20)     2096 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.908603 hysteria2-2.4.3/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner     (501) staff       (20)    28251 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner     (501) staff       (20)    50369 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner     (501) staff       (20)     5491 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner     (501) staff       (20)    17981 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner     (501) staff       (20)    25057 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner     (501) staff       (20)    42266 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner     (501) staff       (20)     1625 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner     (501) staff       (20)    32147 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner     (501) staff       (20)    11792 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner     (501) staff       (20)     4731 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner     (501) staff       (20)     4695 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner     (501) staff       (20)     8262 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner     (501) staff       (20)     8862 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner     (501) staff       (20)    79524 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner     (501) staff       (20)     9103 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner     (501) staff       (20)     2181 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner     (501) staff       (20)   125761 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner     (501) staff       (20)    93848 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.909111 hysteria2-2.4.3/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner     (501) staff       (20)     4185 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner     (501) staff       (20)    15337 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner     (501) staff       (20)    27013 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.917758 hysteria2-2.4.3/pybind11/tools/
--rw-r--r--   0 runner     (501) staff       (20)     2350 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner     (501) staff       (20)     3105 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner     (501) staff       (20)    11103 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner     (501) staff       (20)      817 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 runner     (501) staff       (20)     1423 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/check-style.sh
--rw-r--r--   0 runner     (501) staff       (20)      952 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     1040 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner     (501) staff       (20)     1031 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/libsize.py
--rw-r--r--   0 runner     (501) staff       (20)     1282 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner     (501) staff       (20)      196 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner     (501) staff       (20)    13487 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner     (501) staff       (20)     6930 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     8955 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner     (501) staff       (20)     8359 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner     (501) staff       (20)       94 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1965 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner     (501) staff       (20)     1139 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-29 09:33:20.919466 hysteria2-2.4.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2742 2024-04-29 09:32:37.000000 hysteria2-2.4.3/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.918328 hysteria2-2.4.3/src/
--rw-r--r--   0 runner     (501) staff       (20)      703 2024-04-29 09:32:37.000000 hysteria2-2.4.3/src/hysteria2.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/
+-rw-r--r--   0 runner     (501) staff       (20)     1170 2024-05-28 02:16:44.000000 hysteria2-2.4.4/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      195 2024-05-28 02:16:44.000000 hysteria2-2.4.4/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     5476 2024-05-28 02:17:11.000000 hysteria2-2.4.4/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3772 2024-05-28 02:16:44.000000 hysteria2-2.4.4/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/gobuild/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 02:16:44.000000 hysteria2-2.4.4/gobuild/.gitkeep
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2/
+-rw-r--r--   0 runner     (501) staff       (20)       60 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2-go/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2-go/.github/
+-rw-r--r--   0 runner     (501) staff       (20)       57 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/FUNDING.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2-go/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner     (501) staff       (20)      536 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner     (501) staff       (20)      511 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.zh.md
+-rw-r--r--   0 runner     (501) staff       (20)      605 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner     (501) staff       (20)      597 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.zh.md
+-rw-r--r--   0 runner     (501) staff       (20)      204 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/dependabot.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1171 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/workflows/docker.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1188 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/workflows/master.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1947 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/workflows/release.yml
+-rw-r--r--   0 runner     (501) staff       (20)      668 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.github/workflows/scripts.yml
+-rw-r--r--   0 runner     (501) staff       (20)     9265 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)       57 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/CHANGELOG.md
+-rw-r--r--   0 runner     (501) staff       (20)     1257 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/Dockerfile
+-rw-r--r--   0 runner     (501) staff       (20)     1052 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)     8028 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/PROTOCOL.md
+-rw-r--r--   0 runner     (501) staff       (20)     2288 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/
+-rw-r--r--   0 runner     (501) staff       (20)    33618 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     4790 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/client_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1386 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/client_test.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/errors.go
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/ping.go
+-rw-r--r--   0 runner     (501) staff       (20)     4779 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/root.go
+-rw-r--r--   0 runner     (501) staff       (20)    29942 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/server.go
+-rw-r--r--   0 runner     (501) staff       (20)     3860 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/server_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2091 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/server_test.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     4506 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/speedtest.go
+-rw-r--r--   0 runner     (501) staff       (20)     2292 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/update.go
+-rw-r--r--   0 runner     (501) staff       (20)      359 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/cmd/version.go
+-rw-r--r--   0 runner     (501) staff       (20)     3167 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/go.mod
+-rw-r--r--   0 runner     (501) staff       (20)    60261 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/go.sum
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2-go/app/internal/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/forwarding/
+-rw-r--r--   0 runner     (501) staff       (20)     1047 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/forwarding/tcp.go
+-rw-r--r--   0 runner     (501) staff       (20)      743 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/forwarding/tcp_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3633 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/forwarding/udp.go
+-rw-r--r--   0 runner     (501) staff       (20)      749 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/forwarding/udp_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/http/
+-rw-r--r--   0 runner     (501) staff       (20)     7744 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/http/server.go
+-rw-r--r--   0 runner     (501) staff       (20)     1316 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/http/server_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      582 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/http/server_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1363 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/http/test.crt
+-rw-r--r--   0 runner     (501) staff       (20)     1675 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/http/test.key
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/
+-rw-r--r--   0 runner     (501) staff       (20)      209 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/.mockery.yaml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/internal/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/internal/mocks/
+-rw-r--r--   0 runner     (501) staff       (20)    10390 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Conn.go
+-rw-r--r--   0 runner     (501) staff       (20)     4297 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Listener.go
+-rw-r--r--   0 runner     (501) staff       (20)     1343 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/manager.go
+-rw-r--r--   0 runner     (501) staff       (20)     1789 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/manager_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     5951 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/mux.go
+-rw-r--r--   0 runner     (501) staff       (20)     3044 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/mux_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/redirect/
+-rw-r--r--   0 runner     (501) staff       (20)      328 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/redirect/getsockopt_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      551 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/redirect/getsockopt_linux_386.go
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/redirect/syscall_socketcall_linux_386.s
+-rw-r--r--   0 runner     (501) staff       (20)     2734 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/redirect/tcp_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      424 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/redirect/tcp_others.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/sockopts/
+-rw-r--r--   0 runner     (501) staff       (20)     1981 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/sockopts/fd_control_unix_socket_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1900 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/sockopts/sockopts.go
+-rw-r--r--   0 runner     (501) staff       (20)     2300 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/sockopts/sockopts_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)     1105 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/sockopts/sockopts_linux_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/socks5/
+-rw-r--r--   0 runner     (501) staff       (20)     7613 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/socks5/server.go
+-rw-r--r--   0 runner     (501) staff       (20)      578 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/socks5/server_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1423 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/socks5/server_test.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/tproxy/
+-rw-r--r--   0 runner     (501) staff       (20)     1408 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/tproxy/tcp_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      418 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/tproxy/tcp_others.go
+-rw-r--r--   0 runner     (501) staff       (20)     3082 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/tproxy/udp_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      453 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/tproxy/udp_others.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/tun/
+-rw-r--r--   0 runner     (501) staff       (20)     1450 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/tun/log.go
+-rw-r--r--   0 runner     (501) staff       (20)     5114 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/tun/server.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/url/
+-rw-r--r--   0 runner     (501) staff       (20)    35764 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/url/url.go
+-rw-r--r--   0 runner     (501) staff       (20)     1760 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/url/url_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/utils/
+-rw-r--r--   0 runner     (501) staff       (20)     1549 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/utils/bpsconv.go
+-rw-r--r--   0 runner     (501) staff       (20)     1088 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/utils/bpsconv_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3887 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/utils/geoloader.go
+-rw-r--r--   0 runner     (501) staff       (20)      267 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/utils/qr.go
+-rw-r--r--   0 runner     (501) staff       (20)     2519 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/utils/update.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/internal/utils_test/
+-rw-r--r--   0 runner     (501) staff       (20)     1823 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/internal/utils_test/mock.go
+-rw-r--r--   0 runner     (501) staff       (20)      225 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/main.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/app/misc/
+-rw-r--r--   0 runner     (501) staff       (20)     1405 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/misc/socks5_test.py
+-rw-r--r--   0 runner     (501) staff       (20)      310 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/app/pprof.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/client/
+-rw-r--r--   0 runner     (501) staff       (20)      171 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/client/.mockery.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     8098 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/client/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     4190 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/client/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     3770 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/client/mock_udpIO.go
+-rw-r--r--   0 runner     (501) staff       (20)     3135 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/client/reconnect.go
+-rw-r--r--   0 runner     (501) staff       (20)     3402 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/client/udp.go
+-rw-r--r--   0 runner     (501) staff       (20)     2934 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/client/udp_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/errors/
+-rw-r--r--   0 runner     (501) staff       (20)     1590 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/errors/errors.go
+-rw-r--r--   0 runner     (501) staff       (20)     1202 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/go.mod
+-rw-r--r--   0 runner     (501) staff       (20)     6432 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/go.sum
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2-go/core/internal/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/
+-rw-r--r--   0 runner     (501) staff       (20)      602 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/bandwidth.go
+-rw-r--r--   0 runner     (501) staff       (20)    31585 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/bandwidth_sampler.go
+-rw-r--r--   0 runner     (501) staff       (20)    32614 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/bbr_sender.go
+-rw-r--r--   0 runner     (501) staff       (20)      327 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/clock.go
+-rw-r--r--   0 runner     (501) staff       (20)     5684 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/packet_number_indexed_queue.go
+-rw-r--r--   0 runner     (501) staff       (20)     3225 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/ringbuffer.go
+-rw-r--r--   0 runner     (501) staff       (20)     5609 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/windowed_filter.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/brutal/
+-rw-r--r--   0 runner     (501) staff       (20)     5432 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/brutal/brutal.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/common/
+-rw-r--r--   0 runner     (501) staff       (20)     2267 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/common/pacer.go
+-rw-r--r--   0 runner     (501) staff       (20)      449 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/congestion/utils.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/frag/
+-rw-r--r--   0 runner     (501) staff       (20)     1952 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/frag/frag.go
+-rw-r--r--   0 runner     (501) staff       (20)     5867 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/frag/frag_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/
+-rw-r--r--   0 runner     (501) staff       (20)      543 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/.mockery.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     8156 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/close_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2558 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/masq_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/
+-rw-r--r--   0 runner     (501) staff       (20)     2753 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_Authenticator.go
+-rw-r--r--   0 runner     (501) staff       (20)    10390 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_Conn.go
+-rw-r--r--   0 runner     (501) staff       (20)     8645 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_EventLogger.go
+-rw-r--r--   0 runner     (501) staff       (20)     3800 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_Outbound.go
+-rw-r--r--   0 runner     (501) staff       (20)     3580 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_TrafficLogger.go
+-rw-r--r--   0 runner     (501) staff       (20)     4910 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_UDPConn.go
+-rw-r--r--   0 runner     (501) staff       (20)     7704 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/smoke_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6021 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/stress_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1363 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/test.crt
+-rw-r--r--   0 runner     (501) staff       (20)     1675 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/test.key
+-rw-r--r--   0 runner     (501) staff       (20)     5625 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/trafficlogger_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1611 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/utils_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/pmtud/
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/pmtud/avail.go
+-rw-r--r--   0 runner     (501) staff       (20)      480 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/pmtud/unavail.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/protocol/
+-rw-r--r--   0 runner     (501) staff       (20)     1826 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/protocol/http.go
+-rw-r--r--   0 runner     (501) staff       (20)      637 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/protocol/padding.go
+-rw-r--r--   0 runner     (501) staff       (20)     6130 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/protocol/proxy.go
+-rw-r--r--   0 runner     (501) staff       (20)    11136 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/protocol/proxy_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/internal/utils/
+-rw-r--r--   0 runner     (501) staff       (20)      316 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/utils/atomic.go
+-rw-r--r--   0 runner     (501) staff       (20)     1517 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/internal/utils/qstream.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/core/server/
+-rw-r--r--   0 runner     (501) staff       (20)      311 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/server/.mockery.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     7613 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/server/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     1526 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/server/copy.go
+-rw-r--r--   0 runner     (501) staff       (20)     4911 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/server/mock_UDPConn.go
+-rw-r--r--   0 runner     (501) staff       (20)     3130 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/server/mock_udpEventLogger.go
+-rw-r--r--   0 runner     (501) staff       (20)     5169 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/server/mock_udpIO.go
+-rw-r--r--   0 runner     (501) staff       (20)     9245 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/server/server.go
+-rw-r--r--   0 runner     (501) staff       (20)     5871 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/server/udp.go
+-rw-r--r--   0 runner     (501) staff       (20)     5208 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/core/server/udp_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/auth/
+-rw-r--r--   0 runner     (501) staff       (20)      621 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/auth/command.go
+-rw-r--r--   0 runner     (501) staff       (20)     1756 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/auth/http.go
+-rw-r--r--   0 runner     (501) staff       (20)      760 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/auth/http_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      547 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/auth/http_test.py
+-rw-r--r--   0 runner     (501) staff       (20)      477 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/auth/password.go
+-rw-r--r--   0 runner     (501) staff       (20)     1106 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/auth/password_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      847 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/auth/userpass.go
+-rw-r--r--   0 runner     (501) staff       (20)     1729 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/auth/userpass_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/correctnet/
+-rw-r--r--   0 runner     (501) staff       (20)     2064 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/correctnet/correctnet.go
+-rw-r--r--   0 runner     (501) staff       (20)     1436 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/go.mod
+-rw-r--r--   0 runner     (501) staff       (20)    10610 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/go.sum
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/masq/
+-rw-r--r--   0 runner     (501) staff       (20)     2865 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/masq/server.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/obfs/
+-rw-r--r--   0 runner     (501) staff       (20)     2915 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/obfs/conn.go
+-rw-r--r--   0 runner     (501) staff       (20)     1527 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/obfs/salamander.go
+-rw-r--r--   0 runner     (501) staff       (20)     1048 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/obfs/salamander_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/.mockery.yaml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/
+-rw-r--r--   0 runner     (501) staff       (20)     7738 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/compile.go
+-rw-r--r--   0 runner     (501) staff       (20)     6601 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/compile_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1468 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/matchers.go
+-rw-r--r--   0 runner     (501) staff       (20)     6123 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/matchers_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     4808 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/matchers_v2geo.go
+-rw-r--r--   0 runner     (501) staff       (20)     2489 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/matchers_v2geo_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1716 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/parse.go
+-rw-r--r--   0 runner     (501) staff       (20)     1611 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/parse_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/
+-rw-r--r--   0 runner     (501) staff       (20)  9640091 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/geoip.dat
+-rw-r--r--   0 runner     (501) staff       (20)  4143750 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/geosite.dat
+-rw-r--r--   0 runner     (501) staff       (20)     1080 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/load.go
+-rw-r--r--   0 runner     (501) staff       (20)     1348 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/load_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    21809 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1561 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.proto
+-rw-r--r--   0 runner     (501) staff       (20)     3266 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl.go
+-rw-r--r--   0 runner     (501) staff       (20)     1675 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1956 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/dns_https.go
+-rw-r--r--   0 runner     (501) staff       (20)     5508 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/dns_standard.go
+-rw-r--r--   0 runner     (501) staff       (20)     1053 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/dns_system.go
+-rw-r--r--   0 runner     (501) staff       (20)     3913 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/interface.go
+-rw-r--r--   0 runner     (501) staff       (20)     1225 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/interface_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     4044 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/mock_PluggableOutbound.go
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/mock_UDPConn.go
+-rw-r--r--   0 runner     (501) staff       (20)    11736 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_direct.go
+-rw-r--r--   0 runner     (501) staff       (20)     1287 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_direct_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      628 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_direct_others.go
+-rw-r--r--   0 runner     (501) staff       (20)     4596 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_http.go
+-rw-r--r--   0 runner     (501) staff       (20)     6928 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_socks5.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest/
+-rw-r--r--   0 runner     (501) staff       (20)     3031 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     3381 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest/protocol.go
+-rw-r--r--   0 runner     (501) staff       (20)     9544 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest/protocol_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2163 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest/server.go
+-rw-r--r--   0 runner     (501) staff       (20)      796 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest.go
+-rw-r--r--   0 runner     (501) staff       (20)      963 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/utils.go
+-rw-r--r--   0 runner     (501) staff       (20)     1603 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/outbounds/utils_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/trafficlogger/
+-rw-r--r--   0 runner     (501) staff       (20)     4053 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/trafficlogger/http.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2-go/extras/transport/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/extras/transport/udphop/
+-rw-r--r--   0 runner     (501) staff       (20)     1960 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/transport/udphop/addr.go
+-rw-r--r--   0 runner     (501) staff       (20)     2488 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/transport/udphop/addr_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6863 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/extras/transport/udphop/conn.go
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/go.work
+-rw-r--r--   0 runner     (501) staff       (20)    33613 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/go.work.sum
+-rw-r--r--   0 runner     (501) staff       (20)    14484 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/hyperbole.py
+-rw-r--r--   0 runner     (501) staff       (20)     2490 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/logo.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2-go/media-kit/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/
+-rw-r--r--   0 runner     (501) staff       (20)    18296 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/black 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    38595 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/black 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    19475 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/black 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    40667 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/black 4@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    17502 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/dark bg 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    37286 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/dark bg 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    18565 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/dark bg 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    38855 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/dark bg 4@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    18334 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/light bg 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    38791 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/light bg 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    19526 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/light bg 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    40734 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/light bg 4@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    12744 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/symbol 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    12395 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/symbol 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    12672 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/symbol 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    12013 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/symbol 4@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    17426 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/white 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    37014 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/white 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    18330 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/white 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    38461 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/png/white 4@2x.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/
+-rw-r--r--   0 runner     (501) staff       (20)     2126 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/black 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)    14333 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/black 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2427 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/black 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)    14626 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/black 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2347 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/dark bg 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)    15086 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/dark bg 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2662 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/dark bg 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)    15393 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/dark bg 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2189 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/light bg 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)    14396 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/light bg 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2490 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/light bg 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)    14689 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/light bg 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)      714 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/symbol 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/symbol 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)      651 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/symbol 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)      767 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/symbol 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2326 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/white 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)    15065 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/white 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2641 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/white 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)    15372 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/media-kit/svg/white 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)      488 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/platforms.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2-go/scripts/
+-rw-r--r--   0 runner     (501) staff       (20)       25 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/scripts/_redirects
+-rw-r--r--   0 runner     (501) staff       (20)    26403 2024-05-28 02:16:44.000000 hysteria2-2.4.4/hysteria2-go/scripts/install_server.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/hysteria2.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     5476 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    12013 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-05-28 02:17:10.000000 hysteria2-2.4.4/hysteria2.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    11911 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1684 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)        7 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/VERSION
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:10.000000 hysteria2-2.4.4/pybind11/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/pybind11/include/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    23979 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner     (501) staff       (20)     7069 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner     (501) staff       (20)    65638 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner     (501) staff       (20)     8458 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner     (501) staff       (20)      120 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     2096 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner     (501) staff       (20)    28251 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner     (501) staff       (20)    50369 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     5491 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner     (501) staff       (20)    17981 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner     (501) staff       (20)    25057 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner     (501) staff       (20)    42266 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner     (501) staff       (20)     1625 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner     (501) staff       (20)    32147 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner     (501) staff       (20)    11792 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner     (501) staff       (20)     4731 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner     (501) staff       (20)     4695 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner     (501) staff       (20)     8262 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner     (501) staff       (20)     8862 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner     (501) staff       (20)    79524 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner     (501) staff       (20)     9103 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner     (501) staff       (20)     2181 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner     (501) staff       (20)   125761 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner     (501) staff       (20)    93848 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner     (501) staff       (20)     4185 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner     (501) staff       (20)    15337 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner     (501) staff       (20)    27013 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/pybind11/tools/
+-rw-r--r--   0 runner     (501) staff       (20)     2350 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     3105 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner     (501) staff       (20)    11103 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner     (501) staff       (20)      817 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/JoinPaths.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     1423 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner     (501) staff       (20)      952 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner     (501) staff       (20)     1040 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner     (501) staff       (20)     1031 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/libsize.py
+-rw-r--r--   0 runner     (501) staff       (20)     1282 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner     (501) staff       (20)      196 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner     (501) staff       (20)    13487 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     6930 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner     (501) staff       (20)     8955 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     8359 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner     (501) staff       (20)       94 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)     1965 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner     (501) staff       (20)     1139 2024-05-28 02:16:44.000000 hysteria2-2.4.4/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-28 02:17:11.000000 hysteria2-2.4.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2742 2024-05-28 02:16:44.000000 hysteria2-2.4.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 02:17:11.000000 hysteria2-2.4.4/src/
+-rw-r--r--   0 runner     (501) staff       (20)      703 2024-05-28 02:16:44.000000 hysteria2-2.4.4/src/hysteria2.cpp
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `hysteria2-2.4.3/CMakeLists.txt` & `hysteria2-2.4.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/LICENSE` & `hysteria2-2.4.4/hysteria2-go/LICENSE.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-MIT License
+Copyright 2023 Toby
 
-Copyright (c) 2023 Loren Eteval
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hysteria2-2.4.3/PKG-INFO` & `hysteria2-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hysteria2
-Version: 2.4.3
+Version: 2.4.4
 Summary: Python bindings for hysteria2.
 Home-page: https://github.com/LorenEteval/hysteria2-python
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: MIT
 Description: # hysteria2-python
```

### Comparing `hysteria2-2.4.3/README.md` & `hysteria2-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.md` & `hysteria2-2.4.4/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.md` & `hysteria2-2.4.4/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.zh.md` & `hysteria2-2.4.4/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.zh.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/.github/workflows/docker.yml` & `hysteria2-2.4.4/hysteria2-go/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/.github/workflows/master.yml` & `hysteria2-2.4.4/hysteria2-go/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/.github/workflows/release.yml` & `hysteria2-2.4.4/hysteria2-go/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/.github/workflows/scripts.yml` & `hysteria2-2.4.4/hysteria2-go/.github/workflows/scripts.yml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/.gitignore` & `hysteria2-2.4.4/hysteria2-go/.gitignore`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/Dockerfile` & `hysteria2-2.4.4/hysteria2-go/Dockerfile`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/PROTOCOL.md` & `hysteria2-2.4.4/hysteria2-go/PROTOCOL.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/README.md` & `hysteria2-2.4.4/hysteria2-go/README.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/client.go` & `hysteria2-2.4.4/hysteria2-go/app/cmd/client.go`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 	"crypto/x509"
 	"encoding/hex"
 	"errors"
 	"fmt"
 	"net"
 	"net/netip"
 	"os"
+	"os/signal"
 	"runtime"
 	"slices"
 	"strconv"
 	"strings"
+	"syscall"
 	"time"
 
 	"github.com/spf13/cobra"
 	"github.com/spf13/viper"
 	"go.uber.org/zap"
 
 	"github.com/apernet/hysteria/app/internal/forwarding"
@@ -593,31 +595,60 @@
 	}
 	if config.TUN != nil {
 		runner.Add("TUN", func() error {
 			return clientTUN(*config.TUN, c)
 		})
 	}
 
-	runner.Run()
+	signalChan := make(chan os.Signal, 1)
+	signal.Notify(signalChan, os.Interrupt, syscall.SIGTERM)
+	defer signal.Stop(signalChan)
+
+	runnerChan := make(chan clientModeRunnerResult, 1)
+	go func() {
+		runnerChan <- runner.Run()
+	}()
+
+	select {
+	case <-signalChan:
+		logger.Info("received signal, shutting down gracefully")
+	case r := <-runnerChan:
+		if r.OK {
+			logger.Info(r.Msg)
+		} else {
+			_ = c.Close() // Close the client here as Fatal will exit the program without running defer
+			if r.Err != nil {
+				logger.Fatal(r.Msg, zap.Error(r.Err))
+			} else {
+				logger.Fatal(r.Msg)
+			}
+		}
+	}
 }
 
 type clientModeRunner struct {
 	ModeMap map[string]func() error
 }
 
+type clientModeRunnerResult struct {
+	OK  bool
+	Msg string
+	Err error
+}
+
 func (r *clientModeRunner) Add(name string, f func() error) {
 	if r.ModeMap == nil {
 		r.ModeMap = make(map[string]func() error)
 	}
 	r.ModeMap[name] = f
 }
 
-func (r *clientModeRunner) Run() {
+func (r *clientModeRunner) Run() clientModeRunnerResult {
 	if len(r.ModeMap) == 0 {
-		logger.Fatal("no mode specified")
+		return clientModeRunnerResult{OK: false, Msg: "no mode specified"}
 	}
 
 	type modeError struct {
 		Name string
 		Err  error
 	}
 	errChan := make(chan modeError, len(r.ModeMap))
@@ -627,17 +658,21 @@
 			errChan <- modeError{name, err}
 		}(name, f)
 	}
 	// Fatal if any one of the modes fails
 	for i := 0; i < len(r.ModeMap); i++ {
 		e := <-errChan
 		if e.Err != nil {
-			logger.Fatal("failed to run "+e.Name, zap.Error(e.Err))
+			return clientModeRunnerResult{OK: false, Msg: "failed to run " + e.Name, Err: e.Err}
 		}
 	}
+
+	// We don't really have any such cases, as currently none of our modes would stop on themselves without error.
+	// But we leave the possibility here for future expansion.
+	return clientModeRunnerResult{OK: true, Msg: "finished without error"}
 }
 
 func clientSOCKS5(config socks5Config, c client.Client) error {
 	if config.Listen == "" {
 		return configError{Field: "listen", Err: errors.New("listen address is empty")}
 	}
 	l, err := proxymux.ListenSOCKS(config.Listen)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/client_test.go` & `hysteria2-2.4.4/hysteria2-go/app/cmd/client_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/client_test.yaml` & `hysteria2-2.4.4/hysteria2-go/app/cmd/client_test.yaml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/ping.go` & `hysteria2-2.4.4/hysteria2-go/app/cmd/ping.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/root.go` & `hysteria2-2.4.4/hysteria2-go/app/cmd/root.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/server.go` & `hysteria2-2.4.4/hysteria2-go/app/cmd/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/server_test.go` & `hysteria2-2.4.4/hysteria2-go/app/cmd/server_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/server_test.yaml` & `hysteria2-2.4.4/hysteria2-go/app/cmd/server_test.yaml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/speedtest.go` & `hysteria2-2.4.4/hysteria2-go/app/cmd/speedtest.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/cmd/update.go` & `hysteria2-2.4.4/hysteria2-go/app/cmd/update.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/go.mod` & `hysteria2-2.4.4/hysteria2-go/app/go.mod`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	github.com/txthinking/socks5 v0.0.0-20230325130024-4230056ae301
 	go.uber.org/zap v1.24.0
 	golang.org/x/exp v0.0.0-20221205204356-47842c84f3db
 	golang.org/x/sys v0.19.0
 )
 
 require (
-	github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 // indirect
+	github.com/apernet/quic-go v0.43.1-0.20240515053213-5e9e635fd9f0 // indirect
 	github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6 // indirect
 	github.com/davecgh/go-spew v1.1.1 // indirect
 	github.com/fsnotify/fsnotify v1.7.0 // indirect
 	github.com/go-ole/go-ole v1.3.0 // indirect
 	github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 // indirect
 	github.com/google/pprof v0.0.0-20210407192527-94a9f03dee38 // indirect
 	github.com/hashicorp/golang-lru/v2 v2.0.5 // indirect
```

### Comparing `hysteria2-2.4.3/hysteria2-go/app/go.sum` & `hysteria2-2.4.4/hysteria2-go/app/go.sum`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 cloud.google.com/go/storage v1.10.0/go.mod h1:FLPqc6j+Ki4BU591ie1oL6qBQGu2Bl/tZ9ullr3+Kg0=
 cloud.google.com/go/storage v1.14.0/go.mod h1:GrKmX003DSIwi9o29oFT7YDnHYwZoctc3fOKtUw0Xmo=
 dmitri.shuralyov.com/gpu/mtl v0.0.0-20190408044501-666a987793e9/go.mod h1:H6x//7gZCb22OMCxBHrMx7a5I7Hp++hsVxbQ4BYO7hU=
 github.com/BurntSushi/toml v0.3.1/go.mod h1:xHWCNGjB5oqiDr8zfno3MHue2Ht5sIBksp03qcyfWMU=
 github.com/BurntSushi/xgb v0.0.0-20160522181843-27f122750802/go.mod h1:IVnqGOEym/WlBOVXweHU+Q+/VP0lqqI8lqeDx9IjBqo=
 github.com/apernet/go-tproxy v0.0.0-20230809025308-8f4723fd742f h1:uVh0qpEslrWjgzx9vOcyCqsOY3c9kofDZ1n+qaw35ZY=
 github.com/apernet/go-tproxy v0.0.0-20230809025308-8f4723fd742f/go.mod h1:xkkq9D4ygcldQQhKS/w9CadiCKwCngU7K9E3DaKahpM=
-github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 h1:ZfaQo52EyyhNCxfMNk64W1YHcIh+0rCkp3e0gR7BO5E=
-github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6/go.mod h1:j3QaAM7sVJqptDQyIQRWA6mASCfuxoHJszn67JQh1GE=
+github.com/apernet/quic-go v0.43.1-0.20240515053213-5e9e635fd9f0 h1:zilb2vx37DiBV5tfJRapxbXJqKavuCBKUl6kE4guShQ=
+github.com/apernet/quic-go v0.43.1-0.20240515053213-5e9e635fd9f0/go.mod h1:j3QaAM7sVJqptDQyIQRWA6mASCfuxoHJszn67JQh1GE=
 github.com/apernet/sing-tun v0.2.6-0.20240323130332-b9f6511036ad h1:QzQ2sKpc9o42HNRR8ukM5uMC/RzR2HgZd/Nvaqol2C0=
 github.com/apernet/sing-tun v0.2.6-0.20240323130332-b9f6511036ad/go.mod h1:S5IydyLSN/QAfvY+r2GoomPJ6hidtXWm/Ad18sJVssk=
 github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6 h1:4NNbNM2Iq/k57qEu7WfL67UrbPq1uFWxW4qODCohi+0=
 github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6/go.mod h1:J29hk+f9lJrblVIfiJOtTFk+OblBawmib4uz/VdKzlg=
 github.com/benbjohnson/clock v1.1.0 h1:Q92kusRqC1XV2MjkWETPvjJVqKetz1OzxZB7mHJLju8=
 github.com/benbjohnson/clock v1.1.0/go.mod h1:J11/hYXuz8f4ySSvYwY0FKfm+ezbsZBKZxNJlLklBHA=
 github.com/caddyserver/certmagic v0.17.2 h1:o30seC1T/dBqBCNNGNHWwj2i5/I/FMjBbTAhjADP3nE=
```

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/tcp.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/forwarding/tcp.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/tcp_test.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/forwarding/tcp_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/udp.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/forwarding/udp.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/udp_test.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/forwarding/udp_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/http/server.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/http/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/http/server_test.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/http/server_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/http/server_test.py` & `hysteria2-2.4.4/hysteria2-go/app/internal/http/server_test.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/http/test.crt` & `hysteria2-2.4.4/hysteria2-go/app/internal/http/test.crt`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/http/test.key` & `hysteria2-2.4.4/hysteria2-go/app/internal/http/test.key`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Conn.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Conn.go`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.42.2. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package mocks
 
 import (
 	net "net"
 
 	mock "github.com/stretchr/testify/mock"
```

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Listener.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Listener.go`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.42.2. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package mocks
 
 import (
 	net "net"
 
 	mock "github.com/stretchr/testify/mock"
```

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/manager.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/manager.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/manager_test.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/manager_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/mux.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/mux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/mux_test.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/proxymux/mux_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/redirect/getsockopt_linux_386.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/redirect/getsockopt_linux_386.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/redirect/tcp_linux.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/redirect/tcp_linux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/fd_control_unix_socket_test.py` & `hysteria2-2.4.4/hysteria2-go/app/internal/sockopts/fd_control_unix_socket_test.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/sockopts.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/sockopts/sockopts.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/sockopts_linux.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/sockopts/sockopts_linux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/sockopts_linux_test.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/sockopts/sockopts_linux_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/socks5/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server_test.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/socks5/server_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server_test.py` & `hysteria2-2.4.4/hysteria2-go/app/internal/socks5/server_test.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/tcp_linux.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/tproxy/tcp_linux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/udp_linux.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/tproxy/udp_linux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/tun/log.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/tun/log.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/tun/server.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/tun/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/url/url.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/url/url.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/url/url_test.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/url/url_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/utils/bpsconv.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/utils/bpsconv.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/utils/bpsconv_test.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/utils/bpsconv_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/utils/geoloader.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/utils/geoloader.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/utils/update.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/utils/update.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/internal/utils_test/mock.go` & `hysteria2-2.4.4/hysteria2-go/app/internal/utils_test/mock.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/app/misc/socks5_test.py` & `hysteria2-2.4.4/hysteria2-go/app/misc/socks5_test.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/client/client.go` & `hysteria2-2.4.4/hysteria2-go/core/client/client.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/client/config.go` & `hysteria2-2.4.4/hysteria2-go/core/client/config.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/client/mock_udpIO.go` & `hysteria2-2.4.4/hysteria2-go/core/client/mock_udpIO.go`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package client
 
 import (
 	protocol "github.com/apernet/hysteria/core/internal/protocol"
 	mock "github.com/stretchr/testify/mock"
 )
@@ -20,14 +20,18 @@
 	return &mockUDPIO_Expecter{mock: &_m.Mock}
 }
 
 // ReceiveMessage provides a mock function with given fields:
 func (_m *mockUDPIO) ReceiveMessage() (*protocol.UDPMessage, error) {
 	ret := _m.Called()
 
+	if len(ret) == 0 {
+		panic("no return value specified for ReceiveMessage")
+	}
+
 	var r0 *protocol.UDPMessage
 	var r1 error
 	if rf, ok := ret.Get(0).(func() (*protocol.UDPMessage, error)); ok {
 		return rf()
 	}
 	if rf, ok := ret.Get(0).(func() *protocol.UDPMessage); ok {
 		r0 = rf()
@@ -73,14 +77,18 @@
 	return _c
 }
 
 // SendMessage provides a mock function with given fields: _a0, _a1
 func (_m *mockUDPIO) SendMessage(_a0 []byte, _a1 *protocol.UDPMessage) error {
 	ret := _m.Called(_a0, _a1)
 
+	if len(ret) == 0 {
+		panic("no return value specified for SendMessage")
+	}
+
 	var r0 error
 	if rf, ok := ret.Get(0).(func([]byte, *protocol.UDPMessage) error); ok {
 		r0 = rf(_a0, _a1)
 	} else {
 		r0 = ret.Error(0)
 	}
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/client/reconnect.go` & `hysteria2-2.4.4/hysteria2-go/core/client/reconnect.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/client/udp.go` & `hysteria2-2.4.4/hysteria2-go/core/client/udp.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/client/udp_test.go` & `hysteria2-2.4.4/hysteria2-go/core/client/udp_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/errors/errors.go` & `hysteria2-2.4.4/hysteria2-go/core/errors/errors.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/go.mod` & `hysteria2-2.4.4/hysteria2-go/core/go.mod`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 module github.com/apernet/hysteria/core
 
 go 1.21
 
 require (
-	github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6
+	github.com/apernet/quic-go v0.43.1-0.20240515053213-5e9e635fd9f0
 	github.com/stretchr/testify v1.8.4
 	go.uber.org/goleak v1.2.1
 	golang.org/x/exp v0.0.0-20221205204356-47842c84f3db
 	golang.org/x/time v0.5.0
 )
 
 require (
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/go.sum` & `hysteria2-2.4.4/hysteria2-go/core/go.sum`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 h1:ZfaQo52EyyhNCxfMNk64W1YHcIh+0rCkp3e0gR7BO5E=
-github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6/go.mod h1:j3QaAM7sVJqptDQyIQRWA6mASCfuxoHJszn67JQh1GE=
+github.com/apernet/quic-go v0.43.1-0.20240515053213-5e9e635fd9f0 h1:zilb2vx37DiBV5tfJRapxbXJqKavuCBKUl6kE4guShQ=
+github.com/apernet/quic-go v0.43.1-0.20240515053213-5e9e635fd9f0/go.mod h1:j3QaAM7sVJqptDQyIQRWA6mASCfuxoHJszn67JQh1GE=
 github.com/chzyer/logex v1.1.10/go.mod h1:+Ywpsq7O8HXn0nuIou7OrIPyXbp3wmkHB+jjWRnGsAI=
 github.com/chzyer/readline v0.0.0-20180603132655-2972be24d48e/go.mod h1:nSuG5e5PlCu98SY8svDHJxuZscDgtXS6KTTbou5AhLI=
 github.com/chzyer/test v0.0.0-20180213035817-a1ea475d72b1/go.mod h1:Q3SI9o4m/ZMnBNeIyt5eFwwo7qiLfzFZmjNmxjkiQlU=
 github.com/creack/pty v1.1.9/go.mod h1:oKZEueFk5CKHvIhNR5MUki03XCEU+Q6VDXinZuGJ33E=
 github.com/davecgh/go-spew v1.1.0/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
 github.com/davecgh/go-spew v1.1.1 h1:vj9j/u1bqnvCEfJOwUhtlOARqs3+rkHYY13jYWTU97c=
 github.com/davecgh/go-spew v1.1.1/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bandwidth.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/bandwidth.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bandwidth_sampler.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/bandwidth_sampler.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bbr_sender.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/bbr_sender.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/packet_number_indexed_queue.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/packet_number_indexed_queue.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/ringbuffer.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/ringbuffer.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/windowed_filter.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/congestion/bbr/windowed_filter.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/brutal/brutal.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/congestion/brutal/brutal.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/common/pacer.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/congestion/common/pacer.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/frag/frag.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/frag/frag.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/frag/frag_test.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/frag/frag_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/.mockery.yaml` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/.mockery.yaml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/close_test.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/close_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/masq_test.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/masq_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Authenticator.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_Authenticator.go`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package mocks
 
 import (
 	net "net"
 
 	mock "github.com/stretchr/testify/mock"
@@ -21,14 +21,18 @@
 	return &MockAuthenticator_Expecter{mock: &_m.Mock}
 }
 
 // Authenticate provides a mock function with given fields: addr, auth, tx
 func (_m *MockAuthenticator) Authenticate(addr net.Addr, auth string, tx uint64) (bool, string) {
 	ret := _m.Called(addr, auth, tx)
 
+	if len(ret) == 0 {
+		panic("no return value specified for Authenticate")
+	}
+
 	var r0 bool
 	var r1 string
 	if rf, ok := ret.Get(0).(func(net.Addr, string, uint64) (bool, string)); ok {
 		return rf(addr, auth, tx)
 	}
 	if rf, ok := ret.Get(0).(func(net.Addr, string, uint64) bool); ok {
 		r0 = rf(addr, auth, tx)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Conn.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_Conn.go`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package mocks
 
 import (
 	net "net"
 
 	mock "github.com/stretchr/testify/mock"
@@ -23,14 +23,18 @@
 	return &MockConn_Expecter{mock: &_m.Mock}
 }
 
 // Close provides a mock function with given fields:
 func (_m *MockConn) Close() error {
 	ret := _m.Called()
 
+	if len(ret) == 0 {
+		panic("no return value specified for Close")
+	}
+
 	var r0 error
 	if rf, ok := ret.Get(0).(func() error); ok {
 		r0 = rf()
 	} else {
 		r0 = ret.Error(0)
 	}
 
@@ -64,14 +68,18 @@
 	return _c
 }
 
 // LocalAddr provides a mock function with given fields:
 func (_m *MockConn) LocalAddr() net.Addr {
 	ret := _m.Called()
 
+	if len(ret) == 0 {
+		panic("no return value specified for LocalAddr")
+	}
+
 	var r0 net.Addr
 	if rf, ok := ret.Get(0).(func() net.Addr); ok {
 		r0 = rf()
 	} else {
 		if ret.Get(0) != nil {
 			r0 = ret.Get(0).(net.Addr)
 		}
@@ -107,14 +115,18 @@
 	return _c
 }
 
 // Read provides a mock function with given fields: b
 func (_m *MockConn) Read(b []byte) (int, error) {
 	ret := _m.Called(b)
 
+	if len(ret) == 0 {
+		panic("no return value specified for Read")
+	}
+
 	var r0 int
 	var r1 error
 	if rf, ok := ret.Get(0).(func([]byte) (int, error)); ok {
 		return rf(b)
 	}
 	if rf, ok := ret.Get(0).(func([]byte) int); ok {
 		r0 = rf(b)
@@ -159,14 +171,18 @@
 	return _c
 }
 
 // RemoteAddr provides a mock function with given fields:
 func (_m *MockConn) RemoteAddr() net.Addr {
 	ret := _m.Called()
 
+	if len(ret) == 0 {
+		panic("no return value specified for RemoteAddr")
+	}
+
 	var r0 net.Addr
 	if rf, ok := ret.Get(0).(func() net.Addr); ok {
 		r0 = rf()
 	} else {
 		if ret.Get(0) != nil {
 			r0 = ret.Get(0).(net.Addr)
 		}
@@ -202,14 +218,18 @@
 	return _c
 }
 
 // SetDeadline provides a mock function with given fields: t
 func (_m *MockConn) SetDeadline(t time.Time) error {
 	ret := _m.Called(t)
 
+	if len(ret) == 0 {
+		panic("no return value specified for SetDeadline")
+	}
+
 	var r0 error
 	if rf, ok := ret.Get(0).(func(time.Time) error); ok {
 		r0 = rf(t)
 	} else {
 		r0 = ret.Error(0)
 	}
 
@@ -244,14 +264,18 @@
 	return _c
 }
 
 // SetReadDeadline provides a mock function with given fields: t
 func (_m *MockConn) SetReadDeadline(t time.Time) error {
 	ret := _m.Called(t)
 
+	if len(ret) == 0 {
+		panic("no return value specified for SetReadDeadline")
+	}
+
 	var r0 error
 	if rf, ok := ret.Get(0).(func(time.Time) error); ok {
 		r0 = rf(t)
 	} else {
 		r0 = ret.Error(0)
 	}
 
@@ -286,14 +310,18 @@
 	return _c
 }
 
 // SetWriteDeadline provides a mock function with given fields: t
 func (_m *MockConn) SetWriteDeadline(t time.Time) error {
 	ret := _m.Called(t)
 
+	if len(ret) == 0 {
+		panic("no return value specified for SetWriteDeadline")
+	}
+
 	var r0 error
 	if rf, ok := ret.Get(0).(func(time.Time) error); ok {
 		r0 = rf(t)
 	} else {
 		r0 = ret.Error(0)
 	}
 
@@ -328,14 +356,18 @@
 	return _c
 }
 
 // Write provides a mock function with given fields: b
 func (_m *MockConn) Write(b []byte) (int, error) {
 	ret := _m.Called(b)
 
+	if len(ret) == 0 {
+		panic("no return value specified for Write")
+	}
+
 	var r0 int
 	var r1 error
 	if rf, ok := ret.Get(0).(func([]byte) (int, error)); ok {
 		return rf(b)
 	}
 	if rf, ok := ret.Get(0).(func([]byte) int); ok {
 		r0 = rf(b)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_EventLogger.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_EventLogger.go`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package mocks
 
 import (
 	net "net"
 
 	mock "github.com/stretchr/testify/mock"
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Outbound.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_Outbound.go`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package mocks
 
 import (
 	net "net"
 
 	mock "github.com/stretchr/testify/mock"
@@ -23,14 +23,18 @@
 	return &MockOutbound_Expecter{mock: &_m.Mock}
 }
 
 // TCP provides a mock function with given fields: reqAddr
 func (_m *MockOutbound) TCP(reqAddr string) (net.Conn, error) {
 	ret := _m.Called(reqAddr)
 
+	if len(ret) == 0 {
+		panic("no return value specified for TCP")
+	}
+
 	var r0 net.Conn
 	var r1 error
 	if rf, ok := ret.Get(0).(func(string) (net.Conn, error)); ok {
 		return rf(reqAddr)
 	}
 	if rf, ok := ret.Get(0).(func(string) net.Conn); ok {
 		r0 = rf(reqAddr)
@@ -77,14 +81,18 @@
 	return _c
 }
 
 // UDP provides a mock function with given fields: reqAddr
 func (_m *MockOutbound) UDP(reqAddr string) (server.UDPConn, error) {
 	ret := _m.Called(reqAddr)
 
+	if len(ret) == 0 {
+		panic("no return value specified for UDP")
+	}
+
 	var r0 server.UDPConn
 	var r1 error
 	if rf, ok := ret.Get(0).(func(string) (server.UDPConn, error)); ok {
 		return rf(reqAddr)
 	}
 	if rf, ok := ret.Get(0).(func(string) server.UDPConn); ok {
 		r0 = rf(reqAddr)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_UDPConn.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/mocks/mock_UDPConn.go`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package mocks
 
 import mock "github.com/stretchr/testify/mock"
 
 // MockUDPConn is an autogenerated mock type for the UDPConn type
 type MockUDPConn struct {
@@ -17,14 +17,18 @@
 	return &MockUDPConn_Expecter{mock: &_m.Mock}
 }
 
 // Close provides a mock function with given fields:
 func (_m *MockUDPConn) Close() error {
 	ret := _m.Called()
 
+	if len(ret) == 0 {
+		panic("no return value specified for Close")
+	}
+
 	var r0 error
 	if rf, ok := ret.Get(0).(func() error); ok {
 		r0 = rf()
 	} else {
 		r0 = ret.Error(0)
 	}
 
@@ -58,14 +62,18 @@
 	return _c
 }
 
 // ReadFrom provides a mock function with given fields: b
 func (_m *MockUDPConn) ReadFrom(b []byte) (int, string, error) {
 	ret := _m.Called(b)
 
+	if len(ret) == 0 {
+		panic("no return value specified for ReadFrom")
+	}
+
 	var r0 int
 	var r1 string
 	var r2 error
 	if rf, ok := ret.Get(0).(func([]byte) (int, string, error)); ok {
 		return rf(b)
 	}
 	if rf, ok := ret.Get(0).(func([]byte) int); ok {
@@ -117,14 +125,18 @@
 	return _c
 }
 
 // WriteTo provides a mock function with given fields: b, addr
 func (_m *MockUDPConn) WriteTo(b []byte, addr string) (int, error) {
 	ret := _m.Called(b, addr)
 
+	if len(ret) == 0 {
+		panic("no return value specified for WriteTo")
+	}
+
 	var r0 int
 	var r1 error
 	if rf, ok := ret.Get(0).(func([]byte, string) (int, error)); ok {
 		return rf(b, addr)
 	}
 	if rf, ok := ret.Get(0).(func([]byte, string) int); ok {
 		r0 = rf(b, addr)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/smoke_test.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/smoke_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/stress_test.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/stress_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/test.crt` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/test.crt`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/test.key` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/test.key`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/trafficlogger_test.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/trafficlogger_test.go`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 		TrafficLogger: trafficLogger,
 	})
 	assert.NoError(t, err)
 	defer s.Close()
 	go s.Serve()
 
 	// Create client
+	trafficLogger.EXPECT().LogOnlineState("nobody", true).Return().Once()
 	c, _, err := client.NewClient(&client.Config{
 		ServerAddr: udpAddr,
 		TLSConfig:  client.TLSConfig{InsecureSkipVerify: true},
 	})
 	assert.NoError(t, err)
 	defer c.Close()
 
@@ -62,32 +63,33 @@
 	})
 	serverOb.EXPECT().TCP(addr).Return(sobConn, nil).Once()
 
 	conn, err := c.TCP(addr)
 	assert.NoError(t, err)
 
 	// Client reads from server
-	trafficLogger.EXPECT().Log("nobody", uint64(0), uint64(11)).Return(true).Once()
+	trafficLogger.EXPECT().LogTraffic("nobody", uint64(0), uint64(11)).Return(true).Once()
 	sobConnCh <- []byte("knock knock")
 	buf := make([]byte, 100)
 	n, err := conn.Read(buf)
 	assert.NoError(t, err)
 	assert.Equal(t, 11, n)
 	assert.Equal(t, "knock knock", string(buf[:n]))
 
 	// Client writes to server
-	trafficLogger.EXPECT().Log("nobody", uint64(12), uint64(0)).Return(true).Once()
+	trafficLogger.EXPECT().LogTraffic("nobody", uint64(12), uint64(0)).Return(true).Once()
 	sobConn.EXPECT().Write([]byte("who is there")).Return(12, nil).Once()
 	n, err = conn.Write([]byte("who is there"))
 	assert.NoError(t, err)
 	assert.Equal(t, 12, n)
 	time.Sleep(1 * time.Second) // Need some time for the server to receive the data
 
 	// Client reads from server again but blocked
-	trafficLogger.EXPECT().Log("nobody", uint64(0), uint64(4)).Return(false).Once()
+	trafficLogger.EXPECT().LogTraffic("nobody", uint64(0), uint64(4)).Return(false).Once()
+	trafficLogger.EXPECT().LogOnlineState("nobody", false).Return().Once()
 	sobConnCh <- []byte("nope")
 	n, err = conn.Read(buf)
 	assert.Zero(t, n)
 	assert.Error(t, err)
 
 	// The client should be disconnected
 	_, err = c.TCP("whatever")
@@ -112,14 +114,15 @@
 		TrafficLogger: trafficLogger,
 	})
 	assert.NoError(t, err)
 	defer s.Close()
 	go s.Serve()
 
 	// Create client
+	trafficLogger.EXPECT().LogOnlineState("nobody", true).Return().Once()
 	c, _, err := client.NewClient(&client.Config{
 		ServerAddr: udpAddr,
 		TLSConfig:  client.TLSConfig{InsecureSkipVerify: true},
 	})
 	assert.NoError(t, err)
 	defer c.Close()
 
@@ -142,30 +145,31 @@
 	})
 	serverOb.EXPECT().UDP(addr).Return(sobConn, nil).Once()
 
 	conn, err := c.UDP()
 	assert.NoError(t, err)
 
 	// Client writes to server
-	trafficLogger.EXPECT().Log("nobody", uint64(9), uint64(0)).Return(true).Once()
+	trafficLogger.EXPECT().LogTraffic("nobody", uint64(9), uint64(0)).Return(true).Once()
 	sobConn.EXPECT().WriteTo([]byte("small sad"), addr).Return(9, nil).Once()
 	err = conn.Send([]byte("small sad"), addr)
 	assert.NoError(t, err)
 	time.Sleep(1 * time.Second) // Need some time for the server to receive the data
 
 	// Client reads from server
-	trafficLogger.EXPECT().Log("nobody", uint64(0), uint64(7)).Return(true).Once()
+	trafficLogger.EXPECT().LogTraffic("nobody", uint64(0), uint64(7)).Return(true).Once()
 	sobConnCh <- []byte("big mad")
 	bs, rAddr, err := conn.Receive()
 	assert.NoError(t, err)
 	assert.Equal(t, rAddr, addr)
 	assert.Equal(t, "big mad", string(bs))
 
 	// Client reads from server again but blocked
-	trafficLogger.EXPECT().Log("nobody", uint64(0), uint64(4)).Return(false).Once()
+	trafficLogger.EXPECT().LogTraffic("nobody", uint64(0), uint64(4)).Return(false).Once()
+	trafficLogger.EXPECT().LogOnlineState("nobody", false).Return().Once()
 	sobConnCh <- []byte("nope")
 	bs, rAddr, err = conn.Receive()
 	assert.Equal(t, err, io.EOF)
 	assert.Empty(t, rAddr)
 	assert.Empty(t, bs)
 
 	// The client should be disconnected
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/utils_test.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/integration_tests/utils_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/protocol/http.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/protocol/http.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/protocol/padding.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/protocol/padding.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/protocol/proxy.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/protocol/proxy.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/protocol/proxy_test.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/protocol/proxy_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/internal/utils/qstream.go` & `hysteria2-2.4.4/hysteria2-go/core/internal/utils/qstream.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/server/config.go` & `hysteria2-2.4.4/hysteria2-go/core/server/config.go`

 * *Files 1% similar despite different names*

```diff
@@ -191,9 +191,10 @@
 // Tx is the bytes sent from the server to the remote.
 // Rx is the bytes received by the server from the remote.
 // Apart from logging, the Log function can also return false to signal
 // that the client should be disconnected. This can be used to implement
 // bandwidth limits or post-connection authentication, for example.
 // The implementation of this interface must be thread-safe.
 type TrafficLogger interface {
-	Log(id string, tx, rx uint64) (ok bool)
+	LogTraffic(id string, tx, rx uint64) (ok bool)
+	LogOnlineState(id string, online bool)
 }
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/server/copy.go` & `hysteria2-2.4.4/hysteria2-go/core/server/copy.go`

 * *Files 15% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 	}
 }
 
 func copyTwoWayWithLogger(id string, serverRw, remoteRw io.ReadWriter, l TrafficLogger) error {
 	errChan := make(chan error, 2)
 	go func() {
 		errChan <- copyBufferLog(serverRw, remoteRw, func(n uint64) bool {
-			return l.Log(id, 0, n)
+			return l.LogTraffic(id, 0, n)
 		})
 	}()
 	go func() {
 		errChan <- copyBufferLog(remoteRw, serverRw, func(n uint64) bool {
-			return l.Log(id, n, 0)
+			return l.LogTraffic(id, n, 0)
 		})
 	}()
 	// Block until one of the two goroutines returns
 	return <-errChan
 }
 
 // copyTwoWay is the "fast-path" version of copyTwoWayWithLogger that does not log traffic.
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/server/mock_UDPConn.go` & `hysteria2-2.4.4/hysteria2-go/core/server/mock_UDPConn.go`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package server
 
 import mock "github.com/stretchr/testify/mock"
 
 // mockUDPConn is an autogenerated mock type for the UDPConn type
 type mockUDPConn struct {
@@ -17,14 +17,18 @@
 	return &mockUDPConn_Expecter{mock: &_m.Mock}
 }
 
 // Close provides a mock function with given fields:
 func (_m *mockUDPConn) Close() error {
 	ret := _m.Called()
 
+	if len(ret) == 0 {
+		panic("no return value specified for Close")
+	}
+
 	var r0 error
 	if rf, ok := ret.Get(0).(func() error); ok {
 		r0 = rf()
 	} else {
 		r0 = ret.Error(0)
 	}
 
@@ -58,14 +62,18 @@
 	return _c
 }
 
 // ReadFrom provides a mock function with given fields: b
 func (_m *mockUDPConn) ReadFrom(b []byte) (int, string, error) {
 	ret := _m.Called(b)
 
+	if len(ret) == 0 {
+		panic("no return value specified for ReadFrom")
+	}
+
 	var r0 int
 	var r1 string
 	var r2 error
 	if rf, ok := ret.Get(0).(func([]byte) (int, string, error)); ok {
 		return rf(b)
 	}
 	if rf, ok := ret.Get(0).(func([]byte) int); ok {
@@ -117,14 +125,18 @@
 	return _c
 }
 
 // WriteTo provides a mock function with given fields: b, addr
 func (_m *mockUDPConn) WriteTo(b []byte, addr string) (int, error) {
 	ret := _m.Called(b, addr)
 
+	if len(ret) == 0 {
+		panic("no return value specified for WriteTo")
+	}
+
 	var r0 int
 	var r1 error
 	if rf, ok := ret.Get(0).(func([]byte, string) (int, error)); ok {
 		return rf(b, addr)
 	}
 	if rf, ok := ret.Get(0).(func([]byte, string) int); ok {
 		r0 = rf(b, addr)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/server/mock_udpEventLogger.go` & `hysteria2-2.4.4/hysteria2-go/core/server/mock_udpEventLogger.go`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package server
 
 import mock "github.com/stretchr/testify/mock"
 
 // mockUDPEventLogger is an autogenerated mock type for the udpEventLogger type
 type mockUDPEventLogger struct {
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/server/mock_udpIO.go` & `hysteria2-2.4.4/hysteria2-go/core/server/mock_udpIO.go`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package server
 
 import (
 	protocol "github.com/apernet/hysteria/core/internal/protocol"
 	mock "github.com/stretchr/testify/mock"
 )
@@ -20,14 +20,18 @@
 	return &mockUDPIO_Expecter{mock: &_m.Mock}
 }
 
 // ReceiveMessage provides a mock function with given fields:
 func (_m *mockUDPIO) ReceiveMessage() (*protocol.UDPMessage, error) {
 	ret := _m.Called()
 
+	if len(ret) == 0 {
+		panic("no return value specified for ReceiveMessage")
+	}
+
 	var r0 *protocol.UDPMessage
 	var r1 error
 	if rf, ok := ret.Get(0).(func() (*protocol.UDPMessage, error)); ok {
 		return rf()
 	}
 	if rf, ok := ret.Get(0).(func() *protocol.UDPMessage); ok {
 		r0 = rf()
@@ -73,14 +77,18 @@
 	return _c
 }
 
 // SendMessage provides a mock function with given fields: _a0, _a1
 func (_m *mockUDPIO) SendMessage(_a0 []byte, _a1 *protocol.UDPMessage) error {
 	ret := _m.Called(_a0, _a1)
 
+	if len(ret) == 0 {
+		panic("no return value specified for SendMessage")
+	}
+
 	var r0 error
 	if rf, ok := ret.Get(0).(func([]byte, *protocol.UDPMessage) error); ok {
 		r0 = rf(_a0, _a1)
 	} else {
 		r0 = ret.Error(0)
 	}
 
@@ -116,14 +124,18 @@
 	return _c
 }
 
 // UDP provides a mock function with given fields: reqAddr
 func (_m *mockUDPIO) UDP(reqAddr string) (UDPConn, error) {
 	ret := _m.Called(reqAddr)
 
+	if len(ret) == 0 {
+		panic("no return value specified for UDP")
+	}
+
 	var r0 UDPConn
 	var r1 error
 	if rf, ok := ret.Get(0).(func(string) (UDPConn, error)); ok {
 		return rf(reqAddr)
 	}
 	if rf, ok := ret.Get(0).(func(string) UDPConn); ok {
 		r0 = rf(reqAddr)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/server/server.go` & `hysteria2-2.4.4/hysteria2-go/core/server/server.go`

 * *Files 8% similar despite different names*

```diff
@@ -78,16 +78,21 @@
 	handler := newH3sHandler(s.config, conn)
 	h3s := http3.Server{
 		Handler:        handler,
 		StreamHijacker: handler.ProxyStreamHijacker,
 	}
 	err := h3s.ServeQUICConn(conn)
 	// If the client is authenticated, we need to log the disconnect event
-	if handler.authenticated && s.config.EventLogger != nil {
-		s.config.EventLogger.Disconnect(conn.RemoteAddr(), handler.authID, err)
+	if handler.authenticated {
+		if tl := s.config.TrafficLogger; tl != nil {
+			tl.LogOnlineState(handler.authID, false)
+		}
+		if el := s.config.EventLogger; el != nil {
+			el.Disconnect(conn.RemoteAddr(), handler.authID, err)
+		}
 	}
 	_ = conn.CloseWithError(closeErrCodeOK, "")
 }
 
 type h3sHandler struct {
 	config *Config
 	conn   quic.Connection
@@ -149,16 +154,19 @@
 			protocol.AuthResponseToHeader(w.Header(), protocol.AuthResponse{
 				UDPEnabled: !h.config.DisableUDP,
 				Rx:         h.config.BandwidthConfig.MaxRx,
 				RxAuto:     h.config.IgnoreClientBandwidth,
 			})
 			w.WriteHeader(protocol.StatusAuthOK)
 			// Call event logger
-			if h.config.EventLogger != nil {
-				h.config.EventLogger.Connect(h.conn.RemoteAddr(), id, actualTx)
+			if tl := h.config.TrafficLogger; tl != nil {
+				tl.LogOnlineState(id, true)
+			}
+			if el := h.config.EventLogger; el != nil {
+				el.Connect(h.conn.RemoteAddr(), id, actualTx)
 			}
 			// Initialize UDP session manager (if UDP is enabled)
 			// We use sync.Once to make sure that only one goroutine is started,
 			// as ServeHTTP may be called by multiple goroutines simultaneously
 			if !h.config.DisableUDP {
 				go func() {
 					sm := newUDPSessionManager(
@@ -264,28 +272,28 @@
 		}
 		udpMsg, err := protocol.ParseUDPMessage(msg)
 		if err != nil {
 			// Invalid message, this is fine - just wait for the next
 			continue
 		}
 		if io.TrafficLogger != nil {
-			ok := io.TrafficLogger.Log(io.AuthID, uint64(len(udpMsg.Data)), 0)
+			ok := io.TrafficLogger.LogTraffic(io.AuthID, uint64(len(udpMsg.Data)), 0)
 			if !ok {
 				// TrafficLogger requested to disconnect the client
 				_ = io.Conn.CloseWithError(closeErrCodeTrafficLimitReached, "")
 				return nil, errDisconnect
 			}
 		}
 		return udpMsg, nil
 	}
 }
 
 func (io *udpIOImpl) SendMessage(buf []byte, msg *protocol.UDPMessage) error {
 	if io.TrafficLogger != nil {
-		ok := io.TrafficLogger.Log(io.AuthID, 0, uint64(len(msg.Data)))
+		ok := io.TrafficLogger.LogTraffic(io.AuthID, 0, uint64(len(msg.Data)))
 		if !ok {
 			// TrafficLogger requested to disconnect the client
 			_ = io.Conn.CloseWithError(closeErrCodeTrafficLimitReached, "")
 			return errDisconnect
 		}
 	}
 	msgN := msg.Serialize(buf)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/core/server/udp.go` & `hysteria2-2.4.4/hysteria2-go/core/server/udp.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/core/server/udp_test.go` & `hysteria2-2.4.4/hysteria2-go/core/server/udp_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/auth/command.go` & `hysteria2-2.4.4/hysteria2-go/extras/auth/command.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/auth/http.go` & `hysteria2-2.4.4/hysteria2-go/extras/auth/http.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/auth/http_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/auth/http_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/auth/http_test.py` & `hysteria2-2.4.4/hysteria2-go/extras/auth/http_test.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/auth/password_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/auth/password_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/auth/userpass.go` & `hysteria2-2.4.4/hysteria2-go/extras/auth/userpass.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/auth/userpass_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/auth/userpass_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/correctnet/correctnet.go` & `hysteria2-2.4.4/hysteria2-go/extras/correctnet/correctnet.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/go.mod` & `hysteria2-2.4.4/hysteria2-go/extras/go.mod`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	github.com/txthinking/socks5 v0.0.0-20230325130024-4230056ae301
 	golang.org/x/crypto v0.22.0
 	golang.org/x/net v0.24.0
 	google.golang.org/protobuf v1.33.0
 )
 
 require (
-	github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 // indirect
+	github.com/apernet/quic-go v0.43.1-0.20240515053213-5e9e635fd9f0 // indirect
 	github.com/davecgh/go-spew v1.1.1 // indirect
 	github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 // indirect
 	github.com/google/pprof v0.0.0-20210407192527-94a9f03dee38 // indirect
 	github.com/onsi/ginkgo/v2 v2.9.5 // indirect
 	github.com/patrickmn/go-cache v2.1.0+incompatible // indirect
 	github.com/pmezard/go-difflib v1.0.0 // indirect
 	github.com/quic-go/qpack v0.4.0 // indirect
```

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/go.sum` & `hysteria2-2.4.4/hysteria2-go/extras/go.sum`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 h1:ZfaQo52EyyhNCxfMNk64W1YHcIh+0rCkp3e0gR7BO5E=
-github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6/go.mod h1:j3QaAM7sVJqptDQyIQRWA6mASCfuxoHJszn67JQh1GE=
+github.com/apernet/quic-go v0.43.1-0.20240515053213-5e9e635fd9f0 h1:zilb2vx37DiBV5tfJRapxbXJqKavuCBKUl6kE4guShQ=
+github.com/apernet/quic-go v0.43.1-0.20240515053213-5e9e635fd9f0/go.mod h1:j3QaAM7sVJqptDQyIQRWA6mASCfuxoHJszn67JQh1GE=
 github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6 h1:4NNbNM2Iq/k57qEu7WfL67UrbPq1uFWxW4qODCohi+0=
 github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6/go.mod h1:J29hk+f9lJrblVIfiJOtTFk+OblBawmib4uz/VdKzlg=
 github.com/chzyer/logex v1.1.10/go.mod h1:+Ywpsq7O8HXn0nuIou7OrIPyXbp3wmkHB+jjWRnGsAI=
 github.com/chzyer/readline v0.0.0-20180603132655-2972be24d48e/go.mod h1:nSuG5e5PlCu98SY8svDHJxuZscDgtXS6KTTbou5AhLI=
 github.com/chzyer/test v0.0.0-20180213035817-a1ea475d72b1/go.mod h1:Q3SI9o4m/ZMnBNeIyt5eFwwo7qiLfzFZmjNmxjkiQlU=
 github.com/davecgh/go-spew v1.1.0/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
 github.com/davecgh/go-spew v1.1.1 h1:vj9j/u1bqnvCEfJOwUhtlOARqs3+rkHYY13jYWTU97c=
```

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/masq/server.go` & `hysteria2-2.4.4/hysteria2-go/extras/masq/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/obfs/conn.go` & `hysteria2-2.4.4/hysteria2-go/extras/obfs/conn.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/obfs/salamander.go` & `hysteria2-2.4.4/hysteria2-go/extras/obfs/salamander.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/obfs/salamander_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/obfs/salamander_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/compile.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/compile.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/compile_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/compile_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/matchers.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/matchers_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_v2geo.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/matchers_v2geo.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_v2geo_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/matchers_v2geo_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/parse.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/parse.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/parse_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/parse_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/geoip.dat` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/geoip.dat`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/geosite.dat` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/geosite.dat`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/load.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/load.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/load_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/load_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.pb.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.pb.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.proto` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.proto`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/acl_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_https.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/dns_https.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_standard.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/dns_standard.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_system.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/dns_system.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/interface.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/interface.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/interface_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/interface_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/mock_PluggableOutbound.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/mock_PluggableOutbound.go`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package outbounds
 
 import (
 	net "net"
 
 	mock "github.com/stretchr/testify/mock"
@@ -21,14 +21,18 @@
 	return &mockPluggableOutbound_Expecter{mock: &_m.Mock}
 }
 
 // TCP provides a mock function with given fields: reqAddr
 func (_m *mockPluggableOutbound) TCP(reqAddr *AddrEx) (net.Conn, error) {
 	ret := _m.Called(reqAddr)
 
+	if len(ret) == 0 {
+		panic("no return value specified for TCP")
+	}
+
 	var r0 net.Conn
 	var r1 error
 	if rf, ok := ret.Get(0).(func(*AddrEx) (net.Conn, error)); ok {
 		return rf(reqAddr)
 	}
 	if rf, ok := ret.Get(0).(func(*AddrEx) net.Conn); ok {
 		r0 = rf(reqAddr)
@@ -75,14 +79,18 @@
 	return _c
 }
 
 // UDP provides a mock function with given fields: reqAddr
 func (_m *mockPluggableOutbound) UDP(reqAddr *AddrEx) (UDPConn, error) {
 	ret := _m.Called(reqAddr)
 
+	if len(ret) == 0 {
+		panic("no return value specified for UDP")
+	}
+
 	var r0 UDPConn
 	var r1 error
 	if rf, ok := ret.Get(0).(func(*AddrEx) (UDPConn, error)); ok {
 		return rf(reqAddr)
 	}
 	if rf, ok := ret.Get(0).(func(*AddrEx) UDPConn); ok {
 		r0 = rf(reqAddr)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/mock_UDPConn.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/mock_UDPConn.go`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Code generated by mockery v2.32.0. DO NOT EDIT.
+// Code generated by mockery v2.43.0. DO NOT EDIT.
 
 package outbounds
 
 import mock "github.com/stretchr/testify/mock"
 
 // mockUDPConn is an autogenerated mock type for the UDPConn type
 type mockUDPConn struct {
@@ -17,14 +17,18 @@
 	return &mockUDPConn_Expecter{mock: &_m.Mock}
 }
 
 // Close provides a mock function with given fields:
 func (_m *mockUDPConn) Close() error {
 	ret := _m.Called()
 
+	if len(ret) == 0 {
+		panic("no return value specified for Close")
+	}
+
 	var r0 error
 	if rf, ok := ret.Get(0).(func() error); ok {
 		r0 = rf()
 	} else {
 		r0 = ret.Error(0)
 	}
 
@@ -58,14 +62,18 @@
 	return _c
 }
 
 // ReadFrom provides a mock function with given fields: b
 func (_m *mockUDPConn) ReadFrom(b []byte) (int, *AddrEx, error) {
 	ret := _m.Called(b)
 
+	if len(ret) == 0 {
+		panic("no return value specified for ReadFrom")
+	}
+
 	var r0 int
 	var r1 *AddrEx
 	var r2 error
 	if rf, ok := ret.Get(0).(func([]byte) (int, *AddrEx, error)); ok {
 		return rf(b)
 	}
 	if rf, ok := ret.Get(0).(func([]byte) int); ok {
@@ -119,14 +127,18 @@
 	return _c
 }
 
 // WriteTo provides a mock function with given fields: b, addr
 func (_m *mockUDPConn) WriteTo(b []byte, addr *AddrEx) (int, error) {
 	ret := _m.Called(b, addr)
 
+	if len(ret) == 0 {
+		panic("no return value specified for WriteTo")
+	}
+
 	var r0 int
 	var r1 error
 	if rf, ok := ret.Get(0).(func([]byte, *AddrEx) (int, error)); ok {
 		return rf(b, addr)
 	}
 	if rf, ok := ret.Get(0).(func([]byte, *AddrEx) int); ok {
 		r0 = rf(b, addr)
```

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_direct.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct_linux.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_direct_linux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct_others.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_direct_others.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_http.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_http.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_socks5.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/ob_socks5.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/client.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest/client.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/protocol.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest/protocol.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/protocol_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest/protocol_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/server.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/speedtest.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/utils.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/utils.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/outbounds/utils_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/outbounds/utils_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/trafficlogger/http.go` & `hysteria2-2.4.4/hysteria2-go/extras/trafficlogger/http.go`

 * *Files 11% similar despite different names*

```diff
@@ -18,33 +18,35 @@
 type TrafficStatsServer interface {
 	server.TrafficLogger
 	http.Handler
 }
 
 func NewTrafficStatsServer(secret string) TrafficStatsServer {
 	return &trafficStatsServerImpl{
-		StatsMap: make(map[string]*trafficStatsEntry),
-		KickMap:  make(map[string]struct{}),
-		Secret:   secret,
+		StatsMap:  make(map[string]*trafficStatsEntry),
+		KickMap:   make(map[string]struct{}),
+		OnlineMap: make(map[string]int),
+		Secret:    secret,
 	}
 }
 
 type trafficStatsServerImpl struct {
-	Mutex    sync.RWMutex
-	StatsMap map[string]*trafficStatsEntry
-	KickMap  map[string]struct{}
-	Secret   string
+	Mutex     sync.RWMutex
+	StatsMap  map[string]*trafficStatsEntry
+	OnlineMap map[string]int
+	KickMap   map[string]struct{}
+	Secret    string
 }
 
 type trafficStatsEntry struct {
 	Tx uint64 `json:"tx"`
 	Rx uint64 `json:"rx"`
 }
 
-func (s *trafficStatsServerImpl) Log(id string, tx, rx uint64) (ok bool) {
+func (s *trafficStatsServerImpl) LogTraffic(id string, tx, rx uint64) (ok bool) {
 	s.Mutex.Lock()
 	defer s.Mutex.Unlock()
 
 	_, ok = s.KickMap[id]
 	if ok {
 		delete(s.KickMap, id)
 		return false
@@ -57,14 +59,29 @@
 	}
 	entry.Tx += tx
 	entry.Rx += rx
 
 	return true
 }
 
+// LogOnlineStateChanged updates the online state to the online map.
+func (s *trafficStatsServerImpl) LogOnlineState(id string, online bool) {
+	s.Mutex.Lock()
+	defer s.Mutex.Unlock()
+
+	if online {
+		s.OnlineMap[id]++
+	} else {
+		s.OnlineMap[id]--
+		if s.OnlineMap[id] <= 0 {
+			delete(s.OnlineMap, id)
+		}
+	}
+}
+
 func (s *trafficStatsServerImpl) ServeHTTP(w http.ResponseWriter, r *http.Request) {
 	if s.Secret != "" && r.Header.Get("Authorization") != s.Secret {
 		http.Error(w, "unauthorized", http.StatusUnauthorized)
 		return
 	}
 	if r.Method == http.MethodGet && r.URL.Path == "/" {
 		_, _ = w.Write([]byte(indexHTML))
@@ -74,14 +91,18 @@
 		s.getTraffic(w, r)
 		return
 	}
 	if r.Method == http.MethodPost && r.URL.Path == "/kick" {
 		s.kick(w, r)
 		return
 	}
+	if r.Method == http.MethodGet && r.URL.Path == "/online" {
+		s.getOnline(w, r)
+		return
+	}
 	http.NotFound(w, r)
 }
 
 func (s *trafficStatsServerImpl) getTraffic(w http.ResponseWriter, r *http.Request) {
 	bClear, _ := strconv.ParseBool(r.URL.Query().Get("clear"))
 	var jb []byte
 	var err error
@@ -98,14 +119,27 @@
 	if err != nil {
 		http.Error(w, err.Error(), http.StatusInternalServerError)
 		return
 	}
 	w.Header().Set("Content-Type", "application/json; charset=utf-8")
 	_, _ = w.Write(jb)
 }
+
+func (s *trafficStatsServerImpl) getOnline(w http.ResponseWriter, r *http.Request) {
+	s.Mutex.RLock()
+	defer s.Mutex.RUnlock()
+
+	jb, err := json.Marshal(s.OnlineMap)
+	if err != nil {
+		http.Error(w, err.Error(), http.StatusInternalServerError)
+		return
+	}
+	w.Header().Set("Content-Type", "application/json; charset=utf-8")
+	_, _ = w.Write(jb)
+}
 
 func (s *trafficStatsServerImpl) kick(w http.ResponseWriter, r *http.Request) {
 	var ids []string
 	err := json.NewDecoder(r.Body).Decode(&ids)
 	if err != nil {
 		http.Error(w, err.Error(), http.StatusBadRequest)
 		return
```

#### html2text {}

```diff
@@ -3,34 +3,44 @@
 This is a Hysteria Traffic Stats API server.
 Check the documentation for usage.
 ` ) // TrafficStatsServer implements both server.TrafficLogger and http.Handler
 // to provide a simple HTTP API to get the traffic stats per user. type
 TrafficStatsServer interface { server.TrafficLogger http.Handler } func
 NewTrafficStatsServer(secret string) TrafficStatsServer { return
 &trafficStatsServerImpl{ StatsMap: make(map[string]*trafficStatsEntry),
-KickMap: make(map[string]struct{}), Secret: secret, } } type
-trafficStatsServerImpl struct { Mutex sync.RWMutex StatsMap map
-[string]*trafficStatsEntry KickMap map[string]struct{} Secret string } type
-trafficStatsEntry struct { Tx uint64 `json:"tx"` Rx uint64 `json:"rx"` } func
-(s *trafficStatsServerImpl) Log(id string, tx, rx uint64) (ok bool)
-{ s.Mutex.Lock() defer s.Mutex.Unlock() _, ok = s.KickMap[id] if ok { delete
-(s.KickMap, id) return false } entry, ok := s.StatsMap[id] if !ok { entry =
-&trafficStatsEntry{} s.StatsMap[id] = entry } entry.Tx += tx entry.Rx += rx
-return true } func (s *trafficStatsServerImpl) ServeHTTP(w http.ResponseWriter,
-r *http.Request) { if s.Secret != "" && r.Header.Get("Authorization") !=
-s.Secret { http.Error(w, "unauthorized", http.StatusUnauthorized) return } if
-r.Method == http.MethodGet && r.URL.Path == "/" { _, _ = w.Write([]byte
-(indexHTML)) return } if r.Method == http.MethodGet && r.URL.Path == "/traffic"
-{ s.getTraffic(w, r) return } if r.Method == http.MethodPost && r.URL.Path ==
-"/kick" { s.kick(w, r) return } http.NotFound(w, r) } func (s
-*trafficStatsServerImpl) getTraffic(w http.ResponseWriter, r *http.Request)
-{ bClear, _ := strconv.ParseBool(r.URL.Query().Get("clear")) var jb []byte var
-err error if bClear { s.Mutex.Lock() jb, err = json.Marshal(s.StatsMap)
-s.StatsMap = make(map[string]*trafficStatsEntry) s.Mutex.Unlock() } else
-{ s.Mutex.RLock() jb, err = json.Marshal(s.StatsMap) s.Mutex.RUnlock() } if err
-!= nil { http.Error(w, err.Error(), http.StatusInternalServerError) return }
-w.Header().Set("Content-Type", "application/json; charset=utf-8") _, _ =
-w.Write(jb) } func (s *trafficStatsServerImpl) kick(w http.ResponseWriter, r
+KickMap: make(map[string]struct{}), OnlineMap: make(map[string]int), Secret:
+secret, } } type trafficStatsServerImpl struct { Mutex sync.RWMutex StatsMap
+map[string]*trafficStatsEntry OnlineMap map[string]int KickMap map
+[string]struct{} Secret string } type trafficStatsEntry struct { Tx uint64
+`json:"tx"` Rx uint64 `json:"rx"` } func (s *trafficStatsServerImpl) LogTraffic
+(id string, tx, rx uint64) (ok bool) { s.Mutex.Lock() defer s.Mutex.Unlock() _,
+ok = s.KickMap[id] if ok { delete(s.KickMap, id) return false } entry, ok :
+= s.StatsMap[id] if !ok { entry = &trafficStatsEntry{} s.StatsMap[id] = entry }
+entry.Tx += tx entry.Rx += rx return true } // LogOnlineStateChanged updates
+the online state to the online map. func (s *trafficStatsServerImpl)
+LogOnlineState(id string, online bool) { s.Mutex.Lock() defer s.Mutex.Unlock()
+if online { s.OnlineMap[id]++ } else { s.OnlineMap[id]-- if s.OnlineMap[id] <=
+0 { delete(s.OnlineMap, id) } } } func (s *trafficStatsServerImpl) ServeHTTP(w
+http.ResponseWriter, r *http.Request) { if s.Secret != "" && r.Header.Get
+("Authorization") != s.Secret { http.Error(w, "unauthorized",
+http.StatusUnauthorized) return } if r.Method == http.MethodGet && r.URL.Path
+== "/" { _, _ = w.Write([]byte(indexHTML)) return } if r.Method ==
+http.MethodGet && r.URL.Path == "/traffic" { s.getTraffic(w, r) return } if
+r.Method == http.MethodPost && r.URL.Path == "/kick" { s.kick(w, r) return } if
+r.Method == http.MethodGet && r.URL.Path == "/online" { s.getOnline(w, r)
+return } http.NotFound(w, r) } func (s *trafficStatsServerImpl) getTraffic(w
+http.ResponseWriter, r *http.Request) { bClear, _ := strconv.ParseBool
+(r.URL.Query().Get("clear")) var jb []byte var err error if bClear
+{ s.Mutex.Lock() jb, err = json.Marshal(s.StatsMap) s.StatsMap = make(map
+[string]*trafficStatsEntry) s.Mutex.Unlock() } else { s.Mutex.RLock() jb, err =
+json.Marshal(s.StatsMap) s.Mutex.RUnlock() } if err != nil { http.Error(w,
+err.Error(), http.StatusInternalServerError) return } w.Header().Set("Content-
+Type", "application/json; charset=utf-8") _, _ = w.Write(jb) } func (s
+*trafficStatsServerImpl) getOnline(w http.ResponseWriter, r *http.Request)
+{ s.Mutex.RLock() defer s.Mutex.RUnlock() jb, err := json.Marshal(s.OnlineMap)
+if err != nil { http.Error(w, err.Error(), http.StatusInternalServerError)
+return } w.Header().Set("Content-Type", "application/json; charset=utf-8") _, _
+= w.Write(jb) } func (s *trafficStatsServerImpl) kick(w http.ResponseWriter, r
 *http.Request) { var ids []string err := json.NewDecoder(r.Body).Decode(&ids)
 if err != nil { http.Error(w, err.Error(), http.StatusBadRequest) return }
 s.Mutex.Lock() for _, id := range ids { s.KickMap[id] = struct{}{} }
 s.Mutex.Unlock() w.WriteHeader(http.StatusOK) }
```

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/addr.go` & `hysteria2-2.4.4/hysteria2-go/extras/transport/udphop/addr.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/addr_test.go` & `hysteria2-2.4.4/hysteria2-go/extras/transport/udphop/addr_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/conn.go` & `hysteria2-2.4.4/hysteria2-go/extras/transport/udphop/conn.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/go.work.sum` & `hysteria2-2.4.4/hysteria2-go/go.work.sum`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/hyperbole.py` & `hysteria2-2.4.4/hysteria2-go/hyperbole.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/logo.svg` & `hysteria2-2.4.4/hysteria2-go/logo.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/black 1@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/black 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/black 2@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/black 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/black 3@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/black 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/black 4@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/black 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 1@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/dark bg 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 2@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/dark bg 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 3@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/dark bg 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 4@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/dark bg 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 1@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/light bg 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 2@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/light bg 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 3@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/light bg 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 4@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/light bg 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 1@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/symbol 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 2@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/symbol 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 3@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/symbol 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 4@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/symbol 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/white 1@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/white 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/white 2@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/white 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/white 3@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/white 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/png/white 4@2x.png` & `hysteria2-2.4.4/hysteria2-go/media-kit/png/white 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 1.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/black 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 2.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/black 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 3.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/black 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 4.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/black 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 1.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/dark bg 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 2.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/dark bg 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 3.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/dark bg 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 4.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/dark bg 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 1.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/light bg 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 2.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/light bg 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 3.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/light bg 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 4.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/light bg 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 1.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/symbol 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 2.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/symbol 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 3.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/symbol 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 4.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/symbol 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 1.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/white 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 2.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/white 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 3.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/white 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 4.svg` & `hysteria2-2.4.4/hysteria2-go/media-kit/svg/white 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2-go/scripts/install_server.sh` & `hysteria2-2.4.4/hysteria2-go/scripts/install_server.sh`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/hysteria2.egg-info/PKG-INFO` & `hysteria2-2.4.4/hysteria2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hysteria2
-Version: 2.4.3
+Version: 2.4.4
 Summary: Python bindings for hysteria2.
 Home-page: https://github.com/LorenEteval/hysteria2-python
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: MIT
 Description: # hysteria2-python
```

### Comparing `hysteria2-2.4.3/hysteria2.egg-info/SOURCES.txt` & `hysteria2-2.4.4/hysteria2.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 CMakeLists.txt
-LICENSE
 MANIFEST.in
 README.md
 setup.py
 gobuild/.gitkeep
 hysteria2/__init__.py
 hysteria2-go/.gitignore
 hysteria2-go/CHANGELOG.md
```

### Comparing `hysteria2-2.4.3/pybind11/CMakeLists.txt` & `hysteria2-2.4.4/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/LICENSE` & `hysteria2-2.4.4/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/attr.h` & `hysteria2-2.4.4/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/buffer_info.h` & `hysteria2-2.4.4/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/cast.h` & `hysteria2-2.4.4/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/chrono.h` & `hysteria2-2.4.4/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/complex.h` & `hysteria2-2.4.4/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/detail/class.h` & `hysteria2-2.4.4/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/detail/common.h` & `hysteria2-2.4.4/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/detail/descr.h` & `hysteria2-2.4.4/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/detail/init.h` & `hysteria2-2.4.4/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/detail/internals.h` & `hysteria2-2.4.4/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/detail/type_caster_base.h` & `hysteria2-2.4.4/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/detail/typeid.h` & `hysteria2-2.4.4/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/eigen.h` & `hysteria2-2.4.4/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/embed.h` & `hysteria2-2.4.4/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/eval.h` & `hysteria2-2.4.4/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/functional.h` & `hysteria2-2.4.4/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/gil.h` & `hysteria2-2.4.4/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/iostream.h` & `hysteria2-2.4.4/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/numpy.h` & `hysteria2-2.4.4/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/operators.h` & `hysteria2-2.4.4/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/options.h` & `hysteria2-2.4.4/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/pybind11.h` & `hysteria2-2.4.4/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/pytypes.h` & `hysteria2-2.4.4/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/stl/filesystem.h` & `hysteria2-2.4.4/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/stl.h` & `hysteria2-2.4.4/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/include/pybind11/stl_bind.h` & `hysteria2-2.4.4/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/FindCatch.cmake` & `hysteria2-2.4.4/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/FindEigen3.cmake` & `hysteria2-2.4.4/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/FindPythonLibsNew.cmake` & `hysteria2-2.4.4/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/JoinPaths.cmake` & `hysteria2-2.4.4/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/check-style.sh` & `hysteria2-2.4.4/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/cmake_uninstall.cmake.in` & `hysteria2-2.4.4/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/codespell_ignore_lines_from_errors.py` & `hysteria2-2.4.4/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/libsize.py` & `hysteria2-2.4.4/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/make_changelog.py` & `hysteria2-2.4.4/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/pybind11Common.cmake` & `hysteria2-2.4.4/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/pybind11Config.cmake.in` & `hysteria2-2.4.4/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/pybind11NewTools.cmake` & `hysteria2-2.4.4/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/pybind11Tools.cmake` & `hysteria2-2.4.4/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/setup_global.py.in` & `hysteria2-2.4.4/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/pybind11/tools/setup_main.py.in` & `hysteria2-2.4.4/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `hysteria2-2.4.3/setup.py` & `hysteria2-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ROOT_DIR = pathlib.Path().resolve()
 PACKAGE_NAME = 'hysteria2'
 BINDING_NAME = 'hysteria2'
 CMAKE_BUILD_CACHE = 'CMakeBuildCache'
 
 
 def getHysteriaVersion():
-    return '2.4.3'
+    return '2.4.4'
 
 
 def runCommand(command):
     subprocess.run(command, check=True)
 
 
 def buildHysteria():
```

### Comparing `hysteria2-2.4.3/src/hysteria2.cpp` & `hysteria2-2.4.4/src/hysteria2.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -25,10 +25,10 @@
 
     PYBIND11_MODULE(hysteria2, m) {
         m.def("startFromJSON",
             &startFromJSON,
             "Start Hysteria2 client with JSON",
             py::arg("json"));
 
-        m.attr("__version__") = "2.4.3";
+        m.attr("__version__") = "2.4.4";
     }
 }
```

