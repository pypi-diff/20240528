# Comparing `tmp/sigcalc-0.1.0.tar.gz` & `tmp/sigcalc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigcalc-0.1.0.tar", max compression
+gzip compressed data, was "sigcalc-0.1.1.tar", max compression
```

## Comparing `sigcalc-0.1.0.tar` & `sigcalc-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0    35401 2023-04-14 02:29:28.249028 sigcalc-0.1.0/LICENSE.rst
--rw-r--r--   0        0        0     8755 2024-01-27 01:18:12.396924 sigcalc-0.1.0/README.rst
--rw-r--r--   0        0        0     2606 2024-05-26 12:37:22.205007 sigcalc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      511 2024-01-19 20:33:31.539540 sigcalc-0.1.0/sigcalc/__init__.py
--rw-r--r--   0        0        0     1108 2024-01-21 20:58:17.408544 sigcalc-0.1.0/sigcalc/constants.py
--rw-r--r--   0        0        0    54495 2024-05-26 13:10:30.112546 sigcalc-0.1.0/sigcalc/quantity.py
--rw-r--r--   0        0        0      904 2024-01-23 01:59:15.001015 sigcalc-0.1.0/sigcalc/test_constants.py
--rw-r--r--   0        0        0    29982 2024-05-26 13:10:30.112546 sigcalc-0.1.0/sigcalc/test_quantity.py
--rw-r--r--   0        0        0    34784 2024-05-26 13:10:30.116546 sigcalc-0.1.0/sigcalc/test_quantity_hypothesis.py
--rw-r--r--   0        0        0     9770 1970-01-01 00:00:00.000000 sigcalc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35401 2024-05-26 23:38:44.160467 sigcalc-0.1.1/LICENSE.rst
+-rw-r--r--   0        0        0     6076 2024-05-26 23:38:44.160467 sigcalc-0.1.1/README.rst
+-rw-r--r--   0        0        0     2596 2024-05-26 23:38:44.164467 sigcalc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      409 2024-05-26 23:38:44.164467 sigcalc-0.1.1/sigcalc/__init__.py
+-rw-r--r--   0        0        0     7953 2024-05-26 23:38:44.164467 sigcalc-0.1.1/sigcalc/quantity.py
+-rw-r--r--   0        0        0    23249 2024-05-26 23:38:44.164467 sigcalc-0.1.1/sigcalc/test_quantity.py
+-rw-r--r--   0        0        0     5121 2024-05-26 23:38:44.164467 sigcalc-0.1.1/sigcalc/test_quantity_hypothesis.py
+-rw-r--r--   0        0        0     7060 1970-01-01 00:00:00.000000 sigcalc-0.1.1/PKG-INFO
```

### Comparing `sigcalc-0.1.0/LICENSE.rst` & `sigcalc-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sigcalc-0.1.0/README.rst` & `sigcalc-0.1.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. *****************************************************************************
 ..
 .. sigcalc, significant figures calculations
 ..
-.. Copyright 2023-2024 Jeremy A Gray <gray@flyquackswim.com>.
+.. Copyright 2023 Jeremy A Gray <gray@flyquackswim.com>.
 ..
 .. All rights reserved.
 ..
 .. SPDX-License-Identifier: GPL-3.0-or-later
 ..
 .. *****************************************************************************
 
@@ -32,47 +32,37 @@
 
   pip install sigcalc
 
 or with poetry::
 
   poetry add sigcalc
 
