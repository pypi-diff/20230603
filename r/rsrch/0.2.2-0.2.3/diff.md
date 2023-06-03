# Comparing `tmp/rsrch-0.2.2.tar.gz` & `tmp/rsrch-0.2.3.tar.gz`

## Comparing `rsrch-0.2.2.tar` & `rsrch-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.2.2/.DS_Store
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 rsrch-0.2.2/examples/yitay.md
--rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.2.2/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.2.3/.DS_Store
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 rsrch-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 rsrch-0.2.3/requirements.txt
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 rsrch-0.2.3/examples/yitay.md
+-rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.2.3/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
 Understanding_and_Reduce_the_Spread_of_Misinformation.pdf
--rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.2.2/papers/Decision_Transformer:_Reinforcement
+-rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.2.3/papers/Decision_Transformer:_Reinforcement
 Learning_via_Sequence_Modeling.pdf
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.2.2/rsrch/__about__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 rsrch-0.2.2/rsrch/__init__.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 rsrch-0.2.2/rsrch/_src/labml.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 rsrch-0.2.2/rsrch/_src/notion.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 rsrch-0.2.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.2.2/LICENSE
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 rsrch-0.2.2/README.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rsrch-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 rsrch-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.2.3/rsrch/__about__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 rsrch-0.2.3/rsrch/__init__.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 rsrch-0.2.3/rsrch/_src/notion.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 rsrch-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 rsrch-0.2.3/README.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 rsrch-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 rsrch-0.2.3/PKG-INFO
```

### Comparing `rsrch-0.2.2/.DS_Store` & `rsrch-0.2.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.2/examples/yitay.md` & `rsrch-0.2.3/examples/yitay.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 Let's say you were browsing Twitter and you saw a tweet from Yi Tay, a researcher at Google Brain, about his [favorite NLP papers from 2022](https://www.yitay.net/blog/2022-best-nlp-papers). You want to download them all, but you don't want to click on each link and download them one by one.
 
 With a few lines of Python and a call to `rsrch`, you can download all of the papers in a single command.
 
 ```python
 import requests
 import re
-import rsrch
+from rsrch import RsrchClient
 
 # Get the HTML of the page
 html = requests.get("https://www.yitay.net/blog/2022-best-nlp-papers").text
 
 # Regex match all arXiv abstracts
 matches = re.findall(r"https:\/\/arxiv\.org\/abs\/[\w\-]+\.[\w\-]+", html)
 
-# Concatenate all the matches into a single string and remove quotes
-urls = " ".join(matches).replace('"', '')
+# Concatenate all the matches into a single string, remove quotes, and make a list
+urls = " ".join(matches).replace('"', '').split()
 
-# Upload the links to Notion and download the papers
+# Upload the links to Notion and download the paper PDFs
+rsrch = RsrchClient(token="your_notion_token", database="your_notion_database")
 rsrch.upload(urls)
 rsrch.download()
-```
+```
```

### Comparing `rsrch-0.2.2/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf` & `rsrch-0.2.3/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.2/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf` & `rsrch-0.2.3/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.2/rsrch/_src/notion.py` & `rsrch-0.2.3/rsrch/_src/notion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,181 +1,162 @@
 import math
 import os
+from typing import List, Union
 
 import arxiv
 import requests
-import urllib3
-from dotenv import load_dotenv
 from notion_client import Client
 from tqdm import tqdm
 
 
