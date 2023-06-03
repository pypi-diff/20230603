# Comparing `tmp/dcs-code-injector-1.0.2.tar.gz` & `tmp/dcs-code-injector-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcs-code-injector-1.0.2.tar", last modified: Wed May 24 11:02:27 2023, max compression
+gzip compressed data, was "dcs-code-injector-1.0.4.tar", last modified: Sat Jun  3 06:49:09 2023, max compression
```

## Comparing `dcs-code-injector-1.0.2.tar` & `dcs-code-injector-1.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.866660 dcs-code-injector-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 11:02:27.866660 dcs-code-injector-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.850660 dcs-code-injector-1.0.2/dcs_code_injector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/dcs_code_injector_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/log_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/lua_syntax_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/settings_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.854660 dcs-code-injector-1.0.2/dcs_code_injector/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/dcs_code_injector_settings_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/dcs_code_injector_window_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.858660 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/cloud_done.png
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/cloud_off.png
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.862660 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   629069 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_01.png
--rw-r--r--   0 runner    (1001) docker     (123)   831944 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_02.png
--rw-r--r--   0 runner    (1001) docker     (123)   927761 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_03.png
--rw-r--r--   0 runner    (1001) docker     (123)   932507 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_04.png
--rw-r--r--   0 runner    (1001) docker     (123)   723796 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_05.png
--rw-r--r--   0 runner    (1001) docker     (123)   916284 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_06.png
--rw-r--r--   0 runner    (1001) docker     (123)   968922 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_07.png
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/dcs_code_injector/variables_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:02:27.854660 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 11:02:27.000000 dcs-code-injector-1.0.2/dcs_code_injector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:02:27.866660 dcs-code-injector-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-24 11:02:16.000000 dcs-code-injector-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:49:09.130469 dcs-code-injector-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4171 2023-06-03 06:49:09.130469 dcs-code-injector-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3808 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 06:49:09.099216 dcs-code-injector-1.0.4/dcs_code_injector/
+-rw-rw-rw-   0        0        0        0 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/app.py
+-rw-rw-rw-   0        0        0    15823 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/dcs_code_injector_window.py
+-rw-rw-rw-   0        0        0     1281 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/log_highlighter.py
+-rw-rw-rw-   0        0        0    10001 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/lua_syntax_highlighter.py
+-rw-rw-rw-   0        0        0     1848 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/server.py
+-rw-rw-rw-   0        0        0     1269 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/settings_dialog.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:49:09.114843 dcs-code-injector-1.0.4/dcs_code_injector/ui/
+-rw-rw-rw-   0        0        0        0 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/__init__.py
+-rw-rw-rw-   0        0        0     2947 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/dcs_code_injector_settings_ui.py
+-rw-rw-rw-   0        0        0     5005 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/dcs_code_injector_window_ui.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:49:09.114843 dcs-code-injector-1.0.4/dcs_code_injector/ui/icons/
+-rw-rw-rw-   0        0        0        0 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/icons/__init__.py
+-rw-rw-rw-   0        0        0      855 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/icons/cloud_done.png
+-rw-rw-rw-   0        0        0     1126 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/icons/cloud_off.png
+-rw-rw-rw-   0        0        0     5569 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/icons/icon.png
+drwxrwxrwx   0        0        0        0 2023-06-03 06:49:09.130469 dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/
+-rw-rw-rw-   0        0        0        0 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/__init__.py
+-rw-rw-rw-   0        0        0   629069 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_01.png
+-rw-rw-rw-   0        0        0   831944 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_02.png
+-rw-rw-rw-   0        0        0   927761 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_03.png
+-rw-rw-rw-   0        0        0   932507 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_04.png
+-rw-rw-rw-   0        0        0   723796 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_05.png
+-rw-rw-rw-   0        0        0   916284 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_06.png
+-rw-rw-rw-   0        0        0   968922 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_07.png
+-rw-rw-rw-   0        0        0     3188 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/dcs_code_injector/variables_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:49:09.114843 dcs-code-injector-1.0.4/dcs_code_injector.egg-info/
+-rw-rw-rw-   0        0        0     4171 2023-06-03 06:49:09.000000 dcs-code-injector-1.0.4/dcs_code_injector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1244 2023-06-03 06:49:09.000000 dcs-code-injector-1.0.4/dcs_code_injector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 06:49:09.000000 dcs-code-injector-1.0.4/dcs_code_injector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-03 06:49:09.000000 dcs-code-injector-1.0.4/dcs_code_injector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-06-03 06:49:09.000000 dcs-code-injector-1.0.4/dcs_code_injector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-03 06:49:09.000000 dcs-code-injector-1.0.4/dcs_code_injector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 06:49:09.130469 dcs-code-injector-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-06-03 06:47:43.000000 dcs-code-injector-1.0.4/setup.py
```

### Comparing `dcs-code-injector-1.0.2/LICENSE` & `dcs-code-injector-1.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/app.py` & `dcs-code-injector-1.0.4/dcs_code_injector/app.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from PySide6.QtWidgets import *
-from PySide6.QtGui import *
-import os
-import random
-import time
-from ez_settings import EZSettings
-from qt_material import apply_stylesheet
-from .dcs_code_injector_window import CodeInjectorWindow
-
-SETTINGS_DIR = os.path.join(os.path.expanduser('~'),'Documents', "dcs_code_injector")
-if not os.path.exists(SETTINGS_DIR):
-    os.makedirs(SETTINGS_DIR)
-SETTINGS_PATH = os.path.join(SETTINGS_DIR, "settings.json")
-SPLASH_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "ui", "splashscreens")
-EZSettings(SETTINGS_PATH)
-
-application = QApplication()
-
-def main():
-    splashscreens = [os.path.join(SPLASH_DIR, file) for file in os.listdir(SPLASH_DIR) if file.endswith(".png")]
-    splash = QSplashScreen(QPixmap(splashscreens[random.randint(0, len(splashscreens) - 1)]))
-    splash.show()
-
-    application.processEvents()
-    apply_stylesheet(application, "dark_teal.xml")
-    win = CodeInjectorWindow()
-
-    splash.finish(win)
-    application.exec_()
-
-if __name__ == '__main__':
+from PySide6.QtWidgets import *
+from PySide6.QtGui import *
+import os
+import random
+import time
+from ez_settings import EZSettings
+from qt_material import apply_stylesheet
+from .dcs_code_injector_window import CodeInjectorWindow
+
+SETTINGS_DIR = os.path.join(os.path.expanduser('~'),'Documents', "dcs_code_injector")
+if not os.path.exists(SETTINGS_DIR):
+    os.makedirs(SETTINGS_DIR)
+SETTINGS_PATH = os.path.join(SETTINGS_DIR, "settings.json")
+SPLASH_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "ui", "splashscreens")
+EZSettings(SETTINGS_PATH)
+
+application = QApplication()
+
+def main():
+    splashscreens = [os.path.join(SPLASH_DIR, file) for file in os.listdir(SPLASH_DIR) if file.endswith(".png")]
+    splash = QSplashScreen(QPixmap(splashscreens[random.randint(0, len(splashscreens) - 1)]))
+    splash.show()
+
+    application.processEvents()
+    apply_stylesheet(application, "dark_teal.xml")
+    win = CodeInjectorWindow()
+
+    splash.finish(win)
+    application.exec_()
+
+if __name__ == '__main__':
     main()
