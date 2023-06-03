# Comparing `tmp/pronotepy-2.8.0.tar.gz` & `tmp/pronotepy-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pronotepy-2.8.0.tar", last modified: Tue Dec 27 14:12:32 2022, max compression
+gzip compressed data, was "dist/pronotepy-2.9.0.tar", last modified: Thu Feb  2 17:32:31 2023, max compression
```

## Comparing `pronotepy-2.8.0.tar` & `pronotepy-2.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 14:12:32.000000 pronotepy-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2022-12-27 14:12:32.000000 pronotepy-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2022-12-27 14:12:22.000000 pronotepy-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 14:12:32.000000 pronotepy-2.8.0/pronotepy/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25066 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    60980 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/dataClasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 14:12:32.000000 pronotepy-2.8.0/pronotepy/ent/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/ent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/ent/complex_ent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/ent/ent.py
--rw-r--r--   0 runner    (1001) docker     (123)    12994 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/ent/generic_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/ent/test_ent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/pronoteAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2022-12-27 14:12:22.000000 pronotepy-2.8.0/pronotepy/test_pronotepy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 14:12:32.000000 pronotepy-2.8.0/pronotepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2022-12-27 14:12:32.000000 pronotepy-2.8.0/pronotepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-27 14:12:32.000000 pronotepy-2.8.0/pronotepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 14:12:32.000000 pronotepy-2.8.0/pronotepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 14:12:32.000000 pronotepy-2.8.0/pronotepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-27 14:12:32.000000 pronotepy-2.8.0/pronotepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-27 14:12:32.000000 pronotepy-2.8.0/pronotepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-27 14:12:32.000000 pronotepy-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      855 2022-12-27 14:12:22.000000 pronotepy-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:32:31.000000 pronotepy-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-02-02 17:32:31.000000 pronotepy-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-02-02 17:32:18.000000 pronotepy-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:32:31.000000 pronotepy-2.9.0/pronotepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25278 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64427 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/dataClasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:32:31.000000 pronotepy-2.9.0/pronotepy/ent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/ent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/ent/complex_ent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/ent/ent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/ent/generic_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/ent/test_ent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/pronoteAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-02-02 17:32:18.000000 pronotepy-2.9.0/pronotepy/test_pronotepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:32:31.000000 pronotepy-2.9.0/pronotepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-02-02 17:32:31.000000 pronotepy-2.9.0/pronotepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-02 17:32:31.000000 pronotepy-2.9.0/pronotepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 17:32:31.000000 pronotepy-2.9.0/pronotepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 17:32:31.000000 pronotepy-2.9.0/pronotepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-02 17:32:31.000000 pronotepy-2.9.0/pronotepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-02 17:32:31.000000 pronotepy-2.9.0/pronotepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 17:32:31.000000 pronotepy-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-02 17:32:18.000000 pronotepy-2.9.0/setup.py
```

### Comparing `pronotepy-2.8.0/PKG-INFO` & `pronotepy-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pronotepy
-Version: 2.8.0
+Version: 2.9.0
 Summary: A wrapper for the pronote "API"
 Home-page: https://www.github.com/bain3/pronotepy
 Author: bain
 License: MIT
 Description: <br />
         <p align="center">
           <a href="https://github.com/bain3/pronotepy">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pronotepy Version: 2.8.0 Summary: A wrapper for the
