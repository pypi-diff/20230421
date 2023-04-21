# Comparing `tmp/dhapi-1.2.2.tar.gz` & `tmp/dhapi-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhapi-1.2.2.tar", last modified: Mon Apr  3 17:20:32 2023, max compression
+gzip compressed data, was "dhapi-1.3.1.tar", last modified: Fri Apr 21 16:18:49 2023, max compression
```

## Comparing `dhapi-1.2.2.tar` & `dhapi-1.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-03 17:20:32.518956 dhapi-1.2.2/
--rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-03-30 00:28:46.000000 dhapi-1.2.2/LICENSE.txt
--rw-r--r--   0 roeniss    (501) staff       (20)     1542 2023-04-03 17:20:32.518842 dhapi-1.2.2/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)      505 2023-03-31 04:41:29.000000 dhapi-1.2.2/README.md
--rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-03-31 04:02:48.000000 dhapi-1.2.2/pyproject.toml
--rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-04-03 17:20:32.518984 dhapi-1.2.2/setup.cfg
--rw-r--r--   0 roeniss    (501) staff       (20)     1560 2023-04-03 17:18:29.000000 dhapi-1.2.2/setup.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-03 17:20:32.515809 dhapi-1.2.2/src/
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-03 17:20:32.517031 dhapi-1.2.2/src/dhapi/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-03-31 04:23:43.000000 dhapi-1.2.2/src/dhapi/__init__.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-03 17:20:32.517838 dhapi-1.2.2/src/dhapi/client/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-03-30 10:49:15.000000 dhapi-1.2.2/src/dhapi/client/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     4628 2023-04-03 17:18:02.000000 dhapi-1.2.2/src/dhapi/client/lottery_client.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-03 17:20:32.518008 dhapi-1.2.2/src/dhapi/domain_object/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-03-31 00:11:19.000000 dhapi-1.2.2/src/dhapi/domain_object/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     3346 2023-03-31 04:01:28.000000 dhapi-1.2.2/src/dhapi/domain_object/lotto645_buy_request.py
--rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-04-03 17:18:10.000000 dhapi-1.2.2/src/dhapi/main.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-03 17:20:32.518190 dhapi-1.2.2/src/dhapi/purchase/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-03-30 10:50:55.000000 dhapi-1.2.2/src/dhapi/purchase/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     2477 2023-03-31 04:26:21.000000 dhapi-1.2.2/src/dhapi/purchase/lotto645_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-03 17:20:32.518481 dhapi-1.2.2/src/dhapi/router/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-03-30 11:45:43.000000 dhapi-1.2.2/src/dhapi/router/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     3833 2023-04-03 17:18:58.000000 dhapi-1.2.2/src/dhapi/router/arg_parser.py
--rw-r--r--   0 roeniss    (501) staff       (20)      425 2023-03-31 04:26:21.000000 dhapi-1.2.2/src/dhapi/router/router.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-03 17:20:32.518664 dhapi-1.2.2/src/dhapi/user_info/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-03-30 08:29:51.000000 dhapi-1.2.2/src/dhapi/user_info/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-03-31 04:26:21.000000 dhapi-1.2.2/src/dhapi/user_info/user_info_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-03 17:20:32.517661 dhapi-1.2.2/src/dhapi.egg-info/
--rw-r--r--   0 roeniss    (501) staff       (20)     1542 2023-04-03 17:20:32.000000 dhapi-1.2.2/src/dhapi.egg-info/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)      637 2023-04-03 17:20:32.000000 dhapi-1.2.2/src/dhapi.egg-info/SOURCES.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-04-03 17:20:32.000000 dhapi-1.2.2/src/dhapi.egg-info/dependency_links.txt
--rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-04-03 17:20:32.000000 dhapi-1.2.2/src/dhapi.egg-info/entry_points.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-04-03 17:20:32.000000 dhapi-1.2.2/src/dhapi.egg-info/top_level.txt
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.127054 dhapi-1.3.1/
+-rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-03-28 15:41:09.000000 dhapi-1.3.1/LICENSE.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)     1542 2023-04-21 16:18:49.126858 dhapi-1.3.1/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)      505 2023-04-21 16:11:39.000000 dhapi-1.3.1/README.md
+-rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-04-21 16:11:39.000000 dhapi-1.3.1/pyproject.toml
+-rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-04-21 16:18:49.127109 dhapi-1.3.1/setup.cfg
+-rw-r--r--   0 roeniss    (501) staff       (20)     1560 2023-04-21 16:12:55.000000 dhapi-1.3.1/setup.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.122649 dhapi-1.3.1/src/
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.124384 dhapi-1.3.1/src/dhapi/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/__init__.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.125381 dhapi-1.3.1/src/dhapi/client/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/client/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     4657 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/client/lottery_client.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.125627 dhapi-1.3.1/src/dhapi/domain_object/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/domain_object/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     3393 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/domain_object/lotto645_buy_request.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/main.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.125870 dhapi-1.3.1/src/dhapi/purchase/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/purchase/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     2372 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/purchase/lotto645_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.126219 dhapi-1.3.1/src/dhapi/router/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/router/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     3919 2023-04-21 16:15:47.000000 dhapi-1.3.1/src/dhapi/router/arg_parser.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      463 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/router/router.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.126446 dhapi-1.3.1/src/dhapi/user_info/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/user_info/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-04-21 16:11:39.000000 dhapi-1.3.1/src/dhapi/user_info/user_info_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-21 16:18:49.125129 dhapi-1.3.1/src/dhapi.egg-info/
+-rw-r--r--   0 roeniss    (501) staff       (20)     1542 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)      637 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/SOURCES.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/dependency_links.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/entry_points.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-04-21 16:18:49.000000 dhapi-1.3.1/src/dhapi.egg-info/top_level.txt
```

### Comparing `dhapi-1.2.2/LICENSE.txt` & `dhapi-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dhapi-1.2.2/PKG-INFO` & `dhapi-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhapi
-Version: 1.2.2
+Version: 1.3.1
 Summary: DongHaeng Lottery Unofficial API
 Home-page: https://github.com/roeniss/dhlottery-api
 Author: Roeniss Moon
 Author-email: roeniss2@gmail.com
 Project-URL: Bug Reports, https://github.com/roeniss/dhlottery-api/issues
 Project-URL: Source, https://github.com/roeniss/dhlottery-api/
 Keywords: api,korean,donghaeng,lottery
