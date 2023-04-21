# Comparing `tmp/neuromeka-clients-0.1.2.tar.gz` & `tmp/neuromeka-clients-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuromeka-clients-0.1.2.tar", last modified: Fri Apr  7 10:01:14 2023, max compression
+gzip compressed data, was "neuromeka-clients-0.1.4.tar", last modified: Fri Apr 21 04:20:16 2023, max compression
```

## Comparing `neuromeka-clients-0.1.2.tar` & `neuromeka-clients-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 10:01:14.529444 neuromeka-clients-0.1.2/
--rw-rw-rw-   0        0        0     2126 2023-04-07 10:01:14.528469 neuromeka-clients-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1199 2023-04-06 12:40:10.000000 neuromeka-clients-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 10:01:14.425014 neuromeka-clients-0.1.2/neuromeka/
--rw-rw-rw-   0        0        0      117 2023-04-06 23:37:07.000000 neuromeka-clients-0.1.2/neuromeka/__init__.py
--rw-rw-rw-   0        0        0     7442 2023-04-06 12:30:11.000000 neuromeka-clients-0.1.2/neuromeka/ecat.py
--rw-rw-rw-   0        0        0    10651 2023-04-06 11:41:45.000000 neuromeka-clients-0.1.2/neuromeka/indy.py
--rw-rw-rw-   0        0        0     7394 2023-04-07 08:00:44.000000 neuromeka-clients-0.1.2/neuromeka/moby.py
--rw-rw-rw-   0        0        0     3379 2023-04-06 11:41:58.000000 neuromeka-clients-0.1.2/neuromeka/motor.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:01:14.496263 neuromeka-clients-0.1.2/neuromeka/proto/
--rw-rw-rw-   0        0        0    65863 2023-04-04 06:23:00.000000 neuromeka-clients-0.1.2/neuromeka/proto/EtherCATCommgRPCServer_pb2.py
--rw-rw-rw-   0        0        0    61370 2023-04-06 12:15:44.000000 neuromeka-clients-0.1.2/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py
--rw-rw-rw-   0        0        0    61466 2023-03-16 08:41:07.000000 neuromeka-clients-0.1.2/neuromeka/proto/IndygRPCTask_pb2.py
--rw-rw-rw-   0        0        0   128168 2023-03-16 08:41:07.000000 neuromeka-clients-0.1.2/neuromeka/proto/IndygRPCTask_pb2_grpc.py
--rw-rw-rw-   0        0        0    74988 2023-04-04 06:23:04.000000 neuromeka-clients-0.1.2/neuromeka/proto/MobygRPCServer_pb2.py
--rw-rw-rw-   0        0        0    54393 2023-04-04 06:23:04.000000 neuromeka-clients-0.1.2/neuromeka/proto/MobygRPCServer_pb2_grpc.py
--rw-rw-rw-   0        0        0    41733 2023-04-04 06:23:10.000000 neuromeka-clients-0.1.2/neuromeka/proto/MotorControlgRPCServer_pb2.py
--rw-rw-rw-   0        0        0    39460 2023-04-04 06:23:10.000000 neuromeka-clients-0.1.2/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py
--rw-rw-rw-   0        0        0        0 2023-04-06 12:35:30.000000 neuromeka-clients-0.1.2/neuromeka/proto/__init__.py
--rw-rw-rw-   0        0        0      519 2023-04-06 12:33:27.000000 neuromeka-clients-0.1.2/neuromeka/proto/grpc_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:01:14.523590 neuromeka-clients-0.1.2/neuromeka_clients.egg-info/
--rw-rw-rw-   0        0        0     2126 2023-04-07 10:01:14.000000 neuromeka-clients-0.1.2/neuromeka_clients.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      729 2023-04-07 10:01:14.000000 neuromeka-clients-0.1.2/neuromeka_clients.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 10:01:14.000000 neuromeka-clients-0.1.2/neuromeka_clients.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-07 10:01:14.000000 neuromeka-clients-0.1.2/neuromeka_clients.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-07 10:01:14.000000 neuromeka-clients-0.1.2/neuromeka_clients.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 10:01:14.529444 neuromeka-clients-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1221 2023-04-07 10:00:12.000000 neuromeka-clients-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.235648 neuromeka-clients-0.1.4/
+-rw-rw-rw-   0        0        0     1076 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2168 2023-04-21 04:20:16.235648 neuromeka-clients-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1311 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.105648 neuromeka-clients-0.1.4/neuromeka/
+-rw-rw-rw-   0        0        0      148 2023-04-18 02:59:59.000000 neuromeka-clients-0.1.4/neuromeka/__init__.py
+-rw-rw-rw-   0        0        0     7442 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/ecat.py
+-rw-rw-rw-   0        0        0    14598 2023-04-18 04:44:44.000000 neuromeka-clients-0.1.4/neuromeka/eye.py
+-rw-rw-rw-   0        0        0    10651 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/indy.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.115649 neuromeka-clients-0.1.4/neuromeka/indy_dcp/
+-rw-rw-rw-   0        0        0        0 2020-01-22 08:47:24.000000 neuromeka-clients-0.1.4/neuromeka/indy_dcp/__init__.py
+-rw-rw-rw-   0        0        0    21703 2020-04-14 06:11:08.000000 neuromeka-clients-0.1.4/neuromeka/indy_dcp/indy_program_maker.py
+-rw-rw-rw-   0        0        0    61482 2020-07-10 04:18:53.000000 neuromeka-clients-0.1.4/neuromeka/indy_dcp/indydcp_client.py
+-rw-rw-rw-   0        0        0     7436 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/neuromeka/moby.py
+-rw-rw-rw-   0        0        0     3379 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/motor.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.225648 neuromeka-clients-0.1.4/neuromeka/proto/
+-rw-rw-rw-   0        0        0    65863 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/EtherCATCommgRPCServer_pb2.py
+-rw-rw-rw-   0        0        0    61370 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5567 2023-04-18 02:59:14.000000 neuromeka-clients-0.1.4/neuromeka/proto/EyeTask_pb2.py
+-rw-rw-rw-   0        0        0     6780 2023-04-18 02:59:14.000000 neuromeka-clients-0.1.4/neuromeka/proto/EyeTask_pb2_grpc.py
+-rw-rw-rw-   0        0        0    61466 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/IndygRPCTask_pb2.py
+-rw-rw-rw-   0        0        0   128168 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/IndygRPCTask_pb2_grpc.py
+-rw-rw-rw-   0        0        0    74574 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/neuromeka/proto/MobygRPCServer_pb2.py
+-rw-rw-rw-   0        0        0    52785 2023-04-18 01:34:49.000000 neuromeka-clients-0.1.4/neuromeka/proto/MobygRPCServer_pb2_grpc.py
+-rw-rw-rw-   0        0        0    41733 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/MotorControlgRPCServer_pb2.py
+-rw-rw-rw-   0        0        0    39460 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py
+-rw-rw-rw-   0        0        0        0 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-04-18 01:34:41.000000 neuromeka-clients-0.1.4/neuromeka/proto/grpc_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:20:16.235648 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/
+-rw-rw-rw-   0        0        0     2168 2023-04-21 04:20:15.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2023-04-21 04:20:16.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:20:15.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-04-21 04:20:15.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 04:20:15.000000 neuromeka-clients-0.1.4/neuromeka_clients.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 04:20:16.235648 neuromeka-clients-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1186 2023-04-21 04:20:07.000000 neuromeka-clients-0.1.4/setup.py
```

### Comparing `neuromeka-clients-0.1.2/PKG-INFO` & `neuromeka-clients-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: neuromeka-clients
-Version: 0.1.2
-Summary: Neuromeka client protocols for Indy, Moby, Ecat, and Motor
+Version: 0.1.4
+Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients
-Author: Your Name
+Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Neuromeka Clients
 
 This package provides client protocols for users to interact with Neuromeka's products, including Indy, Moby, Ecat, and Motor.
 
 ## Installation
 
