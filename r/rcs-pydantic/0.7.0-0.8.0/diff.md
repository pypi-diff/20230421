# Comparing `tmp/rcs_pydantic-0.7.0.tar.gz` & `tmp/rcs_pydantic-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcs_pydantic-0.7.0.tar", max compression
+gzip compressed data, was "rcs_pydantic-0.8.0.tar", max compression
```

## Comparing `rcs_pydantic-0.7.0.tar` & `rcs_pydantic-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-02-24 05:39:27.180618 rcs_pydantic-0.7.0/LICENSE
--rw-r--r--   0        0        0     6172 2023-02-24 05:39:27.180618 rcs_pydantic-0.7.0/README.md
--rw-r--r--   0        0        0     1287 2023-02-24 05:39:27.180618 rcs_pydantic-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1462 2023-02-24 05:39:27.180618 rcs_pydantic-0.7.0/rcs_pydantic/__init__.py
--rw-r--r--   0        0        0     4923 2023-02-24 05:39:27.180618 rcs_pydantic-0.7.0/rcs_pydantic/enums.py
--rw-r--r--   0        0        0    45689 2023-02-24 05:39:27.180618 rcs_pydantic-0.7.0/rcs_pydantic/errors.py
--rw-r--r--   0        0        0      713 2023-02-24 05:39:27.180618 rcs_pydantic-0.7.0/rcs_pydantic/exceptions.py
--rw-r--r--   0        0        0     3954 2023-02-24 05:39:27.180618 rcs_pydantic-0.7.0/rcs_pydantic/main.py
--rw-r--r--   0        0        0    18797 2023-02-24 05:39:27.180618 rcs_pydantic-0.7.0/rcs_pydantic/scheme.py
--rw-r--r--   0        0        0     7059 1970-01-01 00:00:00.000000 rcs_pydantic-0.7.0/setup.py
--rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 rcs_pydantic-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6172 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/README.md
+-rw-r--r--   0        0        0     1287 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1462 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/__init__.py
+-rw-r--r--   0        0        0     5037 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/enums.py
+-rw-r--r--   0        0        0    45689 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/errors.py
+-rw-r--r--   0        0        0      713 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/exceptions.py
+-rw-r--r--   0        0        0     3954 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/main.py
+-rw-r--r--   0        0        0    20259 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/scheme.py
+-rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 rcs_pydantic-0.8.0/PKG-INFO
```

### Comparing `rcs_pydantic-0.7.0/LICENSE` & `rcs_pydantic-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.7.0/README.md` & `rcs_pydantic-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.7.0/pyproject.toml` & `rcs_pydantic-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rcs-pydantic"
-version = "0.7.0"
+version = "0.8.0"
 description = ""
 authors = ["xncbf <xncbf12@gmail.com>"]
 keywords = ["pydantic", "rcs", "fastapi"]
 homepage = "https://github.com/xncbf/rcs-pydantic"
 repository = "https://github.com/xncbf/rcs-pydantic"
 license = "MIT"
 readme = "README.md"
```

### Comparing `rcs_pydantic-0.7.0/rcs_pydantic/__init__.py` & `rcs_pydantic-0.8.0/rcs_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.7.0/rcs_pydantic/enums.py` & `rcs_pydantic-0.8.0/rcs_pydantic/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     URL_ACTION: str = "urlAction"  # 단말기에 기본 웹 브라우저로 설정된 앱을 통해서, 웹페이지로 이동할 수있습니다
     LOCAL_BROWSER_ACTION: str = "localBrowserAction"  # 단말기의 메시지 앱 내부 브라우저를 통해 웹페이지로 이동할 수 있습니다
     MAP_ACTION: str = "mapAction"  # 미리 지정된 위치를 보여주거나 사용자의 현재 위치를 서버로 전송 할 수 있습니다.
     CALENDAR_ACTION: str = "calendarAction"  # 사용자의 캘린더에 특정 일정을 등록 할 수 있습니다.
     CLIPBOARD_ACTION: str = "clipboardAction"  # 특정 문구를 사용자 단말이 자동으로 복사 할 수 있게 합니다
     COMPOSE_ACTION: str = "composeAction"  # 다른 번호로 메시지를 보낼 수 있도록 대화방을 엽니다.
     DIALER_ACTION: str = "dialerAction"  # 특정 전화번호로 전화를 걸 수 있습니다.
+    REPLY: str = "reply"  # postbackData 및 displayText 등의 값을 양방향 MO 메시지로 전송합니다.
 
 
 class MessageStatusEnum(Enum):
     SUCCESS: str = "success"
     FAIL: str = "fail"
