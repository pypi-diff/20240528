# Comparing `tmp/sippy-2.1.0.tar.gz` & `tmp/sippy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sippy-2.1.0.tar", last modified: Tue Apr 23 22:19:21 2024, max compression
+gzip compressed data, was "sippy-2.1.1.tar", last modified: Mon May 27 22:32:12 2024, max compression
```

## Comparing `sippy-2.1.0.tar` & `sippy-2.1.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-23 22:19:14.000000 sippy-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 22:19:14.000000 sippy-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-23 22:19:21.865348 sippy-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-23 22:19:14.000000 sippy-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 22:19:14.000000 sippy-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:19:21.865348 sippy-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1170 2024-04-23 22:19:14.000000 sippy-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.861348 sippy-2.1.0/sippy/
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/B2BRoute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/CCEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/CLIManager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Core/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Core/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/ESipHeaderCSV.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/ESipHeaderIgnore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Exceptions/RtpProxyError.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Exceptions/SipParseError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/External_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/FakeAccounting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Math/recfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/MsgBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/MultipartMixBody.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/MyConfigParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/RadiusAccounting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/RadiusAuthorisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Radius_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client_udp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23877 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpConnecton.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpGeneric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpMediaDescription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpOrigin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Security/
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Security/SipNonce.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAddressHF.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAllow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAlso.py
--rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAuthorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipCCDiversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipCSeq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipCallId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipCiscoGUID.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipConf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipContact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipContentLength.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipContentType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipDiversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipExpires.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipFrom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipGenericHF.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipMaxForwards.py
--rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipMsg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipNumericHF.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipPAssertedIdentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipProxyAuthenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipProxyAuthorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRAck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRSeq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipReason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRecordRoute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipReferTo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipReferredBy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRegistrationAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipReplaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRoute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipSupported.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipTo.py
--rw-r--r--   0 runner    (1001) docker     (127)    31731 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipTransactionManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipURL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipUserAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipVia.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipWWWAuthenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipWarning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/StatefulProxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Time/
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Time/MonoTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Time/Timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Time/clock_dtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    15766 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UA.py
--rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateConnected.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateDead.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateDisconnected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateFailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateGeneric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateCancelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateIdle.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateRinging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateTrying.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateUpdating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UasStateIdle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UasStateRinging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UasStateTrying.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UasStateUpdating.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14425 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Udp_server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9603 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/XMPP_server.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    35567 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/b2bua_radius.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5527 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/b2bua_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/dictionary
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-23 22:19:14.000000 sippy-2.1.0/tests/test_SdbBody.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:12.232815 sippy-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-27 22:32:07.000000 sippy-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 22:32:07.000000 sippy-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-27 22:32:12.232815 sippy-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-27 22:32:07.000000 sippy-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 22:32:07.000000 sippy-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:32:12.232815 sippy-2.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1170 2024-05-27 22:32:07.000000 sippy-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:12.228815 sippy-2.1.1/sippy/
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/B2BRoute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/CCEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/CLIManager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:12.228815 sippy-2.1.1/sippy/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Core/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Core/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/ESipHeaderCSV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/ESipHeaderIgnore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:12.232815 sippy-2.1.1/sippy/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Exceptions/RtpProxyError.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Exceptions/SipParseError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/External_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/FakeAccounting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:12.232815 sippy-2.1.1/sippy/Math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Math/recfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/MsgBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/MultipartMixBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/MyConfigParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/RadiusAccounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/RadiusAuthorisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Radius_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Rtp_proxy_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Rtp_proxy_client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Rtp_proxy_client_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Rtp_proxy_client_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Rtp_proxy_client_udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Rtp_proxy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23877 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Rtp_proxy_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SdpBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SdpConnecton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SdpGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SdpMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SdpMediaDescription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SdpOrigin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:12.232815 sippy-2.1.1/sippy/Security/
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Security/SipNonce.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipAddressHF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipAllow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipAlso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipAuthorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipCCDiversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipCSeq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipCallId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipCiscoGUID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipContact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipContentLength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipContentType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipDiversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipExpires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipFrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipGenericHF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipMaxForwards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipMsg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipNumericHF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipPAssertedIdentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipProxyAuthenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipProxyAuthorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipRAck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipRSeq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipReason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipRecordRoute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipReferTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipReferredBy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipRegistrationAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipReplaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipRoute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipSupported.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31731 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipTransactionManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipURL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipUserAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipVia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipWWWAuthenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/SipWarning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/StatefulProxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:12.232815 sippy-2.1.1/sippy/Time/
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Time/MonoTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Time/Timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Time/clock_dtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15766 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UaStateConnected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UaStateDead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UaStateDisconnected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UaStateFailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UaStateGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UacStateCancelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UacStateIdle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UacStateRinging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UacStateTrying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UacStateUpdating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UasStateIdle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UasStateRinging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UasStateTrying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/UasStateUpdating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14622 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/Udp_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9603 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/XMPP_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35567 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/b2bua_radius.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5527 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/b2bua_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/dictionary
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-27 22:32:07.000000 sippy-2.1.1/sippy/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:12.232815 sippy-2.1.1/sippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-27 22:32:12.000000 sippy-2.1.1/sippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-27 22:32:12.000000 sippy-2.1.1/sippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:32:12.000000 sippy-2.1.1/sippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-27 22:32:12.000000 sippy-2.1.1/sippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 22:32:12.000000 sippy-2.1.1/sippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 22:32:12.000000 sippy-2.1.1/sippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:12.232815 sippy-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:32:07.000000 sippy-2.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-27 22:32:07.000000 sippy-2.1.1/tests/test_SdbBody.py
```

### Comparing `sippy-2.1.0/LICENSE` & `sippy-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/PKG-INFO` & `sippy-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sippy
-Version: 2.1.0
+Version: 2.1.1
 Summary: RFC3261 SIP Stack and Back-to-Back User Agent (B2BUA)
 Home-page: http://www.b2bua.org/
 Author: Sippy Software, Inc.
 Author-email: sobomax@sippysoft.com
 License: BSD
 Keywords: sip,b2bua,voip,rfc3261,sippy
 Classifier: License :: OSI Approved :: BSD License
