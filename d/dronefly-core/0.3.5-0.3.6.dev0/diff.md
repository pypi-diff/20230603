# Comparing `tmp/dronefly_core-0.3.5.tar.gz` & `tmp/dronefly_core-0.3.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_core-0.3.5.tar", max compression
+gzip compressed data, was "dronefly_core-0.3.6.dev0.tar", max compression
```

## Comparing `dronefly_core-0.3.5.tar` & `dronefly_core-0.3.6.dev0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.5/LICENSE
--rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.5/README.md
--rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.5/dronefly/core/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.5/dronefly/core/clients/__init__.py
--rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.5/dronefly/core/clients/inat.py
--rw-r--r--   0        0        0     4734 2023-04-16 14:27:09.193332 dronefly_core-0.3.5/dronefly/core/commands/__init__.py
--rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.5/dronefly/core/constants.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.5/dronefly/core/formatters/__init__.py
--rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.5/dronefly/core/formatters/constants.py
--rw-r--r--   0        0        0    30581 2023-04-30 15:34:08.268856 dronefly_core-0.3.5/dronefly/core/formatters/generic.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.5/dronefly/core/models/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.5/dronefly/core/models/controlled_terms.py
--rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.5/dronefly/core/models/user.py
--rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.5/dronefly/core/parsers/__init__.py
--rw-r--r--   0        0        0     3672 2023-03-06 21:18:23.821142 dronefly_core-0.3.5/dronefly/core/parsers/constants.py
--rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.5/dronefly/core/parsers/natural.py
--rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.5/dronefly/core/parsers/unixlike.py
--rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.5/dronefly/core/parsers/url.py
--rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.5/dronefly/core/query/__init__.py
--rw-r--r--   0        0        0    19236 2023-04-16 13:38:29.366402 dronefly_core-0.3.5/dronefly/core/query/query.py
--rw-r--r--   0        0        0      527 2023-04-22 12:12:03.306747 dronefly_core-0.3.5/dronefly/core/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-05-06 10:34:27.666900 dronefly_core-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 dronefly_core-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev0/LICENSE
+-rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev0/README.md
+-rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev0/dronefly/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev0/dronefly/core/clients/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev0/dronefly/core/clients/inat.py
+-rw-r--r--   0        0        0     6065 2023-06-03 17:20:18.843066 dronefly_core-0.3.6.dev0/dronefly/core/commands/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev0/dronefly/core/constants.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev0/dronefly/core/formatters/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev0/dronefly/core/formatters/constants.py
+-rw-r--r--   0        0        0    29903 2023-06-03 20:23:10.683148 dronefly_core-0.3.6.dev0/dronefly/core/formatters/generic.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev0/dronefly/core/models/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev0/dronefly/core/models/controlled_terms.py
+-rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev0/dronefly/core/models/user.py
+-rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev0/dronefly/core/parsers/__init__.py
+-rw-r--r--   0        0        0     3672 2023-03-06 21:18:23.821142 dronefly_core-0.3.6.dev0/dronefly/core/parsers/constants.py
+-rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev0/dronefly/core/parsers/natural.py
+-rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev0/dronefly/core/parsers/unixlike.py
+-rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev0/dronefly/core/parsers/url.py
+-rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev0/dronefly/core/query/__init__.py
+-rw-r--r--   0        0        0    19236 2023-04-16 13:38:29.366402 dronefly_core-0.3.6.dev0/dronefly/core/query/query.py
+-rw-r--r--   0        0        0      527 2023-04-22 12:12:03.306747 dronefly_core-0.3.6.dev0/dronefly/core/utils/__init__.py
+-rw-r--r--   0        0        0      741 2023-06-03 20:27:06.376039 dronefly_core-0.3.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev0/setup.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev0/PKG-INFO
```

### Comparing `dronefly_core-0.3.5/LICENSE` & `dronefly_core-0.3.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/README.md` & `dronefly_core-0.3.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/dronefly/core/clients/inat.py` & `dronefly_core-0.3.6.dev0/dronefly/core/clients/inat.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/dronefly/core/constants.py` & `dronefly_core-0.3.6.dev0/dronefly/core/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/dronefly/core/formatters/generic.py` & `dronefly_core-0.3.6.dev0/dronefly/core/formatters/generic.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,14 +113,35 @@
             regex = f"(?:{_URL_REGEX}|{regex})"
         return re.sub(regex, replacement, text, 0, re.MULTILINE)
     else:
         text = re.sub(r"\\", r"\\\\", text)
         return _MARKDOWN_ESCAPE_REGEX.sub(r"\\\1", text)
 
 