```

### Comparing `rcs_pydantic-0.7.0/rcs_pydantic/errors.py` & `rcs_pydantic-0.8.0/rcs_pydantic/errors.py`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.7.0/rcs_pydantic/exceptions.py` & `rcs_pydantic-0.8.0/rcs_pydantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.7.0/rcs_pydantic/main.py` & `rcs_pydantic-0.8.0/rcs_pydantic/main.py`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.7.0/rcs_pydantic/scheme.py` & `rcs_pydantic-0.8.0/rcs_pydantic/scheme.py`

 * *Files 5% similar despite different names*

```diff
@@ -283,14 +283,28 @@
     # agencyId
     대행사 ID
     ktbizrcs (Default: KT 중계가 브랜드 대행사인 경우)
     Maximum : 20Byte
     * Agency ID는 "Rcs Biz Center - 브랜드 운영관리" 에서 기업의 브랜드가 대행사 권한을 부여한 대행사의 ID
     Agency ID가 "ktbizrcs" 가 아닌 경우 필수 입력 필요.
     """
+    agencyKey: Optional[str]
+    """
+    # agencyKey
+    agencyId (대행사 ID) 와 매핑되는 대행사 Key 값
+    [보안성 강화] agencyId - agencyKey 가 불일치 하는 경우, 통신사에서 실패 처리. 대행사 고객인 경우 필수값. * agencyKey 는 RBC 에서 발급 및 갱신 가능하며,
+    갱신시 기존(old) agencyKey 는 최대 24 시간 유효함
+    """
+    brandKey: Optional[str]
+    """
+    # brandKey
+    chatbotId (챗봇 ID) 소유 brandId (브랜드 ID) 와 매핑되는 브랜드 Key 값
+    [보안성 강화] brandId - brandKey 가 불일치 하는 경우, 통신사에서 실패 처리. 대행사 고객인 경우 필수값. *brandKey 는 기존 RBC 에서 발급, 제공 중인 값
+    """
+
     messagebaseId: Union[enums.MessageEnum, enums.RCSMessageEnum, str]
     serviceType: enums.ServiceTypeEnum
     expiryOption: Optional[enums.ExpiryOptionEnum]
     """
     # expiryOption
     메시지 처리 옵션 enum: [1, 2]
     - 1: 최대3일 까지 결과 webhook 전송 (default)