```

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/dcs_code_injector_window.py` & `dcs-code-injector-1.0.4/dcs_code_injector/dcs_code_injector_window.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,411 +1,411 @@
-from PySide6.QtWidgets import *
-from PySide6.QtGui import *
-from PySide6.QtCore import *
-import os
-import json
-from functools import partial
-from ez_settings import EZSettings
-from datetime import datetime, timedelta
-# import ez_icons
-# from ez_icons import i, c
-
-from .settings_dialog import SettingsDialog
-
-from .server import Server
-from .lua_syntax_highlighter import SimpleLuaHighlighter
-from .log_highlighter import LogHighlighter
-# from .variables_tree import VariablesTree
-from .ui.dcs_code_injector_window_ui import Ui_MainWindow
-ICON = os.path.join(os.path.dirname(__file__), "ui", "icons", "icon.png")
-
-CODE_INSERTS = {
-    "base": ["BASE:I()", -1],
-    "msg_to_all": ["MessageToAll()", -1]
-}
-
-class CodeInjectorWindow(QMainWindow, Ui_MainWindow):
-    def __init__(self):
-        super().__init__()
-        self.setupUi(self)
-        self.setWindowIcon(QIcon(ICON))
-        self.resize(1280, 800)
-        self.setWindowTitle("DCS Code Injector")
-
-        self.favorites_widget = FavoritesWidget()
-        self.favorites_layout.addWidget(self.favorites_widget)
-
-        # self.variables_tree = VariablesTree()
-        # self.variables_layout.addWidget(self.variables_tree)
-
-        self.last_log_file_size = 0
-
-        self.log_file = EZSettings().get("log_file", "")
-        self.previous = []
-        LogHighlighter(self.txt_log.document())
-        self.read_log()
-
-        self.load()
-
-        self.log_font_size = 10
-        self.update_log_font_size()
-
-        self.server = Server()
-        self.server_thread = QThread()
-        self.server.moveToThread(self.server_thread)
-
-        self.timer = QTimer()
-        self.timer.setInterval(500)
-        self.timer.timeout.connect(self.read_log)
-        self.timer.start()
-
-        self.connect_signals()
-
-        QCoreApplication.instance().aboutToQuit.connect(self.stop_server)
-
-        self.connection_label = QLabel()
-        self.statusbar.addWidget(self.connection_label)
-        self.on_disconnected()
-
-        self.show()
-
-    def read_log(self):
-        if not os.path.isfile(self.log_file):
-            self.show_settings()
-            self.log_file = EZSettings().get("log_file", "")
-
-        file_size = os.path.getsize(self.log_file)
-        if file_size > self.last_log_file_size:
-            with open(self.log_file, "r", encoding="utf-8") as read_file:
-                original_lines = read_file.readlines()
-            lines = []
-
-            for line in original_lines:
-                try:
-                    line = line.replace("                    ", "   ")
-                    time_str = line[0:22]
-                    time = datetime.strptime(time_str, "%Y-%m-%d %H:%M:%S.%f")
-                    shift_hours = EZSettings().get("shift_hours", 0)
-                    time += timedelta(hours=shift_hours)
-                    shifted_time_str = time.strftime("%Y-%m-%d %H:%M:%S.%f")[:-4]
-                    line = line.replace(time_str, shifted_time_str)
-                    lines.append(line)
-                except:
-                    pass
-
-            diff = len(lines) - len(self.previous)
-            if diff > 0:
-                if diff == len(lines):
-                    new_text = "".join(lines)
-                else:
-                    new_lines = lines[-diff:]
-                    new_text = "".join(new_lines)
-                self.add_text_to_log(new_text)
-            self.previous = lines
-        self.last_log_file_size = file_size
-
-    def connect_signals(self):
-        self.tab_widget.tabBarDoubleClicked.connect(self.rename_tab)
-        self.tab_widget.tabCloseRequested.connect(self.close_tab)
-        self.action_settings.triggered.connect(self.show_settings)
-        self.action_clear_log.triggered.connect(self.clear_log)
-        self.favorites_widget.new_button_added.connect(self.connect_favorite_button)
-
-        self.server_thread.started.connect(self.server.start)
-        self.server.connected.connect(self.on_connected)
-        self.server.received.connect(self.on_received)
-        self.server.disconnected.connect(self.on_disconnected)
-        self.server_thread.start()
-
-    def on_received(self, data):
-        try:
-            data = json.loads(data.strip())
-            if data.get("connection", "") == "not_active":
-                print("connection closed!")
-
-        except json.decoder.JSONDecodeError as err:
-            print(err)
-
-    def on_connected(self):
-        pixmap = QPixmap(os.path.join(os.path.dirname(__file__), "ui", "icons", "cloud_done.png"))
-        pixmap = pixmap.scaledToWidth(20, Qt.SmoothTransformation)
-        self.connection_label.setPixmap(pixmap)
-        self.statusbar.showMessage("Connected to DCS", 2500)
-
-    def on_disconnected(self):
-        pixmap = QPixmap(os.path.join(os.path.dirname(__file__), "ui", "icons", "cloud_off.png"))
-        pixmap = pixmap.scaledToWidth(20, Qt.SmoothTransformation)
-        self.connection_label.setPixmap(pixmap)
-        self.statusbar.showMessage("Disconnected from DCS", 2500)
-
-    def stop_server(self):
-        print("killing server")
-        self.server.exit = True
-        self.server_thread.quit()
-        self.server_thread.wait()
-
-    def clear_log(self):
-        self.add_text_to_log("\n" * 60)
-
-    def update_log_font_size(self):
-        self.txt_log.setStyleSheet(f"font: {self.log_font_size}pt 'Courier New';")
-
-    def connect_favorite_button(self, favorite_button):
-        favorite_button.clicked.connect(partial(self.set_server_response, favorite_button.code))
-        favorite_button.open_tab_with_code.connect(partial(self.add_new_tab))
-
-    def close_tab(self, tab_index):
-        answer = QMessageBox.question(self, 'Close', "Are you sure you want to remove this tab?", QMessageBox.Yes, QMessageBox.No)
-        if answer == QMessageBox.Yes:
-            setting_name = self.tab_widget.tabText(tab_index)
-            if tab_index > 0:
-                new_index = tab_index - 1
-            else:
-                new_index = 0
-
-            self.tab_widget.setCurrentIndex(new_index)
-            self.tab_widget.removeTab(tab_index)
-            EZSettings().remove(setting_name)
-
-    def add_new_tab(self, name=None, code=None):
-        code_text_edit = CodeTextEdit()
-        code_text_edit.textChanged.connect(self.save_code)
-        self.tab_widget.insertTab(self.tab_widget.count() - 1, code_text_edit, "UNNAMED")
-
-        self.tab_widget.setCurrentIndex(self.tab_widget.count() - 2)
-        if name is not None:
-            self.tab_widget.setTabText(self.tab_widget.currentIndex(), name)
-        if code is not None:
-            self.tab_widget.currentWidget().setPlainText(code)
-        else:
-            self.tab_widget.currentWidget().setPlainText("log.write(\"DCS Code Injector\", log.INFO, \"Hello, DCS!\")\n")
-
-    def rename_tab(self):
-        name, accepted = QInputDialog().getText(self, "DCS Code Injector", "Enter a name for this tab: ", QLineEdit.Normal, "")
-        if not accepted:
-            return
-
-        for index in range(self.tab_widget.count()):
-            tab_name = self.tab_widget.tabText(index)
-            if tab_name == name:
-                name = name + "_01"
-
-        self.tab_widget.setTabText(self.tab_widget.currentIndex(), name)
-        self.save_code()
-
-    def load(self):
-        for setting in EZSettings().get_all_settings():
-            if setting != "log_file" and setting != "shift_hours" and not setting.startswith("btn_"):
-                self.add_new_tab(name=setting, code=EZSettings().get(setting))
-            if setting.startswith("btn_"):
-                self.favorites_widget.add_new_button(setting.replace("btn_", ""), EZSettings().get(setting))
-
-    def save_code(self):
-        tab_name = self.tab_widget.tabText(self.tab_widget.currentIndex())
-        code = self.tab_widget.currentWidget().toPlainText()
-        if code != "" and not tab_name == "UNNAMED":
-            EZSettings().set(tab_name, code)
-
-    def show_settings(self):
-        dlg = SettingsDialog()
-        dlg.exec_()
-        self.setWindowTitle(f"DCS Code Injector - {dlg.txt_log_file.text()}")
-
-    def add_code_to_log(self, text):
-        line_number = 1
-        numbered_lines = []
-        numbered_lines.append("\n------------------- CODE BLOCK -------------------")
-        for line in text.split("\n"):
-            line = f"{str(line_number).zfill(2)}          {line}"
-            numbered_lines.append(line)
-            line_number += 1
-        numbered_lines.append("\n------------------ /CODE BLOCK -------------------\n")
-        complete_text = "\n".join(numbered_lines)
-        self.add_text_to_log(complete_text)
-
-    def add_text_to_log(self, complete_text):
-        self.txt_log.moveCursor(QTextCursor.End)
-        self.txt_log.insertPlainText(complete_text)
-        self.txt_log.verticalScrollBar().setValue(self.txt_log.verticalScrollBar().maximum())
-
-    def set_server_response(self, code):
-        self.add_code_to_log(code)
-        self.server.response = code
-
-    def keyPressEvent(self, event: QKeyEvent) -> None:
-        if event.key() == Qt.Key_Enter or event.key() == Qt.Key_Return and event.modifiers() == Qt.ControlModifier:
-            text = self.tab_widget.currentWidget().textCursor().selection().toPlainText()
-            self.set_server_response(text)
-
-        if event.key() == Qt.Key_F5:
-            self.read_log()
-
-        if event.key() == Qt.Key_N and event.modifiers() == Qt.ControlModifier:
-            self.add_new_tab(name="UNNAMED", code="-- add code here")
-
-        if event.key() == Qt.Key_Up and event.modifiers() == Qt.ControlModifier:
-            self.tab_widget.currentWidget().font_size += 1
-            self.tab_widget.currentWidget().update_document_size()
-            self.log_font_size = self.tab_widget.currentWidget().font_size
-            self.update_log_font_size()
-        if event.key() == Qt.Key_Down and event.modifiers() == Qt.ControlModifier:
-            self.tab_widget.currentWidget().font_size -= 1
-            self.tab_widget.currentWidget().update_document_size()
-            self.log_font_size = self.tab_widget.currentWidget().font_size
-            self.update_log_font_size()
-
-
-class CodeTextEdit(QPlainTextEdit):
-    def __init__(self):
-        super().__init__()
-
-        self.font_size = 10
-        self.update_document_size()
-        SimpleLuaHighlighter(self.document())
-
-    def update_document_size(self):
-        self.setStyleSheet(f"font: {self.font_size}pt 'Courier New';")
-
-    def get_selected_text(self):
-        return self.textCursor().selectedText()
-
-    def __insert_code(self, text, move_back_pos):
-        cursor = self.textCursor()
-        selected_text = cursor.selection().toPlainText()
-        self.insertPlainText(text)
-        pos = cursor.position() + move_back_pos
-        cursor.setPosition(pos)
-        self.setTextCursor(cursor)
-        self.insertPlainText(selected_text)
-
-    def keyPressEvent(self, event: QKeyEvent) -> None:
-        if event.key() == Qt.Key_Slash and event.modifiers() == Qt.ControlModifier:
-            cursor = self.textCursor()
-            selected_text = cursor.selection().toPlainText()
-            lines = selected_text.split("\n")
-            commented_lines = []
-            for line in lines:
-                if line.startswith("-- "):
-                    line = line.replace("-- ", "")
-                else:
-                    line = "-- " + line
-                commented_lines.append(line)
-
-            self.insertPlainText("\n".join(commented_lines))
-        if event.key() == Qt.Key_Up and event.modifiers() == Qt.ControlModifier:
-            self.font_size += 1
-            self.update_document_size()
-        if event.key() == Qt.Key_Down and event.modifiers() == Qt.ControlModifier:
-            self.font_size -= 1
-            self.update_document_size()
-        if event.key() == Qt.Key_P and event.modifiers() == Qt.ControlModifier:
-            self.__insert_code("BASE:I()", -1)
-        if event.key() == Qt.Key_M and event.modifiers() == Qt.ControlModifier:
-            self.__insert_code("MessageToAll()", -1)
-        if event.key() == Qt.Key_QuoteDbl:
-            self.__insert_code('"', -1)
-        if event.key() == Qt.Key_BraceLeft:
-            self.__insert_code("}", -1)
-        if event.key() == Qt.Key_BracketLeft:
-            self.__insert_code("]", -1)
-        if event.key() == Qt.Key_ParenLeft:
-            self.__insert_code(")", -1)
-
-        super().keyPressEvent(event)
-
-
-class FavoritesButton(QPushButton):
-    exec_code = Signal(str)
-    delete = Signal()
-    open_tab_with_code = Signal(str, str)
-    def __init__(self, label, code):
-        super().__init__()
-        self.label = label
-        self.code = code
-        self.setText(label)
-        self.setMaximumWidth(150)
-        self.setContextMenuPolicy(Qt.CustomContextMenu)
-        self.customContextMenuRequested.connect(self.show_menu)
-
-    def show_menu(self):
-        build_menu_from_action_list(
-            [
-                {"Delete": self.remove},
-                {"Open as tab": self.open_as_tab}
-            ])
-
-    def remove(self):
-        self.delete.emit()
-
-    def open_as_tab(self):
-        self.open_tab_with_code.emit(self.label, self.code)
-
-
-class FavoritesWidget(QWidget):
-    new_button_added = Signal(FavoritesButton)
-    def __init__(self):
-        super().__init__()
-        self.setAcceptDrops(True)
-        self.lay = QHBoxLayout()
-        self.lay.setSpacing(2)
-        self.lay.setContentsMargins(0, 0, 10, 10)
-        self.setLayout(self.lay)
-        self.layout().setAlignment(Qt.AlignLeft)
-        self.setMaximumHeight(35)
-        self.setAttribute(Qt.WA_StyledBackground, True)
-        # self.setStyleSheet("background-color: white;")
-
-    def add_new_button(self, label, code):
-        button = FavoritesButton(label, code)
-        self.layout().addWidget(button)
-        EZSettings().set(f"btn_{label}", code)
-
-        self.new_button_added.emit(button)
-        button.delete.connect(partial(self.delete_button, button))
-
-    def delete_button(self, button):
-        button.setParent(None)
-        # self.lay.removeWidget(button)
-        button.deleteLater()
-        EZSettings().remove(f"btn_{button.text()}")
-
-    def dragEnterEvent(self, event):
-        event.accept() if event.mimeData().hasText() else event.ignore()
-
-    def dragMoveEvent(self, event):
-        event.accept() if event.mimeData().hasText() else event.ignore()
-
-    def dropEvent(self, event):
-        if event.mimeData().hasText():
-            event.setDropAction(Qt.CopyAction)
-
-            label, accepted = QInputDialog().getText(self.parent(), "DCS Code Injector", "Name:")
-            if accepted:
-                self.add_new_button(label, event.mimeData().text())
-            event.accept()
-        else:
-            event.ignore()
-
-
-def build_menu_from_action_list(actions, menu=None, is_sub_menu=False):
-    if not menu:
-        menu = QMenu()
-
-    for action in actions:
-        if action == "-":
-            menu.addSeparator()
-            continue
-
-        for action_title, action_command in action.items():
-            if isinstance(action_command, list):
-                sub_menu = menu.addMenu(action_title)
-                build_menu_from_action_list(action_command, menu=sub_menu, is_sub_menu=True)
-                continue
-
-            atn = menu.addAction(action_title)
-            atn.triggered.connect(action_command)
-
-    if not is_sub_menu:
-        cursor = QCursor()
-        menu.exec_(cursor.pos())
-
+from PySide6.QtWidgets import *
+from PySide6.QtGui import *
+from PySide6.QtCore import *
+import os
+import json
+from functools import partial
+from ez_settings import EZSettings
+from datetime import datetime, timedelta
+# import ez_icons
+# from ez_icons import i, c
+
+from .settings_dialog import SettingsDialog
+
+from .server import Server
+from .lua_syntax_highlighter import SimpleLuaHighlighter
+from .log_highlighter import LogHighlighter
+# from .variables_tree import VariablesTree
+from .ui.dcs_code_injector_window_ui import Ui_MainWindow
+ICON = os.path.join(os.path.dirname(__file__), "ui", "icons", "icon.png")
+
+CODE_INSERTS = {
+    "base": ["BASE:I()", -1],
+    "msg_to_all": ["MessageToAll()", -1]
+}
+
+class CodeInjectorWindow(QMainWindow, Ui_MainWindow):
+    def __init__(self):
+        super().__init__()
+        self.setupUi(self)
+        self.setWindowIcon(QIcon(ICON))
+        self.resize(1280, 800)
+        self.setWindowTitle("DCS Code Injector")
+
+        self.favorites_widget = FavoritesWidget()
+        self.favorites_layout.addWidget(self.favorites_widget)
+
+        # self.variables_tree = VariablesTree()
+        # self.variables_layout.addWidget(self.variables_tree)
+
+        self.last_log_file_size = 0
+
+        self.log_file = EZSettings().get("log_file", "")
+        self.previous = []
+        LogHighlighter(self.txt_log.document())
+        self.read_log()
+
+        self.load()
+
+        self.log_font_size = 10
+        self.update_log_font_size()
+
+        self.server = Server()
+        self.server_thread = QThread()
+        self.server.moveToThread(self.server_thread)
+
+        self.timer = QTimer()
+        self.timer.setInterval(500)
+        self.timer.timeout.connect(self.read_log)
+        self.timer.start()
+
+        self.connect_signals()
+
+        QCoreApplication.instance().aboutToQuit.connect(self.stop_server)
+
+        self.connection_label = QLabel()
+        self.statusbar.addWidget(self.connection_label)
+        self.on_disconnected()
+
+        self.show()
+
+    def read_log(self):
+        if not os.path.isfile(self.log_file):
+            self.show_settings()
+            self.log_file = EZSettings().get("log_file", "")
+
+        file_size = os.path.getsize(self.log_file)
+        if file_size > self.last_log_file_size:
+            with open(self.log_file, "r", encoding="utf-8") as read_file:
+                original_lines = read_file.readlines()
+            lines = []
+
+            for line in original_lines:
+                try:
+                    line = line.replace("                    ", "   ")
+                    time_str = line[0:22]
+                    time = datetime.strptime(time_str, "%Y-%m-%d %H:%M:%S.%f")
+                    shift_hours = EZSettings().get("shift_hours", 0)
+                    time += timedelta(hours=shift_hours)
+                    shifted_time_str = time.strftime("%Y-%m-%d %H:%M:%S.%f")[:-4]
+                    line = line.replace(time_str, shifted_time_str)
+                    lines.append(line)
+                except:
+                    pass
+
+            diff = len(lines) - len(self.previous)
+            if diff > 0:
+                if diff == len(lines):
+                    new_text = "".join(lines)
+                else:
+                    new_lines = lines[-diff:]
+                    new_text = "".join(new_lines)
+                self.add_text_to_log(new_text)
+            self.previous = lines
+        self.last_log_file_size = file_size
+
+    def connect_signals(self):
+        self.tab_widget.tabBarDoubleClicked.connect(self.rename_tab)
+        self.tab_widget.tabCloseRequested.connect(self.close_tab)
+        self.action_settings.triggered.connect(self.show_settings)
+        self.action_clear_log.triggered.connect(self.clear_log)
+        self.favorites_widget.new_button_added.connect(self.connect_favorite_button)
+
+        self.server_thread.started.connect(self.server.start)
+        self.server.connected.connect(self.on_connected)
+        self.server.received.connect(self.on_received)
+        self.server.disconnected.connect(self.on_disconnected)
+        self.server_thread.start()
+
+    def on_received(self, data):
+        try:
+            data = json.loads(data.strip())
+            if data.get("connection", "") == "not_active":
+                print("connection closed!")
+
+        except json.decoder.JSONDecodeError as err:
+            print(err)
+
+    def on_connected(self):
+        pixmap = QPixmap(os.path.join(os.path.dirname(__file__), "ui", "icons", "cloud_done.png"))
+        pixmap = pixmap.scaledToWidth(20, Qt.SmoothTransformation)
+        self.connection_label.setPixmap(pixmap)
+        self.statusbar.showMessage("Connected to DCS", 2500)
+
+    def on_disconnected(self):
+        pixmap = QPixmap(os.path.join(os.path.dirname(__file__), "ui", "icons", "cloud_off.png"))
+        pixmap = pixmap.scaledToWidth(20, Qt.SmoothTransformation)
+        self.connection_label.setPixmap(pixmap)
+        self.statusbar.showMessage("Disconnected from DCS", 2500)
+
+    def stop_server(self):
+        print("killing server")
+        self.server.exit = True
+        self.server_thread.quit()
+        self.server_thread.wait()
+
+    def clear_log(self):
+        self.add_text_to_log("\n" * 60)
+
+    def update_log_font_size(self):
+        self.txt_log.setStyleSheet(f"font: {self.log_font_size}pt 'Courier New';")
+
+    def connect_favorite_button(self, favorite_button):
+        favorite_button.clicked.connect(partial(self.set_server_response, favorite_button.code))
+        favorite_button.open_tab_with_code.connect(partial(self.add_new_tab))
+
+    def close_tab(self, tab_index):
+        answer = QMessageBox.question(self, 'Close', "Are you sure you want to remove this tab?", QMessageBox.Yes, QMessageBox.No)
+        if answer == QMessageBox.Yes:
+            setting_name = self.tab_widget.tabText(tab_index)
+            if tab_index > 0:
+                new_index = tab_index - 1
+            else:
+                new_index = 0
+
+            self.tab_widget.setCurrentIndex(new_index)
+            self.tab_widget.removeTab(tab_index)
+            EZSettings().remove(setting_name)
+
+    def add_new_tab(self, name=None, code=None):
+        code_text_edit = CodeTextEdit()
+        code_text_edit.textChanged.connect(self.save_code)
+        self.tab_widget.insertTab(self.tab_widget.count() - 1, code_text_edit, "UNNAMED")
+
+        self.tab_widget.setCurrentIndex(self.tab_widget.count() - 2)
+        if name is not None:
+            self.tab_widget.setTabText(self.tab_widget.currentIndex(), name)
+        if code is not None:
+            self.tab_widget.currentWidget().setPlainText(code)
+        else:
+            self.tab_widget.currentWidget().setPlainText("log.write(\"DCS Code Injector\", log.INFO, \"Hello, DCS!\")\n")
+
+    def rename_tab(self):
+        name, accepted = QInputDialog().getText(self, "DCS Code Injector", "Enter a name for this tab: ", QLineEdit.Normal, "")
+        if not accepted:
+            return
+
+        for index in range(self.tab_widget.count()):
+            tab_name = self.tab_widget.tabText(index)
+            if tab_name == name:
+                name = name + "_01"
+
+        self.tab_widget.setTabText(self.tab_widget.currentIndex(), name)
+        self.save_code()
+
+    def load(self):
+        for setting in EZSettings().get_all_settings():
+            if setting != "log_file" and setting != "shift_hours" and not setting.startswith("btn_"):
+                self.add_new_tab(name=setting, code=EZSettings().get(setting))
+            if setting.startswith("btn_"):
+                self.favorites_widget.add_new_button(setting.replace("btn_", ""), EZSettings().get(setting))
+
+    def save_code(self):
+        tab_name = self.tab_widget.tabText(self.tab_widget.currentIndex())
+        code = self.tab_widget.currentWidget().toPlainText()
+        if code != "" and not tab_name == "UNNAMED":
+            EZSettings().set(tab_name, code)
+
+    def show_settings(self):
+        dlg = SettingsDialog()
+        dlg.exec_()
+        self.setWindowTitle(f"DCS Code Injector - {dlg.txt_log_file.text()}")
+
+    def add_code_to_log(self, text):
+        line_number = 1
+        numbered_lines = []
+        numbered_lines.append("\n------------------- CODE BLOCK -------------------")
+        for line in text.split("\n"):
+            line = f"{str(line_number).zfill(2)}          {line}"
+            numbered_lines.append(line)
+            line_number += 1
+        numbered_lines.append("\n------------------ /CODE BLOCK -------------------\n")
+        complete_text = "\n".join(numbered_lines)
+        self.add_text_to_log(complete_text)
+
+    def add_text_to_log(self, complete_text):
+        self.txt_log.moveCursor(QTextCursor.End)
+        self.txt_log.insertPlainText(complete_text)
+        self.txt_log.verticalScrollBar().setValue(self.txt_log.verticalScrollBar().maximum())
+
+    def set_server_response(self, code):
+        self.add_code_to_log(code)
+        self.server.response = code
+
+    def keyPressEvent(self, event: QKeyEvent) -> None:
+        if event.key() == Qt.Key_Enter or event.key() == Qt.Key_Return and event.modifiers() == Qt.ControlModifier:
+            text = self.tab_widget.currentWidget().textCursor().selection().toPlainText()
+            self.set_server_response(text)
+
+        if event.key() == Qt.Key_F5:
+            self.read_log()
+
+        if event.key() == Qt.Key_N and event.modifiers() == Qt.ControlModifier:
+            self.add_new_tab(name="UNNAMED", code="-- add code here")
+
+        if event.key() == Qt.Key_Up and event.modifiers() == Qt.ControlModifier:
+            self.tab_widget.currentWidget().font_size += 1
+            self.tab_widget.currentWidget().update_document_size()
+            self.log_font_size = self.tab_widget.currentWidget().font_size
+            self.update_log_font_size()
+        if event.key() == Qt.Key_Down and event.modifiers() == Qt.ControlModifier:
+            self.tab_widget.currentWidget().font_size -= 1
+            self.tab_widget.currentWidget().update_document_size()
+            self.log_font_size = self.tab_widget.currentWidget().font_size
+            self.update_log_font_size()
+
+
+class CodeTextEdit(QPlainTextEdit):
+    def __init__(self):
+        super().__init__()
+
+        self.font_size = 10
+        self.update_document_size()
+        SimpleLuaHighlighter(self.document())
+
+    def update_document_size(self):
+        self.setStyleSheet(f"font: {self.font_size}pt 'Courier New';")
+
+    def get_selected_text(self):
+        return self.textCursor().selectedText()
+
+    def __insert_code(self, text, move_back_pos):
+        cursor = self.textCursor()
+        selected_text = cursor.selection().toPlainText()
+        self.insertPlainText(text)
+        pos = cursor.position() + move_back_pos
+        cursor.setPosition(pos)
+        self.setTextCursor(cursor)
+        self.insertPlainText(selected_text)
+
+    def keyPressEvent(self, event: QKeyEvent) -> None:
+        if event.key() == Qt.Key_Slash and event.modifiers() == Qt.ControlModifier:
+            cursor = self.textCursor()
+            selected_text = cursor.selection().toPlainText()
+            lines = selected_text.split("\n")
+            commented_lines = []
+            for line in lines:
+                if line.startswith("-- "):
+                    line = line.replace("-- ", "")
+                else:
+                    line = "-- " + line
+                commented_lines.append(line)
+
+            self.insertPlainText("\n".join(commented_lines))
+        if event.key() == Qt.Key_Up and event.modifiers() == Qt.ControlModifier:
+            self.font_size += 1
+            self.update_document_size()
+        if event.key() == Qt.Key_Down and event.modifiers() == Qt.ControlModifier:
+            self.font_size -= 1
+            self.update_document_size()
+        if event.key() == Qt.Key_P and event.modifiers() == Qt.ControlModifier:
+            self.__insert_code("BASE:I()", -1)
+        if event.key() == Qt.Key_M and event.modifiers() == Qt.ControlModifier:
+            self.__insert_code("MessageToAll()", -1)
+        if event.key() == Qt.Key_QuoteDbl:
+            self.__insert_code('"', -1)
+        if event.key() == Qt.Key_BraceLeft:
+            self.__insert_code("}", -1)
+        if event.key() == Qt.Key_BracketLeft:
+            self.__insert_code("]", -1)
+        if event.key() == Qt.Key_ParenLeft:
+            self.__insert_code(")", -1)
+
+        super().keyPressEvent(event)
+
+
+class FavoritesButton(QPushButton):
+    exec_code = Signal(str)
+    delete = Signal()
+    open_tab_with_code = Signal(str, str)
+    def __init__(self, label, code):
+        super().__init__()
+        self.label = label
+        self.code = code
+        self.setText(label)
+        self.setMaximumWidth(150)
+        self.setContextMenuPolicy(Qt.CustomContextMenu)
+        self.customContextMenuRequested.connect(self.show_menu)
+
+    def show_menu(self):
+        build_menu_from_action_list(
+            [
+                {"Delete": self.remove},
+                {"Open as tab": self.open_as_tab}
+            ])
+
+    def remove(self):
+        self.delete.emit()
+
+    def open_as_tab(self):
+        self.open_tab_with_code.emit(self.label, self.code)
+
+
+class FavoritesWidget(QWidget):
+    new_button_added = Signal(FavoritesButton)
+    def __init__(self):
+        super().__init__()
+        self.setAcceptDrops(True)
+        self.lay = QHBoxLayout()
+        self.lay.setSpacing(2)
+        self.lay.setContentsMargins(0, 0, 10, 10)
+        self.setLayout(self.lay)
+        self.layout().setAlignment(Qt.AlignLeft)
+        self.setMaximumHeight(35)
+        self.setAttribute(Qt.WA_StyledBackground, True)
+        # self.setStyleSheet("background-color: white;")
+
+    def add_new_button(self, label, code):
+        button = FavoritesButton(label, code)
+        self.layout().addWidget(button)
+        EZSettings().set(f"btn_{label}", code)
+
+        self.new_button_added.emit(button)
+        button.delete.connect(partial(self.delete_button, button))
+
+    def delete_button(self, button):
+        button.setParent(None)
+        # self.lay.removeWidget(button)
+        button.deleteLater()
+        EZSettings().remove(f"btn_{button.text()}")
+
+    def dragEnterEvent(self, event):
+        event.accept() if event.mimeData().hasText() else event.ignore()
+
+    def dragMoveEvent(self, event):
+        event.accept() if event.mimeData().hasText() else event.ignore()
+
+    def dropEvent(self, event):
+        if event.mimeData().hasText():
+            event.setDropAction(Qt.CopyAction)
+
+            label, accepted = QInputDialog().getText(self.parent(), "DCS Code Injector", "Name:")
+            if accepted:
+                self.add_new_button(label, event.mimeData().text())
+            event.accept()
+        else:
+            event.ignore()
+
+
+def build_menu_from_action_list(actions, menu=None, is_sub_menu=False):
+    if not menu:
+        menu = QMenu()
+
+    for action in actions:
+        if action == "-":
+            menu.addSeparator()
+            continue
+
+        for action_title, action_command in action.items():
+            if isinstance(action_command, list):
+                sub_menu = menu.addMenu(action_title)
+                build_menu_from_action_list(action_command, menu=sub_menu, is_sub_menu=True)
+                continue
+
+            atn = menu.addAction(action_title)
+            atn.triggered.connect(action_command)
+
+    if not is_sub_menu:
+        cursor = QCursor()
+        menu.exec_(cursor.pos())
+
     return menu
```

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/log_highlighter.py` & `dcs-code-injector-1.0.4/dcs_code_injector/log_highlighter.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from PySide6.QtCore import *
-from PySide6.QtGui import *
-
-
-class LogHighlighter(QSyntaxHighlighter):
-    def __init__(self, doc):
-        self.rules = {
-            r"^.*\b(SCRIPTING)\b.*$": self.make_format(foreground_color=Qt.cyan),
-            r"^.*\b(WARNING)\b.*$": self.make_format(foreground_color=Qt.yellow),
-            r"^.*\b(ERROR|stack traceback|in function|in main chunk)\b.*$": self.make_format(Qt.red),
-            r"^.*(\/E:).*$": self.make_format(Qt.red),
-            r"^.*\b(ERROR_ONCE)\b.*$": self.make_format(QColor(255, 139, 30)),
-            r"^.*\b(MOOSE INCLUDE END|MOOSE STATIC INCLUDE START)\b.*$": self.make_format(QColor(54, 194, 72)),
-        }
-        super().__init__(doc)
-
-    def highlightBlock(self, text: str) -> None:
-        for regex, format in self.rules.items():
-            i = QRegularExpression(regex).globalMatch(text)
-            while i.hasNext():
-                match = i.next()
-                self.setFormat(match.capturedStart(), match.capturedLength(), format)
-
-    def make_format(self, background_color=Qt.transparent, foreground_color=Qt.white):
-        format = QTextCharFormat()
-        format.setBackground(background_color)
-        format.setForeground(foreground_color)
-        return format
+from PySide6.QtCore import *
+from PySide6.QtGui import *
+
+
+class LogHighlighter(QSyntaxHighlighter):
+    def __init__(self, doc):
+        self.rules = {
+            r"^.*\b(SCRIPTING)\b.*$": self.make_format(foreground_color=Qt.cyan),
+            r"^.*\b(WARNING)\b.*$": self.make_format(foreground_color=Qt.yellow),
+            r"^.*\b(ERROR|stack traceback|in function|in main chunk)\b.*$": self.make_format(Qt.red),
+            r"^.*(\/E:).*$": self.make_format(Qt.red),
+            r"^.*\b(ERROR_ONCE)\b.*$": self.make_format(QColor(255, 139, 30)),
+            r"^.*\b(MOOSE INCLUDE END|MOOSE STATIC INCLUDE START)\b.*$": self.make_format(QColor(54, 194, 72)),
+        }
+        super().__init__(doc)
+
+    def highlightBlock(self, text: str) -> None:
+        for regex, format in self.rules.items():
+            i = QRegularExpression(regex).globalMatch(text)
+            while i.hasNext():
+                match = i.next()
+                self.setFormat(match.capturedStart(), match.capturedLength(), format)
+
+    def make_format(self, background_color=Qt.transparent, foreground_color=Qt.white):
+        format = QTextCharFormat()
+        format.setBackground(background_color)
+        format.setForeground(foreground_color)
+        return format
```

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/server.py` & `dcs-code-injector-1.0.4/dcs_code_injector/server.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from PySide6.QtCore import *
-import socket
-
-
-class Server(QObject):
-    connected = Signal()
-    received = Signal(object)
-    disconnected = Signal()
-
-    def __init__(self):
-        super().__init__()
-        self.response = ""
-        self.exit = False
-
-    #some messy server code, but too lazy to try and make it prettier right now
-    def start(self):
-        server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        server_socket.bind(('localhost', 40322))
-        server_socket.listen(1)
-
-        server_socket.settimeout(0.1)
-
-        while not self.exit:
-            try:
-                client_socket, address = server_socket.accept()
-                self.connected.emit()
-                data = client_socket.recv(1024).decode()
-                self.received.emit(data)
-
-                while True:
-                    if self.response != "":
-                        self.response += "\n"
-                        client_socket.settimeout(0.1)
-                        client_socket.sendall(self.response.encode())
-                        self.response = ""
-
-                    try:
-                        data = client_socket.recv(1024).decode()
-                        if data:
-                            self.received.emit(data)
-                            if data == '{"connection": "not_active"}':
-                                break
-                    except TimeoutError:
-                        print("recv timed out")
-                        break
-                    except socket.error:
-                        break
-
-                    if self.exit:
-                        break
-
-                self.disconnected.emit()
-                client_socket.close()
-
-            except TimeoutError:
-                pass
-
+from PySide6.QtCore import *
+import socket
+
+
+class Server(QObject):
+    connected = Signal()
+    received = Signal(object)
+    disconnected = Signal()
+
+    def __init__(self):
+        super().__init__()
+        self.response = ""
+        self.exit = False
+
+    #some messy server code, but too lazy to try and make it prettier right now
+    def start(self):
+        server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        server_socket.bind(('localhost', 40322))
+        server_socket.listen(1)
+
+        server_socket.settimeout(0.1)
+
+        while not self.exit:
+            try:
+                client_socket, address = server_socket.accept()
+                self.connected.emit()
+                data = client_socket.recv(1024).decode()
+                self.received.emit(data)
+
+                while True:
+                    if self.response != "":
+                        self.response += "\n"
+                        client_socket.settimeout(0.1)
+                        client_socket.sendall(self.response.encode())
+                        self.response = ""
+
+                    try:
+                        data = client_socket.recv(1024).decode()
+                        if data:
+                            self.received.emit(data)
+                            if data == '{"connection": "not_active"}':
+                                break
+                    except TimeoutError:
+                        print("recv timed out")
+                        break
+                    except socket.error:
+                        break
+
+                    if self.exit:
+                        break
+
+                self.disconnected.emit()
+                client_socket.close()
+
+            except TimeoutError:
+                pass
+
         server_socket.close()
```

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/settings_dialog.py` & `dcs-code-injector-1.0.4/dcs_code_injector/settings_dialog.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from PySide6.QtWidgets import *
-from PySide6.QtGui import *
-from ez_settings import EZSettings
-import os
-from .ui.dcs_code_injector_settings_ui import Ui_settings_dialog
-
-
-class SettingsDialog(QDialog, Ui_settings_dialog):
-    def __init__(self):
-        super().__init__()
-        self.setupUi(self)
-        self.load()
-        self.btn_browse.clicked.connect(self.open_file_browser)
-
-    def open_file_browser(self):
-        file_dialog = QFileDialog()
-        file_dialog.setDirectory(os.path.join(os.environ.get('USERPROFILE'), 'Saved Games'))
-        file_dialog.setNameFilter("Log files (*.log)")
-        file_dialog.exec_()
-
-        selected_files = file_dialog.selectedFiles()
-        if selected_files:
-            file_path = selected_files[0]
-            self.txt_log_file.setText(file_path)
-
-    def load(self):
-        self.txt_log_file.setText(EZSettings().get("log_file", ""))
-        self.spin_offset_time.setValue(EZSettings().get("shift_hours", 0))
-
-    def save(self):
-        EZSettings().set("log_file", self.txt_log_file.text())
-        EZSettings().set("shift_hours", self.spin_offset_time.value())
-
-
-    def closeEvent(self, arg__1: QCloseEvent) -> None:
-        self.save()
+from PySide6.QtWidgets import *
+from PySide6.QtGui import *
+from ez_settings import EZSettings
+import os
+from .ui.dcs_code_injector_settings_ui import Ui_settings_dialog
+
+
+class SettingsDialog(QDialog, Ui_settings_dialog):
+    def __init__(self):
+        super().__init__()
+        self.setupUi(self)
+        self.load()
+        self.btn_browse.clicked.connect(self.open_file_browser)
+
+    def open_file_browser(self):
+        file_dialog = QFileDialog()
+        file_dialog.setDirectory(os.path.join(os.environ.get('USERPROFILE'), 'Saved Games'))
+        file_dialog.setNameFilter("Log files (*.log)")
+        file_dialog.exec_()
+
+        selected_files = file_dialog.selectedFiles()
+        if selected_files:
+            file_path = selected_files[0]
+            self.txt_log_file.setText(file_path)
+
+    def load(self):
+        self.txt_log_file.setText(EZSettings().get("log_file", ""))
+        self.spin_offset_time.setValue(EZSettings().get("shift_hours", 0))
+
+    def save(self):
+        EZSettings().set("log_file", self.txt_log_file.text())
+        EZSettings().set("shift_hours", self.spin_offset_time.value())
+
+
+    def closeEvent(self, arg__1: QCloseEvent) -> None:
+        self.save()
         super().closeEvent(arg__1)