-``sigcalc`` depends on the internal ``decimal``
-`module <https://docs.python.org/3/library/decimal.html>`_
-for arithmetic and `mpmath <https://mpmath.org/>`_ for transcendental
-and other functions.
+``sigcalc`` depends on the internal ``decimal`` module for arithmetic
+and ``mpmath`` (https://mpmath.org/) for transcendental and other
+functions.
 
 Usage
 -----
 
 Import the ``Quantity`` class:
 
 >>> from sigcalc import Quantity
->>> from decimal import getcontext
->>> getcontext().prec = 28
 
 Create ``Quantity`` objects as necessary:
 
 >>> a = Quantity("3.14", "3")
 >>> b = Quantity("2.72", "3")
 
 The precision of the underlying ``decimal`` context should adjust
 automatically to contain the number of digits specified or the number
 of significant figures, within the limits of the ``decimal`` module.
 
 Arithmetic for ``Quantity`` objects is implemented on the usual magic
 methods:
 
->>> from sigcalc import Quantity
->>> from decimal import getcontext
->>> from decimal import ROUND_HALF_EVEN
->>> getcontext().prec = 28
->>> getcontext().rounding = ROUND_HALF_EVEN
->>> a = Quantity("3.14", "3")
->>> b = Quantity("2.72", "3")
 >>> a + b
 Quantity("5.86", "3")
 >>> a - b
 Quantity("0.42", "2")
 >>> a * b
 Quantity("8.5408", "3")
 >>> a / b
@@ -82,15 +72,15 @@
 >>> -a
 Quantity("-3.14", "3")
 >>> +a
 Quantity("3.14", "3")
 
 Beware that rounding is not performed during calculations and that
 reported significant figures for calculated values are for the
-unrounded value.  For example, a calculation that resulted in a result
+unrounded value.  For example, a claculation that resulted in a result
 of ``Quantity("99.9", "3")`` could round to ``Quantity("100.0",
 "4")``, depending on the current rounding mode.
 
 Note that ``__floordiv__`` is not implemented as it is not useful for
 significant figures calculations.
 
 >>> a // b
@@ -178,79 +168,31 @@
 >>> getcontext().rounding = ROUND_HALF_UP
 >>> format(a, ".2e")
 '3.15e+0'
 >>> getcontext().rounding = ROUND_HALF_EVEN
 >>> format(b, ".2e")
 '3.14e+0'
 
-Power and Square Root Functions
-...............................
-
-The power and square root (``__pow__()`` and ``sqrt()``) functions and
-are implemented as wrappers around the appropriate functions from
-``decimal.Decimal``, calculating results based on the ``value`` of a
-``Quantity`` combined with the correct significant figures, following
-the "significance in, significance out" rule for both functions.
-
-Exponential and Logarithmic Functions
-.....................................
-
-The exponential and logarithmic (``exp()``, ``exp10()``, ``ln()``, and
-``log10()``) functions are implemented as wrappers around the
-corresponding functions from ``decimal`` to calculate the ``value`` of
-a ``Quantity`` combined with the correct significant figures.
-Abscissa digits are treated as placeholders so a logarithm will
-increase significance by the number of significant abscissa digits;
-exponentials will decrease the significance by the number of
-significant abscissa digits.  Consequently, if a ``Quantity`` has
-significant figures less than or equal to the number of abscissa
-digits, a ``RuntimeWarning`` will be raised and a ``Quantity`` with
-zero significant figures will be returned.  See the references for
-more information.
-
-Transcendental Functions
-........................
-
-The transcendental functions and their inverses are implemented as
-wrappers around the appropriate functions from ``mpmath``, calculating
-results based on the ``value`` of a ``Quantity`` combined with the
-correct significant figures, following the "significance in,
-significance out" rule.
-
-Hyperbolic Functions
-....................
-
-The hyperbolic functions and their inverses are implemented as
-wrappers around the appropriate functions from ``mpmath``, calculating
-results based on the ``value`` of a ``Quantity`` combined with the
-correct significant figures, following the "significance in,
-significance out" rule.
+The transcendental and exponential functions will be implemented as
+wrappers around the appropriate functions from ``decimal`` and
+``mpmath``, calculating results based on the ``value`` of a
+``Quantity`` with the correct significant figures.
 
 References
 ----------
 
 ``sigcalc`` implements significant figures calculations as commonly
 described in high school and undergraduate chemistry and physics
 textbooks, examples of which may be found at:
 
 1. `Significant Figures at Wikipedia <https://en.wikipedia.org/wiki/Significant_figures>`_
 2. `Significance Arithmetic at Wikipedia <https://en.wikipedia.org/wiki/Significance_arithmetic>`_
 3. Myers, R.T.; Tocci, S.; Oldham, K.B., Holt Chemistry, Holt, Rinehart and Winston: 2006.
-4. `"How many significant figures in 0.0" <https://math.stackexchange.com/questions/2149316/>`_
-
-Thanks to the developers of Python's ``decimal``
-`module <https://docs.python.org/3/library/decimal.html>`_,
-the `mpmath <https://mpmath.org/>`_ library, and the
-`hypothesis <https://hypothesis.readthedocs.io/>`_ testing library,
-without which, this would be a much smaller and less functional
-library.
-
-Thanks also to LibreTexts Mathematics for their reference on `hyperbolic functions <https://math.libretexts.org/Courses/Monroe_Community_College/MTH_211_Calculus_II/Chapter_6%3A_Applications_of_Integration/6.9%3A_Calculus_of_the_Hyperbolic_Functions>`_.
 
-Remember, calculating with significant figures is not a substitute for
+Calculating with significant figures is not a substitute for
 repetition of measurements and proper statistical analysis.
 
 Copyright and License
 ---------------------
 
 SPDX-License-Identifier: `GPL-3.0-or-later <https://spdx.org/licenses/GPL-3.0-or-later.html>`_
```

### Comparing `sigcalc-0.1.0/pyproject.toml` & `sigcalc-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 [tool.poetry]
 
 authors = [
   "Jeremy A Gray <gray@flyquackswim.com>",
 ]
 description = "significant figures calculations"
 name = "sigcalc"
-version = "0.1.0"
+version = "0.1.1"
 license = "GPL-3.0-or-later"
 maintainers = [
   "Jeremy A Gray <gray@flyquackswim.com>",
 ]
 readme = "README.rst"
 homepage = "https://github.com/jeremyagray/sigcalc"
 repository = "https://github.com/jeremyagray/sigcalc"
@@ -123,28 +123,28 @@
 packages = [
   { include = "sigcalc" },
 ]
 
 [tool.poetry.dependencies]
 
 python = ">=3.10.1,<4.0"
-mpmath = ">=1,<2"
 
 [tool.poetry.group.dev.dependencies]
 
-Sphinx = ">=7"
-black = ">=24"
-flake8 = ">=7"
-flake8-docstrings = ">=1"
-hypothesis = ">=6"
-isort = ">=5"
-pccc = ">=0"
-pre-commit = ">=3"
-pytest = ">=8"
-pytest-cov = ">=5"
-tox = ">=4"
+Sphinx = "^7"
+black = "^23"
+factory-boy = "^3"
+flake8 = "^6"
+flake8-docstrings = "^1"
+hypothesis = "^6"
+isort = "^5"
+pccc = "^0"
+pre-commit = "^3"
+pytest = "^7"
+pytest-cov = "^4"
+tox = "^4"
 
 [tool.poetry.urls]
 
 "Issues" = "https://github.com/jeremyagray/sigcalc/issues"
 "Documentation" = "https://sigcalc.readthedocs.io/"
 "Repository" = "https://github.com/jeremyagray/sigcalc"
```

### Comparing `sigcalc-0.1.0/sigcalc/test_quantity.py` & `sigcalc-0.1.1/sigcalc/test_quantity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ******************************************************************************
 #
 # sigcalc, significant figures calculations
 #
-# Copyright 2023-2024 Jeremy A Gray <gray@flyquackswim.com>.
+# Copyright 2023 Jeremy A Gray <gray@flyquackswim.com>.
 #
 # All rights reserved.
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # ******************************************************************************
 
@@ -23,108 +23,29 @@
 from decimal import Decimal
 from decimal import getcontext
 from decimal import localcontext
 
 import pytest
 
 from sigcalc import Quantity
-from sigcalc import _most_significant_place
 
 # Default values from ``decimal``.
 default_rounding = ROUND_HALF_EVEN
 default_prec = 28
 
-# Reusable decimal constants.
-NegThousand = Decimal("-1000")
-NegTen = Decimal("-10")
-NegOne = Decimal("-1")
-Zero = Decimal("0")
-One = Decimal("1")
-Two = Decimal("2")
-Ten = Decimal("10")
-Hundred = Decimal("100")
-Thousand = Decimal("1000")
-
-
-# Helper function tests.
-def test__most_significant_place():
-    """Should return the power of the most significant place."""
-    # Set default precision and rounding.
-    getcontext().prec = default_prec
-    getcontext().rounding = default_rounding
-
-    assert _most_significant_place(Zero) == Zero
-    assert _most_significant_place(Decimal("0.5")) == NegOne
-    assert _most_significant_place(One) == Zero
-    assert _most_significant_place(Ten) == One
-
-    assert _most_significant_place(Decimal("31415926540")) == Ten
-    assert _most_significant_place(Decimal("3141592654")) == Decimal("9")
-    assert _most_significant_place(Decimal("314159265.4")) == Decimal("8")
-    assert _most_significant_place(Decimal("31415926.54")) == Decimal("7")
-    assert _most_significant_place(Decimal("3141592.654")) == Decimal("6")
-    assert _most_significant_place(Decimal("314159.2654")) == Decimal("5")
-    assert _most_significant_place(Decimal("31415.92654")) == Decimal("4")
-    assert _most_significant_place(Decimal("3141.592654")) == Decimal("3")
-    assert _most_significant_place(Decimal("314.1592654")) == Two
-    assert _most_significant_place(Decimal("31.41592654")) == One
-    assert _most_significant_place(Decimal("3.141592654")) == Zero
-    assert _most_significant_place(Decimal("0.3141592654")) == NegOne
-    assert _most_significant_place(Decimal("0.03141592654")) == Decimal("-2")
-    assert _most_significant_place(Decimal("0.003141592654")) == Decimal("-3")
-    assert _most_significant_place(Decimal("0.0003141592654")) == Decimal("-4")
-    assert _most_significant_place(Decimal("0.00003141592654")) == Decimal("-5")
-    assert _most_significant_place(Decimal("0.000003141592654")) == Decimal("-6")
-    assert _most_significant_place(Decimal("0.0000003141592654")) == Decimal("-7")
-    assert _most_significant_place(Decimal("0.00000003141592654")) == Decimal("-8")
-    assert _most_significant_place(Decimal("0.000000003141592654")) == Decimal("-9")
-    assert _most_significant_place(Decimal("0.0000000003141592654")) == Decimal("-10")
-    assert _most_significant_place(Decimal("-31415926540")) == Decimal("10")
-    assert _most_significant_place(Decimal("-3141592654")) == Decimal("9")
-    assert _most_significant_place(Decimal("-314159265.4")) == Decimal("8")
-    assert _most_significant_place(Decimal("-31415926.54")) == Decimal("7")
-    assert _most_significant_place(Decimal("-3141592.654")) == Decimal("6")
-    assert _most_significant_place(Decimal("-314159.2654")) == Decimal("5")
-    assert _most_significant_place(Decimal("-31415.92654")) == Decimal("4")
-    assert _most_significant_place(Decimal("-3141.592654")) == Decimal("3")
-    assert _most_significant_place(Decimal("-314.1592654")) == Two
-    assert _most_significant_place(Decimal("-31.41592654")) == One
-    assert _most_significant_place(Decimal("-3.141592654")) == Zero
-    assert _most_significant_place(Decimal("-0.3141592654")) == NegOne
-    assert _most_significant_place(Decimal("-0.03141592654")) == Decimal("-2")
-    assert _most_significant_place(Decimal("-0.003141592654")) == Decimal("-3")
-    assert _most_significant_place(Decimal("-0.0003141592654")) == Decimal("-4")
-    assert _most_significant_place(Decimal("-0.00003141592654")) == Decimal("-5")
-    assert _most_significant_place(Decimal("-0.000003141592654")) == Decimal("-6")
-    assert _most_significant_place(Decimal("-0.0000003141592654")) == Decimal("-7")
-    assert _most_significant_place(Decimal("-0.00000003141592654")) == Decimal("-8")
-    assert _most_significant_place(Decimal("-0.000000003141592654")) == Decimal("-9")
-    assert _most_significant_place(Decimal("-0.0000000003141592654")) == Decimal("-10")
-
-
-def test__most_significant_place_zero():
-    """Should return zero as the most significant place for zero."""
-    # Set default precision and rounding.
-    getcontext().prec = default_prec
-    getcontext().rounding = default_rounding
-
-    assert _most_significant_place(Zero) == Zero
-    assert _most_significant_place(Decimal("0.000")) == Zero
-
 
 # Output operations tests.
 def test___repr__():
     """Should reproduce a ``Quantity`` object."""
     # Set default precision and rounding.
     getcontext().prec = default_prec
     getcontext().rounding = default_rounding
 
     q = Quantity("3.14", "3")
     assert repr(q) == f'Quantity("{str(q.value)}", "{str(q.figures)}")'
-
     q = Quantity("3.14", "3", constant=True)
     assert repr(q) == f'Quantity("{str(q.value)}", "{str(q.figures)}", constant=True)'
 
 
 def test___format__():
     """Should format a ``Quantity`` object."""
     # Set default precision and rounding.
@@ -152,15 +73,15 @@
     q = Quantity("0.0314", "3")
     assert f"{q:.2e}" == "3.14e-2"
     q = Quantity("0.0314", "4")
     assert f"{q:.3e}" == "3.140e-2"
 
 
 @pytest.mark.parametrize(
-    "mode, value, figures, expected",
+    "mode, value, figures, output",
     [
         (ROUND_05UP, "31.4", "1", "3E+1"),
         (ROUND_CEILING, "31.4", "1", "4E+1"),
         (ROUND_DOWN, "31.4", "1", "3E+1"),
         (ROUND_FLOOR, "31.4", "1", "3E+1"),
         (ROUND_HALF_DOWN, "31.4", "1", "3E+1"),
         (ROUND_HALF_EVEN, "31.4", "1", "3E+1"),
@@ -232,21 +153,20 @@
         (ROUND_UP, "-3.135", "3", "-3.14"),
         (ROUND_05UP, "3.101", "3", "3.11"),
         (ROUND_05UP, "3.151", "3", "3.16"),
         (ROUND_05UP, "-3.101", "3", "-3.11"),
         (ROUND_05UP, "-3.151", "3", "-3.16"),
     ],
 )
-def test___str__(mode, value, figures, expected):
+def test___str__(mode, value, figures, output):
     """Should stringify a ``Quantity`` object."""
     # Test in a local context since the rounding modes are changing.
     with localcontext() as ctx:
         ctx.rounding = mode
-        actual = str(Quantity(value, figures))
-        assert actual == expected
+        assert str(Quantity(value, figures)) == output
 
 
 def test__round_constants():
     """Constants should not round."""
     # Set default precision and rounding.
     getcontext().prec = default_prec
     getcontext().rounding = default_rounding
@@ -263,638 +183,370 @@
 
     q = Quantity("3.14", "2", constant=True)
     assert q.round() == q
 
 
 def test_round():
     """Should round a ``Quantity`` object."""
-    actual = Quantity("3.14", "2").round()
-    expected = Quantity("3.1", "2")
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
 
-    assert actual == expected
+    q = Quantity("3.14", "2")
+    assert q.round() == Quantity("3.1", "2")
 
 
 # Unary operations tests.
-@pytest.mark.parametrize(
-    "quantity, expected",
-    [
-        (
-            Quantity("3.14", "3"),
-            Quantity("3.14", "3"),
-        ),
-        (
-            Quantity("-3.14", "3"),
-            Quantity("3.14", "3"),
-        ),
-        (
-            Quantity("+3.14", "3"),
-            Quantity("3.14", "3"),
-        ),
-        (
-            Quantity("0", "3"),
-            Quantity("0", "3"),
-        ),
-        (
-            Quantity("-0", "3"),
-            Quantity("0", "3"),
-        ),
-        (
-            Quantity("+0", "3"),
-            Quantity("0", "3"),
-        ),
-        # Constants.
-        (
-            Quantity("3.14", "3", constant=True),
-            Quantity("3.14", "3", constant=True),
-        ),
-    ],
-)
-def test_abs(quantity, expected):
+def test_abs():
     """Should return the absolute value of a ``Quantity`` object."""
-    actual = abs(quantity)
-    assert actual == expected
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
 
+    assert abs(Quantity("3.14", "3")) == Quantity("3.14", "3")
+    assert abs(Quantity("-3.14", "3")) == Quantity("3.14", "3")
+    assert abs(Quantity("+3.14", "3")) == Quantity("3.14", "3")
+    assert abs(Quantity("0", "3")) == Quantity("0", "3")
+    assert abs(Quantity("-0", "3")) == Quantity("0", "3")
+    assert abs(Quantity("+0", "3")) == Quantity("0", "3")
+    # Constants.
+    assert abs(Quantity("3.14", "3", constant=True)) == Quantity(
+        "3.14", "3", constant=True
+    )
 
-@pytest.mark.parametrize(
-    "quantity, expected",
-    [
-        (
-            Quantity("3.14", "3"),
-            Quantity("-3.14", "3"),
-        ),
-        (
-            Quantity("-3.14", "3"),
-            Quantity("3.14", "3"),
-        ),
-        (
-            Quantity("+3.14", "3"),
-            Quantity("-3.14", "3"),
-        ),
-        (
-            Quantity("0", "3"),
-            Quantity("0", "3"),
-        ),
-        (
-            Quantity("-0", "3"),
-            Quantity("0", "3"),
-        ),
-        (
-            Quantity("+0", "3"),
-            Quantity("0", "3"),
-        ),
-        # Constants.
-        (
-            Quantity("3.14", "3", constant=True),
-            Quantity("-3.14", "3", constant=True),
-        ),
-    ],
-)
-def test_neg(quantity, expected):
+
+def test_neg():
     """Should return the negation of a ``Quantity`` object."""
-    actual = -quantity
-    assert actual == expected
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
 
+    assert -Quantity("3.14", "3") == Quantity("-3.14", "3")
+    assert -Quantity("-3.14", "3") == Quantity("3.14", "3")
+    assert -Quantity("+3.14", "3") == Quantity("-3.14", "3")
+    assert -Quantity("0", "3") == Quantity("-0", "3")
+    assert -Quantity("-0", "3") == Quantity("0", "3")
+    assert -Quantity("+0", "3") == Quantity("0", "3")
+    # Constants.
+    assert -Quantity("3.14", "3", constant=True) == Quantity(
+        "-3.14", "3", constant=True
+    )
 
-@pytest.mark.parametrize(
-    "quantity, expected",
-    [
-        (
-            Quantity("3.14", "3"),
-            Quantity("3.14", "3"),
-        ),
-        (
-            Quantity("-3.14", "3"),
-            Quantity("-3.14", "3"),
-        ),
-        (
-            Quantity("+3.14", "3"),
-            Quantity("3.14", "3"),
-        ),
-        (
-            Quantity("0", "3"),
-            Quantity("0", "3"),
-        ),
-        (
-            Quantity("-0", "3"),
-            Quantity("0", "3"),
-        ),
-        (
-            Quantity("+0", "3"),
-            Quantity("0", "3"),
-        ),
-        # Constants.
-        (
-            Quantity("3.14", "3", constant=True),
-            Quantity("3.14", "3", constant=True),
-        ),
-    ],
-)
-def test_pos(quantity, expected):
+
+def test_pos():
     """Should return the positive of a ``Quantity`` object."""
-    actual = +quantity
-    assert actual == expected
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
+
+    assert +Quantity("3.14", "3") == Quantity("3.14", "3")
+    assert +Quantity("-3.14", "3") == Quantity("-3.14", "3")
+    assert +Quantity("+3.14", "3") == Quantity("3.14", "3")
+    assert +Quantity("0", "3") == Quantity("0", "3")
+    assert +Quantity("-0", "3") == Quantity("0", "3")
+    assert +Quantity("+0", "3") == Quantity("0", "3")
+    # Constants.
+    assert +Quantity("3.14", "3", constant=True) == Quantity("3.14", "3", constant=True)
 
 
 # Comparisons tests.
 def test___lt__():
     """Lesser ``Quantity`` objects should be ordered correctly."""
     # Set default precision and rounding.
     getcontext().prec = default_prec
     getcontext().rounding = default_rounding
 
     # Lesser value.
     assert Quantity("3.14", "3") < Quantity("3.15", "3")
-
     # Significance is irrelevant.
     assert Quantity("3.14", "3") < Quantity("3.15", "5")
     assert Quantity("3.14", "5") < Quantity("3.15", "3")
     assert Quantity("3.14", "5") < Quantity("3.15", "3", constant=True)
 
     # Greater value.
     assert not Quantity("3.15", "3") < Quantity("3.14", "3")
-
     # Significance is irrelevant.
     assert not Quantity("3.15", "3") < Quantity("3.14", "5")
     assert not Quantity("3.15", "5") < Quantity("3.14", "3")
     assert not Quantity("3.15", "5") < Quantity("3.14", "3", constant=True)
 
 
 def test___le__():
     """Less than or equal ``Quantity`` objects should be ordered correctly."""
     # Set default precision and rounding.
     getcontext().prec = default_prec
     getcontext().rounding = default_rounding
 
     # Lesser value.
     assert Quantity("3.14", "3") <= Quantity("3.15", "3")
-
     # Significance is irrelevant.
     assert Quantity("3.14", "3") <= Quantity("3.15", "5")
     assert Quantity("3.14", "5") <= Quantity("3.15", "3")
     assert Quantity("3.14", "5") <= Quantity("3.15", "3", constant=True)
-
     # Equal values.
     assert Quantity("3.14", "3") <= Quantity("3.14", "3")
     assert Quantity("3.140", "3") <= Quantity("3.14", "3")
     assert Quantity("3.14", "3") <= Quantity("3.140", "3")
-
     # Equal values after rounding.
     assert Quantity("3.137", "3") <= Quantity("3.136", "3")
-
     # Constants.
     assert Quantity("3.14", "3", constant=True) <= Quantity("3.14", "5", constant=True)
 
 
 def test___eq__():
     """Equal ``Quantity`` objects should be equal."""
     # Set default precision and rounding.
     getcontext().prec = default_prec
     getcontext().rounding = default_rounding
 
     # Equal values.
     assert Quantity("3.14", "3") == Quantity("3.14", "3")
     assert Quantity("3.140", "3") == Quantity("3.14", "3")
     assert Quantity("3.14", "3") == Quantity("3.140", "3")
-
     # Equal values after rounding.
     assert Quantity("3.138", "3") == Quantity("3.141", "3")
-
     # Constants.
     assert Quantity("3.14", "3", constant=True) == Quantity("3.14", "5", constant=True)
     assert Quantity("3.14", getcontext().prec) == Quantity("3.14", "5", constant=True)
 
 
 def test___ne__():
     """Unequal ``Quantity`` objects should not be equal."""
     # Set default precision and rounding.
     getcontext().prec = default_prec
     getcontext().rounding = default_rounding
 
     # Different significance.
     assert Quantity("3.14", "3") != Quantity("3.14", "2")
     assert Quantity("3.14", "3") != Quantity("3.14", "4")
-
     # Different significance and values.
     assert Quantity("3.14", "3") != Quantity("3.15", "2")
     assert Quantity("3.14", "3") != Quantity("3.15", "3")
     assert Quantity("3.14", "3") != Quantity("3.15", "4")
     assert Quantity("3.14", "3") != Quantity("3.13", "2")
     assert Quantity("3.14", "3") != Quantity("3.13", "3")
     assert Quantity("3.14", "3") != Quantity("3.13", "4")
-
     # Constants.
     assert Quantity("3.14", "3", constant=True) != Quantity("3.14", "3")
     assert Quantity("3.14", "3") != Quantity("3.14", "3", constant=True)
 
 
 def test___gt__():
     """Greater ``Quantity`` objects should be greater."""
     # Set default precision and rounding.
     getcontext().prec = default_prec
     getcontext().rounding = default_rounding
 
     # Greater value.
     assert Quantity("3.15", "3") > Quantity("3.14", "3")
-
     # Significance is irrelevant.
     assert Quantity("3.15", "3") > Quantity("3.14", "5")
     assert Quantity("3.15", "5") > Quantity("3.14", "3")
     assert Quantity("3.15", "5") > Quantity("3.14", "3", constant=True)
 
 
 def test___ge__():
     """Greater than or equal ``Quantity`` objects should be ordered correctly."""
     # Set default precision and rounding.
     getcontext().prec = default_prec
     getcontext().rounding = default_rounding
 
     # Greater value.
     assert Quantity("3.15", "3") >= Quantity("3.14", "3")
-
     # Significance is irrelevant.
     assert Quantity("3.15", "3") >= Quantity("3.14", "5")
     assert Quantity("3.15", "5") >= Quantity("3.14", "3")
     assert Quantity("3.15", "5") >= Quantity("3.14", "3", constant=True)
-
     # Equal values.
     assert Quantity("3.14", "3") >= Quantity("3.14", "3")
     assert Quantity("3.140", "3") >= Quantity("3.14", "3")
     assert Quantity("3.14", "3") >= Quantity("3.140", "3")
-
     # Equal values after rounding.
     assert Quantity("3.136", "3") >= Quantity("3.137", "3")
-
     # Constants.
     assert Quantity("3.14", "3", constant=True) >= Quantity("3.14", "5", constant=True)
 
 
 # Arithmetic operations tests.
-@pytest.mark.parametrize(
-    "one, two, expected",
-    [
-        (
-            Quantity("3.14", "3"),
-            Quantity("2.72", "3"),
-            Quantity("5.86", "3"),
-        ),
-        (
-            Quantity("3.14", "3"),
-            Quantity("0.272", "3"),
-            Quantity("3.412", "3"),
-        ),
-        (
-            Quantity("100", "1"),
-            Quantity("0.001", "1"),
-            Quantity("100.001", "1"),
-        ),
-        (
-            Quantity("100", "3"),
-            Quantity("0.001", "1"),
-            Quantity("100.001", "3"),
-        ),
-        (
-            Quantity("100.0", "4"),
-            Quantity("0.001", "1"),
-            Quantity("100.001", "4"),
-        ),
-        # Exponents.
-        (
-            Quantity("3.14e-8", "3"),
-            Quantity("2.72e-8", "3"),
-            Quantity("5.86e-8", "3"),
-        ),
-        (
-            Quantity("3.14e8", "3"),
-            Quantity("2.72e8", "3"),
-            Quantity("5.86e8", "3"),
-        ),
-        # Constants.
-        (
-            Quantity("3.1415", "5"),
-            Quantity("2.72", "3", constant=True),
-            Quantity("5.8615", "5"),
-        ),
-        (
-            Quantity("3.1415", "5", constant=True),
-            Quantity("2.72", "3"),
-            Quantity("5.8615", "3"),
-        ),
-        (
-            Quantity("3.1415", "5", constant=True),
-            Quantity("2.72", "3", constant=True),
-            Quantity("5.8615", "5", constant=True),
-        ),
-    ],
-)
-def test_add(one, two, expected):
+def test_add():
     """Quantities should add."""
-    actual = one + two
-    assert actual == expected
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
 
+    assert Quantity("3.14", "3") + Quantity("2.72", "3") == Quantity("5.86", "3")
+    assert Quantity("3.14", "3") + Quantity("0.272", "3") == Quantity("3.412", "3")
+    assert Quantity("100", "1") + Quantity("0.001", "1") == Quantity("100.001", "1")
+    assert Quantity("100", "3") + Quantity("0.001", "1") == Quantity("100.001", "3")
+    assert Quantity("100.0", "4") + Quantity("0.001", "1") == Quantity("100.001", "4")
+    # Exponents.
+    assert Quantity("3.14e-8", "3") + Quantity("2.72e-8", "3") == Quantity(
+        "5.86e-8", "3"
+    )
+    assert Quantity("3.14e8", "3") + Quantity("2.72e8", "3") == Quantity("5.86e8", "3")
+    # Constants.
+    assert Quantity("3.1415", "5") + Quantity("2.72", "3", constant=True) == Quantity(
+        "5.8615", "5"
+    )
+    assert Quantity("3.1415", "5", constant=True) + Quantity("2.72", "3") == Quantity(
+        "5.8615", "3"
+    )
+    assert Quantity("3.1415", "5", constant=True) + Quantity(
+        "2.72", "3", constant=True
+    ) == Quantity("5.8615", "5", constant=True)
 
-@pytest.mark.parametrize(
-    "one, two",
-    [
-        (
-            Quantity("3.14", "3"),
-            3,
-        ),
-        (
-            3,
-            Quantity("3.14", "3"),
-        ),
-    ],
-)
-def test_add_bad_types(one, two):
+
+def test_add_bad_types():
     """Only quantities should add."""
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
+
+    with pytest.raises(TypeError):
+        Quantity("3.14", "3") + 3
     with pytest.raises(TypeError):
-        one + two
+        3 + Quantity("3.14", "3")
 
 
-@pytest.mark.parametrize(
-    "one, two, expected",
-    [
-        # Easy.
-        (
-            Quantity("3.14", "3"),
-            Quantity("1.72", "3"),
-            Quantity("1.42", "3"),
-        ),
-        # Loss of precision.
-        (
-            Quantity("3.14", "3"),
-            Quantity("2.72", "3"),
-            Quantity("0.42", "2"),
-        ),
-        # First subtrahend more precise.
-        (
-            Quantity("3.1415", "5"),
-            Quantity("2.72", "3"),
-            Quantity("0.4215", "2"),
-        ),
-        (
-            Quantity("3.1415", "5"),
-            Quantity("0.272", "3"),
-            Quantity("2.8695", "4"),
-        ),
-        # Second subtrahend more precise.
-        (
-            Quantity("3.14", "3"),
-            Quantity("0.272", "3"),
-            Quantity("2.868", "3"),
-        ),
-        # No overlap between subtrahends.
-        (
-            Quantity("3.14", "3"),
-            Quantity("0.00272", "3"),
-            Quantity("3.13728", "3"),
-        ),
-        # Rounding regains precision.
-        (
-            Quantity("100", "1"),
-            Quantity("0.001", "1"),
-            Quantity("99.999", "1"),
-        ),
-        (
-            Quantity("100", "1"),
-            Quantity("0.005", "1"),
-            Quantity("99.995", "1"),
-        ),
-        (
-            Quantity("100", "1"),
-            Quantity("0.006", "1"),
-            Quantity("99.994", "1"),
-        ),
-        (
-            Quantity("100.0", "4"),
-            Quantity("0.001", "1"),
-            Quantity("99.999", "3"),
-        ),
-        # Constants.
-        (
-            Quantity("3.1415", "5"),
-            Quantity("1.12", "3", constant=True),
-            Quantity("2.0215", "5"),
-        ),
-        (
-            Quantity("3.1415", "5", constant=True),
-            Quantity("1.12", "3"),
-            Quantity("2.0215", "3"),
-        ),
-        (
-            Quantity("3.1415", "5", constant=True),
-            Quantity("1.12", "3", constant=True),
-            Quantity("2.0215", "4", constant=True),
-        ),
-        (
-            Quantity("3.1415", "5"),
-            Quantity("2.72", "3", constant=True),
-            Quantity("0.4215", "4"),
-        ),
-        (
-            Quantity("3.1415", "5", constant=True),
-            Quantity("2.72", "3"),
-            Quantity("0.4215", "2"),
-        ),
-        (
-            Quantity("3.1415", "5", constant=True),
-            Quantity("2.72", "3", constant=True),
-            Quantity("0.4215", "4", constant=True),
-        ),
-    ],
-)
-def test_sub(one, two, expected):
+def test_sub():
     """Quantities should subtract."""
-    actual = one - two
-    assert actual == expected
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
 
+    # Easy.
+    assert Quantity("3.14", "3") - Quantity("1.72", "3") == Quantity("1.42", "3")
+    # Loss of precision.
+    assert Quantity("3.14", "3") - Quantity("2.72", "3") == Quantity("0.42", "2")
+    # First subtrahend more precise.
+    assert Quantity("3.1415", "5") - Quantity("2.72", "3") == Quantity("0.4215", "2")
+    assert Quantity("3.1415", "5") - Quantity("0.272", "3") == Quantity("2.8695", "4")
+    # Second subtrahend more precise.
+    assert Quantity("3.14", "3") - Quantity("0.272", "3") == Quantity("2.868", "3")
+    # No overlap between subtrahends.
+    assert Quantity("3.14", "3") - Quantity("0.00272", "3") == Quantity("3.13728", "3")
+    # Rounding regains precision.
+    assert Quantity("100", "1") - Quantity("0.001", "1") == Quantity("99.999", "1")
+    assert Quantity("100", "1") - Quantity("0.005", "1") == Quantity("99.995", "1")
+    assert Quantity("100", "1") - Quantity("0.006", "1") == Quantity("99.994", "1")
+    assert Quantity("100.0", "4") - Quantity("0.001", "1") == Quantity("99.999", "3")
+    # Constants.
+    assert Quantity("3.1415", "5") - Quantity("1.12", "3", constant=True) == Quantity(
+        "2.0215", "5"
+    )
+    assert Quantity("3.1415", "5", constant=True) - Quantity("1.12", "3") == Quantity(
+        "2.0215", "3"
+    )
+    assert Quantity("3.1415", "5", constant=True) - Quantity(
+        "1.12", "3", constant=True
+    ) == Quantity("2.0215", "4", constant=True)
+    assert Quantity("3.1415", "5") - Quantity("2.72", "3", constant=True) == Quantity(
+        "0.4215", "4"
+    )
+    assert Quantity("3.1415", "5", constant=True) - Quantity("2.72", "3") == Quantity(
+        "0.4215", "2"
+    )
+    assert Quantity("3.1415", "5", constant=True) - Quantity(
+        "2.72", "3", constant=True
+    ) == Quantity("0.4215", "4", constant=True)
 
-@pytest.mark.parametrize(
-    "one, two",
-    [
-        (
-            Quantity("3.14", "3"),
-            3,
-        ),
-        (
-            3,
-            Quantity("3.14", "3"),
-        ),
-    ],
-)
-def test_sub_bad_types(one, two):
+
+def test_sub_bad_types():
     """Only quantities should subtract."""
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
+
+    with pytest.raises(TypeError):
+        Quantity("3.14", "3") - 3
     with pytest.raises(TypeError):
-        one - two
+        3 - Quantity("3.14", "3")
 
 
-@pytest.mark.parametrize(
-    "one, two, expected",
-    [
-        (
-            Quantity("3.14", "3"),
-            Quantity("2.72", "3"),
-            Quantity("8.5408", "3"),
-        ),
-        (
-            Quantity("3.14", "3"),
-            Quantity("0.272", "3"),
-            Quantity("0.85408", "3"),
-        ),
-        (
-            Quantity("3.14", "3"),
-            Quantity("0.0272", "3"),
-            Quantity("0.085408", "3"),
-        ),
-        (
-            Quantity("314", "3"),
-            Quantity("272", "3"),
-            Quantity("85408", "3"),
-        ),
-        (
-            Quantity("3140", "3"),
-            Quantity("2720", "3"),
-            Quantity("8540800", "3"),
-        ),
-        (
-            Quantity("0.00314", "3"),
-            Quantity("0.00272", "3"),
-            Quantity("0.0000085408", "3"),
-        ),
-        # Constants.
-        (
-            Quantity("3.1415", "5"),
-            Quantity("2.72", "3", constant=True),
-            Quantity("8.54488", "5"),
-        ),
-        (
-            Quantity("2.72", "3", constant=True),
-            Quantity("3.1415", "5"),
-            Quantity("8.54488", "5"),
-        ),
-        (
-            Quantity("2.72", "3", constant=True),
-            Quantity("3.1415", "5", constant=True),
-            Quantity("8.54488", "5", constant=True),
-        ),
-    ],
-)
-def test_mult(one, two, expected):
+def test_mult():
     """Quantities should multiply."""
-    actual = one * two
-    assert actual == expected
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
 
+    # 3.14 * 2.72 = 8.5408
+    assert Quantity("3.14", "3") * Quantity("2.72", "3") == Quantity("8.5408", "3")
+    assert Quantity("3.14", "3") * Quantity("0.272", "3") == Quantity("0.85408", "3")
+    assert Quantity("3.14", "3") * Quantity("0.0272", "3") == Quantity("0.085408", "3")
+    assert Quantity("314", "3") * Quantity("272", "3") == Quantity("85408", "3")
+    assert Quantity("3140", "3") * Quantity("2720", "3") == Quantity("8540800", "3")
+    assert Quantity("0.00314", "3") * Quantity("0.00272", "3") == Quantity(
+        "0.0000085408", "3"
+    )
+    # Constants.
+    assert Quantity("3.1415", "5") * Quantity("2.72", "3", constant=True) == Quantity(
+        "8.54488", "5"
+    )
+    assert Quantity("2.72", "3", constant=True) * Quantity("3.1415", "5") == Quantity(
+        "8.54488", "5"
+    )
+    assert Quantity("2.72", "3", constant=True) * Quantity(
+        "3.1415", "5", constant=True
+    ) == Quantity("8.54488", "5", constant=True)
 
-@pytest.mark.parametrize(
-    "one, two",
-    [
-        (
-            Quantity("3.14", "3"),
-            3,
-        ),
-        (
-            3,
-            Quantity("3.14", "3"),
-        ),
-    ],
-)
-def test_mul_bad_types(one, two):
+
+def test_mul_bad_types():
     """Only quantities should multiply."""
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
+
     with pytest.raises(TypeError):
-        one * two
+        Quantity("3.14", "3") * 3
+    with pytest.raises(TypeError):
+        3 * Quantity("3.14", "3")
 
 
-@pytest.mark.parametrize(
-    "num, den, expected",
-    [
-        (
-            Quantity("8.5408", "3"),
-            Quantity("2.72", "3"),
-            Quantity("3.14", "3"),
-        ),
-        (
-            Quantity("8.5408", "3"),
-            Quantity("0.272", "3"),
-            Quantity("31.4", "3"),
-        ),
-        (
-            Quantity("8.5408", "3"),
-            Quantity("0.0272", "3"),
-            Quantity("314", "3"),
-        ),
-        (
-            Quantity("85408", "3"),
-            Quantity("272", "3"),
-            Quantity("314", "3"),
-        ),
-        (
-            Quantity("854080", "3"),
-            Quantity("2720", "3"),
-            Quantity("314", "3"),
-        ),
-        (
-            Quantity("0.0085408", "3"),
-            Quantity("0.00272", "3"),
-            Quantity("3.14", "3"),
-        ),
-        (
-            Quantity("0.85408", "3"),
-            Quantity("2.72", "3"),
-            Quantity("0.314", "3"),
-        ),
-        (
-            Quantity("0.085408", "3"),
-            Quantity("2.72", "3"),
-            Quantity("0.0314", "3"),
-        ),
-        (
-            Quantity("0.0085408", "3"),
-            Quantity("2.72", "3"),
-            Quantity("0.00314", "3"),
-        ),
-        (
-            Quantity("3.1415", "5"),
-            Quantity("2.72", constant=True),
-            Quantity("1.154963235294117647058823529", "5"),
-        ),
-        (
-            Quantity("3.1415", constant=True),
-            Quantity("2.72", "3"),
-            Quantity("1.154963235294117647058823529", "3"),
-        ),
-        (
-            Quantity("3.1415", constant=True),
-            Quantity("2.72", constant=True),
-            Quantity("1.154963235294117647058823529", constant=True),
-        ),
-    ],
-)
-def test_div(num, den, expected):
+def test_div():
     """Quantities should divide."""
-    actual = num / den
-    assert actual == expected
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
 
+    # 8.5408 / 2.72 = 3.14
+    assert Quantity("8.5408", "3") / Quantity("2.72", "3") == Quantity("3.14", "3")
+    assert Quantity("8.5408", "3") / Quantity("0.272", "3") == Quantity("31.4", "3")
+    assert Quantity("8.5408", "3") / Quantity("0.0272", "3") == Quantity("314", "3")
+    assert Quantity("85408", "3") / Quantity("272", "3") == Quantity("314", "3")
+    assert Quantity("854080", "3") / Quantity("2720", "3") == Quantity("314", "3")
+    assert Quantity("0.0085408", "3") / Quantity("0.00272", "3") == Quantity(
+        "3.14", "3"
+    )
+    assert Quantity("0.85408", "3") / Quantity("2.72", "3") == Quantity("0.314", "3")
+    assert Quantity("0.085408", "3") / Quantity("2.72", "3") == Quantity("0.0314", "3")
+    assert Quantity("0.0085408", "3") / Quantity("2.72", "3") == Quantity(
+        "0.00314", "3"
+    )
+    # Constants.
+    assert Quantity("3.1415", "5") / Quantity("2.72", "3", constant=True) == Quantity(
+        "1.154963235294117647058823529", "5"
+    )
+    assert Quantity("3.1415", "5", constant=True) / Quantity("2.72", "3") == Quantity(
+        "1.154963235294117647058823529", "3"
+    )
+    assert Quantity("3.1415", "5", constant=True) / Quantity(
+        "2.72", "3", constant=True
+    ) == Quantity("1.154963235294117647058823529", "3", constant=True)
 
-@pytest.mark.parametrize(
-    "num, den",
-    [
-        (
-            Quantity("3.14", "3"),
-            3,
-        ),
-        (
-            3,
-            Quantity("3.14", "3"),
-        ),
-    ],
-)
-def test_div_bad_types(num, den):
+
+def test_div_bad_types():
     """Only quantities should divide."""
+    # Set default precision and rounding.
+    getcontext().prec = default_prec
+    getcontext().rounding = default_rounding
+
+    with pytest.raises(TypeError):
+        Quantity("3.14", "3") / 3
     with pytest.raises(TypeError):
-        num / den
+        3 / Quantity("3.14", "3")
 
 
 def test_textbook_examples():
     """Should corroborate answers to textbook problems."""
     # Set default precision and rounding.
     getcontext().prec = default_prec
     getcontext().rounding = default_rounding
```

### Comparing `sigcalc-0.1.0/PKG-INFO` & `sigcalc-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigcalc
-Version: 0.1.0
+Version: 0.1.1
 Summary: significant figures calculations
 Home-page: https://github.com/jeremyagray/sigcalc
 License: GPL-3.0-or-later
 Author: Jeremy A Gray
 Author-email: gray@flyquackswim.com
 Maintainer: Jeremy A Gray
 Maintainer-email: gray@flyquackswim.com
@@ -13,25 +13,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: mpmath (>=1,<2)
 Project-URL: Documentation, https://sigcalc.readthedocs.io/
 Project-URL: Issues, https://github.com/jeremyagray/sigcalc/issues
 Project-URL: Repository, https://github.com/jeremyagray/sigcalc
 Description-Content-Type: text/x-rst
 
 .. *****************************************************************************
 ..
 .. sigcalc, significant figures calculations
 ..
-.. Copyright 2023-2024 Jeremy A Gray <gray@flyquackswim.com>.
+.. Copyright 2023 Jeremy A Gray <gray@flyquackswim.com>.
 ..
 .. All rights reserved.
 ..
 .. SPDX-License-Identifier: GPL-3.0-or-later
 ..
 .. *****************************************************************************
 
@@ -57,47 +56,37 @@
 
   pip install sigcalc
 
 or with poetry::
 
   poetry add sigcalc
 
-``sigcalc`` depends on the internal ``decimal``
-`module <https://docs.python.org/3/library/decimal.html>`_
-for arithmetic and `mpmath <https://mpmath.org/>`_ for transcendental
-and other functions.
+``sigcalc`` depends on the internal ``decimal`` module for arithmetic
+and ``mpmath`` (https://mpmath.org/) for transcendental and other
+functions.
 
 Usage
 -----
 
 Import the ``Quantity`` class:
 
 >>> from sigcalc import Quantity
->>> from decimal import getcontext
->>> getcontext().prec = 28
 
 Create ``Quantity`` objects as necessary:
 
 >>> a = Quantity("3.14", "3")
 >>> b = Quantity("2.72", "3")
 
 The precision of the underlying ``decimal`` context should adjust
 automatically to contain the number of digits specified or the number
 of significant figures, within the limits of the ``decimal`` module.
 
 Arithmetic for ``Quantity`` objects is implemented on the usual magic
 methods:
 
->>> from sigcalc import Quantity
->>> from decimal import getcontext
->>> from decimal import ROUND_HALF_EVEN
->>> getcontext().prec = 28
->>> getcontext().rounding = ROUND_HALF_EVEN
->>> a = Quantity("3.14", "3")
->>> b = Quantity("2.72", "3")
 >>> a + b
 Quantity("5.86", "3")
 >>> a - b
 Quantity("0.42", "2")
 >>> a * b
 Quantity("8.5408", "3")
 >>> a / b
@@ -107,15 +96,15 @@
 >>> -a
 Quantity("-3.14", "3")
 >>> +a
 Quantity("3.14", "3")
 
 Beware that rounding is not performed during calculations and that
 reported significant figures for calculated values are for the
-unrounded value.  For example, a calculation that resulted in a result
+unrounded value.  For example, a claculation that resulted in a result
 of ``Quantity("99.9", "3")`` could round to ``Quantity("100.0",
 "4")``, depending on the current rounding mode.
 
 Note that ``__floordiv__`` is not implemented as it is not useful for
 significant figures calculations.
 
 >>> a // b
@@ -203,79 +192,31 @@
 >>> getcontext().rounding = ROUND_HALF_UP
 >>> format(a, ".2e")
 '3.15e+0'
 >>> getcontext().rounding = ROUND_HALF_EVEN
 >>> format(b, ".2e")
 '3.14e+0'
 
-Power and Square Root Functions
-...............................
-
-The power and square root (``__pow__()`` and ``sqrt()``) functions and
-are implemented as wrappers around the appropriate functions from
-``decimal.Decimal``, calculating results based on the ``value`` of a
-``Quantity`` combined with the correct significant figures, following
-the "significance in, significance out" rule for both functions.
-
-Exponential and Logarithmic Functions
-.....................................
-
-The exponential and logarithmic (``exp()``, ``exp10()``, ``ln()``, and
-``log10()``) functions are implemented as wrappers around the
-corresponding functions from ``decimal`` to calculate the ``value`` of
-a ``Quantity`` combined with the correct significant figures.
-Abscissa digits are treated as placeholders so a logarithm will
-increase significance by the number of significant abscissa digits;
-exponentials will decrease the significance by the number of
-significant abscissa digits.  Consequently, if a ``Quantity`` has
-significant figures less than or equal to the number of abscissa
-digits, a ``RuntimeWarning`` will be raised and a ``Quantity`` with
-zero significant figures will be returned.  See the references for
-more information.
-
-Transcendental Functions
-........................
-
-The transcendental functions and their inverses are implemented as
-wrappers around the appropriate functions from ``mpmath``, calculating
-results based on the ``value`` of a ``Quantity`` combined with the
-correct significant figures, following the "significance in,
-significance out" rule.
-
-Hyperbolic Functions
-....................
-
-The hyperbolic functions and their inverses are implemented as
-wrappers around the appropriate functions from ``mpmath``, calculating
-results based on the ``value`` of a ``Quantity`` combined with the
-correct significant figures, following the "significance in,
-significance out" rule.
+The transcendental and exponential functions will be implemented as
+wrappers around the appropriate functions from ``decimal`` and
+``mpmath``, calculating results based on the ``value`` of a
+``Quantity`` with the correct significant figures.
 
 References
 ----------
 
 ``sigcalc`` implements significant figures calculations as commonly
 described in high school and undergraduate chemistry and physics
 textbooks, examples of which may be found at:
 
 1. `Significant Figures at Wikipedia <https://en.wikipedia.org/wiki/Significant_figures>`_
 2. `Significance Arithmetic at Wikipedia <https://en.wikipedia.org/wiki/Significance_arithmetic>`_
 3. Myers, R.T.; Tocci, S.; Oldham, K.B., Holt Chemistry, Holt, Rinehart and Winston: 2006.
-4. `"How many significant figures in 0.0" <https://math.stackexchange.com/questions/2149316/>`_
-
-Thanks to the developers of Python's ``decimal``
-`module <https://docs.python.org/3/library/decimal.html>`_,
-the `mpmath <https://mpmath.org/>`_ library, and the
-`hypothesis <https://hypothesis.readthedocs.io/>`_ testing library,
-without which, this would be a much smaller and less functional
-library.
-
-Thanks also to LibreTexts Mathematics for their reference on `hyperbolic functions <https://math.libretexts.org/Courses/Monroe_Community_College/MTH_211_Calculus_II/Chapter_6%3A_Applications_of_Integration/6.9%3A_Calculus_of_the_Hyperbolic_Functions>`_.
 
-Remember, calculating with significant figures is not a substitute for
+Calculating with significant figures is not a substitute for
 repetition of measurements and proper statistical analysis.
 
 Copyright and License
 ---------------------
 
 SPDX-License-Identifier: `GPL-3.0-or-later <https://spdx.org/licenses/GPL-3.0-or-later.html>`_
```

