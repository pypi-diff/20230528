# Comparing `tmp/cobra_db-0.2.4.tar.gz` & `tmp/cobra_db-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobra_db-0.2.4.tar", max compression
+gzip compressed data, was "cobra_db-0.3.8.tar", max compression
```

## Comparing `cobra_db-0.2.4.tar` & `cobra_db-0.3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0      609 2023-04-14 11:52:48.232131 cobra_db-0.2.4/LICENSE
--rw-r--r--   0        0        0     3540 2023-04-14 11:52:48.232131 cobra_db-0.2.4/README.md
--rw-r--r--   0        0        0     1813 2023-04-14 11:53:31.316266 cobra_db-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      332 2023-04-14 11:52:48.248131 cobra_db-0.2.4/src/cobra_db/__init__.py
--rw-r--r--   0        0        0     2160 2023-04-14 11:52:48.248131 cobra_db-0.2.4/src/cobra_db/dataset_mod.py
--rw-r--r--   0        0        0     4177 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/deid.py
--rw-r--r--   0        0        0    18585 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/deid_recipe.txt
--rw-r--r--   0        0        0     2382 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/deid_recipe_mr.txt
--rw-r--r--   0        0        0     4423 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/encrypt.py
--rw-r--r--   0        0        0     4603 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/enums.py
--rw-r--r--   0        0        0     2266 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/filesystem.py
--rw-r--r--   0        0        0    17338 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/model.py
--rw-r--r--   0        0        0    19218 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/mongo_dao.py
--rw-r--r--   0        0        0        0 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/__init__.py
--rw-r--r--   0        0        0     9731 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/pseudonymize_image_metadata.py
--rw-r--r--   0        0        0    13064 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_1_ingest_images.py
--rw-r--r--   0        0        0     2508 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_2.py
--rw-r--r--   0        0        0     2397 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_patients.py
--rw-r--r--   0        0        0     4709 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_series.py
--rw-r--r--   0        0        0     5058 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_studies.py
--rw-r--r--   0        0        0     1042 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/utils.py
--rw-r--r--   0        0        0      535 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/types.py
--rw-r--r--   0        0        0     4635 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/utils.py
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 cobra_db-0.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0      609 2022-08-25 09:24:06.242378 cobra_db-0.3.8/LICENSE
+-rw-r--r--   0        0        0     3540 2023-05-23 08:22:03.656463 cobra_db-0.3.8/README.md
+-rw-r--r--   0        0        0     1846 2023-05-28 10:55:15.766056 cobra_db-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      332 2022-08-26 14:33:49.499529 cobra_db-0.3.8/src/cobra_db/__init__.py
+-rw-r--r--   0        0        0     2160 2022-08-25 10:25:47.249683 cobra_db-0.3.8/src/cobra_db/dataset_mod.py
+-rw-r--r--   0        0        0     4849 2023-05-27 06:45:18.857910 cobra_db-0.3.8/src/cobra_db/deid.py
+-rw-r--r--   0        0        0    19064 2023-05-27 06:45:18.858208 cobra_db-0.3.8/src/cobra_db/deid_recipe.txt
+-rw-r--r--   0        0        0     2382 2023-02-09 15:28:28.969845 cobra_db-0.3.8/src/cobra_db/deid_recipe_mr.txt
+-rw-r--r--   0        0        0     4423 2023-05-23 08:22:03.657525 cobra_db-0.3.8/src/cobra_db/encrypt.py
+-rw-r--r--   0        0        0     4603 2022-09-22 19:04:29.847121 cobra_db-0.3.8/src/cobra_db/enums.py
+-rw-r--r--   0        0        0     2266 2023-02-16 16:28:15.413447 cobra_db-0.3.8/src/cobra_db/filesystem.py
+-rw-r--r--   0        0        0    17338 2023-05-23 08:22:03.658032 cobra_db-0.3.8/src/cobra_db/model.py
+-rw-r--r--   0        0        0    19451 2023-05-23 08:22:03.658390 cobra_db-0.3.8/src/cobra_db/mongo_dao.py
+-rw-r--r--   0        0        0        0 2022-09-20 13:32:34.744297 cobra_db-0.3.8/src/cobra_db/scripts/__init__.py
+-rw-r--r--   0        0        0    10333 2023-05-23 09:13:53.676827 cobra_db-0.3.8/src/cobra_db/scripts/pseudonymize_image_metadata.py
+-rw-r--r--   0        0        0    13064 2022-11-15 12:38:50.520888 cobra_db-0.3.8/src/cobra_db/scripts/stage_1_ingest_images.py
+-rw-r--r--   0        0        0     2508 2022-09-22 11:58:01.231405 cobra_db-0.3.8/src/cobra_db/scripts/stage_2.py
+-rw-r--r--   0        0        0     2397 2022-09-22 11:38:28.493491 cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_patients.py
+-rw-r--r--   0        0        0     4709 2022-09-21 16:52:48.434815 cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_series.py
+-rw-r--r--   0        0        0     5058 2023-05-23 08:22:03.658713 cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_studies.py
+-rw-r--r--   0        0        0     1042 2022-09-20 13:32:34.746137 cobra_db-0.3.8/src/cobra_db/scripts/utils.py
+-rw-r--r--   0        0        0      535 2022-08-25 10:25:47.234583 cobra_db-0.3.8/src/cobra_db/types.py
+-rw-r--r--   0        0        0     4635 2022-10-20 08:57:54.475224 cobra_db-0.3.8/src/cobra_db/utils.py
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 cobra_db-0.3.8/PKG-INFO
```

### Comparing `cobra_db-0.2.4/LICENSE` & `cobra_db-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/README.md` & `cobra_db-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/pyproject.toml` & `cobra_db-0.3.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cobra_db"
-version = "0.2.4"
+version = "0.3.8"
 description = "COnsolidated BReast cancer Analysis DataBase"
 authors = ["Fernando Cossio", "Apostolia Tsirikoglou", "Haiko Schurz", "Hui Li", "Fredrik Strand"]
 license = "Apache License 2.0"
 readme = "README.md"
 include = ["src/cobra_db/deid_recipe.txt"]
 
 [tool.poetry.dependencies]
