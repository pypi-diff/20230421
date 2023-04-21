# Comparing `tmp/dtwinpy-0.0.3.9-py3-none-any.whl.zip` & `tmp/dtwinpy-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 80045 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat    39744 b- defN 23-Mar-28 00:46 dtwinpy/Digital_Twin.py
+Zip file size: 93810 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat    40171 b- defN 23-Apr-21 09:41 dtwinpy/Digital_Twin.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 19:45 dtwinpy/__init__.py
--rw-rw-rw-  2.0 fat    23151 b- defN 23-Mar-27 13:21 dtwinpy/broker_manager.py
--rw-rw-rw-  2.0 fat    54424 b- defN 23-Mar-27 22:37 dtwinpy/components.py
--rw-rw-rw-  2.0 fat    46557 b- defN 23-Mar-27 16:27 dtwinpy/digital_model.py
--rw-rw-rw-  2.0 fat     8049 b- defN 23-Mar-27 13:16 dtwinpy/helper.py
--rw-rw-rw-  2.0 fat    11063 b- defN 23-Mar-23 15:10 dtwinpy/interfaceAPI.py
--rw-rw-rw-  2.0 fat    47352 b- defN 23-Mar-27 22:16 dtwinpy/interfaceDB.py
--rw-rw-rw-  2.0 fat    36842 b- defN 23-Mar-27 13:28 dtwinpy/services.py
--rw-rw-rw-  2.0 fat    33354 b- defN 23-Mar-23 23:30 dtwinpy/synchronizer.py
--rw-rw-rw-  2.0 fat    22342 b- defN 23-Mar-27 22:41 dtwinpy/tester.py
--rw-rw-rw-  2.0 fat    13021 b- defN 23-Mar-27 17:01 dtwinpy/updator.py
--rw-rw-rw-  2.0 fat    35858 b- defN 23-Mar-28 00:21 dtwinpy/validator.py
--rw-rw-rw-  2.0 fat      140 b- defN 23-Mar-28 00:46 dtwinpy-0.0.3.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-28 00:46 dtwinpy-0.0.3.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-28 00:46 dtwinpy-0.0.3.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1324 b- defN 23-Mar-28 00:46 dtwinpy-0.0.3.9.dist-info/RECORD
-17 files, 373321 bytes uncompressed, 77917 bytes compressed:  79.1%
+-rw-rw-rw-  2.0 fat    23407 b- defN 23-Apr-21 09:41 dtwinpy/broker_manager.py
+-rw-rw-rw-  2.0 fat    54494 b- defN 23-Apr-21 09:41 dtwinpy/components.py
+-rw-rw-rw-  2.0 fat    48951 b- defN 23-Apr-21 09:41 dtwinpy/digital_model.py
+-rw-rw-rw-  2.0 fat     9075 b- defN 23-Apr-21 09:41 dtwinpy/helper.py
+-rw-rw-rw-  2.0 fat    11063 b- defN 23-Apr-21 09:41 dtwinpy/interfaceAPI.py
+-rw-rw-rw-  2.0 fat    58461 b- defN 23-Apr-21 09:41 dtwinpy/interfaceDB.py
+-rw-rw-rw-  2.0 fat    39752 b- defN 23-Apr-21 09:41 dtwinpy/services.py
+-rw-rw-rw-  2.0 fat    35637 b- defN 23-Apr-21 09:41 dtwinpy/synchronizer.py
+-rw-rw-rw-  2.0 fat    68985 b- defN 23-Apr-21 09:41 dtwinpy/tester.py
+-rw-rw-rw-  2.0 fat    14051 b- defN 23-Apr-21 09:41 dtwinpy/updator.py
+-rw-rw-rw-  2.0 fat    38152 b- defN 23-Apr-21 09:41 dtwinpy/validator.py
+-rw-rw-rw-  2.0 fat      132 b- defN 23-Apr-21 09:45 dtwinpy-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 09:45 dtwinpy-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-21 09:45 dtwinpy-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1316 b- defN 23-Apr-21 09:45 dtwinpy-0.1.0.dist-info/RECORD
+17 files, 443747 bytes uncompressed, 91698 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: dtwinpy/updator.py
 Comment: 
 
 Filename: dtwinpy/validator.py
 Comment: 
 
-Filename: dtwinpy-0.0.3.9.dist-info/METADATA
+Filename: dtwinpy-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: dtwinpy-0.0.3.9.dist-info/WHEEL
+Filename: dtwinpy-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: dtwinpy-0.0.3.9.dist-info/top_level.txt
+Filename: dtwinpy-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dtwinpy-0.0.3.9.dist-info/RECORD
+Filename: dtwinpy-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dtwinpy/Digital_Twin.py

```diff
@@ -41,15 +41,15 @@
 importlib.reload(dtwinpylib.dtwinpy.interfaceDB)
 importlib.reload(dtwinpylib.dtwinpy.helper)
 importlib.reload(dtwinpylib.dtwinpy.services)"""
 
 
 
 class Digital_Twin():
-    def __init__(self, name, copied_realDB= False,model_path= None, ip_address= None, initial= True, targeted_part_id= None, targeted_cluster= None, until= None, digital_database_path= None, real_database_path= None, ID_database_path= None, experimental_database_path= None, Freq_Sync= 1000, Freq_Valid= 10000, delta_t_treshold= 100, logic_threshold= 0.75, input_threshold= 0.75, rct_threshold= 0.02, queue_position= 2, Freq_Service = None, part_type= "A", loop_type= "closed", maxparts = None, template= False, keepDB= True, plot= False, verbose= True, flag_API= False, flag_external_service= False, flag_publish= True, rct_queue= 3):
+    def __init__(self, name, copied_realDB= False,model_path= None, ip_address= None, initial= True, targeted_part_id= None, targeted_cluster= None, palletID_tracked= 'Pallet 1', until= None, digital_database_path= None, real_database_path= None, ID_database_path= None, experimental_database_path= None, Freq_Sync= 1000, Freq_Valid= 10000, delta_t_treshold= 100, logic_threshold= 0.75, input_threshold= 0.75, rct_threshold= 0.02, queue_position= 2, Freq_Service = None, part_type= "A", loop_type= "closed", maxparts = None, template= False, keepDB= True, keepModels= False, plot= False, verbose= True, flag_API= False, flag_external_service= False, flag_publish= True, flag_validation= False, rct_queue= 3):
         self.helper = Helper()
         #--- Model Parameters
         self.name = name
         self.part_type = "A"
         self.loop_type = "closed"
         self.digital_model = None
         self.initial = initial
@@ -69,27 +69,29 @@
         
     
         #--- Simulation stop conditions
         self.until = until
         self.maxparts = maxparts
         self.targeted_part_id = targeted_part_id
         self.targeted_cluster = targeted_cluster
+        self.palletID_tracked = palletID_tracked
 
         #--- Frequencies
         self.Freq_Sync = Freq_Sync
         self.Freq_Valid = Freq_Valid
         self.Freq_Service = self.Freq_Sync
 
         #--- Flag of Features
         self.flag_API = flag_API
         if flag_API: 
             self.interfaceAPI = interfaceAPI()
             print("Interface API created....")
         self.flag_external_service = flag_external_service
         self.flag_publish = flag_publish
+        self.flag_validation = flag_validation
 
         #--- Time intervals
         (initial_time_str, initial_timestamp) = self.helper.get_time_now()
         self.current_timestamp = initial_timestamp
         
 
         self.next_Tsync = initial_timestamp + self.Freq_Sync + 5
@@ -126,16 +128,16 @@
             pointer2: 'timestamp2_pointer2',
             pointer3: 'timestamp3_pointer3'.
         }
         """
 
     
         #--- Figure path
-        if not os.path.exists(f"figures"):
-            os.makedirs(f"figures/")
+        if not os.path.exists(f"figures/{self.name}"):
+            os.makedirs(f"figures/{self.name}")
 
         #------ Model JSON ------
 
         #-- Models root
         self.model_root = f"models/{self.name}"
 
         if model_path == None:
@@ -146,15 +148,16 @@
             #-- First model name
             first_model = "initial.json"
 
             #-- Model Path default
             self.model_path = f"{self.model_root}/{first_model}"
 
             #-- Clean existing model files
-            self.helper.delete_old_model(self.model_root, first_model)
+            if keepModels == False:
+                self.helper.delete_old_model(self.model_root, first_model)
         else:
             self.model_path = model_path
 
         #-- delete the current model and copy the template
         """
         if template == True:
             #- Delete old model
@@ -342,15 +345,15 @@
         #--- Verbose if necessary
         if verbose == True:
             self.digital_model.verbose()
 
         return self.digital_model
     
     #--- Run normally the Digital Model and analyze the results
-    def run_digital_model(self, plot= True, maxparts = None, until = None, targeted_part_id = None, targeted_cluster= None, verbose= True, generate_model = True):
+    def run_digital_model(self, plot= False, maxparts = None, until = None, targeted_part_id = None, targeted_cluster= None, verbose= True, generate_model = True):
         if generate_model == True:
             if maxparts == None:
                 maxparts = self.maxparts
 
             #--- If the target conditions doesn't exist, assign it
             if targeted_part_id == None:
                 targeted_part_id = self.targeted_part_id
@@ -484,25 +487,28 @@
 
         #--- Run the synchronizer (positioning)
         (machine_status, queue_status)= synchronizer.run(repositioning= repositioning)
 
         return (machine_status, queue_status)
 
     #--- Run RCT Services
-    def run_RCT_services(self, verbose= True, plot= False, queue_position= 3, rct_threshold= 0):
+    def run_RCT_services(self, verbose= True, plot= False, queue_position= 3, rct_threshold= 0, palletID_tracked= 'Pallet 1'):
         """
         This functions creates Service object that is responsible for finding parts making decisions in the simulation,
         generate all possible paths, and calculate the most optimized path for those parts.
         """
         #--- Create a Service 
         RCT_Service = Service_Handler(name= "RCT", generate_digital_model= self.generate_digital_model, broker_manager= self.broker_manager, rct_threshold= rct_threshold, flag_publish= self.flag_publish)
         
         #--- Run the RCT Service
         rct_results= RCT_Service.run_RCT_service(verbose=verbose, plot= plot, queue_position= queue_position)
 
+        #--- RCT tracking
+        RCT_Service.run_RCT_tracking(palletID= palletID_tracked)
+
         return rct_results
     # ------------------------------------------------------------------------------------------------------------------------------------------------------
 
     # -------------------------------------------------- INTERNAL & EXTERNAL SERVICES --------------------------------------------------
 
     #--- Internal Services (Synchronization and Validation)    
     def Internal_Services(self):
@@ -572,15 +578,15 @@
 
             # --- User Interface
             (current_time_str, x) = self.helper.get_time_now()
             nexttime = datetime.datetime.fromtimestamp(self.next_Tsync).strftime("%d %B %H:%M:%S")
             self.helper.printer(f"[Internal Service] System Synchronized. Next Sync (n° {self.counter_Sync}): {nexttime}", 'blue')
         
         # ====================== Running Validation ======================
-        if  self.flag_time_to_validate:
+        if  self.flag_time_to_validate and self.flag_validation:
             # --------------------- BEFORE SERVICES SETTINGS ---------------------
             # --- User Interface
             (current_time_str, x) = self.helper.get_time_now()
             self.helper.printer(f"[Internal Service] Starting Validation (n° {self.counter_Valid})", 'green')
 
             # --- Update Start and End time
             start_time = round(self.last_Tvalid)
@@ -710,15 +716,15 @@
             subpath = self.model_subpath_dict[self.model_pointer_Serv]
 
             # --- Update the model path for Service
             self.model_path = f"{self.model_root}/{subpath}.json"
             print(f"--- Model Path being used: {self.model_path}")
 
             # -------------------- Run Service ---------------------------------
-            rct_results= self.run_RCT_services(verbose= self.verbose, plot= self.plot, queue_position= self.rct_queue, rct_threshold= self.rct_threshold)
+            rct_results= self.run_RCT_services(verbose= self.verbose, plot= self.plot, queue_position= self.rct_queue, rct_threshold= self.rct_threshold, palletID_tracked= self.palletID_tracked)
             # ------------------------------------------------------------------
 
             # ------------------------ API INTERFACE ------------------------
             #--- Check if there is a path taking a decision
             if rct_results != False:
                 #--- Assign the results
                 (part_id, path_1, path_2, queue_id, feedback_flag, gain) = (rct_results[0], rct_results[1], rct_results[2], rct_results[3], rct_results[4], rct_results[5])
```

## dtwinpy/broker_manager.py

```diff
@@ -154,16 +154,14 @@
 
         #--- Add the UID with the current PID counter in the dictionary
         self.UID_to_PID_dict[unique_ID] = part_id
 
         #----- Clean the selected Branch Queue for this UID that now has a new PID
         self.ID_database.write_selected_branch_queue(UID= unique_ID, selected_queue= None)
 
-
-
     def part_ID_translator(self, unique_ID):
         """
         This function takes a UID and searches in the PID dictionary for the related PID. The function returns
         this PID. This is used for all the machines.
         """
 
         #--- Searches in the dictionary for the related PID to the UID and return it
@@ -221,16 +219,14 @@
             #--- When a machine sends Started, it didn't have the time yet to read the RFID, so it assigns Part 0
             # this id is going to be replaced by the topic 'part_id'
             part_id = "Part 0"
 
         #--- Write the information into the real database
         self.real_database.write_event('real_log', 0, machine_id, status, part_id, queue_id, current_time_str, current_timestamp)
 
-
-
     def part_id_handler(self, message_translated):
         """
         This functions is used when a MQTT message of the topic 'part_id' is received by the broker.
         When the broker receive this message, it means that a new part arrive in one of the machines
         and at this point the machine already had sent the message to the broker with "Started", but in
         the database we have the part id for that event as 0. So the mission here is to take the id 
         received and update for the right machine (given by the reader as well) in the Started event.
@@ -292,16 +288,15 @@
             line_id = line_id_ltuple[-1][0] # Take the most recent 
 
             #--- UPDATE the part id started for the specific machine into the Real Database
             self.real_database.update_column(
                 table= "real_log",
                 column= "part_id",
                 line_id= line_id,
-                new_value= part_id,
-                current_time_str_= current_time_str
+                new_value= part_id
             )
 
         except IndexError:
             self.helper.printer(f"[WARNING][BROKER]: Your Broker Manager didn't find {machine_id} with 'Part 0' in the database ({self.real_database_path}). Please, check if the previous attempt was successful.", 'yellow')
         
     def rct_handler(self, message_translated):
         """
@@ -533,8 +528,13 @@
                 topic = 'system_status', 
                 payload= action
             )
             
             except ConnectionRefusedError:
                 self.helper.printer(f"[ERROR][broker_manager.py/publish_setting_action()] Mosquitto / Broker is not running in the IP address '{self.ip_address}'", 'red')
                 self.helper.printer(f"---- Digital Twin was killed ----", 'red')
+                sys.exit()
+
+            except TimeoutError:
+                self.helper.printer(f"[ERROR][broker_manager.py/publish_setting_action()] Mosquitto / Broker is not running in the IP address '{self.ip_address}'", 'red')
+                self.helper.printer(f"---- Digital Twin was killed ----", 'red')
                 sys.exit()
```

