# Comparing `tmp/python-canvas-0.3.4.tar.gz` & `tmp/python-canvas-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-canvas-0.3.4.tar", last modified: Sun Aug 21 13:05:49 2022, max compression
+gzip compressed data, was "python-canvas-0.3.5.tar", last modified: Sat Jun  3 14:57:29 2023, max compression
```

## Comparing `python-canvas-0.3.4.tar` & `python-canvas-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2022-08-21 13:05:49.263332 python-canvas-0.3.4/
--rw-r--r--   0 user      (1000) user      (1001)        0 2022-08-21 12:57:22.000000 python-canvas-0.3.4/LICENSE
--rw-r--r--   0 user      (1000) user      (1001)      985 2022-08-21 13:05:49.259999 python-canvas-0.3.4/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      422 2022-08-21 12:57:22.000000 python-canvas-0.3.4/README.md
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2022-08-21 13:05:49.243332 python-canvas-0.3.4/canvas_db/
--rw-r--r--   0 user      (1000) user      (1001)        0 2022-08-21 12:57:22.000000 python-canvas-0.3.4/canvas_db/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      214 2022-08-21 12:57:22.000000 python-canvas-0.3.4/canvas_db/config.py
--rw-r--r--   0 user      (1000) user      (1001)    69786 2022-08-21 13:01:28.000000 python-canvas-0.3.4/canvas_db/models.py
--rw-r--r--   0 user      (1000) user      (1001)      501 2022-08-21 12:57:22.000000 python-canvas-0.3.4/canvas_db/orm.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2022-08-21 13:05:49.259999 python-canvas-0.3.4/python_canvas.egg-info/
--rw-r--r--   0 user      (1000) user      (1001)      985 2022-08-21 13:05:49.000000 python-canvas-0.3.4/python_canvas.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      289 2022-08-21 13:05:49.000000 python-canvas-0.3.4/python_canvas.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1001)        1 2022-08-21 13:05:49.000000 python-canvas-0.3.4/python_canvas.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1001)       20 2022-08-21 13:05:49.000000 python-canvas-0.3.4/python_canvas.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1001)       10 2022-08-21 13:05:49.000000 python-canvas-0.3.4/python_canvas.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1001)       38 2022-08-21 13:05:49.263332 python-canvas-0.3.4/setup.cfg
--rw-r--r--   0 user      (1000) user      (1001)      815 2022-08-21 13:04:53.000000 python-canvas-0.3.4/setup.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-06-03 14:57:29.179999 python-canvas-0.3.5/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-06-03 14:39:28.000000 python-canvas-0.3.5/LICENSE
+-rw-r--r--   0 user      (1000) user      (1001)      949 2023-06-03 14:57:29.179999 python-canvas-0.3.5/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      422 2023-06-03 14:39:28.000000 python-canvas-0.3.5/README.md
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-06-03 14:57:29.179999 python-canvas-0.3.5/canvas_db/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-06-03 14:39:28.000000 python-canvas-0.3.5/canvas_db/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      214 2023-06-03 14:39:28.000000 python-canvas-0.3.5/canvas_db/config.py
+-rw-r--r--   0 user      (1000) user      (1001)    73935 2023-06-03 14:55:16.000000 python-canvas-0.3.5/canvas_db/models.py
+-rw-r--r--   0 user      (1000) user      (1001)      501 2023-06-03 14:39:28.000000 python-canvas-0.3.5/canvas_db/orm.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-06-03 14:57:29.179999 python-canvas-0.3.5/python_canvas.egg-info/
+-rw-r--r--   0 user      (1000) user      (1001)      949 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      289 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1001)        1 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1001)       20 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1001)       10 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1001)       38 2023-06-03 14:57:29.179999 python-canvas-0.3.5/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1001)      815 2023-06-03 14:55:30.000000 python-canvas-0.3.5/setup.py
```

### Comparing `python-canvas-0.3.4/PKG-INFO` & `python-canvas-0.3.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-canvas
-Version: 0.3.4
+Version: 0.3.5
 Summary: Данная библиотека содержить SqlAlchemy ORM для системы Canvas
 Home-page: https://github.com/yessenovuniversity/python_canvas
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,8 +20,7 @@
 from canvas_db.config import Config
 from canvas_db.orm import get_session
 
 
 config = Config(host='Адрес БД Canvas LMS', user='Пользователь БД Canvas LMS', passowrd='Пароль БД Canvas LMS')
 session = get_session(config)
 ```
-
```

### Comparing `python-canvas-0.3.4/canvas_db/models.py` & `python-canvas-0.3.5/canvas_db/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,15 +578,15 @@
 
     def __str__(self):
         return self.current_score
 
 
 class Submission(Base):
     """
-    Отправленные работы задании
+    Результат сдачи задания студентом
     """
     __tablename__ = 'submissions'
 
     # Идентификатор
     id = Column(Integer, primary_key=True)
 
     # Неизвестное поле
@@ -795,14 +795,123 @@
     def __repr__(self):
         return f'<Submission {self} (id={self.id} assignment_id={self.assignment_id} user_id={self.user_id})>'
 
     def __str__(self):
         return f'{self.score}'
 
 