@@ -14,28 +14,29 @@
 dnspython = "^2.2.1"
 pymongo = {extras = ["srv"], version = "^4.2.0"}
 tqdm = "^4.64.1"
 deid = "^0.2.36"
 pycryptodome = "^3.15.0"
 pyaml-env = "^1.1.5"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pre-commit = "^2.20.0"
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^5.0.4"
 Sphinx = "^5.1.1"
 sphinx-autoapi = "^1.9.0"
 sphinx-rtd-theme = "^1.0.0"
 myst-nb = {version = "^0.16.0", python = "^3.9"}
 python-semantic-release = "^7.31.4"
 pytest-mongodb = "^2.2.0"
 python-dotenv = "^0.21.0"
+dicom-validator = "^0.3.4"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version" # version location
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build dists
 dist_path = "dist/"                         # where to put dists
```

### Comparing `cobra_db-0.2.4/src/cobra_db/dataset_mod.py` & `cobra_db-0.3.8/src/cobra_db/dataset_mod.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/deid.py` & `cobra_db-0.3.8/src/cobra_db/deid.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pydicom
 from deid.config import DeidRecipe
 from deid.dicom.parser import DicomParser
 from deid.logger import bot
 
 from cobra_db.encrypt import Hasher
-from cobra_db.utils import parse_AS_as_int
+from cobra_db.utils import parse_AS_as_int, parse_DA_TM_as_datetime
 
 base_recipe_path = os.path.join(os.path.dirname(__file__), "deid_recipe.txt")
 mr_recipe_path = os.path.join(os.path.dirname(__file__), "deid_recipe_mr.txt")
 
 deid_logging_levels = dict(
     ABORT=-5,
     FLAG=-4,
@@ -65,15 +65,15 @@
         parser = DicomParser(dataset, self.recipe)
         parser.define("replace_name", self._replace_name)
         parser.define("hash_func", self._deid_hash_func)
         parser.define("remove_day", self._remove_day)
         parser.define("round_AS_to_nearest_5y", self._round_AS_to_nearest_5y)
         parser.define("round_DS_to_nearest_5", self._round_DS_to_nearest_5)
         parser.define("round_DS_to_nearest_0_05", self._round_DS_to_nearest_0_05)
-        parser.parse(strip_sequences=True, remove_private=True)
+        parser.parse(strip_sequences=False, remove_private=True)
         return parser.dicom
 
     @staticmethod
     def _remove_day(item, value, field, dicom):
         """Removes the day from a DT field in the deid framework"""
         date = field.element.value
         if date == "":
@@ -92,21 +92,36 @@
     def _round_to_nearest(value, interval):
         """Rounds value to closest multiple of interval"""
         return interval * round(value / interval)
 
     @staticmethod
     def _round_AS_to_nearest_5y(item, value, field, dicom):
         """Rounds age(AS) field to 5 year intervals in the deid framework"""
-        age = parse_AS_as_int(field.element.value)
+        value = field.element.value
+        # if age is empty, try to calculate it from the StudyDate and PatientBirthDate
+        if value == '' or value == None:
+            try:
+                study_date = dicom.get('StudyDate')
+                study_date = parse_DA_TM_as_datetime(DA=study_date, TM='000000')
+                birth_date = dicom.get('PatientBirthDate')
+                birth_date = parse_DA_TM_as_datetime(DA=birth_date, TM='000000')
+                age = (study_date - birth_date).days/365
+            except:
+                return ''
+        else:
+            age = parse_AS_as_int(field.element.value)
         return f"{Deider._round_to_nearest(age, 5):03d}Y"
 
     @staticmethod
     def _round_DS_to_nearest_5(item, value, field, dicom):
         """Rounds age(AS) field to 5 year intervals in the deid framework"""
-        return f"{Deider._round_to_nearest(float(field.element.value), 5)}"
+        value = field.element.value
+        if value is None:
+            value = -1
+        return f"{Deider._round_to_nearest(float(value), 5)}"
 
     @staticmethod
     def _round_DS_to_nearest_0_05(item, value, field, dicom) -> str:
         """Rounds field.element.value to increments of 0.05"""
         value = field.element.value
         if value is None:
             value = -1
```

### Comparing `cobra_db-0.2.4/src/cobra_db/deid_recipe.txt` & `cobra_db-0.3.8/src/cobra_db/deid_recipe.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,40 +15,49 @@
 # •	UIDs are kept.
 
 FORMAT dicom
 
 %header
 
 ADD PatientIdentityRemoved Yes
-ADD DeidentificationMethod vaib_deid_v1.0.1
+ADD DeidentificationMethod vaib_deid_v1.0.2
 
-# Replacements with custom functions. Those can be found in cobra_db.deid
+# Replacements with custom functions. These can be found in cobra_db.deid
 
+REPLACE PatientAge func:round_AS_to_nearest_5y
 REPLACE PatientName func:replace_name
+REPLACE ReferringPhysicianName func:hash_func
 REPLACE AccessionNumber func:hash_func
 REPLACE AdmissionID func:hash_func
 REPLACE InterpretationID func:hash_func
 REPLACE PatientBirthDate func:remove_day
 REPLACE PatientID func:hash_func
 REPLACE PerformedProcedureStepID func:hash_func
 REPLACE PerformingPhysicianName func:hash_func
 REPLACE RequestedProcedureID func:hash_func
 REPLACE ResultsID func:hash_func
 REPLACE StudyID func:hash_func
 REPLACE PatientWeight func:round_DS_to_nearest_5
 REPLACE PatientSize func:round_DS_to_nearest_0_05
-REPLACE PatientAge func:round_AS_to_nearest_5y
+
 
 # Tags that require custom treatment
+
+# BEWARE OF UNEXPECTED REGEX MATCHES
+# the underlying `deid` library uses regex on all the possible versions of
+# the tag. For example the expression "^.{2}[dD]" can match any of the following
+# ["00D0001", "(0DEF,0001)", "Modality"].
+# Therefore, it is recommended to search for the tag with parenthesis.
+
 # Curve Data"(50xx,xxxx)"
-REMOVE contains:^50.{6}$
+REMOVE contains:^\(50.{2},.{4}\)$
 # Overlay comments and data (60xx[34]000)
-REMOVE contains:^60.{2}[34]000$
+REMOVE contains:^\(60.{2},[34]000\)$
 # Private tags ggggeeee where gggg is odd
-REMOVE contains:^.{3}[13579].{4}$
+REMOVE contains:^\(.{3}[13579BDFbdf],.{4}\)$
 
 # Tags not found in pydicom._data_dict
 BLANK contains:001811BB
 BLANK contains:006A0003
 BLANK contains:006A0005
 KEEP contains:00080017
 KEEP contains:00181203
@@ -60,30 +69,28 @@
 REMOVE contains:300A0792
 REMOVE contains:300A0794
 REMOVE contains:300A079A
 
 # Everything else in Table E1 of the dicom standard (In alphabetical order).
 # pydicom.datadict.keyword_for_tag and tag_for_keyword can be used to convert these names to tags
 BLANK AcquisitionContextSequence
-BLANK AcquisitionDeviceProcessingDescription
 BLANK Allergies
 BLANK BarcodeValue
 BLANK ClinicalTrialProtocolID
 BLANK ClinicalTrialProtocolName
 BLANK ClinicalTrialSponsorName
 BLANK ClinicalTrialSubjectID
 BLANK ClinicalTrialSubjectReadingID
 BLANK ClinicalTrialTimePointID
 BLANK ConceptualVolumeCombinationDescription
 BLANK ConceptualVolumeDescription
 BLANK ConsultingPhysicianName
 BLANK ContainerIdentifier
 BLANK ContentCreatorName
 BLANK ContentSequence
-BLANK ContrastBolusAgent
 BLANK DeviceAlternateIdentifier
 BLANK EntityLabel
 BLANK EntityLongLabel
 BLANK FillerOrderNumberImagingServiceRequest
 BLANK FlowIdentifier
 BLANK FlowIdentifierSequence
 BLANK FractionationNotes
@@ -97,15 +104,14 @@
 BLANK PatientState
 BLANK PersonIdentificationCodeSequence
 BLANK PersonName
 BLANK PlacerOrderNumberImagingServiceRequest
 BLANK PreMedication
 BLANK PrescriptionNotes
 BLANK PrescriptionNotesSequence
-BLANK ProtocolName
 BLANK ROIInterpreter
 BLANK ROIName
 BLANK RTAccessoryDeviceSlotID
 BLANK RTAccessoryHolderSlotID
 BLANK RTPhysicianIntentNarrative
 BLANK RTPlanLabel
 BLANK RTPrescriptionLabel
@@ -114,15 +120,14 @@
 BLANK RadiationDoseIdentificationLabel
 BLANK RadiationDoseInVivoMeasurementLabel
 BLANK RadiationGenerationModeDescription
 BLANK RadiationGenerationModeLabel
 BLANK ReasonForSuperseding
 BLANK ReasonForTheAttributeModification
 BLANK ReferencedStudySequence
-BLANK RequestedProcedureDescription
 BLANK ReviewerName
 BLANK SelectorLOValue
 BLANK SelectorLTValue
 BLANK SelectorOBValue
 BLANK SelectorPNValue
 BLANK SelectorSHValue
 BLANK SelectorSTValue
@@ -163,14 +168,15 @@
 KEEP ConcatenationUID
 KEEP ConceptualVolumeUID
 KEEP ConstituentConceptualVolumeUID
 KEEP ContentDate
 KEEP ContentTime
 KEEP ContextGroupLocalVersion
 KEEP ContextGroupVersion
+KEEP ContrastBolusAgent
 KEEP ContrastBolusStartTime
 KEEP ContrastBolusStopTime
 KEEP ContributionDateTime
 KEEP CreationDate
 KEEP CreationTime
 KEEP CurveDate
 KEEP CurveTime
@@ -248,14 +254,15 @@
 KEEP LensMake
 KEEP LensModel
 KEEP LensSerialNumber
 KEEP LensSpecification
 KEEP ManufacturerDeviceClassUID
 KEEP ManufacturerDeviceIdentifier
 KEEP MediaStorageSOPInstanceUID
+KEEP Modality
 KEEP ModifiedImageDate
 KEEP ModifiedImageTime
 KEEP ModifyingDeviceID
 KEEP ModifyingSystem
 KEEP MostRecentTreatmentDate
 KEEP MultiplexGroupUID
 KEEP ObservationDateTime
@@ -285,14 +292,15 @@
 KEEP PregnancyStatus
 KEEP PresentationCreationDate
 KEEP PresentationCreationTime
 KEEP PresentationDisplayCollectionUID
 KEEP PresentationSequenceCollectionUID
 KEEP ProcedureStepCancellationDateTime
 KEEP ProductExpirationDateTime
+KEEP ProtocolName
 KEEP RTPlanDate
 KEEP RTPlanTime
 KEEP RTTreatmentPhaseUID
 KEEP RadiopharmaceuticalStartDateTime
 KEEP RadiopharmaceuticalStartTime
 KEEP RadiopharmaceuticalStopDateTime
 KEEP RadiopharmaceuticalStopTime
@@ -305,14 +313,16 @@
 KEEP ReferencedFrameOfReferenceUID
 KEEP ReferencedGeneralPurposeScheduledProcedureStepTransactionUID
 KEEP ReferencedObservationUIDTrial
 KEEP ReferencedSOPInstanceUID
 KEEP ReferencedSOPInstanceUIDInFile
 KEEP RelatedFrameOfReferenceUID
 KEEP RequestedSOPInstanceUID
+KEEP RescaleIntercept
+KEEP RescaleSlope
 KEEP ReviewDate
 KEEP ReviewTime
 KEEP SOPAuthorizationDateTime
 KEEP SOPInstanceUID
 KEEP SafePositionExitDate
 KEEP SafePositionExitTime
 KEEP SafePositionReturnDate
@@ -398,18 +408,23 @@
 KEEP TreatmentSessionUID
 KEEP TreatmentTime
 KEEP TreatmentToleranceViolationDateTime
 KEEP UDISequence
 KEEP UID
 KEEP UniqueDeviceIdentifier
 KEEP VerificationDateTime
+KEEP VOILUTSequence
+KEEP VOILUTFunction
+KEEP WindowCenter
+KEEP WindowWidth
 KEEP XRayDetectorID
 KEEP XRayDetectorLabel
 KEEP XRaySourceID
 REMOVE AcquisitionComments
+REMOVE AcquisitionDeviceProcessingDescription
 REMOVE AcquisitionProtocolDescription
 REMOVE ActualHumanPerformersSequence
 REMOVE AdditionalPatientHistory
 REMOVE AddressTrial
 REMOVE AdmittingDiagnosesCodeSequence
 REMOVE AdmittingDiagnosesDescription
 REMOVE AffectedSOPInstanceUID
@@ -569,22 +584,22 @@
 REMOVE ReferencedDigitalSignatureSequence
 REMOVE ReferencedImageSequence
 REMOVE ReferencedPatientAliasSequence
 REMOVE ReferencedPatientPhotoSequence
 REMOVE ReferencedPatientSequence
 REMOVE ReferencedPerformedProcedureStepSequence
 REMOVE ReferencedSOPInstanceMACSequence
-REMOVE ReferringPhysicianName
 REMOVE ReferringPhysicianAddress
 REMOVE ReferringPhysicianIdentificationSequence
 REMOVE ReferringPhysicianTelephoneNumbers
 REMOVE RegionOfResidence
 REMOVE RequestAttributesSequence
 REMOVE RequestedContrastAgent
 REMOVE RequestedProcedureComments
+REMOVE RequestedProcedureDescription
 REMOVE RequestedProcedureLocation
 REMOVE RequestedSeriesDescription
 REMOVE RequestingPhysician
 REMOVE RequestingService
 REMOVE RespiratoryMotionCompensationTechniqueDescription
 REMOVE ResponsibleOrganization
 REMOVE ResponsiblePerson
```

### Comparing `cobra_db-0.2.4/src/cobra_db/deid_recipe_mr.txt` & `cobra_db-0.3.8/src/cobra_db/deid_recipe_mr.txt`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/encrypt.py` & `cobra_db-0.3.8/src/cobra_db/encrypt.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/enums.py` & `cobra_db-0.3.8/src/cobra_db/enums.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/filesystem.py` & `cobra_db-0.3.8/src/cobra_db/filesystem.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/model.py` & `cobra_db-0.3.8/src/cobra_db/model.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/mongo_dao.py` & `cobra_db-0.3.8/src/cobra_db/mongo_dao.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,21 @@
         :param _id: ObjectId or str version of ObjectId of the document that will be
         deleted.
         """
         _id = get_obj_id(_id)
         result = self.collection.delete_one({"_id": _id})
         assert result.deleted_count == 1
 
+    def insert_one(self, entity_instance: Entity) -> ObjectId:
+        """
+        Insert an instance into the database.
+        """
+        _id = self.collection.insert_one(entity_instance.to_dict()).inserted_id
+        return _id
+
 
 class PatientDao(EntityDao):
     """
     Get or insert patient from / to the database
     (Manages access to the Patient collection in MongoDB)
     """
```

### Comparing `cobra_db-0.2.4/src/cobra_db/scripts/pseudonymize_image_metadata.py` & `cobra_db-0.3.8/src/cobra_db/scripts/pseudonymize_image_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from cobra_db.dataset_mod import DatasetMod
 from cobra_db.deid import Deider, base_recipe_path, mr_recipe_path
 from cobra_db.filesystem import get_instance_path
 from cobra_db.model import FileSource, ImageMetadata
 from cobra_db.mongo_dao import Connector, ImageMetadataDao
 from cobra_db.scripts.utils import add_args_to_iterable, batcher
 
+from time import sleep
+
 
 def parse_arguments(raw_args: List[str]) -> str:
     """Parse the arguments for the pseudonymization process
 
     :param raw_args: arguments from sys.argv[1:]
     :return: a namespace with the required cfg
     """
@@ -115,15 +117,19 @@
         src_im_dao.connector.close()
         dst_im_dao.connector.close()
 
     return seen, processed
 
 
 def process_im_meta(
-    im_meta_dict: dict, cfg, src_im_dao: ImageMetadataDao, dst_im_dao: ImageMetadataDao
+    im_meta_dict: dict,
+    cfg,
+    src_im_dao: ImageMetadataDao,
+    dst_im_dao: ImageMetadataDao,
+    retries=10,
 ):
     im_meta = ImageMetadata.from_dict(im_meta_dict)
     # get source file
     src_filepath = im_meta.get_local_filepath(cfg.mount_paths)
     try:
         src_ds = pydicom.read_file(src_filepath)
     except Exception as e:
@@ -157,14 +163,24 @@
     dst_filepath = dst_file_source.get_local_filepath(cfg.mount_paths)
 
     os.makedirs(os.path.dirname(dst_filepath), exist_ok=True)
     try:
         pydicom.write_file(dst_filepath, deid_ds)
     except ValueError as e:
         logging.error(f"{e}")
+    except OSError as e:
+        print(f"{e} - {dst_filepath}")
+        if retries > 0:
+            sleep(2)
+            print(f"Retrying now, {r} retries left - {dst_filepath}")
+            r = retries - 1
+            return process_im_meta(im_meta_dict, cfg, src_im_dao, dst_im_dao, r)
+        print(
+            f"Unknown OS error, could not fix by retrying, will not write - {dst_filepath}"
+        )
 
     # the _id of the dataset is stored with the same database _id so that a super user
     # with access to both collections, can quickly check that everything is okay.
     try:
         del deid_ds.PixelData
     except AttributeError as e:
         logging.error(f"{e}")
@@ -181,14 +197,15 @@
     return 1
 
 
 def get_required_drive_names(src_mongo, query):
     connector = Connector(**src_mongo)
     im_dao = ImageMetadataDao(connector)
     logging.info("Searching images to obtain required drives for query")
+    print(f"Running query: {query}")
     cursor = im_dao.collection.aggregate(
         [{"$match": query}, {"$sortByCount": "$file_source.drive_name"}]
     )
     drive_names = []
     images = 0
     for doc in cursor:
         drive_names.append(doc["_id"])
@@ -257,15 +274,17 @@
     # Check how many files will be processed and if the cfg is enough
     required_drive_names, total_imgs = get_required_drive_names(
         cfg.src_mongo, cfg.query
     )
     check_mount_paths(cfg.mount_paths, required_drive_names, cfg.dst_drive_name)
     im_meta_gen = im_meta_generator(cfg.src_mongo, cfg.query)
     logging.info("Saving list of files to be processed")
-    imgs = list(im_meta_gen)  # save as list to avoid losing the
+    imgs = list(
+        tqdm(im_meta_gen, desc="Reading list of files to be processed")
+    )  # save as list to avoid losing the cursor
     batches = batcher(imgs, batch_size=cfg.batch_size)
 
     # Due to a weird configuration system of the deid library this has to be loaded
     # after setting the MESSAGELEVEL env var.
     os.environ["MESSAGELEVEL"] = cfg.logging_level
 
     cfg.deider = Deider(
@@ -275,16 +294,16 @@
             cfg.deid_default_recipes["mr"],
             cfg.user_recipe_path,
         ),
         logging_level=cfg.logging_level,
     )
 
     batches = add_args_to_iterable(batches, cfg)