## dtwinpy/components.py

```diff
@@ -262,14 +262,16 @@
                         try_to_get = self.queue_to_get.get() 
                         self.part_in_machine = try_to_get.value
 
                 #-- There is an initial part being processed, I don't need to take from the queue
                 if self.worked_time != 0:
                     #-- machine has an initial part to be processed
                     self.part_in_machine = self.initial_part
+                    # [NEW]
+                    self.simtype = None
 
 
                 #-- Lower the flag that we finish the process
                 flag_process_finished = False
                 self.working = True
                 self.part_started_time = self.env.now
```

## dtwinpy/digital_model.py

```diff
@@ -970,14 +970,42 @@
     def get_all_parts(self):
         self.parts_vector = []
         for queue in self.queues_vector:
             parts_in_queue = queue.get_all_items()
             for part in parts_in_queue:
                 self.parts_vector.append(part)
         return self.parts_vector
+    def get_working_parts(self):
+        working_parts_vec = []
+        for machine in self.machines_vector:
+            initial_part = machine.get_initial_part()
+            if initial_part != None: working_parts_vec.append(initial_part)
+        
+        return working_parts_vec
+    def check_partID_in_simulation(self, part_id):
+        #--- Separate vector of parts
+        working_parts_vec = self.get_working_parts()
+        queue_parts_vec = self.get_all_parts()
+        #--- Merge parts 
+        all_parts = []
+        for part in working_parts_vec:
+            all_parts.append(part)
+        for part in queue_parts_vec:
+            all_parts.append(part)
+        
+        #--- Check if the selected part in within the all parts:
+        flag_found = False
+        for part in all_parts:
+            if part_id == part.get_name():
+                flag_found = True
+        
+        return flag_found
+
+
+
     def get_model_constrains(self):
         return (self.until, self.maxparts, self.targeted_part_id, self.targeted_cluster)
     def get_database_path(self):
         return self.database_path
     def get_selected_machine(self, machine_name= None, machine_id= None):
         """
         This function receives a machine name or a machine id and looks through all the 
@@ -988,15 +1016,52 @@
                 if machine.get_name() == machine_name:
                     return machine
 
         if machine_id != None:
             for machine in self.machines_vector:
                 if machine.get_id() == machine_id:
                     return machine
+    def get_terminated_parts(self):
+        return self.terminator.get_all_items()
+    def get_parts_CT_ordered(self):
+        #--- Get the finished Parts and each Time
+        parts_finished = self.terminator.get_all_items()
+
+        #--- Number of finished parts in the simulation
+        number_parts = len(parts_finished)
+
+        #--- create empty lists
+        parts_finished_time = []
+        parts_finished_id = []
+        parts_finished_id_ASIS = []
+        parts_creation_time = []
+
+        #---Create the list with parts ID
+        for part in parts_finished:
+            parts_finished_id.append(part.get_id())
+            parts_finished_id_ASIS.append(part.get_id())
+        
+        #--- Sort the list in ascending
+        parts_finished_id.sort()
 
+        #--- Adjust the sort of other variables following the ID sort
+        for id in parts_finished_id:
+            for part in parts_finished:
+                if part.get_id() == id:
+                    parts_finished_time.append(part.get_termination())
+                    parts_creation_time.append(part.get_creation())
+                    break
+        
+        #--- Calculate parts cycle time
+        parts_cycle_time = []
+        for i in range(number_parts):
+            #-- calculate individual CT
+            parts_cycle_time.append(parts_finished_time[i] - parts_creation_time[i])
+        
+        return (parts_finished_id,parts_cycle_time)
     # ==============================================
 
     # ================= SETs =================
     def set_targeted_part_id(self, value):
         self.targeted_part_id = value
     def set_targeted_cluster(self, value):
         self.targeted_cluster= value
```

## dtwinpy/helper.py

```diff
@@ -5,14 +5,15 @@
 #--- Common Libraries
 import datetime
 from time import sleep
 import shutil
 import os
 import re
 import sys
+import json
 
 
 
 
 class Helper():
     def __init__(self, type= "py"):
         self.type = type
@@ -166,29 +167,60 @@
         except FileNotFoundError:
             self.printer(f"[WARNING][helper.py/delete_databases()] The ID Database doesn't exist yet in the path '{ID_database_path}', proceding without deleting...")
         except PermissionError:
             self.printer(f"[ERROR][helper.py/delete_databases()] The ID Database is busy somewhere, please close and try again.", 'red')
             self.printer(f"---- Digital Twin was killed at {tstr} ----", 'red')
             sys.exit()
 
-        #- Delete ID database
+        #- Delete Experimental database
+        """
         try:
             os.remove(exp_database_path)
-            print(f"|-- ID Database deleted successfuly from {exp_database_path}")
+            print(f"|-- Experimental Database deleted successfuly from {exp_database_path}")
         except FileNotFoundError:
-            self.printer(f"[WARNING][helper.py/delete_databases()] The ID Database doesn't exist yet in the path '{exp_database_path}', proceding without deleting...")
+            self.printer(f"[WARNING][helper.py/delete_databases()] The Experimental Database doesn't exist yet in the path '{exp_database_path}', proceding without deleting...")
         except PermissionError:
-            self.printer(f"[ERROR][helper.py/delete_databases()] The ID Database is busy somewhere, please close and try again.", 'red')
+            self.printer(f"[ERROR][helper.py/delete_databases()] The Experimental Database is busy somewhere, please close and try again.", 'red')
             self.printer(f"---- Digital Twin was killed at {tstr} ----", 'red')
             sys.exit()
+        """
+
 
     #--- Delete models (except by one specific file)
     def delete_old_model(self, folder_path, file_to_save):
         print(f"Deleting existing model (excepted by '{file_to_save}') from the relative folder path:'{folder_path}'")
         model_counter = 0
         for file_name in os.listdir(folder_path):
             file_path = os.path.join(folder_path, file_name)
             if file_name != file_to_save:
                 os.remove(file_path)
                 print(f"File '{file_name}' deleted...")
                 model_counter += 1
-        print(f"Done! Deleted {model_counter} successfuly")
+        print(f"Done! Deleted {model_counter} successfuly")
+
+    def delete_figures(self, folder_path):
+        print(f"Deleting existing figures from the relative folder path:'{folder_path}'")
+        
+        for file_name in os.listdir(folder_path):
+            file_path = os.path.join(folder_path, file_name)
+            os.remove(file_path)
+            print(f"File '{file_name}' deleted...")
+
+        print(f"Done! Deleted Figures successfuly")
+
+
+
+    def convert_stringVect_to_listVect(self, stringVect):
+        return json.loads(stringVect)
+    
+    def convert_tuple_vector_to_list(self, tuple_vector):
+        for i in range(len(tuple_vector)):
+            tuple_vector[i] = tuple_vector[i][0]
+        return tuple_vector
+    
+    def adjust_relative_vector(self, vector):
+        first_value = vector[0]
+        for i in range(len(vector)):
+            relative_value = vector[i] - first_value
+            vector[i] = relative_value
+        
+        return vector
```

## dtwinpy/interfaceDB.py

