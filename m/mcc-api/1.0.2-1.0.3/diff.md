# Comparing `tmp/mcc_api-1.0.2.tar.gz` & `tmp/mcc_api-1.0.3.tar.gz`

## Comparing `mcc_api-1.0.2.tar` & `mcc_api-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.0.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 mcc_api-1.0.2/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 mcc_api-1.0.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mcc_api-1.0.2/docs/conf.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 mcc_api-1.0.2/docs/index.rst
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 mcc_api-1.0.2/mcc_api/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 mcc_api-1.0.2/mcc_api/enums.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 mcc_api-1.0.2/mcc_api/exceptions.py
--rw-r--r--   0        0        0    12551 2020-02-02 00:00:00.000000 mcc_api-1.0.2/mcc_api/responses.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/run_tests.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/test_event.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/test_halloffame.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/test_participants.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/test_rundown.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/200_event.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/200_halloffame.json
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/200_halloffame_game.json
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/200_participants.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/200_participants_team.json
--rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/200_rundown.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/400_halloffame_game.json
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/400_participants_team.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/400_rundown.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.0.2/tests/mock_data/429_ratelimit.json
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.0.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mcc_api-1.0.2/LICENSE
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 mcc_api-1.0.2/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mcc_api-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 mcc_api-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.0.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 mcc_api-1.0.3/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mcc_api-1.0.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mcc_api-1.0.3/docs/conf.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 mcc_api-1.0.3/docs/index.rst
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 mcc_api-1.0.3/mcc_api/__init__.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.0.3/mcc_api/enums.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.0.3/mcc_api/exceptions.py
+-rw-r--r--   0        0        0    12687 2020-02-02 00:00:00.000000 mcc_api-1.0.3/mcc_api/responses.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/run_tests.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/test_event.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/test_halloffame.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/test_participants.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/test_rundown.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_event.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_halloffame.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_halloffame_game.json
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_participants.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_participants_team.json
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/200_rundown.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/400_halloffame_game.json
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/400_participants_team.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/400_rundown.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.0.3/tests/mock_data/429_ratelimit.json
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mcc_api-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 mcc_api-1.0.3/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mcc_api-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 mcc_api-1.0.3/PKG-INFO
```

### Comparing `mcc_api-1.0.2/.github/workflows/docs.yml` & `mcc_api-1.0.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/.github/workflows/pypi_publish.yml` & `mcc_api-1.0.3/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/docs/index.rst` & `mcc_api-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/mcc_api/__init__.py` & `mcc_api-1.0.3/mcc_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "get_rundown",
     "get_participants",
 
     "enums",
     "exceptions",
     "responses"
 ]
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 __base_url: t.Final[str] = "https://api.mcchampionship.com/v1"
 __user_agent: t.Final[str] = f"python_mcc_api/{__version__} (https://github.com/JamesMCo/python_mcc_api)"
 
 
 @ratelimit.sleep_and_retry
 @ratelimit.limits(calls=40, period=60)
```

### Comparing `mcc_api-1.0.2/mcc_api/exceptions.py` & `mcc_api-1.0.3/mcc_api/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     """The base exception from which all other mcc_api exceptions inherit."""
 
     code: int
     """Response code of the request from the API."""
     reason: t.Optional[str]
     """Reason for the response code, if applicable."""
 
-    def __init__(self: t.Self, code: int, reason: t.Optional[str]) -> None:
+    def __init__(self: "MCCAPIError", code: int, reason: t.Optional[str]) -> None:
         self.code = code
         self.reason = reason
 
         super().__init__(f"MCC API returned code {self.code}" + f": \"{self.reason}\"" if self.reason else "")
 
 
 class InvalidEventError(MCCAPIError):
```

### Comparing `mcc_api-1.0.2/mcc_api/responses.py` & `mcc_api-1.0.3/mcc_api/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     code: int
     """Response code of the request from the API."""
     reason: t.Optional[str]
     """Reason for the response code, if applicable."""
     __json: str
 