+def format_datetime(time, compact=False):
+    """Format datetime with compact option that drops less relevant parts."""
+    hour = time.strftime("%I").lstrip("0")
+    minute = time.strftime("%M")
+    am_pm = time.strftime("%p").lower()
+    day = time.strftime("%d").lstrip("0")
+    mon = time.strftime("%b")
+    year = time.strftime("%Y")
+    if compact:
+        if time.date() == dt.now().date():
+            formatted_time = f"{hour}:{minute}{am_pm}"
+        elif time.year == dt.now().year:
+            formatted_time = f"{day}-{mon}"
+        else:
+            formatted_time = f"{mon}-{year}"
+    else:
+        wday = time.strftime("%a")
+        formatted_time = f"{wday} {mon} {day}, {year} · {hour}:{minute} {am_pm}"
+    return formatted_time
+
+
 def format_user_name(user: User):
     """Format user's display name with Markdown special characters escaped."""
     if user.name:
         return f"{escape_markdown(user.name)} ({escape_markdown(user.login)})"
     return escape_markdown(user.login)
 
 
@@ -450,15 +471,14 @@
     def __init__(
         self,
         taxon: Taxon,
         lang: str = None,
         with_url: bool = True,
         matched_term: str = None,
         max_len: int = 0,
-        newline: str = "\n",
     ):
         """
         Parameters
         ----------
         taxon: Taxon
             The taxon to format.
 
@@ -473,27 +493,26 @@
             When True, link the name to taxon.url.
         """
         self.taxon = taxon
         self.lang = lang
         self.with_url = with_url
         self.matched_term = matched_term
         self.max_len = max_len
-        self.newline = newline
         self.obs_count_formatter = self.ObsCountFormatter(taxon)
 
     def format(self, with_title: bool = True, with_ancestors: bool = True):
         """Format the taxon as markdown.
 
         with_title: bool, optional
         with_ancestors: bool, optional
             When False, omit ancestors
         """
         description = self.format_taxon_description()
         if with_title:
-            description = self.newline.join([self.format_title(), description])
+            description = "\n".join([self.format_title(), description])
         if with_ancestors and self.taxon.ancestors:
             description += " in: " + format_taxon_names(
                 self.taxon.ancestors,
                 hierarchy=True,
                 max_len=self.max_len,
             )
         else:
@@ -599,47 +618,63 @@
     def __init__(
         self,
         obs: Observation,
         with_description=True,
         with_link=False,
         compact=False,
         with_user=True,
+        taxon: Taxon = None,
         taxon_summary: TaxonSummary = None,
         community_taxon: Taxon = None,
         community_taxon_summary: TaxonSummary = None,
     ):
         self.obs = obs
         self.compact = compact
         self.with_description = with_description
         self.with_link = with_link
         self.compact = compact
         self.with_user = with_user
+        self.taxon = taxon or self.obs.taxon
         self.taxon_summary = taxon_summary
         self.community_taxon = community_taxon
         self.community_taxon_summary = community_taxon_summary
 
-    def format(self):
-        title = self.format_title()
-        summary = self.format_summary(self.obs.taxon, self.taxon_summary)
+    def format(self, join_title: bool = True):
+        title = self.format_title(with_link=join_title)
+        summary = self.format_summary(self.taxon, self.taxon_summary)
         title, summary = self.format_community_id(
             title, summary, self.community_taxon_summary
         )
         if not self.compact:
             title += self.format_media_counts()