```diff
@@ -110,14 +110,17 @@
             """
             # --- Create table for validation indicators
             self.create_valid_indicator_table()
 
             # --- Create table for RCT path
             self.create_RCTpaths_table()
 
+            # --- Create table for RCT tracking
+            self.create_RCTtracking_table()
+
             
 
         if event_table == "digital_log":
             with sqlite3.connect(self.database_path) as digital_model_DB:
                 digital_model_DB.execute(f"""
                 CREATE TABLE IF NOT EXISTS {self.event_table} (
                     event_id INTEGER PRIMARY KEY,
@@ -172,15 +175,14 @@
                     timestamp_real INTEGER
                 )
                 """)
 
                 db.commit()
     
     def create_valid_indicator_table(self):
-        # TODO: Finish up
         with sqlite3.connect(self.database_path) as db:
                 # --- Create table of validator indicators
                 db.execute("""
                 CREATE TABLE IF NOT EXISTS valid_indicators(
                     line_id INTEGER PRIMARY KEY,
                     current_time_str TEXT,
                     timestamp_real INTEGER,
@@ -206,15 +208,28 @@
                 queue_selected TEXT,
                 gain INTEGER,
                 partid TEXT
             )
             
             """)
 
-
+    def create_RCTtracking_table(self):
+        with sqlite3.connect(self.database_path) as db:
+            db.execute(
+                """
+                CREATE TABLE IF NOT EXISTS RCTtracking (
+                line_id INTEGER PRIMARY KEY,
+                current_time_str TEXT,
+                timestamp_real INTEGER,
+                PID TEXT,
+                RCT INTEGER,
+                palletID TEXT
+                )
+                """
+            )
 
     # -------- Setting Functions --------
     def rename_digital_to_real(self):
         with sqlite3.connect(self.database_path) as db:
                 tables = db.execute("SELECT name FROM sqlite_master WHERE type='table';").fetchall()
                 if len(tables) == 1 and tables[0][0] == "digital_log":
                     self.rename_table("digital_log", "real_log")
@@ -744,17 +759,17 @@
                 #return DB.execute(f"SELECT event_id FROM {table} WHERE {column1}=? AND {column2}= ? AND timestamp_real >= ? AND timestamp_real <= ?", (condition1, condition2, self.start_time, self.end_time)).fetchall()
                 return DB.execute(f"SELECT event_id FROM {table} WHERE {column1}=? AND {column2}= ? AND event_id >= ? AND event_id <= ?", (condition1, condition2, self.start_time_id, self.end_time_id)).fetchall()
 
             else:
                 return DB.execute(f"SELECT event_id FROM {table} WHERE {column1}=? AND {column2}= ? ", (condition1, condition2)).fetchall()
 
 
-    def update_column(self, table, column, line_id, new_value, current_time_str_):
+    def update_column(self, table, column, line_id, new_value):
         with sqlite3.connect(self.database_path) as DB:
-            DB.execute(f"UPDATE {table} SET {column} = ?, current_time_str= ? WHERE event_id = ?", (new_value, current_time_str_, line_id))
+            DB.execute(f"UPDATE {table} SET {column} = ? WHERE event_id = ?", (new_value, line_id))
             DB.commit()
 
     # ============================ ID DATABASE ============================
     # --------- Function to add a UID and partid to the table ---------
     def add_UID_partid(self, table_name, uid, partid, current_time_str, palletID):
         with sqlite3.connect(self.database_path) as DB:
             # Check if UID already exists in table
@@ -774,15 +789,21 @@
             if result is None:
                 #--- [ERROR] Part ID not stored in dictionary
                 self.helper.printer(f"[ERROR][interfaceDB.py/get_PID()] The part id '{partid}' was not found in the database: '{self.database_path}'", 'red')
                 print("Sending a generic UID: {x}")
                 return "x"
             else:
                 return result[0]
-            
+
+    # --------- Get a PID for a given PalletID ---------
+    def get_PID_from_PalletID(self, palletID):
+        with sqlite3.connect(self.database_path) as db:
+            PID = db.execute("SELECT PID from ID WHERE palletID= ?", (palletID,)).fetchone()[0]
+            return PID
+
     # --------- Database Replicator Function ---------
     def replicate_database(self):
         
         # --- Copy targeted database
         #shutil.copy2(self.database_path, self.replicated_database_path)
 
         # --- clear the table of the old database
@@ -978,8 +999,247 @@
         #-- Write into the database
         with sqlite3.connect(self.database_path) as db:
             db.execute("""
                 INSERT INTO valid_indicators (current_time_str, timestamp_real, logic_indicator, input_indicator, model_in, model_out)
                 VALUES (?,?,?,?,?,?)
             """, (tstr, t, logic_indicator, input_indicator, model_in, model_out))
 
-            db.commit()
+            db.commit()
+
+    # --------- Read valid indicators ---------
+    def read_ValidIndicator(self, indicator_name):
+        with sqlite3.connect(self.database_path) as db:
+            indicator = db.execute(
+                f"""
+                SELECT {indicator_name} FROM valid_indicators
+                """
+            ).fetchall()
+
+            # --- Fix tuple
+            for i in range(len(indicator)): indicator[i] = indicator[i][0] 
+
+            timestamp = db.execute(
+                """
+                SELECT timestamp_real FROM valid_indicators
+                """
+            ).fetchall()
+
+            # --- Fix tuple
+            for i in range(len(timestamp)): timestamp[i] = timestamp[i][0] 
+
+            return (indicator, timestamp)
+    
+    # --------- Read RCT Paths ---------
+    def read_RCT_path(self):
+        with sqlite3.connect(self.database_path) as db:
+            # --- Get timestamp
+            timestamp = db.execute("""SELECT timestamp_real FROM RCTpaths""").fetchall()
+            # --- Fix tuple
+            for i in range(len(timestamp)): timestamp[i] = timestamp[i][0] 
+
+            # --- Get rct from path 1
+            rct_path1 = db.execute("""SELECT RCT_path1 FROM RCTpaths""").fetchall()
+            # --- Fix tuple
+            for i in range(len(rct_path1)): rct_path1[i] = rct_path1[i][0] 
+
+            # --- Get rct from path 2
+            rct_path2 = db.execute("""SELECT RCT_path2 FROM RCTpaths""").fetchall()
+            # --- Fix tuple
+            for i in range(len(rct_path2)): rct_path2[i] = rct_path2[i][0] 
+
+            return (rct_path1, rct_path2, timestamp)
+    
+    # --------- Read Queue Occupation ---------
+    def read_queue_occupation(self, queue_id):
+        """ Read the evolution of queue occupation for a given queue"""
+        #--- Create the occupation vector to store the queue length after every Sync
+        occupation_vector = []
+
+        with sqlite3.connect(self.database_path) as db:
+            #--- Create the table name
+            table = f'queue_{queue_id}'
+
+            #--- Extract all the strings ("lists")
+            list_parts = db.execute(
+                f"""
+                SELECT n_parts FROM {table}
+                """
+            ).fetchall()
+
+            # --- Fix tuple
+            for i in range(len(list_parts)): list_parts[i] = list_parts[i][0] 
+
+            #--- Loop to extracted results to convert into a list and count the length
+            
+            # -------- Add the last element first ('initial') --------
+            str_list= list_parts[-1]
+            #--- convert in list
+            created_list = eval(str_list)
+            occupation_vector.append(len(created_list))
+            # ---------------------------------------------------------
+
+            for i in range(len(list_parts) -1):
+                #--- Take the string (list)
+                str_list= list_parts[i]
+
+                #--- convert in list
+                created_list = eval(str_list)
+
+                #--- Length
+                occupation_vector.append(len(created_list))
+        
+        #--- Return the occupation vector
+        return occupation_vector
+
+    # --------- Get specific value from one column of the Result table ---------
+    def get_global_result(self, result):
+        """ Get a specific result from a column from the result table"""
+        with sqlite3.connect(self.database_path) as db:
+            result = db.execute(
+                f"""
+                SELECT {result} from results
+                """
+            ).fetchone()
+        
+        return result[0]
+
+    def get_real_RCT(self, real_database_path):
+        """ Calculates the RCT of the parts from the real log when they are in the branch machine (Machine 2)"""
+        #--- Take the name and time of the parts that finish the simulation
+        with sqlite3.connect(real_database_path) as db:
+            #-- Get name of parts finished by Machine 5
+            parts_name_finished_vec = db.execute("SELECT part_id FROM real_log WHERE machine_id= ? and activity_type= ?", ('Machine 5', 'Finished')).fetchall()
+            parts_time_finished_vec = db.execute("SELECT timestamp_real FROM real_log WHERE machine_id= ? and activity_type= ?", ('Machine 5', 'Finished')).fetchall()
+            #-- convert tuple
+            parts_name_finished_vec = self.helper.convert_tuple_vector_to_list(parts_name_finished_vec)
+            parts_time_finished_vec = self.helper.convert_tuple_vector_to_list(parts_time_finished_vec)
+
+
+        #--- Take the finish time in machine 1 (branch machine) only for the parts that exits the system
+        # NOTE: We know that the DT is calculating the RCT based on the first position of the queue and
+        # here we're taking when the machine starts, but this is okay. The maximun error will be the process
+        # time of the first machine... 
+        with sqlite3.connect(real_database_path) as db:
+            parts_time_start_vec = []
+            for part_name in parts_name_finished_vec:
+                #--- Get start time 
+                parts_time_start = db.execute("SELECT timestamp_real FROM real_log WHERE machine_id= ? and activity_type= ? and part_id= ?", ('Machine 2', 'Started', part_name)).fetchall()
+                parts_time_start_vec.append(parts_time_start[0][0])
+
+        #--- Calculate the RCT based on the finish and start time
+        RCT_real = []
+        for i in range(len(parts_name_finished_vec)):
+            #--- Parameters
+            part_name = parts_name_finished_vec[i]
+            start_time = parts_time_start_vec[i]
+            finish_time = parts_time_finished_vec[i]
+
+            #--- RCT
+            RCT = finish_time - start_time
+            RCT_real.append(RCT)
+
+        #--- Takes the RCT predicted by the Digital Twin for each part finished in the system
+        RCT_path1_vec = []
+        RCT_path2_vec = []
+
+        for part_name in parts_name_finished_vec:
+            with sqlite3.connect(self.database_path) as db:
+                RCT_raw = db.execute("SELECT RCT_path1, RCT_path2 FROM RCTpaths WHERE partid = ?", (part_name,)).fetchall()
+
+                #--- take the most recent in case of recalculation
+                RCT_raw = RCT_raw[-1]
+
+                #--- Takes for each path
+                rct_path1 = RCT_raw[0]
+                rct_path2 = RCT_raw[1]
+
+                #--- Add into the vector
+                RCT_path1_vec.append(rct_path1)
+                RCT_path2_vec.append(rct_path2)
+        
+        return (parts_name_finished_vec, RCT_real, RCT_path1_vec, RCT_path2_vec)
+
+    # --------- Write the RCT tracking ---------
+    def write_RCTtracking(self, PID, RCT, palletID):
+        with sqlite3.connect(self.database_path) as db:
+            #-- Get time
+            (tstr, t)= self.helper.get_time_now()
+
+            #-- Write into the database
+            db.execute(
+                """
+                INSERT INTO RCTtracking (current_time_str, timestamp_real, PID, RCT, palletID)
+                VALUES (?, ?, ?, ?, ?)
+                """, (tstr, t, PID, RCT, palletID)
+            )
+
+            db.commit()
+
+    def get_real_RCTtracking(self, real_database_path, PID):
+        """
+        This function receives a PID and look through the real database to calculate
+        for every event that happen what was the RCT in the perspective of that event.
+        """
+        flag_part_completed = False
+        with sqlite3.connect(real_database_path) as db:
+            #-- Time in which the PID was finished
+            finished_time = db.execute("SELECT timestamp_real FROM real_log WHERE part_id= ? and machine_id= ? and activity_type= ?", (PID, 'Machine 5', 'Finished')).fetchone()
+            
+            # ----------- CHECK IF THE PART WAS FINISHED -----------
+            if finished_time == None:
+                flag_part_completed = False
+                return ([], [], flag_part_completed)
+            
+            if finished_time != None:
+                flag_part_completed = True
+                finished_time = finished_time[0]
+            # -------------------------------------------------------
+
+            #--- First time (considering waiting time in the first queue)
+            start_time_initial = db.execute("SELECT timestamp_real FROM real_log WHERE event_id= ?", (1,)).fetchone()[0]
+            
+
+            #-- Get all the timestamp where the PID appeared
+            start_time_rest = db.execute("SELECT timestamp_real FROM real_log WHERE part_id= ?", (PID,)).fetchall()
+            #-- convert tuples
+            start_time_rest = self.helper.convert_tuple_vector_to_list(start_time_rest)
+
+            #--- Merge all the start time with the initial
+            # ### [HARD CODED] ###
+            PID_number = self.helper.extract_int(PID)
+            if PID_number <= 12:
+                start_time = [start_time_initial]
+            else:
+                start_time = []
+            for time in start_time_rest:
+                start_time.append(time)
+            
+            timestamp = start_time
+
+            
+            #timestamp = self.helper.convert_tuple_vector_to_list(timestamp)
+
+            #--- Calculate the RCT in the perspective of all events
+            rct_evolution = []
+            for start_time_event in start_time:
+                rct = finished_time - start_time_event
+                rct_evolution.append(rct)
+            
+        return (rct_evolution, timestamp, flag_part_completed)
+    
+    def get_digital_RCTtracking(self, PID):
+        """
+        This function takes the RCT calculated by the Digital Twin
+        """
+        PID = int(self.helper.extract_int(PID))
+
+        with sqlite3.connect(self.database_path) as db:
+            #--- Extract RCT and Timestamp
+            RCT = db.execute("SELECT RCT FROM RCTtracking WHERE PID= ?", (PID,)).fetchall()
+            timestamp = db.execute("SELECT timestamp_real FROM RCTtracking WHERE PID= ?", (PID,)).fetchall()
+
+            #--- Convert tuple
+            RCT = self.helper.convert_tuple_vector_to_list(RCT)
+            timestamp = self.helper.convert_tuple_vector_to_list(timestamp)
+
+        return (RCT, timestamp)
+
```

## dtwinpy/services.py

```diff
@@ -469,31 +469,35 @@
 
             #--- Find the highest RCT for that part
             ASIS_RCT = rcts_paths[0]
 
             #--- Create the gain vector
             gain_vect = []
 
+            #--- Remove the AS IS gain, because it's not in the vector of possible paths
+            rcts_paths.pop(0)
+
             #--- For each RCT of that part
             for rct in rcts_paths:
                 #--- Calculate the RCT Indicator (how close it's from the worst scenario)
                 rct_indicator = rct / ASIS_RCT
 
                 #--- Calculate the RCT Gain (how far it's from the worst scenario)
                 rct_gain = 1 - rct_indicator
 
                 #--- Store this gain into the gain vector
                 gain_vect.append(rct_gain)
 
             #--- Compare the higher gain with the threshold
             highets_gain = max(gain_vect)
             
+            """
             #--- Remove the AS IS gain, because it's not in the vector of possible paths
             gain_vect.pop(0)
-
+            """
 
             if highets_gain >= rct_threshold:
                 #-- Rise the feedback flag
                 flag_feedback = True
                 #-- Take note of the optimized path
                 path_to_implement = gain_vect.index(highets_gain) 
 
@@ -689,18 +693,18 @@
 
         #--- Get the first dictionary key 
         part_name_list = list(rct_dict.keys())
         part_name = part_name_list[0]
         part_id = int(re.findall(r'\d+', part_name)[0])
 
         #--- Get the first path
-        path_1 = rct_dict[part_name][1]
+        path_1 = rct_dict[part_name][0] # path_1 = rct_dict[part_name][1]
 
         #--- Get the second path
-        path_2 = rct_dict[part_name][2]
+        path_2 = rct_dict[part_name][1] # path_2 = rct_dict[part_name][2]
 
         #--- Get the feedback flag (if need to implement or not the feedback)
         feedback_flag = publish_results[0]
 
         #--- Get the part id of the first part making decision
         queue_id = publish_results[1]
 
@@ -779,9 +783,56 @@
             #--- Return for the first branch
             rct_results = self.return_first_branch(rct_dict= rct_dict, publish_results= publish_results)
             return rct_results
 
     # =================================================================================
 
     # ================================== RCT Tracking ==================================
+    def run_RCT_tracking(self, palletID):
+        """
+        Run RCT tracking for a specific palletID. The function should translate the palletID to
+        a PID. For this specific PID, the function runs a simulation until the PID get finished
+        and based on that calculates the RCT. Ideally, this function is called every time that the
+        service is required (align with Synchronization). After every prediction the function saves
+        the RCT in a table of the exp_database writing the PID and the RCT. So when the PID is finished
+        a new PID is created for the same palletID and the calculation continues. In the end, with this function
+        (since the DT is aligned and updated) it will be possible to have a more precise prediction.
+
+        TODO:
+        1) Extract the PID for a given PalletID
+        2) Run a simulation for this targeted PID
+        3) Calculate the Remaining Cycle Time for that target PID
+        4) Write the PID and RCT in a table
+        
+        WARNINGS:
+        1) In the physical system when the last machine finished a PID it takes a while to 
+        be created a ne PID (needs to reach the first machine again)
+        """
+
+        # ------------- Extract PID for a given PalletID -------------
+        PID = self.ID_database.get_PID_from_PalletID(palletID)
+        # ------------------------------------------------------------
+
+        # ------------- Run simulation for a PID -------------
+        targeted_PID = self.helper.extract_int(PID)
+        # --- Generate a new model
+        self.digital_model =  self.generate_digital_model(targeted_part_id= targeted_PID)
+
+        # --- Check if the PID is in the simulation
+        part_in_model = self.digital_model.check_partID_in_simulation(PID)
+
+        if part_in_model == True:
+            # --- Run the simulation
+            self.digital_model.run()
+            # -----------------------------------------------------
+
+            # ------------- Calculates the RCT -------------
+            RCT = self.digital_model.calculate_RCT(part_id_selected= targeted_PID)
+            # ----------------------------------------------
+
+            # ------------- Write the results -------------
+            self.exp_database.write_RCTtracking(PID= targeted_PID, RCT= RCT, palletID= palletID)
 
-    
+            self.helper.printer(f"RCT Tracking for {PID} ({palletID}) done. RCT: {RCT}. Writing into the database", 'brown')
+
+        else:
+            self.helper.printer(f"[WARNING] Not possible to track the RCT of the {PID} because the part was not found in the model. Possibly the {palletID} didn't manage to get in the Machine 1 yet.")
```

## dtwinpy/synchronizer.py