@@ -62,16 +62,16 @@
 `pip install git+https://github.com/sippy/b2bua`
 
 ## Running
 
 To get started, you can use the b2bua_simple implementation. The following
 example will cause the b2bua run in the foreground so you can see the SIP
 messaging. If you make a call to the IP address of your host machine, the b2bua
-will recieve the call on its UAC side, and it will send a new call leg out its
-UAS side to the IP address 192.168.1.1. It is expected that 192.168.1.1 is some
+will recieve the call on its UAS side, and it will send a new call leg out its
+UAC side to the IP address 192.168.1.1. It is expected that 192.168.1.1 is some
 sort of SIP switch or termination gateway.
 
 `b2bua_simple -f -n 192.168.1.1`
 
 ## Documentation
 
 See [documentation/documentation.md](documentation/documentation.md)
```

### Comparing `sippy-2.1.0/README.md` & `sippy-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 `pip install git+https://github.com/sippy/b2bua`
 
 ## Running
 
 To get started, you can use the b2bua_simple implementation. The following
 example will cause the b2bua run in the foreground so you can see the SIP
 messaging. If you make a call to the IP address of your host machine, the b2bua
-will recieve the call on its UAC side, and it will send a new call leg out its
-UAS side to the IP address 192.168.1.1. It is expected that 192.168.1.1 is some
+will recieve the call on its UAS side, and it will send a new call leg out its
+UAC side to the IP address 192.168.1.1. It is expected that 192.168.1.1 is some
 sort of SIP switch or termination gateway.
 
 `b2bua_simple -f -n 192.168.1.1`
 
 ## Documentation
 
 See [documentation/documentation.md](documentation/documentation.md)
