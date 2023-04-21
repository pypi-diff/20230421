# Comparing `tmp/pizazz-1.3.0.tar.gz` & `tmp/pizazz-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizazz-1.3.0.tar", last modified: Sat Oct  8 16:56:52 2022, max compression
+gzip compressed data, was "pizazz-1.3.1.tar", last modified: Fri Apr 21 13:55:53 2023, max compression
```

## Comparing `pizazz-1.3.0.tar` & `pizazz-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-10-08 16:56:52.173912 pizazz-1.3.0/
--rw-rw-rw-   0        0        0      163 2022-05-22 15:07:55.000000 pizazz-1.3.0/AUTHORS.md
--rw-rw-rw-   0        0        0      579 2022-10-08 16:56:25.000000 pizazz-1.3.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2022-05-22 14:38:29.000000 pizazz-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      203 2022-05-22 14:38:29.000000 pizazz-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10510 2022-10-08 16:56:52.174645 pizazz-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     9294 2022-06-17 15:20:34.000000 pizazz-1.3.0/README.md
--rw-rw-rw-   0        0        0     2215 2022-10-08 16:54:54.000000 pizazz-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0     1479 2022-10-08 16:56:52.175640 pizazz-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      116 2022-05-22 14:38:29.000000 pizazz-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-08 16:56:52.142638 pizazz-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2022-10-08 16:56:52.158639 pizazz-1.3.0/src/pizazz/
--rw-rw-rw-   0        0        0      337 2022-10-08 16:56:26.000000 pizazz-1.3.0/src/pizazz/__init__.py
--rw-rw-rw-   0        0        0     8085 2022-05-22 17:47:31.000000 pizazz-1.3.0/src/pizazz/pizazz.py
-drwxrwxrwx   0        0        0        0 2022-10-08 16:56:52.172643 pizazz-1.3.0/src/pizazz.egg-info/
--rw-rw-rw-   0        0        0    10510 2022-10-08 16:56:52.000000 pizazz-1.3.0/src/pizazz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2022-10-08 16:56:52.000000 pizazz-1.3.0/src/pizazz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-08 16:56:52.000000 pizazz-1.3.0/src/pizazz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-10-08 16:56:52.000000 pizazz-1.3.0/src/pizazz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2022-10-08 16:56:52.000000 pizazz-1.3.0/src/pizazz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 13:55:53.484700 pizazz-1.3.1/
+-rw-rw-rw-   0        0        0      157 2023-04-18 15:26:46.000000 pizazz-1.3.1/AUTHORS.md
+-rw-rw-rw-   0        0        0     1283 2023-04-21 13:55:39.000000 pizazz-1.3.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2022-05-22 14:38:29.000000 pizazz-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      203 2022-05-22 14:38:29.000000 pizazz-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11450 2023-04-21 13:55:53.484700 pizazz-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10217 2023-04-19 22:06:08.000000 pizazz-1.3.1/README.md
+-rw-rw-rw-   0        0        0     2215 2022-10-08 16:54:54.000000 pizazz-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1473 2023-04-21 13:55:53.484700 pizazz-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      115 2023-04-21 12:33:15.000000 pizazz-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:55:53.400021 pizazz-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 13:55:53.469066 pizazz-1.3.1/src/pizazz/
+-rw-rw-rw-   0        0        0      356 2023-04-21 13:55:39.000000 pizazz-1.3.1/src/pizazz/__init__.py
+-rw-rw-rw-   0        0        0     8109 2023-04-21 12:33:15.000000 pizazz-1.3.1/src/pizazz/pizazz.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:55:53.484700 pizazz-1.3.1/src/pizazz.egg-info/
+-rw-rw-rw-   0        0        0    11450 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/top_level.txt
```

### Comparing `pizazz-1.3.0/LICENSE` & `pizazz-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.0/PKG-INFO` & `pizazz-1.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pizazz
-Version: 1.3.0
+Version: 1.3.1
 Summary: Easy configuration and control of 74HC595 Shift Registers on a Raspberry Pi
 Home-page: https://github.com/stephen-ra-king/pizazz
 Download-URL: 
 Author: Stephen R A King
-Author-email: stephen.ra.king@gmail.com
+Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
-Maintainer-email: stephen.ra.king@gmail.com
+Maintainer-email: sking.github@gmail.com
 License: MIT
 Keywords: utility,74HC595,GPIO,Raspberry,Pi
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # Pizazz
 
