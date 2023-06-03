# Comparing `tmp/travis_emulator-2.0.4.tar.gz` & `tmp/travis_emulator-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "travis_emulator-2.0.4.tar", last modified: Sun Apr 23 14:03:50 2023, max compression
+gzip compressed data, was "dist/travis_emulator-2.0.5.tar", last modified: Sat Jun  3 06:22:52 2023, max compression
```

## Comparing `travis_emulator-2.0.4.tar` & `travis_emulator-2.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2607 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    20883 2023-04-23 14:03:49.000000 travis_emulator-2.0.4/README.rst
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3324 2023-04-15 07:38:01.000000 travis_emulator-2.0.4/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/travis_emulator/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       77 2022-12-09 05:08:44.000000 travis_emulator-2.0.4/travis_emulator/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 travis_emulator-2.0.4/travis_emulator/__main__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5097 2023-04-14 13:30:50.000000 travis_emulator-2.0.4/travis_emulator/make_travis_conf.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/travis_emulator/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 travis_emulator-2.0.4/travis_emulator/scripts/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7460 2023-04-15 07:33:00.000000 travis_emulator-2.0.4/travis_emulator/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3324 2023-04-23 13:43:49.000000 travis_emulator-2.0.4/travis_emulator/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3683 2023-04-13 17:52:56.000000 travis_emulator-2.0.4/travis_emulator/template_travis.yml
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    47417 2023-04-15 08:02:21.000000 travis_emulator-2.0.4/travis_emulator/travis
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9772 2022-12-09 05:08:44.000000 travis_emulator-2.0.4/travis_emulator/travis.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    39019 2023-04-15 08:02:21.000000 travis_emulator-2.0.4/travis_emulator/travisrc
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-23 14:03:50.035239 travis_emulator-2.0.4/travis_emulator.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2607 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      599 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      145 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:51:08.000000 travis_emulator-2.0.4/travis_emulator.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       16 2023-04-23 14:03:50.000000 travis_emulator-2.0.4/travis_emulator.egg-info/top_level.txt
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 travis_emulator-2.0.5/travis_emulator/__main__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5097 2023-04-14 13:30:50.000000 travis_emulator-2.0.5/travis_emulator/make_travis_conf.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3683 2023-05-20 06:25:25.000000 travis_emulator-2.0.5/travis_emulator/template_travis.yml
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3324 2023-06-02 13:07:37.000000 travis_emulator-2.0.5/travis_emulator/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7868 2023-05-20 06:25:25.000000 travis_emulator-2.0.5/travis_emulator/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 travis_emulator-2.0.5/travis_emulator/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9772 2022-12-09 05:08:44.000000 travis_emulator-2.0.5/travis_emulator/travis.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    38654 2023-05-29 13:26:46.000000 travis_emulator-2.0.5/travis_emulator/travisrc
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    46782 2023-05-21 06:35:50.000000 travis_emulator-2.0.5/travis_emulator/travis
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       77 2022-12-09 05:08:44.000000 travis_emulator-2.0.5/travis_emulator/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3324 2023-05-20 06:25:25.000000 travis_emulator-2.0.5/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       16 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:51:08.000000 travis_emulator-2.0.5/travis_emulator.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      145 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      599 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2898 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2898 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    17054 2023-05-21 12:21:55.000000 travis_emulator-2.0.5/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `travis_emulator-2.0.4/setup.py` & `travis_emulator-2.0.5/travis_emulator/scripts/setup.info`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='travis_emulator',
-    version='2.0.4',
+    version='2.0.5',
     description='Travis CI emulator for local develop environment',
     long_description="""
 Travis emulator can emulate TravisCi parsing the **.travis.yml** file in local Linux machine.
 You can test your application before pushing code to github.com web site.
 
 Travis emulator can creates all the build declared in **.travis.yml**;
 all the builds are executed in sequential way.
```

### Comparing `travis_emulator-2.0.4/travis_emulator/make_travis_conf.py` & `travis_emulator-2.0.5/travis_emulator/make_travis_conf.py`

 * *Files identical despite different names*

### Comparing `travis_emulator-2.0.4/travis_emulator/scripts/main.py` & `travis_emulator-2.0.5/travis_emulator/scripts/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# template 20
+# template 21
 """
 Travis emulator can emulate TravisCi parsing the **.travis.yml** file in
 local Linux machine and it is osx/darwin compatible.
 You can test your application before pushing code to github.com web site.
 
 Travis emulator can creates all the build declared in **.travis.yml**;
 all the builds are executed in sequential way.
