# Comparing `tmp/nhl_api_py-0.1.3.tar.gz` & `tmp/nhl_api_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.1.3.tar", max compression
+gzip compressed data, was "nhl_api_py-0.1.4.tar", max compression
```

## Comparing `nhl_api_py-0.1.3.tar` & `nhl_api_py-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1370 2023-06-02 19:17:51.559748 nhl_api_py-0.1.3/README.md
--rw-r--r--   0        0        0       33 2023-06-02 18:53:59.479744 nhl_api_py-0.1.3/nhlpy/__init__.py
--rw-r--r--   0        0        0      309 2023-06-01 16:00:57.059417 nhl_api_py-0.1.3/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      472 2023-06-01 16:03:00.509418 nhl_api_py-0.1.3/nhlpy/api/core.py
--rw-r--r--   0        0        0     1884 2023-06-02 19:14:40.749748 nhl_api_py-0.1.3/nhlpy/api/players.py
--rw-r--r--   0        0        0      389 2023-06-02 18:52:47.229744 nhl_api_py-0.1.3/nhlpy/api/schedule.py
--rw-r--r--   0        0        0     1365 2023-06-02 19:18:58.449748 nhl_api_py-0.1.3/nhlpy/api/standings.py
--rw-r--r--   0        0        0     1073 2023-06-02 18:40:42.149742 nhl_api_py-0.1.3/nhlpy/api/teams.py
--rw-r--r--   0        0        0      392 2023-06-02 19:19:13.409748 nhl_api_py-0.1.3/nhlpy/nhl_client.py
--rw-r--r--   0        0        0     1257 2023-06-02 19:22:11.479749 nhl_api_py-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 nhl_api_py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3702 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/README.md
+-rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/core.py
+-rw-r--r--   0        0        0     2045 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/players.py
+-rw-r--r--   0        0        0      561 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/schedule.py
+-rw-r--r--   0        0        0     1829 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/standings.py
+-rw-r--r--   0        0        0     1999 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      394 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/nhl_client.py
+-rw-r--r--   0        0        0     1257 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 nhl_api_py-0.1.4/PKG-INFO
```

### Comparing `nhl_api_py-0.1.3/nhlpy/api/players.py` & `nhl_api_py-0.1.4/nhlpy/api/players.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from typing import Optional
 from nhlpy.api import BaseNHLAPIClient
 
 
 class Players(BaseNHLAPIClient):
     def get_player(self, person_id: str) -> dict:
+        """
+        Returns a player based on the person_id.
+        :param person_id:
+        :return:
+        """
         return self._get(resource=f"people/{person_id}").json()
 
-    def get_player_stats(self, person_id: str, season: str = None, stat_type: str = "statsSingleSeason") -> dict:
+    def get_player_stats(
+        self, person_id: str, season: str = None, stat_type: str = "statsSingleSeason"
+    ) -> dict:
         """
         This returns a players statistics based on the param stat_type: and season:  An example of this
         may be client.players.get_player_stats(stat_type="yearByYear", season="20202021").  In some instances season:
         does not matter, such as yearByYear.
         :param person_id: int - Player ID
         :param season: str - Season in format of 20202021
         :param stat_type: str - These can be accessed programmatically via get_player_stat_types()
@@ -20,15 +27,17 @@
             byMonth, byMonthPlayoffs, byDayOfWeek, byDayOfWeekPlayoffs, homeAndAway, homeAndAwayPlayoffs,
             winLoss, winLossPlayoffs, onPaceRegularSeason, regularSeasonStatRankings, playoffStatRankings,
             goalsByGameSituation, goalsByGameSituationPlayoffs, statsSingleSeason, statsSingleSeasonPlayoffs
 
         :return:
         """
         query = f"stats={stat_type}" if stat_type else ""
-        return self._get(resource=f"people/{person_id}/stats?season={season}&{query}").json()
+        return self._get(
+            resource=f"people/{person_id}/stats?season={season}&{query}"
+        ).json()
 
     def get_player_stat_types(self) -> dict:
         """
         Returns the full list of stat(types) that can be used in get_player_stats()'s stat_type param
         :return:
         """
         return self._get(resource="statTypes").json()
```

### Comparing `nhl_api_py-0.1.3/nhlpy/api/standings.py` & `nhl_api_py-0.1.4/nhlpy/api/standings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from nhlpy.api import BaseNHLAPIClient
 
 
 class Standings(BaseNHLAPIClient):
     def get_standings(self, season: str = None, detailed_record: bool = False) -> dict:
         """
-        year: str - Format of 20212022
-        detailed_record: bool - Detailed information for each team including
+        Gets the standings for the season supplied via season: param.
+        :param season:
+        :param detailed_record: Detailed information for each team including
             home and away records, record in shootouts, last ten games, and split
-            head-to-head records against divisions and conferences
+            head-to-head records against divisions and conferences.
+        :return: dict
         """
         modifier = f"season={season}&" if season else ""
         detailed = "expand=standings.record&" if detailed_record else ""
-        return self._get(resource=f'standings?{modifier}{detailed}').json()
+        return self._get(resource=f"standings?{modifier}{detailed}").json()
 
     def get_standing_types(self) -> dict:
         """
         Returns a list of standing types that can be used in get_standings_by_standing_type()
-        :return:
+        :return: dict of standing types
         """
-        return self._get(resource='standingsTypes').json()
+        return self._get(resource="standingsTypes").json()
 
-    def get_standings_by_standing_type(self, standing_type: str) -> dict:
+    def get_standings_by_standing_type(
+        self, season: str, standing_type: str, detailed_records: bool = False
+    ) -> dict:
         """
 
-        :param standing_type: string, full list found in get_standing_types() with the following options:
+        :param detailed_records:  bool, indicates whether or not to return detailed records for each team
+        :param season: str, Season in the format of 20202021
+        :param standing_type: str, full list found in get_standing_types() with the following options:
             regularSeason, wildCard,divisionLeaders, wildCardWithLeaders, preseason,
             postseason, byDivision, byConference, byLeague
-        :return:
+        :return: dict
         """
-        return self._get(resource=f'standings/{standing_type}').json()
+        query = f"season={season}&"
+        detailed = "expand=standings.record&" if detailed_records else ""
+        return self._get(resource=f"standings/{standing_type}?{query}{detailed}").json()
```

### Comparing `nhl_api_py-0.1.3/pyproject.toml` & `nhl_api_py-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "0.1.3"
+version = "0.1.4"
 description = "NHL API Wrapper.  For standings, team stats and outcomes."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/coreyjs/nhl-api-py"
 repository = "https://github.com/coreyjs/nhl-api-py"
```