```

### Comparing `dhapi-1.2.2/setup.py` & `dhapi-1.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="dhapi",
-    version="1.2.2",
+    version="1.3.1",
     description="DongHaeng Lottery Unofficial API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/roeniss/dhlottery-api",
     author="Roeniss Moon",
     author_email="roeniss2@gmail.com",
     classifiers=[
```

### Comparing `dhapi-1.2.2/src/dhapi/client/lottery_client.py` & `dhapi-1.3.1/src/dhapi/client/lottery_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,29 +46,29 @@
             if cookie.name == "JSESSIONID":
                 self._headers["Cookie"] = f"JSESSIONID={cookie.value}"
                 break
         else:
             raise KeyError("JSESSIONID cookie is not set in response")
 
     def login(self, user_id: str, user_pw: str):
-        requests.post(
+        resp = requests.post(
             LotteryClient._login_request_url,
             headers=self._headers,
             data={
                 "returnUrl": LotteryClient._main_url,
                 "userId": user_id,
                 "password": user_pw,
                 "checkSave": "off",
                 "newsEventYn": "",
             },
             timeout=10,
         )
-        # TODO: 로그인 실패해도 여기서 확인하지 않고 (ex. 마이페이지 방문 X),
-        #  이후 로또 구매를 시도할 때나 알게 됨
-        #  로그인 성공 실패를 이 페이즈에서 아는게 바람직하다고 생각함
+        soup = BeautifulSoup(resp.text, "html5lib")
+        if soup.find("a", {"class": "btn_common"}) is not None:
+            raise ValueError("로그인에 실패했습니다. \n아이디 또는 비밀번호를 확인해주세요.\n아이디는 대소문자를 구분합니다.")
 
     def _get_round(self):
         resp = requests.get(self._round_info_url, timeout=10)
         soup = BeautifulSoup(resp.text, "html5lib")  # 'html5lib' : in case that the html don't have clean tag pairs
         last_drawn_round = int(soup.find("strong", id="lottoDrwNo").text)
         return last_drawn_round + 1
```

### Comparing `dhapi-1.2.2/src/dhapi/domain_object/lotto645_buy_request.py` & `dhapi-1.3.1/src/dhapi/domain_object/lotto645_buy_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import json
 
 
 class Lotto645BuyRequest:
     def __init__(self, games=None):
         """
-        :param 게임은 다섯개의 list 로 이루어져 있다. 각 게임은 여섯 칸 짜리 list 로 이루어져 있다. 각 칸은 1~45 의 숫자 또는 '자동'을 의미하는 "*" 를 사용한다.
+        :param 게임은 다섯 개의 list 로 이루어져 있다. 각 게임은 여섯 칸 짜리 list 로 이루어져 있다. 각 칸은 1~45 의 숫자 또는 '자동'을 의미하는 "*" 를 사용한다.
          Asterisk("*") can be to indicate auto mode for that position.
-         e.g. [["*", "*", "*", "*", "*"], ["*", "*", "*", "*", "*"], [1, 2, 3, 4, 15, 45], None, [3, 5, "*", "*", "*"]]
+         e.g. [["*", "*", "*", "*", "*"], ["*"], [1, 2, 3, 4, 15, 45], None, [3, 5, "*", "*", "*"]]
          - This example shows two auto games, one manual game, one half-auto game and forth game is not used.
         """
         self._games = games
 
         if not self._is_correct_games(games):
             raise ValueError(f"비정상적인 입력값입니다. {self.format()}")
 
     def _is_correct_games(self, games):
         return isinstance(games, list) and len(games) == 5 and all(map(lambda x: self._is_correct_game(x), games))
 
     def _is_correct_game(self, game):
         return game is None or (
             isinstance(game, list)
-            and len(game) == 6
+            and (len(game) == 6 or len(game) == 1)
             and (len(set(filter(lambda x: x != "*", game))) == len(list(filter(lambda x: x != "*", game))))
             and all(map(lambda x: x == "*" or 1 <= x <= 45, game))
         )
 
     def has_auto_game(self):
         return any(filter(lambda game: self._is_auto_game(game), self._filter_used_games()))
 
     def _is_auto_game(self, game):
         return self._get_auto_count_in_game(game) == 6
 
     def has_half_auto_game(self):
         return any(filter(lambda game: self._is_half_auto_game(game), self._filter_used_games()))
 
     def _is_half_auto_game(self, game):
-        return 0 < self._get_auto_count_in_game(game) < 6
+        return 0 < self._get_auto_count_in_game(game) < 6 and (self._get_auto_count_in_game(game) != 1)
 
     def has_manual_game(self):
         return any(filter(lambda game: self._is_manual_game(game), self._filter_used_games()))
 
     def _is_manual_game(self, game):
         return self._get_auto_count_in_game(game) == 0
```

### Comparing `dhapi-1.2.2/src/dhapi/purchase/lotto645_controller.py` & `dhapi-1.3.1/src/dhapi/purchase/lotto645_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,27 @@
         else:
             result = self.client.buy_lotto645(req)
             self._show_result(result)
 
     def _confirm_purchase(self, req, quiet):
         print(
             f"""{req.format()}
-위와 같이 구매하시겠습니까? [Y/n] """,
+위와 같이 구매하시겠습니까? [[Y]/n] """,
             end="",
         )
 
         if quiet:
-            print("quiet 플래그가 주어져 자동으로 구매를 진행합니다.")
+            print("\nquiet 플래그가 주어져 자동으로 구매를 진행합니다.")
             return True
         else:
             answer = input().strip().lower()
             return answer in ["y", "yes", ""]
 
-    # TODO: 이쪽은 전혀 보지 못함
+    # ID가 다른 경우 loginYn이 N으로 나옴
     def _show_result(self, body: dict) -> None:
-        if body.get("loginYn") != "Y":
-            print("Fail to purchase (reason: not logged in)")
-            return
-
         result = body.get("result", {})
         if result.get("resultMsg", "FAILURE").upper() != "SUCCESS":
             print(f'Fail to purchase (reason: {result.get("resultMsg", f"Unknown (resultMsg field is empty. full response: {body})")})')
             return
 
         print(
             f"""Success to purchase
@@ -53,10 +49,11 @@
 Numbers: \n{self._format_lotto_numbers(result["arrGameChoiceNum"])}
 Result Message: {result["resultMsg"]}
 Body: {body}
 ------------------"""
         )
 
     def _format_lotto_numbers(self, numbers: list) -> None:
-        tabbed_numbers = ["\t\t" + number for number in numbers]  # TODO: what is trailing '3' in each number?
+        # Manual : 1, Combine : 2, Automatic : 3
+        tabbed_numbers = ["\t\t" + number for number in numbers]
         linebroken_tabbed_numbers = "\n".join(tabbed_numbers)
         return linebroken_tabbed_numbers
```

### Comparing `dhapi-1.2.2/src/dhapi/router/arg_parser.py` & `dhapi-1.3.1/src/dhapi/router/arg_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,29 @@
         self.print_help()
         sys.exit(2)
 
 
 class ArgParser:
     def __init__(self):
         parser = HelpOnErrorParser(description="동행복권 비공식 API", formatter_class=argparse.RawTextHelpFormatter)
-        parser.add_argument("-v", "--version", action="version", version="%(prog)s 1.2.2")
+        parser.add_argument("-v", "--version", action="version", version="%(prog)s 1.3.1")
 
         command_subparser = parser.add_subparsers(title="명령어 구분", dest="command", required=True)
 
         buy_lotto645 = command_subparser.add_parser(
             "buy_lotto645",
             help="로또6/45 구매",
             epilog="""
  
 [buy_lotto645 명령어 사용 예시]
     
 dhapi buy_lotto645 -u $USER_ID -q  # 확인 절차 없이 자동으로 5장 구매
 dhapi buy_lotto645 -u $USER_ID -p $USER_PW -g *,*,*,*,*,*  # 자동으로 1장 구매
-dhapi buy_lotto645 -u $USER_ID -g 1,2,3,4,5,6 -g 11,12,13,16,17,18 -g 5,6,7,*,*,* -g *,*,*,*,*,*  # 2장 수동, 1장 반자동, 1장 자동 - 총 4장 구매
+dhapi buy_lotto645 -u $USER_ID -p $USER_PW -g *  # 자동으로 1장 구매 (단축형)
+dhapi buy_lotto645 -u $USER_ID -g 1,2,3,4,5,6 -g 5,6,7,*,*,* -g *,*,*,*,*,* -g *  # 1장 수동, 1장 반자동, 2장 자동 - 총 4장 구매
 """,
         )
 
         buy_lotto645.formatter_class = argparse.RawTextHelpFormatter
 
         buy_lotto645.add_argument("-u", "--username", required=True, help="동행복권 아이디")
         buy_lotto645.add_argument(
@@ -47,15 +48,15 @@
             "--game",
             required=False,
             action="append",
             dest="games",
             help="""
 구매할 번호 6개를 콤마로 구분해 입력합니다.
 옵션을 여러번 사용하여 여러 게임을 구매할 수 있습니다 (매주 최대 5 게임).
-'-g *,*,*,*,*,*' 형태로 제시하면 해당 게임의 모든 번호를 자동으로 선택합니다 (자동 모드). 
+'-g *,*,*,*,*,*' 또는 '-g *' 형태로 제시하면 해당 게임의 모든 번호를 자동으로 선택합니다 (자동 모드). 
 특정 숫자 대신 '*'를 입력해 해당 값만 자동으로 구매할 수 있습니다 (반자동 모드).
 옵션을 아예 입력하지 않으면 '자동으로 5장 구매'를 수행합니다.""",
         )
 
         self._args = parser.parse_args()
 
         if self._args.password is None:
```

### Comparing `dhapi-1.2.2/src/dhapi.egg-info/PKG-INFO` & `dhapi-1.3.1/src/dhapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhapi
-Version: 1.2.2
+Version: 1.3.1
 Summary: DongHaeng Lottery Unofficial API
 Home-page: https://github.com/roeniss/dhlottery-api
 Author: Roeniss Moon
 Author-email: roeniss2@gmail.com
 Project-URL: Bug Reports, https://github.com/roeniss/dhlottery-api/issues
 Project-URL: Source, https://github.com/roeniss/dhlottery-api/
 Keywords: api,korean,donghaeng,lottery
```

### Comparing `dhapi-1.2.2/src/dhapi.egg-info/SOURCES.txt` & `dhapi-1.3.1/src/dhapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