@@ -38,35 +37,37 @@
 * MobyClient in moby.py
 * EcatClient in ecat.py
 * MotorClient in motor.py
 
 To use a client class, simply import it and create an instance:
 
 ```python
-from neuromeka.ecat import EcatClient
+from neuromeka import EcatClient, MobyClient, IndyClient, MotorClient
 
-ecat_client = EcatClient("192.168.214.20")
+ecat = EcatClient("192.168.214.20")
+moby = IndyClient("192.168.214.20")
+indy = IndyClient("192.168.0.11")
+motor = MotorClient("192.168.0.20")
 ```
 
 Replace EcatClient with the desired client class and the IP address with the appropriate address for your device.
 
 ## Dependencies
 This package requires the following dependencies:
 
 * grpcio
 * grpcio-tools
 * protobuf
-* six
 
 These dependencies will be automatically installed when you install the package using pip.
 
 ## Examples
 Please refer to the 'example.py' file in the package for usage examples.
 
 ## Support
 If you encounter any issues or need help, please open an issue on the project's repository.
 
 ## License
-This package is released under the [LICENSE_NAME]. For more information, please refer to the LICENSE file.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `neuromeka-clients-0.1.2/README.md` & `neuromeka-clients-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,35 +17,37 @@
 * MobyClient in moby.py
 * EcatClient in ecat.py
 * MotorClient in motor.py
 
 To use a client class, simply import it and create an instance:
 
 ```python
-from neuromeka.ecat import EcatClient
+from neuromeka import EcatClient, MobyClient, IndyClient, MotorClient
 
-ecat_client = EcatClient("192.168.214.20")
+ecat = EcatClient("192.168.214.20")
+moby = IndyClient("192.168.214.20")
+indy = IndyClient("192.168.0.11")
+motor = MotorClient("192.168.0.20")
 ```
 
 Replace EcatClient with the desired client class and the IP address with the appropriate address for your device.
 
 ## Dependencies
 This package requires the following dependencies:
 
 * grpcio
 * grpcio-tools
 * protobuf
-* six
 
 These dependencies will be automatically installed when you install the package using pip.
 
 ## Examples
 Please refer to the 'example.py' file in the package for usage examples.
 
 ## Support
 If you encounter any issues or need help, please open an issue on the project's repository.
 
 ## License
-This package is released under the [LICENSE_NAME]. For more information, please refer to the LICENSE file.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `neuromeka-clients-0.1.2/neuromeka/ecat.py` & `neuromeka-clients-0.1.4/neuromeka/ecat.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka/indy.py` & `neuromeka-clients-0.1.4/neuromeka/indy.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka/moby.py` & `neuromeka-clients-0.1.4/neuromeka/moby.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,42 +56,45 @@
             }
         
         return error_dict.get(error_code, "Normal (UNKNOWN ERROR CODE)")
 
     def recover(self):
         return self.stub.Recover()
     
-    ## Get Moby's odometry and physical data
+    ## Get Moby's odometry data
     def get_moby_pose(self):
         pose = self.stub.GetMobyPose(Empty())
         return [pose.px, pose.py, pose.pw]
     
     def get_moby_vel(self):
         vel = self.stub.GetMobyVel(Empty())
         return [vel.vx, vel.vy, vel.vw]
     
     def reset_moby_pose(self):
         return self.stub.ResetMobyPose(Empty())
     
+    def get_target_vel(self):
+        target = self.stub.GetTargetVel(Empty())
+        return [target.vx, target.vy, target.vw]
+    
+    ## Swerve drive    
     def get_rotation_angle(self):
         val = self.stub.GetRotationAngleDeg(Empty())
         return {'fl': val.fl, 'fr': val.fr, 'bl':val.bl, 'br':val.br}
     
     def get_drive_speed(self):
         val = self.stub.GetDriveSpeed(Empty())
         return {'fl': val.fl, 'fr': val.fr, 'bl':val.bl, 'br':val.br}
     
-    def get_target_vel(self):
-        target = self.stub.GetTargetVel(Empty())
-        return [target.vx, target.vy, target.vw]
-    
     def get_zero(self):
         val = self.stub.GetRotationZeroCount(Empty())
         return {'fl': val.fl, 'fr': val.fr, 'bl':val.bl, 'br':val.br}
     
+    ## Differential drive
+    
     def get_cmode(self):
         return self.stub.GetCMode(Empty()).val    
     
     ## Get sensor data
     def get_gyro_data(self):
         return self.stub.GetGyroData(Empty()).val