+class QuizSubmission(Base):
+    """
+    Результат сдачи контрольной работы студентом
+    """
+    __tablename__ = 'quiz_submissions'
+
+    # Идентификатор
+    id = Column(Integer, primary_key=True)
+
+    # Контрольная работа
+    quiz_id = Column(ForeignKey('quizzes.id'))
+    quiz = relationship('Quiz')
+
+    # Версия контрольной работы (Неизвестно)
+    quiz_version = Column(Integer)
+
+    # Пользователь
+    user_id = Column(ForeignKey('users.id'))
+    user = relationship('User')
+
+    # Данные результата (В формате YAML)
+    submission_data = Column(String)
+
+    # Результат сдачи задания
+    # Когда студент сдает контрольную работу, он одновременно сдает и привязанную задание (Assignment)
+    # Поэтому как Quiz привязан к Assignment, так и quiz_submission привязан к submission
+    submission_id = Column(ForeignKey('submissions.id'))
+    submission = relationship('Submission')
+
+    # Оценка в виде числа
+    score = Column(Integer)
+
+    # Неизвестное значение (Но он обычно равен score)
+    kept_score = Column(Integer)
+
+    # Данные контрольной работы (В формате YAML)
+    # Здесь содержится данные контрольной работы (список вопросов и список ответов) на момент начатия
+    # работу студентом. Если преподаватель меняет содержимое теста во-время сдачи этим студентом, то у него
+    # ничего не меняется
+    quiz_data = Column(String)
+
+    # Когда студент начал работу
+    started_at = Column(DateTime)
+
+    # Когда работа закончена
+    end_at = Column(DateTime)
+
+    # Когда студент закончил работу
+    finished_at = Column(DateTime)
+
+    # Текущая попытка
+    attempt = Column(Integer)
+
+    # Статус работы
+    workflow_state = Column(String)
+
+    # Дата и время создания
+    created_at = Column(DateTime, server_default=func.now())
+
+    # Дата и время изменения
+    updated_at = Column(DateTIme, onupdate=func.now())
+
+    # Неизвестное значение
+    fudge_points = Column(Integer)
+
+    # Неизвестное значение (Возможно сколько максимум студент может набрать баллов)
+    quiz_points_possible = Column(Integer)
+
+    # Неизвестное значение (Возможно данные дополнительные попытки)
+    extra_attempts = Column(Integer)
+
+    # Неизвестное значение
+    temporary_user_code = Column(String)
+
+    # Неизвестное значение
+    extra_time = Column(Integer)
+
+    # Неизвестное значение
+    manually_unlocked = Column(Boolean)
+
+    # Неизвестное значение
+    manually_scored = Column(Boolean)
+
+    # Неизвестное значение
+    validation_token = Column(String)
+
+    # Неизвестное значение
+    score_before_regrade = Column(Integer)
+
+    # Неизвестное значение
+    was_preview = Column(Boolean)
+
+    # Неизвестное значение (Возможно обозначает видел ли студент свои результаты)
+    has_seen_results = Column(Boolean)
+
+    # Неизвестное значение
+    question_references_fixed = Column(Boolean)
+
+    # Корневая учетная запись
+    root_account_id = Column(ForeignKey('accounts.id'))
+    root_account = relationship('Account')
+
+    def __repr__(self):
+        return f'<QuizSubmission {self} (id={self.id} quiz_id={self.quiz_id} user_id={self.user_id})>'
+
+    def __str__(self):
+        return f'{self.score}'
+
+
 class GradingStandard(Base):
     """
     Стандарт оценки
     """
     __tablename__ = 'grading_standards'
 
     # Идентификатор
@@ -2004,15 +2113,15 @@
     # Неизвестное поле
     disable_timer_autosubmission = Column(Boolean)
 
     def __repr__(self):
         return f'<Quiz {self} (id={self.id} workflow_state={self.workflow_state})>'
 
     def __str__(self):
-        return f'{self.name}'
+        return f'{self.title}'
 
 
 class Enrollment(Base):
     """
     Модель "Участник курса"
     """
     __tablename__ = 'enrollments'
```

### Comparing `python-canvas-0.3.4/python_canvas.egg-info/PKG-INFO` & `python-canvas-0.3.5/python_canvas.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-canvas
-Version: 0.3.4
+Version: 0.3.5
 Summary: Данная библиотека содержить SqlAlchemy ORM для системы Canvas
 Home-page: https://github.com/yessenovuniversity/python_canvas
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,8 +20,7 @@
 from canvas_db.config import Config
 from canvas_db.orm import get_session
 
 
 config = Config(host='Адрес БД Canvas LMS', user='Пользователь БД Canvas LMS', passowrd='Пароль БД Canvas LMS')
 session = get_session(config)
 ```
-
```

### Comparing `python-canvas-0.3.4/setup.py` & `python-canvas-0.3.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python-canvas",
-    version="0.3.4",
+    version="0.3.5",
     author="Nauryzbek Aitbayev",
     author_email="nauryzbek.aitbayev@yu.edu.kz",
     description="Данная библиотека содержить SqlAlchemy ORM для системы Canvas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yessenovuniversity/python_canvas",
     packages=setuptools.find_packages(),
```