-def fetch_table():
-    notion = Client(auth=os.getenv("NOTION_TOKEN"))
-    paper_db = notion.databases.query(database_id=os.getenv("NOTION_DATABASE_ID"))
-
-    papers = []
-    for paper in paper_db["results"]:
-        if not paper["properties"]["Title"]["title"] == []:
-            title = paper["properties"]["Title"]["title"][0]["plain_text"]
-            url = paper["properties"]["URL"]["url"]
-            date = paper["properties"]["Date"]["date"]["start"]
-            authors = paper["properties"]["Authors"]["rich_text"][0]["plain_text"]
-            if not url == None and url.startswith("http"):
-                papers.append((title, url, date, authors))
-
-    return papers
-
-
-def download():
+class RsrchClient:
     """
-    Downloads papers from Notion.
-
-    Returns:
-        None
-
-    Downloads papers from the Notion database.
-    Paper URLs are fetched from the table using the 'fetch_table' function.
-    The downloaded papers are saved in a 'papers' directory.
-    Existing files are skipped.
-    Prints progress information for each paper being downloaded.
-
-    Note:
-        - Requires the 'python-dotenv', 'urllib3', 'requests', and 'tqdm' libraries.
-        - 'fetch_table' function is assumed to be defined elsewhere.
-
-    Example Usage:
-        download()
-    """
-    print("Downloading papers from Notion...")
-    urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-    load_dotenv()
-    papers = fetch_table()
-
-    if not os.path.exists("papers"):
-        os.mkdir("papers")
-
-    for title, url, _, _ in papers:
-        path = f"papers/{title.replace(' ', '_')}.pdf"
-        if not os.path.exists(path):
-            print(f'\nDownloading "{title}"')
-            try:
-                r = requests.get(url, stream=True, verify=True)
-            except requests.exceptions.SSLError:
-                r = requests.get(url, stream=True, verify=False)
-
-            with open(path, "wb") as f:
-                for chunk in tqdm(
-                    r.iter_content(chunk_size=1024),
-                    total=math.ceil(int(r.headers["Content-Length"]) / 1024),
-                    unit="KB",
-                ):
-                    if chunk:
-                        f.write(chunk)
-
-
-def create_paper(notion, title, url, date, authors):
-    notion.pages.create(
-        parent={
-            "database_id": os.getenv("NOTION_DATABASE_ID"),
-        },
-        properties={
-            "Title": {
-                "title": [
-                    {
-                        "text": {
-                            "content": title,
-                        },
-                    },
-                ],
-            },
-            "URL": {
-                "url": url,
-            },
-            "Date": {
-                "date": {
-                    "start": date,
-                },
-            },
-            "Authors": {
-                "rich_text": [
-                    {
-                        "text": {
-                            "content": authors,
-                        },
-                    },
-                ],
-            },
-        },
-    )
+    A class to interface with the Notion API and perform operations related to research papers.
 
-    print(f"- {title}")
-
-
-def upload(arxiv_urls):
+    Attributes
+    ----------
+    notion : Client
+        The Notion API client.
+    database_id : str
+        The ID of the database in Notion.
     """
-    Uploads papers from arXiv to Notion.
-
-    Parameters:
-        arxiv_urls (list): List of arXiv URLs or IDs.
 
-    Returns:
-        None
-
-    Connects to Notion API and uploads papers from arXiv.
-    Creates new papers in Notion, skipping existing ones.
-    Prints "Done!" when finished.
-
-    Example:
-        urls = [
-            "https://arxiv.org/abs/2105.12345",
-            "https://arxiv.org/abs/2106.67890",
-            "https://arxiv.org/pdf/2107.24680.pdf"
+    def __init__(self, token: str, database_id: str):
+        """
+        Initializes the RsrchClient with the provided API key and database ID.
+
+        Parameters
+        ----------
+        token : str
+            The API key for Notion. If not provided, raises a ValueError.
+        database_id : str
+            The ID of the database in Notion. If not provided, raises a ValueError.
+        """
+        if not token:
+            raise ValueError("API key must be provided.")
+        if not database_id:
+            raise ValueError("Database ID must be provided.")
+
+        self.notion = Client(auth=token)
+        self.database_id = database_id
+
+    def _get_paper_properties(self, paper):
+        title = paper["properties"]["Title"]["title"][0]["plain_text"]
+        url = paper["properties"]["URL"]["url"]
+        date = paper["properties"]["Date"]["date"]["start"]
+        authors = paper["properties"]["Authors"]["rich_text"][0]["plain_text"]
+        return title, url, date, authors
+
+    def fetch_table(self):
+        """
+        Retrieves the data of all papers in the Notion database.
+
+        Returns
+        -------
+        list
+            A list of tuples, where each tuple contains the title, URL, date, and authors of a paper.
+        """
+        paper_db = self.notion.databases.query(database_id=self.database_id)
+        papers = [
+            self._get_paper_properties(paper) for paper in paper_db["results"] if paper["properties"]["Title"]["title"]
         ]
-        upload(urls)
-    """
-    load_dotenv()
-    notion = Client(auth=os.getenv("NOTION_TOKEN"))
+        return [paper for paper in papers if paper[1] and paper[1].startswith("http")]
 