-> A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.
+\_**A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.**-
 
 [![PyPI version](https://badge.fury.io/py/pizazz.svg)](https://badge.fury.io/py/pizazz)
 [![Documentation Status](https://readthedocs.org/projects/pizazz/badge/?version=latest)](https://pizazz.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/personalized-badge/pizazz?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pizazz)
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -46,18 +46,18 @@
 That is great in itself however 595's can be daisy-chained together to give you multiples of 8 pin outputs yet still
 always controlled by only 3 input pins! Wow!
 
 If you are not sure why this is useful then let me explain.
 
 I had a requirement to create a LED "Status Board" for a monitoring and automation application that I am also writing.
 The status board would reflect the current operation status of things like Jenkins jobs, Github Actions, Linux services etc etc.
-I needed a minimum of 16 LEDs. Now there already exists a [**status board**][status-board-url] HAT. However it only tracks 5 items.
+I needed a minimum of 16 LEDs. Now there already exists a [**status board**][status-board-url] HAT. However it only tracks 5 items (that is 10 LED's). However, each LED requires it's own GPIO and the HAT masks all other pins making them unavailable.
 
 Using the Raspberry [**RPi.GPIO**][rpi-gpio-url] library it is possible to individually switch the 27 GPIO pins. However each LED would require
-a wire from the GPIO pin. This is very physically unwieldy and clunky to control in python.
+a wire from the GPIO pin. This is very physically unwieldy and clunky to control in Python.
 
 Enter the 74HC595...
 
 This class enables you to individually control any number of LEDS (or other output devices) with only 3 GPIO pins.
 
 ### Basic Wiring of the 74HC595 8-bit shift register to a Raspberry Pi
 
@@ -94,22 +94,26 @@
 2. Bit 0 in the Shift Register accepts the current value on DATA pin. At the rising edge of the pulse, if the data pin is high, then a 1 gets pushed into the shift register. Otherwise, it is a 0.
 
 On enabling the Latch pin, the contents of Shift Register are copied into the Storage Register.
 Each bit of the Storage Register is connected to one of the output pins Q0–Q7 of the IC, so in general, when the value in the Storage Register changes, so do the outputs.
 
 ## Installation
 
+---
+
 Raspberry Pi:
 
 ```sh
 pip3 install pizazz
 ```
 
 ## Connecting the Raspberry Pi
 
+---
+
 The 40 pins of the Raspberry Pi are GPIO, 5v, 3.3V and ground. Some of the GPIO pins can have special purposes.
 However, all of them can be controlled by the RPi.GPIO Python Library.
 The RPi.GPIO requires that you specify how you will identify the pins that you use. There are 2 ways:
 
 1. **GPIO.BOARD:** option specifies that you are referring to the pins by the number of the pin.
 
 2. **BCM:** option means that you are referring to the pins by the "Broadcom SOC channel" number, these are
@@ -117,20 +121,23 @@
 
 So referring to the diagram below: BCM mode GPIO2 is the same as BOARD mode pin 2
 
 ![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/40pinheader.png)
 
 Connect any GPIO's to the clock, latch and data pins of the register and connect the the 5v supply and earth
 as indicated in the register diagram.
+If you are connecting the outputs to LED's then you need to wire 330 ohm resistors serially to protect them in the usual way.
 
 ## Library Usage examples
 
+---
+
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
-https://user-images.githubusercontent.com/33905365/163853342-a1a19d5e-e392-483d-845f-40bfe25d4cb3.mp4
+https://user-images.githubusercontent.com/33905365/220999848-e6062e9d-af53-4c91-8db8-0f8b5fdf1ff3.mp4
 
 Import the library
 
 ```sh
 from pizazz.pizazz import HC595
 ```
 
@@ -212,38 +219,54 @@
 
 ```sh
 shifter.set_pattern([0, 0, 1, 1, 0, 0, 0, 0])
 ```
 
 ## Documentation
 
-[**Read the Docs**](https://pizazz.readthedocs.io/en/latest/)
+---
+
+[**Read the Docs**](https://pizazz.readthedocs.io/en/latest/?)
+
+- [**Example Usage**](https://pizazz.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://pizazz.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://pizazz.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://pizazz.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**][wiki]
 
 ## Meta
 
-[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/linkedin.png)](https://linkedin.com/in/stephen-k-3a4644210)
+---
+
+[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/github.png)](https://github.com/Stephen-RA-King/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pizazz/)
+[![](assets/pypi.png)](https://pypi.org/project/pizazz)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/www.png)](https://www.justpython.tech)
-[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/email.png)](mailto:stephen.ra.king@gmail.com)
+[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/email.png)](mailto:sking.github@gmail.com)
 
-Author: Stephen R A King
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
+
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Distributed under the MIT License. See `LICENSE` for more information.
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [rpi-gpio-url]: https://pypi.org/project/RPi.GPIO/
 [status-board-url]: https://thepihut.com/products/status-board-pro
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://pycqa.github.io/isort/
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[license-image]: https://img.shields.io/pypi/l/pizazz
+[license-url]: https://github.com/Stephen-RA-King/pizazz/blob/main/LICENSE
 [mit-license-image]: https://img.shields.io/badge/license-MIT-blue
 [mit-license-url]: https://choosealicense.com/licenses/mit/
 [wiki]: https://github.com/stephen-ra-king/pizazz/wiki
```

### Comparing `pizazz-1.3.0/README.md` & `pizazz-1.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Pizazz
 
-> A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.
+\_**A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.**-
 
 [![PyPI version](https://badge.fury.io/py/pizazz.svg)](https://badge.fury.io/py/pizazz)
 [![Documentation Status](https://readthedocs.org/projects/pizazz/badge/?version=latest)](https://pizazz.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/personalized-badge/pizazz?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pizazz)
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -19,18 +19,18 @@
 That is great in itself however 595's can be daisy-chained together to give you multiples of 8 pin outputs yet still
 always controlled by only 3 input pins! Wow!
 
 If you are not sure why this is useful then let me explain.
 
 I had a requirement to create a LED "Status Board" for a monitoring and automation application that I am also writing.
 The status board would reflect the current operation status of things like Jenkins jobs, Github Actions, Linux services etc etc.
-I needed a minimum of 16 LEDs. Now there already exists a [**status board**][status-board-url] HAT. However it only tracks 5 items.
+I needed a minimum of 16 LEDs. Now there already exists a [**status board**][status-board-url] HAT. However it only tracks 5 items (that is 10 LED's). However, each LED requires it's own GPIO and the HAT masks all other pins making them unavailable.
 
 Using the Raspberry [**RPi.GPIO**][rpi-gpio-url] library it is possible to individually switch the 27 GPIO pins. However each LED would require
-a wire from the GPIO pin. This is very physically unwieldy and clunky to control in python.
+a wire from the GPIO pin. This is very physically unwieldy and clunky to control in Python.
 
 Enter the 74HC595...
 
 This class enables you to individually control any number of LEDS (or other output devices) with only 3 GPIO pins.
 
 ### Basic Wiring of the 74HC595 8-bit shift register to a Raspberry Pi
 
@@ -67,22 +67,26 @@
 2. Bit 0 in the Shift Register accepts the current value on DATA pin. At the rising edge of the pulse, if the data pin is high, then a 1 gets pushed into the shift register. Otherwise, it is a 0.
 
 On enabling the Latch pin, the contents of Shift Register are copied into the Storage Register.
 Each bit of the Storage Register is connected to one of the output pins Q0–Q7 of the IC, so in general, when the value in the Storage Register changes, so do the outputs.
 
 ## Installation
 
+---
+
 Raspberry Pi:
 
 ```sh
 pip3 install pizazz
 ```
 
 ## Connecting the Raspberry Pi
 
+---
+
 The 40 pins of the Raspberry Pi are GPIO, 5v, 3.3V and ground. Some of the GPIO pins can have special purposes.
 However, all of them can be controlled by the RPi.GPIO Python Library.
 The RPi.GPIO requires that you specify how you will identify the pins that you use. There are 2 ways:
 
 1. **GPIO.BOARD:** option specifies that you are referring to the pins by the number of the pin.
 
 2. **BCM:** option means that you are referring to the pins by the "Broadcom SOC channel" number, these are
@@ -90,20 +94,23 @@
 
 So referring to the diagram below: BCM mode GPIO2 is the same as BOARD mode pin 2
 
 ![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/40pinheader.png)
 
 Connect any GPIO's to the clock, latch and data pins of the register and connect the the 5v supply and earth
 as indicated in the register diagram.
+If you are connecting the outputs to LED's then you need to wire 330 ohm resistors serially to protect them in the usual way.
 
 ## Library Usage examples
 
+---
+
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
-https://user-images.githubusercontent.com/33905365/163853342-a1a19d5e-e392-483d-845f-40bfe25d4cb3.mp4
+https://user-images.githubusercontent.com/33905365/220999848-e6062e9d-af53-4c91-8db8-0f8b5fdf1ff3.mp4
 
 Import the library
 
 ```sh
 from pizazz.pizazz import HC595
 ```
 
@@ -185,38 +192,54 @@
 
 ```sh
 shifter.set_pattern([0, 0, 1, 1, 0, 0, 0, 0])
 ```
 
 ## Documentation
 
-[**Read the Docs**](https://pizazz.readthedocs.io/en/latest/)
+---
+
+[**Read the Docs**](https://pizazz.readthedocs.io/en/latest/?)
+
+- [**Example Usage**](https://pizazz.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://pizazz.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://pizazz.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://pizazz.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**][wiki]
 
 ## Meta
 
-[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/linkedin.png)](https://linkedin.com/in/stephen-k-3a4644210)
+---
+
+[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/github.png)](https://github.com/Stephen-RA-King/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pizazz/)
+[![](assets/pypi.png)](https://pypi.org/project/pizazz)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/www.png)](https://www.justpython.tech)
-[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/email.png)](mailto:stephen.ra.king@gmail.com)
+[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/email.png)](mailto:sking.github@gmail.com)
+
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
-Author: Stephen R A King
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Distributed under the MIT License. See `LICENSE` for more information.
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [rpi-gpio-url]: https://pypi.org/project/RPi.GPIO/
 [status-board-url]: https://thepihut.com/products/status-board-pro
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://pycqa.github.io/isort/
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[license-image]: https://img.shields.io/pypi/l/pizazz
+[license-url]: https://github.com/Stephen-RA-King/pizazz/blob/main/LICENSE
 [mit-license-image]: https://img.shields.io/badge/license-MIT-blue
 [mit-license-url]: https://choosealicense.com/licenses/mit/
 [wiki]: https://github.com/stephen-ra-king/pizazz/wiki
```

### Comparing `pizazz-1.3.0/pyproject.toml` & `pizazz-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.0/setup.cfg` & `pizazz-1.3.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 697a 617a 7a0d 0a76 6572 7369   = pizazz..versi
 00000020: 6f6e 203d 2061 7474 723a 2070 697a 617a  on = attr: pizaz
 00000030: 7a2e 5f5f 7665 7273 696f 6e5f 5f0d 0a61  z.__version__..a
 00000040: 7574 686f 7220 3d20 5374 6570 6865 6e20  uthor = Stephen 
 00000050: 5220 4120 4b69 6e67 0d0a 6175 7468 6f72  R A King..author
-00000060: 5f65 6d61 696c 203d 2073 7465 7068 656e  _email = stephen
-00000070: 2e72 612e 6b69 6e67 4067 6d61 696c 2e63  .ra.king@gmail.c
-00000080: 6f6d 0d0a 6d61 696e 7461 696e 6572 203d  om..maintainer =
-00000090: 2053 7465 7068 656e 2052 2041 204b 696e   Stephen R A Kin
-000000a0: 670d 0a6d 6169 6e74 6169 6e65 725f 656d  g..maintainer_em
-000000b0: 6169 6c20 3d20 7374 6570 6865 6e2e 7261  ail = stephen.ra
-000000c0: 2e6b 696e 6740 676d 6169 6c2e 636f 6d0d  .king@gmail.com.
-000000d0: 0a64 6573 6372 6970 7469 6f6e 203d 2045  .description = E
-000000e0: 6173 7920 636f 6e66 6967 7572 6174 696f  asy configuratio
-000000f0: 6e20 616e 6420 636f 6e74 726f 6c20 6f66  n and control of
-00000100: 2037 3448 4335 3935 2053 6869 6674 2052   74HC595 Shift R
-00000110: 6567 6973 7465 7273 206f 6e20 6120 5261  egisters on a Ra
-00000120: 7370 6265 7272 7920 5069 0d0a 6c6f 6e67  spberry Pi..long
-00000130: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-00000140: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-00000150: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000160: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000170: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a6b  text/markdown..k
-00000180: 6579 776f 7264 7320 3d20 7574 696c 6974  eywords = utilit
-00000190: 792c 2037 3448 4335 3935 2c20 4750 494f  y, 74HC595, GPIO
-000001a0: 2c20 5261 7370 6265 7272 792c 2050 690d  , Raspberry, Pi.
-000001b0: 0a70 6c61 7466 6f72 6d73 203d 204c 696e  .platforms = Lin
-000001c0: 7578 0d0a 7572 6c20 3d20 6874 7470 733a  ux..url = https:
-000001d0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7465  //github.com/ste
-000001e0: 7068 656e 2d72 612d 6b69 6e67 2f70 697a  phen-ra-king/piz
-000001f0: 617a 7a0d 0a64 6f77 6e6c 6f61 645f 7572  azz..download_ur
-00000200: 6c20 3d20 0d0a 6c69 6365 6e73 6520 3d20  l = ..license = 
-00000210: 4d49 540d 0a63 6c61 7373 6966 6965 7273  MIT..classifiers
-00000220: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
-00000230: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
-00000240: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
-00000250: 650d 0a09 496e 7465 6e64 6564 2041 7564  e...Intended Aud
-00000260: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000270: 6572 730d 0a09 4f70 6572 6174 696e 6720  ers...Operating 
-00000280: 5379 7374 656d 203a 3a20 504f 5349 5820  System :: POSIX 
-00000290: 3a3a 204c 696e 7578 0d0a 094e 6174 7572  :: Linux...Natur
-000002a0: 616c 204c 616e 6775 6167 6520 3a3a 2045  al Language :: E
-000002b0: 6e67 6c69 7368 0d0a 0950 726f 6772 616d  nglish...Program
-000002c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002d0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
-000002e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000300: 2033 203a 3a20 4f6e 6c79 0d0a 0950 726f   3 :: Only...Pro
-00000310: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000320: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000330: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
-00000340: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000350: 686f 6e20 3a3a 2033 2e39 0d0a 0950 726f  hon :: 3.9...Pro
-00000360: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000370: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000380: 2e31 300d 0a0d 0a5b 6f70 7469 6f6e 735d  .10....[options]
-00000390: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-000003a0: 0d0a 093d 7372 630d 0a70 6163 6b61 6765  ...=src..package
-000003b0: 7320 3d20 6669 6e64 3a0d 0a69 6e63 6c75  s = find:..inclu
-000003c0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-000003d0: 3d20 5472 7565 0d0a 7079 7468 6f6e 5f72  = True..python_r
-000003e0: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
-000003f0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000400: 7320 3d20 0d0a 0d0a 5b6f 7074 696f 6e73  s = ....[options
-00000410: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000420: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-00000430: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-00000440: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
-00000450: 7363 7269 7074 7320 3d20 0d0a 0970 697a  scripts = ...piz
-00000460: 617a 7a20 3d20 7069 7a61 7a7a 2e63 6c69  azz = pizazz.cli
-00000470: 3a65 6e74 7279 5f70 6f69 6e74 0d0a 0d0a  :entry_point....
-00000480: 5b66 6c61 6b65 385d 0d0a 646f 6373 7472  [flake8]..docstr
-00000490: 696e 672d 636f 6e76 656e 7469 6f6e 203d  ing-convention =
-000004a0: 206e 756d 7079 0d0a 6d61 782d 636f 6d70   numpy..max-comp
-000004b0: 6c65 7869 7479 203d 2031 380d 0a6d 6178  lexity = 18..max
-000004c0: 2d6c 696e 652d 6c65 6e67 7468 203d 2038  -line-length = 8
-000004d0: 380d 0a73 656c 6563 7420 3d20 422c 2042  8..select = B, B
-000004e0: 392c 2043 2c20 442c 2045 2c20 462c 204e  9, C, D, E, F, N
-000004f0: 2c20 570d 0a65 7863 6c75 6465 203d 2074  , W..exclude = t
-00000500: 6573 7473 2f2a 2c2e 746f 782f 2a2c 2e6e  ests/*,.tox/*,.n
-00000510: 6f78 2f2a 2c64 6f63 732f 2a2c 2e67 6974  ox/*,docs/*,.git
-00000520: 2f2a 2c2e 6769 7468 7562 2f2a 0d0a 6967  /*,.github/*..ig
-00000530: 6e6f 7265 203d 200d 0a09 4532 3033 2c0d  nore = ...E203,.
-00000540: 0a09 5735 3033 2c0d 0a70 6572 2d66 696c  ..W503,..per-fil
-00000550: 652d 6967 6e6f 7265 7320 3d20 0d0a 095f  e-ignores = ..._
-00000560: 5f69 6e69 745f 5f2e 7079 3a46 3430 310d  _init__.py:F401.
-00000570: 0a09 7061 7468 6d61 6769 632e 7079 3a46  ..pathmagic.py:F
-00000580: 3430 310d 0a09 7465 7374 5f70 697a 617a  401...test_pizaz
-00000590: 7a2e 7079 3a46 3430 310d 0a0d 0a5b 6567  z.py:F401....[eg
-000005a0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000005b0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000005c0: 3d20 300d 0a0d 0a                        = 0....
+00000060: 5f65 6d61 696c 203d 2073 6b69 6e67 2e67  _email = sking.g
+00000070: 6974 6875 6240 676d 6169 6c2e 636f 6d0d  ithub@gmail.com.
+00000080: 0a6d 6169 6e74 6169 6e65 7220 3d20 5374  .maintainer = St
+00000090: 6570 6865 6e20 5220 4120 4b69 6e67 0d0a  ephen R A King..
+000000a0: 6d61 696e 7461 696e 6572 5f65 6d61 696c  maintainer_email
+000000b0: 203d 2073 6b69 6e67 2e67 6974 6875 6240   = sking.github@
+000000c0: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
+000000d0: 6970 7469 6f6e 203d 2045 6173 7920 636f  iption = Easy co
+000000e0: 6e66 6967 7572 6174 696f 6e20 616e 6420  nfiguration and 
+000000f0: 636f 6e74 726f 6c20 6f66 2037 3448 4335  control of 74HC5
+00000100: 3935 2053 6869 6674 2052 6567 6973 7465  95 Shift Registe
+00000110: 7273 206f 6e20 6120 5261 7370 6265 7272  rs on a Raspberr
+00000120: 7920 5069 0d0a 6c6f 6e67 5f64 6573 6372  y Pi..long_descr
+00000130: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+00000140: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+00000150: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000160: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000170: 6172 6b64 6f77 6e0d 0a6b 6579 776f 7264  arkdown..keyword
+00000180: 7320 3d20 7574 696c 6974 792c 2037 3448  s = utility, 74H
+00000190: 4335 3935 2c20 4750 494f 2c20 5261 7370  C595, GPIO, Rasp
+000001a0: 6265 7272 792c 2050 690d 0a70 6c61 7466  berry, Pi..platf
+000001b0: 6f72 6d73 203d 204c 696e 7578 0d0a 7572  orms = Linux..ur
+000001c0: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+000001d0: 7562 2e63 6f6d 2f73 7465 7068 656e 2d72  ub.com/stephen-r
+000001e0: 612d 6b69 6e67 2f70 697a 617a 7a0d 0a64  a-king/pizazz..d
+000001f0: 6f77 6e6c 6f61 645f 7572 6c20 3d20 0d0a  ownload_url = ..
+00000200: 6c69 6365 6e73 6520 3d20 4d49 540d 0a63  license = MIT..c
+00000210: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+00000220: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+00000230: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
+00000240: 7469 6f6e 2f53 7461 626c 650d 0a09 496e  tion/Stable...In
+00000250: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000260: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
+00000270: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000280: 203a 3a20 504f 5349 5820 3a3a 204c 696e   :: POSIX :: Lin
+00000290: 7578 0d0a 094e 6174 7572 616c 204c 616e  ux...Natural Lan
+000002a0: 6775 6167 6520 3a3a 2045 6e67 6c69 7368  guage :: English
+000002b0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000002c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002d0: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
+000002e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002f0: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
+00000300: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
+00000310: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000320: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
+00000330: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000340: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000350: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
+00000360: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000370: 7974 686f 6e20 3a3a 2033 2e31 300d 0a0d  ython :: 3.10...
+00000380: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
+00000390: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
+000003a0: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
+000003b0: 6e64 3a0d 0a69 6e63 6c75 6465 5f70 6163  nd:..include_pac
+000003c0: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
+000003d0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+000003e0: 7320 3d20 3e3d 332e 380d 0a69 6e73 7461  s = >=3.8..insta
+000003f0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
+00000400: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000410: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
+00000420: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
+00000430: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
+00000440: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
+00000450: 7320 3d20 0d0a 0970 697a 617a 7a20 3d20  s = ...pizazz = 
+00000460: 7069 7a61 7a7a 2e63 6c69 3a65 6e74 7279  pizazz.cli:entry
+00000470: 5f70 6f69 6e74 0d0a 0d0a 5b66 6c61 6b65  _point....[flake
+00000480: 385d 0d0a 646f 6373 7472 696e 672d 636f  8]..docstring-co
+00000490: 6e76 656e 7469 6f6e 203d 206e 756d 7079  nvention = numpy
+000004a0: 0d0a 6d61 782d 636f 6d70 6c65 7869 7479  ..max-complexity
+000004b0: 203d 2031 380d 0a6d 6178 2d6c 696e 652d   = 18..max-line-
+000004c0: 6c65 6e67 7468 203d 2038 380d 0a73 656c  length = 88..sel
+000004d0: 6563 7420 3d20 422c 2042 392c 2043 2c20  ect = B, B9, C, 
+000004e0: 442c 2045 2c20 462c 204e 2c20 570d 0a65  D, E, F, N, W..e
+000004f0: 7863 6c75 6465 203d 2074 6573 7473 2f2a  xclude = tests/*
+00000500: 2c2e 746f 782f 2a2c 2e6e 6f78 2f2a 2c64  ,.tox/*,.nox/*,d
+00000510: 6f63 732f 2a2c 2e67 6974 2f2a 2c2e 6769  ocs/*,.git/*,.gi
+00000520: 7468 7562 2f2a 0d0a 6967 6e6f 7265 203d  thub/*..ignore =
+00000530: 200d 0a09 4532 3033 2c0d 0a09 5735 3033   ...E203,...W503
+00000540: 2c0d 0a70 6572 2d66 696c 652d 6967 6e6f  ,..per-file-igno
+00000550: 7265 7320 3d20 0d0a 095f 5f69 6e69 745f  res = ...__init_
+00000560: 5f2e 7079 3a46 3430 310d 0a09 7061 7468  _.py:F401...path
+00000570: 6d61 6769 632e 7079 3a46 3430 310d 0a09  magic.py:F401...
+00000580: 7465 7374 5f70 697a 617a 7a2e 7079 3a46  test_pizazz.py:F
+00000590: 3430 310d 0a0d 0a5b 6567 675f 696e 666f  401....[egg_info
+000005a0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000005b0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+000005c0: 0a                                       .
```

### Comparing `pizazz-1.3.0/src/pizazz/pizazz.py` & `pizazz-1.3.1/src/pizazz/pizazz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 """A utility class to leverage 74HC595 shift register chips with a Raspberry Pi."""
 
 # Core Library modules
 import time
 from typing import Union
 
 # Third party modules
```

### Comparing `pizazz-1.3.0/src/pizazz.egg-info/PKG-INFO` & `pizazz-1.3.1/src/pizazz.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pizazz
-Version: 1.3.0
+Version: 1.3.1
 Summary: Easy configuration and control of 74HC595 Shift Registers on a Raspberry Pi
 Home-page: https://github.com/stephen-ra-king/pizazz
 Download-URL: 
 Author: Stephen R A King
-Author-email: stephen.ra.king@gmail.com
+Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
-Maintainer-email: stephen.ra.king@gmail.com
+Maintainer-email: sking.github@gmail.com
 License: MIT
 Keywords: utility,74HC595,GPIO,Raspberry,Pi
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # Pizazz
 
-> A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.
+\_**A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.**-
 
 [![PyPI version](https://badge.fury.io/py/pizazz.svg)](https://badge.fury.io/py/pizazz)
 [![Documentation Status](https://readthedocs.org/projects/pizazz/badge/?version=latest)](https://pizazz.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/personalized-badge/pizazz?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pizazz)
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -46,18 +46,18 @@
 That is great in itself however 595's can be daisy-chained together to give you multiples of 8 pin outputs yet still
 always controlled by only 3 input pins! Wow!
 
 If you are not sure why this is useful then let me explain.
 
 I had a requirement to create a LED "Status Board" for a monitoring and automation application that I am also writing.
 The status board would reflect the current operation status of things like Jenkins jobs, Github Actions, Linux services etc etc.
-I needed a minimum of 16 LEDs. Now there already exists a [**status board**][status-board-url] HAT. However it only tracks 5 items.
+I needed a minimum of 16 LEDs. Now there already exists a [**status board**][status-board-url] HAT. However it only tracks 5 items (that is 10 LED's). However, each LED requires it's own GPIO and the HAT masks all other pins making them unavailable.
 
 Using the Raspberry [**RPi.GPIO**][rpi-gpio-url] library it is possible to individually switch the 27 GPIO pins. However each LED would require
-a wire from the GPIO pin. This is very physically unwieldy and clunky to control in python.
+a wire from the GPIO pin. This is very physically unwieldy and clunky to control in Python.
 
 Enter the 74HC595...
 
 This class enables you to individually control any number of LEDS (or other output devices) with only 3 GPIO pins.
 
 ### Basic Wiring of the 74HC595 8-bit shift register to a Raspberry Pi
 
@@ -94,22 +94,26 @@
 2. Bit 0 in the Shift Register accepts the current value on DATA pin. At the rising edge of the pulse, if the data pin is high, then a 1 gets pushed into the shift register. Otherwise, it is a 0.
 
 On enabling the Latch pin, the contents of Shift Register are copied into the Storage Register.
 Each bit of the Storage Register is connected to one of the output pins Q0–Q7 of the IC, so in general, when the value in the Storage Register changes, so do the outputs.
 
 ## Installation
 
+---
+
 Raspberry Pi:
 
 ```sh
 pip3 install pizazz
 ```
 
 ## Connecting the Raspberry Pi
 
+---
+
 The 40 pins of the Raspberry Pi are GPIO, 5v, 3.3V and ground. Some of the GPIO pins can have special purposes.
 However, all of them can be controlled by the RPi.GPIO Python Library.
 The RPi.GPIO requires that you specify how you will identify the pins that you use. There are 2 ways:
 
 1. **GPIO.BOARD:** option specifies that you are referring to the pins by the number of the pin.
 
 2. **BCM:** option means that you are referring to the pins by the "Broadcom SOC channel" number, these are
@@ -117,20 +121,23 @@
 
 So referring to the diagram below: BCM mode GPIO2 is the same as BOARD mode pin 2
 
 ![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/40pinheader.png)
 
 Connect any GPIO's to the clock, latch and data pins of the register and connect the the 5v supply and earth
 as indicated in the register diagram.
+If you are connecting the outputs to LED's then you need to wire 330 ohm resistors serially to protect them in the usual way.
 
 ## Library Usage examples
 
+---
+
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
-https://user-images.githubusercontent.com/33905365/163853342-a1a19d5e-e392-483d-845f-40bfe25d4cb3.mp4
+https://user-images.githubusercontent.com/33905365/220999848-e6062e9d-af53-4c91-8db8-0f8b5fdf1ff3.mp4
 
 Import the library
 
 ```sh
 from pizazz.pizazz import HC595
 ```
 
@@ -212,38 +219,54 @@
 
 ```sh
 shifter.set_pattern([0, 0, 1, 1, 0, 0, 0, 0])
 ```
 
 ## Documentation
 
-[**Read the Docs**](https://pizazz.readthedocs.io/en/latest/)
+---
+
+[**Read the Docs**](https://pizazz.readthedocs.io/en/latest/?)
+
+- [**Example Usage**](https://pizazz.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://pizazz.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://pizazz.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://pizazz.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**][wiki]
 
 ## Meta
 
-[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/linkedin.png)](https://linkedin.com/in/stephen-k-3a4644210)
+---
+
+[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/github.png)](https://github.com/Stephen-RA-King/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pizazz/)
+[![](assets/pypi.png)](https://pypi.org/project/pizazz)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/www.png)](https://www.justpython.tech)
-[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/email.png)](mailto:stephen.ra.king@gmail.com)
+[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/email.png)](mailto:sking.github@gmail.com)
 
-Author: Stephen R A King
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
+
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Distributed under the MIT License. See `LICENSE` for more information.
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [rpi-gpio-url]: https://pypi.org/project/RPi.GPIO/
 [status-board-url]: https://thepihut.com/products/status-board-pro
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://pycqa.github.io/isort/
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[license-image]: https://img.shields.io/pypi/l/pizazz
+[license-url]: https://github.com/Stephen-RA-King/pizazz/blob/main/LICENSE
 [mit-license-image]: https://img.shields.io/badge/license-MIT-blue
 [mit-license-url]: https://choosealicense.com/licenses/mit/
 [wiki]: https://github.com/stephen-ra-king/pizazz/wiki
```