```diff
@@ -15,16 +15,17 @@
 import dtwinpylib
 #reload this specifc module to upadte the class
 importlib.reload(dtwinpylib.dtwinpy.validator)"""
 
 
 
 class Zone():
-    def __init__(self, machine, queue_list):
-        self.help = Helper()
+    def __init__(self, machine, queue_list, digital_model= None):
+        self.helper = Helper()
+        self.digital_model = digital_model
         self.name = "Zone of " + machine.get_name()
         self.machine = machine
         self.zoneID = self.machine.get_id()
         self.queue_list = queue_list
         self.zoneInd = None
         #--- Counters for in and out number of parts
         self.inZone = 0
@@ -81,14 +82,24 @@
 
             #-- Rase the flag that this machine started the simulation with a part
             self.flag_initial_working = True
 
             #-- Increment the initial condition indicator
             self.Zone_initial += 1
 
+            print(f"[SYNC] {self.machine.get_name()} started with part already been processed!")
+            print(f"--- From the Digital Mode: ---")
+            print(f"machine_working: {self.machine_working}")
+            print(f"last_started_time: {self.last_started_time}")
+            print(f"initial_part: {initial_part.get_name()}")
+
+
+        # ------- DOUBLE CHECK -------
+        self.check_inital_working_machine()
+
 
 
     #--- A part entered the Zone
     def addIn(self, part_id):
         self.inZone += 1
         
         #--- Everytime a part is ADD to the zone we add it to the queue
@@ -121,19 +132,18 @@
         # OLD: if self.get_first_zone_event() == False and len(self.parts_ids_in_queue)>0:
         #--- Moda a caralha
         if part_id in self.parts_ids_in_queue:
             #--- I just remove if is not the first event (Finished). If something never
             # entered the zone and it's leaveing, I don't care about it.
             self.parts_ids_in_queue.remove(part_id)
         else:
-            self.help.printer(f"[WARNING][synchronizer.py/Mstarted()] {part_id} was not found in elements vector of the queue", "yellow")
+            self.helper.printer(f"[WARNING][synchronizer.py/Mstarted()] {part_id} was not found in elements vector of the queue", "yellow")
             #print(f"[WARNING][synchronizer.py/Mstarted()] {part_id} was not found in elements vector of the queue")
             print("This might happen if the element is an initial part. If that not the case, CHECK IT OUT!")
-            print(f"printing the list of parts in the queue: {self.parts_ids_in_queue}")
-    
+            print(f"printing the list of parts in the queue: {self.parts_ids_in_queue}")    
     def Mfinished(self, part_id):
         #-- In the case that this was the part that the machine started the simulation
         if self.flag_initial_working == True:
             self.flag_initial_working = False
         
         #-- Decrease the machine counter
         self.machine_working -= 1
@@ -143,17 +153,15 @@
             #--- I just remove if is not the first event (Finished). If something never
             # entered the zone and it's leaveing, I don't care about it.
             self.parts_ids_in_machine.remove(part_id)"""
         
         if part_id in self.parts_ids_in_machine:
             self.parts_ids_in_machine.remove(part_id)
         else:
-            self.help.printer(f"[WARNING][synchronizer.py/Mstarted()] {part_id} was not found in elements vector of the machine", "yellow")
-
-       
+            self.helper.printer(f"[WARNING][synchronizer.py/Mstarted()] {part_id} was not found in elements vector of the machine", "yellow")     
     def next_allocation(self, queue_allocated):
             # --- Check if it's a branching machine
             if self.machine.get_branch() != None:
                 machine_queues = self.machine.get_queue_out()
 
                 # Create a vector with the names of the queues
                 machine_queues_name = []
@@ -167,15 +175,38 @@
                 if queue_position == len(machine_queues_name) - 1:
                     # If it was the last, the next is the first
                     self.next_queue_position = 0
                 # Incase it was not the last
                 else:
                     self.next_queue_position = queue_position + 1
 
-    
+    def check_inital_working_machine(self):
+        model_path = self.digital_model.get_model_path()
+        with open(model_path, 'r+') as model_file:
+            data = json.load(model_file)
+            #--- For each machine (node)
+            for node in data['nodes']:
+                if node['activity'] == self.machine.get_id():
+                    self.machine_worked_time = node['worked_time']
+        
+        if self.machine_worked_time != 0:
+            self.machine_worked_time_initial = self.machine_worked_time[0]
+            self.machine_working_initial_part = self.machine_worked_time[1]
+
+        # ---------- CHECK ------------
+        if (self.machine_working == 0 and self.machine_worked_time != 0):
+            self.helper.printer(f"[ERROR][synchronizer.py/check_inital_working_machine()] The Sync thinks that there is no part in the machine, but actually the worked time in the model is different than 0", 'red')
+            print(f"--- From the Digital Mode: ---")
+            print(f"machine_working: {self.machine_working}")
+            print(f"last_started_time: {self.last_started_time}")
+
+            print(f"--- From the Model JSON: ---")
+            print(f"machine_worked_time_initial: {self.machine_worked_time_initial}")
+            print(f"machine_working_initial_part: {self.machine_working_initial_part}")
+
 
     def self_validation(self, Verbose = True):
         #--- Use the data from the simulation (digital log)
         self_counter = 0
         #--- Check the number of parts in the queues ins
         for queue in self.queue_list:
             self_counter += queue.get_len()
@@ -292,15 +323,15 @@
     def create_zones(self):
         for machine in self.machines_vector:
             #--- Basic information from the machine
             machine_name = machine.get_name()
             machine_queues_in_list = machine.get_queue_in()
 
             #--- create a temp Zone object
-            new_zone = Zone(machine= machine, queue_list= machine_queues_in_list)
+            new_zone = Zone(machine= machine, queue_list= machine_queues_in_list, digital_model= self.digital_model)
 
             #--- add the Zone object in the dictionary of zones
             self.zones_dict[machine_name] = new_zone
 
     def count_total_parts(self):
         """
         This function counts the total number of part in the system. This function is used
@@ -554,14 +585,19 @@
                 # ============= Update Model.json =============
                 model_path = self.digital_model.get_model_path()
                 with open(model_path, 'r+') as model_file:
                     data = json.load(model_file)
                     #--- For each machine (node)
                     for node in data['nodes']:
                         if node['activity'] == current_machine.get_id():
+                            # ISSUE #278: Sometimes Sync was not updating, maybe the flag initial was being updated wrong somewhere
+                            # because it came from the digital model, and we're running Sync very fast or even some change in
+                            # validation that change this property of the machine object
+
+                            # [OLD]
                             node['worked_time'] = (Delta_T_started, parts_id_in_machine) 
  
                             #---- Write Back the Changes
                             # Move the file pointer to the beginning of the file
                             model_file.seek(0)
                             # Write the modified data back to the file
                             json.dump(data, model_file)
```

## dtwinpy/tester.py

