# Comparing `tmp/housenomics-0.0.9.tar.gz` & `tmp/housenomics-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "housenomics-0.0.9.tar", max compression
+gzip compressed data, was "housenomics-1.2.4.tar", max compression
```

## Comparing `housenomics-0.0.9.tar` & `housenomics-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,24 @@
--rw-r--r--   0        0        0     1211 2022-08-12 18:05:08.000000 housenomics-0.0.9/LICENSE
--rw-r--r--   0        0        0     1099 2023-02-15 08:57:15.746494 housenomics-0.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-12 18:05:08.000000 housenomics-0.0.9/src/housenomics/__init__.py
--rw-r--r--   0        0        0        0 2022-11-14 20:48:08.000000 housenomics-0.0.9/src/housenomics/application/__init__.py
--rw-r--r--   0        0        0      184 2023-02-04 09:42:37.647818 housenomics-0.0.9/src/housenomics/application/import_transactions.py
--rw-r--r--   0        0        0      281 2023-02-15 08:44:00.551860 housenomics-0.0.9/src/housenomics/application/list_transactions.py
--rw-r--r--   0        0        0     1287 2023-02-14 21:53:36.272822 housenomics-0.0.9/src/housenomics/application/views/transactions.py
--rw-r--r--   0        0        0     1736 2023-02-04 09:42:37.648096 housenomics-0.0.9/src/housenomics/infrastructure/cgd_csv_file.py
--rw-r--r--   0        0        0      201 2023-02-04 09:42:37.648242 housenomics-0.0.9/src/housenomics/infrastructure/transactions.py
--rw-r--r--   0        0        0      386 2023-02-14 21:21:41.435788 housenomics-0.0.9/src/housenomics/transaction.py
--rw-r--r--   0        0        0        0 2023-02-04 09:42:37.648453 housenomics-0.0.9/src/housenomics/ui/cli/__init__.py
--rw-r--r--   0        0        0     2907 2023-02-15 08:57:01.254278 housenomics-0.0.9/src/housenomics/ui/cli/main.py
--rw-r--r--   0        0        0      670 2023-02-09 17:59:03.622478 housenomics-0.0.9/src/toolbox/database.py
--rw-r--r--   0        0        0     1291 1970-01-01 00:00:00.000000 housenomics-0.0.9/setup.py
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 housenomics-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-05 20:39:03.022505 housenomics-1.2.4/LICENSE
+-rw-r--r--   0        0        0     1311 2023-06-03 19:45:48.704560 housenomics-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.032709 housenomics-1.2.4/src/housenomics/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.033041 housenomics-1.2.4/src/housenomics/application/__init__.py
+-rw-r--r--   0        0        0      787 2023-04-06 08:51:23.764662 housenomics-1.2.4/src/housenomics/application/import_transactions.py
+-rw-r--r--   0        0        0      572 2023-05-28 21:46:38.921062 housenomics-1.2.4/src/housenomics/application/import_transactions_test.py
+-rw-r--r--   0        0        0      758 2023-04-14 20:32:53.007626 housenomics-1.2.4/src/housenomics/application/repositories/transactions.py
+-rw-r--r--   0        0        0     1803 2023-04-05 20:39:03.034847 housenomics-1.2.4/src/housenomics/application/views/transactions.py
+-rw-r--r--   0        0        0     4981 2023-05-22 14:25:53.731138 housenomics-1.2.4/src/housenomics/application/views/transactions_test.py
+-rw-r--r--   0        0        0     2983 2023-04-07 14:24:59.019481 housenomics-1.2.4/src/housenomics/infrastructure/gateway_cgd_file.py
+-rw-r--r--   0        0        0     2045 2023-04-14 20:32:53.007236 housenomics-1.2.4/src/housenomics/infrastructure/gateway_cgd_file_test.py
+-rw-r--r--   0        0        0      494 2023-04-14 20:32:53.008002 housenomics-1.2.4/src/housenomics/transaction.py
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.038982 housenomics-1.2.4/src/housenomics/ui/cli/__init__.py
+-rw-r--r--   0        0        0     2451 2023-05-22 14:25:53.732424 housenomics-1.2.4/src/housenomics/ui/cli/main.py
+-rw-r--r--   0        0        0      670 2023-04-05 20:39:03.039671 housenomics-1.2.4/src/housenomics/ui/cli/report.py
+-rw-r--r--   0        0        0      323 2023-04-05 20:39:03.039911 housenomics-1.2.4/src/housenomics/ui/cli/version.py
+-rw-r--r--   0        0        0      479 2023-04-05 20:39:03.041120 housenomics-1.2.4/src/toolbox/cli.py
+-rw-r--r--   0        0        0     2288 2023-05-22 14:25:53.743334 housenomics-1.2.4/src/toolbox/database.py
+-rw-r--r--   0        0        0     1649 2023-05-22 14:25:53.747558 housenomics-1.2.4/src/toolbox/database_test.py
+-rw-r--r--   0        0        0      607 2023-06-03 18:46:28.056797 housenomics-1.2.4/src/toolbox/project.py
+-rw-r--r--   0        0        0     1482 2023-06-03 18:51:23.522195 housenomics-1.2.4/src/toolbox/projects_test.py
+-rw-r--r--   0        0        0       64 2023-04-05 20:39:03.042194 housenomics-1.2.4/src/toolbox/views.py
+-rw-r--r--   0        0        0      143 2023-04-05 20:39:03.042641 housenomics-1.2.4/src/toolbox/views_test.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 housenomics-1.2.4/PKG-INFO
```

### Comparing `housenomics-0.0.9/LICENSE` & `housenomics-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `housenomics-0.0.9/pyproject.toml` & `housenomics-1.2.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,66 @@
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "housenomics"
-version = "0.0.9"
+version = "1.2.4"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
-packages = [
-    { include = "toolbox", from = "src" },
-    { include = "housenomics", from = "src" }
-]
+
+[[tool.poetry.packages]]
+include = "toolbox"
+from = "src"
+
+[[tool.poetry.packages]]
+include = "housenomics"
+from = "src"
+
+[tool.mypy]
+ignore_missing_imports = true
+
+[tool.isort]
+profile = "black"
+multi_line_output = 3
+
+[tool.black]
+max-line-length = 99
+target-version = ["py311"]
 
 [tool.poetry.scripts]
-housenomics = "housenomics.ui.cli.main:app"
+housenomics = "housenomics.ui.cli.main:housenomics_cli.app"
 
 [tool.poetry.dependencies]
-python = "3.11.1"
-rich = "^13.3.1"
-typer = "^0.7.0"
+python = "^3.10"
+rich = "^13.3.5"
+typer = "^0.9.0"
 pendulum = "^2.1.2"
-sqlalchemy = "^2.0.3"
+sqlalchemy = "^2.0.15"
+toml = "^0.10.2"
+toolcat = "0.0.2"
+
+[tool.pytest.ini_options]
+markers = ["integration: tags a test as integration tests"]
+
+[tool.poetry.dev-dependencies.bandit]
+extras = ["toml"]
+version = "^1.7.5"
 
-[tool.poetry.dev-dependencies]
-bandit = { extras = ["toml"], version = "^1.7.4" }
+[tool.poetry.group.dev.dependencies]
 behave = "^1.2.6"
 black = "^23.1.0"
-coverage = "^7.1.0"
+coverage = "^7.2.1"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
-mypy = "^1.0.0"
-pre-commit = "^3.0.4"
+mypy = "^1.0.1"
+pre-commit = "^3.1.1"
 pytest = "^7.2.1"
 pytest-xdist = "^3.2.0"
 pytest-bdd = "^6.1.1"
-types-python-dateutil = "^2.8.19.6"
-types-tabulate = "^0.9.0.0"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.mypy]
-ignore_missing_imports = true
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-
-[tool.black]
-max-line-length = 99
-target-version = ['py311']
+types-toml = "^0.10.8.6"
+types-python-dateutil = "^2.8.19.9"
+types-tabulate = "^0.9.0.1"
```

