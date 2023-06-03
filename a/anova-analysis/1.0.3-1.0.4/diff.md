# Comparing `tmp/anova_analysis-1.0.3.tar.gz` & `tmp/anova_analysis-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anova_analysis-1.0.3.tar", last modified: Wed May 31 19:35:09 2023, max compression
+gzip compressed data, was "anova_analysis-1.0.4.tar", last modified: Sat Jun  3 03:16:18 2023, max compression
```

## Comparing `anova_analysis-1.0.3.tar` & `anova_analysis-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/anova_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/anova_analysis/ANOVA_RBD.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/anova_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/anova_analysis/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/anova_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/anova_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/anova_analysis/ANOVA_RBD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/anova_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/anova_analysis/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/anova_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/setup.py
```

### Comparing `anova_analysis-1.0.3/LICENSE.txt` & `anova_analysis-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anova_analysis-1.0.3/PKG-INFO` & `anova_analysis-1.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: anova_analysis
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for performing ANOVA analysis by RBD
 Home-page: https://github.com/Insight-deviler/anova_analysis
 Author-email: insightagri10@gmail.com
 License: MIT
-Keywords: python,ANOVA,Two-way ANOVA,RBD,analysis of variance
+Keywords: line x tester,lxt,Line x Tester,Line Tester,Genetics and Plant breeding,Quantitative Genetics,ANOVA,Two-way ANOVA,RBD,analysis of variance
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -17,34 +17,57 @@
 
 The ANOVA Analysis Package is a Python package that provides functions for performing ``Two-Way ANOVA (Analysis of Variance) analysis`` on experimental data.
 Currently it can perform RBD analysis only
 
 ## Installation
 
 You can install the package using pip:
-
 ```
 pip install anova_analysis
 ```
 ## Usage
 
+- If you just want the output as a file:
 ```
 from anova_analysis import ANOVA_RBD
 
-#Set the replication, treatment, input_file path and output_file_name
+ #Set the replication, treatment, input_file path and output_file_name
 
 replication = 4
 treatment = 23
 input_file_path = "data/MODEL_DATA.xlsx"
 output_file_name = "test"
 
-# Perform ANOVA analysis
+ #Perform ANOVA analysis
 
 ANOVA_RBD.RBD(replication, treatment, input_file_path, output_file_name )
 ```
+- If you want the output to be used in for further analysis, 
+you can then access the calculated values from the ``result`` dictionary:
+```
+result = ANOVA_RBD.RBD(replication, treatment, input_file_path, output_file_name)
+```
+- To access the ``result`` use the following
+```
+CF = result["correction_factor"]
+TSS = result["total_sum_of_square"]
+RSS = result["replication_sum_of_square"]
+TSS = result["treatment_sum_of_square"]
+ESS = result["error_sum_of_square"]
+Rdf = result["replication_df"]
+Tdf = result["treatment_df"],
+Edf = result["errors_df"],
+RMSS = result["rep_mean_ss"],
+TMSS = result["tre_mean_ss"],
+EMSS = result["error_mean_ss"]
+
+# Where CF, TSS,.. are variables
+```
+-  You can easily access them in your other Python file and use them as needed. Modify the returned data structure to suit your preferences and the specific values you want to access.
+
 ## Features
 
 - Calculates the correction factor, total sum of squares, replication sum of squares, treatment sum of squares, and error sum of squares.
 - Generates an ANOVA table with the source, degrees of freedom, sum of squares, mean square, F-values, and p-values at the 5% and 1% significance levels.
 - Performs significance testing at the 5% and 1% levels to determine the statistical significance of the factors.
 - Saves the ANOVA results in a text file for further analysis or reporting purposes.
 
@@ -56,26 +79,27 @@
                 | Genotypes | R1    | R2     | R3     | R4     |
                 |-----------|-------|--------|--------|--------|
                 | 1x6       | 74.4  | 70.86  | 60.94  | 68     |
                 | 1x7       | 91.82 | 99.18  | 118.88 | 120.68 |
                 | 1x8       | 48.08 | 62.1   | 58.54  | 41.84  |
                 | 2x6       | 59.06 | 65.62  | 81.62  | 86.76  |
                 | 2x7       | 84.16 | 109.74 | 102.14 | 94.52  |