```

### Comparing `sippy-2.1.0/setup.py` & `sippy-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 requirements = [x.strip() for x in open("requirements.txt", "r").readlines()]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "sippy",
-    version = "2.1.0",
+    version = "2.1.1",
     packages = find_packages(),
 
     install_requires = requirements,
     package_data = {
         '': ['dictionary', '*.md']
         },
     test_suite = 'tests',
```

### Comparing `sippy-2.1.0/sippy/B2BRoute.py` & `sippy-2.1.1/sippy/B2BRoute.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/CCEvents.py` & `sippy-2.1.1/sippy/CCEvents.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/CLIManager.py` & `sippy-2.1.1/sippy/CLIManager.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Core/EventDispatcher.py` & `sippy-2.1.1/sippy/Core/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Core/Exceptions.py` & `sippy-2.1.1/sippy/Core/Exceptions.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/ESipHeaderCSV.py` & `sippy-2.1.1/sippy/ESipHeaderCSV.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/ESipHeaderIgnore.py` & `sippy-2.1.1/sippy/ESipHeaderIgnore.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Exceptions/RtpProxyError.py` & `sippy-2.1.1/sippy/Exceptions/RtpProxyError.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Exceptions/SipParseError.py` & `sippy-2.1.1/sippy/Exceptions/SipParseError.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/External_command.py` & `sippy-2.1.1/sippy/External_command.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/FakeAccounting.py` & `sippy-2.1.1/sippy/FakeAccounting.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Math/recfilter.py` & `sippy-2.1.1/sippy/Math/recfilter.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/MsgBody.py` & `sippy-2.1.1/sippy/MsgBody.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/MultipartMixBody.py` & `sippy-2.1.1/sippy/MultipartMixBody.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/MyConfigParser.py` & `sippy-2.1.1/sippy/MyConfigParser.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/RadiusAccounting.py` & `sippy-2.1.1/sippy/RadiusAccounting.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/RadiusAuthorisation.py` & `sippy-2.1.1/sippy/RadiusAuthorisation.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Radius_client.py` & `sippy-2.1.1/sippy/Radius_client.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Rtp_proxy_client.py` & `sippy-2.1.1/sippy/Rtp_proxy_client.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Rtp_proxy_client_local.py` & `sippy-2.1.1/sippy/Rtp_proxy_client_local.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Rtp_proxy_client_net.py` & `sippy-2.1.1/sippy/Rtp_proxy_client_net.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Rtp_proxy_client_stream.py` & `sippy-2.1.1/sippy/Rtp_proxy_client_stream.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Rtp_proxy_client_udp.py` & `sippy-2.1.1/sippy/Rtp_proxy_client_udp.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Rtp_proxy_cmd.py` & `sippy-2.1.1/sippy/Rtp_proxy_cmd.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Rtp_proxy_session.py` & `sippy-2.1.1/sippy/Rtp_proxy_session.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SdpBody.py` & `sippy-2.1.1/sippy/SdpBody.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SdpConnecton.py` & `sippy-2.1.1/sippy/SdpConnecton.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SdpGeneric.py` & `sippy-2.1.1/sippy/SdpGeneric.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SdpMedia.py` & `sippy-2.1.1/sippy/SdpMedia.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SdpMediaDescription.py` & `sippy-2.1.1/sippy/SdpMediaDescription.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SdpOrigin.py` & `sippy-2.1.1/sippy/SdpOrigin.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Security/SipNonce.py` & `sippy-2.1.1/sippy/Security/SipNonce.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Signal.py` & `sippy-2.1.1/sippy/Signal.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipAddress.py` & `sippy-2.1.1/sippy/SipAddress.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipAddressHF.py` & `sippy-2.1.1/sippy/SipAddressHF.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipAllow.py` & `sippy-2.1.1/sippy/SipAllow.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipAlso.py` & `sippy-2.1.1/sippy/SipAlso.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipAuthorization.py` & `sippy-2.1.1/sippy/SipAuthorization.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipCCDiversion.py` & `sippy-2.1.1/sippy/SipCCDiversion.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipCSeq.py` & `sippy-2.1.1/sippy/SipCSeq.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipCallId.py` & `sippy-2.1.1/sippy/SipCallId.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipCiscoGUID.py` & `sippy-2.1.1/sippy/SipCiscoGUID.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipConf.py` & `sippy-2.1.1/sippy/SipConf.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipContact.py` & `sippy-2.1.1/sippy/SipContact.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipContentLength.py` & `sippy-2.1.1/sippy/SipContentLength.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipContentType.py` & `sippy-2.1.1/sippy/SipContentType.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipDiversion.py` & `sippy-2.1.1/sippy/SipDiversion.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipExpires.py` & `sippy-2.1.1/sippy/SipExpires.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipFrom.py` & `sippy-2.1.1/sippy/SipFrom.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipGenericHF.py` & `sippy-2.1.1/sippy/SipGenericHF.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipHeader.py` & `sippy-2.1.1/sippy/SipHeader.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipLogger.py` & `sippy-2.1.1/sippy/SipLogger.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipMaxForwards.py` & `sippy-2.1.1/sippy/SipMaxForwards.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipMsg.py` & `sippy-2.1.1/sippy/SipMsg.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipNumericHF.py` & `sippy-2.1.1/sippy/SipNumericHF.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipPAssertedIdentity.py` & `sippy-2.1.1/sippy/SipPAssertedIdentity.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipProxyAuthenticate.py` & `sippy-2.1.1/sippy/SipProxyAuthenticate.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipProxyAuthorization.py` & `sippy-2.1.1/sippy/SipProxyAuthorization.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipRAck.py` & `sippy-2.1.1/sippy/SipRAck.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipRSeq.py` & `sippy-2.1.1/sippy/SipRSeq.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipReason.py` & `sippy-2.1.1/sippy/SipSupported.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,47 +22,37 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from sippy.SipGenericHF import SipGenericHF
 