### Comparing `housenomics-0.0.9/src/housenomics/ui/cli/main.py` & `housenomics-1.2.4/src/housenomics/ui/cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,86 @@
 import logging
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
-import typer
-from sqlalchemy import delete
 from sqlalchemy.orm import Session
 
 from housenomics.application.import_transactions import ServiceImportTransactions
-from housenomics.application.list_transactions import ServiceListTransactions
-from housenomics.application.views.transactions import ViewTransactions
-from housenomics.infrastructure.cgd_csv_file import GatewayCGD
-from housenomics.infrastructure.transactions import Transactions
-from housenomics.transaction import Transaction
+from housenomics.application.repositories.transactions import Transactions
+from housenomics.infrastructure.gateway_cgd_file import GatewayCGDFile
+from housenomics.ui.cli.report import report
+from housenomics.ui.cli.version import CommandVersion
+from toolbox import cli
+from toolbox.cli import CLIApplication
 from toolbox.database import Database
 
 logging_format: dict = {
     "level": logging.CRITICAL,
     "format": "%(asctime)s - %(name)s - %(levelname)s - %(message)s",
 }
 
 logging.basicConfig(**logging_format)
 logger = logging.getLogger(__name__)
 
-application_help = """
-Housenomics helps you manage your personal finances.
-"""
+database_path = Path.home() / Path("Library/Application Support/Housenomics")
 