-    # Extract arXiv IDs from valid URLs
-    ids = []
-    for url in arxiv_urls:
+    def _save_paper(self, r, path):
+        with open(path, "wb") as f:
+            for chunk in tqdm(
+                r.iter_content(chunk_size=1024),
+                total=math.ceil(int(r.headers["Content-Length"]) / 1024),
+                unit="KB",
+            ):
+                if chunk:
+                    f.write(chunk)
+
+    def download(self):
+        """
+        Downloads all papers from the Notion database and saves them as PDFs.
+
+        The papers are saved in a directory named "papers". Each paper is saved as a separate PDF file.
+
+        If a paper has already been downloaded (i.e., a PDF file with the same name exists in the directory),
+        the download is skipped for that paper.
+
+        All download progress is logged to the console.
+        """
+        print("Downloading papers from Notion...")
+        papers = self.fetch_table()
+
+        if not os.path.exists("papers"):
+            os.mkdir("papers")
+
+        for title, url, _, _ in papers:
+            path = f"papers/{title.replace(' ', '_')}.pdf"
+            if not os.path.exists(path):
+                print(f'\nDownloading "{title}"')
+                r = requests.get(url, stream=True)
+                self._save_paper(r, path)
+
+    def create_paper(self, title, url, date, authors):
+        self.notion.pages.create(
+            parent={"database_id": self.database_id},
+            properties={
+                "Title": {"title": [{"text": {"content": title}}]},
+                "URL": {"url": url},
+                "Date": {"date": {"start": date}},
+                "Authors": {"rich_text": [{"text": {"content": authors}}]},
+            },
+        )
+        print(f"- {title}")
+
+    def _extract_arxiv_id(self, url):
         if url.startswith("https://arxiv.org/abs/"):
-            ids.append(url.replace("https://arxiv.org/abs/", ""))
+            return url.replace("https://arxiv.org/abs/", "")
         elif url.startswith("https://arxiv.org/pdf/") and url.endswith(".pdf"):
-            ids.append(url.replace("https://arxiv.org/pdf/", "").replace(".pdf", ""))
-        elif requests.get("https://arxiv.org/abs/" + url).status_code == 200:
-            ids.append(url)
+            return url.replace("https://arxiv.org/pdf/", "").replace(".pdf", "")
+        elif requests.get(f"https://arxiv.org/abs/{url}").status_code == 200:
+            return url
         else:
             print(f"ERROR: {url} is not a valid arXiv abstract URL, PDF URL, or ID.")
+            return None
 
-    # Fetch titles of papers already in Notion
-    papers = fetch_table()
-    titles = [title for title, _, _, _ in papers]
-
-    # Fetch paper data from arXiv
-    print("Uploading papers to Notion...\n")
-    results = arxiv.Search(id_list=ids)
-    for paper in results.results():
-        # Date is in ISO 8601 format, e.g. 2020-01-01
-        date = paper.published.isoformat().split("T")[0]
-
-        # Paper title
-        title = paper.title
-
-        # Paper authors (max 5)
-        authors = [author.name for author in paper.authors]
-        if len(authors) > 5:
-            authors = ", ".join(authors[:5]) + ", et al."
-        else:
-            authors = ", ".join(authors)
-
-        # Paper URL
-        pdf_url = paper.pdf_url
-
-        # Create paper in Notion if it doesn't already exist
-        if title not in titles:
-            create_paper(notion, title, pdf_url, date, authors)
-        else:
-            print(f"- {title} (already exists)")
+    def upload(self, arxiv_urls: Union[List[str], str]):
+        """
+        Uploads papers from arXiv to the Notion database.
+
+        The papers to upload are specified by providing their arXiv URLs.
+
+        If a paper with the same title already exists in the database, the upload is skipped for that paper.
+
+        Parameters
+        ----------
+        arxiv_urls : list of str
+            The arXiv URLs of the papers to upload.
+        """
+        if isinstance(arxiv_urls, str):
+            arxiv_urls = [arxiv_urls]
+
+        ids = [self._extract_arxiv_id(url) for url in arxiv_urls if self._extract_arxiv_id(url)]
+        if not ids:
+            raise ValueError("No valid arXiv URLs provided.")
+
+        papers = self.fetch_table()
+        titles = [title for title, _, _, _ in papers]
+
+        print("Uploading papers to Notion...\n")
+        results = arxiv.Search(id_list=ids)
+        for paper in results.results():
+            date = paper.published.isoformat().split("T")[0]
+            title = paper.title
+            authors = [author.name for author in paper.authors]
+            if len(authors) > 5:
+                authors = ", ".join(authors[:5]) + ", et al."
+            else:
+                authors = ", ".join(authors)
+
+            pdf_url = paper.pdf_url
+
+            if title not in titles:
+                self.create_paper(title, pdf_url, date, authors)
+            else:
+                print(f"- {title} (already exists)")
 