-    pbar_seen = tqdm(total=total_imgs, desc="Images seen")
-    pbar_processed = tqdm(total=total_imgs, desc="Images processed")
+    pbar_seen = tqdm(total=total_imgs, desc="Images seen", smoothing=0.001)
+    pbar_processed = tqdm(total=total_imgs, desc="Images processed", smoothing=0.001)
     if cfg.n_proc == 1:
         process_func = single_proc
     if cfg.n_proc > 1:
         process_func = multi_proc
     if cfg.n_proc < 1:
         raise ValueError("n_proc must be bigger than 0")
     for seen, processed in process_func(batches, cfg.n_proc):
```

### Comparing `cobra_db-0.2.4/src/cobra_db/scripts/stage_1_ingest_images.py` & `cobra_db-0.3.8/src/cobra_db/scripts/stage_1_ingest_images.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/scripts/stage_2.py` & `cobra_db-0.3.8/src/cobra_db/scripts/stage_2.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_patients.py` & `cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_patients.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_series.py` & `cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_series.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_studies.py` & `cobra_db-0.3.8/src/cobra_db/scripts/stage_2_group_studies.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/scripts/utils.py` & `cobra_db-0.3.8/src/cobra_db/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/types.py` & `cobra_db-0.3.8/src/cobra_db/types.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/src/cobra_db/utils.py` & `cobra_db-0.3.8/src/cobra_db/utils.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.4/PKG-INFO` & `cobra_db-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobra-db
-Version: 0.2.4
+Version: 0.3.8
 Summary: COnsolidated BReast cancer Analysis DataBase
 License: Apache-2.0
 Author: Fernando Cossio
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