-            if self.with_link:
-                link_url = f"{WWW_BASE_URL}/observations/{self.obs.id}"
-                title = f"{title} [🔗]({link_url})"
-        return title + "\n> " + summary + "\n> "
+        result = (title, summary)
+        if join_title:
+            result = ("" if self.compact else "\n").join(result)
+        return result
+
+    def format_taxon_link(self, taxon: Taxon):
+        taxon_str = self.get_taxon_name(taxon)
+        if taxon and self.with_link:
+            common = (
+                f" ({taxon.preferred_common_name})"
+                if taxon.preferred_common_name
+                else ""
+            )
+            taxon_str = (
+                format_link(taxon_str, f"{WWW_BASE_URL}/taxa/{taxon.id}") + common
+            )
+        return taxon_str
 
-    def format_title(self):
+    def format_title(self, with_link: bool = True):
         title = ""
-        taxon_str = self.get_taxon_name(self.obs.taxon)
-        if self.with_link:
-            link_url = f"{WWW_BASE_URL}/observations/{self.obs.id}"
-            taxon_str = f"[{taxon_str}]({link_url})"
+        taxon_str = self.get_taxon_name(self.taxon)
+        if with_link and self.with_link:
+            taxon_str = format_link(
+                taxon_str, f"{WWW_BASE_URL}/observations/{self.obs.id}"
+            )
         title += taxon_str
         if not self.compact:
             title += f" by {self.obs.user.login} " + ICONS[self.obs.quality_grade]
             if self.obs.faves:
                 title += self.format_count("fave", len(self.obs.faves))
             if self.obs.comments:
                 title += self.format_count("comment", len(self.obs.comments))
@@ -656,119 +691,112 @@
             )
         else:
             taxon_str = "Unknown"
         return taxon_str
 
     def format_summary(self, taxon, taxon_summary):
         summary = ""
-        if not self.compact:
-            taxon_str = self.get_taxon_name(taxon)
-            if taxon:
-                common = (
-                    f" ({taxon.preferred_common_name})"
-                    if taxon.preferred_common_name
-                    else ""
-                )
-                link_url = f"{WWW_BASE_URL}/taxa/{taxon.id}"
-                taxon_str = f"[{taxon_str}]({link_url}){common}"
+        obs = self.obs
+        compact = self.compact
+        with_user = self.with_user
+        with_description = self.with_description
+
+        if not compact:
+            taxon_str = self.format_taxon_link(taxon)
             summary += f"Taxon: {taxon_str}\n"
         if taxon_summary:
             means = taxon_summary.listed_taxon
             status = taxon_summary.conservation_status
             if status:
                 formatted_status = format_taxon_conservation_status(status)
                 summary += f"Conservation Status: {formatted_status}\n"
             if means:
                 summary += f"{format_taxon_establishment_means(means)}\n"
         login = ""
-        if self.compact:
-            if self.with_user:
-                login = self.obs.user.login
+        if compact:
+            if with_user:
+                login = obs.user.login
             summary += "\n"
         else:
-            summary += "Observed by " + format_user_link(self.obs.user)
+            summary += "Observed by " + format_user_link(obs.user)
         obs_on = ""
         obs_at = ""
-        if self.obs.observed_on:
-            if self.compact:
-                if self.obs.observed_on.date() == dt.datetime.now().date():
-                    obs_on = self.obs.observed_on.strftime("%-I:%M%P")
-                elif self.obs.observed_on.year == dt.datetime.now().year:
-                    obs_on = self.obs.observed_on.strftime("%-d-%b")
-                else:
-                    obs_on = self.obs.observed_on.strftime("%b-%Y")
-            else:
-                obs_on = self.obs.observed_on.strftime("%a %b %-d, %Y · %-I:%M %P")
+        if obs.observed_on:
+            obs_on = format_datetime(obs.observed_on, compact)
+            if not compact:
                 summary += " on " + obs_on