```

### Comparing `neuromeka-clients-0.1.2/neuromeka/motor.py` & `neuromeka-clients-0.1.4/neuromeka/motor.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka/proto/EtherCATCommgRPCServer_pb2.py` & `neuromeka-clients-0.1.4/neuromeka/proto/EtherCATCommgRPCServer_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py` & `neuromeka-clients-0.1.4/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka/proto/IndygRPCTask_pb2.py` & `neuromeka-clients-0.1.4/neuromeka/proto/IndygRPCTask_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka/proto/IndygRPCTask_pb2_grpc.py` & `neuromeka-clients-0.1.4/neuromeka/proto/IndygRPCTask_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka/proto/MobygRPCServer_pb2.py` & `neuromeka-clients-0.1.4/neuromeka/proto/MobygRPCServer_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='MobygRPCServer.proto',
   package='GRPCMoby',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x14MobygRPCServer.proto\x12\x08GRPCMoby\"\x07\n\x05\x45mpty\"*\n\tJsonParam\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x10\n\x08json_str\x18\x02 \x01(\t\"}\n\rMotorDriverTx\x12\x12\n\nstatusWord\x18\x01 \x01(\r\x12\x12\n\nmodeOpDisp\x18\x02 \x01(\x05\x12\x16\n\x0e\x61\x63tualPosition\x18\x03 \x01(\x05\x12\x16\n\x0e\x61\x63tualVelocity\x18\x04 \x01(\x05\x12\x14\n\x0c\x61\x63tualTorque\x18\x05 \x01(\x05\"z\n\rMotorDriverRx\x12\x13\n\x0b\x63ontrolWord\x18\x01 \x01(\r\x12\x0e\n\x06modeOp\x18\x02 \x01(\x05\x12\x16\n\x0etargetPosition\x18\x03 \x01(\x05\x12\x16\n\x0etargetVelocity\x18\x04 \x01(\x05\x12\x14\n\x0ctargetTorque\x18\x05 \x01(\x05\"@\n\x0eMotorDriverRxs\x12.\n\rmotorDriverRx\x18\x01 \x03(\x0b\x32\x17.GRPCMoby.MotorDriverRx\"\x90\x02\n\tMobyState\x12\x0f\n\x07isReady\x18\x01 \x01(\x08\x12\x10\n\x08isMoving\x18\x02 \x01(\x08\x12\x16\n\x0eisMoveFinished\x18\x03 \x01(\x08\x12\x13\n\x0bisEmgPushed\x18\x04 \x01(\x08\x12\x14\n\x0cisErrorState\x18\x05 \x01(\x08\x12\x12\n\nisHomePose\x18\x06 \x01(\x08\x12\x16\n\x0eisRotationZero\x18\x07 \x01(\x08\x12\x13\n\x0bisResetting\x18\x08 \x01(\x08\x12\x16\n\x0eisIMUAvailable\x18\t \x01(\x08\x12\x12\n\nisCollided\x18\n \x01(\x08\x12\x18\n\x10isProgramRunning\x18\x0b \x01(\x08\x12\x16\n\x0eisProgramPause\x18\x0c \x01(\x08\"$\n\x0eMobyErrorState\x12\x12\n\nerrorState\x18\x01 \x01(\x05\".\n\x08MobyPose\x12\n\n\x02px\x18\x01 \x01(\x01\x12\n\n\x02py\x18\x02 \x01(\x01\x12\n\n\x02pw\x18\x03 \x01(\x01\"\xa5\x01\n\x07IMUData\x12\x0e\n\x06\x61ngleX\x18\x01 \x01(\x01\x12\x0e\n\x06\x61ngleY\x18\x02 \x01(\x01\x12\x0e\n\x06\x61ngleZ\x18\x03 \x01(\x01\x12\x11\n\tangleVelX\x18\x04 \x01(\x01\x12\x11\n\tangleVelY\x18\x05 \x01(\x01\x12\x11\n\tangleVelZ\x18\x06 \x01(\x01\x12\x0f\n\x07linAccX\x18\x07 \x01(\x01\x12\x0f\n\x07linAccY\x18\x08 \x01(\x01\x12\x0f\n\x07linAccZ\x18\t \x01(\x01\"-\n\x07MobyVel\x12\n\n\x02vx\x18\x01 \x01(\x01\x12\n\n\x02vy\x18\x02 \x01(\x01\x12\n\n\x02vw\x18\x03 \x01(\x01\"?\n\rSwerveDoubles\x12\n\n\x02\x66l\x18\x01 \x01(\x01\x12\n\n\x02\x66r\x18\x02 \x01(\x01\x12\n\n\x02\x62l\x18\x03 \x01(\x01\x12\n\n\x02\x62r\x18\x04 \x01(\x01\"/\n\tTargetVel\x12\n\n\x02vx\x18\x01 \x01(\x01\x12\n\n\x02vy\x18\x02 \x01(\x01\x12\n\n\x02vw\x18\x03 \x01(\x01\";\n\tZeroCount\x12\n\n\x02\x66l\x18\x01 \x01(\x05\x12\n\n\x02\x66r\x18\x02 \x01(\x05\x12\n\n\x02\x62l\x18\x03 \x01(\x05\x12\n\n\x02\x62r\x18\x04 \x01(\x05\"\xae\x01\n\x06IRData\x12\x11\n\tir_front1\x18\x01 \x01(\x05\x12\x11\n\tir_front2\x18\x02 \x01(\x05\x12\x10\n\x08ir_left1\x18\x03 \x01(\x05\x12\x10\n\x08ir_left2\x18\x04 \x01(\x05\x12\x10\n\x08ir_left3\x18\x05 \x01(\x05\x12\x0f\n\x07ir_rear\x18\x06 \x01(\x05\x12\x11\n\tir_right1\x18\x07 \x01(\x05\x12\x11\n\tir_right2\x18\x08 \x01(\x05\x12\x11\n\tir_right3\x18\t \x01(\x05\"t\n\x07\x42MSData\x12\x12\n\nbms_status\x18\x01 \x03(\x05\x12\x11\n\tpack_volt\x18\x02 \x03(\x05\x12\x14\n\x0c\x62\x61ttery_volt\x18\x03 \x03(\x05\x12\x15\n\rpack_current1\x18\x04 \x03(\x05\x12\x15\n\rpack_current2\x18\x05 \x03(\x05\"!\n\x05GBool\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0b\n\x03val\x18\x02 \x01(\x08\" \n\x04GInt\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0b\n\x03val\x18\x02 \x01(\x05\"\"\n\x06GFloat\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0b\n\x03val\x18\x02 \x01(\x02\"#\n\x07GString\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0b\n\x03val\x18\x02 \x01(\t\"\x16\n\x07\x42oolVal\x12\x0b\n\x03val\x18\x01 \x01(\x08\"\x15\n\x06IntVal\x12\x0b\n\x03val\x18\x01 \x01(\x05\"\x16\n\x07IntVals\x12\x0b\n\x03val\x18\x01 \x03(\x05\"\x17\n\x08\x46loatVal\x12\x0b\n\x03val\x18\x01 \x01(\x02\"\x18\n\tFloatVals\x12\x0b\n\x03val\x18\x01 \x03(\x02\"\x18\n\tDoubleVal\x12\x0b\n\x03val\x18\x01 \x01(\x01\"\x19\n\nDoubleVals\x12\x0b\n\x03val\x18\x01 \x03(\x01\">\n\x0cRotationGain\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\t\n\x01k\x18\x02 \x01(\x01\x12\n\n\x02kv\x18\x03 \x01(\x01\x12\n\n\x02kp\x18\x04 \x01(\x01\"9\n\x0eVelAccBoundary\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0c\n\x04vmax\x18\x02 \x01(\x02\x12\x0c\n\x04\x61max\x18\x03 \x01(\x02\x32\x8f\x10\n\x0cGRPCMobyTask\x12<\n\rGetMobyTxData\x12\x10.GRPCMoby.IntVal\x1a\x17.GRPCMoby.MotorDriverTx\"\x00\x12<\n\rGetMobyRxData\x12\x10.GRPCMoby.IntVal\x1a\x17.GRPCMoby.MotorDriverRx\"\x00\x12\x46\n\x17\x44irectMotorDriveControl\x12\x18.GRPCMoby.MotorDriverRxs\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x36\n\x0cGetMobyState\x12\x0f.GRPCMoby.Empty\x1a\x13.GRPCMoby.MobyState\"\x00\x12@\n\x11GetMobyErrorState\x12\x0f.GRPCMoby.Empty\x1a\x18.GRPCMoby.MobyErrorState\"\x00\x12-\n\x07Recover\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x34\n\x0bGetMobyPose\x12\x0f.GRPCMoby.Empty\x1a\x12.GRPCMoby.MobyPose\"\x00\x12\x32\n\nGetMobyVel\x12\x0f.GRPCMoby.Empty\x1a\x11.GRPCMoby.MobyVel\"\x00\x12\x33\n\rResetMobyPose\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x41\n\x13GetRotationAngleDeg\x12\x0f.GRPCMoby.Empty\x1a\x17.GRPCMoby.SwerveDoubles\"\x00\x12;\n\rGetDriveSpeed\x12\x0f.GRPCMoby.Empty\x1a\x17.GRPCMoby.SwerveDoubles\"\x00\x12\x36\n\x0cGetTargetVel\x12\x0f.GRPCMoby.Empty\x1a\x13.GRPCMoby.TargetVel\"\x00\x12>\n\x14GetRotationZeroCount\x12\x0f.GRPCMoby.Empty\x1a\x13.GRPCMoby.ZeroCount\"\x00\x12/\n\x08GetCMode\x12\x0f.GRPCMoby.Empty\x1a\x10.GRPCMoby.IntVal\"\x00\x12\x36\n\x0bGetGyroData\x12\x0f.GRPCMoby.Empty\x1a\x14.GRPCMoby.DoubleVals\"\x00\x12\x35\n\x0fResetGyroSensor\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x36\n\x0eUseGyroForOdom\x12\x11.GRPCMoby.BoolVal\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x37\n\x0fGetGyroFullData\x12\x0f.GRPCMoby.Empty\x1a\x11.GRPCMoby.IMUData\"\x00\x12\x36\n\x0fGetIRSensorData\x12\x0f.GRPCMoby.Empty\x1a\x10.GRPCMoby.IRData\"\x00\x12\x32\n\nGetBMSData\x12\x0f.GRPCMoby.Empty\x1a\x11.GRPCMoby.BMSData\"\x00\x12\x38\n\x0eSetStepControl\x12\x13.GRPCMoby.TargetVel\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x30\n\nStopMotion\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x41\n\x13SetRotationAngleDeg\x12\x17.GRPCMoby.SwerveDoubles\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x38\n\nDriveWheel\x12\x17.GRPCMoby.SwerveDoubles\x1a\x0f.GRPCMoby.Empty\"\x00\x12<\n\x16SetZeroPosAsCurrentPos\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12<\n\x11SetRotationVelAcc\x12\x14.GRPCMoby.DoubleVals\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x39\n\x0eSetDriveAccDec\x12\x14.GRPCMoby.DoubleVals\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x41\n\x19SetDriveInterpolatorOnOff\x12\x11.GRPCMoby.BoolVal\x1a\x0f.GRPCMoby.Empty\"\x00\x12G\n\x1cSetRotationInterpolatorParam\x12\x14.GRPCMoby.DoubleVals\x1a\x0f.GRPCMoby.Empty\"\x00\x12=\n\x15SetRotationTorqueMode\x12\x11.GRPCMoby.BoolVal\x1a\x0f.GRPCMoby.Empty\"\x00\x12<\n\x0fSetControlParam\x12\x16.GRPCMoby.RotationGain\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x34\n\x0eStartRTLogging\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x32\n\x0c\x45ndRTLogging\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x37\n\x0fSetLoggerBuffer\x12\x11.GRPCMoby.IntVals\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x32\n\x0cRTLoggerSave\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x62\x06proto3'