-class SipReason(SipGenericHF):
-    '''
-    Class that implements RFC 3326 Reason header field.
-    '''
-    hf_names = ('reason',)
-    protocol = None
-    cause = None
-    reason = None
+from functools import reduce
 
-    def __init__(self, body = None, protocol = None, cause = None, reason = None):
+class SipSupported(SipGenericHF):
+    hf_names = ('supported',)
+    caps = None
+
+    def __init__(self, body = None, caps = None):
         SipGenericHF.__init__(self, body)
         if body == None:
             self.parsed = True
-            self.protocol = protocol
-            self.cause = cause
-            self.reason = reason
+            self.caps = caps[:]
 
     def parse(self):
-        protocol, reason_params = self.body.split(';', 1)
-        self.protocol = protocol.strip()
-        for reason_param in reason_params.split(';'):
-            rp_name, rp_value = [x.strip() for x in reason_param.split('=', 1)]
-            if rp_name == 'cause':
-                self.cause = int(rp_value)
-            elif rp_name == 'text':
-                self.reason = rp_value.strip('"')
-        assert(self.cause != None)
+        self.caps = [x.strip() for x in self.body.split(',')]
         self.parsed = True
 
     def __str__(self):
         if not self.parsed:
             return self.body
-        if self.reason == None:
-            return '%s; cause=%d' % (self.protocol, self.cause)
-        return '%s; cause=%d; text="%s"' % (self.protocol, self.cause, self.reason)
+        return reduce(lambda x,y: '%s,%s' % (x, y), self.caps)
 
     def getCopy(self):
         if not self.parsed:
