# Comparing `tmp/Fr1997v011-1.6.3.tar.gz` & `tmp/Fr1997v011-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.6.3.tar", last modified: Wed May 22 06:34:41 2024, max compression
+gzip compressed data, was "Fr1997v011-1.6.5.tar", last modified: Tue May 28 06:01:18 2024, max compression
```

## Comparing `Fr1997v011-1.6.3.tar` & `Fr1997v011-1.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.795069 Fr1997v011-1.6.3/
-drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.790076 Fr1997v011-1.6.3/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.6.3/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-22 06:34:41.794176 Fr1997v011-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.791077 Fr1997v011-1.6.3/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.6.3/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.792076 Fr1997v011-1.6.3/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.6.3/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   161601 2024-05-22 01:12:48.000000 Fr1997v011-1.6.3/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.793156 Fr1997v011-1.6.3/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.6.3/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-22 06:34:41.795069 Fr1997v011-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.353311 Fr1997v011-1.6.5/
+drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.345308 Fr1997v011-1.6.5/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-28 06:01:18.000000 Fr1997v011-1.6.5/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.6.5/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-28 06:01:18.352311 Fr1997v011-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-28 04:18:40.000000 Fr1997v011-1.6.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.346309 Fr1997v011-1.6.5/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.6.5/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.349311 Fr1997v011-1.6.5/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.6.5/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   171518 2024-05-28 06:01:16.000000 Fr1997v011-1.6.5/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:01:18.351309 Fr1997v011-1.6.5/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.6.5/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 06:01:18.353311 Fr1997v011-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-28 06:01:16.000000 Fr1997v011-1.6.5/setup.py
```

### Comparing `Fr1997v011-1.6.3/LICENSE` & `Fr1997v011-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.6.3/README.md` & `Fr1997v011-1.6.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.6.3.tar.gz
+pip install dist/Fr1997v011-1.6.4.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.6.3/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.6.5/fr1997_mode/mode_func/all_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 """
     配置文件
         所有配置在这个地方读取 
         使用内存缓存机制 memcache
         没有读取到内存中的配置，这个包相当于不能用
     pip3 cache purge
-    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.4.8
+    pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.6.1
 """
 
 """
     pip3 install --upgrade Fr1997v011
     pip3 install redis
     pip3 install pymysql
     pip3 install elasticsearch
@@ -1573,14 +1573,183 @@
             base_ret_data['sec_uid'] = sec_uid
             base_ret_data['wav_size'] = bit_rate['bit_rate']
             base_ret_data['wav_url'] = bit_rate['play_addr']['url_list']
             return base_ret_data
         else:
             return base_ret_data
 
+    # 【api】 视频详情 2024-05-28
+    @staticmethod
+    def douyin_video_response2(res_data, tp='django_video_info'):
+        base_ret_data = {'aweme_type': 1, 'is_alive': 1}
+
+        # 是否存在
+        if '因作品权限或已被删除，无法观看，去看看其他作品吧' in str(res_data):
+            base_ret_data['is_alive'] = 0
+            return base_ret_data
+
+        # 获取视频类型
+        aweme_type = res_data["aweme_type"]
+        if aweme_type == 68:
+            base_ret_data['aweme_type'] = 68
+            return base_ret_data
+
+        like_num = res_data["statistics"]["digg_count"]
+        forward_num = res_data["statistics"]["share_count"]
+        comment_num = res_data["statistics"]["comment_count"]
+        collect_count = res_data["statistics"]["collect_count"]
+
+        # 播放时长
+        try:
+            release_time = round(int(res_data['duration']) / 1000)  # 视频长度
+        except:
+            release_time = 0
+
+        # 昵称
+        nickname = res_data["author"]["nickname"]
+
+        # 描述
+        describe = res_data["author"]["signature"]
+
+        # sec_uid
+        sec_uid = res_data['author']['sec_uid']
+
+        # user_id
+        user_id = res_data['author']['uid']
+
+        # 标题
+        desc = res_data["desc"]
+
+        # 封面
+        try:
+            cover_img = res_data['video']['cover']['url_list'][0]
+        except:
+            cover_img = ''
+
+        # 视频 vid
+        try:
+            v_id = res_data['video']['vid']
+        except:
+            v_id = res_data['video']['play_addr']['uri']
+
+        # 视频下载地址
+        try:
+            download_addr_url_list = res_data['video']['download_addr']['url_list']
+        except:
+            download_addr_url_list = []
+
+        # 视频下载地址 第二类型
+        try:
+            download_addr_url_list2 = res_data['video']['play_addr']['url_list']
+        except:
+            download_addr_url_list2 = []
+
+        # mp3 url
+        try:
+            mp3_url_list = res_data['music']['play_url']['url_list']
+
+            if '.mp3' in res_data['music']['play_url']['url_list'][0]:
+                pass
+            else:
+                mp3_url_list = []
+        except:
+            mp3_url_list = []
+
+        # 视频创建时间比较特殊，如果没有创建时间，默认一个值
+        create_time = res_data.get('create_time', config_dict['douyin']['douyin_video_create_time'])
+
+        # author_head
+        author_head = res_data['author']['avatar_thumb']['url_list'][0]
+        base_ret_data['video_id'] = res_data["aweme_id"]
+        base_ret_data['v_id'] = v_id
+        base_ret_data['title'] = desc
+        base_ret_data['video_cover'] = cover_img
+
+        base_ret_data['play_num'] = 0
+        base_ret_data['good_count'] = like_num
+        base_ret_data['comment_count'] = comment_num
+        base_ret_data['share_count'] = forward_num
+        base_ret_data['collect_count'] = collect_count
+        base_ret_data['user_id'] = user_id
+
+        base_ret_data['update_time'] = int(time.time())
+        base_ret_data['create_date'] = create_time
+        base_ret_data['release_time'] = release_time
+        base_ret_data['nickname'] = nickname
+        base_ret_data['author_head'] = author_head
+        base_ret_data['describe'] = describe
+
+        base_ret_data['download_addr_url_list2'] = download_addr_url_list2
+        base_ret_data['download_addr_url_list'] = download_addr_url_list
+        base_ret_data['mp3_url_list'] = mp3_url_list
+
+        if tp == 'django_video_info':
+            return {
+                "video_id": res_data["aweme_id"],
+                "v_id": v_id,
+                'video_description': desc,
+                'video_cover': cover_img,
+
+                'play_num': 0,  # 播放量
+                'good_count': like_num,  # 点赞量
+                'comment_count': comment_num,  # 评论量
+                'share_count': forward_num,  # 分享数
+                'collect_count': collect_count,  # 收藏数
+
+                'update_time': int(time.time()),
+                'create_date': create_time,
+                'video_time_count': release_time,  # 视频时常
+                'release_time': release_time,  # 视频时常
+                'describe': describe,
+
+                'nickname': nickname,
+                'sec_uid': sec_uid,
+                'user_id': user_id,
+                'author_head': author_head,
+            }
+        elif tp == 'video_info':
+            try:
+                base_ret_data['follower_count'] = res_data['author']['follower_count']
+            except:
+                base_ret_data['follower_count'] = 0
+            base_ret_data['sec_uid'] = res_data['author']['sec_uid']
+            return base_ret_data
+        elif tp == 'wav':
+            # 获取音频
+            bit_rate = res_data['video']['bit_rate'][-1]
+            base_ret_data['sec_uid'] = sec_uid
+            base_ret_data['wav_size'] = bit_rate['bit_rate']
+            base_ret_data['wav_url'] = bit_rate['play_addr']['url_list']
+
+            # 改版 bit_rate中有很多链接，找到&cs=2为标准音频链接
+            bit_rate = res_data['video']['bit_rate'][0]  # 保底一个
+            base_ret_data['sec_uid'] = sec_uid
+            base_ret_data['wav_size'] = bit_rate['bit_rate']
+            base_ret_data['wav_url'] = bit_rate['play_addr']['url_list']
+
+            # 获取新的
+            bit_rate = res_data['video']['bit_rate']
+            for bt in bit_rate:
+                wav_url_list = bt['play_addr']['url_list']
+                if wav_url_list:
+                    if '&cs=2' in wav_url_list[0]:
+                        base_ret_data['wav_size'] = bt['bit_rate']
+                        base_ret_data['wav_url'] = bt['play_addr']['url_list']
+
+            return base_ret_data
+        elif tp == 'wav_small':
+            # 获取音频
+            bit_rate = res_data['video']['bit_rate'][-1]
+            base_ret_data['sec_uid'] = sec_uid
+            base_ret_data['wav_size'] = bit_rate['bit_rate']
+            base_ret_data['wav_url'] = bit_rate['play_addr']['url_list']
+            return base_ret_data
+        else:
+            return base_ret_data
+
 
 # 抖音
 class DouyinJike:
     # 抖音视频id短链
     def short_url(self, url):
         return HttpJike.get(url=url).ret_url
 
@@ -1785,15 +1954,15 @@
             data_data = response.json
             user_detail = data_data.get('user')
 
             data_json = self.analysis_douyin_user(user_detail)  # 数据获取
             return data_json
 
     # 【api】 视频详情
-    def api_douyin_video(self, video_id, use_proxies=1, res_tp='video_info'):
+    def api_douyin_video_old(self, video_id, use_proxies=1, res_tp='video_info'):
         cookies = mode_pro.ttwid_cookie_tt(get_cache=1)
         headers = {
             "authority": "www.douyin.com",
             "pragma": "no-cache",
             "cache-control": "no-cache",
             "accept": "application/json, text/plain, */*",
             "user-agent": config_dict['base_ua'],
@@ -1804,14 +1973,77 @@
 
         url = f'https://www.douyin.com/aweme/v1/web/aweme/detail/?device_platform=webapp&aid=6383&channel=channel_pc_web&aweme_id={video_id}&pc_client_type=1&version_code=190500&version_name=19.5.0'
         url = mode_pro.get_xbogus_new_gbk(url, config_dict['base_ua'])
         try:
             if use_proxies:
                 response = HttpJike.get(url=url, headers=headers, proxies=HttpJike.proxies_choose())
             else:
+                response = HttpJike.get(url=url, headers=headers)
+            if response.status_code == 200:
+                data_data = response.json
+
+                # 是否存在
+                if '因作品权限或已被删除，无法观看，去看看其他作品吧' in str(data_data):
+                    return {'aweme_type': 1, 'is_alive': 0, 'err': 'del'}
+
+                video_detail = data_data['aweme_detail']
+                data_json = mode_spider.douyin_video_response(video_detail, tp=res_tp)  # 数据获取
+                return data_json
+        except Exception as E:
+            return {'aweme_type': 1, 'is_alive': 0, 'err': E}
+
+    # 【api】 视频详情 2024-05-28
+    def api_douyin_video(self, video_id, use_proxies=1, res_tp='video_info'):
+        headers = {
+            "user-agent": config_dict['base_ua'],
+        }
+        url = f'https://aweme.snssdk.com/aweme/v1/multi/aweme/detail/?aweme_ids=[{video_id}]'
+        try:
+            if use_proxies:
+                response = HttpJike.get(url=url, headers=headers, proxies=HttpJike.proxies_choose())
+            else:
+                response = HttpJike.get(url=url, headers=headers)
+            if response.status_code == 200:
+                data_data = response.json
+                aweme_details = data_data['aweme_details']
+                if aweme_details:
+                    video_detail = aweme_details[0]
+                    data_json = mode_spider.douyin_video_response2(video_detail, tp=res_tp)  # 数据获取
+                    return data_json
+                else:
+                    print("没有数据")
+
+        except Exception as E:
+            return {'aweme_type': 1, 'is_alive': 0, 'err': E}
+
+    # 【api】 视频详情
+    def api_douyin_video_cookie(self, video_id, use_proxies=1, res_tp='video_info', nc=None):
+        cookies = mode_pro.ttwid_cookie_tt(get_cache=1)
+
+        print(random.choice(cookies))
+        headers = {
+            "authority": "www.douyin.com",
+            "pragma": "no-cache",
+            "cache-control": "no-cache",
+            "accept": "application/json, text/plain, */*",
+            "user-agent": config_dict['base_ua'],
+            "referer": "https://www.douy" + "in.com/user/MS4wLjABAAAAM5BxLLRhN2jrzttuOUI3LEmFClP8t6dp0bf67Oi3deE",
+            "accept-language": "zh-CN,zh;q=0.9",
+            # 'cookie':f'msToken={mode_pro.get_douyin_token(107)};odin_tt=;passport_csrf_token=1;__ac_nonce=066555a45000c53ec2bfd; __ac_signature=_02B4Z6wo00f018lQJLAAAIDDFidCqT5aCBfJcCAAAJQKaI0pMYyKNFyZl3yW2m1RRFENvDzftFrOz8CPtglGy14SoXj9SUTLrpuAX8h6P9Z-ERHDzPFm8BMUKNBbhdqW34Wfm1aEewD8aUd7bc;'
+            # 'cookie': 'ttwid=1%7CARl_GZTLCKZHJ57UtJTQd4d2gvGRa6im27p4kVMquO8%7C1713580624%7C33cbf11ff924db7aa2566de888817f3729d15736a8f76f49b27ee77fa5b23ea9;'
+            'cookie': f'msToken={mode_pro.get_douyin_token(107)};odin_tt=;passport_csrf_token=1;__ac_nonce=0658c0c6200a36d7cfa0a; __ac_signature=_02B4Z6wo00001ztv5IAAAIDBuvhKN7Rrq887b-AAAKtic9;ttwid={nc}; __ac_referer=__ac_blank'
+        }
+        print(headers)
+
+        url = f'https://www.douyin.com/aweme/v1/web/aweme/detail/?device_platform=webapp&aid=6383&channel=channel_pc_web&aweme_id={video_id}&pc_client_type=1&version_code=190500&version_name=19.5.0'
+        url = mode_pro.get_xbogus_new_gbk(url, config_dict['base_ua'])
+        try:
+            if use_proxies:
+                response = HttpJike.get(url=url, headers=headers, proxies=HttpJike.proxies_choose())
+            else:
                 response = HttpJike.get(url=url, headers=headers)
             if response.status_code == 200:
                 data_data = response.json
 
                 # 是否存在
                 if '因作品权限或已被删除，无法观看，去看看其他作品吧' in str(data_data):
                     return {'aweme_type': 1, 'is_alive': 0, 'err': 'del'}
```