+  serialized_pb=b'\n\x14MobygRPCServer.proto\x12\x08GRPCMoby\"\x07\n\x05\x45mpty\"*\n\tJsonParam\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x10\n\x08json_str\x18\x02 \x01(\t\"}\n\rMotorDriverTx\x12\x12\n\nstatusWord\x18\x01 \x01(\r\x12\x12\n\nmodeOpDisp\x18\x02 \x01(\x05\x12\x16\n\x0e\x61\x63tualPosition\x18\x03 \x01(\x05\x12\x16\n\x0e\x61\x63tualVelocity\x18\x04 \x01(\x05\x12\x14\n\x0c\x61\x63tualTorque\x18\x05 \x01(\x05\"z\n\rMotorDriverRx\x12\x13\n\x0b\x63ontrolWord\x18\x01 \x01(\r\x12\x0e\n\x06modeOp\x18\x02 \x01(\x05\x12\x16\n\x0etargetPosition\x18\x03 \x01(\x05\x12\x16\n\x0etargetVelocity\x18\x04 \x01(\x05\x12\x14\n\x0ctargetTorque\x18\x05 \x01(\x05\"@\n\x0eMotorDriverRxs\x12.\n\rmotorDriverRx\x18\x01 \x03(\x0b\x32\x17.GRPCMoby.MotorDriverRx\"\x90\x02\n\tMobyState\x12\x0f\n\x07isReady\x18\x01 \x01(\x08\x12\x10\n\x08isMoving\x18\x02 \x01(\x08\x12\x16\n\x0eisMoveFinished\x18\x03 \x01(\x08\x12\x13\n\x0bisEmgPushed\x18\x04 \x01(\x08\x12\x14\n\x0cisErrorState\x18\x05 \x01(\x08\x12\x12\n\nisHomePose\x18\x06 \x01(\x08\x12\x16\n\x0eisRotationZero\x18\x07 \x01(\x08\x12\x13\n\x0bisResetting\x18\x08 \x01(\x08\x12\x16\n\x0eisIMUAvailable\x18\t \x01(\x08\x12\x12\n\nisCollided\x18\n \x01(\x08\x12\x18\n\x10isProgramRunning\x18\x0b \x01(\x08\x12\x16\n\x0eisProgramPause\x18\x0c \x01(\x08\"$\n\x0eMobyErrorState\x12\x12\n\nerrorState\x18\x01 \x01(\x05\".\n\x08MobyPose\x12\n\n\x02px\x18\x01 \x01(\x01\x12\n\n\x02py\x18\x02 \x01(\x01\x12\n\n\x02pw\x18\x03 \x01(\x01\"\xa5\x01\n\x07IMUData\x12\x0e\n\x06\x61ngleX\x18\x01 \x01(\x01\x12\x0e\n\x06\x61ngleY\x18\x02 \x01(\x01\x12\x0e\n\x06\x61ngleZ\x18\x03 \x01(\x01\x12\x11\n\tangleVelX\x18\x04 \x01(\x01\x12\x11\n\tangleVelY\x18\x05 \x01(\x01\x12\x11\n\tangleVelZ\x18\x06 \x01(\x01\x12\x0f\n\x07linAccX\x18\x07 \x01(\x01\x12\x0f\n\x07linAccY\x18\x08 \x01(\x01\x12\x0f\n\x07linAccZ\x18\t \x01(\x01\"-\n\x07MobyVel\x12\n\n\x02vx\x18\x01 \x01(\x01\x12\n\n\x02vy\x18\x02 \x01(\x01\x12\n\n\x02vw\x18\x03 \x01(\x01\"?\n\rSwerveDoubles\x12\n\n\x02\x66l\x18\x01 \x01(\x01\x12\n\n\x02\x66r\x18\x02 \x01(\x01\x12\n\n\x02\x62l\x18\x03 \x01(\x01\x12\n\n\x02\x62r\x18\x04 \x01(\x01\"/\n\tTargetVel\x12\n\n\x02vx\x18\x01 \x01(\x01\x12\n\n\x02vy\x18\x02 \x01(\x01\x12\n\n\x02vw\x18\x03 \x01(\x01\";\n\tZeroCount\x12\n\n\x02\x66l\x18\x01 \x01(\x05\x12\n\n\x02\x66r\x18\x02 \x01(\x05\x12\n\n\x02\x62l\x18\x03 \x01(\x05\x12\n\n\x02\x62r\x18\x04 \x01(\x05\"\xae\x01\n\x06IRData\x12\x11\n\tir_front1\x18\x01 \x01(\x05\x12\x11\n\tir_front2\x18\x02 \x01(\x05\x12\x10\n\x08ir_left1\x18\x03 \x01(\x05\x12\x10\n\x08ir_left2\x18\x04 \x01(\x05\x12\x10\n\x08ir_left3\x18\x05 \x01(\x05\x12\x0f\n\x07ir_rear\x18\x06 \x01(\x05\x12\x11\n\tir_right1\x18\x07 \x01(\x05\x12\x11\n\tir_right2\x18\x08 \x01(\x05\x12\x11\n\tir_right3\x18\t \x01(\x05\"t\n\x07\x42MSData\x12\x12\n\nbms_status\x18\x01 \x03(\x05\x12\x11\n\tpack_volt\x18\x02 \x03(\x05\x12\x14\n\x0c\x62\x61ttery_volt\x18\x03 \x03(\x05\x12\x15\n\rpack_current1\x18\x04 \x03(\x05\x12\x15\n\rpack_current2\x18\x05 \x03(\x05\"!\n\x05GBool\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0b\n\x03val\x18\x02 \x01(\x08\" \n\x04GInt\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0b\n\x03val\x18\x02 \x01(\x05\"\"\n\x06GFloat\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0b\n\x03val\x18\x02 \x01(\x02\"#\n\x07GString\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0b\n\x03val\x18\x02 \x01(\t\"\x16\n\x07\x42oolVal\x12\x0b\n\x03val\x18\x01 \x01(\x08\"\x15\n\x06IntVal\x12\x0b\n\x03val\x18\x01 \x01(\x05\"\x16\n\x07IntVals\x12\x0b\n\x03val\x18\x01 \x03(\x05\"\x17\n\x08\x46loatVal\x12\x0b\n\x03val\x18\x01 \x01(\x02\"\x18\n\tFloatVals\x12\x0b\n\x03val\x18\x01 \x03(\x02\"\x18\n\tDoubleVal\x12\x0b\n\x03val\x18\x01 \x01(\x01\"\x19\n\nDoubleVals\x12\x0b\n\x03val\x18\x01 \x03(\x01\">\n\x0cRotationGain\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\t\n\x01k\x18\x02 \x01(\x01\x12\n\n\x02kv\x18\x03 \x01(\x01\x12\n\n\x02kp\x18\x04 \x01(\x01\"9\n\x0eVelAccBoundary\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x0c\n\x04vmax\x18\x02 \x01(\x02\x12\x0c\n\x04\x61max\x18\x03 \x01(\x02\x32\xc7\x0f\n\x0cGRPCMobyTask\x12<\n\rGetMobyTxData\x12\x10.GRPCMoby.IntVal\x1a\x17.GRPCMoby.MotorDriverTx\"\x00\x12<\n\rGetMobyRxData\x12\x10.GRPCMoby.IntVal\x1a\x17.GRPCMoby.MotorDriverRx\"\x00\x12\x36\n\x0cGetMobyState\x12\x0f.GRPCMoby.Empty\x1a\x13.GRPCMoby.MobyState\"\x00\x12@\n\x11GetMobyErrorState\x12\x0f.GRPCMoby.Empty\x1a\x18.GRPCMoby.MobyErrorState\"\x00\x12-\n\x07Recover\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x34\n\x0bGetMobyPose\x12\x0f.GRPCMoby.Empty\x1a\x12.GRPCMoby.MobyPose\"\x00\x12\x32\n\nGetMobyVel\x12\x0f.GRPCMoby.Empty\x1a\x11.GRPCMoby.MobyVel\"\x00\x12\x33\n\rResetMobyPose\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x41\n\x13GetRotationAngleDeg\x12\x0f.GRPCMoby.Empty\x1a\x17.GRPCMoby.SwerveDoubles\"\x00\x12;\n\rGetDriveSpeed\x12\x0f.GRPCMoby.Empty\x1a\x17.GRPCMoby.SwerveDoubles\"\x00\x12\x36\n\x0cGetTargetVel\x12\x0f.GRPCMoby.Empty\x1a\x13.GRPCMoby.TargetVel\"\x00\x12>\n\x14GetRotationZeroCount\x12\x0f.GRPCMoby.Empty\x1a\x13.GRPCMoby.ZeroCount\"\x00\x12/\n\x08GetCMode\x12\x0f.GRPCMoby.Empty\x1a\x10.GRPCMoby.IntVal\"\x00\x12\x36\n\x0bGetGyroData\x12\x0f.GRPCMoby.Empty\x1a\x14.GRPCMoby.DoubleVals\"\x00\x12\x35\n\x0fResetGyroSensor\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x36\n\x0eUseGyroForOdom\x12\x11.GRPCMoby.BoolVal\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x37\n\x0fGetGyroFullData\x12\x0f.GRPCMoby.Empty\x1a\x11.GRPCMoby.IMUData\"\x00\x12\x36\n\x0fGetIRSensorData\x12\x0f.GRPCMoby.Empty\x1a\x10.GRPCMoby.IRData\"\x00\x12\x32\n\nGetBMSData\x12\x0f.GRPCMoby.Empty\x1a\x11.GRPCMoby.BMSData\"\x00\x12\x38\n\x0eSetStepControl\x12\x13.GRPCMoby.TargetVel\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x30\n\nStopMotion\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x41\n\x13SetRotationAngleDeg\x12\x17.GRPCMoby.SwerveDoubles\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x38\n\nDriveWheel\x12\x17.GRPCMoby.SwerveDoubles\x1a\x0f.GRPCMoby.Empty\"\x00\x12<\n\x16SetZeroPosAsCurrentPos\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12<\n\x11SetRotationVelAcc\x12\x14.GRPCMoby.DoubleVals\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x39\n\x0eSetDriveAccDec\x12\x14.GRPCMoby.DoubleVals\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x41\n\x19SetDriveInterpolatorOnOff\x12\x11.GRPCMoby.BoolVal\x1a\x0f.GRPCMoby.Empty\"\x00\x12G\n\x1cSetRotationInterpolatorParam\x12\x14.GRPCMoby.DoubleVals\x1a\x0f.GRPCMoby.Empty\"\x00\x12=\n\x15SetRotationTorqueMode\x12\x11.GRPCMoby.BoolVal\x1a\x0f.GRPCMoby.Empty\"\x00\x12<\n\x0fSetControlParam\x12\x16.GRPCMoby.RotationGain\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x34\n\x0eStartRTLogging\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x32\n\x0c\x45ndRTLogging\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x37\n\x0fSetLoggerBuffer\x12\x11.GRPCMoby.IntVals\x1a\x0f.GRPCMoby.Empty\"\x00\x12\x32\n\x0cRTLoggerSave\x12\x0f.GRPCMoby.Empty\x1a\x0f.GRPCMoby.Empty\"\x00\x62\x06proto3'
 )
 
 
 
 
 _EMPTY = _descriptor.Descriptor(
   name='Empty',
@@ -1573,15 +1573,15 @@
   name='GRPCMobyTask',
   full_name='GRPCMoby.GRPCMobyTask',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
   serialized_start=1891,
-  serialized_end=3954,
+  serialized_end=3882,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetMobyTxData',
     full_name='GRPCMoby.GRPCMobyTask.GetMobyTxData',
     index=0,
     containing_service=None,
     input_type=_INTVAL,
@@ -1596,337 +1596,327 @@
     containing_service=None,
     input_type=_INTVAL,
     output_type=_MOTORDRIVERRX,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
-    name='DirectMotorDriveControl',
-    full_name='GRPCMoby.GRPCMobyTask.DirectMotorDriveControl',
-    index=2,
-    containing_service=None,
-    input_type=_MOTORDRIVERRXS,
-    output_type=_EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
     name='GetMobyState',
     full_name='GRPCMoby.GRPCMobyTask.GetMobyState',
-    index=3,
+    index=2,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_MOBYSTATE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetMobyErrorState',
     full_name='GRPCMoby.GRPCMobyTask.GetMobyErrorState',
-    index=4,
+    index=3,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_MOBYERRORSTATE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='Recover',
     full_name='GRPCMoby.GRPCMobyTask.Recover',
-    index=5,
+    index=4,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetMobyPose',
     full_name='GRPCMoby.GRPCMobyTask.GetMobyPose',
-    index=6,
+    index=5,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_MOBYPOSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetMobyVel',
     full_name='GRPCMoby.GRPCMobyTask.GetMobyVel',
-    index=7,
+    index=6,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_MOBYVEL,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ResetMobyPose',
     full_name='GRPCMoby.GRPCMobyTask.ResetMobyPose',
-    index=8,
+    index=7,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetRotationAngleDeg',
     full_name='GRPCMoby.GRPCMobyTask.GetRotationAngleDeg',
-    index=9,
+    index=8,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_SWERVEDOUBLES,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetDriveSpeed',
     full_name='GRPCMoby.GRPCMobyTask.GetDriveSpeed',
-    index=10,
+    index=9,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_SWERVEDOUBLES,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetTargetVel',
     full_name='GRPCMoby.GRPCMobyTask.GetTargetVel',
-    index=11,
+    index=10,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_TARGETVEL,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetRotationZeroCount',
     full_name='GRPCMoby.GRPCMobyTask.GetRotationZeroCount',
-    index=12,
+    index=11,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_ZEROCOUNT,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetCMode',
     full_name='GRPCMoby.GRPCMobyTask.GetCMode',
-    index=13,
+    index=12,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_INTVAL,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetGyroData',
     full_name='GRPCMoby.GRPCMobyTask.GetGyroData',
-    index=14,
+    index=13,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_DOUBLEVALS,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ResetGyroSensor',
     full_name='GRPCMoby.GRPCMobyTask.ResetGyroSensor',
-    index=15,
+    index=14,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='UseGyroForOdom',
     full_name='GRPCMoby.GRPCMobyTask.UseGyroForOdom',
-    index=16,
+    index=15,
     containing_service=None,
     input_type=_BOOLVAL,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetGyroFullData',
     full_name='GRPCMoby.GRPCMobyTask.GetGyroFullData',
-    index=17,
+    index=16,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_IMUDATA,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetIRSensorData',
     full_name='GRPCMoby.GRPCMobyTask.GetIRSensorData',
-    index=18,
+    index=17,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_IRDATA,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetBMSData',
     full_name='GRPCMoby.GRPCMobyTask.GetBMSData',
-    index=19,
+    index=18,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_BMSDATA,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetStepControl',
     full_name='GRPCMoby.GRPCMobyTask.SetStepControl',
-    index=20,
+    index=19,
     containing_service=None,
     input_type=_TARGETVEL,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='StopMotion',
     full_name='GRPCMoby.GRPCMobyTask.StopMotion',
-    index=21,
+    index=20,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetRotationAngleDeg',
     full_name='GRPCMoby.GRPCMobyTask.SetRotationAngleDeg',
-    index=22,
+    index=21,
     containing_service=None,
     input_type=_SWERVEDOUBLES,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='DriveWheel',
     full_name='GRPCMoby.GRPCMobyTask.DriveWheel',
-    index=23,
+    index=22,
     containing_service=None,
     input_type=_SWERVEDOUBLES,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetZeroPosAsCurrentPos',
     full_name='GRPCMoby.GRPCMobyTask.SetZeroPosAsCurrentPos',
-    index=24,
+    index=23,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetRotationVelAcc',
     full_name='GRPCMoby.GRPCMobyTask.SetRotationVelAcc',
-    index=25,
+    index=24,
     containing_service=None,
     input_type=_DOUBLEVALS,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetDriveAccDec',
     full_name='GRPCMoby.GRPCMobyTask.SetDriveAccDec',
-    index=26,
+    index=25,
     containing_service=None,
     input_type=_DOUBLEVALS,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetDriveInterpolatorOnOff',
     full_name='GRPCMoby.GRPCMobyTask.SetDriveInterpolatorOnOff',
-    index=27,
+    index=26,
     containing_service=None,
     input_type=_BOOLVAL,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetRotationInterpolatorParam',
     full_name='GRPCMoby.GRPCMobyTask.SetRotationInterpolatorParam',
-    index=28,
+    index=27,
     containing_service=None,
     input_type=_DOUBLEVALS,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetRotationTorqueMode',
     full_name='GRPCMoby.GRPCMobyTask.SetRotationTorqueMode',
-    index=29,
+    index=28,
     containing_service=None,
     input_type=_BOOLVAL,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetControlParam',
     full_name='GRPCMoby.GRPCMobyTask.SetControlParam',
-    index=30,
+    index=29,
     containing_service=None,
     input_type=_ROTATIONGAIN,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='StartRTLogging',
     full_name='GRPCMoby.GRPCMobyTask.StartRTLogging',
-    index=31,
+    index=30,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='EndRTLogging',
     full_name='GRPCMoby.GRPCMobyTask.EndRTLogging',
-    index=32,
+    index=31,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='SetLoggerBuffer',
     full_name='GRPCMoby.GRPCMobyTask.SetLoggerBuffer',
-    index=33,
+    index=32,
     containing_service=None,
     input_type=_INTVALS,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='RTLoggerSave',
     full_name='GRPCMoby.GRPCMobyTask.RTLoggerSave',
-    index=34,
+    index=33,
     containing_service=None,
     input_type=_EMPTY,
     output_type=_EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
 ])
