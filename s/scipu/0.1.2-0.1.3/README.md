# Comparing `tmp/scipu-0.1.2.tar.gz` & `tmp/scipu-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipu-0.1.2.tar", last modified: Sun May 26 13:21:25 2024, max compression
+gzip compressed data, was "scipu-0.1.3.tar", last modified: Tue May 28 09:22:06 2024, max compression
```

## Comparing `scipu-0.1.2.tar` & `scipu-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 13:21:25.830673 scipu-0.1.2/
--rw-rw-rw-   0        0        0       38 2024-05-26 12:40:51.000000 scipu-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       18 2024-05-26 10:39:36.000000 scipu-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      389 2024-05-26 13:21:25.830673 scipu-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       31 2024-05-26 10:39:32.000000 scipu-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 13:21:25.824693 scipu-0.1.2/scipu/
--rw-rw-rw-   0        0        0       29 2024-05-26 13:20:14.000000 scipu-0.1.2/scipu/__init__.py
--rw-rw-rw-   0        0        0     5598 2024-05-26 11:31:26.000000 scipu-0.1.2/scipu/package.py
-drwxrwxrwx   0        0        0        0 2024-05-26 13:21:25.830673 scipu-0.1.2/scipu.egg-info/
--rw-rw-rw-   0        0        0      389 2024-05-26 13:21:25.000000 scipu-0.1.2/scipu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-05-26 13:21:25.000000 scipu-0.1.2/scipu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 13:21:25.000000 scipu-0.1.2/scipu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-26 13:21:25.000000 scipu-0.1.2/scipu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-26 13:21:25.831670 scipu-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      579 2024-05-26 13:20:03.000000 scipu-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:22:06.369518 scipu-0.1.3/
+-rw-rw-rw-   0        0        0       38 2024-05-26 12:40:51.000000 scipu-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       18 2024-05-26 10:39:36.000000 scipu-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      389 2024-05-28 09:22:06.369518 scipu-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2024-05-26 10:39:32.000000 scipu-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 09:22:06.361542 scipu-0.1.3/scipu/
+-rw-rw-rw-   0        0        0       29 2024-05-26 13:20:14.000000 scipu-0.1.3/scipu/__init__.py
+-rw-rw-rw-   0        0        0     5607 2024-05-28 09:20:43.000000 scipu-0.1.3/scipu/package.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:22:06.369518 scipu-0.1.3/scipu.egg-info/
+-rw-rw-rw-   0        0        0      389 2024-05-28 09:22:06.000000 scipu-0.1.3/scipu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-05-28 09:22:06.000000 scipu-0.1.3/scipu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:22:06.000000 scipu-0.1.3/scipu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-28 09:22:06.000000 scipu-0.1.3/scipu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-28 09:22:06.370515 scipu-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      579 2024-05-28 09:20:56.000000 scipu-0.1.3/setup.py
```

### Comparing `scipu-0.1.2/scipu/package.py` & `scipu-0.1.3/scipu/package.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     task = 'Абсолютно непрерывная случайная величина  X  может принимать значения только в отрезке [a, b]. На этом отрезке плотность распределения случайной величины  X  имеет вид: f(x)=C(1+a^0.1+2b^0.2+3c^0.3)^1.1, где С - положительная константа. Найти:\n- константу C математическое ожидание E(X)\n- стандартное отклонение σX\n- квантиль уровня k распределения X'
     print(task)
     answer = '\n#условие\n# [a,b]\na,b = 4,9\n# F = f(x) без C\nF = lambda x: (1 + 7*x**(0.5) + 8*x**(0.7) + 4*x**(0.9))**(1.3)\nC = 1 / integrate.quad(F, a, b)[0]\ndef f(x):\n    return C * F(x)\nclass dist_f_C(rv_continuous):\n  #функция вероятности\n  def _pdf(self,x):\n    return f(x) if (a<= x <=b) else 0\n  #функция значений\n  def _expect(self,x):\n    return x\n#зададим распределение\nf_C = dist_f_C(a = a, b = b)\n#1\nprint(f"C = {C}")\n#2\nprint(f"E = {f_C.mean()}")\n#3\nprint(f"sigma = {f_C.std()}")\n#4\nprint(f"q = {f_C.ppf(0.9)}")\n'
     print(answer)
 def CRV_2():
     task = 'Случайная величина X равномерно распределена на отрезке [a,b]. Случайная величина Y выражается через X следующим образом: Y = (1+a^0.1+2b^0.2+3c^0.3)^1.1. Найдите:\n- математическое ожидание  E(Y)\n- стандартное отклонение σY\n- асимметрию As(Y)\n- квантиль уровня 0,8 распределения Y'
     print(task)