-    print("\nDone!")
+        print("\nDone!")
```

### Comparing `rsrch-0.2.2/LICENSE` & `rsrch-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.2/README.md` & `rsrch-0.2.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,21 +6,15 @@
 </p>
 
 ## Installation
 1. Create an [internal integration](https://www.notion.so/help/create-integrations-with-the-notion-api) in Notion.
 
 2. [Add the integration](https://www.notion.so/help/add-and-manage-connections-with-the-api#add-connections-to-pages) to the database you want to download from.
 
-3. Create a `.env` file with the following variables:
-
-    ```
-    NOTION_TOKEN=secret_XXXXXXXX
-    NOTION_DATABASE_ID=XXXXXXXXXXXXXXXX
-    ```
-    Your `NOTION_TOKEN` can be found in your [integrations page](https://www.notion.so/my-integrations) and is called the **Internal Integration Token**. The `NOTION_DATABASE_ID` can be found in the [URL of your database](https://www.notion.so/my-integrations) (`https://www.notion.so/{workspace_name}/{database_id}?v={view_id}`).
+3. Store your `NOTION_TOKEN` and `NOTION_DATABASE_ID` somewhere safe. Your `NOTION_TOKEN` can be found in your [integrations page](https://www.notion.so/my-integrations) and is called the **Internal Integration Token**. The `NOTION_DATABASE_ID` can be found in the [URL of your database](https://www.notion.so/my-integrations) (`https://www.notion.so/{workspace_name}/{database_id}?v={view_id}`).
 
 4. Install local dependencies:
 
     ```bash
     pip install rsrch
     ```
 
@@ -29,57 +23,58 @@
     - **URL**: `URL`
     - **Date**: `Date`
     - **Authors**: `Text`
 
     You can add more columns, but these are the ones that are required.
 
 ## Usage
+### Setup
+```python
+from rsrch import RsrchClient
+
+client = RsrchClient(
+    token=NOTION_TOKEN,
+    database_id=NOTION_DATABASE_ID,
+)
+```
+
 ### Download
 This will download all the papers from your Notion database to the `papers/` directory.
 
 ```python
-from rsrch import download
-download()
+client.download()
 ```
 
 <p>
     <img width="1097" alt="image" src="https://user-images.githubusercontent.com/47067154/232264456-4bdef487-36e8-4627-95c3-82f5c3876082.png">
 </p>
 
 ### Upload
 You can upload arXiv abstract links, PDF links, or IDs to your Notion database and have it autofill all of the relevant fields.
 
 ```python
-from rsrch import upload
-upload()
+client.upload(
+    arxiv_urls=[
+        "https://arxiv.org/abs/1706.03762",
+        "https://arxiv.org/pdf/1706.03762.pdf",
+        "1706.03762",
+    ]
+)
 ```
 
 <p>
     <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/232264615-82b42d8c-ca1c-4f21-899f-439a6c8a7879.png">
 </p>
 
 Alternatively, you can add non-arXiv links manually to Notion.
 
-### Popular
-You can get the most popular papers from this day, week, or month from the [LabML database](https://papers.labml.ai/).
-
-```python
-from rsrch import popular
-popular(sort_by="weekly", num_papers=10)
-```
-
-<p>
-    <img width="1095" alt="image" src="https://github.com/ishan0102/rsrch/assets/47067154/b99197a1-8556-4469-82f4-786a4c974447">
-</p>
-
-
 ## Notes
 - Uploading papers to Notion is currently only supported for arXiv links. Papers with titles that already exist in the database will not be uploaded.
 - I plan on adding support for other databases in the future, but for now it only works with Notion databases.
 - To build and release this:
   - Make new code accessible in `src/__init__.py`
   - Update the version in `src/__about__.py`
   - Run `python3 -m build`
   - Run `python3 -m twine upload dist/*`
 
 ### Resources
-- [Notion API](https://developers.notion.com/)
+- [Notion API](https://developers.notion.com/)
```

### Comparing `rsrch-0.2.2/pyproject.toml` & `rsrch-0.2.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -13,22 +13,17 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "arxiv==1.4.2",
-    "click==8.1.3",
     "notion-client==2.0.0",
-    "python-dotenv==0.21.0",
     "requests==2.28.1",
-    "rich==13.3.4",
-    "selenium==4.9.1",
     "tqdm==4.64.1",
-    "urllib3==1.26.13",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/ishan0102/rsrch"
 "Bug Tracker" = "https://github.com/ishan0102/rsrch/issues"
```

### Comparing `rsrch-0.2.2/PKG-INFO` & `rsrch-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,38 @@
 Metadata-Version: 2.1
 Name: rsrch
-Version: 0.2.2
+Version: 0.2.3
 Summary: Manage your ever-growing list of research papers
 Project-URL: Homepage, https://github.com/ishan0102/rsrch
 Project-URL: Bug Tracker, https://github.com/ishan0102/rsrch/issues
 Author-email: Ishan Shah <ishan0102@utexas.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: arxiv==1.4.2
-Requires-Dist: click==8.1.3
 Requires-Dist: notion-client==2.0.0
-Requires-Dist: python-dotenv==0.21.0
 Requires-Dist: requests==2.28.1
-Requires-Dist: rich==13.3.4
-Requires-Dist: selenium==4.9.1
 Requires-Dist: tqdm==4.64.1
-Requires-Dist: urllib3==1.26.13
 Description-Content-Type: text/markdown
 
 # rsrch
 Manage your research papers from Python. This project lets you update a Notion database with arXiv links and download PDFs of papers to your local machine.
 
 <p align="center">
     <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/219932040-ab4962f8-b01e-4d94-9eba-77a155b0e933.png">
 </p>
 
 ## Installation
 1. Create an [internal integration](https://www.notion.so/help/create-integrations-with-the-notion-api) in Notion.
 
 2. [Add the integration](https://www.notion.so/help/add-and-manage-connections-with-the-api#add-connections-to-pages) to the database you want to download from.
 
-3. Create a `.env` file with the following variables:
-
-    ```
-    NOTION_TOKEN=secret_XXXXXXXX
-    NOTION_DATABASE_ID=XXXXXXXXXXXXXXXX
-    ```
-    Your `NOTION_TOKEN` can be found in your [integrations page](https://www.notion.so/my-integrations) and is called the **Internal Integration Token**. The `NOTION_DATABASE_ID` can be found in the [URL of your database](https://www.notion.so/my-integrations) (`https://www.notion.so/{workspace_name}/{database_id}?v={view_id}`).
+3. Store your `NOTION_TOKEN` and `NOTION_DATABASE_ID` somewhere safe. Your `NOTION_TOKEN` can be found in your [integrations page](https://www.notion.so/my-integrations) and is called the **Internal Integration Token**. The `NOTION_DATABASE_ID` can be found in the [URL of your database](https://www.notion.so/my-integrations) (`https://www.notion.so/{workspace_name}/{database_id}?v={view_id}`).
 
 4. Install local dependencies:
 
     ```bash
     pip install rsrch
     ```
 
@@ -52,57 +41,58 @@
     - **URL**: `URL`
     - **Date**: `Date`
     - **Authors**: `Text`
 
     You can add more columns, but these are the ones that are required.
 
 ## Usage
+### Setup
+```python
+from rsrch import RsrchClient
+
+client = RsrchClient(
+    token=NOTION_TOKEN,
+    database_id=NOTION_DATABASE_ID,
+)
+```
+
 ### Download
 This will download all the papers from your Notion database to the `papers/` directory.
 
 ```python
-from rsrch import download
-download()
+client.download()
 ```
 
 <p>
     <img width="1097" alt="image" src="https://user-images.githubusercontent.com/47067154/232264456-4bdef487-36e8-4627-95c3-82f5c3876082.png">
 </p>
 
 ### Upload
 You can upload arXiv abstract links, PDF links, or IDs to your Notion database and have it autofill all of the relevant fields.
 
 ```python
-from rsrch import upload
-upload()
+client.upload(
+    arxiv_urls=[
+        "https://arxiv.org/abs/1706.03762",
+        "https://arxiv.org/pdf/1706.03762.pdf",
+        "1706.03762",
+    ]
+)
 ```
 
 <p>
     <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/232264615-82b42d8c-ca1c-4f21-899f-439a6c8a7879.png">
 </p>
 
 Alternatively, you can add non-arXiv links manually to Notion.
 
-### Popular
-You can get the most popular papers from this day, week, or month from the [LabML database](https://papers.labml.ai/).
-
-```python
-from rsrch import popular
-popular(sort_by="weekly", num_papers=10)
-```
-
-<p>
-    <img width="1095" alt="image" src="https://github.com/ishan0102/rsrch/assets/47067154/b99197a1-8556-4469-82f4-786a4c974447">
-</p>
-
-
 ## Notes
 - Uploading papers to Notion is currently only supported for arXiv links. Papers with titles that already exist in the database will not be uploaded.
 - I plan on adding support for other databases in the future, but for now it only works with Notion databases.
 - To build and release this:
   - Make new code accessible in `src/__init__.py`
   - Update the version in `src/__about__.py`
   - Run `python3 -m build`
   - Run `python3 -m twine upload dist/*`
 
 ### Resources
-- [Notion API](https://developers.notion.com/)
+- [Notion API](https://developers.notion.com/)
```