-        if self.obs.place_guess:
-            if self.compact:
-                obs_at = self.obs.place_guess
+        if obs.place_guess:
+            if compact:
+                obs_at = obs.place_guess
             else:
-                summary += " at " + self.obs.place_guess
-        if self.compact:
+                summary += " at " + obs.place_guess
+        if compact:
             line = " ".join((item for item in (login, obs_on, obs_at) if item))
             if len(line) > 32:
                 line = line[0:31] + "…"
             summary += "`{0: <32}`".format(line)
-            summary += ICONS[self.obs.quality_grade]
-            if self.obs.faves:
-                summary += self.format_count("fave", len(self.obs.faves))
-            if self.obs.comments:
-                summary += self.format_count("comment", len(self.obs.comments))
-            summary += self.format_media_counts(self.obs)
-        if self.with_description and self.obs.description:
+            summary += ICONS[obs.quality_grade]
+            if obs.faves:
+                summary += self.format_count("fave", len(obs.faves))
+            if obs.comments:
+                summary += self.format_count("comment", len(obs.comments))
+            summary += self.format_media_counts()
+        if with_description and obs.description:
             # Contribute up to 10 lines from the description, and no more
             # than 500 characters:
             #
             # TODO: if https://bugs.launchpad.net/beautifulsoup/+bug/1873787 is
             # ever fixed, suppress the warning instead of adding this blank
             # as a workaround.
-            text_description = html2markdown.convert(" " + self.obs.description)
+            text_description = html2markdown.convert(" " + obs.description)
             lines = text_description.split("\n", 11)
             description = "\n> %s" % "\n> ".join(lines[:10])
             if len(lines) > 10:
                 description += "\n> …"
             if len(description) > 500:
                 description = description[:498] + "…"
             summary += description + "\n"
         return summary
 
     def format_community_id(self, title, summary, taxon_summary):
         idents_count = ""
         if self.obs.identifications_count:
             if self.obs.community_taxon_id:
-                (idents_count, idents_agree) = self.count_community_id()
+                (idents_count, idents_agree) = self.obs.cumulative_ids
                 idents_count = f"{ICONS['community']} ({idents_agree}/{idents_count})"
             else:
                 obs_idents_count = (
                     self.obs.identifications_count
                     if self.obs.identifications_count > 1
                     else ""
                 )
                 idents_count = f"{ICONS['ident']}{obs_idents_count}"
         if (
             not self.compact
             and self.obs.community_taxon_id
-            and self.obs.community_taxon_id != self.obs.taxon.id
+            and self.obs.community_taxon_id != self.taxon.id
         ):
             means_link = ""
             status_link = ""
             if taxon_summary:
                 means = taxon_summary.listed_taxon
                 status = taxon_summary.conservation_status
                 if status:
                     status_link = (
                         "\nConservation Status: "
                         f"{format_taxon_conservation_status(status)}"
                     )
                 if means:
                     means_link = f"\n{format_taxon_establishment_means(means)}"
+            community_taxon_str = f"{format_taxon_name(self.community_taxon)}"
+            if self.with_link:
+                community_taxon_str = self.format_taxon_link(self.community_taxon)
             summary = (
-                f"{format_taxon_name(self.community_taxon)} "
-                f"{status_link}{idents_count}{means_link}\n\n" + summary
+                f"Community Taxon: {community_taxon_str} {status_link}{idents_count}{means_link}\n"
+                + summary
             )
         else:
             if idents_count:
                 if self.compact:
                     summary += " " + idents_count
                 else:
                     title += " " + idents_count
@@ -778,46 +806,14 @@
         media_counts = ""
         if self.obs.photos:
             media_counts += self.format_count("image", len(self.obs.photos))
         if self.obs.sounds:
             media_counts += self.format_count("sound", len(self.obs.sounds))
         return media_counts
 