```diff
@@ -1,41 +1,184 @@
+from dtwinpylib.dtwinpy.helper import Helper
+from dtwinpylib.dtwinpy.interfaceDB import Database
+from dtwinpylib.dtwinpy.Digital_Twin import Digital_Twin
 
+#--- Commom Libraries
 import sqlite3
 import json
 import os
 from dtwinpylib.dtwinpy.helper import Helper
+import numpy as np
 import shutil
 import sys
+from matplotlib import pyplot as plt
+import re
+from natsort import natsort_keygen
+
+
+
 
 class Tester():
-    def __init__(self, exp_id = 'recent'):
-        
+    def __init__(self, exp_id = 'recent', from_data_generation= False, name= None):
         #--- attributes from allexp_database
         self.allexp_path = 'allexp_database.db'
         self.allexp_table = 'experiment_setup'
         self.exp_id = exp_id
         self.helper = Helper()
-        
-    def initiate(self):
-        #--- loading the experiment setup from allexp
+        self.from_data_generation = from_data_generation
+    
+    def initiate_for_analysis(self):
         self.load_exp_setup()
-        self.replace_initial_json()
+        # ------ Create a Digital Twin object ------
+        self.mydt = Digital_Twin(name= self.name, keepModels= True)
+        self.initial_digital_mode = self.mydt.generate_digital_model()
+        self.intial_WIP = self.initial_digital_mode.get_all_parts()
+
+        #------------------------------- experimental database & Figure path ------------------------------
+        if self.from_data_generation == False:
+            self.exp_db_path = f"databases/{self.name}/exp_database.db"
+            self.figures_folder = f"figures/{self.name}"
+
+        if self.from_data_generation == True:
+            self.exp_db_path = f"data_generation/{self.exp_id}/databases/exp_database.db"
+            self.figures_folder = f"data_generation/{self.exp_id}/figures"
+        
+        #--- generate the path of the real database
+        self.real_database_path = self.exp_db_path.replace('exp', 'real')
+
+        print("|-- Printing Paths:")
+        print(f"|---- Experimental Database Path: {self.exp_db_path}")
+        print(f"|---- Figures Folder Path: {self.figures_folder}")
+        #------------------------------------------------------------------------------------------
+
+        
 
 
-        self.exp_db_path = f"databases/{self.name}/exp_database.db"
-        self.exp_setup_table = "setup_data"
 
+    # ----- Deafult procedures to deal with allexp_db -----   
+    def initiate(self):
+        #--------------- LOAD SETUP -----------------
+        self.load_exp_setup()      
+        self.replace_initial_json() #--- replace initial json in models folder
+
+        print(f"'{self.exp_id}' experiment is loaded")
+        #-------------------------------------------
+
+        #------------------------------- experimental database & Figure path ------------------------------
+        if self.from_data_generation == False:
+            self.exp_db_path = f"databases/{self.name}/exp_database.db"
+            self.figures_folder = f"figures/{self.name}"
+
+        if self.from_data_generation == True:
+            self.exp_db_path = f"data_generation/{self.exp_id}/databases/exp_database.db"
+            self.figures_folder = f"data_generation/{self.exp_id}/figures"
+        
+        #
+        print("|-- Printing Paths:")
+        print(f"|---- Experimental Database Path: {self.exp_db_path}")
+        print(f"|---- Figures Folder Path: {self.figures_folder}")
+        #------------------------------------------------------------------------------------------
         
+        #-- delete the existing exp_database in the databases folder
         self.delete_exp_database()  #--- delete existing exp_database to create new
+
+        #-- Figures Folder
+        if not os.path.exists(self.figures_folder):
+            os.makedirs(self.figures_folder)
+            print(f"Folder {self.figures_folder} created...")
+
+        #-- create a Database object
+        try:
+            self.exp_db = Database(
+                database_path= self.exp_db_path,
+                experimental_mode= True
+            )
+        except sqlite3.OperationalError:
+            self.helper.printer(f"[ERROR][tester.py/__init__()] It was not possible to open the database path: {self.exp_db_path}. Check it out! Skiping...", 'red')
+     
+        
+        
+        
+        self.exp_setup_table = "setup_data"
+
         self.create_exp_database()  #--- create new exp_db and create setup_data table
         self.write_setup()          #--- write setup data from allexp_db to exp_db setup_data table
+        self.create_rt_process_time_log()
         
+    # ----- Plotting -----
+    def plot(self, show_plot= False):
+        """
+        Plot all the data available after an experiment. The function includes the following plots:
+        - Validation Indicators
+        - RCT paths
+        - Queue Occupation
+        """
+        if not os.path.exists(self.exp_db_path):
+            self.helper.printer(f"[WARNING][tester.py/__init__()] The experimental database path: {self.exp_db_path} doesn't exist! SKIPING PLOT")
+
         
+        else:
+            # ----------- CREATE PLOTTER ---------------
+            plotter = Plotter(
+                exp_database_path= self.exp_db_path,
+                plotterDT= self.mydt,
+                figures_path= self.figures_folder,
+                show= show_plot,
+                save= True
+            )
+            # -------------------------------------------
+
+            # ------------- PLOT VALIDATION INDICATORS ----------
+            plotter.plot_valid_indicators(threshold= self.input_threshold)
+            # ---------------------------------------------------
+
+            # ------------- PLOT RCT PATH -------------
+            plotter.plot_RCT_paths()
+            # -----------------------------------------
+
+            # ------------- PLOT QUEUE OCCUPATION -------------
+            plotter.plot_queues_occupation()
+            # --------------------------------------------------
+
+            # ------------- PLOT COMPARATIVE CT ----------------
+            # only for system with alternating policy
+            if self.flag_publish == False: plotter.plot_comparative_parts_CT()
+
+
+    # ----- Analyses -----
+    def run_analysis(self, real_db_path):
+        #--- Create global results table
+        self.create_results_table()
+
+        #--- Calculate main global results
+        self.calculate_CT(real_db_path= real_db_path, WIP_parts= self.intial_WIP)
+
+    def plot_utilization(self):
+        utilization_dict = self.run_utilization()
+        plotter = Plotter(
+                exp_database_path= self.exp_db_path,
+                plotterDT= self.mydt,
+                figures_path= self.figures_folder,
+                show= False,
+                save= True
+            )
         
+        plotter.plot_utilization(utilization_dict)
 
+    def plot_RCTtracking(self):
+        plotter = Plotter(
+                exp_database_path= self.exp_db_path,
+                plotterDT= self.mydt,
+                figures_path= self.figures_folder,
+                show= True,
+                save= True
+            )
+        
+        plotter.plot_RCTtracking()
+        
 
 #-------------------------------------------------------------------------------------------------
 #---------------------------------------- MAIN FUNCTIONS -----------------------------------------
 #-------------------------------------------------------------------------------------------------
 
     #--- to create experimental_data table
     def create_allexp_database(self):
@@ -128,15 +271,16 @@
                 contemp_Q5_2 INTEGER DEFAULT 6,
 
                 n_parts_Q1 INTEGER DEFAULT '["Part 1","Part 2","Part 3","Part 4","Part 5","Part 6","Part 7","Part 8","Part 9","Part 10","Part 11","Part 12"]',
                 n_parts_Q2 INTEGER DEFAULT '[]',
                 n_parts_Q3 INTEGER DEFAULT '[]',
                 n_parts_Q4 INTEGER DEFAULT '[]',
                 n_parts_Q5 INTEGER DEFAULT '[]',
-                flag_publish TEXT DEFAULT True
+                flag_publish TEXT DEFAULT True,
+                flag_validation  TEXT DEFAULT True
             )
             """)
             allexp.commit()
 
     #--- load all the setup variables from allexp_database
     def load_exp_setup(self):
         with sqlite3.connect(self.allexp_path) as allexp:
@@ -148,71 +292,72 @@
             self.objective = exp_setup[0][1]
             self.name= exp_setup[0][2]
             self.Freq_Sync= exp_setup[0][3] 
             self.Freq_Valid= exp_setup[0][4] 
             self.Freq_Service= exp_setup[0][5]
             self.delta_t_treshold=exp_setup[0][6]
             self.flag_API= True if exp_setup[0][7] == 'True' else False
-            self.rct_threshold= exp_setup[0][8]
+            self.rct_threshold= -1
             self.rct_queue= exp_setup[0][9]
             self.flag_external_service= True if exp_setup[0][10] == 'True' else False
             self.logic_threshold= exp_setup[0][11]
             self.input_threshold= exp_setup[0][12]
             self.flag_publish= True if exp_setup[0][78] == 'True' else False
+            self.flag_validation= True if exp_setup[0][79] == 'True' else False
 
             self.initial_json = {
                 "nodes": [
                     {
                     "activity": 1,
                     "predecessors": json.loads(exp_setup[0][13]),
                     "successors": json.loads(exp_setup[0][14]),
                     "frequency": exp_setup[0][15],
                     "capacity": exp_setup[0][16],
-                    "contemp": exp_setup[0][17],
+                    "contemp": json.loads(exp_setup[0][17]),
                     "cluster": exp_setup[0][18],
                     "worked_time": exp_setup[0][19]
                     },
                     {
                     "activity": 2,
                     "predecessors": json.loads(exp_setup[0][20]),
                     "successors": json.loads(exp_setup[0][21]),
                     "frequency": exp_setup[0][22],
                     "capacity": exp_setup[0][23],
-                    "contemp": exp_setup[0][24],
+                    "contemp": json.loads(exp_setup[0][24]),
                     "cluster": exp_setup[0][25],
                     "worked_time": exp_setup[0][26],
                     "allocation_counter": exp_setup[0][27]
                     },
                     {
                     "activity": 3,
                     "predecessors": json.loads(exp_setup[0][28]),
                     "successors": json.loads(exp_setup[0][29]),
                     "frequency": exp_setup[0][30],
                     "capacity": exp_setup[0][31],
-                    "contemp": exp_setup[0][32],
+                    "contemp": json.loads(exp_setup[0][32]),
                     "cluster": exp_setup[0][33],
                     "worked_time": exp_setup[0][34]
                     },
                     {
                     "activity": 4,
                     "predecessors": json.loads(exp_setup[0][35]),
                     "successors": json.loads(exp_setup[0][36]),
                     "frequency": exp_setup[0][37],
                     "capacity": exp_setup[0][38],
-                    "contemp": exp_setup[0][39],
+                    "contemp": json.loads(exp_setup[0][39]),
                     "cluster": exp_setup[0][40],
                     "worked_time": exp_setup[0][41]
                     },
                     {
                     "activity": 5,
                     "predecessors": json.loads(exp_setup[0][42]),
                     "successors": json.loads(exp_setup[0][43]),
                     "frequency": exp_setup[0][44],
                     "capacity": exp_setup[0][45],
-                    "contemp": exp_setup[0][46],
+                    "contemp": json.loads(exp_setup[0][46]),
                     "cluster": exp_setup[0][47],
                     "worked_time": exp_setup[0][48]
                     }
                 ],
                 "arcs": [
                     {
                     "arc": json.loads(exp_setup[0][53]),
@@ -255,29 +400,38 @@
                     json.loads(exp_setup[0][73]),
                     json.loads(exp_setup[0][74]),
                     json.loads(exp_setup[0][75]),
                     json.loads(exp_setup[0][76]),
                     json.loads(exp_setup[0][77])
                 ]
                 }
-            
+
+    def get_setup(self):
+        """
+        Return the basic setups 'selfs' of the specific Tester object
+        """      
+        return (self.exp_db_path, self.figures_folder, self.mydt)
+
     #--- replace the existing initial json file in models folder with the data from allexp_database
     def replace_initial_json(self):
         json_path = f"models/{self.name}/initial.json"
         with open(json_path, 'w') as file:
             json.dump(self.initial_json, file)
 
     #--- delete existing exp_database
     def delete_exp_database(self):
         if os.path.exists(self.exp_db_path):
             os.remove(self.exp_db_path)
             print(f"Existing exp_database deleted")
         else:
             print(f"No exp_database was found. New one will be created.")
 
+    def delete_figures(self):
+        self.helper.delete_figures(self.figures_folder)
+
     #--- to create exp_database and experimental_data table
     def create_exp_database(self):
         with sqlite3.connect(self.exp_db_path) as exp_db:
                 exp_db.execute(f"""CREATE TABLE IF NOT EXISTS {self.exp_setup_table} (
                     exp_id TEXT PRIMARY KEY DEFAULT 'recent',
                     timestamp TEXT,
                     objective TEXT,
@@ -287,15 +441,17 @@
                     Freq_Service INTEGER DEFAULT 2,
                     delta_t_treshold INTEGER DEFAULT 20,
                     flag_API TEXT DEFAULT 'True',
                     rct_threshold FLOAT DEFAULT 0,
                     rct_queue INTEGER DEFAULT 2,
                     flag_external_service INTEGER DEFAULT 'True',
                     logic_threshold FLOAT DEFAULT 0.8,
-                    input_threshold FLOAT DEFAULT 0.8
+                    input_threshold FLOAT DEFAULT 0.8,
+                    flag_publish TEXT DEFAULT True,
+                    flag_validation  TEXT DEFAULT True
                     )
                     """)
                 exp_db.commit()
 
     #--- write mydt definitions
     def write_setup(self):
         with sqlite3.connect(self.exp_db_path) as exp_db:
@@ -310,19 +466,21 @@
                     Freq_Service,
                     delta_t_treshold,
                     flag_API,
                     rct_threshold,
                     rct_queue,
                     flag_external_service,
                     logic_threshold,
-                    input_threshold) VALUES (?,?,?,?,?,?,?,?,?,?,?,?,?,?)
+                    input_threshold,
+                    flag_publish,
+                    flag_validation) VALUES (?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)
                 """,(self.exp_id, self.helper.get_time_now()[0], self.objective, self.name, self.Freq_Sync, 
-                        self.Freq_Valid, self.Freq_Service, self.delta_t_treshold, self.flag_API, 
-                        self.rct_threshold, self.rct_queue, self.flag_external_service, self.logic_threshold, 
-                        self.input_threshold))
+                        self.Freq_Valid, self.Freq_Service, self.delta_t_treshold, str(self.flag_API), 
+                        self.rct_threshold, self.rct_queue, str(self.flag_external_service), self.logic_threshold, 
+                        self.input_threshold, str(self.flag_publish), str(self.flag_validation)))
                 exp_db.commit()
 
     #--- create exp_models_tables for all machines
     def create_exp_machines_table(self, machine_id, branching = False):
         if branching == False:        
             with sqlite3.connect(self.exp_db_path) as exp_db:
                 exp_db.execute(f"""CREATE TABLE IF NOT EXISTS machine_{machine_id} (
@@ -452,15 +610,15 @@
                 cluster,
                 worked_time) VALUES (?,?,?,?,?,?,?,?)
                 """,(str(model_name), 
                     json.dumps(model_dict['nodes'][machine_id-1]['predecessors']),
                     json.dumps(model_dict['nodes'][machine_id-1]['successors']),
                     model_dict['nodes'][machine_id-1]['frequency'],
                     model_dict['nodes'][machine_id-1]['capacity'],
-                    model_dict['nodes'][machine_id-1]['contemp'],
+                    json.dumps(model_dict['nodes'][machine_id-1]['contemp']),
                     model_dict['nodes'][machine_id-1]['cluster'],
                     json.dumps(model_dict['nodes'][machine_id-1]['worked_time'])))
 
             #--- write allocation counter for machine 2    
             cursor.execute(f"""UPDATE machine_2 SET allocation_counter = {model_dict['nodes'][1]['allocation_counter']} WHERE model_name = '{model_name}'""")
             
             #--- save changes
@@ -484,15 +642,1083 @@
         
         self.create_exp_queues_table(queue_id = 1, converging = False)
         self.create_exp_queues_table(queue_id = 2, converging = False)
         self.create_exp_queues_table(queue_id = 3, converging = False)
         self.create_exp_queues_table(queue_id = 4, converging = False)
         self.create_exp_queues_table(queue_id = 5, converging = True)
 
-    #--- assign exp_id to the 'recent' experiment in the allexp_database
+    #--- assign exp_id to the 'recent' experiment in the allexp_database and exp_database
     def assign_exp_id(self,exp_id):
+        #--- updating in allexp
         with sqlite3.connect(self.allexp_path) as allexp:
             cursor = allexp.cursor()
-            cursor.execute(f"""UPDATE {self.allexp_table} SET exp_id = {exp_id} WHERE exp_id = 'recent'""")
+            cursor.execute(f"""UPDATE {self.allexp_table} SET exp_id = '{exp_id}' WHERE exp_id = 'recent'""")
             allexp.commit()
+        #--- updating in exp_db
+        with sqlite3.connect(self.exp_db_path) as exp_db:
+            cursor = exp_db.cursor()
+            cursor.execute(f"""UPDATE setup_data SET exp_id = '{exp_id}' WHERE exp_id = 'recent'""")
+            exp_db.commit()
+        self.exp_id = exp_id
+
+    #--- for writing process time change of real tein in real time basis
+    #-- to be used in change_rt_process_time.py
+    def write_rt_process_time_log(self, process_time_vector):
+        time = self.helper.get_time_now()
+        with sqlite3.connect(self.exp_db_path) as exp_db:
+            cursor = exp_db.cursor()
+            cursor.execute(f"""INSERT INTO rt_process_time_log (
+                publish_time_real,
+                publish_time_str,
+                Machine_1,
+                Machine_2,
+                Machine_3,
+                Machine_4,
+                Machine_5) VALUES (?,?,?,?,?,?,?)
+                """,
+                (time[1], 
+                time[0],
+                process_time_vector[0],
+                process_time_vector[1],
+                process_time_vector[2],
+                process_time_vector[3],
+                process_time_vector[4]))
+            exp_db.commit()
+
+    #--- create rt_process_time_log
+    def create_rt_process_time_log(self):
+        with sqlite3.connect(self.exp_db_path) as exp_db:
+            exp_db.execute(f"""CREATE TABLE IF NOT EXISTS rt_process_time_log (
+                publish_id INTEGER PRIMARY KEY,
+                publish_time_real INTEGER,
+                publish_time_str TEXT,
+                Machine_1 INTEGER DEFAULT NULL,
+                Machine_2 INTEGER DEFAULT NULL,
+                Machine_3 INTEGER DEFAULT NULL,
+                Machine_4 INTEGER DEFAULT NULL,
+                Machine_5 INTEGER DEFAULT NULL
+                )
+                """)
+            exp_db.commit()
+
+    #--- create results table
+    def create_results_table(self):
+        with sqlite3.connect(self.exp_db_path) as exp_db:
+            exp_db.execute(f"""CREATE TABLE IF NOT EXISTS results (
+                result_id INTEGER PRIMARY KEY,
+                run_time INTEGER,
+                start_time INTEGER,
+                finish_time INTEGER,
+                last_part TEXT,
+                number_of_parts_processed INTEGER,
+                throughput_per_seconds FLOAT,
+                thourhput_per_hour FLOAT,
+                CT_system FLOAT,
+                List_parts_finished  TEXT,
+                CT_parts TEXT,
+                average_CT FLOAT
+                )
+                """)
+            exp_db.commit()
+
+    # =============================== ANALYSIS FUNCTIONS =====================================
+    #--- complete CT of each part (considering waiting time)
+    def calculate_CT_complete(self, real_db_path, WIP_parts):
+        #--- Create a list with name of the initial parts
+        intial_parts= []
+        initial_parts_id = []
+        for part in WIP_parts:
+            intial_parts.append(part.get_name())
+            initial_parts_id.append(part.get_id())
+        
+        #--- Get the highest part id
+        print(f"initial_parts_id: {initial_parts_id}")
+        last_part_id = max(initial_parts_id)
+
+        #--- Define vectors
+        CT_parts_name_vector = []
+        CT_parts_time_vector = []
+        CT_start_dictionary = {}
+        CT_finish_dictionary = {}
+
+        # ------ Connect with the real database ------
+        with sqlite3.connect(real_db_path) as db:
+            #-- Get name of parts finished by Machine 5
+            parts_name_finished = db.execute("SELECT part_id FROM real_log WHERE machine_id= ? and activity_type= ?", ('Machine 5', 'Finished')).fetchall()
+            parts_time_finished = db.execute("SELECT timestamp_real FROM real_log WHERE machine_id= ? and activity_type= ?", ('Machine 5', 'Finished')).fetchall()
+            
+            #-- convert tuple
+            parts_name_finished = self.helper.convert_tuple_vector_to_list(parts_name_finished)
+            parts_time_finished = self.helper.convert_tuple_vector_to_list(parts_time_finished)
+
+            #--- Get the global start time of the simulation
+            start_time_global = db.execute("SELECT timestamp_real FROM real_log WHERE event_id= ?", (1,)).fetchall()
+            start_time_global= self.helper.convert_tuple_vector_to_list(start_time_global)
+            start_time_global = start_time_global[0]
+
+        #--- Cycle time for initial parts
+        for part_name in parts_name_finished:
+            # ------------ CHECK FOR INITIAL PART ------------
+            flag_initial = True
+            try:
+                part_index = intial_parts.index(part_name)
+                #print(f"{part_name} is an initial part...")
+                
+            except ValueError:
+                flag_initial = False
+            # -------------------------------------------------
+
+            if flag_initial == True:
+                CT_start_dictionary[part_name] = start_time_global
+
+                # ----------- CHECK FOR FINISHED TIME -------------
+                flag_initial_finished = True
+                try: 
+                    part_index = parts_name_finished.index(part_name)
+                except ValueError:
+                    flag_initial_finished = False
+
+                if flag_initial_finished == True:
+                    finished_time = parts_time_finished[part_index]
+                    CT_finish_dictionary[part_name] = finished_time
+            
+        #--- Cycle time for parts higher than the previous last_part_id
+        for i in range(len(parts_name_finished)):
+            part_name = parts_name_finished[i]
+
+            #-- Extract the ID of the part finished
+            part_finished_id = self.helper.extract_int(part_name)
+
+            #-- Update next id and last id
+            next_part_id = last_part_id + 1
+            last_part_id += 1
+            next_part_name = f'Part {next_part_id}'
+
+            #-- Get the finished (started for the next part)
+            next_start_time = parts_time_finished[i]
+
+            #-- Check if that part finished the next cycle
+            flag_finished = True
+            try:
+                part_index = parts_name_finished.index(next_part_name)
+                
+            except ValueError:
+                flag_finished = False
+                #print(f"{next_part_name} didn't finished the cycle...")
+            
+            if flag_finished == True:
+                CT_start_dictionary[next_part_name] = next_start_time
+
+                #-- Since the part was finished, looks for the Finished time of that part
+                finished_time = parts_time_finished[part_index]
+                CT_finish_dictionary[next_part_name] = finished_time
+
+        #--- Order the dictionaries based on the numerical order
+        # Define a function to split the keys into alphabetical and numerical parts
+        # Generate a key function using natsort_keygen() to sort the keys in natural numerical order
+        key_func = natsort_keygen()
+    
+        # --------------------------------- ORDERING --------------------------------------
+        CT_start_dictionary = dict(sorted(CT_start_dictionary.items(), key=lambda x: key_func(x[0])))
+        CT_finish_dictionary = dict(sorted(CT_finish_dictionary.items(), key=lambda x: key_func(x[0])))
+        # ---------------------------------------------------------------------------------
+
+        # ---------- WRITE dictionary results in the vector ----------
+        #print(f"CT_finish_dictionary: {CT_finish_dictionary}")
+        #print(f"CT_start_dictionary: {CT_start_dictionary}")
+
+        for key_part in CT_start_dictionary:
+            CT_parts_name_vector.append(key_part)
+            CT_parts_time_vector.append(CT_finish_dictionary[key_part] - CT_start_dictionary[key_part])
+        
+        return (CT_parts_name_vector, CT_parts_time_vector)
+
+    #--- calculate CT and TH of system & parts and write to results table
+    def calculate_CT(self, real_db_path, WIP_parts):
+
+        with sqlite3.connect(real_db_path) as real_db:
+            cursor = real_db.cursor()
+
+            # first and last trace of started nd finished.
+            cursor.execute("SELECT * FROM real_log LIMIT 1")
+            first_start_time = cursor.fetchone()[-1]
+
+            cursor.execute("SELECT * FROM real_log WHERE machine_id = ? AND activity_type = ? ORDER BY rowid DESC LIMIT 1", ('Machine 5','Finished'))
+            event = cursor.fetchall()
+            last_finish_time = event[0][-1]
+            last_part = event[0][4]
+            print(f"last_part to exit is: {last_part}")
+            
+            # count number of times machine 5 appears with activity as finished
+            cursor.execute("SELECT COUNT(*) FROM real_log WHERE machine_id = ? AND activity_type = ?", ('Machine 5','Finished'))
+            count = cursor.fetchone()[0]
+
+        #---throughput
+        run_time = last_finish_time - first_start_time
+        throughput_second = count/run_time #--- parts/second
+        throughput_hour = (count*3600)/run_time #--- parts/hour
+        ct_system = run_time/count
+
+
+        print(f"start: {first_start_time}\nstop: {last_finish_time}\nnumber of parts: {count}\nduration: {run_time}\nthroughput per seconds: {throughput_second}\nthourhput per hour: {throughput_hour}\nct_system: {ct_system}")
+        
+
+        #--- part level cycle time
+        CT_part_time = []
+        CT_part_list = []
+        """
+        #--- cycle time of parts
+        with sqlite3.connect(real_db_path) as real_db:
+            cursor = real_db.cursor()
+            # get a list of the unique values in the column
+            values = cursor.execute("SELECT DISTINCT part_id FROM real_log").fetchall()
+            # iterate over the values in the column
+            for value in values:
+                # execute the query with the current value
+                part_name = value[0]
+
+                start = cursor.execute(f"SELECT timestamp_real FROM real_log WHERE part_id = '{value[0]}' AND machine_id = 'Machine 1' AND activity_type = 'Started'").fetchall()
+
+                
+                finish = cursor.execute(f"SELECT timestamp_real FROM real_log WHERE part_id = '{value[0]}' AND machine_id = 'Machine 5' AND activity_type = 'Finished'").fetchall()
+                # print(start,finish,value[0])
+                if finish != []:
+                    CT_part_time.append(finish[0][0] - start[0][0])
+                    CT_part_list.append(value[0])
+        """
+
+        # ----------------- CALCULATE CT FOR EACH PART -----------------
+        (CT_part_list, CT_part_time) = self.calculate_CT_complete(real_db_path, WIP_parts)
+
+        average_CT = np.mean(CT_part_time)
+        print(f"average cycle time of parts: {average_CT}")
+
+        #--- write to results table in exp_db
+        with sqlite3.connect(self.exp_db_path) as exp_db:
+            cursor = exp_db.cursor()
+            cursor.execute(f"""INSERT INTO results (
+            run_time,
+            start_time,
+            finish_time,
+            last_part,
+            number_of_parts_processed,
+            throughput_per_seconds,
+            thourhput_per_hour,
+            CT_system,
+            List_parts_finished ,
+            CT_parts,
+            average_CT) VALUES (?,?,?,?,?,?,?,?,?,?,?)
+            """,(run_time,
+                first_start_time,
+                last_finish_time,
+                str(last_part),
+                count,
+                throughput_second,
+                throughput_hour,
+                ct_system,
+                json.dumps(CT_part_list),
+                json.dumps(CT_part_time),
+                average_CT))
+            
+            exp_db.commit()
+
+    def calculate_utilization(self,real_database_path, start_time_id, end_time_id, machine_id):
+        # ----------- SUPPORTING FUNCTION -----------
+        def update_utilization_end_id(real_database_path, start_time_id, end_time_id, machine_id):
+            with sqlite3.connect(real_database_path) as db:
+                #--- Read activity type (started and Finished) and event_id for a specific machien within a range
+                read_machine_events = db.execute("SELECT activity_type, event_id FROM real_log WHERE machine_id= ? and event_id>=? AND event_id<=?",
+                    (machine_id, start_time_id, end_time_id)).fetchall()
+                
+                machine_acitivities= []
+                machine_events_id = []
+                for i in range(len(read_machine_events)):
+                    machine_acitivities.append(read_machine_events[i][0])
+                    machine_events_id.append(read_machine_events[i][1])
+
+                #--- Flag to indicates if there is a finished before a start
+                flag_last_is_started = False
+
+                #--- Just the last value that matters, because for a specific machine either it's finish or started
+                #------------ MACHINE LAST EVENT: STARTED -------------
+                if machine_acitivities[-1] == 'Started':
+                    # If the last event is Started, it means that the previous one was Finished and tha
+                    # you should consider its end time id
+                    print(f"{machine_id} last trace is 'Started', updating the end time id from {end_time_id} to {machine_events_id[-2]}")
+                    end_time_id = machine_events_id[-2]
+                    flag_last_is_started = True
+
+                if machine_acitivities[-1] == 'Finished':
+                    # Everything fine...
+                    pass
+
+                return end_time_id
+        
+        #--- Update end time checking the last trace:
+        end_time_id= update_utilization_end_id(real_database_path, start_time_id, end_time_id, machine_id)
+
+        # connect to the database
+        conn = sqlite3.connect(real_database_path)
+        c = conn.cursor()
+
+        # query the database for the machine's events within the given period
+        c.execute("SELECT * FROM real_log WHERE machine_id=? AND event_id>=? AND event_id<=?",
+                (machine_id, start_time_id, end_time_id))
+        rows = c.fetchall()
+
+        # calculate the total time the machine spent working within the given period
+        total_working_time = 0
+        last_start_time = None
+        for row in rows:
+            if row[3] == 'Started':
+                last_start_time = row[7]
+            elif row[3] == 'Finished' and last_start_time is not None:
+                total_working_time += row[7] - last_start_time
+                last_start_time = None
+        
+        # calculate the initial time
+        c.execute("SELECT MIN(timestamp_real) FROM real_log WHERE event_id >= ? AND event_id <= ?", 
+                (start_time_id, end_time_id))
+        initial_time = c.fetchone()[0]
+
+        # calculate the total time within the given period
+        c.execute("SELECT MAX(timestamp_real) FROM real_log WHERE event_id>=? AND event_id<=?",
+                (start_time_id, end_time_id))
+        final_time = c.fetchone()[0] 
+
+        # calculate the total time
+        total_time = final_time - initial_time
+
+        # calculate the utilization rate
+        utilization_rate = (total_working_time / total_time) * 100
+
+        print(f"--- Utilization Rate: {utilization_rate} %")
+        print(f"--- Total Working Time: {total_working_time}")
+        print(f"--- Total Time: {total_time}")
+
+        # close the connection
+        conn.close()
+
+        return utilization_rate
+
+    def run_utilization(self):
+        """
+        Calculates the evolution of utilization of each machine trhough the simulation and also
+        the total utilization rate of each machine.
+        """
+        
+        #--- List of machine's name
+        machines_name = ['Machine 1', 'Machine 2', 'Machine 3', 'Machine 4', 'Machine 5']
+        
+        #--- Initial Pointers
+        start_time_id= 1
+        end_time_id= 3
+
+        #--- step (delta) between events id being analyzed
+        id_step = 2
+
+        #--- Dictionary to store the utilization for each machine
+        utilization_dict = {}
+        global_utilization_dict = {}
+
+        #--- Count the number of rows in the database
+        with sqlite3.connect(self.real_database_path) as db:
+            max_end_id = db.execute('SELECT COUNT(*) FROM real_log').fetchone()[0]
+
+        #--- calculate the evolution of utilization
+        for machine_name in machines_name:
+            #-- Temporary to store data
+            temp_utilization_vec = []
+            end_time_id= 3
+
+            while end_time_id <= max_end_id:
+
+                #--- Try to calculate the utilization
+                try:
+                    #-- calculate utilization for a given range
+                    machine_utilization = self.calculate_utilization(self.real_database_path, start_time_id, end_time_id, machine_name)
+                    
+                    #-- Add datapoint in the temporary vector
+                    temp_utilization_vec.append(machine_utilization)
+                
+                except:
+                    print(f"[WARINING] For some reason it was not possible to calculate the utilization for {machine_name}... Maybe because that machine didn't appeared within the following range of pointers: Start Time ID: {start_time_id} End Time ID: {end_time_id}")
+            
+                #--- Increment the end pointer, and keep always the start pointer
+                end_time_id += id_step
+
+
+            #--- After finishing the loop, add it into the dictionary
+            utilization_dict[machine_name]= temp_utilization_vec
+
+            #--- Global
+            machine_global_utilization= self.calculate_utilization(self.real_database_path, start_time_id, max_end_id, machine_name)
+            global_utilization_dict[machine_name] = machine_global_utilization
+
+        
+        print(" --------- Utilization Global ---------")
+        for key_name in global_utilization_dict:
+            print(f"[{key_name}]: {global_utilization_dict[key_name]}")
+
+        return utilization_dict
+    
+
+class Plotter():
+    def __init__(self, exp_database_path, plotterDT, figures_path= None,  show= False, save= True):
+        self.helper = Helper()
+        self.plotterDT = plotterDT
+        plt.clf()
+
+        #--- Experimental Database
+        self.exp_database_path = exp_database_path
+        self.exp_database = Database(
+            database_path= self.exp_database_path
+        )
+
+        #--- Real database path
+        self.real_database_path = self.exp_database_path.replace('exp', 'real')
+
+        #--- Figures Folder
+        self.figures_path = figures_path
+
+        #--- Common flags
+        self.show = show
+        self.save = save
+
+        #--- vector of markers and colors
+        self.markers = ['o', '*', '^', 's', 'd', 'v', 'p', 'x', '+']
+        self.colors = ['blue', 'orange', 'green', 'red' , 'purple']
+
+    #--- Basic Functions ---
+    def ADD_complemts(self, title, xlable, ylable):
+        """ Adds title, x lable and y lable"""
+
+        plt.title(title)
+        plt.xlabel(xlable)
+        plt.ylabel(ylable)
+        plt.legend()
+    
+    def set_max_min(self, xlim= None, ylim= None):
+        """ Set max and min for x and y. Receive vectors"""
+        if xlim:
+            plt.xlim(xlim)
+        if ylim:
+            plt.ylim(ylim)
+
+    def save_fig(self, name):
+        """Function takes the figure path and save the given figure using the given name"""
+        path_to_save = f"{self.figures_path}/{name}.png"
+        
+        print(f"Saving figure in the path {path_to_save}")
+
+        plt.savefig(path_to_save)
+
+
+    def plot_valid_indicators(self, threshold= 0.7, adjust = True):
+        """
+        This functions plots the validation indicators (logic and input) from
+        the experimental database. If threshold is given, the function also
+        trace the line of the threshold in the plot.
+        """
+        #---------
+        plt.clf()
+        #---------
+
+        #--- Read logic indicators
+        (logic_indicators, timestamp) = self.exp_database.read_ValidIndicator('logic_indicator')
+
+        #--- read input indicators
+        (input_indicators, timestamp) = self.exp_database.read_ValidIndicator('input_indicator')
+
+        #--- Check if there is any data:
+        if len(input_indicators) <= 1:
+            self.helper.printer(f"[ERROR][tester.py/plot_valid_indicators()] Not enough data to plot validation indicators... SKIPING PLOT")
+        
+        else:
+
+            #--- Plot logic indicator
+            plt.plot(timestamp, logic_indicators, marker='o', label= 'logic_indicator')
+
+            #--- Plot input indicator
+            plt.plot(timestamp, input_indicators, marker= 'x', label= 'input_indicator')
+
+            #--- Add threshold line
+            if threshold:   plt.axhline(threshold, color='red', linestyle='--', label='Indicator Threshold')
+            
+            #--- Adjust the scale of the graph
+            if adjust: self.set_max_min(ylim=[0, 1.05])
+
+            #--- Add complements
+            self.ADD_complemts(
+                title= "Validation Indicators",
+                xlable= "Timestamp (secs)",
+                ylable= "Indicator (%)"
+            )
+            
+            #--- Save
+            if self.save:
+                self.save_fig("Validation_Indicators")
+
+            #--- Show
+            if self.show:
+                plt.show()
+
+    def plot_RCT_paths(self):
+        """
+        This functions plots the validation indicators (logic and input) from
+        the experimental database. If threshold is given, the function also
+        trace the line of the threshold in the plot.
+        """
+        #---------
+        plt.clf()
+        #---------
+
+        #--- Read RCT paths
+        (rct_path1, rct_path2, timestamp) = self.exp_database.read_RCT_path()
+
+        #--- Plot logic indicator
+        plt.plot(timestamp, rct_path1, marker='o', label= 'Path 1 (Queue 3)')
+
+        #--- Plot input indicator
+        plt.plot(timestamp, rct_path2, marker= 'o', label= 'Path 2 (Queue 4)')
+
+        #--- Add complements
+        self.ADD_complemts(
+            title= "RCT Paths 1 and 2",
+            xlable= "Timestamp (secs)",
+            ylable= "RCT"
+        )
+        
+        #--- Save
+        if self.save:
+            self.save_fig("RCT_Path")
+
+        #--- Show
+        if self.show:
+            plt.show()
+
+    def plot_queues_occupation(self, number_queues = 5, stacked= False):
+        """
+        Loop through the queues table to get the amount of parts in the queue
+        after each synchronization. Plot this amount over time.
+        """
+        #---------
+        plt.clf()
+        #---------
+        
+        #--- Create a dictionary to store the occupation of each queue
+        queue_occupation = {}
+
+        #--- Loop through all the queues id 
+        for i in range(0, number_queues):
+            #-- Create Queue ID
+            queue_id= i + 1
+
+            #-- Extract occupation vector
+            occupation_vector = self.exp_database.read_queue_occupation(queue_id)
+
+            #-- Add the occupation of this queue in the global dictionary
+            queue_occupation[f'Queue {queue_id}'] = occupation_vector
+        
+        #--- Create the x_vector (syncs) with the same length as the queue_occupation
+        x_vector = []
+        for i in range(len(occupation_vector)):x_vector.append(i)
+
+        # ------ Plot for each queue ------
+        if stacked == False:
+            marker = 0
+            for i in range(0, number_queues): 
+                #-- Create Queue ID
+                queue_id= i + 1
+
+                #--- reset markers
+                if marker > len(self.markers): marker = 0
+
+                # ------------------ PLOT ----------------------
+                plt.step(
+                    x_vector, 
+                    queue_occupation[f'Queue {queue_id}'],
+                    label= f'Queue {queue_id}',
+                    color= self.colors[marker]
+                
+                )
+                # -------------------------------------------------
+
+                #--- Increase marker for the next
+                marker += 1
+        if stacked == True:
+            #--- creator matrix with queue occupation
+            stacked_vector = []
+            labels = []
+            for key in queue_occupation:
+                stacked_vector.append(queue_occupation[key])
+                labels.append(key)
+
+            plt.stackplot(
+                x_vector,
+                stacked_vector,
+                labels= labels
+            )
+
+        #--- Add complements
+        self.ADD_complemts(
+            title= "Queues Occupation",
+            xlable= "Number of Sync",
+            ylable= "Parts in Queue"
+        )
+
+        #--- Save
+        if self.save:
+            self.save_fig("Queues_Occupation")
+
+        #--- Show
+        if self.show:
+            plt.show()
+
+        # --------------------- COMPARE QUEUE 3 AND QUEUE 4 ---------------------
+        #---------
+        plt.clf()
+        #---------
+
+        marker = 2
+        if stacked == False:
+            for i in range(2, 4): 
+                #-- Create Queue ID
+                queue_id= i + 1
+
+                #--- reset markers
+                if marker > len(self.markers): marker = 0
+
+                # ------------------ PLOT ----------------------
+                plt.step(
+                    x_vector, 
+                    queue_occupation[f'Queue {queue_id}'],
+                    label= f'Queue {queue_id}',
+                    color= self.colors[marker]
+                )
+                # -------------------------------------------------
+
+                #--- Increase marker for the next
+                marker += 1
+        if stacked == True:
+            #--- creator matrix with queue occupation
+            stacked_vector = [queue_occupation['Queue 3'], queue_occupation['Queue 4']]
+            labels = ['Queue 3', 'Queue 4']
+
+            plt.stackplot(
+                x_vector,
+                queue_occupation['Queue 3'],
+                queue_occupation['Queue 4'],
+                labels= labels
+            )
+
+
+        #--- Add complements
+        self.ADD_complemts(
+            title= "Queue 3 x Queue 4",
+            xlable= "Number of Sync",
+            ylable= "Parts in Queue"
+        )
+
+        #--- Save
+        if self.save:
+            self.save_fig("Queues_Occupation_3_4")
+
+        #--- Show
+        if self.show:
+            plt.show()
+
+    def plot_comparative_parts_CT(self):
+        """
+        This function take the total time of a simulation from the table results and
+        with that runs a simulation using the digital model from the Digital Twin. Extracting
+        the cycle of each part from the results and from the digital simulation it's possible
+        to plot for each part.
+
+        IMPORTANT: Don't use this funtion in a system were the RCT was publishing the decisions,
+        because than running a normal simulation would not have the right policy
+        """
+        #---------
+        plt.clf()
+        #---------
+
+        # --------------------- PHYSICAL TWIN ------------------------------
+        #--- Get the total time of simulation from the results table
+        total_time = self.exp_database.get_global_result('run_time')
+
+        #--- Get the list of finished parts and CT from the results table
+        str_parts_vector_real = self.exp_database.get_global_result('List_parts_finished')
+        str_CT_vector_real = self.exp_database.get_global_result('CT_parts')
+
+        #-- Convert string vector into a list vector
+        list_parts_vector_real = self.helper.convert_stringVect_to_listVect(str_parts_vector_real)
+        list_CT_vector_real = self.helper.convert_stringVect_to_listVect(str_CT_vector_real)
+
+        #-- Get only parts id
+        for i in range(len(list_parts_vector_real)): list_parts_vector_real[i] = self.helper.extract_int(list_parts_vector_real[i])
+        
+        #-------------------------------------------------------------------
+
+        #------------- RUN DIGITAL SIMULATION -----------
+        digital_model = self.plotterDT.generate_digital_model(until= total_time)
+        digital_model.run()
+        #------------------------------------------------
+
+        #--- Get finished parts and cycle from digital model
+        (list_parts_vector_digital, list_CT_vector_digital) = digital_model.get_parts_CT_ordered()
+        
+        #--- Excludes Extra Parts
+        if len(list_CT_vector_digital) > len(list_CT_vector_real):
+            extra_parts = len(list_CT_vector_digital) - len(list_CT_vector_real)
+            for i in range(extra_parts): 
+                list_CT_vector_digital.pop()
+                list_parts_vector_digital.pop()
+
+        if len(list_CT_vector_real) > len(list_CT_vector_digital):
+            extra_parts = len(list_CT_vector_real) - len(list_CT_vector_digital)
+            for i in range(extra_parts): 
+                list_CT_vector_real.pop()
+                list_parts_vector_real.pop()
+
+
+
+
+        # ----- PLOT real Parts-CTs -----
+        plt.plot(
+            list_parts_vector_real,
+            list_CT_vector_real,
+            marker='o',
+            label= 'Physical Twin'
+        )
+        # --------------------------------
+
+        # ----- PLOT digital Parts-CTs -----
+        plt.plot(
+            list_parts_vector_digital,
+            list_CT_vector_digital,
+            marker='o',
+            label= 'Digital Twin'
+        )
+        # --------------------------------
+
+        #--- Add complements
+        self.ADD_complemts(
+            title= "Part-CT Phsycial x Digital",
+            xlable= "Parts ID",
+            ylable= "Cycle Time"
+        )
+
+
+        #--- Save
+        if self.save:
+            self.save_fig("Part-CT")
+
+        #--- Show
+        if self.show:
+            plt.show()
+
+        # ------------------------- ERROR PLOT -------------------------
+        #---------
+        plt.clf()
+        #---------
+
+        #--- Calculates the common len
+        len_digital = len(list_CT_vector_digital)
+        len_real = len(list_CT_vector_real)
+        common_len = min(len_digital, len_real)
+
+        #--- Creates a error vector
+        error_vector = []
+        error_vector_relative = []
+        error_parts = []
+
+        #--- Fullfil the error vector
+        for i in range(common_len):
+            #-- Add the parts id
+            error_parts.append(list_parts_vector_real[i])
+
+            #-- Calculates the error
+            error = abs(list_CT_vector_digital[i] - list_CT_vector_real[i])
+            error_vector.append(error)
+
+            #-- Error Relative
+            error_relative = error / list_CT_vector_real[i]
+            error_vector_relative.append(error_relative)
+            
+
+        
+        # ---------- PLOT ERROR EVOLUTION ----------
+        fig, ax1 = plt.subplots()
+
+        ax1.plot(
+            error_parts,
+            error_vector,
+            marker='o',
+            label= 'Raw Error'
+        )
+
+        ax1.set_xlabel('Part IDs')
+        ax1.set_ylabel('Raw error')
+        ax1.set_title("Raw Error between phsyical and digital system")
+
+        #--- Save
+        if self.save:
+            self.save_fig("ERROR_CT_raw")
+
+        #--- Show
+        if self.show:
+            plt.show()
+
+
+        # create the second axis
+        #ax2 = ax1.twinx()
+        fig, ax2 = plt.subplots()
+
+        ax2.plot(
+            error_parts, 
+            error_vector_relative, 
+            marker='^',
+            label= "Percentage Error",
+            color= 'red'
+        )
+        ax2.set_ylabel('Percentage of error')
+        ax2.set_title("Relative Error between phsyical and digital system")
+
+
+        # add a legend
+        ax1.legend(['Raw error'], loc='upper left')
+        ax2.legend(['Percentage of error'], loc='upper right')
+
+
+        #--- Save
+        if self.save:
+            self.save_fig("ERROR_CT_rel")
+
+        #--- Show
+        if self.show:
+            plt.show()
+
+        # ---------- PLOT ERROR BAR EVOLUTION ----------
+        #---------
+        plt.clf()
+        #---------
+
+        plt.plot(
+            list_parts_vector_digital,
+            list_CT_vector_digital,
+            marker='o',
+            label= 'ERROR Bar'
+        )
+
+        plt.errorbar(list_parts_vector_digital, list_CT_vector_digital, yerr=error_vector, linestyle='None', capsize=5, color='orange')
+
+        #--- Add complements
+        self.ADD_complemts(
+            title= "Error BAR between Phsycial x Digital",
+            xlable= "Parts ID",
+            ylable= "Cycle Time"
+        )
+
+        #--- Save
+        if self.save:
+            self.save_fig("Part_CT_error_bar")
+
+        #--- Show
+        if self.show:
+            plt.show()
+        
+    def plot_comparative_RCT(self):
+        """
+        This function calculates the RCT for all the parts in the perspective of machine 2.
+        In this way is possible to compare with the predicted RCT from the Digital Twin with
+        the actual path that the part took.
+        """
+
+        #--- Get the Real RCT and the predicted RCT (for both path) from the real log
+        (parts_name_finished_vec, RCT_real, RCT_path1_vec, RCT_path2_vec) = self.exp_database.get_real_RCT(self.real_database_path)
+        
+        #--- Convert the list of parts names in integers ids
+        parts_finished_ids_vec = []
+        for part_name in parts_name_finished_vec: parts_finished_ids_vec.append(self.helper.extract_int(part_name))
+                
+        #---------
+        plt.clf()
+        #---------
+        linestyle= 'dashdot'
+        #--- Plot REAL RCT for each finished part
+        plt.plot(
+            parts_finished_ids_vec, 
+            RCT_real, 
+            marker='o',
+            linestyle= linestyle,
+            label= 'Physical RCT'
+        )
+
+        #--- Plot Predicted RCT Path 1 RCT for each finished part
+        plt.plot(
+            parts_finished_ids_vec, 
+            RCT_path1_vec, 
+            marker='o',
+            linestyle= linestyle,
+            label= 'Predicted RCT Path 1 (Queue 3)'
+        )
+
+        #--- Plot Predicted RCT Path 2 RCT for each finished part
+        plt.plot(
+            parts_finished_ids_vec, 
+            RCT_path2_vec, 
+            marker='o',
+            linestyle= linestyle,
+            label= 'Predicted RCT Path 2 (Queue 4)'
+        )
+
+        #--- Add complements
+        self.ADD_complemts(
+            title= "Comparing Real RCT with DT predictions",
+            xlable= "Parts IDs",
+            ylable= "RCT"
+        )
+        
+        #--- Save
+        if self.save:
+            self.save_fig("Real_RCT")
+
+        #--- Show
+        if self.show:
+            plt.show()
+
+    def plot_utilization(self, utilization_dict):
+        plt.clf()
+        linestyle = "dotted"
+        # ----------- PLOT OF ALL MACHINES TOEGETHER -----------
+        for key_name in utilization_dict:
+            #--- Create the x vector
+            intervals_x= []
+            for i in range(len(utilization_dict[key_name])): intervals_x.append(i+1)
+
+            #--- Plot for that machine
+            plt.plot(
+                intervals_x,
+                utilization_dict[key_name],
+                marker='o',
+                linestyle= linestyle,
+                label= key_name
+            )
+
+            #--- Add complements
+            self.ADD_complemts(
+                title= "Cumulative Utilization",
+                xlable= "intervals (secs)",
+                ylable= "Utilization (%)"
+            )
+        
+        #--- Save
+        if self.save:
+            self.save_fig("global_utilization")
+
+        #--- Show
+        if self.show:
+            plt.show()
+
+        # ----------- PLOT Machine 3 x 4 -----------
+        
+        plt.clf()
+        #--- Create the x vector
+        intervals_x= []
+        for i in range(len(utilization_dict['Machine 3'])): intervals_x.append(i+1)
+
+        #--- Plot for that machine
+        plt.plot(
+            intervals_x,
+            utilization_dict['Machine 3'],
+            marker='o',
+            linestyle= linestyle,
+            label= 'Machine 3'
+        )
+        # -----------------------------------------
+
+        #--- Create the x vector
+        intervals_x= []
+        for i in range(len(utilization_dict['Machine 4'])): intervals_x.append(i+1)
+
+        #--- Plot for that machine
+        plt.plot(
+            intervals_x,
+            utilization_dict['Machine 4'],
+            marker='o',
+            linestyle= linestyle,
+            label= 'Machine 4'
+        )
+
+        #--- Add complements
+        self.ADD_complemts(
+            title= "Cumulative Utilization between Machine 3 and 4",
+            xlable= "intervals (secs)",
+            ylable= "Utilization (%)"
+        )
+        
+        #--- Save
+        if self.save:
+            self.save_fig("utilization_3_4")
+
+        #--- Show
+        if self.show:
+            plt.show()
+
+    def plot_RCTtracking(self):
+        """
+        This function plot the comparation between RCT evolution of a specific part tracked by
+        the Digital Twin and by the Real System.
+        """
+
+        #--- Get the distinc (unique) PIDs calculates by the Digital Twin
+        PIDs_tracked = self.exp_database.get_distinct_values('PID', 'RCTtracking')
+
+        #--- For every PIDs tracked
+        for PID in PIDs_tracked:
+            #---------
+            plt.clf()
+            #---------
+             
+            PID = f'Part {PID[0]}'
+            #--- Take the REAL RCT and timestamp for that PID
+            (rct_real, timestamp_real, flag_part_completed) = self.exp_database.get_real_RCTtracking(self.real_database_path, PID)
+            
+            if flag_part_completed == True:
+                timestamp_real = self.helper.adjust_relative_vector(timestamp_real)
+
+                #--- Take the DIGITAL RCT and timestamp for that PID
+                (rct_digital, timestamp_digital) = self.exp_database.get_digital_RCTtracking(PID)
+                timestamp_digital = self.helper.adjust_relative_vector(timestamp_digital)
+
+                #--- PLOT RCT real
+                plt.plot(
+                    timestamp_real,
+                    rct_real,
+                    marker='o',
+                    label= f'[{PID}] RCT Real'
+                )
+
+                #--- PLOT RCT digital
+                plt.plot(
+                timestamp_digital,
+                rct_digital,
+                marker='o',
+                linestyle= 'dashdot',
+                label= f'[{PID}] RCT Digital'
+            )
+
+                #--- Add complements
+                self.ADD_complemts(
+                    title= "RCT Tracking",
+                    xlable= "Relative Timestamp (s)",
+                    ylable= "RCT (s)"
+                )
+                
+                #--- Save
+                if self.save:
+                    self.save_fig(f"tracking/rct_tracking_{PID}")
+
+                #--- Show
+                if self.show:
+                    plt.show()
 
-    #--- get objective
```