@@ -41,15 +41,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -125,20 +125,28 @@
                             else:
                                 fd.write(help_text)
                         if verbose:
                             print("$ gzip -c %s > %s" % (full_fn, tgt_fn))
                         continue
                     if lib_path:
                         tgt_fn = os.path.join(lib_path, base)
-                        try:
-                            shutil.copy(full_fn, tgt_fn)
-                            if verbose:
-                                print("$ cp %s %s" % (full_fn, tgt_fn))
-                        except shutil.SameFileError:
-                            pass
+                        if sys.version_info[0] == 3:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except shutil.SameFileError:
+                                pass
+                        else:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except BaseException:
+                                pass
                     # TODO> compatibility mode
                     tgt_fn = os.path.join(bin_path, base)
                     if os.path.isfile(tgt_fn):
                         os.unlink(tgt_fn)
                     if not os.path.exists(tgt_fn):
                         if verbose:
                             print("$ ln -s %s %s" % (full_fn, tgt_fn))
```

### Comparing `travis_emulator-2.0.4/travis_emulator/scripts/setup.info` & `travis_emulator-2.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='travis_emulator',
-    version='2.0.4',
+    version='2.0.5',
     description='Travis CI emulator for local develop environment',
     long_description="""
 Travis emulator can emulate TravisCi parsing the **.travis.yml** file in local Linux machine.
 You can test your application before pushing code to github.com web site.
 
 Travis emulator can creates all the build declared in **.travis.yml**;
 all the builds are executed in sequential way.
```

### Comparing `travis_emulator-2.0.4/travis_emulator/template_travis.yml` & `travis_emulator-2.0.5/travis_emulator/template_travis.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Odoo yaml template for travis-ci
-# __version__=2.0.4
+# __version__=2.0.5
 # Can used both in local travis emulator both in travis environment
 # Notice: in local travis emulator macroes are substituted in 2 steps:
 # - format: ${macro} are replaced before execution (at travis.yml read)
 # - format: $macro are replace by shell during execution
 
 language: python
 sudo: false
```

### Comparing `travis_emulator-2.0.4/travis_emulator/travis` & `travis_emulator-2.0.5/travis_emulator/travis`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.4
+__version__=2.0.5
 
 
 store_cfg_param_value() {
   #store_cfg_param_value(tid key value [opt] [section])
   local p
   if [[ $2 =~ ^pip_pkgver__ ]]; then
     if [ -z "$PIPPKGVER" ]; then
@@ -92,41 +92,38 @@
     YML_repo=odoo/odoo
   else
     YML_repo=
   fi
   export TRAVIS_PULL_REQUEST="false"
   export MQT_TEMPLATE_DB="$(get_cfg_value "" "MQT_TEMPLATE_DB")$YML_pid"
   export MQT_TEST_DB="$(get_cfg_value "" "MQT_TEST_DB")$YML_pid"
-  # export PGUSER="$(get_cfg_value "" "MQT_DBUSER")"
   [[ -z $PGUSER ]] && export PGUSER=$(get_dbuser)
   python_ver_yaml=""
-  # python_ver_ena=""
-  # [[ -f $PRJPATH/travis.ini ]] && python_ver_ena=$(cat $PRJPATH/travis.ini|grep "^PYPI_RUN_PYVER"|awk -F= '{print $2}'|grep --color=never -Eo "[0-9.]+"|head -n1)
   if [ $opt_dbgmnt -ne 0 ]; then
     [[ -d $HOME_DEVEL/pypi ]] && export YML_lisa=$HOME_DEVEL/pypi/lisa/lisa/lisa
     (($opt_debug)) && export TRAVIS_PDB="true"
   else
     export YML_lisa=lisa
     export YML_mgrodoo=manage_odoo
   fi
-  # export TRAVIS_DEBUG_MODE="${opt_dlvl:-1}"
   [[ $TRAVIS_DEBUG_MODE -gt 1 ]] && export VERBOSE_MODE=$TRAVIS_DEBUG_MODE
-  [[ $osx_d -ne 0 ]] && export TRAVIS_EMULATE_OSX="true"
+  # [[ $osx_d -ne 0 ]] && export TRAVIS_EMULATE_OSX="true"
   ODOO_TNLBOT="${opt_tnl:-0}"
   if [ $opt_full -ne 0 ]; then
     export SYSTEM_SITE_PACKAGES="${opt_syspkg:-false}"
   else
     export SYSTEM_SITE_PACKAGES="${opt_syspkg:-true}"
   fi
   LINT_CHECK_LEVEL="${opt_llvl^^}"
   for i in {1..9}; do
     declare YML_CMD_DIS_$i=$(get_cfg_value "" "yaml__cmd_dis__$i")
   done
   FH=$(xuname -f)
   TRAVIS_VERBOSE=$opt_verbose
+  [[ -n $opt_patrn ]] && export TRAVIS_TEST_PATTERN="$opt_patrn"
 }
 
 process_yaml_unquote() {
   lne="$(echo $1 | sed -e s/\"/%%22/g -e s/\'/%%26/g -e s/\ /%%20/g)"
   echo $lne
 }
 
@@ -754,21 +751,14 @@
     [[ $c != $xcmd && ! $xcmd =~ ^# ]] && echo "\e[${PS_NOP_COLOR}m## $c\e[${PS_TXT_COLOR}m"
     echo "$xcmd"
     s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
   else
     [[ $c != $xcmd && ! $xcmd =~ ^# ]] && wlog "\e[${PS_NOP_COLOR}m> $c\e[${PS_TXT_COLOR}m" && ((Z0_STACK=Z0_STACK+2))
     run_traced "$line1$xcmd"
     s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
-#    if [[ $xcmd =~ "travis_install_env" ]]; then
-#      ((Z0_STACK=Z0_STACK+2))
-#      opts=$(inherits_travis_opts "" "V")
-#      [[ $TRAVIS == "true" ]] || opts="$opts -f"
-#      [ $opt_keepE -eq 0 ] || run_traced "vem create $VENVOPTS $TRAVIS_HOME $opts -p$TRAVIS_PYTHON_VERSION"
-#      ((Z0_STACK=Z0_STACK-2))
-#    fi
     [[ $c != $xcmd && ! $xcmd =~ ^# ]] && ((Z0_STACK=Z0_STACK-2))
   fi
   [[ $TRAVIS_DEBUG_MODE -gt 2 ]] && echo "<<<PATH=$PATH>>>"
   [[ -n $opt_tafter && $xcmd =~ $opt_tafter ]] && debug_shell
   return $sts
 }
 
@@ -809,26 +799,26 @@
   export TRAVIS_HOME_BRANCH=$PWD
   process_yaml_file "$TRAVIS_YAML_FILE"
   unset PYTHONPATH
   sts=$STS_SUCCESS
 
   if [[ $sts -eq $STS_SUCCESS ]]; then
     [[ -n $opt_trace && ::matrix =~ $opt_trace ]] && debug_shell "::matrix"
-    [[ -z "$python_ver_yaml" ]] && python_ver_yaml="2.7 3.5 3.6 3.7 3.8 3.9 3.10 3.11"
+    [[ -z "$python_ver_yaml" ]] && python_ver_yaml="3.11 3.10 3.9 3.8 3.7 3.5 3.6 2.7"
     if [[ -n $opt_pyv ]]; then
       TRAVIS_PYTHON_MATRIX="${opt_pyv//,/ }"
       python_ver_yaml="$TRAVIS_PYTHON_MATRIX"
     elif [[ $PRJNAME == "Odoo" ]]; then
       v=$(build_odoo_param "MAJVER" $BRANCH)
       TRAVIS_PYTHON_MATRIX="3.7"
       [[ $v -le 10 ]] && TRAVIS_PYTHON_MATRIX="2.7"
       [[ $v -ge 15 ]] && TRAVIS_PYTHON_MATRIX="3.8"
     else
       TRAVIS_PYTHON_MATRIX=""
-      for v in "2.7" "3.5" "3.6" "3.7" "3.8" "3.9" "3.10" "3.11"; do
+      for v in "3.11" "3.10" "3.9" "3.8" "3.7" "3.6" "3.5" "2.7"; do
           grep -q "^ *.Programming Language :: Python :: $v" $PKGPATH/setup.py && TRAVIS_PYTHON_MATRIX="$TRAVIS_PYTHON_MATRIX|$v"
       done
       TRAVIS_PYTHON_MATRIX="${TRAVIS_PYTHON_MATRIX:1}"
     fi
     TRAVIS_PYTHON_MATRIX="${TRAVIS_PYTHON_MATRIX//,/|}"
     TRAVIS_PYTHON_MATRIX="${TRAVIS_PYTHON_MATRIX// /|}"
     [[ $TRAVIS_PYTHON_MATRIX =~ ^\( ]] || TRAVIS_PYTHON_MATRIX="($TRAVIS_PYTHON_MATRIX)"
@@ -891,16 +881,16 @@
         TODAY=$(date "+%Y-%m-%d %H:%M:%S")
         for p in TODAY job-id __version__ TCONF YML_lisa YML_mgrodoo YML_repo\
          BRANCH DIST HOME HOME_BRANCH HOME_DEVEL LOGFILE MQT_TEMPLATE_DB MQT_TEST_DB\
           ODOO_ROOT PATH PKGNAME PKGPATH PIP PIPVER PRJNAME PRJPATH PGUSER PYPI_CACHED\
            PYTHON PYTHONPATH REPOSNAME TRAVIS TRAVIS_BRANCH TRAVIS_BUILD_DIR\
              TRAVIS_HOME TRAVIS_HOME_BRANCH TRAVIS_PDB TRAVIS_PYTHON_MATRIX\
               TRAVIS_PYTHON_VERSION TRAVIS_REPO_SLUG TRAVIS_SAVED_HOME\
-               TRAVIS_SAVED_HOME_DEVEL TRAVIS_YAML_FILE TRAVIS_YAML_ORIG\
-                SYSTEM_SITE_PACKAGES; do
+               TRAVIS_SAVED_HOME_DEVEL TRAVIS_TEST_PATTERN TRAVIS_YAML_FILE\
+                TRAVIS_YAML_ORIG SYSTEM_SITE_PACKAGES; do
           if [[ $p == "job-id" ]]; then
             X=$$
           elif [[ $p == "DIST" ]]; then
             X=$(xuname -a)
           elif [[ $p == "__version__" ]]; then
             X=$__version__
           else
@@ -988,16 +978,14 @@
     fi
     return $sts
 }
 
 set_log_filename() {
     # UDI (Unique DB Identifier): format "{pkgname}_{git_org}{major_version}"
     # UMLI (Unique Module Log Identifier): format "{git_org}{major_version}.{repos}.{pkgname}"
-    # set -x  #debug
-    # local odoo_ver=$(build_odoo_param MAJVER ${BRANCH})
     local m="$PKGNAME" odoo_ver=$(build_odoo_param MAJVER ${BRANCH})
     [[ -z $GIT_ORGID ]] && GIT_ORGID="$(build_odoo_param GIT_ORGID '.')"
     [[ -n $ODOO_GIT_ORGID && $GIT_ORGID =~ $ODOO_GIT_ORGID ]] && UDI="$m" || UDI="$m_${GIT_ORGID}"
     [[ $PRJNAME == "Odoo" && -n $UDI ]] && UDI="${UDI}_${odoo_ver}"
     [[ $PRJNAME == "Odoo" && -z $UDI ]] && UDI="${odoo_ver}"
     [[ $PRJNAME == "Odoo" ]] && UMLI="${GIT_ORGID}${odoo_ver}" || UMLI="${GIT_ORGID}"
     [[ -n "$REPOSNAME" && $REPOSNAME != "OCB" ]] && UMLI="${UMLI}.${REPOSNAME//,/+}"
@@ -1012,39 +1000,38 @@
       LOGFILE="$LOGDIR/${UMLI}.log"
     fi
     OLD_LOGFILE=${LOGFILE/.log/_old.log}
     # set +x  #debug
 }
 
 
-OPTOPTS=(h        A           B         C         D           E         e       F        f         k        j       L          l        M          m       n            O         P           p        Q        q           r     S            T         V           v           X           Y         Z)
-OPTLONG=(help     trace-after debug     no-cache  debug-level no-savenv locale  full     force     keep     pyver   lint-level logdir   ''         missing dry-run      org       python-brk  pytest   config   quiet       ''    syspkg       trace     version     verbose     translation yaml-file zero)
-OPTDEST=(opt_help opt_tafter  opt_debug opt_cache opt_dlvl    opt_keepE opt_loc opt_full opt_force opt_keep opt_pyv opt_llvl   opt_flog opt_dbgmnt opt_mis opt_dry_run  opt_org   opt_pybrk   opt_pyth opt_tcfg opt_verbose opt_r  opt_syspkg  opt_trace opt_version opt_verbose opt_tnl     opt_fyaml opt_dbgmnt)
-OPTACTI=('+'      "="         1         0         "="         0         "="     1        1         1        "="     "="        "="      1          1       "1>"         "="       "="         1        "="      0           1     "="          "="       "*>"        "+"         "="         "="       1)
-OPTDEFL=(0        ""          0         1         ""          1         ""      0        0         0        ""      ""         ""       0          0       0            "local"   ""          0        ""       0           0     ""           ""        ""          -1          ""          ""        0)
-OPTMETA=("help"   "regex"     "version" ""        "number"    ""        "iso"   ""       ""        ""       "pyver" "number"   "dir"    ""         ""      "do nothing" "git-org" "file:line" ""       "file"   "verbose"   "res" "false|true" "regex"   "version"   "verbose"   "0|1"       "file"    "")
+OPTOPTS=(h        A           B         C         D           E         e       F        f         k        j       L          l        m       n            O         P           p         Q        q           r     S            T         V           v           X           Y         Z)
+OPTLONG=(help     trace-after debug     no-cache  debug-level no-savenv locale  full     force     keep     python  lint-level logdir   missing dry-run      org       python-brk  pattern   config   quiet       ''    syspkg       trace     version     verbose     translation yaml-file zero)
+OPTDEST=(opt_help opt_tafter  opt_debug opt_cache opt_dlvl    opt_keepE opt_loc opt_full opt_force opt_keep opt_pyv opt_llvl   opt_flog opt_mis opt_dry_run  opt_org   opt_pybrk   opt_patrn opt_tcfg opt_verbose opt_r  opt_syspkg  opt_trace opt_version opt_verbose opt_tnl     opt_fyaml opt_dbgmnt)
+OPTACTI=('+'      "="         1         0         "="         0         "="     1        1         1        "="     "="        "="      1       "1>"         "="       "="         "="       "="      0           1     "="          "="       "*>"        "+"         "="         "="       1)
+OPTDEFL=(0        ""          0         1         ""          1         ""      0        0         0        ""      ""         ""       0       0            "local"   ""          ""        ""       0           0     ""           ""        ""          -1          ""          ""        0)
+OPTMETA=("help"   "regex"     "version" ""        "number"    ""        "iso"   ""       ""        ""       "pyver" "number"   "dir"    ""      "do nothing" "git-org" "file:line" "pattern" "file"   "verbose"   "res" "false|true" "regex"   "version"   "verbose"   "0|1"       "file"    "")
 OPTHELP=("this help"
   "travis stops after executed yaml statement"
   "debug mode: do not create log"
   "do not use stored PYPI"
   "travis_debug_mode: may be 0,1,2,3,8 or 9 (def yaml dependents)"
   "do not save virtual environment into ~/VME/... if does not exist"
   "use locale"
   "run final travis with full features"
   "force to create stored VME or remove recent log (wep-db)"
   "keep DB and virtual environment before and after tests"
   "test with specific python versions (comma separated)"
   "lint_check_level: may be minimal,reduced,average,nearby,oca; def value from .travis.yml"
   "log directory (def=$ODOO_ROOT/travis_log)"
-  "deprecated: kept just for compatibility"
   "show missing line in report coverage"
   "do nothing (dry-run)"
-  "prefer python test over bash test when avaiable"
-  "git organization, i.e. oca or zeroincombenze"
+  "git organization to test, i.e. oca or zeroincombenze"
   "set python breakpoint at file:linenumber"
+  "pattern to apply for test files (comma separated)"
   "configuration file (def .z0tools.conf)"
   "silent mode"
   "run restricted mode (deprecated)"
   "use python system packages (def yaml dependents)"
   "trace stops before executing yaml statement"
   "show version"
   "verbose mode"
@@ -1062,16 +1049,17 @@
 if [[ $opt_help -gt 0 ]]; then
   print_help "Travis-ci emulator for local developer environment\nAction may be: ${ACTIONS//|/,}" \
   "© 2015-2022 by zeroincombenze®\nhttps://zeroincombenze-tools.readthedocs.io/\nAuthor: antoniomaria.vigliotti@gmail.com"
   exit $STS_SUCCESS
 fi
 
 export PYTHONWARNINGS="ignore"
-[[ -z "$action" ]] && action=emulate
 [[ -n "$opt_tafter" || -n "$opt_trace" || -n "$opt_pybrk" ]] && opt_debug=1
+[[ -z "$action" && $opt_debug -ne 0 ]] && action="test"
+[[ -z "$action" ]] && action="emulate"
 VIRTACTS="(force-lint|lint|force-test|test|force-test-multi|test-multi|emulate)"
 opt_virt=1
 if [[ $action =~ $ACTIONS ]]; then
   [[ ! $action =~ $VIRTACTS ]] && opt_virt=0
 else
   echo "Invalid action!"
   echo "action should be one of ${ACTIONS//|/,}"
```

### Comparing `travis_emulator-2.0.4/travis_emulator/travis.man` & `travis_emulator-2.0.5/travis_emulator/travis.man`

 * *Files identical despite different names*

### Comparing `travis_emulator-2.0.4/travis_emulator/travisrc` & `travis_emulator-2.0.5/travis_emulator/travisrc`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env bash
 #
 # Common file for travis emulator scripts
 #
-#__version__=2.0.4
+#__version__=2.0.5
 
 [[ "${BASH_SOURCE-}" == "$0" ]] && echo "You must source this script: \$ source $0" >&2 && exit 33
 XRGI="^(.*\/|)conf\/.*sample$"
 READLINK=$(which greadlink 2>/dev/null) || READLINK=$(which readlink 2>/dev/null)
 export READLINK
 # Based on template 2.0.0
 THIS=$(basename "$0")
@@ -80,16 +80,16 @@
           opts="${opts}$o"
         elif [ "$o" == "n" -a ${opt_dry_run:-0} -gt 0 ]; then
           opts="${opts}$o"
         elif [ "$o" == "o" ]; then
           [ -n "$opt_ids" ] && opts2="-o$opt_ids"
         elif [ "$o" == "P" -a "$opt_cpush" == "-$o" ]; then
           opts="${opts}$o"
-        elif [ "$o" == "p" -a "${opt_pyth:-0}" -gt 0 ]; then
-          opts="${opts}$o"
+        # elif [ "$o" == "p" -a "${opt_pyth:-0}" -gt 0 ]; then
+        #   opts="${opts}$o"
         elif [ "$o" == "q" -a ${opt_verbose:-1} -eq 0 ]; then
           opts="${opts}$o"
         elif [ "$o" == "R" -a "$opt_cpush" == "-$o" ]; then
           opts="${opts}$o"
         elif [ "$o" == "r" -a ${opt_r:-0} -eq 1 ]; then
           opts="${opts}$o"
         elif [ "$o" == "u" -a ${opt_uop:-0} -eq 1 ]; then
@@ -278,27 +278,14 @@
 
 uname() {
     local x UNAME
     UNAME=$(which uname)
     [[ -x $TRAVIS_HOME/bin/greadlink ]] && echo "Darwin" || $UNAME "$@"
 }
 
-set_osx() {
-    local x
-    x=$(which readlink)
-    run_traced "ln -s $x $TRAVIS_HOME/bin/greadlink"
-    echo "echo '*** INVALID READLINK: use GREADLINK! ***'" >$TRAVIS_HOME/bin/readlink
-    echo "echo -e \"\\e[31mDir stack\\e[0m\"" >>$TRAVIS_HOME/bin/readlink
-    echo "echo $DIRSTACK" >>$TRAVIS_HOME/bin/readlink
-    echo "echo -e \"\\e[31mCaller\\e[0m\"" >>$TRAVIS_HOME/bin/readlink
-    echo "caller" >>$TRAVIS_HOME/bin/readlink
-    echo "exit 126" >>$TRAVIS_HOME/bin/readlink
-    chmod +x $TRAVIS_HOME/bin/readlink
-}
-
 create_virtual_env() {
   local f opts p sts=0 t x xp1 xp2
   [[ -z ${Z0_STACK:+_} ]] && export Z0_STACK=0
   ((Z0_STACK=Z0_STACK+2))
   unset TOOLS_PATH
   init_travis
   export TRAVIS_BRANCH=$(git branch --list|grep "^\* "|cut -d" " -f2|head -n1|tr -d "\n")
@@ -394,15 +381,15 @@
   [[ $sts -ne 0 ]] && return
 
   run_traced "source $TRAVIS_HOME/bin/activate"
   [[ ${opt_keep:-0} -ne 0 ]] && run_traced "export ODOO_COMMIT_TEST=\"1\""
   set_pybin $TRAVIS_PYTHON_VERSION
   if [[ $opt_dbgmnt -ne 0 ]]; then
     # Install unstable packages to run them when needed
-    for p in $(get_cfg_value "" "PKGS_LIST"); do
+    for p in $(get_cfg_value "" "LOCAL_PKGS"); do
         # Use unstable version
         [[ $p =~ (python-plus|z0bug-odoo) ]] && p="${p//-/_}"
         [[ -f $TRAVIS_SAVED_HOME_DEVEL/pypi/$p/$p/scripts/setup.info ]] && \
           run_traced "$PIP install -qU $TRAVIS_SAVED_HOME_DEVEL/pypi/$p"
     done
   fi
   [[ -n $NVM_DIR && -f $NVM_DIR/nvm.sh ]] && source $NVM_DIR/nvm.sh
@@ -502,20 +489,21 @@
     else
       d="./"
     fi
     [[ -z $SAVED_ODOO_ROOT ]] && SAVE_ODOO_ROOT=$(readlink -f $TRAVIS_SAVED_HOME_DEVEL/..)
     run_traced "cp -R $SAVED_ODOO_ROOT/tools $d"
     if [[ $opt_dbgmnt -ne 0 ]]; then
       x=${TRAVIS_REPO_SLUG#*/}
-      for p in $(get_cfg_value "" "PKGS_LIST"); do
+      for p in $(get_cfg_value "" "LOCAL_PKGS"); do
         # Load unstable version
         [[ $p =~ (python-plus|z0bug-odoo) ]] && p="${p//-/_}"
         [[ -f $TRAVIS_SAVED_HOME_DEVEL/pypi/$p/$p/scripts/setup.info ]] && \
           run_traced "rsync -rlpgoW --delete $TRAVIS_SAVED_HOME_DEVEL/pypi/$p/$p/ $HOME/tools/$p/" && \
           run_traced "cp $TRAVIS_SAVED_HOME_DEVEL/pypi/$p/setup.py $HOME/tools/$p/"
+          [[ -f $TRAVIS_SAVED_HOME_DEVEL/pypi/$p/README.rst ]] && run_traced "cp $TRAVIS_SAVED_HOME_DEVEL/pypi/$p/README.rst $HOME/tools/$p/"
         s=$?; [ ${s-1} -eq 0 ] || echo "Internal error $s! Statement rsync $p failed!!"
       done
       for p in install_tools.sh odoo_default_tnl.xlsx; do
         [[ -d $TRAVIS_SAVED_HOME_DEVEL/pypi/tools/ ]] && \
           run_traced "cp $TRAVIS_SAVED_HOME_DEVEL/pypi/tools/$p $HOME/tools/$p"
       done
       true # FIX: return no error
@@ -601,18 +589,18 @@
   export PRJPATH
   export PKGPATH
   export PKGNAME
   export LGITPATH
 }
 
 check_4_travis() {
-  if [ ! -d "$PRJPATH" ]; then
+  if [[ ! -d "$PRJPATH" ]]; then
     echo "Invalid project path $PRJPATH"
     exit $STS_FAILED
-  elif [ ! -d "$PKGPATH" ]; then
+  elif [[ ! -d "$PKGPATH" ]]; then
     echo "Invalid package path $PKGPATH"
     exit $STS_FAILED
   fi
 }
 
 conf_default() {
   [[ -z $(get_cfg_value "" "loglevel") ]] && CFG_set "loglevel" "-1"
@@ -623,15 +611,15 @@
   [[ -z $(get_cfg_value "" "MQT_TEST_DB") ]] && CFG_set "MQT_TEST_DB" "test_odoo"
   [[ -z $(get_cfg_value "" "MQT_DBUSER") ]] && CFG_set "MQT_DBUSER" ""
   [[ -z $(get_cfg_value "" "UNBUFFER") ]] && CFG_set "UNBUFFER" "0"
   [[ -z $(get_cfg_value "" "ME_BOS") ]] && CFG_set "ME_BOS" "test_nightly .test_nightly.conf.sample"
   [[ -z $(get_cfg_value "" "Environment") ]] && CFG_set "Environment" "bash"
   [[ -z $(get_cfg_value "" "virtualenv_opts") ]] && CFG_set "virtualenv_opts" ""
   [[ -z $(get_cfg_value "" "NPM_CONFIG_PREFIX") ]] && CFG_set "NPM_CONFIG_PREFIX" "$HOME/.npm-global"
-  [[ -z $(get_cfg_value "" "PYTHON_MATRIX") ]] && CFG_set "PYTHON_MATRIX" "(2.7|3.6|3.7|3.8|3.9)"
+  [[ -z $(get_cfg_value "" "PYTHON_MATRIX") ]] && CFG_set "PYTHON_MATRIX" "(3.9|3.8|3.7|3.6|2.7)"
   [[ -z $(get_cfg_value "" "LOGDIR") ]] && CFG_set "LOGDIR" "$HOME/travis_log"
   # Test disabled by default: they are added to EXCLUDE paramater
   [[ -z $(get_cfg_value "" "GBL_EXCLUDE") ]] && CFG_set "GBL_EXCLUDE" "test_impex,test_ir_actions,test_lint,test_main_flows,test_search,test_user_has_group,test_mimetypes"
 }
 
 #
 # [antoniov: 2022-08-06] TODO: remove early
@@ -693,15 +681,15 @@
     a_append "--new"
     a_append "^.*\.egg-info$" ""
     if [ "$1" == "Odoo" ]; then
       a_append "^.*" "/"
     else
       a_append "setup.py" ""
       if [ "$2" == "OCB" ]; then
-        local p=$(echo $PWD | grep --color=never -Eo "(v7|6.1|7.0|8.0|9.0|10.0|11.0|12.0|13.0|14.0|15.0)" | head -n1)
+        local p=$(echo $PWD | grep --color=never -Eo "(v7|6.1|7.0|8.0|9.0|10.0|11.0|12.0|13.0|14.0|15.0|16.0)" | head -n1)
         if [ -n "$p" ]; then
           a_append "$p" "/"
         fi
       else
         a_append "$2" "/"
       fi
       a_append "conf" "/"
```

### Comparing `travis_emulator-2.0.4/travis_emulator.egg-info/SOURCES.txt` & `travis_emulator-2.0.5/travis_emulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