```

### Comparing `neuromeka-clients-0.1.2/neuromeka/proto/MobygRPCServer_pb2_grpc.py` & `neuromeka-clients-0.1.4/neuromeka/proto/MobygRPCServer_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,14 @@
                 response_deserializer=MobygRPCServer__pb2.MotorDriverTx.FromString,
                 )
         self.GetMobyRxData = channel.unary_unary(
                 '/GRPCMoby.GRPCMobyTask/GetMobyRxData',
                 request_serializer=MobygRPCServer__pb2.IntVal.SerializeToString,
                 response_deserializer=MobygRPCServer__pb2.MotorDriverRx.FromString,
                 )
-        self.DirectMotorDriveControl = channel.unary_unary(
-                '/GRPCMoby.GRPCMobyTask/DirectMotorDriveControl',
-                request_serializer=MobygRPCServer__pb2.MotorDriverRxs.SerializeToString,
-                response_deserializer=MobygRPCServer__pb2.Empty.FromString,
-                )
         self.GetMobyState = channel.unary_unary(
                 '/GRPCMoby.GRPCMobyTask/GetMobyState',
                 request_serializer=MobygRPCServer__pb2.Empty.SerializeToString,
                 response_deserializer=MobygRPCServer__pb2.MobyState.FromString,
                 )
         self.GetMobyErrorState = channel.unary_unary(
                 '/GRPCMoby.GRPCMobyTask/GetMobyErrorState',
@@ -203,20 +198,14 @@
 
     def GetMobyRxData(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DirectMotorDriveControl(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def GetMobyState(self, request, context):
         """Get Moby state
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -423,19 +412,14 @@
                     response_serializer=MobygRPCServer__pb2.MotorDriverTx.SerializeToString,
             ),
             'GetMobyRxData': grpc.unary_unary_rpc_method_handler(
                     servicer.GetMobyRxData,
                     request_deserializer=MobygRPCServer__pb2.IntVal.FromString,
                     response_serializer=MobygRPCServer__pb2.MotorDriverRx.SerializeToString,
             ),
-            'DirectMotorDriveControl': grpc.unary_unary_rpc_method_handler(
-                    servicer.DirectMotorDriveControl,
-                    request_deserializer=MobygRPCServer__pb2.MotorDriverRxs.FromString,
-                    response_serializer=MobygRPCServer__pb2.Empty.SerializeToString,
-            ),
             'GetMobyState': grpc.unary_unary_rpc_method_handler(
                     servicer.GetMobyState,
                     request_deserializer=MobygRPCServer__pb2.Empty.FromString,
                     response_serializer=MobygRPCServer__pb2.MobyState.SerializeToString,
             ),
             'GetMobyErrorState': grpc.unary_unary_rpc_method_handler(
                     servicer.GetMobyErrorState,
@@ -633,31 +617,14 @@
         return grpc.experimental.unary_unary(request, target, '/GRPCMoby.GRPCMobyTask/GetMobyRxData',
             MobygRPCServer__pb2.IntVal.SerializeToString,
             MobygRPCServer__pb2.MotorDriverRx.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DirectMotorDriveControl(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/GRPCMoby.GRPCMobyTask/DirectMotorDriveControl',
-            MobygRPCServer__pb2.MotorDriverRxs.SerializeToString,
-            MobygRPCServer__pb2.Empty.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetMobyState(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `neuromeka-clients-0.1.2/neuromeka/proto/MotorControlgRPCServer_pb2.py` & `neuromeka-clients-0.1.4/neuromeka/proto/MotorControlgRPCServer_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py` & `neuromeka-clients-0.1.4/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka/proto/grpc_wrapper.py` & `neuromeka-clients-0.1.4/neuromeka/proto/grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.2/neuromeka_clients.egg-info/PKG-INFO` & `neuromeka-clients-0.1.4/neuromeka_clients.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: neuromeka-clients
-Version: 0.1.2
-Summary: Neuromeka client protocols for Indy, Moby, Ecat, and Motor
+Version: 0.1.4
+Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients
-Author: Your Name
+Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Neuromeka Clients
 
 This package provides client protocols for users to interact with Neuromeka's products, including Indy, Moby, Ecat, and Motor.
 
 ## Installation
 
@@ -38,35 +37,37 @@
 * MobyClient in moby.py
 * EcatClient in ecat.py
 * MotorClient in motor.py
 
 To use a client class, simply import it and create an instance:
 
 ```python
-from neuromeka.ecat import EcatClient
+from neuromeka import EcatClient, MobyClient, IndyClient, MotorClient
 
-ecat_client = EcatClient("192.168.214.20")
+ecat = EcatClient("192.168.214.20")
+moby = IndyClient("192.168.214.20")
+indy = IndyClient("192.168.0.11")
+motor = MotorClient("192.168.0.20")
 ```
 
 Replace EcatClient with the desired client class and the IP address with the appropriate address for your device.
 
 ## Dependencies
 This package requires the following dependencies:
 
 * grpcio
 * grpcio-tools
 * protobuf
-* six
 
 These dependencies will be automatically installed when you install the package using pip.
 
 ## Examples
 Please refer to the 'example.py' file in the package for usage examples.
 
 ## Support
 If you encounter any issues or need help, please open an issue on the project's repository.
 
 ## License
-This package is released under the [LICENSE_NAME]. For more information, please refer to the LICENSE file.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `neuromeka-clients-0.1.2/neuromeka_clients.egg-info/SOURCES.txt` & `neuromeka-clients-0.1.4/neuromeka_clients.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+LICENSE
 README.md
 setup.py
 neuromeka/__init__.py
 neuromeka/ecat.py
+neuromeka/eye.py
 neuromeka/indy.py
 neuromeka/moby.py
 neuromeka/motor.py
+neuromeka/indy_dcp/__init__.py
+neuromeka/indy_dcp/indy_program_maker.py
+neuromeka/indy_dcp/indydcp_client.py
 neuromeka/proto/EtherCATCommgRPCServer_pb2.py
 neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py
+neuromeka/proto/EyeTask_pb2.py
+neuromeka/proto/EyeTask_pb2_grpc.py
 neuromeka/proto/IndygRPCTask_pb2.py
 neuromeka/proto/IndygRPCTask_pb2_grpc.py
 neuromeka/proto/MobygRPCServer_pb2.py
 neuromeka/proto/MobygRPCServer_pb2_grpc.py
 neuromeka/proto/MotorControlgRPCServer_pb2.py
 neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py
 neuromeka/proto/__init__.py
```

### Comparing `neuromeka-clients-0.1.2/setup.py` & `neuromeka-clients-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+
 setup(
     name="neuromeka-clients",
-    version="0.1.2",
-    author="Your Name",
+    version="0.1.4",
+    author="Neuromeka",
     author_email="youngjin.heo@neuromeka.com",
-    description="Neuromeka client protocols for Indy, Moby, Ecat, and Motor",
+    description="Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/neuromeka-robotics/neuromeka-clients",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.6",
     install_requires=[
         "grpcio==1.39.0",
         "grpcio-tools==1.39.0",
-        "protobuf==3.17.3"
+        "protobuf==3.17.3",
+        "requests",
+        "Pillow",
+        "numpy"
     ],
 )
```