-            return SipReason(self.body)
-        return SipReason(protocol = self.protocol, cause = self.cause, reason = self.reason)
+            return SipSupported(self.body)
+        return SipSupported(caps = self.caps)
+
+    def getCanName(self, name, compact = False):
+        if compact:
+            return 'k'
+        return 'Supported'
```

### Comparing `sippy-2.1.0/sippy/SipRecordRoute.py` & `sippy-2.1.1/sippy/SipRecordRoute.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipReferTo.py` & `sippy-2.1.1/sippy/SipReferTo.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipReferredBy.py` & `sippy-2.1.1/sippy/SipReferredBy.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipRegistrationAgent.py` & `sippy-2.1.1/sippy/SipRegistrationAgent.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipReplaces.py` & `sippy-2.1.1/sippy/SipReplaces.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipRequest.py` & `sippy-2.1.1/sippy/SipRequest.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipResponse.py` & `sippy-2.1.1/sippy/SipResponse.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipRoute.py` & `sippy-2.1.1/sippy/SipRoute.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipServer.py` & `sippy-2.1.1/sippy/SipServer.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipSupported.py` & `sippy-2.1.1/sippy/SipTo.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,39 +20,17 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.SipGenericHF import SipGenericHF
+from sippy.SipFrom import SipFrom
 
-from functools import reduce
-
-class SipSupported(SipGenericHF):
-    hf_names = ('supported',)
-    caps = None
-
-    def __init__(self, body = None, caps = None):
-        SipGenericHF.__init__(self, body)
-        if body == None:
-            self.parsed = True
-            self.caps = caps[:]
-
-    def parse(self):
-        self.caps = [x.strip() for x in self.body.split(',')]
-        self.parsed = True
-
-    def __str__(self):
-        if not self.parsed:
-            return self.body
-        return reduce(lambda x,y: '%s,%s' % (x, y), self.caps)
-
-    def getCopy(self):
-        if not self.parsed:
-            return SipSupported(self.body)
-        return SipSupported(caps = self.caps)
+class SipTo(SipFrom):
+    hf_names = ('to', 't')
+    relaxedparser = True
 
     def getCanName(self, name, compact = False):
         if compact:
-            return 'k'
-        return 'Supported'
+            return 't'
+        return 'To'
```

### Comparing `sippy-2.1.0/sippy/SipTo.py` & `sippy-2.1.1/sippy/SipUserAgent.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,17 +20,14 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.SipFrom import SipFrom
+from sippy.SipServer import SipServer
 
-class SipTo(SipFrom):
-    hf_names = ('to', 't')
-    relaxedparser = True
+class SipUserAgent(SipServer):
+    hf_names = ('user-agent',)
 
     def getCanName(self, name, compact = False):
-        if compact:
-            return 't'
-        return 'To'
+        return 'User-Agent'
```

### Comparing `sippy-2.1.0/sippy/SipTransactionManager.py` & `sippy-2.1.1/sippy/SipTransactionManager.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipURL.py` & `sippy-2.1.1/sippy/SipURL.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipUserAgent.py` & `sippy-2.1.1/sippy/UaStateFailed.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,25 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.SipServer import SipServer
+from sippy.Time.Timeout import Timeout
+from sippy.UaStateGeneric import UaStateGeneric
 
-class SipUserAgent(SipServer):
-    hf_names = ('user-agent',)
+class UaStateFailed(UaStateGeneric):
+    sname = 'Failed'
 