```

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/dcs_code_injector_settings_ui.py` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/dcs_code_injector_settings_ui.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'dcs_code_injector_settings_ui.ui'
-##
-## Created by: Qt User Interface Compiler version 6.5.0
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
-    QMetaObject, QObject, QPoint, QRect,
-    QSize, QTime, QUrl, Qt)
-from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
-    QFont, QFontDatabase, QGradient, QIcon,
-    QImage, QKeySequence, QLinearGradient, QPainter,
-    QPalette, QPixmap, QRadialGradient, QTransform)
-from PySide6.QtWidgets import (QApplication, QDialog, QGridLayout, QLabel,
-    QLineEdit, QPushButton, QSizePolicy, QSpinBox,
-    QWidget)
-
-class Ui_settings_dialog(object):
-    def setupUi(self, settings_dialog):
-        if not settings_dialog.objectName():
-            settings_dialog.setObjectName(u"settings_dialog")
-        settings_dialog.resize(495, 112)
-        self.gridLayout = QGridLayout(settings_dialog)
-        self.gridLayout.setObjectName(u"gridLayout")
-        self.txt_log_file = QLineEdit(settings_dialog)
-        self.txt_log_file.setObjectName(u"txt_log_file")
-
-        self.gridLayout.addWidget(self.txt_log_file, 0, 1, 1, 1)
-
-        self.temp_folder_3 = QLabel(settings_dialog)
-        self.temp_folder_3.setObjectName(u"temp_folder_3")
-
-        self.gridLayout.addWidget(self.temp_folder_3, 0, 0, 1, 1)
-
-        self.temp_folder_4 = QLabel(settings_dialog)
-        self.temp_folder_4.setObjectName(u"temp_folder_4")
-
-        self.gridLayout.addWidget(self.temp_folder_4, 1, 0, 1, 1)
-
-        self.btn_browse = QPushButton(settings_dialog)
-        self.btn_browse.setObjectName(u"btn_browse")
-
-        self.gridLayout.addWidget(self.btn_browse, 0, 2, 1, 1)
-
-        self.spin_offset_time = QSpinBox(settings_dialog)
-        self.spin_offset_time.setObjectName(u"spin_offset_time")
-        self.spin_offset_time.setMinimum(-12)
-        self.spin_offset_time.setMaximum(12)
-
-        self.gridLayout.addWidget(self.spin_offset_time, 1, 1, 1, 2)
-
-
-        self.retranslateUi(settings_dialog)
-
-        QMetaObject.connectSlotsByName(settings_dialog)
-    # setupUi
-
-    def retranslateUi(self, settings_dialog):
-        settings_dialog.setWindowTitle(QCoreApplication.translate("settings_dialog", u"Settings", None))
-        self.txt_log_file.setPlaceholderText("")
-        self.temp_folder_3.setText(QCoreApplication.translate("settings_dialog", u"Log file path", None))
-        self.temp_folder_4.setText(QCoreApplication.translate("settings_dialog", u"Offset log time", None))
-        self.btn_browse.setText(QCoreApplication.translate("settings_dialog", u"...", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'dcs_code_injector_settings_ui.ui'
+##
+## Created by: Qt User Interface Compiler version 6.5.0
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
+    QMetaObject, QObject, QPoint, QRect,
+    QSize, QTime, QUrl, Qt)
+from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
+    QFont, QFontDatabase, QGradient, QIcon,
+    QImage, QKeySequence, QLinearGradient, QPainter,
+    QPalette, QPixmap, QRadialGradient, QTransform)
+from PySide6.QtWidgets import (QApplication, QDialog, QGridLayout, QLabel,
+    QLineEdit, QPushButton, QSizePolicy, QSpinBox,
+    QWidget)
+
+class Ui_settings_dialog(object):
+    def setupUi(self, settings_dialog):
+        if not settings_dialog.objectName():
+            settings_dialog.setObjectName(u"settings_dialog")
+        settings_dialog.resize(495, 112)
+        self.gridLayout = QGridLayout(settings_dialog)
+        self.gridLayout.setObjectName(u"gridLayout")
+        self.txt_log_file = QLineEdit(settings_dialog)
+        self.txt_log_file.setObjectName(u"txt_log_file")
+
+        self.gridLayout.addWidget(self.txt_log_file, 0, 1, 1, 1)
+
+        self.temp_folder_3 = QLabel(settings_dialog)
+        self.temp_folder_3.setObjectName(u"temp_folder_3")
+
+        self.gridLayout.addWidget(self.temp_folder_3, 0, 0, 1, 1)
+
+        self.temp_folder_4 = QLabel(settings_dialog)
+        self.temp_folder_4.setObjectName(u"temp_folder_4")
+
+        self.gridLayout.addWidget(self.temp_folder_4, 1, 0, 1, 1)
+
+        self.btn_browse = QPushButton(settings_dialog)
+        self.btn_browse.setObjectName(u"btn_browse")
+
+        self.gridLayout.addWidget(self.btn_browse, 0, 2, 1, 1)
+
+        self.spin_offset_time = QSpinBox(settings_dialog)
+        self.spin_offset_time.setObjectName(u"spin_offset_time")
+        self.spin_offset_time.setMinimum(-12)
+        self.spin_offset_time.setMaximum(12)
+
+        self.gridLayout.addWidget(self.spin_offset_time, 1, 1, 1, 2)
+
+
+        self.retranslateUi(settings_dialog)
+
+        QMetaObject.connectSlotsByName(settings_dialog)
+    # setupUi
+
+    def retranslateUi(self, settings_dialog):
+        settings_dialog.setWindowTitle(QCoreApplication.translate("settings_dialog", u"Settings", None))
+        self.txt_log_file.setPlaceholderText("")
+        self.temp_folder_3.setText(QCoreApplication.translate("settings_dialog", u"Log file path", None))
+        self.temp_folder_4.setText(QCoreApplication.translate("settings_dialog", u"Offset log time", None))
+        self.btn_browse.setText(QCoreApplication.translate("settings_dialog", u"...", None))
+    # retranslateUi
+
```

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/dcs_code_injector_window_ui.py` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/dcs_code_injector_window_ui.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'dcs_code_injector_window_ui.ui'
-##
-## Created by: Qt User Interface Compiler version 6.5.0
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
-    QMetaObject, QObject, QPoint, QRect,
-    QSize, QTime, QUrl, Qt)
-from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
-    QCursor, QFont, QFontDatabase, QGradient,
-    QIcon, QImage, QKeySequence, QLinearGradient,
-    QPainter, QPalette, QPixmap, QRadialGradient,
-    QTransform)
-from PySide6.QtWidgets import (QApplication, QGridLayout, QHBoxLayout, QMainWindow,
-    QMenu, QMenuBar, QPlainTextEdit, QSizePolicy,
-    QSplitter, QStatusBar, QTabWidget, QWidget)
-
-class Ui_MainWindow(object):
-    def setupUi(self, MainWindow):
-        if not MainWindow.objectName():
-            MainWindow.setObjectName(u"MainWindow")
-        MainWindow.resize(863, 665)
-        self.action_settings = QAction(MainWindow)
-        self.action_settings.setObjectName(u"action_settings")
-        self.action_clear_execution_file = QAction(MainWindow)
-        self.action_clear_execution_file.setObjectName(u"action_clear_execution_file")
-        self.action_clear_log = QAction(MainWindow)
-        self.action_clear_log.setObjectName(u"action_clear_log")
-        self.centralwidget = QWidget(MainWindow)
-        self.centralwidget.setObjectName(u"centralwidget")
-        self.gridLayout = QGridLayout(self.centralwidget)
-        self.gridLayout.setObjectName(u"gridLayout")
-        self.log_code_splitter = QSplitter(self.centralwidget)
-        self.log_code_splitter.setObjectName(u"log_code_splitter")
-        self.log_code_splitter.setOrientation(Qt.Vertical)
-        self.log_variables_splitter = QSplitter(self.log_code_splitter)
-        self.log_variables_splitter.setObjectName(u"log_variables_splitter")
-        self.log_variables_splitter.setOrientation(Qt.Horizontal)
-        self.txt_log = QPlainTextEdit(self.log_variables_splitter)
-        self.txt_log.setObjectName(u"txt_log")
-        self.txt_log.setEnabled(True)
-        self.log_variables_splitter.addWidget(self.txt_log)
-        self.log_code_splitter.addWidget(self.log_variables_splitter)
-        self.tab_widget = QTabWidget(self.log_code_splitter)
-        self.tab_widget.setObjectName(u"tab_widget")
-        self.tab_widget.setAutoFillBackground(True)
-        self.tab_widget.setTabsClosable(True)
-        self.log_code_splitter.addWidget(self.tab_widget)
-
-        self.gridLayout.addWidget(self.log_code_splitter, 0, 0, 1, 1)
-
-        self.favorites_layout = QHBoxLayout()
-        self.favorites_layout.setObjectName(u"favorites_layout")
-
-        self.gridLayout.addLayout(self.favorites_layout, 1, 0, 1, 1)
-
-        MainWindow.setCentralWidget(self.centralwidget)
-        self.menubar = QMenuBar(MainWindow)
-        self.menubar.setObjectName(u"menubar")
-        self.menubar.setGeometry(QRect(0, 0, 863, 22))
-        self.menuFile = QMenu(self.menubar)
-        self.menuFile.setObjectName(u"menuFile")
-        self.menuTools = QMenu(self.menubar)
-        self.menuTools.setObjectName(u"menuTools")
-        MainWindow.setMenuBar(self.menubar)
-        self.statusbar = QStatusBar(MainWindow)
-        self.statusbar.setObjectName(u"statusbar")
-        MainWindow.setStatusBar(self.statusbar)
-
-        self.menubar.addAction(self.menuFile.menuAction())
-        self.menubar.addAction(self.menuTools.menuAction())
-        self.menuFile.addAction(self.action_settings)
-        self.menuTools.addAction(self.action_clear_log)
-
-        self.retranslateUi(MainWindow)
-
-        self.tab_widget.setCurrentIndex(-1)
-
-
-        QMetaObject.connectSlotsByName(MainWindow)
-    # setupUi
-
-    def retranslateUi(self, MainWindow):
-        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"MainWindow", None))
-        self.action_settings.setText(QCoreApplication.translate("MainWindow", u"Settings", None))
-        self.action_clear_execution_file.setText(QCoreApplication.translate("MainWindow", u"Clear execution file", None))
-#if QT_CONFIG(shortcut)
-        self.action_clear_execution_file.setShortcut(QCoreApplication.translate("MainWindow", u"Alt+X", None))
-#endif // QT_CONFIG(shortcut)
-        self.action_clear_log.setText(QCoreApplication.translate("MainWindow", u"Clear log", None))
-#if QT_CONFIG(shortcut)
-        self.action_clear_log.setShortcut(QCoreApplication.translate("MainWindow", u"Alt+L", None))
-#endif // QT_CONFIG(shortcut)
-        self.menuFile.setTitle(QCoreApplication.translate("MainWindow", u"File", None))
-        self.menuTools.setTitle(QCoreApplication.translate("MainWindow", u"Tools", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'dcs_code_injector_window_ui.ui'
+##
+## Created by: Qt User Interface Compiler version 6.5.0
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
+    QMetaObject, QObject, QPoint, QRect,
+    QSize, QTime, QUrl, Qt)
+from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
+    QCursor, QFont, QFontDatabase, QGradient,
+    QIcon, QImage, QKeySequence, QLinearGradient,
+    QPainter, QPalette, QPixmap, QRadialGradient,
+    QTransform)
+from PySide6.QtWidgets import (QApplication, QGridLayout, QHBoxLayout, QMainWindow,
+    QMenu, QMenuBar, QPlainTextEdit, QSizePolicy,
+    QSplitter, QStatusBar, QTabWidget, QWidget)
+
+class Ui_MainWindow(object):
+    def setupUi(self, MainWindow):
+        if not MainWindow.objectName():
+            MainWindow.setObjectName(u"MainWindow")
+        MainWindow.resize(863, 665)
+        self.action_settings = QAction(MainWindow)
+        self.action_settings.setObjectName(u"action_settings")
+        self.action_clear_execution_file = QAction(MainWindow)
+        self.action_clear_execution_file.setObjectName(u"action_clear_execution_file")
+        self.action_clear_log = QAction(MainWindow)
+        self.action_clear_log.setObjectName(u"action_clear_log")
+        self.centralwidget = QWidget(MainWindow)
+        self.centralwidget.setObjectName(u"centralwidget")
+        self.gridLayout = QGridLayout(self.centralwidget)
+        self.gridLayout.setObjectName(u"gridLayout")
+        self.log_code_splitter = QSplitter(self.centralwidget)
+        self.log_code_splitter.setObjectName(u"log_code_splitter")
+        self.log_code_splitter.setOrientation(Qt.Vertical)
+        self.log_variables_splitter = QSplitter(self.log_code_splitter)
+        self.log_variables_splitter.setObjectName(u"log_variables_splitter")
+        self.log_variables_splitter.setOrientation(Qt.Horizontal)
+        self.txt_log = QPlainTextEdit(self.log_variables_splitter)
+        self.txt_log.setObjectName(u"txt_log")
+        self.txt_log.setEnabled(True)
+        self.log_variables_splitter.addWidget(self.txt_log)
+        self.log_code_splitter.addWidget(self.log_variables_splitter)
+        self.tab_widget = QTabWidget(self.log_code_splitter)
+        self.tab_widget.setObjectName(u"tab_widget")
+        self.tab_widget.setAutoFillBackground(True)
+        self.tab_widget.setTabsClosable(True)
+        self.log_code_splitter.addWidget(self.tab_widget)
+
+        self.gridLayout.addWidget(self.log_code_splitter, 0, 0, 1, 1)
+
+        self.favorites_layout = QHBoxLayout()
+        self.favorites_layout.setObjectName(u"favorites_layout")
+
+        self.gridLayout.addLayout(self.favorites_layout, 1, 0, 1, 1)
+
+        MainWindow.setCentralWidget(self.centralwidget)
+        self.menubar = QMenuBar(MainWindow)
+        self.menubar.setObjectName(u"menubar")
+        self.menubar.setGeometry(QRect(0, 0, 863, 22))
+        self.menuFile = QMenu(self.menubar)
+        self.menuFile.setObjectName(u"menuFile")
+        self.menuTools = QMenu(self.menubar)
+        self.menuTools.setObjectName(u"menuTools")
+        MainWindow.setMenuBar(self.menubar)
+        self.statusbar = QStatusBar(MainWindow)
+        self.statusbar.setObjectName(u"statusbar")
+        MainWindow.setStatusBar(self.statusbar)
+
+        self.menubar.addAction(self.menuFile.menuAction())
+        self.menubar.addAction(self.menuTools.menuAction())
+        self.menuFile.addAction(self.action_settings)
+        self.menuTools.addAction(self.action_clear_log)
+
+        self.retranslateUi(MainWindow)
+
+        self.tab_widget.setCurrentIndex(-1)
+
+
+        QMetaObject.connectSlotsByName(MainWindow)
+    # setupUi
+
+    def retranslateUi(self, MainWindow):
+        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"MainWindow", None))
+        self.action_settings.setText(QCoreApplication.translate("MainWindow", u"Settings", None))
+        self.action_clear_execution_file.setText(QCoreApplication.translate("MainWindow", u"Clear execution file", None))
+#if QT_CONFIG(shortcut)
+        self.action_clear_execution_file.setShortcut(QCoreApplication.translate("MainWindow", u"Alt+X", None))
+#endif // QT_CONFIG(shortcut)
+        self.action_clear_log.setText(QCoreApplication.translate("MainWindow", u"Clear log", None))
+#if QT_CONFIG(shortcut)
+        self.action_clear_log.setShortcut(QCoreApplication.translate("MainWindow", u"Alt+L", None))
+#endif // QT_CONFIG(shortcut)
+        self.menuFile.setTitle(QCoreApplication.translate("MainWindow", u"File", None))
+        self.menuTools.setTitle(QCoreApplication.translate("MainWindow", u"Tools", None))
+    # retranslateUi
+
```

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/cloud_done.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/icons/cloud_done.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/cloud_off.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/icons/cloud_off.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/icons/icon.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/icons/icon.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_01.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_01.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_02.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_02.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_03.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_03.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_04.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_04.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_05.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_05.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_06.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_06.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/ui/splashscreens/splash_07.png` & `dcs-code-injector-1.0.4/dcs_code_injector/ui/splashscreens/splash_07.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector/variables_tree.py` & `dcs-code-injector-1.0.4/dcs_code_injector/variables_tree.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from PySide6.QtWidgets import *
-from PySide6.QtGui import *
-from PySide6.QtCore import *
-import json
-from ez_utils import io_utils
-from ez_qt import tree_widget
-
-VARIABLES_FILE = "C:/temp/watch_variables.json"
-
-class VariablesTree(QTreeWidget):
-    def __init__(self):
-        super(VariablesTree, self).__init__()
-        self.setHeaderLabels(["Var", "Value"])
-        self.__previous_values = {}
-
-        # self.timer = QTimer()
-        # self.timer.setInterval(250)
-        # self.timer.timeout.connect(self.update_view)
-        # self.timer.start()
-
-    def update_view(self):
-        info_dict = io_utils.read_json(VARIABLES_FILE)
-        to_remove = []
-
-        for var_name, var_value in self.__previous_values.items():
-            if not var_name in info_dict:
-                to_remove.append(self.get_item_with_text(var_name, 0))
-
-            new_value = info_dict.get(var_name)
-            item = self.get_item_with_text(var_name, 0)
-            if item is None:
-                item = QTreeWidgetItem()
-                item.setText(0, var_name)
-                item.setText(1, str(new_value))
-                self.addTopLevelItem(item)
-
-            if var_value != new_value:
-                item.setText(1, str(new_value))
-
-        self.remove_items(to_remove)
-        self.__previous_values = info_dict
-        self.resize_columns()
-
-    def get_item_with_text(self, text, column_index):
-        """
-        Returns a QTreeWidgetItem that matches the selected text for the selected column
-
-        :param tree_widget: QTreeWidget you want to search in
-        :param text: <string> text
-        :param column_index: <int> column number
-        :return: QTreeWidgetItem if found or None if not found
-        """
-        try:
-            iterator = QTreeWidgetItemIterator(self)
-            while iterator:
-                if iterator.value().text(column_index) == text:
-                    return iterator.value()
-                iterator += 1
-        except:
-            return None
-
-        return None
-
-    def remove_items(self, items=[], selected=False):
-        """
-        Removes the passed items from the tree widget
-
-        :param tree_widget: QTreeWidget to remove items from
-        :param items: <list> items you want to remove
-        :param selected: <bool> if set to True, will remove the selected items
-        :return:
-        """
-        if selected:
-            items = self.selectedItems()
-
-        root = self.invisibleRootItem()
-        for item in items:
-            (item.parent() or root).removeChild(item)
-
-    def resize_columns(self, columns="all"):
-        """
-        Sets the column size to the minimal amount needed
-
-        :param tree_widget: QTreeWidget you want to restructure
-        :param columns: <string> | <list> either the string "all" or a list with specific column numbers
-        :return:
-        """
-        if columns == "all":
-            for column in range(self.columnCount()):
-                self.resizeColumnToContents(column)
-        else:
-            for column in columns:
+from PySide6.QtWidgets import *
+from PySide6.QtGui import *
+from PySide6.QtCore import *
+import json
+from ez_utils import io_utils
+from ez_qt import tree_widget
+
+VARIABLES_FILE = "C:/temp/watch_variables.json"
+
+class VariablesTree(QTreeWidget):
+    def __init__(self):
+        super(VariablesTree, self).__init__()
+        self.setHeaderLabels(["Var", "Value"])
+        self.__previous_values = {}
+
+        # self.timer = QTimer()
+        # self.timer.setInterval(250)
+        # self.timer.timeout.connect(self.update_view)
+        # self.timer.start()
+
+    def update_view(self):
+        info_dict = io_utils.read_json(VARIABLES_FILE)
+        to_remove = []
+
+        for var_name, var_value in self.__previous_values.items():
+            if not var_name in info_dict:
+                to_remove.append(self.get_item_with_text(var_name, 0))
+
+            new_value = info_dict.get(var_name)
+            item = self.get_item_with_text(var_name, 0)
+            if item is None:
+                item = QTreeWidgetItem()
+                item.setText(0, var_name)
+                item.setText(1, str(new_value))
+                self.addTopLevelItem(item)
+
+            if var_value != new_value:
+                item.setText(1, str(new_value))
+
+        self.remove_items(to_remove)
+        self.__previous_values = info_dict
+        self.resize_columns()
+
+    def get_item_with_text(self, text, column_index):
+        """
+        Returns a QTreeWidgetItem that matches the selected text for the selected column
+
+        :param tree_widget: QTreeWidget you want to search in
+        :param text: <string> text
+        :param column_index: <int> column number
+        :return: QTreeWidgetItem if found or None if not found
+        """
+        try:
+            iterator = QTreeWidgetItemIterator(self)
+            while iterator:
+                if iterator.value().text(column_index) == text:
+                    return iterator.value()
+                iterator += 1
+        except:
+            return None
+
+        return None
+
+    def remove_items(self, items=[], selected=False):
+        """
+        Removes the passed items from the tree widget
+
+        :param tree_widget: QTreeWidget to remove items from
+        :param items: <list> items you want to remove
+        :param selected: <bool> if set to True, will remove the selected items
+        :return:
+        """
+        if selected:
+            items = self.selectedItems()
+
+        root = self.invisibleRootItem()
+        for item in items:
+            (item.parent() or root).removeChild(item)
+
+    def resize_columns(self, columns="all"):
+        """
+        Sets the column size to the minimal amount needed
+
+        :param tree_widget: QTreeWidget you want to restructure
+        :param columns: <string> | <list> either the string "all" or a list with specific column numbers
+        :return:
+        """
+        if columns == "all":
+            for column in range(self.columnCount()):
+                self.resizeColumnToContents(column)
+        else:
+            for column in columns:
                 self.resizeColumnToContents(column)
```