+Metadata-Version: 2.1 Name: pronotepy Version: 2.9.0 Summary: A wrapper for the
 pronote "API" Home-page: https://www.github.com/bain3/pronotepy Author: bain
 License: MIT Description:
                                     [Logo]
                               **** pronotepy ****
                           An API wrapper for PRONOTE
                               Explore_the_docs_Â»
 [![pypi version](https://img.shields.io/pypi/v/pronotepy.svg)](https://
```

### Comparing `pronotepy-2.8.0/README.md` & `pronotepy-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pronotepy-2.8.0/pronotepy/clients.py` & `pronotepy-2.9.0/pronotepy/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,17 +595,23 @@
 
         # since we only have week precision, we need to make it more precise on our own
         return [menu for menu in output if date_from <= menu.date <= date_to]
 
     @property
     def current_period(self) -> dataClasses.Period:
         """the current period"""
-        id_period = self.parametres_utilisateur["donneesSec"]["donnees"]["ressource"][
+        onglets = self.parametres_utilisateur["donneesSec"]["donnees"]["ressource"][
             "listeOngletsPourPeriodes"
-        ]["V"][0]["periodeParDefaut"]["V"]["N"]
+        ]["V"]
+
+        # get onglet with number 198 (mes notes), otherwise fallback to the
+        # first one in the list
+        onglet = next(filter(lambda x: x.get("G") == 198, onglets), onglets[0])
+
+        id_period = onglet["periodeParDefaut"]["V"]["N"]
         return dataClasses.Util.get(self.periods, id=id_period)[0]
 
 
 class ParentClient(Client):
     """
     A parent PRONOTE client.
```

### Comparing `pronotepy-2.8.0/pronotepy/dataClasses.py` & `pronotepy-2.9.0/pronotepy/dataClasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,20 @@
                 formatted_date, "%d/%m/%Y %H:%M:%S"
             ).date()
         elif re.match(r"\d{2}/\d{2}/\d{2} \d{2}h\d{2}$", formatted_date):
             return datetime.datetime.strptime(formatted_date, "%d/%m/%y %Hh%M").date()
         elif re.match(r"\d{2}/\d{2}", formatted_date):
             formatted_date += f"/{datetime.date.today().year}"
             return datetime.datetime.strptime(formatted_date, "%d/%m/%Y").date()
+        elif re.match(r"\d{2}\d{2}$", formatted_date):
+            date = datetime.date.today()
+            hours = int(formatted_date[:2])
+            minutes = int(formatted_date[2:])
+            formatted_date = f"{date:%d}/{date:%m}/{date.year} {hours}h{minutes}"
+            return datetime.datetime.strptime(formatted_date, "%d/%m/%Y %Hh%M").date()
         else:
             raise DateParsingError("Could not parse date", formatted_date)
 
     @staticmethod
     def datetime_parse(formatted_date: str) -> datetime.datetime:
         """convert date to a datetime.datetime object"""
         if re.match(r"\d{2}/\d{2}/\d{4}$", formatted_date):
@@ -333,14 +339,44 @@
         self.reasons: List[str] = self._resolver(
             lambda l: [i["L"] for i in l], "listeMotifs", "V", default=[]
         )
 
         del self._resolver
 
 
+class Delay(Object):
+    """
+    Represents a delay with a given period. You shouldn't have to create this class manually.
+
+    Attributes:
+        id (str): the id of the delay (used internally)
+        date (datetime.datetime): date of the delay
+        minutes (str): the number of minutes missed
+        justified (bool): is the delay justified
+        justification (str): the justification for the delay
+        reasons (List[str]): The reason(s) for the delay
+    """
+
+    def __init__(self, json_dict: dict) -> None:
+        super().__init__(json_dict)
+
+        self.id: str = self._resolver(str, "N")
+        self.date: datetime.datetime = self._resolver(Util.datetime_parse, "date", "V")
+        self.minutes: int = self._resolver(int, "duree", default=0)
+        self.justified: bool = self._resolver(bool, "justifie", default=False)
+        self.justification: Optional[str] = self._resolver(
+            str, "justification", strict=False
+        )
+        self.reasons: List[str] = self._resolver(
+            lambda l: [i["L"] for i in l], "listeMotifs", "V", default=[]
+        )
+
+        del self._resolver
+
+
 class Period(Object):
     """
     Represents a period of the school year. You shouldn't have to create this class manually.
 
     Attributes:
         id (str): the id of the period (used internally)
         name (str): name of the period
@@ -386,15 +422,15 @@
             return [Average(c) for c in crs]
         except ParsingError as e:
             if e.path == ["moyEleve", "V"]:
                 raise UnsupportedOperation("Could not get averages")
             raise
 
     @property
-    def overall_average(self) -> float:
+    def overall_average(self) -> str:
         """Get overall average from the period. If the period average is not provided by pronote, then it's calculated.
         Calculation may not be the same as the actual average. (max difference 0.01)"""
         json_data = {"Periode": {"N": self.id, "L": self.name}}
         response = self._client.post("DernieresNotes", 198, json_data)
         average = response["donneesSec"]["donnees"].get("moyGenerale")
         if average:
             return average["V"]
@@ -414,15 +450,26 @@
                     flt = False
                 if flt:
                     a += flt
                     total += 1
             average = round(a / total, 2) if total else -1
         else:
             average = -1
-        return average
+        return str(average)
+
+    @property
+    def class_overall_average(self) -> Optional[str]:
+        """Get group average from the period."""
+        json_data = {"Periode": {"N": self.id, "L": self.name}}
+        response = self._client.post("DernieresNotes", 198, json_data)
+        average = response["donneesSec"]["donnees"].get("moyGeneraleClasse")
+        if average:
+            return average["V"]
+        else:
+            return None
 
     @property
     def evaluations(self) -> List["Evaluation"]:
         """
         All evaluations from this period
         """
         json_data = {"periode": {"N": self.id, "L": self.name, "G": 2}}
@@ -442,14 +489,29 @@
         }
 
         response = self._client.post("PagePresence", 19, json_data)
         absences = response["donneesSec"]["donnees"]["listeAbsences"]["V"]
         return [Absence(a) for a in absences if a["G"] == 13]
 
     @property
+    def delays(self) -> List[Delay]:
+        """
+        All delays from this period
+        """
+        json_data = {
+            "periode": {"N": self.id, "L": self.name, "G": 2},
+            "DateDebut": {"_T": 7, "V": self.start.strftime("%d/%m/%Y %H:%M:%S")},
+            "DateFin": {"_T": 7, "V": self.end.strftime("%d/%m/%Y %H:%M:%S")},
+        }
+
+        response = self._client.post("PagePresence", 19, json_data)
+        delays = response["donneesSec"]["donnees"]["listeAbsences"]["V"]
+        return [Delay(a) for a in delays if a["G"] == 14]
+
+    @property
     def punishments(self) -> List[Punishment]:
         """
         All punishments from a given period
         """
         json_data = {
             "periode": {"N": self.id, "L": self.name, "G": 2},
             "DateDebut": {"_T": 7, "V": self.start.strftime("%d/%m/%Y %H:%M:%S")},
@@ -469,28 +531,32 @@
         student (str): students average in the subject
         class_average (str): classes average in the subject
         max (str): highest average in the class
         min (str): lowest average in the class
         out_of (str): maximum amount of points
         default_out_of (str): the default maximum amount of points
         subject (Subject): subject the average is from
+        background_color (str): background color of the subject
     """
 
     def __init__(self, json_dict: dict) -> None:
         super().__init__(json_dict)
 
         self.student: str = self._resolver(Util.grade_parse, "moyEleve", "V")
         self.out_of: str = self._resolver(Util.grade_parse, "baremeMoyEleve", "V")
         self.default_out_of: str = self._resolver(
             Util.grade_parse, "baremeMoyEleveParDefault", "V", default=""
         )
         self.class_average: str = self._resolver(Util.grade_parse, "moyClasse", "V")
         self.min: str = self._resolver(Util.grade_parse, "moyMin", "V")
         self.max: str = self._resolver(Util.grade_parse, "moyMax", "V")
         self.subject = Subject(json_dict)
+        self.background_color: Optional[str] = self._resolver(
+            str, "couleur", strict=False
+        )
 
         del self._resolver
 
 
 class Grade(Object):
     """Represents a grade. You shouldn't have to create this class manually.
 
@@ -667,14 +733,15 @@
         classrooms (Optional[List[str]]): name of the classrooms
         canceled (bool): if the lesson is canceled
         status (Optional[str]): status of the lesson
         background_color (Optional[str]): background color of the lesson
         outing (bool): if it is a pedagogical outing
         start (datetime.datetime): starting time of the lesson
         end (datetime.datetime): end of the lesson
+        memo (Optional[str]): memo of the lesson
         group_name (Optional[str]): Name of the group.
         group_names (Optional[List[str]]): Name of the groups.
         exempted (bool): Specifies if the student's presence is exempt.
         virtual_classrooms (List[str]): List of urls for virtual classrooms
         num (int): For the same lesson time, the biggest num is the one shown on pronote.
         detention (bool): is marked as detention
         test (bool): if there will be a test in the lesson
@@ -684,14 +751,15 @@
         super().__init__(json_dict)
         self._client = client
         self._content: Optional[LessonContent] = None
 
         self.id: str = self._resolver(str, "N")
         self.canceled: bool = self._resolver(bool, "estAnnule", default=False)
         self.status: Optional[str] = self._resolver(str, "Statut", strict=False)
+        self.memo: Optional[str] = self._resolver(str, "memo", strict=False)
         self.background_color: Optional[str] = self._resolver(
             str, "CouleurFond", strict=False
         )
         self.outing: bool = self._resolver(bool, "estSortiePedagogique", default=False)
         self.start: datetime.datetime = self._resolver(
             Util.datetime_parse, "DateDuCours", "V"
         )
@@ -767,14 +835,15 @@
             ", ".join(self.group_names) if self.group_names else None
         )
 
         del self._resolver
 
     @property
     def normal(self) -> bool:
+        """Is the lesson considered normal (is not detention, or an outing)."""
         if self.detention is None and self.outing is None:
             return True
         return False
 
     @property
     def content(self) -> Optional[LessonContent]:
         """
@@ -902,17 +971,19 @@
             make_attachments, "listeQuestions", "V"
         )
 
         del self._resolver
 
     @property
     def content(self) -> str:
+        """Content of the information"""
         return Util.html_parse(self._raw_content[0]["texte"]["V"])
 
     def mark_as_read(self, status: bool) -> None:
+        """Mark this information as read"""
         data = {
             "listeActualites": [
                 {
                     "N": self.id,
                     "validationDirecte": True,
                     "genrePublic": 4,
                     "public": {
@@ -1019,14 +1090,15 @@
     Represents a discussion.
 
     Attributes:
         id (str): the id of the discussion (used internally)
         subject (str): the subject of the discussion
         creator (str): the person who open the discussion
         messages (List[Message]): messages link to the discussion
+        participants (List[str]): participants of the discussion
         unread (int): number of unread messages
         close (bool): True if the discussion is close
         date (datetime.datetime): the date when the discussion was open
         replyable (bool): because pronotepy does not currently support replying
             to discussions that are inside other discussions, this boolean signifies
             if pronotepy is able to reply
     """
@@ -1050,14 +1122,19 @@
             str, "initiateur", strict=False
         ) or self._resolver(str, "public")
         self.messages: List[Message] = self._resolver(
             lambda l: [Message.get(self._client, m["N"]) for m in l],
             "listePossessionsMessages",
             "V",
         )