-    def getCanName(self, name, compact = False):
-        return 'User-Agent'
+    def __init__(self, ua):
+        UaStateGeneric.__init__(self, ua)
+        ua.on_local_sdp_change = None
+        ua.on_remote_sdp_change = None
+        Timeout(self.goDead, ua.godead_timeout)
+
+    def goDead(self):
+        #print 'Time in Failed state expired, going to the Dead state'
+        self.ua.changeState((UaStateDead,))
+
+if not 'UaStateDead' in globals():
+    from sippy.UaStateDead import UaStateDead
```

### Comparing `sippy-2.1.0/sippy/SipVia.py` & `sippy-2.1.1/sippy/SipVia.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipWWWAuthenticate.py` & `sippy-2.1.1/sippy/SipWWWAuthenticate.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/SipWarning.py` & `sippy-2.1.1/sippy/SipWarning.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/StatefulProxy.py` & `sippy-2.1.1/sippy/StatefulProxy.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Time/MonoTime.py` & `sippy-2.1.1/sippy/Time/MonoTime.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Time/Timeout.py` & `sippy-2.1.1/sippy/Time/Timeout.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Time/clock_dtime.py` & `sippy-2.1.1/sippy/Time/clock_dtime.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UA.py` & `sippy-2.1.1/sippy/UA.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UaStateConnected.py` & `sippy-2.1.1/sippy/UaStateConnected.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UaStateDead.py` & `sippy-2.1.1/sippy/UaStateDead.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UaStateDisconnected.py` & `sippy-2.1.1/sippy/UaStateDisconnected.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UaStateFailed.py` & `sippy-2.1.1/sippy/UaStateGeneric.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,25 +20,33 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.Time.Timeout import Timeout
-from sippy.UaStateGeneric import UaStateGeneric
-
-class UaStateFailed(UaStateGeneric):
-    sname = 'Failed'
+class UaStateGeneric(object):
+    sname = 'Generic'
+    ua = None
+    connected = False
+    dead = False
 
     def __init__(self, ua):
-        UaStateGeneric.__init__(self, ua)
-        ua.on_local_sdp_change = None
-        ua.on_remote_sdp_change = None
-        Timeout(self.goDead, ua.godead_timeout)
-
-    def goDead(self):
-        #print 'Time in Failed state expired, going to the Dead state'
-        self.ua.changeState((UaStateDead,))
+        self.ua = ua
+
+    def recvRequest(self, req):
+        return None
+
+    def recvResponse(self, resp, tr):
+        return None
+
+    def recvEvent(self, event):
+        return None
+
+    def cancel(self, rtime, req):
+        return None
+
+    def onStateChange(self, newstate):
+        pass
 
-if not 'UaStateDead' in globals():
-    from sippy.UaStateDead import UaStateDead
+    def __str__(self):
+        return self.sname
```

### Comparing `sippy-2.1.0/sippy/UacStateCancelling.py` & `sippy-2.1.1/sippy/UacStateCancelling.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UacStateIdle.py` & `sippy-2.1.1/sippy/UacStateIdle.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UacStateRinging.py` & `sippy-2.1.1/sippy/UacStateRinging.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UacStateTrying.py` & `sippy-2.1.1/sippy/UacStateTrying.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UacStateUpdating.py` & `sippy-2.1.1/sippy/UacStateUpdating.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UasStateIdle.py` & `sippy-2.1.1/sippy/UasStateIdle.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UasStateRinging.py` & `sippy-2.1.1/sippy/UasStateRinging.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UasStateTrying.py` & `sippy-2.1.1/sippy/UasStateTrying.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/UasStateUpdating.py` & `sippy-2.1.1/sippy/UasStateUpdating.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/Udp_server.py` & `sippy-2.1.1/sippy/Udp_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,19 +28,20 @@
 
 try: BrokenPipeError()
 except NameError:
     class BrokenPipeError(Exception):
         pass
 
 from errno import ECONNRESET, ENOTCONN, ESHUTDOWN, EWOULDBLOCK, ENOBUFS, EAGAIN, \
-  EINTR
+  EINTR, EBADF
 from datetime import datetime
 from time import sleep, time
 from threading import Thread, Condition
 from random import random
+from sysconfig import get_platform
 import socket
 
 from sippy.Core.EventDispatcher import ED2
 from sippy.Core.Exceptions import dump_exception
 from sippy.Time.Timeout import Timeout
 from sippy.Time.MonoTime import MonoTime
 from sippy.SipConf import MyPort