-    def __init__(self: t.Self, request: requests.Response | dict[str, t.Any]) -> None:
+    def __init__(self: "BaseResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = self._extract_json_data(request)
         self.__json = json.dumps(data)
 
         self.code = data.get("code", data.get("status"))
         self.reason = data.get("reason")
 
         if self.code == 429:
@@ -28,15 +28,15 @@
 
     @staticmethod
     def _extract_json_data(data: requests.Response | dict[str, t.Any]) -> dict[str, t.Any]:
         """Return json data from a requests.Response object, or return the input unchanged"""
         return data.json() if isinstance(data, requests.Response) else data
 
     @property
-    def json(self: t.Self) -> str:
+    def json(self: "BaseResponse") -> str:
         """JSON string of the data returned by the API."""
         return self.__json
 
 
 @dataclass(frozen=True, slots=True)
 class EventInformationData:
     """The current event cycle's event data."""
@@ -54,20 +54,20 @@
 
 class EventInformationResponse(BaseResponse):
     """Response object representing the current event cycle's event."""
 
     data: EventInformationData
     """Current event cycle's event data."""
 
-    def __init__(self: t.Self, request: requests.Response | dict[str, t.Any]) -> None:
+    def __init__(self: "EventInformationResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = self._extract_json_data(request)
         super().__init__(data)
 
         self.data = EventInformationData(
-            date=datetime.fromisoformat(data["data"]["date"]),
+            date=datetime.strptime(data["data"]["date"], "%Y-%m-%dT%H:%M:%S.%f%z"),
             event=data["data"]["event"],
             updateVideo=data["data"].get("updateVideo")
         )
 
 
 @dataclass(frozen=True, slots=True)
 class HallOfFameRecord:
@@ -126,15 +126,15 @@
                    value=0,
                    changedHands=True
                )
            }
        }
     """
 
-    def __init__(self: t.Self, request: requests.Response | dict[str, t.Any]) -> None:
+    def __init__(self: "HallOfFameResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = super()._extract_json_data(request)
         super().__init__(data)
 
         self.data = {
             Game[game]: {
                 record_name: HallOfFameRecord(
                     player=record_data["player"],
@@ -167,15 +167,15 @@
                player="MCChampionship",
                value=0,
                changedHands=True
            )
        }
     """
 