## dtwinpy/updator.py

```diff
@@ -166,14 +166,24 @@
                     machine_trace.append(processed_time)
 
                     #--- reset local started and finished time for the next cycle
                     started_time = None
                     finished_time = None
                     processed_time = None
 
+                #--- ISSUE #263: In case when the first event is a finished...
+                # Previous we were considering that as the process time, because of the worked time
+                # but since now in the update we don't consider the worked time, we can't not carry
+                # this finish trace for the next event, so reset everything...
+                if finished_time != None and started_time == None:
+                    #--- reset local started and finished time for the next cycle
+                    started_time = None
+                    finished_time = None
+                    processed_time = None
+
                 """
                 #--- In the case of part that already was in the machine (worked_time)
                 if finished_time != None and started_time == None:
                     processed_time = finished_time
 
                     #--- Add event process time to the part trace
                     machine_trace.append(processed_time)
@@ -278,20 +288,25 @@
 
                 #--- System Deterministic: Take just the mean value
                 if flag_deterministic:
                     #--- Take the new process time (last position, mean)
                     new_process_time = update_result[-1]
                     new_process_time = round(new_process_time)
 
+                    if new_process_time < 0:
+                        self.helper.printer(f"[ERROR][updator.py/run()] New Process Time calculated is negative for {machine_name}!", 'red')
+                        self.helper.printer(f"Machine Trace: {machine_trace}")
+                        self.helper.kill()
                 #--- System not Deterministic: Take the distribution parameters
                 if not flag_deterministic:
                     #--- Take the whole parameters
                     dist_name = update_result[0]
-                    parameter_a = update_result[1]
-                    parameter_b = update_result[2]
+                    parameter_a = round(update_result[1][0])
+                    parameter_b = round(update_result[1][1])
+                    if parameter_b == 0: parameter_b= 1
 
                     (new_process_time) = [dist_name, parameter_a, parameter_b]
 
 
                 #--- Write the new process time in the json model
                 self.aligner(machine_id, new_process_time)
```