@@ -112,15 +113,15 @@
                     if maxemptydata == 0:
                         break
                     continue
                 else:
                     maxemptydata = 100
                 rtime = MonoTime()
             except Exception as why:
-                if isinstance(why, socket.error) and why.errno in (ECONNRESET, ENOTCONN, ESHUTDOWN):
+                if isinstance(why, socket.error) and why.errno in (ECONNRESET, ENOTCONN, ESHUTDOWN, EBADF):
                     break
                 if isinstance(why, socket.error) and why.errno in (EINTR,):
                     continue
                 else:
                     dump_exception('Udp_server: unhandled exception when receiving incoming data')
                     sleep(1)
                     continue
@@ -190,14 +191,15 @@
         if (self.family, self.laddress[0]) in ((socket.AF_INET, '0.0.0.0'), \
           (socket.AF_INET6, '::')):
             return True
         return False
 
 class Udp_server(object):
     skt = None
+    close_on_shutdown = get_platform().startswith('macosx-')
     uopts = None
     sendqueue = None
     stats = None
     wi_available = None
     wi = None
     asenders = None
     areceivers = None
@@ -277,17 +279,19 @@
             if not isinstance(e, socket.error) or e.errno != ENOTCONN:
                 dump_exception('exception in the self.skt.shutdown()')
             pass
         self.wi_available.acquire()
         self.wi.append(None)
         self.wi_available.notify()
         self.wi_available.release()
+        for worker in self.asenders: worker.join()
+        if self.close_on_shutdown:
+            self.skt.close()
         self.uopts.data_callback = None
-        for worker in self.asenders + self.areceivers:
-            worker.join()
+        for worker in self.areceivers: worker.join()
         self.asenders = None
         self.areceivers = None
 
 class self_test(object):
     from sys import exit
     npongs = 2
     ping_data = b'ping!'
```

### Comparing `sippy-2.1.0/sippy/XMPP_server.py` & `sippy-2.1.1/sippy/XMPP_server.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/b2bua_radius.py` & `sippy-2.1.1/sippy/b2bua_radius.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/b2bua_simple.py` & `sippy-2.1.1/sippy/b2bua_simple.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/dictionary` & `sippy-2.1.1/sippy/dictionary`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy/misc.py` & `sippy-2.1.1/sippy/misc.py`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/sippy.egg-info/PKG-INFO` & `sippy-2.1.1/sippy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sippy
-Version: 2.1.0
+Version: 2.1.1
 Summary: RFC3261 SIP Stack and Back-to-Back User Agent (B2BUA)
 Home-page: http://www.b2bua.org/
 Author: Sippy Software, Inc.
 Author-email: sobomax@sippysoft.com
 License: BSD
 Keywords: sip,b2bua,voip,rfc3261,sippy
 Classifier: License :: OSI Approved :: BSD License
@@ -62,16 +62,16 @@
 `pip install git+https://github.com/sippy/b2bua`
 
 ## Running
 
 To get started, you can use the b2bua_simple implementation. The following
 example will cause the b2bua run in the foreground so you can see the SIP
 messaging. If you make a call to the IP address of your host machine, the b2bua
-will recieve the call on its UAC side, and it will send a new call leg out its
-UAS side to the IP address 192.168.1.1. It is expected that 192.168.1.1 is some
+will recieve the call on its UAS side, and it will send a new call leg out its
+UAC side to the IP address 192.168.1.1. It is expected that 192.168.1.1 is some
 sort of SIP switch or termination gateway.
 
 `b2bua_simple -f -n 192.168.1.1`
 
 ## Documentation
 
 See [documentation/documentation.md](documentation/documentation.md)
```

### Comparing `sippy-2.1.0/sippy.egg-info/SOURCES.txt` & `sippy-2.1.1/sippy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sippy-2.1.0/tests/test_SdbBody.py` & `sippy-2.1.1/tests/test_SdbBody.py`

 * *Files identical despite different names*