+        self.participants: List[str] = self._resolver(
+            lambda l: [d["L"] for d in l],
+            "destinatairesMessage",
+            "V",
+        )
         self.unread: int = self._resolver(int, "nbNonLus", default=0)
         self.close: bool = self._resolver(bool, "ferme", default=False)
         self.date: datetime.date = self._resolver(Util.date_parse, "libelleDate")
 
         del self._resolver
 
     def mark_as(self, read: bool) -> None:
@@ -1199,14 +1276,17 @@
             c["ville"],
             c["province"],
             c["pays"],
         )
 
     @property
     def email(self) -> str:
+        """
+        Email of the client
+        """
         return self._cache()["eMail"]
 
     @property
     def phone(self) -> str:
         """
         Phone of the client
 
@@ -1214,14 +1294,17 @@
             str: Phone in the format +[country-code][phone-number]
         """
         c = self._cache()
         return "+" + c["indicatifTel"] + c["telephonePortable"]
 
     @property
     def ine_number(self) -> str:
+        """
+        INE number of the client
+        """
         return self._cache()["numeroINE"]
 
 
 class Acquisition(Object):
     """
     Contains acquisition info for an evaluation.
 
@@ -1509,14 +1592,20 @@
         self.grade: str = self._resolver(str, "niveau", "V", "L", default="")
 
         self._client = client
 
         del self._resolver
 
     def students(self, period: Optional[Period] = None) -> List[Student]:
+        """
+        Get students in the class
+
+        Args:
+            period (Optional[Period]): select a particular period (client.periods[0] by default)
+        """
         period = period or self._client.periods[0]
         r = self._client.post(
             "ListeRessources",
             105,
             {"classe": {"N": self.id, "G": 1}, "periode": {"N": period.id, "G": 1}},
         )
         return [
```

### Comparing `pronotepy-2.8.0/pronotepy/ent/__init__.py` & `pronotepy-2.9.0/pronotepy/ent/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     cas_seinesaintdenis_edu,
     eclat_bfc,
     ecollege_haute_garonne,
     ecollege_haute_garonne_edu,
     enc_hauts_de_seine,
     ent2d_bordeaux,
     ent77,
+    ent_94,
     ent_auvergnerhonealpe,
     ent_creuse,
     ent_elyco,
     ent_essonne,
     ent_hdf,
     ent_mayotte,
     ent_somme,
```

### Comparing `pronotepy-2.8.0/pronotepy/ent/complex_ent.py` & `pronotepy-2.9.0/pronotepy/ent/complex_ent.py`

 * *Files identical despite different names*

### Comparing `pronotepy-2.8.0/pronotepy/ent/ent.py` & `pronotepy-2.9.0/pronotepy/ent/ent.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,27 +151,33 @@
 
 lyceeconnecte_aquitaine = partial(
     _open_ent_ng, url="https://mon.lyceeconnecte.fr/auth/login"
 )
 
 """Open ENT NG with EduConnect"""
 
+ent_94 = partial(
+    _open_ent_ng_edu,
+    domain="https://ent94.opendigitaleducation.com",
+    providerId="urn:fi:ent:prod-cd94-edu:1.0",
+)
+
 ent_hdf = partial(_open_ent_ng_edu, domain="https://enthdf.fr")
 
 ent_somme = ent_hdf
 
 ent_var = partial(
     _open_ent_ng_edu,
-    domain="https://moncollege-ent.var.fr/",
+    domain="https://moncollege-ent.var.fr",
     providerId="urn:fi:ent:prod-cd83-edu:1.0",
 )
 
 l_normandie = partial(_open_ent_ng_edu, domain="https://ent.l-educdenormandie.fr")
 
-lyceeconnecte_edu = partial(_open_ent_ng_edu, domain="https://mon.lyceeconnecte.fr/")
+lyceeconnecte_edu = partial(_open_ent_ng_edu, domain="https://mon.lyceeconnecte.fr")
 
 """WAYF"""
 
 ent_elyco = partial(_wayf, domain="https://cas3.e-lyco.fr", redirect_form=False)
 
 ent2d_bordeaux = partial(
     _wayf,
```

### Comparing `pronotepy-2.8.0/pronotepy/ent/generic_func.py` & `pronotepy-2.9.0/pronotepy/ent/generic_func.py`

 * *Files identical despite different names*

### Comparing `pronotepy-2.8.0/pronotepy/ent/test_ent.py` & `pronotepy-2.9.0/pronotepy/ent/test_ent.py`

 * *Files identical despite different names*

### Comparing `pronotepy-2.8.0/pronotepy/exceptions.py` & `pronotepy-2.9.0/pronotepy/exceptions.py`

 * *Files identical despite different names*

### Comparing `pronotepy-2.8.0/pronotepy/pronoteAPI.py` & `pronotepy-2.9.0/pronotepy/pronoteAPI.py`

 * *Files identical despite different names*

### Comparing `pronotepy-2.8.0/pronotepy/test_pronotepy.py` & `pronotepy-2.9.0/pronotepy/test_pronotepy.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,23 @@
             self.assertLessEqual(start, lesson.start.date())
             self.assertLessEqual(lesson.start.date(), end)
 
     def test_periods(self) -> None:
         self.assertIsNotNone(client.periods)
 
     def test_current_period(self) -> None:
-        self.assertIsNotNone(client.current_period)
+        p = client.current_period
+        self.assertIsNotNone(p)
+        pronote_time = pronotepy.Util.datetime_parse(
+            client.func_options["donneesSec"]["donnees"]["DateServeurHttp"]["V"]
+        )
+        self.assertTrue(
+            p.start < pronote_time < p.end,
+            "current_period is not in progress",
+        )
 
     def test_homework(self) -> None:
         start = client.start_day
         end = client.start_day + datetime.timedelta(days=31)
         homework = client.homework(start, end)
 
         # We assume demo website will always have homework
@@ -104,20 +112,30 @@
 
     def test_absences(self) -> None:
         all_absences = []
         for period in client.periods:
             all_absences.extend(period.absences)
         self.assertGreater(len(all_absences), 0)
 
+    def test_delays(self) -> None:
+        all_delays = []
+        for period in client.periods:
+            all_delays.extend(period.delays)
+        self.assertGreater(len(all_delays), 0)
+
     def test_punishments(self) -> None:
         all_punishments = []
         for period in client.periods:
             all_punishments.extend(period.punishments)
         self.assertGreater(len(all_punishments), 0)
 
+    def test_class_overall_average(self) -> None:
+        a = self.period.class_overall_average
+        self.assertTrue(type(a) is str or a is None)
+
 
 class TestInformation(unittest.TestCase):
     def test_unread(self) -> None:
         information = client.information_and_surveys(only_unread=True)
         for info in information:
             self.assertFalse(info.read)
```

### Comparing `pronotepy-2.8.0/pronotepy.egg-info/PKG-INFO` & `pronotepy-2.9.0/pronotepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pronotepy
-Version: 2.8.0
+Version: 2.9.0
 Summary: A wrapper for the pronote "API"
 Home-page: https://www.github.com/bain3/pronotepy
 Author: bain
 License: MIT
 Description: <br />
         <p align="center">
           <a href="https://github.com/bain3/pronotepy">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pronotepy Version: 2.8.0 Summary: A wrapper for the
+Metadata-Version: 2.1 Name: pronotepy Version: 2.9.0 Summary: A wrapper for the
 pronote "API" Home-page: https://www.github.com/bain3/pronotepy Author: bain
 License: MIT Description:
                                     [Logo]
                               **** pronotepy ****
                           An API wrapper for PRONOTE
                               Explore_the_docs_Â»
 [![pypi version](https://img.shields.io/pypi/v/pronotepy.svg)](https://
```

### Comparing `pronotepy-2.8.0/setup.py` & `pronotepy-2.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pronotepy",
-    version="2.8.0",
+    version="2.9.0",
     description='A wrapper for the pronote "API"',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.github.com/bain3/pronotepy",
     author="bain",
     license="MIT",
     packages=setuptools.find_packages(),
```