## dtwinpy/validator.py

```diff
@@ -13,16 +13,17 @@
 """import importlib
 import dtwinpylib
 #reload this specifc module to upadte the class
 importlib.reload(dtwinpylib.dtwinpy.interfaceDB)"""
 
 
 class Validator():
-    def __init__(self, digital_model, simtype, real_database_path, start_time, end_time, generate_digital_model, id_database_path= False,copied_realDB= False, delta_t_treshold= 100):
+    def __init__(self, digital_model, simtype, real_database_path, start_time, end_time, generate_digital_model, id_database_path= False,copied_realDB= False, delta_t_treshold= 100, plot= False):
         self.helper = Helper()
+        self.plot = plot
         self.digital_model = digital_model
         self.generate_digital_model= generate_digital_model
         self.simtype = simtype
         self.delta_t_treshold = delta_t_treshold
         # qTDS: each row is the list of process time for each part
         self.matrix_ptime_qTDS = None 
         # TDS: each row is the list of process time for each machine
@@ -287,16 +288,18 @@
     # ==================== QUASI TRACE DRIVEN SIMULATION ====================
 
     #--- Initial Setup of qTDS
     def set_qTDS(self):
         #--- Update each existing machine in the model
 
         #--- Extract the unique parts IDs from the real log
-        machines_ids = self.real_database.get_distinct_values(column= "machine_id", table="real_log")
-        
+        # [OLD] machines_ids = self.real_database.get_distinct_values(column= "machine_id", table="real_log")
+        machines_ids = self.real_database.get_machines_with_completed_traces()
+
+
         # For every machine that was USED in the real world
         # We iterate the within the machines id because it's possible that
         # the simulation has more machines rather than the real log, because
         # one of the machines in the real world was not chosen.
         for machine_id in machines_ids:
             
             # For this machine_id, find the machine object with the same id
@@ -347,37 +350,48 @@
             for event in machine_full_trace:
                 #--- Extract the Started and Finished time
                 if event[1] == 'Started':
                     started_time = event[0]
                 elif event[1] == 'Finished':
                     finished_time = event[0]
                 
+
                 #--- Calculate the process time
                 if started_time != None and finished_time != None:
                     processed_time = finished_time - started_time
 
                     #--- Add event process time to the machine trace
                     machine_trace.append(processed_time)
 
                     #--- reset local started and finished time for the next cycle
                     started_time = None
                     finished_time = None
                     processed_time = None
 
+                
+                if finished_time != None and started_time == None:
+                    #--- reset local started and finished time for the next cycle
+                    started_time = None
+                    finished_time = None
+                    processed_time = None
+
+
+                """
                 #--- In the case of part that already was in the machine (worked_time)
                 if finished_time != None and started_time == None:
                     processed_time = finished_time
 
                     #--- Add event process time to the part trace
                     machine_trace.append(processed_time)
 
                     #--- reset local started and finished time for the next cycle
                     started_time = None
                     finished_time = None
                     processed_time = None
+                """
             
             #--- Add machine trace to the matrix of all machines traces
             matrix_ptime_qTDS[machine_id[0]] = (machine_trace)
             
         #--- Return the matrix of traces
         return matrix_ptime_qTDS
 
@@ -415,17 +429,36 @@
                     u.append(ecdf_value)
 
 
             # print(len(ecdf))
             for i in range(len(u)):
                 if u[i] == 1.0:
                     pos_one = i
+                    try:
+                        u[pos_one]=umax # change 1 to 0.99 to avoid infinity in dist.ppf function
+                        return(u,pos_one)
+                    except UnboundLocalError:
+                        self.helper.printer(f"[ERROR][validator.py/generate_Xs_machine()] 'pos_one not defined. Checking if the U is correct", 'red')
+                        print(f"U: {u}")
+                        self.helper.kill()
+                    break
+            else:
+                self.helper.printer("[WARNING][validator.py/generate_Xs_machine()] value 1 not found in 'u' variable")
+                print(f"u: {u}")
+                print("Printing input parameters...")
+                print(f"loc = {loc}")
+                print(f"scale = {scale}")
+                print(f"distribution= {distribution}")
+                print(f"Xr = {Xr}")
+
+                return(u,[])
             #pos_one = np.where(u == 1.0)
-            u[pos_one]=umax # change 1 to 0.99 to avoid infinity in dist.ppf function
-            return(u,pos_one)
+            
+            
+            
 
         # -----------------------------------------------------
         # Function for Generating dedicated disrtibutions
         # -----------------------------------------------------
         # we mention the number of parameters used to define the distribution as N_Parameter
 
         # Importing required library from SciPy
@@ -466,14 +499,15 @@
         Xs=np.array([])
         diff=np.zeros(901)
         diff[900]=np.inf
         umax=np.zeros(900)
         sse=np.zeros(900)
 
         # Deriving randomness from Xr and generating Xs
+        
         for ii in range(899,498,-1):
             umax[ii]=0.91+(ii*0.0001)
             Xsf=Xs
 
             if N_Parameter==2:  # for distributions with 2 parameters
                 u,pos_one = randomness(ECDF(Xr),umax[ii],Xr) # calculate inverse transform of ecdf.
                 Xs = (dist.ppf(u, loc, scale))    # generate distribution Xs.
@@ -482,26 +516,42 @@
                 u,pos_one = randomness(ECDF(Xr),umax[ii],Xr) # calculate inverse transform of ecdf.
                 Xs = (dist.ppf(u, a, loc, scale))    # generate distribution Xs.
 
             if N_Parameter==4:  # for distributions with 4 parameters
                 u,pos_one = randomness(ECDF(Xr),umax[ii],Xr) # calculate inverse transform of ecdf.
                 Xs = (dist.ppf(u, a, b, loc, scale))    # generate distribution Xs.
 
-            diff[ii]=abs(Xs[pos_one]-Xr[pos_one])   # Calculate error in the highest value due to impact of umax
-            #sse[ii]=np.sum(np.square(Xr-Xs))
-            
-            if diff[ii]>diff[ii+1]:
-                Xs=Xsf
+            if pos_one != []:
+                diff[ii]=abs(Xs[pos_one]-Xr[pos_one])   # Calculate error in the highest value due to impact of umax
+                #sse[ii]=np.sum(np.square(Xr-Xs))
+                if diff[ii]>diff[ii+1]:
+                    Xs=Xsf
+                    break
+            else:
+                
                 break
-
-        i=range(1,len(Xr)+1)
-        plt.plot(i,Xr,color='blue')
-        plt.plot(i,Xs,color='red')
-        plt.show()
         
+        if self.plot == True:
+            i=range(1,len(Xr)+1)
+            plt.plot(i,Xr,color='blue')
+            plt.plot(i,Xs,color='red')
+            plt.show()
+
+        if Xs[0] != int or Xs[0] != float:
+            self.helper.printer(f"[WARNING][validator.py/generate_Xs_machine()] The Xs vector is not a made by numbers! Check the U vector:")
+            print(f"u: {u}")
+            print("|--- Printing input parameters...")
+            print(f"loc = {loc}")
+            print(f"scale = {scale}")
+            print(f"distribution= {distribution}")
+            print(f"Xr = {Xr}")
+            print("|--- Printing output")
+            print(f"Xs= {Xs}")
+
+
         return(Xs)
     # =======================================================================
 
     # ======================== Sequence Generator ========================
     def generate_event_sequence(self, database, table):
         #--- Extract all the events from the table and store each in tuple
         events_full_trace = database.read_store_data(table)
@@ -604,15 +654,18 @@
         # ---------------- qTDS ----------------
         #--generate Xr of real log for all the machines (matrix)
         Xr_matrix = self.generate_qTDS_traces()
         self.matrix_ptime_qTDS = {}
         
         #--- Loop to correlated each Xs with Xr
         # The loop can also be seem as loop through the machines
-        machines_ids = self.real_database.get_distinct_values(column= "machine_id", table="real_log")
+        # [OLD] machines_ids = self.real_database.get_distinct_values(column= "machine_id", table="real_log")
+        # ------- GET MACHINES IDs ONLY OF COMPLETED TRACE (START -> FINISH) -------
+        machines_ids = self.real_database.get_machines_with_completed_traces()
+        
         for machine_id in machines_ids:
             
             # For this machine_id, find the machine object with the same id
             for i in range(len(self.machines_vector)):
                 if machine_id[0] == self.machines_vector[i].get_name():
                     machine = self.machines_vector[i]
                     
@@ -620,18 +673,21 @@
                     machine_process_time = machine.get_process_time()
                     if type(machine_process_time) == list:
                         dist = machine_process_time[0]
                         loc = machine_process_time[1]
                         scale = machine_process_time[2]
 
                         Xr_vector = Xr_matrix[machine.get_name()]
-                        print(Xr_vector)
+                        print(f"machine name: {machine.get_name()}")
+                        print(f"Xr_vector: {Xr_vector}")
 
                         Xs_vector = self.generate_Xs_machine(loc= loc, scale= scale, distribution= dist, Xr= Xr_vector)
                         self.matrix_ptime_qTDS[machine.get_name()] = (Xs_vector)
+                        
+                        break
                     
                     else:
                         #--- WRONG!!! This bellow implementation is wrong. The goal here is not to copy and paste
                         # the process time from the real into the digital machines. We're using it just to get the
                         # the randmness to generate new data using the current distribution parameters of the digital
                         # machines... But in the case that it's deterministic (not a list) we can't just copy from the real!
                         # we need just to run the simulation and compare the final sequences....
```