@@ -438,14 +452,27 @@
             - [IMAGE] 0 = JPG
             - [AUDIO] 0 = AAC, 1 = MA3, MMF
             - [VIDEO] 0 = MP4+AAC
     - 여러 개인 경우, "|" 이용
     예) http://10.217.59.209:5084/data/MEDIA/RCS/send/2021/08/09/test004.jpg^1^JPG
     Maximum : 250Byte
     """
+    prefix: Optional[str] = Field(max_length=10)
+    """
+    RCS 전송성공 가능성 있는 fallback 메시지 전송시 삽입문구
+        - 79998(전송성공불확실함), 55820(Revoked Message)... 등
+        - SMS 는 msg(본문), LMS/MMS 는 subject(제목)내 문구 삽입 예) 재전송, RE:
+    """
+    kisaOrigCode: Optional[int] = Field(ge=0, le=999999999)
+    """
+    최초 발신 사업자코드, 9 자리 숫자 형식
+    [보안성 강화] 대행사 고객의 경우 (즉, KT 중계가 최초 발신
+    대행사가 아닌 경우) 최초 발신 사업자코드 전달 필수
+    예) 123456789
+    """
 
 
 class ErrorInfo(BaseModel):
     code: str
     message: str
 
 
@@ -455,26 +482,32 @@
 
 
 class ResponseErrorInfo(BaseModel):
     status: str
     error: ErrorInfo
 
 
+class ReasonInfo(BaseModel):
+    code: str
+    message: str
+
+
 class StatusInfo(BaseModel):
     """
     메시지 전송 결과
     """
 
     rcsId: Optional[str] = Field(max_length=20)
     msgId: str = Field(max_length=40)
     userContact: Optional[str] = Field(max_length=40)
     status: enums.MessageStatusEnum
     serviceType: Union[enums.ServiceTypeEnum, enums.LegacyServiceTypeEnum, None]
     mnoInfo: Optional[enums.MnoInfoEnum]
     sentTime: Optional[str] = Field(regex=r"^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{3}\+\d{2}$")
+    reason: Optional[ReasonInfo]
     error: Optional[ErrorInfo]
     legacyError: Optional[LegacyErrorInfo]
     timestamp: str = Field(regex=r"^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{3}\+\d{2}$")
     autoReplyMsgId: Optional[str] = Field(max_length=40)
     postbackId: Optional[str] = Field(max_length=40)
     chatbotId: Optional[str] = Field(max_length=40)
     bill: Optional[enums.BillEnum]
```

### Comparing `rcs_pydantic-0.7.0/setup.py` & `rcs_pydantic-0.8.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,266 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rcs-pydantic
+Version: 0.8.0
+Summary: 
+Home-page: https://github.com/xncbf/rcs-pydantic
+License: MIT
+Keywords: pydantic,rcs,fastapi
+Author: xncbf
+Author-email: xncbf12@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Project-URL: Repository, https://github.com/xncbf/rcs-pydantic
+Description-Content-Type: text/markdown
 
-packages = \
-['rcs_pydantic']
+# RCS-PYDANTIC
 
-package_data = \
-{'': ['*']}
+<p align="center">
+<a href="https://github.com/xncbf/rcs-pydantic/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">
+    <img src="https://github.com/xncbf/rcs-pydantic/workflows/Tests/badge.svg?event=push&branch=main" alt="Test">
+</a>
+<a href="https://codecov.io/gh/xncbf/rcs-pydantic" target="_blank">
+    <img src="https://img.shields.io/codecov/c/github/xncbf/rcs-pydantic?color=%2334D058" alt="Coverage">
+</a>
+<a href="https://pypi.org/project/rcs-pydantic" target="_blank">
+    <img src="https://img.shields.io/pypi/v/rcs-pydantic?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/rcs-pydantic" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/rcs-pydantic.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+</p>
 
-install_requires = \
-['pydantic>=1.9.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'rcs-pydantic',
-    'version': '0.7.0',
-    'description': '',
-    'long_description': '# RCS-PYDANTIC\n\n<p align="center">\n<a href="https://github.com/xncbf/rcs-pydantic/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/xncbf/rcs-pydantic/workflows/Tests/badge.svg?event=push&branch=main" alt="Test">\n</a>\n<a href="https://codecov.io/gh/xncbf/rcs-pydantic" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/xncbf/rcs-pydantic?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/rcs-pydantic" target="_blank">\n    <img src="https://img.shields.io/pypi/v/rcs-pydantic?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/rcs-pydantic" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/rcs-pydantic.svg?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n- [RCS-PYDANTIC](#rcs-pydantic)\n  - [Introduce](#introduce)\n  - [Installation](#installation)\n  - [Dependency](#dependency)\n  - [Quick start](#quick-start)\n  - [제공되는 항목](#제공되는-항목)\n    - [제공되는 데이터 pydantic 모델](#제공되는-데이터-pydantic-모델)\n    - [제공되는 데이터 관련 Enum](#제공되는-데이터-관련-enum)\n    - [제공되는 에러 코드 Enum](#제공되는-에러-코드-enum)\n  - [Features](#features)\n    - [RcsMessage](#rcsmessage)\n    - [MessageException](#messageexception)\n  - [Contribution](#contribution)\n\n## Introduce\n\n한국 통신사 rcs 를 위한 pydantic 모델\n\n[fastapi](https://github.com/tiangolo/fastapi) 또는 [django-ninja](https://github.com/vitalik/django-ninja) 와 함께 사용할 때 유용합니다.\n\n## Installation\n\n```sh\npip install rcs-pydantic\n```\n\n## Dependency\n\n- python3.x (3.7 이상)\n- pydantic\n\n## Quick start\n\n```py\nfrom rcs_pydantic import MessageInfo, RcsMessage\n\nmessage_info = {\n    "replyId": "B01RDSFR.KcNNLk67ui.FDSAF432153214",\n    "eventType":"newUser",\n    "displayText": "안녕",\n    "userContact":"01012341234",\n    "chatbotId":"0212351235",\n    "timestamp": "2020-03-03T04:43:55.867+09"\n}\n\nrcs = {\n    "message_base_id": "SS000000",\n    "service_type": "RCSSMS",\n    "agency_id": "<str: agency_id>",\n    "body": {\n        "title": "타이틀",\n        "description": "일반 RCSSMS 테스트 메시지 입니다."\n    }\n}\n\n\nrcs_message = RcsMessage(message_info=MessageInfo(**message_info), **rcs)\n```\n\n```sh\n>>> print(rcs_message.send_info)\ncommon=CommonInfo(\n    msgId=\'4be0072f-0f05-4b3a-adc8-90d7ef309c53\',\n    userContact=\'01012341234\',\n    scheduleType=<ScheduleTypeEnum.IMMEDIATE: 0>,\n    msgServiceType=<MessageServiceTypeEnum.RCS: \'rcs\'>\n)\nrcs=RcsInfo(\n    chatbotId=\'0212351235\',\n    agencyId=\'<str: agency_id>\',\n    messagebaseId=\'SS000000\',\n    serviceType=<ServiceTypeEnum.SMS: \'RCSSMS\'>,\n    expiryOption=<ExpiryOptionEnum.AFTER_SETTING_TIMES: 2>,\n    header=<HeaderEnum.NOT_ADVERTISE: \'0\'>,\n    copyAllowed=True,\n    body=RcsSMSBody(title=\'타이틀\', description=\'일반 RCSSMS 테스트 메시지 입니다.\'),\n)\n>>>\n```\n\n## 제공되는 항목\n\n국내 통신사 RCS 문서에서 제공되는 모든 데이터를 pydandic 모델로써 지원합니다.\n\n### 제공되는 데이터 pydantic 모델\n\n```python\nRcsSMSBody\nRcsLMSBody\nRcsMMSBody\nRcsCHATBody\nRcsSMSCarouselBody\nRcsLMSCarouselBody\nRcsMMSCarouselBody\nRcsCHATCarouselBody\nLocationInfo\nShowLocationInfo\nOpenUrlInfo\nCreateCalendarEventInfo\nCopyToClipboardInfo\nComposeTextMessageInfo\nDialPhoneNumberInfo\nUrlActionInfo\nLocalBrowserActionInfo\nMapActionInfo\nCalendarActionInfo\nClipboardActionInfo\nComposeActionInfo\nDialActionInfo\nPostbackInfo\nActionInfo\nSuggestionInfo\nButtonInfo\nCommonInfo\nRcsInfo\nLegacyInfo\nStatusInfo\nQuerystatusInfo\nErrorInfo\nResponseErrorInfo\nResponseInfo\nTextMessageInfo\nFileMessageInfo\nGeolocationPushMessage\nUserLocationInfo\nMessageInfo\nSendInfo\nTokenInfo\n```\n\n### 제공되는 데이터 관련 Enum\n\n```python\nEventTypeEnum\nRCSMessageEnum\nMessageEnum\nMessageStatusEnum\nMnoInfoEnum\nBillEnum\nMessageServiceTypeEnum\nServiceTypeEnum\nLegacyServiceTypeEnum\nScheduleTypeEnum\nExpiryOptionEnum\nHeaderEnum\nActionEnum\n```\n\n### 제공되는 에러 코드 Enum\n\n```python\nErrorCodeEnum\nMaaPErrorCodeEnum\nRcsBizCenterErrorCodeEnum\nKTErrorCodeEnum\nLegacyErrorCodeEnum\n```\n\n## Features\n\n### RcsMessage\n\n`RcsMessage` 클래스는 서버로 수신된 `MessageInfo` 메세지 모델을 기반으로 메세지 전송을 위한 `SendInfo` 모델을 만듭니다.\n\n```py\nfrom rcs_pydantic import MessageInfo, RcsMessage\n\nmessage_info = {\n    "replyId": "B01RDSFR.KcNNLk67ui.FDSAF432153214",\n    "eventType":"newUser",\n    "displayText": "안녕",\n    "userContact":"01012341234",\n    "chatbotId":"0212351235",\n    "timestamp": "2020-03-03T04:43:55.867+09"\n}\n\nrcs = {\n    "message_base_id": "SS000000",\n    "service_type": "RCSSMS",\n    "agency_id": "<str: agency_id>",\n    "body": {\n        "title": "타이틀",\n        "description": "일반 RCSSMS 테스트 메시지 입니다."\n    }\n}\n\n\nrcs_message = RcsMessage(message_info=MessageInfo(**message_info), **rcs)\n```\n\n### MessageException\n\n`MessageException` 예외 클래스는 제공되는 모든 에러 코드 Enum 을 포함하는 예외 클래스입니다.\n\n다음과 같이 여러 Enum 코드중 한가지를 메세지로 반환합니다.\n\n```python\nfrom rcs_pydantic.errors import ErrorCodeEnum\nfrom rcs_pydantic.exceptions import MessageException\ntry:\n    raise MessageException(ErrorCodeEnum.MISSING_AUTHORIZATION_HEADER.value[0])\nexcept MessageException as e:\n    print(f"ERROR MESSAGE: {e}")\n\nERROR MESSAGE: Valid access token in Authorization header is required for RESTful API calls.\n>>>\n```\n\n다음과 같이 `has_value` 를 통해 특정 `Enum` 에 포함된 에러인지 확인할 수 있습니다.\n\n```python\n>>> from rcs_pydantic.errors import ErrorCodeEnum\n... ErrorCodeEnum.has_value(40003)\nTrue\n>>> ErrorCodeEnum.has_value(11111)\nFalse\n```\n\n## Contribution\n\n이 프로젝트는 기여를 환영합니다!\n\n패치를 제출하기 전에 issue 티켓을 먼저 제출해주세요.\n\nPull request 는 `main` 브랜치로 머지되며 항상 사용 가능한 상태로 유지해야 합니다.\n\n모든 테스트 코드를 통과한 뒤 리뷰한 후 머지됩니다.\n',
-    'author': 'xncbf',
-    'author_email': 'xncbf12@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/xncbf/rcs-pydantic',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+- [RCS-PYDANTIC](#rcs-pydantic)
+  - [Introduce](#introduce)
+  - [Installation](#installation)
+  - [Dependency](#dependency)
+  - [Quick start](#quick-start)
+  - [제공되는 항목](#제공되는-항목)
+    - [제공되는 데이터 pydantic 모델](#제공되는-데이터-pydantic-모델)
+    - [제공되는 데이터 관련 Enum](#제공되는-데이터-관련-enum)
+    - [제공되는 에러 코드 Enum](#제공되는-에러-코드-enum)
+  - [Features](#features)
+    - [RcsMessage](#rcsmessage)
+    - [MessageException](#messageexception)
+  - [Contribution](#contribution)
+
+## Introduce
+
+한국 통신사 rcs 를 위한 pydantic 모델
+
+[fastapi](https://github.com/tiangolo/fastapi) 또는 [django-ninja](https://github.com/vitalik/django-ninja) 와 함께 사용할 때 유용합니다.
+
+## Installation
+
+```sh
+pip install rcs-pydantic
+```
+
+## Dependency
+
+- python3.x (3.7 이상)
+- pydantic
+
+## Quick start
+
+```py
+from rcs_pydantic import MessageInfo, RcsMessage
+
+message_info = {
+    "replyId": "B01RDSFR.KcNNLk67ui.FDSAF432153214",
+    "eventType":"newUser",
+    "displayText": "안녕",
+    "userContact":"01012341234",
+    "chatbotId":"0212351235",
+    "timestamp": "2020-03-03T04:43:55.867+09"
+}
+
+rcs = {
+    "message_base_id": "SS000000",
+    "service_type": "RCSSMS",
+    "agency_id": "<str: agency_id>",
+    "body": {
+        "title": "타이틀",
+        "description": "일반 RCSSMS 테스트 메시지 입니다."
+    }
+}
+
+
+rcs_message = RcsMessage(message_info=MessageInfo(**message_info), **rcs)
+```
+
+```sh
+>>> print(rcs_message.send_info)
+common=CommonInfo(
+    msgId='4be0072f-0f05-4b3a-adc8-90d7ef309c53',
+    userContact='01012341234',
+    scheduleType=<ScheduleTypeEnum.IMMEDIATE: 0>,
+    msgServiceType=<MessageServiceTypeEnum.RCS: 'rcs'>
+)
+rcs=RcsInfo(
+    chatbotId='0212351235',
+    agencyId='<str: agency_id>',
+    messagebaseId='SS000000',
+    serviceType=<ServiceTypeEnum.SMS: 'RCSSMS'>,
+    expiryOption=<ExpiryOptionEnum.AFTER_SETTING_TIMES: 2>,
+    header=<HeaderEnum.NOT_ADVERTISE: '0'>,
+    copyAllowed=True,
+    body=RcsSMSBody(title='타이틀', description='일반 RCSSMS 테스트 메시지 입니다.'),
+)
+>>>
+```
+
+## 제공되는 항목
+
+국내 통신사 RCS 문서에서 제공되는 모든 데이터를 pydandic 모델로써 지원합니다.
+
+### 제공되는 데이터 pydantic 모델
+
+```python
+RcsSMSBody
+RcsLMSBody
+RcsMMSBody
+RcsCHATBody
+RcsSMSCarouselBody
+RcsLMSCarouselBody
+RcsMMSCarouselBody
+RcsCHATCarouselBody
+LocationInfo
+ShowLocationInfo
+OpenUrlInfo
+CreateCalendarEventInfo
+CopyToClipboardInfo
+ComposeTextMessageInfo
+DialPhoneNumberInfo
+UrlActionInfo
+LocalBrowserActionInfo
+MapActionInfo
+CalendarActionInfo
+ClipboardActionInfo
+ComposeActionInfo
+DialActionInfo
+PostbackInfo
+ActionInfo
+SuggestionInfo
+ButtonInfo
+CommonInfo
+RcsInfo
+LegacyInfo
+StatusInfo
+QuerystatusInfo
+ErrorInfo
+ResponseErrorInfo
+ResponseInfo
+TextMessageInfo
+FileMessageInfo
+GeolocationPushMessage
+UserLocationInfo
+MessageInfo
+SendInfo
+TokenInfo
+```
+
+### 제공되는 데이터 관련 Enum
+
+```python
+EventTypeEnum
+RCSMessageEnum
+MessageEnum
+MessageStatusEnum
+MnoInfoEnum
+BillEnum
+MessageServiceTypeEnum
+ServiceTypeEnum
+LegacyServiceTypeEnum
+ScheduleTypeEnum
+ExpiryOptionEnum
+HeaderEnum
+ActionEnum
+```
+
+### 제공되는 에러 코드 Enum
+
+```python
+ErrorCodeEnum
+MaaPErrorCodeEnum
+RcsBizCenterErrorCodeEnum
+KTErrorCodeEnum
+LegacyErrorCodeEnum
+```
+
+## Features
+
+### RcsMessage
+
+`RcsMessage` 클래스는 서버로 수신된 `MessageInfo` 메세지 모델을 기반으로 메세지 전송을 위한 `SendInfo` 모델을 만듭니다.
+
+```py
+from rcs_pydantic import MessageInfo, RcsMessage
+
+message_info = {
+    "replyId": "B01RDSFR.KcNNLk67ui.FDSAF432153214",
+    "eventType":"newUser",
+    "displayText": "안녕",
+    "userContact":"01012341234",
+    "chatbotId":"0212351235",
+    "timestamp": "2020-03-03T04:43:55.867+09"
+}
+
+rcs = {
+    "message_base_id": "SS000000",
+    "service_type": "RCSSMS",
+    "agency_id": "<str: agency_id>",
+    "body": {
+        "title": "타이틀",
+        "description": "일반 RCSSMS 테스트 메시지 입니다."
+    }
 }
 
 
-setup(**setup_kwargs)
+rcs_message = RcsMessage(message_info=MessageInfo(**message_info), **rcs)
+```
+
+### MessageException
+
+`MessageException` 예외 클래스는 제공되는 모든 에러 코드 Enum 을 포함하는 예외 클래스입니다.
+
+다음과 같이 여러 Enum 코드중 한가지를 메세지로 반환합니다.
+
+```python
+from rcs_pydantic.errors import ErrorCodeEnum
+from rcs_pydantic.exceptions import MessageException
+try:
+    raise MessageException(ErrorCodeEnum.MISSING_AUTHORIZATION_HEADER.value[0])
+except MessageException as e:
+    print(f"ERROR MESSAGE: {e}")
+
+ERROR MESSAGE: Valid access token in Authorization header is required for RESTful API calls.
+>>>
+```
+
+다음과 같이 `has_value` 를 통해 특정 `Enum` 에 포함된 에러인지 확인할 수 있습니다.
+
+```python
+>>> from rcs_pydantic.errors import ErrorCodeEnum
+... ErrorCodeEnum.has_value(40003)
+True
+>>> ErrorCodeEnum.has_value(11111)
+False
+```
+
+## Contribution
+
+이 프로젝트는 기여를 환영합니다!
+
+패치를 제출하기 전에 issue 티켓을 먼저 제출해주세요.
+
+Pull request 는 `main` 브랜치로 머지되며 항상 사용 가능한 상태로 유지해야 합니다.
+
+모든 테스트 코드를 통과한 뒤 리뷰한 후 머지됩니다.
+
```

#### html2text {}

```diff
@@ -1,76 +1,82 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['rcs_pydantic'] package_data = \ {'': ['*']} install_requires = \
-['pydantic>=1.9.0,<2.0.0'] setup_kwargs = { 'name': 'rcs-pydantic', 'version':
-'0.7.0', 'description': '', 'long_description': '# RCS-PYDANTIC\n\n
- \n\n_[Test]\n\n\n_[Coverage]\n\n\n_[Package_version]\n\n\n_[Supported_Python
-                                 versions]\n\n
-\n\n- [RCS-PYDANTIC](#rcs-pydantic)\n - [Introduce](#introduce)\n -
-[Installation](#installation)\n - [Dependency](#dependency)\n - [Quick start]
-(#quick-start)\n - [ì ê³µëë í­ëª©](#ì ê³µëë-í­ëª©)\n -
-[ì ê³µëë ë°ì´í° pydantic ëª¨ë¸](#ì ê³µëë-ë°ì´í°-pydantic-
-ëª¨ë¸)\n - [ì ê³µëë ë°ì´í° ê´ë ¨ Enum](#ì ê³µëë-ë°ì´í°-
-ê´ë ¨-enum)\n - [ì ê³µëë ìë¬ ì½ë Enum](#ì ê³µëë-ìë¬-ì½ë-
-enum)\n - [Features](#features)\n - [RcsMessage](#rcsmessage)\n -
-[MessageException](#messageexception)\n - [Contribution](#contribution)\n\n##
-Introduce\n\níêµ­ íµì ì¬ rcs ë¥¼ ìí pydantic ëª¨ë¸\n\n[fastapi]
-(https://github.com/tiangolo/fastapi) ëë [django-ninja](https://github.com/
-vitalik/django-ninja) ì í¨ê» ì¬ì©í  ë ì ì©í©ëë¤.\n\n##
-Installation\n\n```sh\npip install rcs-pydantic\n```\n\n## Dependency\n\n-
-python3.x (3.7 ì´ì)\n- pydantic\n\n## Quick start\n\n```py\nfrom
-rcs_pydantic import MessageInfo, RcsMessage\n\nmessage_info = {\n "replyId":
-"B01RDSFR.KcNNLk67ui.FDSAF432153214",\n "eventType":"newUser",\n "displayText":
-"ìë",\n "userContact":"01012341234",\n "chatbotId":"0212351235",\n
-"timestamp": "2020-03-03T04:43:55.867+09"\n}\n\nrcs = {\n "message_base_id":
-"SS000000",\n "service_type": "RCSSMS",\n "agency_id": "",\n "body": {\n
-"title": "íì´í",\n "description": "ì¼ë° RCSSMS íì¤í¸ ë©ìì§
-ìëë¤."\n }\n}\n\n\nrcs_message = RcsMessage(message_info=MessageInfo
-(**message_info), **rcs)\n```\n\n```sh\n>>> print
-(rcs_message.send_info)\ncommon=CommonInfo(\n msgId=\'4be0072f-0f05-4b3a-adc8-
-90d7ef309c53\',\n userContact=\'01012341234\',\n scheduleType=
-IMMEDIATE: 0>,\n msgServiceType=
-RCS: \'rcs\'>\n)\nrcs=RcsInfo(\n chatbotId=\'0212351235\',\n agencyId=\'\',\n
-messagebaseId=\'SS000000\',\n serviceType=
-SMS: \'RCSSMS\'>,\n expiryOption=
-AFTER_SETTING_TIMES: 2>,\n header=
-NOT_ADVERTISE: \'0\'>,\n copyAllowed=True,\n body=RcsSMSBody
-(title=\'íì´í\', description=\'ì¼ë° RCSSMS íì¤í¸ ë©ìì§
-ìëë¤.\'),\n)\n>>>\n```\n\n## ì ê³µëë í­ëª©\n\nêµ­ë´ íµì ì¬ RCS
-ë¬¸ììì ì ê³µëë ëª¨ë  ë°ì´í°ë¥¼ pydandic ëª¨ë¸ë¡ì¨
-ì§ìí©ëë¤.\n\n### ì ê³µëë ë°ì´í° pydantic
-ëª¨ë¸\n\n```python\nRcsSMSBody\nRcsLMSBody\nRcsMMSBody\nRcsCHATBody\nRcsSMSCarouselBody\nRcsLMSCarouselBody\nRcsMMSCarouselBody\nRcsCHATCarouselBody\nLocationInfo\nShowLocationInfo\nOpenUrlInfo\nCreateCalendarEventInfo\nCopyToClipboardInfo\nComposeTextMessageInfo\nDialPhoneNumberInfo\nUrlActionInfo\nLocalBrowserActionInfo\nMapActionInfo\nCalendarActionInfo\nClipboardActionInfo\nComposeActionInfo\nDialActionInfo\nPostbackInfo\nActionInfo\nSuggestionInfo\nButtonInfo\nCommonInfo\nRcsInfo\nLegacyInfo\nStatusInfo\nQuerystatusInfo\nErrorInfo\nResponseErrorInfo\nResponseInfo\nTextMessageInfo\nFileMessageInfo\nGeolocationPushMessage\nUserLocationInfo\nMessageInfo\nSendInfo\nTokenInfo\n```\n\n###
-ì ê³µëë ë°ì´í° ê´ë ¨
-Enum\n\n```python\nEventTypeEnum\nRCSMessageEnum\nMessageEnum\nMessageStatusEnum\nMnoInfoEnum\nBillEnum\nMessageServiceTypeEnum\nServiceTypeEnum\nLegacyServiceTypeEnum\nScheduleTypeEnum\nExpiryOptionEnum\nHeaderEnum\nActionEnum\n```\n\n###
-ì ê³µëë ìë¬ ì½ë
-Enum\n\n```python\nErrorCodeEnum\nMaaPErrorCodeEnum\nRcsBizCenterErrorCodeEnum\nKTErrorCodeEnum\nLegacyErrorCodeEnum\n```\n\n##
-Features\n\n### RcsMessage\n\n`RcsMessage` í´ëì¤ë ìë²ë¡ ìì ë
-`MessageInfo` ë©ì¸ì§ ëª¨ë¸ì ê¸°ë°ì¼ë¡ ë©ì¸ì§ ì ì¡ì ìí
-`SendInfo` ëª¨ë¸ì ë§ë­ëë¤.\n\n```py\nfrom rcs_pydantic import
-MessageInfo, RcsMessage\n\nmessage_info = {\n "replyId":
-"B01RDSFR.KcNNLk67ui.FDSAF432153214",\n "eventType":"newUser",\n "displayText":
-"ìë",\n "userContact":"01012341234",\n "chatbotId":"0212351235",\n
-"timestamp": "2020-03-03T04:43:55.867+09"\n}\n\nrcs = {\n "message_base_id":
-"SS000000",\n "service_type": "RCSSMS",\n "agency_id": "",\n "body": {\n
-"title": "íì´í",\n "description": "ì¼ë° RCSSMS íì¤í¸ ë©ìì§
-ìëë¤."\n }\n}\n\n\nrcs_message = RcsMessage(message_info=MessageInfo
-(**message_info), **rcs)\n```\n\n### MessageException\n\n`MessageException`
-ìì¸ í´ëì¤ë ì ê³µëë ëª¨ë  ìë¬ ì½ë Enum ì í¬í¨íë
-ìì¸ í´ëì¤ìëë¤.\n\në¤ìê³¼ ê°ì´ ì¬ë¬ Enum ì½ëì¤
-íê°ì§ë¥¼ ë©ì¸ì§ë¡ ë°íí©ëë¤.\n\n```python\nfrom
-rcs_pydantic.errors import ErrorCodeEnum\nfrom rcs_pydantic.exceptions import
-MessageException\ntry:\n raise MessageException
-(ErrorCodeEnum.MISSING_AUTHORIZATION_HEADER.value[0])\nexcept MessageException
-as e:\n print(f"ERROR MESSAGE: {e}")\n\nERROR MESSAGE: Valid access token in
-Authorization header is required for RESTful API calls.\n>>>\n```\n\në¤ìê³¼
+Metadata-Version: 2.1 Name: rcs-pydantic Version: 0.8.0 Summary: Home-page:
+https://github.com/xncbf/rcs-pydantic License: MIT Keywords:
+pydantic,rcs,fastapi Author: xncbf Author-email: xncbf12@gmail.com Requires-
+Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=1.9.0,<2.0.0) Project-URL: Repository, https://
+github.com/xncbf/rcs-pydantic Description-Content-Type: text/markdown # RCS-
+PYDANTIC
+        [Test] [Coverage] [Package_version] [Supported_Python_versions]
+- [RCS-PYDANTIC](#rcs-pydantic) - [Introduce](#introduce) - [Installation]
+(#installation) - [Dependency](#dependency) - [Quick start](#quick-start) -
+[ì ê³µëë í­ëª©](#ì ê³µëë-í­ëª©) - [ì ê³µëë ë°ì´í° pydantic
+ëª¨ë¸](#ì ê³µëë-ë°ì´í°-pydantic-ëª¨ë¸) - [ì ê³µëë ë°ì´í°
+ê´ë ¨ Enum](#ì ê³µëë-ë°ì´í°-ê´ë ¨-enum) - [ì ê³µëë ìë¬ ì½ë
+Enum](#ì ê³µëë-ìë¬-ì½ë-enum) - [Features](#features) - [RcsMessage]
+(#rcsmessage) - [MessageException](#messageexception) - [Contribution]
+(#contribution) ## Introduce íêµ­ íµì ì¬ rcs ë¥¼ ìí pydantic ëª¨ë¸
+[fastapi](https://github.com/tiangolo/fastapi) ëë [django-ninja](https://
+github.com/vitalik/django-ninja) ì í¨ê» ì¬ì©í  ë ì ì©í©ëë¤. ##
+Installation ```sh pip install rcs-pydantic ``` ## Dependency - python3.x (3.7
+ì´ì) - pydantic ## Quick start ```py from rcs_pydantic import MessageInfo,
+RcsMessage message_info = { "replyId": "B01RDSFR.KcNNLk67ui.FDSAF432153214",
+"eventType":"newUser", "displayText": "ìë", "userContact":"01012341234",
+"chatbotId":"0212351235", "timestamp": "2020-03-03T04:43:55.867+09" } rcs =
+{ "message_base_id": "SS000000", "service_type": "RCSSMS", "agency_id": "",
+"body": { "title": "íì´í", "description": "ì¼ë° RCSSMS íì¤í¸
+ë©ìì§ ìëë¤." } } rcs_message = RcsMessage(message_info=MessageInfo
+(**message_info), **rcs) ``` ```sh >>> print(rcs_message.send_info)
+common=CommonInfo( msgId='4be0072f-0f05-4b3a-adc8-90d7ef309c53',
+userContact='01012341234', scheduleType=
+IMMEDIATE: 0>, msgServiceType=
+RCS: 'rcs'> ) rcs=RcsInfo( chatbotId='0212351235', agencyId='',
+messagebaseId='SS000000', serviceType=
+SMS: 'RCSSMS'>, expiryOption=
+AFTER_SETTING_TIMES: 2>, header=
+NOT_ADVERTISE: '0'>, copyAllowed=True, body=RcsSMSBody(title='íì´í',
+description='ì¼ë° RCSSMS íì¤í¸ ë©ìì§ ìëë¤.'), ) >>> ``` ##
+ì ê³µëë í­ëª© êµ­ë´ íµì ì¬ RCS ë¬¸ììì ì ê³µëë ëª¨ë 
+ë°ì´í°ë¥¼ pydandic ëª¨ë¸ë¡ì¨ ì§ìí©ëë¤. ### ì ê³µëë ë°ì´í°
+pydantic ëª¨ë¸ ```python RcsSMSBody RcsLMSBody RcsMMSBody RcsCHATBody
+RcsSMSCarouselBody RcsLMSCarouselBody RcsMMSCarouselBody RcsCHATCarouselBody
+LocationInfo ShowLocationInfo OpenUrlInfo CreateCalendarEventInfo
+CopyToClipboardInfo ComposeTextMessageInfo DialPhoneNumberInfo UrlActionInfo
+LocalBrowserActionInfo MapActionInfo CalendarActionInfo ClipboardActionInfo
+ComposeActionInfo DialActionInfo PostbackInfo ActionInfo SuggestionInfo
+ButtonInfo CommonInfo RcsInfo LegacyInfo StatusInfo QuerystatusInfo ErrorInfo
+ResponseErrorInfo ResponseInfo TextMessageInfo FileMessageInfo
+GeolocationPushMessage UserLocationInfo MessageInfo SendInfo TokenInfo ``` ###
+ì ê³µëë ë°ì´í° ê´ë ¨ Enum ```python EventTypeEnum RCSMessageEnum
+MessageEnum MessageStatusEnum MnoInfoEnum BillEnum MessageServiceTypeEnum
+ServiceTypeEnum LegacyServiceTypeEnum ScheduleTypeEnum ExpiryOptionEnum
+HeaderEnum ActionEnum ``` ### ì ê³µëë ìë¬ ì½ë Enum ```python
+ErrorCodeEnum MaaPErrorCodeEnum RcsBizCenterErrorCodeEnum KTErrorCodeEnum
+LegacyErrorCodeEnum ``` ## Features ### RcsMessage `RcsMessage` í´ëì¤ë
+ìë²ë¡ ìì ë `MessageInfo` ë©ì¸ì§ ëª¨ë¸ì ê¸°ë°ì¼ë¡ ë©ì¸ì§
+ì ì¡ì ìí `SendInfo` ëª¨ë¸ì ë§ë­ëë¤. ```py from rcs_pydantic
+import MessageInfo, RcsMessage message_info = { "replyId":
+"B01RDSFR.KcNNLk67ui.FDSAF432153214", "eventType":"newUser", "displayText":
+"ìë", "userContact":"01012341234", "chatbotId":"0212351235", "timestamp":
+"2020-03-03T04:43:55.867+09" } rcs = { "message_base_id": "SS000000",
+"service_type": "RCSSMS", "agency_id": "", "body": { "title": "íì´í",
+"description": "ì¼ë° RCSSMS íì¤í¸ ë©ìì§ ìëë¤." } } rcs_message =
+RcsMessage(message_info=MessageInfo(**message_info), **rcs) ``` ###
+MessageException `MessageException` ìì¸ í´ëì¤ë ì ê³µëë ëª¨ë 
+ìë¬ ì½ë Enum ì í¬í¨íë ìì¸ í´ëì¤ìëë¤. ë¤ìê³¼ ê°ì´
+ì¬ë¬ Enum ì½ëì¤ íê°ì§ë¥¼ ë©ì¸ì§ë¡ ë°íí©ëë¤. ```python from
+rcs_pydantic.errors import ErrorCodeEnum from rcs_pydantic.exceptions import
+MessageException try: raise MessageException
+(ErrorCodeEnum.MISSING_AUTHORIZATION_HEADER.value[0]) except MessageException
+as e: print(f"ERROR MESSAGE: {e}") ERROR MESSAGE: Valid access token in
+Authorization header is required for RESTful API calls. >>> ``` ë¤ìê³¼
 ê°ì´ `has_value` ë¥¼ íµí´ í¹ì  `Enum` ì í¬í¨ë ìë¬ì¸ì§
-íì¸í  ì ììµëë¤.\n\n```python\n>>> from rcs_pydantic.errors import
-ErrorCodeEnum\n... ErrorCodeEnum.has_value(40003)\nTrue\n>>>
-ErrorCodeEnum.has_value(11111)\nFalse\n```\n\n## Contribution\n\nì´
-íë¡ì í¸ë ê¸°ì¬ë¥¼ íìí©ëë¤!\n\ní¨ì¹ë¥¼ ì ì¶íê¸° ì ì
-issue í°ì¼ì ë¨¼ì  ì ì¶í´ì£¼ì¸ì.\n\nPull request ë `main`
-ë¸ëì¹ë¡ ë¨¸ì§ëë©° í­ì ì¬ì© ê°ë¥í ìíë¡ ì ì§í´ì¼
-í©ëë¤.\n\nëª¨ë  íì¤í¸ ì½ëë¥¼ íµê³¼í ë¤ ë¦¬ë·°í í
-ë¨¸ì§ë©ëë¤.\n', 'author': 'xncbf', 'author_email': 'xncbf12@gmail.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-xncbf/rcs-pydantic', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+íì¸í  ì ììµëë¤. ```python >>> from rcs_pydantic.errors import
+ErrorCodeEnum ... ErrorCodeEnum.has_value(40003) True >>>
+ErrorCodeEnum.has_value(11111) False ``` ## Contribution ì´ íë¡ì í¸ë
+ê¸°ì¬ë¥¼ íìí©ëë¤! í¨ì¹ë¥¼ ì ì¶íê¸° ì ì issue í°ì¼ì ë¨¼ì 
+ì ì¶í´ì£¼ì¸ì. Pull request ë `main` ë¸ëì¹ë¡ ë¨¸ì§ëë©° í­ì
+ì¬ì© ê°ë¥í ìíë¡ ì ì§í´ì¼ í©ëë¤. ëª¨ë  íì¤í¸ ì½ëë¥¼
+íµê³¼í ë¤ ë¦¬ë·°í í ë¨¸ì§ë©ëë¤.
```