### Comparing `dcs-code-injector-1.0.2/dcs_code_injector.egg-info/SOURCES.txt` & `dcs-code-injector-1.0.4/dcs_code_injector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.2/setup.py` & `dcs-code-injector-1.0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import setup, find_packages
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-data_files_to_include = ["*.png", "*.jpg", "*.xml"]
-
-setup(
-    name='dcs-code-injector',
-    version='1.0.2',
-    packages=find_packages(),
-    package_data={
-        "": data_files_to_include,
-    },
-    url='https://www.github.com/nielsvaes/dcs_code_injector',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    install_requires=["ez-icons", "PySide6", "ez_qt", "ez_settings", "ez_utils", "qt_material"],
-    license='GNU v3',
-    author='Niels Vaes',
-    author_email='nielsvaes@gmail.com',
-    description='A REPL to use with Digital Combat Simulator to execute code while a mission is running.',
-
-    entry_points = {
-        'console_scripts': ['dcs-code-injector=dcs_code_injector.app:main'],
-    },
-)
+from setuptools import setup, find_packages
+
+with open("README.md", encoding='utf-8') as fh:
+    long_description = fh.read()
+
+data_files_to_include = ["*.png", "*.jpg", "*.xml"]
+
+setup(
+    name='dcs-code-injector',
+    version='1.0.4',
+    packages=find_packages(),
+    package_data={
+        "": data_files_to_include,
+    },
+    url='https://www.github.com/nielsvaes/dcs_code_injector',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    install_requires=["ez-icons", "PySide6", "ez_qt", "ez_settings", "ez_utils", "qt_material"],
+    license='GNU v3',
+    author='Niels Vaes',
+    author_email='nielsvaes@gmail.com',
+    description='A REPL to use with Digital Combat Simulator to execute code while a mission is running.',
+
+    entry_points = {
+        'console_scripts': ['dcs-code-injector=dcs_code_injector.app:main'],
+    },
+)
```

