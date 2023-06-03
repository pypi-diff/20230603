# Comparing `tmp/pyxirr-0.9.0.tar.gz` & `tmp/pyxirr-0.9.1.tar.gz`

## Comparing `pyxirr-0.9.0.tar` & `pyxirr-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 pyxirr-0.9.0/Cargo.toml
--rw-r--r--   0     1000     1000     1211 2021-10-05 18:13:17.000000 pyxirr-0.9.0/LICENSE
--rw-r--r--   0     1000     1000     5739 2023-03-12 21:56:42.000000 pyxirr-0.9.0/README.md
--rw-r--r--   0     1000     1000      901 2023-03-17 07:38:45.000000 pyxirr-0.9.0/pyproject.toml
--rw-r--r--   0     1000     1000     7997 2023-03-17 06:41:29.000000 pyxirr-0.9.0/src/broadcasting.rs
--rw-r--r--   0     1000     1000     8717 2023-03-16 23:12:21.000000 pyxirr-0.9.0/src/conversions.rs
--rw-r--r--   0     1000     1000      263 2023-03-12 21:56:42.000000 pyxirr-0.9.0/src/core/mod.rs
--rw-r--r--   0     1000     1000     1910 2023-03-16 23:12:21.000000 pyxirr-0.9.0/src/core/models.rs
--rw-r--r--   0     1000     1000     4026 2023-03-16 23:12:23.000000 pyxirr-0.9.0/src/core/optimize.rs
--rw-r--r--   0     1000     1000    12518 2023-03-16 23:12:21.000000 pyxirr-0.9.0/src/core/periodic.rs
--rw-r--r--   0     1000     1000    12172 2023-03-16 23:15:04.000000 pyxirr-0.9.0/src/core/scheduled/day_count.rs
--rw-r--r--   0     1000     1000      151 2023-02-20 11:31:35.000000 pyxirr-0.9.0/src/core/scheduled/mod.rs
--rw-r--r--   0     1000     1000     1967 2023-03-16 23:12:23.000000 pyxirr-0.9.0/src/core/scheduled/xirr.rs
--rw-r--r--   0     1000     1000     1257 2023-03-12 21:56:42.000000 pyxirr-0.9.0/src/core/scheduled/xnfv.rs
--rw-r--r--   0     1000     1000    13098 2023-03-16 23:25:45.000000 pyxirr-0.9.0/src/lib.rs
--rw-r--r--   0     1000     1000    13819 2023-03-12 21:56:52.000000 pyxirr-0.9.0/Cargo.lock
--rw-r--r--   0     1000     1000      374 2021-11-04 16:40:46.000000 pyxirr-0.9.0/.cargo/config
--rw-r--r--   0        0        0     6646 1970-01-01 00:00:00.000000 pyxirr-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 pyxirr-0.9.1/Cargo.toml
+-rw-r--r--   0     1001      123     1211 2023-06-03 15:24:17.000000 pyxirr-0.9.1/LICENSE
+-rw-r--r--   0     1001      123     5742 2023-06-03 15:24:17.000000 pyxirr-0.9.1/README.md
+-rw-r--r--   0     1001      123      895 2023-06-03 15:24:17.000000 pyxirr-0.9.1/pyproject.toml
+-rw-r--r--   0     1001      123     7998 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/broadcasting.rs
+-rw-r--r--   0     1001      123     8776 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/conversions.rs
+-rw-r--r--   0     1001      123      263 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/mod.rs
+-rw-r--r--   0     1001      123     1942 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/models.rs
+-rw-r--r--   0     1001      123     4026 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/optimize.rs
+-rw-r--r--   0     1001      123    14548 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/periodic.rs
+-rw-r--r--   0     1001      123    12268 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/scheduled/day_count.rs
+-rw-r--r--   0     1001      123      151 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/scheduled/mod.rs
+-rw-r--r--   0     1001      123     1963 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/scheduled/xirr.rs
+-rw-r--r--   0     1001      123     1253 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/scheduled/xnfv.rs
+-rw-r--r--   0     1001      123    14395 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/lib.rs
+-rw-r--r--   0     1001      123    13819 2023-06-03 15:24:17.000000 pyxirr-0.9.1/Cargo.lock
+-rw-r--r--   0     1001      123      374 2023-06-03 15:24:17.000000 pyxirr-0.9.1/.cargo/config
+-rw-r--r--   0        0        0     6650 1970-01-01 00:00:00.000000 pyxirr-0.9.1/PKG-INFO
```

### Comparing `pyxirr-0.9.0/Cargo.toml` & `pyxirr-0.9.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyxirr"
-version = "0.9.0"
+version = "0.9.1"
 authors = ["Anexen"]
 edition = "2021"
 description = "Rust-powered collection of financial functions for Python."
 readme = "README.md"
 homepage = "https://github.com/Anexen/pyxirr"
 license = "Unlicense"
 keywords = [
```

### Comparing `pyxirr-0.9.0/LICENSE` & `pyxirr-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.0/README.md` & `pyxirr-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 xirr(pd.DataFrame({"a": dates, "b": amounts}))
 
 # feed Series with DatetimeIndex
 xirr(pd.Series(amounts, index=pd.to_datetime(dates)))
 
 # bonus: apply xirr to a DataFrame with DatetimeIndex:
 df = pd.DataFrame(
-    index=pd.date_range("2021", "2022", freq="MS", closed="left"),
+    index=pd.date_range("2021", "2022", freq="MS", inclusive="left"),
     data={
         "one": [-100] + [20] * 11,
         "two": [-80] + [19] * 11,
     },
 )
 df.apply(xirr)  # Series(index=["one", "two"], data=[5.09623547168478, 8.780801977141174])
 ```
```

### Comparing `pyxirr-0.9.0/pyproject.toml` & `pyxirr-0.9.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: The Unlicense (Unlicense)",
 ]
 
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1,<2"]
 build-backend = "maturin"
 
 [tool.maturin]
 include = [
     "pyproject.toml",
     { path = "Cargo.toml", format = "sdist" },
     { path = "Cargo.lock", format = "sdist" },
```

### Comparing `pyxirr-0.9.0/src/broadcasting.rs` & `pyxirr-0.9.1/src/broadcasting.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 use std::{error::Error, fmt};
 
-use crate::conversions::float_or_none;
 use ndarray::{ArrayD, ArrayViewD, Axis, CowArray, IxDyn};
 use numpy::{npyffi, Element, PyArrayDyn, PY_ARRAY_API};
 use pyo3::{
     exceptions::{PyTypeError, PyValueError},
     prelude::*,
     types::{PyIterator, PyList, PySequence, PyTuple},
     AsPyPointer,
 };
 
+use crate::conversions::float_or_none;
+
 /// An error returned when the payments do not contain both negative and positive payments.
 #[derive(Debug)]
 pub struct BroadcastingError(String);
 
 impl BroadcastingError {
     pub fn new(shapes: &[&[usize]]) -> Self {
         Self(format!("{:?}", shapes))
```

### Comparing `pyxirr-0.9.0/src/conversions.rs` & `pyxirr-0.9.1/src/conversions.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 use std::str::FromStr;
 
-use crate::core::{DateLike, DayCount};
-use numpy::datetime::{units, Datetime as datetime64};
-use numpy::PyArray1;
+use numpy::{
+    datetime::{units, Datetime as datetime64},
+    PyArray1,
+};
 use pyo3::{
     exceptions::{PyTypeError, PyValueError},
     prelude::*,
     types::*,
 };
 use time::Date;
 
+use crate::core::{DateLike, DayCount};
+
 // time::Date::from_ordinal_date(1970, 1).unwrap().to_julian_day();
 static UNIX_EPOCH_JULIAN_DAY: i32 = 2440588;
 
 pub fn float_or_none(result: f64) -> Option<f64> {
     if result.is_nan() {
         None
     } else {
@@ -168,20 +171,30 @@
         .call_method1("astype", ("float64",))?
         .extract::<&PyArray1<f64>>()?
         .readonly()
         .to_vec()?)
 }
 
 fn extract_records(data: &PyAny) -> PyResult<(Vec<DateLike>, Vec<f64>)> {
-    let capacity = if let Ok(capacity) = data.len() { capacity } else { 0 };
+    let capacity = if let Ok(capacity) = data.len() {
+        capacity
+    } else {
+        0
+    };
 
-    let mut _dates: Vec<DateLike> =
-        if capacity > 0 { Vec::with_capacity(capacity) } else { Vec::new() };
-    let mut _amounts: Vec<f64> =
-        if capacity > 0 { Vec::with_capacity(capacity) } else { Vec::new() };
+    let mut _dates: Vec<DateLike> = if capacity > 0 {
+        Vec::with_capacity(capacity)
+    } else {
+        Vec::new()
+    };
+    let mut _amounts: Vec<f64> = if capacity > 0 {
+        Vec::with_capacity(capacity)
+    } else {
+        Vec::new()
+    };
 
     for obj in data.iter()? {
         let obj = obj?;
         // get_item() uses different ffi calls for different objects
         // PyTuple.get_item (ffi::PyTuple_GetItem) is faster than PyAny.get_item (ffi::PyObject_GetItem)
         let tup = if let Ok(py_tuple) = obj.downcast::<PyTuple>() {
             (py_tuple.get_item(0)?, py_tuple.get_item(1)?)
```

### Comparing `pyxirr-0.9.0/src/core/models.rs` & `pyxirr-0.9.1/src/core/models.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-use std::error::Error;
-use std::{fmt, str::FromStr};
+use std::{error::Error, fmt, str::FromStr};
+
 use time::{macros::format_description, Date};
 
 #[derive(Debug, PartialEq, Eq, Hash, PartialOrd, Ord, Clone, Copy)]
 pub struct DateLike(Date);
 
 impl From<DateLike> for Date {
     fn from(val: DateLike) -> Self {
@@ -25,15 +25,19 @@
 
 impl FromStr for DateLike {
     type Err = time::error::Parse;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         // get only date part: yyyy-mm-dd
         // this allows to parse datetime strings
-        let s = if s.len() > 10 { &s[0..10] } else { s };
+        let s = if s.len() > 10 {
+            &s[0..10]
+        } else {
+            s
+        };
 
         // try %Y-%m-%d
         if let Ok(d) = Date::parse(s, &format_description!("[year]-[month]-[day]")) {
             return Ok(d.into());
         }
 
         // try %m/%d/%Y
```

### Comparing `pyxirr-0.9.0/src/core/optimize.rs` & `pyxirr-0.9.1/src/core/optimize.rs`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.0/src/core/periodic.rs` & `pyxirr-0.9.1/src/core/periodic.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-use ndarray::{ArrayD, ArrayViewD};
-use std::iter::successors;
-use std::mem::MaybeUninit;
+use std::{iter::successors, mem::MaybeUninit};
 
-use crate::broadcast_together;
-use crate::broadcasting::BroadcastingError;
+use ndarray::{ArrayD, ArrayViewD};
 
-use super::models::{validate, InvalidPaymentsError};
-use super::optimize::{brentq, find_root, newton_raphson_with_default_deriv};
+use super::{
+    models::{validate, InvalidPaymentsError},
+    optimize::{brentq, find_root, newton_raphson_with_default_deriv},
+};
+use crate::{broadcast_together, broadcasting::BroadcastingError};
 
 // pre calculating powers for performance
 pub fn powers(base: f64, n: usize, start_from_zero: bool) -> Vec<f64> {
-    let (start, n) = if start_from_zero { (1.0, n + 1) } else { (base, n) };
+    let (start, n) = if start_from_zero {
+        (1.0, n + 1)
+    } else {
+        (base, n)
+    };
     successors(Some(start), |x| Some(x * base)).take(n).collect()
 }
 
 fn convert_pmt_at_beginning(pmt_at_beginning: bool) -> f64 {
     if pmt_at_beginning {
         1.
     } else {
@@ -152,27 +156,40 @@
             *result = MaybeUninit::new(value);
         });
 
     Ok(unsafe { result.assume_init() })
 }
 
 pub fn ipmt(rate: f64, per: f64, nper: f64, pv: f64, fv: f64, pmt_at_beginning: bool) -> f64 {
+    // let total_pmt = self::pmt(rate, nper, pv, fv, pmt_at_beginning);
+    // let result = rate * self::fv(rate, per - 1.0, total_pmt, pv, pmt_at_beginning);
+    //
+    // simplify r*(-P*(1+r)**(p-1)-(-(F+P*(1+r)**n)*r/((1+r*t)*((1+r)**n-1)))*(1+r*t)/r*((1+r)**(p-1)-1))
+
     // payments before first period don't make any sense.
     if per < 1.0 || per > nper {
         return f64::NAN;
     }
 
     // no interest if payment occurs at the beginning
     // of a period and this is the first period
     if per == 1.0 && pmt_at_beginning {
         return 0.0;
     }
 
-    let total_pmt = self::pmt(rate, nper, pv, fv, pmt_at_beginning);
-    let result = rate * self::fv(rate, per - 1.0, total_pmt, pv, pmt_at_beginning);
+    // no interest if rate == 0
+    if rate == 0.0 {
+        return 0.0;
+    }
+
+    let f1 = (rate + 1.0).powf(per);
+    let f2 = (rate + 1.0).powf(nper);
+
+    let result = (rate * (pv + fv) * f1 - rate * (rate + 1.0) * (fv + pv * f2))
+        / ((rate + 1.0) * (f2 - 1.0));
 
     if pmt_at_beginning {
         // if paying at the beginning we need to discount by one period.
         result / (1.0 + rate)
     } else {
         result
     }
@@ -185,50 +202,96 @@
     pv: &ArrayViewD<f64>,
     fv: &ArrayViewD<f64>,
     pmt_at_beginning: &ArrayViewD<bool>,
 ) -> Result<ArrayD<f64>, BroadcastingError> {
     let (rate, per, nper, pv, fv, pmt_at_beginning) =
         broadcast_together!(rate, per, nper, pv, fv, pmt_at_beginning)?;
 
-    let total_pmt = self::pmt_vec(&rate, &nper, &pv, &fv, &pmt_at_beginning)?;
-    let per_prev = &per - 1.0;
-    let mut result = &rate
-        * self::fv_vec(&rate, &per_prev.view(), &total_pmt.view(), &pv, &pmt_at_beginning.view())?;
-
-    ndarray::Zip::from(&mut result).and(rate).and(per).and(nper).and(pmt_at_beginning).for_each(
-        |r, rate, per, nper, &pmt_at_beginning| {
-            if per < &1.0 || per > nper {
-                *r = f64::NAN
-            } else if per == &1.0 && pmt_at_beginning {
-                *r = 0.0
-            } else if pmt_at_beginning {
-                *r /= 1.0 + rate
-            }
-        },
-    );
+    let f1 = ndarray::Zip::from(&rate).and(&per).map_collect(|rate, &per| (rate + 1.).powf(per));
+    let f2 =
+        ndarray::Zip::from(&rate).and(&nper).map_collect(|rate, &nper| (rate + 1.0).powf(nper));
+
+    let mut result = (&rate * (&pv + &fv) * &f1 - &rate * (&rate + 1.0) * (&fv + &pv * &f2))
+        / ((&rate + 1.0) * (&f2 - 1.0));
+
+    for (ref idx, r) in result.indexed_iter_mut() {
+        if rate[idx] == 0.0 {
+            *r = 0.0;
+        } else if per[idx] < 1.0 || per[idx] > nper[idx] {
+            *r = f64::NAN;
+        } else if per[idx] == 1.0 && pmt_at_beginning[idx] {
+            *r = 0.0;
+        } else if pmt_at_beginning[idx] {
+            *r /= rate[idx] + 1.0;
+        }
+    }
 
     Ok(result)
 }
 
 pub fn ppmt(rate: f64, per: f64, nper: f64, pv: f64, fv: f64, pmt_at_beginning: bool) -> f64 {
-    self::pmt(rate, nper, pv, fv, pmt_at_beginning)
-        - self::ipmt(rate, per, nper, pv, fv, pmt_at_beginning)
+    // assuming type = 1 if pmt_at_beginning else 0
+    // assuming P=pv;F=fv;r=rate;n=nper;p=per;t=type, type in {1;0}
+    // ppmt = fv(r,p-1,pmt(r,n,P,F,t),P,t) - fv(r,p,pmt(r,n,P,F,t),P,t)
+    // after substitution:
+    // simplify (-P*(1+r)^(p-1)-(-(F+P*(1+r)^n)*r/((1+r)^n-1)/(1+r*t))*(1+r*t)/r*((1+r)^(p-1)-1)) - (-P*(1+r)^p-(-(F+P*(1+r)^n)*r/((1+r)^n-1)/(1+r*t))*(1+r*t)/r*((1+r)^p-1))
+    // shorter formula: -r*(F+P)*(r+1)^(per-1)/((r+1)^n - 1)
+    // type correction: result /= r + 1 if type = 1
+    // denominator => 1/((r+1)^p-1) => 1/(((r+1)^p-1)*(r+1)) =>
+    // => 1/((r+1)^(p+1) - (r+1)) => 1/((r+1)^(p+t) -r*t + 1)
+    //
+    // if rate == 0:
+    // simplify (-P-(-(F+P)/n) *(p-1) - (-P-(-(F+P)/n)*p))
+    // shorter: -(F + P) / n;
+
+    if per < 1.0 || per > nper {
+        return f64::NAN;
+    }
+
+    if rate == 0.0 {
+        return -(fv + pv) / nper;
+    }
+
+    let when = convert_pmt_at_beginning(pmt_at_beginning);
+    -rate * (fv + pv) * (rate + 1.).powf(per - 1.)
+        / ((rate + 1.).powf(nper + when) - rate * when - 1.)
 }
 
 pub fn ppmt_vec(
     rate: &ArrayViewD<f64>,
     per: &ArrayViewD<f64>,
     nper: &ArrayViewD<f64>,
     pv: &ArrayViewD<f64>,
     fv: &ArrayViewD<f64>,
     pmt_at_beginning: &ArrayViewD<bool>,
 ) -> Result<ArrayD<f64>, BroadcastingError> {
-    let pmt = self::pmt_vec(rate, nper, pv, fv, pmt_at_beginning)?;
-    let ipmt = self::ipmt_vec(rate, per, nper, pv, fv, pmt_at_beginning)?;
-    Ok(pmt - ipmt)
+    let (rate, per, nper, pv, fv, pmt_at_beginning) =
+        broadcast_together!(rate, per, nper, pv, fv, pmt_at_beginning)?;
+
+    let when = pmt_at_beginning.mapv(convert_pmt_at_beginning);
+
+    let f1 =
+        ndarray::Zip::from(&rate).and(&per).map_collect(|rate, per| (rate + 1.).powf(per - 1.0));
+
+    let f2 = ndarray::Zip::from(&rate)
+        .and(&nper)
+        .and(&when)
+        .map_collect(|rate, nper, when| (rate + 1.0).powf(nper + when));
+
+    let mut result = -&rate * (&fv + &pv) * &f1 / (&f2 - &rate * &when - 1.0);
+
+    for (ref idx, r) in result.indexed_iter_mut() {
+        if rate[idx] == 0.0 {
+            *r = -(fv[idx] + pv[idx]) / nper[idx];
+        } else if per[idx] < 1.0 || per[idx] > nper[idx] {
+            *r = f64::NAN;
+        }
+    }
+
+    Ok(result)
 }
 
 pub fn nper(rate: f64, pmt: f64, pv: f64, fv: f64, pmt_at_beginning: bool) -> f64 {
     if rate == 0.0 {
         return -(fv + pv) / pmt;
     }
```

### Comparing `pyxirr-0.9.0/src/core/scheduled/day_count.rs` & `pyxirr-0.9.1/src/core/scheduled/day_count.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use std::{cmp::min, fmt, str::FromStr};
+
 use time::{
     util::{days_in_year_month, is_leap_year},
     Date, Month,
 };
 
 #[pyo3::pyclass]
 #[pyo3(frozen)]
@@ -21,16 +22,14 @@
     THIRTY_E_PLUS_360,
     THIRTY_E_360_ISDA,
     THIRTY_U_360,
     NL_365,
     NL_360,
 }
 
-
-
 impl fmt::Display for DayCount {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         use DayCount::*;
         let repr = match self {
             ACT_ACT_ISDA => "Actual/Actual ISDA",
             ACT_365F => "Actual/365F",
             ACT_365_25 => "Actual/365.25",
@@ -162,42 +161,58 @@
     }
 
     leap_days
 }
 
 fn days_between_30_360_isda(d1: &Date, d2: &Date) -> i32 {
     let d1_day = min(d1.day(), 30);
-    let d2_day = if d1_day >= 30 { min(d2.day(), 30) } else { d2.day() };
+    let d2_day = if d1_day >= 30 {
+        min(d2.day(), 30)
+    } else {
+        d2.day()
+    };
     days_between_30_360(d1, d2, d1_day, d2_day)
 }
 
 fn days_between_30_e_360(d1: &Date, d2: &Date) -> i32 {
     let d1_day = min(d1.day(), 30);
     let d2_day = min(d2.day(), 30);
     days_between_30_360(d1, d2, d1_day, d2_day)
 }
 
 fn days_between_30_e_360_isda(d1: &Date, d2: &Date) -> i32 {
-    let d1_day = if is_last_day_of_feb(d1) { 30 } else { min(d1.day(), 30) };
-    let d2_day = if is_last_day_of_feb(d2) { 30 } else { min(d2.day(), 30) };
+    let d1_day = if is_last_day_of_feb(d1) {
+        30
+    } else {
+        min(d1.day(), 30)
+    };
+    let d2_day = if is_last_day_of_feb(d2) {
+        30
+    } else {
+        min(d2.day(), 30)
+    };
     days_between_30_360(d1, d2, d1_day, d2_day)
 }
 
 fn days_between_30_e_plus_360(d1: &Date, d2: &Date) -> i32 {
     let d1_day = min(d1.day(), 30);
     if d2.day() == 31 {
         let d2 = d2.next_day().unwrap();
         days_between_30_360(d1, &d2, d1_day, d2.day())
     } else {
         days_between_30_360(d1, d2, d1_day, d2.day())
     }
 }
 
 fn days_between_30_u_360(d1: &Date, d2: &Date) -> i32 {
-    let d1_day = if is_last_day_of_feb(d1) { 30 } else { min(d1.day(), 30) };
+    let d1_day = if is_last_day_of_feb(d1) {
+        30
+    } else {
+        min(d1.day(), 30)
+    };
     let d2_day = if is_last_day_of_feb(d1) && is_last_day_of_feb(d2) {
         30
     } else if d1_day >= 30 {
         min(d2.day(), 30)
     } else {
         d2.day()
     };
@@ -217,17 +232,18 @@
 
 pub fn is_last_day_of_feb(date: &Date) -> bool {
     date.month() == Month::February && is_last_day_of_month(date)
 }
 
 #[cfg(test)]
 mod tests {
+    use rstest::rstest;
+
     use super::*;
     use crate::core::DateLike;
-    use rstest::rstest;
 
     // test cases from http://www.deltaquants.com/day-count-conventions
     #[rstest]
     #[case("Act/Act", 4./365. + 58./366.)]
     #[case("Act/365F", 62./365.)]
     #[case("Act/360", 62./360.)]
     // #[case("Act/365A", 62./365.)]
```

### Comparing `pyxirr-0.9.0/src/core/scheduled/xirr.rs` & `pyxirr-0.9.1/src/core/scheduled/xirr.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 use super::{year_fraction, DayCount};
-use crate::core::models::{validate, DateLike, InvalidPaymentsError};
-use crate::core::optimize::find_root;
+use crate::core::{
+    models::{validate, DateLike, InvalidPaymentsError},
+    optimize::find_root,
+};
 
 pub fn xirr(
     dates: &[DateLike],
     amounts: &[f64],
     guess: Option<f64>,
     day_count: Option<DayCount>,
 ) -> Result<f64, InvalidPaymentsError> {
```

### Comparing `pyxirr-0.9.0/src/core/scheduled/xnfv.rs` & `pyxirr-0.9.1/src/core/scheduled/xnfv.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 use super::{year_fraction, DayCount};
-use crate::core::models::{validate, DateLike, InvalidPaymentsError};
-use crate::core::periodic::fv;
+use crate::core::{
+    models::{validate, DateLike, InvalidPaymentsError},
+    periodic::fv,
+};
 
 // http://westclintech.com/SQL-Server-Financial-Functions/SQL-Server-XFV-function
 pub fn xfv(
     start_date: &DateLike,
     cash_flow_date: &DateLike,
     end_date: &DateLike,
     cash_flow_rate: f64,
```

### Comparing `pyxirr-0.9.0/src/lib.rs` & `pyxirr-0.9.1/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use broadcasting::Arg;
 use conversions::{fallible_float_or_none, float_or_none, PyDayCount};
-use pyo3::prelude::*;
-use pyo3::{create_exception, exceptions, wrap_pyfunction};
+use pyo3::{create_exception, exceptions, prelude::*, wrap_pyfunction};
 
 mod broadcasting;
 mod conversions;
 mod core;
 
 create_exception!(pyxirr, InvalidPaymentsError, exceptions::PyException);
 create_exception!(pyxirr, BroadcastingError, exceptions::PyException);
@@ -343,14 +342,56 @@
         (nper, pmt, pv, fv, pmt_at_beginning),
         core::rate(nper, pmt, pv, fv, pmt_at_beginning, guess),
         core::rate_vec(&nper, &pmt, &pv, &fv, &pmt_at_beginning, guess)
     )
 }
 
 #[pyfunction]
+#[pyo3(signature = (rate, nper, pv, start_period, end_period, *, pmt_at_beginning=false))]
+fn cumprinc(
+    py: Python,
+    rate: f64,
+    nper: f64,
+    pv: f64,
+    start_period: f64,
+    end_period: f64,
+    pmt_at_beginning: bool,
+) -> Option<f64> {
+    // https://wiki.documentfoundation.org/Documentation/Calc_Functions/CUMPRINC
+    let result = py.allow_threads(move || {
+        (start_period.trunc() as u64..=end_period.trunc() as u64)
+            .map(|per| core::ppmt(rate, per as f64, nper, pv, 0.0, pmt_at_beginning))
+            .sum()
+    });
+
+    float_or_none(result)
+}
+
+#[pyfunction]
+#[pyo3(signature = (rate, nper, pv, start_period, end_period, *, pmt_at_beginning=false))]
+fn cumipmt(
+    py: Python,
+    rate: f64,
+    nper: f64,
+    pv: f64,
+    start_period: f64,
+    end_period: f64,
+    pmt_at_beginning: bool,
+) -> Option<f64> {
+    // https://wiki.documentfoundation.org/Documentation/Calc_Functions/CUMIPMT
+    let result = py.allow_threads(move || {
+        (start_period.trunc() as u64..=end_period.trunc() as u64)
+            .map(|per| core::ipmt(rate, per as f64, nper, pv, 0.0, pmt_at_beginning))
+            .sum()
+    });
+
+    float_or_none(result)
+}
+
+#[pyfunction]
 fn year_fraction(d1: core::DateLike, d2: core::DateLike, day_count: PyDayCount) -> PyResult<f64> {
     Ok(core::year_fraction(&d1, &d2, day_count.try_into()?))
 }
 
 #[pyfunction]
 fn days_between(d1: core::DateLike, d2: core::DateLike, day_count: PyDayCount) -> PyResult<i32> {
     Ok(core::days_between(&d1, &d2, day_count.try_into()?))
@@ -360,15 +401,17 @@
 pub fn pyxirr(py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<core::DayCount>()?;
     m.add_function(wrap_pyfunction!(year_fraction, m)?)?;
     m.add_function(wrap_pyfunction!(days_between, m)?)?;
 
     m.add_function(wrap_pyfunction!(pmt, m)?)?;
     m.add_function(wrap_pyfunction!(ipmt, m)?)?;
+    m.add_function(wrap_pyfunction!(cumipmt, m)?)?;
     m.add_function(wrap_pyfunction!(ppmt, m)?)?;
+    m.add_function(wrap_pyfunction!(cumprinc, m)?)?;
     m.add_function(wrap_pyfunction!(nper, m)?)?;
     m.add_function(wrap_pyfunction!(rate, m)?)?;
     m.add_function(wrap_pyfunction!(fv, m)?)?;
     m.add_function(wrap_pyfunction!(nfv, m)?)?;
     m.add_function(wrap_pyfunction!(xfv, m)?)?;
     m.add_function(wrap_pyfunction!(xnfv, m)?)?;
     m.add_function(wrap_pyfunction!(pv, m)?)?;
```

### Comparing `pyxirr-0.9.0/Cargo.lock` & `pyxirr-0.9.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyxirr"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "ndarray",
  "numpy",
  "pyo3",
  "rstest",
  "time",
 ]
```

### Comparing `pyxirr-0.9.0/PKG-INFO` & `pyxirr-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxirr
-Version: 0.9.0
+Version: 0.9.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 License-File: LICENSE
 Summary: Rust-powered collection of financial functions for Python.
 Keywords: python,fast,financial,xirr,cashflow,day count convention
 Home-Page: https://github.com/Anexen/pyxirr
 Author: Anexen
 License: Unlicense
-Requires-Python: >=3.7,<3.12
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 [![rust-lang.org](https://img.shields.io/badge/Made%20with-Rust-red)](https://www.rust-lang.org/)
 [![License](https://img.shields.io/github/license/Anexen/pyxirr.svg)](https://github.com/Anexen/pyxirr/blob/master/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/pyxirr.svg)](https://pypi.org/project/pyxirr/)
 [![versions](https://img.shields.io/pypi/pyversions/pyxirr.svg)](https://pypi.org/project/pyxirr/)
 
@@ -95,15 +95,15 @@
 xirr(pd.DataFrame({"a": dates, "b": amounts}))
 
 # feed Series with DatetimeIndex
 xirr(pd.Series(amounts, index=pd.to_datetime(dates)))
 
 # bonus: apply xirr to a DataFrame with DatetimeIndex:
 df = pd.DataFrame(
-    index=pd.date_range("2021", "2022", freq="MS", closed="left"),
+    index=pd.date_range("2021", "2022", freq="MS", inclusive="left"),
     data={
         "one": [-100] + [20] * 11,
         "two": [-80] + [19] * 11,
     },
 )
 df.apply(xirr)  # Series(index=["one", "two"], data=[5.09623547168478, 8.780801977141174])
 ```
```