-    def __init__(self: t.Self, request: requests.Response | dict[str, t.Any]) -> None:
+    def __init__(self: "HallOfFameGameResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = super()._extract_json_data(request)
         super().__init__(data)
 
         if self.code == 400:
             raise InvalidGameError(self.code, self.reason)
 
         self.data = {
@@ -248,15 +248,15 @@
 
 class RundownResponse(BaseResponse):
     """Response object representing score, game, and participant data for a single event."""
 
     data: EventRundown
     """Object representing the event's data."""
 
-    def __init__(self: t.Self, request: requests.Response | dict[str, t.Any]) -> None:
+    def __init__(self: "RundownResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = super()._extract_json_data(request)
         super().__init__(data)
 
         if self.code == 400:
             raise InvalidEventError(self.code, self.reason)
 
         self.data = EventRundown(
@@ -296,15 +296,15 @@
 
 class ParticipantsResponse(BaseResponse):
     """Response object representing all teams and their participants in the current event cycle."""
 
     data: dict[Team, list[Creator]]
     """Dictionary mapping from teams to lists of detailed participant data."""
 
-    def __init__(self: t.Self, request: requests.Response | dict[str, t.Any]) -> None:
+    def __init__(self: "ParticipantsResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = super()._extract_json_data(request)
         super().__init__(data)
 
         self.data = {Team[team]: [Creator(
             username=creator["username"],
             uuid=creator["uuid"],
             stream=creator["stream"]
@@ -313,15 +313,15 @@
 
 class ParticipantsTeamResponse(BaseResponse):
     """Response object representing a single team and its participants in the current event cycle."""
 
     data: list[Creator]
     """List of detailed participant data."""
 
-    def __init__(self: t.Self, request: requests.Response | dict[str, t.Any]) -> None:
+    def __init__(self: "ParticipantsTeamResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = super()._extract_json_data(request)
         super().__init__(data)
 
         if self.code == 400:
             raise InvalidTeamError(self.code, self.reason)
 
         self.data = [
```

### Comparing `mcc_api-1.0.2/tests/run_tests.py` & `mcc_api-1.0.3/tests/run_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
+import sys
 import unittest
 
 
 class Result(unittest.TextTestResult):
     def __init__(self, stream, descriptions, verbosity):
         super().__init__(stream, descriptions, verbosity)
         if os.getenv("GITHUB_STEP_SUMMARY"):
             self.job_summary = open(os.getenv("GITHUB_STEP_SUMMARY"), "a", encoding="utf-8")
-            self.job_summary.write("# Test Results\n\nName|Result\n-|-\n")
+            self.job_summary.write(f"# Test Results (Python {'.'.join(str(n) for n in sys.version_info[:3])})\n\n")
+            self.job_summary.write("Name|Result\n-|-\n")
         else:
             self.job_summary = None
 
     def addSuccess(self, test):
         super().addSuccess(test)
         if self.job_summary:
             self.job_summary.write(f"{self.getDescription(test).split()[0]}|✅\n")
@@ -87,16 +89,15 @@
     def __init__(self, stream=None, descriptions=True, verbosity=1,
                  failfast=False, buffer=False, resultclass=Result, warnings=None,
                  *, tb_locals=False):
         super().__init__(stream, descriptions, verbosity, failfast, buffer, resultclass, warnings, tb_locals=tb_locals)
 
 
 if __name__ == "__main__":
-    from test_event import *
-    from test_halloffame import *
-    from test_participants import *
-    from test_rundown import *
-
     if job_summary_path := os.getenv("GITHUB_STEP_SUMMARY"):
         with open(job_summary_path, "w", encoding="utf-8") as job_summary:
             job_summary.write("")
-    unittest.main(verbosity=2, testRunner=Runner)
+
+    tests: unittest.TestSuite = unittest.TestLoader().discover(".")
+    result: unittest.TestResult = Runner(verbosity=2).run(tests)
+
+    sys.exit(not result.wasSuccessful())
```

### Comparing `mcc_api-1.0.2/tests/test_event.py` & `mcc_api-1.0.3/tests/test_event.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import unittest
 
 
 class TestEventEndpoint200(unittest.TestCase):
     response_json: dict[str, t.Any]
     response_object: mcc_api.EventInformationResponse
 
-    def setUp(self: t.Self) -> None:
+    def setUp(self: "TestEventEndpoint200") -> None:
         with open("mock_data/200_event.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
         self.response_object = mcc_api.EventInformationResponse(self.response_json)
 
-    def test_date(self: t.Self) -> None:
+    def test_date(self: "TestEventEndpoint200") -> None:
         self.assertEqual(self.response_object.data.date, datetime(2023, 4, 2, 1, 13, 3, 587000, timezone.utc))
 
-    def test_event_name(self: t.Self) -> None:
+    def test_event_name(self: "TestEventEndpoint200") -> None:
         self.assertEqual(self.response_object.data.event, "22")
 
-    def test_update_video(self: t.Self) -> None:
+    def test_update_video(self: "TestEventEndpoint200") -> None:
         self.assertEqual(self.response_object.data.updateVideo, "https://www.youtube.com/embed/LdelXw4FsAE")
 
 
 class TestEventEndpoint429(unittest.TestCase):
-    def test_event_ratelimit_exception(self: t.Self) -> None:
+    def test_event_ratelimit_exception(self: "TestEventEndpoint429") -> None:
         with open("mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.EventInformationResponse, response_json)
 
 
 if __name__ == "__main__":
```

### Comparing `mcc_api-1.0.2/tests/test_halloffame.py` & `mcc_api-1.0.3/tests/test_halloffame.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import unittest
 
 
 class TestHallOfFameEndpoint200(unittest.TestCase):
     response_json: dict[str, t.Any]
     response_object: mcc_api.HallOfFameResponse
 
-    def setUp(self: t.Self) -> None:
+    def setUp(self: "TestHallOfFameEndpoint200") -> None:
         with open("mock_data/200_halloffame.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
         self.response_object = mcc_api.HallOfFameResponse(self.response_json)
 
-    def test_game_names(self: t.Self) -> None:
+    def test_game_names(self: "TestHallOfFameEndpoint200") -> None:
         self.assertIn(mcc_api.Game.GLOBAL_STATISTICS, self.response_object.data)
         self.assertIn(mcc_api.Game.LEGACY_STATISTICS, self.response_object.data)
 
-    def test_records(self: t.Self) -> None:
+    def test_records(self: "TestHallOfFameEndpoint200") -> None:
         for game in [mcc_api.Game.GLOBAL_STATISTICS, mcc_api.Game.LEGACY_STATISTICS]:
             with self.subTest(game=str(game)):
                 self.assertIn(
                     game,
                     self.response_object.data
                 )
 
@@ -40,32 +40,32 @@
                 self.assertEqual(records["RECORD NAME 2"].value, 0)
                 self.assertTrue(records["RECORD NAME 2"].changedHands)
 
 
 class TestHallOfFameEndpoint429(unittest.TestCase):
     response_json: dict[str, t.Any]
 
-    def test_halloffame_ratelimit_exception(self: t.Self) -> None:
+    def test_halloffame_ratelimit_exception(self: "TestHallOfFameEndpoint429") -> None:
         with open("mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.HallOfFameResponse, response_json)
 
 
 class TestHallOfFameGameEndpoint200(unittest.TestCase):
     response_json: dict[str, t.Any]
     response_object: mcc_api.HallOfFameGameResponse
 
-    def setUp(self: t.Self) -> None:
+    def setUp(self: "TestHallOfFameGameEndpoint200") -> None:
         with open("mock_data/200_halloffame_game.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
         self.response_object = mcc_api.HallOfFameGameResponse(self.response_json)
 
-    def test_records(self: t.Self) -> None:
+    def test_records(self: "TestHallOfFameGameEndpoint200") -> None:
         records: dict[str, mcc_api.responses.HallOfFameRecord] = self.response_object.data
 
         self.assertIn("RECORD NAME 1", records)
         self.assertEqual(records["RECORD NAME 1"].placement, 0)
         self.assertEqual(records["RECORD NAME 1"].player, "MCChampionship")
         self.assertEqual(records["RECORD NAME 1"].value, "String value")
         self.assertFalse(records["RECORD NAME 1"].changedHands)
@@ -74,23 +74,23 @@
         self.assertEqual(records["RECORD NAME 2"].placement, 1)
         self.assertEqual(records["RECORD NAME 2"].player, "MCChampionship")
         self.assertEqual(records["RECORD NAME 2"].value, 0)
         self.assertTrue(records["RECORD NAME 2"].changedHands)
 
 
 class TestHallOfFameGameEndpoint400(unittest.TestCase):
-    def test_halloffame_game_invalid_game_exception(self: t.Self) -> None:
+    def test_halloffame_game_invalid_game_exception(self: "TestHallOfFameGameEndpoint400") -> None:
         with open("mock_data/400_halloffame_game.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.InvalidGameError, mcc_api.HallOfFameGameResponse, response_json)
 
 
 class TestHallOfFameGameEndpoint429(unittest.TestCase):
-    def test_halloffame_game_ratelimit_exception(self: t.Self) -> None:
+    def test_halloffame_game_ratelimit_exception(self: "TestHallOfFameGameEndpoint429") -> None:
         with open("mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.HallOfFameGameResponse, response_json)
 
 
 if __name__ == "__main__":
```

### Comparing `mcc_api-1.0.2/tests/test_participants.py` & `mcc_api-1.0.3/tests/test_participants.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 import unittest
 
 
 class TestEventParticipants200(unittest.TestCase):
     response_json: dict[str, t.Any]
     response_object: mcc_api.ParticipantsResponse
 
-    def setUp(self: t.Self) -> None:
+    def setUp(self: "TestEventParticipants200") -> None:
         with open("mock_data/200_participants.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
         self.response_object = mcc_api.ParticipantsResponse(self.response_json)
 
-    def test_all_teams_present(self: t.Self) -> None:
+    def test_all_teams_present(self: "TestEventParticipants200") -> None:
         for team in mcc_api.Team:
             with self.subTest(team=str(team)):
                 self.assertIn(team, self.response_object.data)
 
-    def test_all_participants_unique(self: t.Self) -> None:
+    def test_all_participants_unique(self: "TestEventParticipants200") -> None:
         participants_count: int = 0
         usernames: set[str] = set()
         uuids: set[str] = set()
 
         for _, participants in self.response_object.data.items():
             participants: list[mcc_api.responses.Creator]
             for participant in participants:
@@ -34,32 +34,32 @@
                 uuids.add(participant.uuid)
 
         self.assertEqual(participants_count, len(usernames))
         self.assertEqual(participants_count, len(uuids))
 
 
 class TestParticipantsEndpoint429(unittest.TestCase):
-    def test_participants_ratelimit_exception(self: t.Self) -> None:
+    def test_participants_ratelimit_exception(self: "TestParticipantsEndpoint429") -> None:
         with open("mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.ParticipantsResponse, response_json)
 
 
 class TestEventParticipantsTeam200(unittest.TestCase):
     response_json: dict[str, t.Any]
     response_object: mcc_api.ParticipantsTeamResponse
 
-    def setUp(self: t.Self) -> None:
+    def setUp(self: "TestEventParticipantsTeam200") -> None:
         with open("mock_data/200_participants_team.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
         self.response_object = mcc_api.ParticipantsTeamResponse(self.response_json)
 
-    def test_all_participants_unique(self: t.Self) -> None:
+    def test_all_participants_unique(self: "TestEventParticipantsTeam200") -> None:
         participants_count: int = 0
         usernames: set[str] = set()
         uuids: set[str] = set()
 
         for participant in self.response_object.data:
             participant: mcc_api.responses.Creator
 
@@ -68,23 +68,23 @@
             uuids.add(participant.uuid)
 
         self.assertEqual(participants_count, len(usernames))
         self.assertEqual(participants_count, len(uuids))
 
 
 class TestParticipantsTeamEndpoint400(unittest.TestCase):
-    def test_participants_team_invalid_team_exception(self: t.Self) -> None:
+    def test_participants_team_invalid_team_exception(self: "TestParticipantsTeamEndpoint400") -> None:
         with open("mock_data/400_participants_team.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.InvalidTeamError, mcc_api.ParticipantsTeamResponse, response_json)
 
 
 class TestParticipantsTeamEndpoint429(unittest.TestCase):
-    def test_participants_team_ratelimit_exception(self: t.Self) -> None:
+    def test_participants_team_ratelimit_exception(self: "TestParticipantsTeamEndpoint429") -> None:
         with open("mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.ParticipantsTeamResponse, response_json)
 
 
 if __name__ == "__main__":
```

### Comparing `mcc_api-1.0.2/tests/test_rundown.py` & `mcc_api-1.0.3/tests/test_rundown.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,46 +4,46 @@
 import unittest
 
 
 class TestRundownEndpoint200(unittest.TestCase):
     response_json: dict[str, t.Any]
     response_object: mcc_api.RundownResponse
 
-    def setUp(self: t.Self) -> None:
+    def setUp(self: "TestRundownEndpoint200") -> None:
         with open("mock_data/200_rundown.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
         self.response_object = mcc_api.RundownResponse(self.response_json)
 
-    def test_dodgebolt(self: t.Self) -> None:
+    def test_dodgebolt(self: "TestRundownEndpoint200") -> None:
         self.assertEqual(len(self.response_object.data.dodgeboltData), 2)
 
         team_one: mcc_api.Team
         team_two: mcc_api.Team
         team_one, team_two = self.response_object.data.dodgeboltData.keys()
 
         self.assertNotEqual(team_one, team_two)
         self.assertNotEqual(
             self.response_object.data.dodgeboltData[team_one],
             self.response_object.data.dodgeboltData[team_two]
         )
 
-    def test_event_placements_and_scores_match(self: t.Self) -> None:
+    def test_event_placements_and_scores_match(self: "TestRundownEndpoint200") -> None:
         placements: list[mcc_api.Team] = sorted(
             self.response_object.data.eventPlacements.keys(),
             key=lambda team: self.response_object.data.eventPlacements[team],
             reverse=True
         )
         scores: list[mcc_api.Team] = sorted(
             self.response_object.data.eventScores.keys(),
             key=lambda team: self.response_object.data.eventScores[team]
         )
         self.assertEqual(placements, scores)
 
-    def test_event_individual_scores_contain_all_participants(self: t.Self) -> None:
+    def test_event_individual_scores_contain_all_participants(self: "TestRundownEndpoint200") -> None:
         participant_teams: list[mcc_api.Team] = [
             mcc_api.Team.RED,
             mcc_api.Team.ORANGE,
             mcc_api.Team.YELLOW,
             mcc_api.Team.LIME,
             mcc_api.Team.GREEN,
             mcc_api.Team.CYAN,
@@ -58,33 +58,33 @@
             for participant in self.response_object.data.creators[team]
         ]
         self.assertEqual(
             sorted(self.response_object.data.individualScores, key=str.casefold),
             sorted(participants, key=str.casefold)
         )
 
-    def test_history_contains_eight_games(self: t.Self) -> None:
+    def test_history_contains_eight_games(self: "TestRundownEndpoint200") -> None:
         self.assertEqual(len(self.response_object.data.history), 8)
 
-    def test_history_multipliers(self: t.Self) -> None:
+    def test_history_multipliers(self: "TestRundownEndpoint200") -> None:
         for game, multiplier in zip(range(8), [1, 1.5, 1.5, 2, 2, 2.5, 2.5, 3]):
             with self.subTest(game=game):
                 self.assertEqual(self.response_object.data.history[str(game)].multiplier, multiplier)
 
 
 class TestRundownEndpoint400(unittest.TestCase):
-    def test_rundown_invalid_event_exception(self: t.Self) -> None:
+    def test_rundown_invalid_event_exception(self: "TestRundownEndpoint400") -> None:
         with open("mock_data/400_rundown.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.InvalidEventError, mcc_api.RundownResponse, response_json)
 
 
 class TestRundownEndpoint429(unittest.TestCase):
-    def test_rundown_ratelimit_exception(self: t.Self) -> None:
+    def test_rundown_ratelimit_exception(self: "TestRundownEndpoint429") -> None:
         with open("mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.RundownResponse, response_json)
 
 
 if __name__ == "__main__":
```

### Comparing `mcc_api-1.0.2/tests/mock_data/200_halloffame.json` & `mcc_api-1.0.3/tests/mock_data/200_halloffame.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/tests/mock_data/200_participants.json` & `mcc_api-1.0.3/tests/mock_data/200_participants.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/tests/mock_data/200_participants_team.json` & `mcc_api-1.0.3/tests/mock_data/200_participants_team.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/tests/mock_data/200_rundown.json` & `mcc_api-1.0.3/tests/mock_data/200_rundown.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/.gitignore` & `mcc_api-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/LICENSE` & `mcc_api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/README.md` & `mcc_api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/pyproject.toml` & `mcc_api-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.2/PKG-INFO` & `mcc_api-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcc-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Wrapper for the MC Championship API
 Project-URL: Repository, https://github.com/JamesMCo/python_mcc_api
 Project-URL: Issues, https://github.com/JamesMCo/python_mcc_api/issues
 Project-URL: Documentation, https://mrjamesco.uk/python_mcc_api
 Author-email: "James C." <james@cordon.click>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