-    def count_community_id(self):
-        idents_count = 0
-        idents_agree = 0
-
-        ident_taxon_ids = []
-        # TODO: when pyinat supports ident_taxon_ids, this can be removed.
-        for ident in self.obs.identifications:
-            if ident.taxon:
-                for ancestor_id in ident.taxon.ancestor_ids:
-                    if ancestor_id not in ident_taxon_ids:
-                        ident_taxon_ids.append(ancestor_id)
-                if ident.taxon.id not in ident_taxon_ids:
-                    ident_taxon_ids.append(ident.taxon.id)
-        for identification in self.obs.identifications:
-            if identification.current:
-                user_taxon_id = identification.taxon.id
-                user_taxon_ids = identification.taxon.ancestor_ids
-                user_taxon_ids.append(user_taxon_id)
-                if self.obs.community_taxon_id in user_taxon_ids:
-                    if user_taxon_id in ident_taxon_ids:
-                        # Count towards total & agree:
-                        idents_count += 1
-                        idents_agree += 1
-                    else:
-                        # Neither counts for nor against
-                        pass
-                else:
-                    # Maverick counts against:
-                    idents_count += 1
-
-        return (idents_count, idents_agree)
-
 
 class QualifiedTaxonFormatter(TaxonFormatter):
     def __init__(
         self,
         query_response: QueryResponse,
         observations: JsonResponse = None,
         **kwargs,
```

### Comparing `dronefly_core-0.3.5/dronefly/core/models/controlled_terms.py` & `dronefly_core-0.3.6.dev0/dronefly/core/models/controlled_terms.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/dronefly/core/parsers/constants.py` & `dronefly_core-0.3.6.dev0/dronefly/core/parsers/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/dronefly/core/parsers/natural.py` & `dronefly_core-0.3.6.dev0/dronefly/core/parsers/natural.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/dronefly/core/parsers/unixlike.py` & `dronefly_core-0.3.6.dev0/dronefly/core/parsers/unixlike.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/dronefly/core/parsers/url.py` & `dronefly_core-0.3.6.dev0/dronefly/core/parsers/url.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/dronefly/core/query/query.py` & `dronefly_core-0.3.6.dev0/dronefly/core/query/query.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/dronefly/core/utils/__init__.py` & `dronefly_core-0.3.6.dev0/dronefly/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.5/pyproject.toml` & `dronefly_core-0.3.6.dev0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 exclude_dirs = ["tests"]
 
 [tool.flake8]
 max-line-length = 100
 
 [tool.poetry]
 name = "dronefly-core"
-version = "0.3.5"
+version = "0.3.6.dev0"
 description = "Core dronefly components"
 authors = ["Ben Armstrong <synrg@debian.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
 	{ include = "dronefly/core" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-pyinaturalist = ">=0.18,<0.20"
+pyinaturalist = ">=0.19.0.dev2,<0.20"
 dateparser = "^1.1.1"
 inflect = "^5.3.0"
 rich = ">=10.9,<14"
 attrs = ">=21.2"
 html2markdown = "^0.1.7"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `dronefly_core-0.3.5/PKG-INFO` & `dronefly_core-0.3.6.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dronefly-core
-Version: 0.3.5
+Version: 0.3.6.dev0
 Summary: Core dronefly components
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=21.2)
 Requires-Dist: dateparser (>=1.1.1,<2.0.0)
 Requires-Dist: html2markdown (>=0.1.7,<0.2.0)
 Requires-Dist: inflect (>=5.3.0,<6.0.0)
-Requires-Dist: pyinaturalist (>=0.18,<0.20)
+Requires-Dist: pyinaturalist (>=0.19.0.dev2,<0.20)
 Requires-Dist: rich (>=10.9,<14)
 Description-Content-Type: text/markdown
 
 # Dronefly core
 
 This is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)
 Discord bot's core components. We're not yet making version guarantees until
```