-app = typer.Typer(add_completion=False, help=application_help)
 
-# SelectOfScalar.inherit_cache = True  # type: ignore
-# Select.inherit_cache = True  # type: ignore
+class HousenomicsCLI(CLIApplication):
+    help = "Housenomics helps you manage your personal finances."
 
 
-@app.command(name="import", help="Imports the transactions to feed the application")
-def import_(file_path: Path):
-    with Session(Database().engine) as session:
-        gateway_cgd = GatewayCGD(file_path)
+housenomics_cli = HousenomicsCLI()
+app = housenomics_cli.app
+housenomics_cli.register_command(CommandVersion)
+
+
+def migrate_database():
+    Database(database_path, Path("migrations/0001 - Initial.sql"))
+
+
+def import_file(file_path: Path):
+    with Session(Database(database_path).engine) as session:
+        gateway_cgd = GatewayCGDFile(file_path)
         transactions = Transactions(session)
-        ServiceImportTransactions().execute(gateway_cgd, transactions)
+        ServiceImportTransactions(gateway_cgd, transactions).execute()
         session.commit()
 
 
-@app.command(name="list", help="Lists all transactions")
-def list_(
-    _: str = typer.Argument(
-        default="transactions",
-        help="The item to be listed",
-    ),
-):
-    with Session(Database().engine) as session:
-        results = ServiceListTransactions().execute(session)
-        for m in results:
-            print(f"Description: '{m.description:>22}', Value: {m.value:>10}")
+@app.command(name="import", help="Imports the transactions to feed the application")
+def import_(file_path: Path):
+    reset()
+    migrate_database()
+    import_file(file_path)
 
 
-@app.command(name="report", help="Reports the transactions filtered by seller")
-def report(
-    seller: str,
-    since: Optional[datetime] = typer.Option(
+@app.command(name="report", help="Builds reports according to filters")
+def report_(
+    seller: Optional[str] = cli.Option(default="", help="Filters report by Seller"),
+    since: Optional[datetime] = cli.Option(
         default=None, help="Show report since specified date"
     ),
-    on: Optional[datetime] = typer.Option(
+    on: Optional[datetime] = cli.Option(
         default=None, help="Show report on specified date"
     ),
 ):
-    with Session(Database().engine) as session:
-        view = ViewTransactions(session, seller, since, on)
+    migrate_database()
+    report(database_path, seller, since, on)
 
-    print(f"Lookup: '{seller}', Value: {round(view.data, 2)}")
 
-
-@app.command(name="version", help="Shows current version")
-def version():
-    typer.echo("0.0.9")
+def reset():
+    db = Database(database_path)
+    db.remove()
 
 
 @app.command(
     name="reset",
     help="Deletes all financial information from the application",
 )
-def reset():
-    delete_information = typer.confirm(
+def reset_():
+    delete_information = cli.confirm(
         "Are you sure you want to delete all financial information ?"
     )
     if not delete_information:
-        raise typer.Abort()
-
-    with Session(Database().engine) as session:
-        statement = delete(Transaction)
-        session.execute(statement)
-        session.commit()
-
+        raise cli.Abort()
 
-if __name__ == "__main__":
-    app()
+    reset()
```