## Comparing `dtwinpy-0.0.3.9.dist-info/RECORD` & `dtwinpy-0.1.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-dtwinpy/Digital_Twin.py,sha256=LPo92jz0xNeSMCN2eAMM9KYjnnvBE62t3OrDVORMB7w,39744
+dtwinpy/Digital_Twin.py,sha256=_2XnHdjvQKCvl4AbO-vJTFLtEClnxEmUJrwnCvFOHOo,40171
 dtwinpy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dtwinpy/broker_manager.py,sha256=Oru3NzfUU92Vqkf1YTbUxJkunsEnNsiVgH8irnELik4,23151
-dtwinpy/components.py,sha256=c2X1UskhX0EjC8PUxKpyA-Ykn_tM1DZggSm_MdCmMuk,54424
-dtwinpy/digital_model.py,sha256=KtFvAi9cqdIJtk40Nx-Su0SI7bciCQz9f26Zw8uDrTU,46557
-dtwinpy/helper.py,sha256=Y7hHTI2F-XgueyAzoGgzCIs6MQ_QCdbqgMuYhaOuEr8,8049
+dtwinpy/broker_manager.py,sha256=gK6yu8WXAs_xxeY0_G7UeOIbLRVDte2osKnCyLt8zDk,23407
+dtwinpy/components.py,sha256=w2DPXXh38LkVVBEYuth66bv5rQGtMN0XSs-F985rnzI,54494
+dtwinpy/digital_model.py,sha256=rfQEjjmlPyBzvZ9Gtp5MS1uxinTby8FjQeNFmThGEAI,48951
+dtwinpy/helper.py,sha256=YJtkbYr3BBsVeOWpypFv1Izw93-XmWVAC-IsOsS9q6M,9075
 dtwinpy/interfaceAPI.py,sha256=5vwn18a5fEkQA0n-eELoO0rSrXsVqaMQKGAN96Ztyvg,11063
-dtwinpy/interfaceDB.py,sha256=J7bkDVKgOByrjApadjdvzLjOZXqdZC8ko-HwS5f98Vw,47352
-dtwinpy/services.py,sha256=TkFNBlCpHZAWvrA_3dPKAg6vihnzy31f9Ahbf45VNMU,36842
-dtwinpy/synchronizer.py,sha256=Dejnl_hFtNm2j2letMMA42rc3VlOh_VOxus4huG5q-Y,33354
-dtwinpy/tester.py,sha256=wDkCv_lIB-IzDUjm4Vv31VpqWQCCw3qdrIpUukVcNTM,22342
-dtwinpy/updator.py,sha256=hRtAtxGVcEW7yM6Oega4Vlhkfj32xOR47QuQ_i3Su58,13021
-dtwinpy/validator.py,sha256=RxBdrAvnk5jS2Eb_ytcxed-HyIibzubwNFCADm37mWk,35858
-dtwinpy-0.0.3.9.dist-info/METADATA,sha256=TE0WSRdi2JXAFgbWFp9IxPcOyE3t6yZzflNUVXqnPLI,140
-dtwinpy-0.0.3.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-dtwinpy-0.0.3.9.dist-info/top_level.txt,sha256=f4_zsiQfNu0yhjVqRRYagp-Oh9G3TAyj6AWUYDsDcR4,8
-dtwinpy-0.0.3.9.dist-info/RECORD,,
+dtwinpy/interfaceDB.py,sha256=YhmexsCVKRXMy7Q-Ok8f1z15rcG82_xzEkDONfleoBs,58461
+dtwinpy/services.py,sha256=Gxb7HjPYZqzDZjvZWtmtM6JcUYVI4gyMdy95DCOelcY,39752
+dtwinpy/synchronizer.py,sha256=BCXpGt33qlK2t9dwSNUa9fMhHB0X8THyhKHyGuFVEHw,35637
+dtwinpy/tester.py,sha256=NX0cXERqgFS0nGx-X60ZJaPOJiIcF7cujLmWcfNrqHU,68985
+dtwinpy/updator.py,sha256=E3imNHsb9DBbEQg_4idv88RhRiCVIyHKYTVb6gysXq8,14051
+dtwinpy/validator.py,sha256=p8wZDBPc4IXTzEF2EQBa5uypmCv9aK-Nz9bWh_B8e1A,38152
+dtwinpy-0.1.0.dist-info/METADATA,sha256=aSkwGrPqm06aaw5BdbwWAykoIPpO_wLEhAM7Xcd677w,132
+dtwinpy-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+dtwinpy-0.1.0.dist-info/top_level.txt,sha256=f4_zsiQfNu0yhjVqRRYagp-Oh9G3TAyj6AWUYDsDcR4,8
+dtwinpy-0.1.0.dist-info/RECORD,,
```