-    answer = '\nF = lambda x: (1 + 6*x**0.5 + 4*x**0.7 + 5 * x**0.9)**1.3\nab = [4, 8]\np = 1/(ab[1]-ab[0])\nEY = p * integrate.quad(F, 4, 8)[0]\nprint(f"EY = {EY}")\nf = lambda x: (F(x))**2\nVarY = p * integrate.quad(f, 4, 8)[0] - EY**2\nQy = math.sqrt(VarY)\nprint(f"Qy = {Qy}")\nf = lambda x: p * (F(x) - EY)**3\nAsY = integrate.quad(f, 4, 8)[0]/Qy**3\nprint(f"AsY = {AsY}")\n#q_l = quantile_level\nq_l = 0.8\n# работает при равномерном случайном распределении!\nq = F(ab[0] + ab[0]*q_l)\nprint(f"q = {q}")\n'
+    answer = '\nF = lambda x: (1 + 6*x**0.5 + 4*x**0.7 + 5 * x**0.9)**1.3\nab = [4, 8]\np = 1/(ab[1]-ab[0])\nEY = p * integrate.quad(F, 4, 8)[0]\nprint(f"EY = {EY}")\nf = lambda x: (F(x))**2\nVarY = p * integrate.quad(f, 4, 8)[0] - EY**2\nQy = math.sqrt(VarY)\nprint(f"Qy = {Qy}")\nf = lambda x: p * (F(x) - EY)**3\nAsY = integrate.quad(f, 4, 8)[0]/Qy**3\nprint(f"AsY = {AsY}")\n#q_l = quantile_level\nq_l = 0.8\n# работает при равномерном случайном распределении!\nq = F(ab[0] + (ab[1]-ab[0])*q_l)\nprint(f"q = {q}")\n'
     print(answer)
 
 #NormalRandomVectors
 def NRV_1():
     task = 'Для нормального случайного вектора (X,Y)∼N(−8;16;49;1;0,8) найдите вероятность P((X−3)(Y−7)<0).'
     print(task)
     answer = "\nN = {'muX': -8, 'muY': 16, 'sigmaX2': 49, 'sigmaY2': 1, 'rho': 0.8}\nmu = np.array([N['muX'], N['muY']])\nCov = np.array([[N['sigmaX2'], N['rho']*math.sqrt(N['sigmaX2'])*math.sqrt(N['sigmaY2'])],\n                [N['rho']*math.sqrt(N['sigmaX2'])*math.sqrt(N['sigmaY2']), N['sigmaY2']]])\nW = multivariate_normal(mu, Cov)\nX = norm(N['muX'], math.sqrt(N['sigmaX2']))\nY = norm(N['muY'], math.sqrt(N['sigmaY2']))\nPx = 3\nPy = 7\nPa=X.cdf(Px)-W.cdf([Px,Py])\nPb=Y.cdf(Py)-W.cdf([Px,Py])\nPa+Pb\n"
@@ -32,8 +32,8 @@
     print(task)
     answer = "\n#Смотрим на распределение, которое задано\nmuX = -4\nmuY = 4\nsigmaX = 64**0.5\nsigmaY = 81**0.5\nrho = -0.31\n#Смотрим на вероятность, которую хотят от нас\nxminus1 = 8\nxminus2 = 10\nyminus = 1\nmu = np.array([muX,muY])\nCov = np.array([[sigmaX**2, rho*sigmaX*sigmaY], [rho*sigmaX*sigmaY, sigmaY**2]])\nX = norm(muX, sigmaX)\nY = norm(muY, sigmaY)\nW = multivariate_normal(mu, Cov)\nPa = W.cdf([xminus1, yminus])\nPb = X.cdf(xminus2) - X.cdf(xminus1) - (W.cdf([xminus2, yminus]) - W.cdf([xminus1, yminus]))\nPc = Y.cdf(yminus) - W.cdf([xminus2, yminus])\nPa+Pb+Pc\n"
     print(answer)
 def NRV_3():
     task = 'Случайный вектор (X,Y) имеет плотность распределения fX,Y(x,y)=(18e^(−30x2−48xy+8x−30y2−5y−8524))\π\nНайдите:\n- математическое ожидание E(X)\n-математическое ожидание E(Y)\n-дисперсию  Var(X)\n-дисперсию  Var(Y)\n-ковариацию  Cov(X,Y)\n-коэффициент корреляции  ρ(X,Y)'
     print(task)
     answer = "\n#после выноса -1/2!!!!!!\ncoefs = {\n    'x^2': 60,\n    'x': -16,\n    'xy': 96,\n    'y': 10,\n    'y^2': 60,\n}\nC = np.matrix([[coefs['x^2'], coefs['xy']/2], [coefs['xy']/2, coefs['y^2']]])\nC1 = C**(-1)\nVarX = C1[0, 0]\nsigmaX = np.sqrt(VarX)\nVarY = C1[1, 1]\nsigmaY = np.sqrt(VarY)\nCovXY = C1[0, 1]\nroXY = CovXY/(sigmaX*sigmaY)\nEX, EY = sympy.symbols('EX, EY')\nequations = (\n    sympy.Eq(coefs['x^2']*EX + coefs['xy']/2*EY, coefs['x']*(-1/2)),\n    sympy.Eq(coefs['xy']/2*EX + coefs['y^2']*EY, coefs['y']*(-1/2))\n)\nsol = sympy.solve(equations, (EX, EY))\nprint(f'EX = {sol[EX]}, EY = {sol[EY]}, VarX = {VarX}, VarY = {VarY}, CovXY = {CovXY}, roXY = {roXY}')\n"
-    print(answer)
+    print(answer)
```

### Comparing `scipu-0.1.2/setup.py` & `scipu-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   with open('README.md', 'r') as f:
     return f.read()
 
 
 
 setup(
     name='scipu',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     description='A simple TVIMS library',
     author='Ackrome',
     author_email='ivansergeyevicht@gmail.com',
     url='https://github.com/Ackrome/scipu',
     classifiers=[
         'Programming Language :: Python :: 3',
```