+
 - If you have data in the below format, transform it to above said model (individual character) by using this [code](https://github.com/Insight-deviler/Folder-based-Character-Column-Transformation)
 
         | GENOTYPE | REPLICATION | Days to Maturity | PLANT HEIGHT (cm) |
         |----------|-------------|------------------|-------------------|
         | G1       | R1          | 4                | 5                 |
         | G1       | R2          | 5                | 6                 |
         | G1       | R3          | 4                | 9.3               |
         | G2       | R1          | 3                | 9.9               |
         | G2       | R2          | 6                | 7.5               |
 
 ## License
-This package is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
+This package is licensed under the MIT License. See the [LICENSE](https://github.com/Insight-deviler/anova-analysis/blob/main/LICENSE.txt) file for more information.
 
 ## Contributing
 Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request on the GitHub repository.
 
 ## Authors
 - Sarath S (insightagri10@gmail.com)
 - Saranyadevi S
```

### Comparing `anova_analysis-1.0.3/README.md` & `anova_analysis-1.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,34 +2,57 @@
 
 The ANOVA Analysis Package is a Python package that provides functions for performing ``Two-Way ANOVA (Analysis of Variance) analysis`` on experimental data.
 Currently it can perform RBD analysis only
 
 ## Installation
 
 You can install the package using pip:
-
 ```
 pip install anova_analysis
 ```
 ## Usage
 
+- If you just want the output as a file:
 ```
 from anova_analysis import ANOVA_RBD
 
-#Set the replication, treatment, input_file path and output_file_name
+ #Set the replication, treatment, input_file path and output_file_name
 
 replication = 4
 treatment = 23
 input_file_path = "data/MODEL_DATA.xlsx"
 output_file_name = "test"
 
-# Perform ANOVA analysis
+ #Perform ANOVA analysis
 
 ANOVA_RBD.RBD(replication, treatment, input_file_path, output_file_name )
 ```
+- If you want the output to be used in for further analysis, 
+you can then access the calculated values from the ``result`` dictionary:
+```
+result = ANOVA_RBD.RBD(replication, treatment, input_file_path, output_file_name)
+```
+- To access the ``result`` use the following
+```
+CF = result["correction_factor"]
+TSS = result["total_sum_of_square"]
+RSS = result["replication_sum_of_square"]
+TSS = result["treatment_sum_of_square"]
+ESS = result["error_sum_of_square"]
+Rdf = result["replication_df"]
+Tdf = result["treatment_df"],
+Edf = result["errors_df"],
+RMSS = result["rep_mean_ss"],
+TMSS = result["tre_mean_ss"],
+EMSS = result["error_mean_ss"]
+
+# Where CF, TSS,.. are variables
+```
+-  You can easily access them in your other Python file and use them as needed. Modify the returned data structure to suit your preferences and the specific values you want to access.
+
 ## Features
 
 - Calculates the correction factor, total sum of squares, replication sum of squares, treatment sum of squares, and error sum of squares.
 - Generates an ANOVA table with the source, degrees of freedom, sum of squares, mean square, F-values, and p-values at the 5% and 1% significance levels.
 - Performs significance testing at the 5% and 1% levels to determine the statistical significance of the factors.
 - Saves the ANOVA results in a text file for further analysis or reporting purposes.
 
@@ -41,26 +64,27 @@
                 | Genotypes | R1    | R2     | R3     | R4     |
                 |-----------|-------|--------|--------|--------|
                 | 1x6       | 74.4  | 70.86  | 60.94  | 68     |
                 | 1x7       | 91.82 | 99.18  | 118.88 | 120.68 |
                 | 1x8       | 48.08 | 62.1   | 58.54  | 41.84  |
                 | 2x6       | 59.06 | 65.62  | 81.62  | 86.76  |
                 | 2x7       | 84.16 | 109.74 | 102.14 | 94.52  |
+
 - If you have data in the below format, transform it to above said model (individual character) by using this [code](https://github.com/Insight-deviler/Folder-based-Character-Column-Transformation)
 
         | GENOTYPE | REPLICATION | Days to Maturity | PLANT HEIGHT (cm) |
         |----------|-------------|------------------|-------------------|
         | G1       | R1          | 4                | 5                 |
         | G1       | R2          | 5                | 6                 |
         | G1       | R3          | 4                | 9.3               |
         | G2       | R1          | 3                | 9.9               |
         | G2       | R2          | 6                | 7.5               |
 
 ## License
-This package is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
+This package is licensed under the MIT License. See the [LICENSE](https://github.com/Insight-deviler/anova-analysis/blob/main/LICENSE.txt) file for more information.
 
 ## Contributing
 Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request on the GitHub repository.
 
 ## Authors
 - Sarath S (insightagri10@gmail.com)
 - Saranyadevi S
```

### Comparing `anova_analysis-1.0.3/anova_analysis/ANOVA_RBD.py` & `anova_analysis-1.0.4/anova_analysis/ANOVA_RBD.py`

 * *Files 15% similar despite different names*

```diff
@@ -89,8 +89,24 @@
         file.write("Correction Factor: {:.2f}\n".format(correctionFactor))
         file.write("Total Sum of Square: {:.2f}\n".format(totalsum))
         file.write("Replication Sum of Square: {:.2f}\n".format(replicationSum))
         file.write("Treatment Sum of Square: {:.2f}\n".format(treatmentSum))
         file.write("Error Sum of Square: {:.2f}\n\n".format(Error_sum_square))
         file.write(tabulate(table_df, headers='keys', tablefmt='fancy_grid'))
 
-    print(f"Result saved in {output_file_name}_result.txt")
+    print(f"Result saved in {output_file_name}_result.txt")
+
+    result = {
+        "correction_factor": round(correctionFactor, 2),
+        "total_sum_of_square": round(totalsum, 2),
+        "replication_sum_of_square": round(replicationSum, 2),
+        "treatment_sum_of_square": round(treatmentSum, 2),
+        "error_sum_of_square": round(Error_sum_square, 2),
+        "replication_df": rep,
+        "treatment_df": tre,
+        "errors_df": error_df,
+        "rep_mean_ss":round(rep_mss, 2),
+        "tre_mean_ss": round(tre_mss, 2),
+        "error_mean_ss":round(error_mss, 2)
+    }
+    # Return the result
+    return result
```

### Comparing `anova_analysis-1.0.3/anova_analysis.egg-info/PKG-INFO` & `anova_analysis-1.0.4/anova_analysis.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: anova-analysis
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for performing ANOVA analysis by RBD
 Home-page: https://github.com/Insight-deviler/anova_analysis
 Author-email: insightagri10@gmail.com
 License: MIT
-Keywords: python,ANOVA,Two-way ANOVA,RBD,analysis of variance
+Keywords: line x tester,lxt,Line x Tester,Line Tester,Genetics and Plant breeding,Quantitative Genetics,ANOVA,Two-way ANOVA,RBD,analysis of variance
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -17,34 +17,57 @@
 
 The ANOVA Analysis Package is a Python package that provides functions for performing ``Two-Way ANOVA (Analysis of Variance) analysis`` on experimental data.
 Currently it can perform RBD analysis only
 
 ## Installation
 
 You can install the package using pip:
-
 ```
 pip install anova_analysis
 ```
 ## Usage
 
+- If you just want the output as a file:
 ```
 from anova_analysis import ANOVA_RBD
 
-#Set the replication, treatment, input_file path and output_file_name
+ #Set the replication, treatment, input_file path and output_file_name
 
 replication = 4
 treatment = 23
 input_file_path = "data/MODEL_DATA.xlsx"
 output_file_name = "test"
 
-# Perform ANOVA analysis
+ #Perform ANOVA analysis
 
 ANOVA_RBD.RBD(replication, treatment, input_file_path, output_file_name )
 ```
+- If you want the output to be used in for further analysis, 
+you can then access the calculated values from the ``result`` dictionary:
+```
+result = ANOVA_RBD.RBD(replication, treatment, input_file_path, output_file_name)
+```
+- To access the ``result`` use the following
+```
+CF = result["correction_factor"]
+TSS = result["total_sum_of_square"]
+RSS = result["replication_sum_of_square"]
+TSS = result["treatment_sum_of_square"]
+ESS = result["error_sum_of_square"]
+Rdf = result["replication_df"]
+Tdf = result["treatment_df"],
+Edf = result["errors_df"],
+RMSS = result["rep_mean_ss"],
+TMSS = result["tre_mean_ss"],
+EMSS = result["error_mean_ss"]
+
+# Where CF, TSS,.. are variables
+```
+-  You can easily access them in your other Python file and use them as needed. Modify the returned data structure to suit your preferences and the specific values you want to access.
+
 ## Features
 
 - Calculates the correction factor, total sum of squares, replication sum of squares, treatment sum of squares, and error sum of squares.
 - Generates an ANOVA table with the source, degrees of freedom, sum of squares, mean square, F-values, and p-values at the 5% and 1% significance levels.
 - Performs significance testing at the 5% and 1% levels to determine the statistical significance of the factors.
 - Saves the ANOVA results in a text file for further analysis or reporting purposes.
 
@@ -56,26 +79,27 @@
                 | Genotypes | R1    | R2     | R3     | R4     |
                 |-----------|-------|--------|--------|--------|
                 | 1x6       | 74.4  | 70.86  | 60.94  | 68     |
                 | 1x7       | 91.82 | 99.18  | 118.88 | 120.68 |
                 | 1x8       | 48.08 | 62.1   | 58.54  | 41.84  |
                 | 2x6       | 59.06 | 65.62  | 81.62  | 86.76  |
                 | 2x7       | 84.16 | 109.74 | 102.14 | 94.52  |
+
 - If you have data in the below format, transform it to above said model (individual character) by using this [code](https://github.com/Insight-deviler/Folder-based-Character-Column-Transformation)
 
         | GENOTYPE | REPLICATION | Days to Maturity | PLANT HEIGHT (cm) |
         |----------|-------------|------------------|-------------------|
         | G1       | R1          | 4                | 5                 |
         | G1       | R2          | 5                | 6                 |
         | G1       | R3          | 4                | 9.3               |
         | G2       | R1          | 3                | 9.9               |
         | G2       | R2          | 6                | 7.5               |
 
 ## License
-This package is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
+This package is licensed under the MIT License. See the [LICENSE](https://github.com/Insight-deviler/anova-analysis/blob/main/LICENSE.txt) file for more information.
 
 ## Contributing
 Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request on the GitHub repository.
 
 ## Authors
 - Sarath S (insightagri10@gmail.com)
 - Saranyadevi S
```

