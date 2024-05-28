# Comparing `tmp/peakfit-0.5.0.tar.gz` & `tmp/peakfit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakfit-0.5.0.tar", last modified: Wed May 22 21:42:15 2024, max compression
+gzip compressed data, was "peakfit-0.6.0.tar", last modified: Tue May 28 20:20:43 2024, max compression
```

## Comparing `peakfit-0.5.0.tar` & `peakfit-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    34916 2024-05-22 21:42:11.421680 peakfit-0.5.0/LICENSE
--rw-r--r--   0        0        0       75 2024-05-22 21:42:11.421680 peakfit-0.5.0/README.md
--rw-r--r--   0        0        0       73 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/__init__.py
--rw-r--r--   0        0        0      126 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/__main__.py
--rw-r--r--   0        0        0     1431 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/cli.py
--rw-r--r--   0        0        0     3845 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/clustering.py
--rw-r--r--   0        0        0      999 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/computing.py
--rw-r--r--   0        0        0     2597 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/messages.py
--rw-r--r--   0        0        0      467 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/noise.py
--rw-r--r--   0        0        0     8075 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/peakfit.py
--rw-r--r--   0        0        0     1678 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/plot_cest.py
--rw-r--r--   0        0        0     2725 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/plot_cpmg.py
--rw-r--r--   0        0        0     1225 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/plot_intensities.py
--rw-r--r--   0        0        0     1719 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/shapes.py
--rw-r--r--   0        0        0        0 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/writing.py
--rw-r--r--   0        0        0     1138 2024-05-22 21:42:15.869702 peakfit-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 peakfit-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34916 2024-05-28 20:20:31.933946 peakfit-0.6.0/LICENSE
+-rw-r--r--   0        0        0       75 2024-05-28 20:20:31.933946 peakfit-0.6.0/README.md
+-rw-r--r--   0        0        0       73 2024-05-28 20:20:32.345948 peakfit-0.6.0/peakfit/__init__.py
+-rw-r--r--   0        0        0      126 2024-05-28 20:20:32.345948 peakfit-0.6.0/peakfit/__main__.py
+-rw-r--r--   0        0        0     1431 2024-05-28 20:20:32.345948 peakfit-0.6.0/peakfit/cli.py
+-rw-r--r--   0        0        0     3903 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/clustering.py
+-rw-r--r--   0        0        0     1243 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/computing.py
+-rw-r--r--   0        0        0     2602 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/messages.py
+-rw-r--r--   0        0        0      467 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/noise.py
+-rw-r--r--   0        0        0     8970 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/peakfit.py
+-rw-r--r--   0        0        0     3175 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/peaklist.py
+-rw-r--r--   0        0        0     1678 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/plot_cest.py
+-rw-r--r--   0        0        0     2725 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/plot_cpmg.py
+-rw-r--r--   0        0        0     1225 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/plot_intensities.py
+-rw-r--r--   0        0        0     2900 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/plots.py
+-rw-r--r--   0        0        0     2039 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/shapes.py
+-rw-r--r--   0        0        0        0 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/writing.py
+-rw-r--r--   0        0        0     1203 2024-05-28 20:20:43.769992 peakfit-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 peakfit-0.6.0/PKG-INFO
```

### Comparing `peakfit-0.5.0/LICENSE` & `peakfit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peakfit-0.5.0/peakfit/cli.py` & `peakfit-0.6.0/peakfit/cli.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.5.0/peakfit/computing.py` & `peakfit-0.6.0/peakfit/computing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
+import lmfit as lf
 import numpy as np
 
 import peakfit.shapes as ps
+from peakfit.clustering import Cluster
 
 
-def calculate_shape_heights(params, cluster):
+def calculate_shape_heights(
+    params: lf.Parameters, cluster: Cluster
+) -> tuple[np.ndarray, np.ndarray]:
     shapes = []
 
     for index in range(len(cluster.peaks)):
         pre = f"p{index}_"
         shapes.append(
             ps.pvoigt2d(
                 cluster.x,
                 cluster.y,
-                params[f"{pre}x0"],
-                params[f"{pre}y0"],
-                params[f"{pre}x_fwhm_ppm"],
-                params[f"{pre}y_fwhm_ppm"],
-                params[f"{pre}x_eta"],
-                params[f"{pre}y_eta"],
+                params[f"{pre}x0_pt"].value,
+                params[f"{pre}y0_pt"].value,
+                params[f"{pre}x_fwhm_pt"].value,
+                params[f"{pre}y_fwhm_pt"].value,
+                params[f"{pre}x_eta"].value,
+                params[f"{pre}y_eta"].value,
             ),
         )
 
     shapes = np.asarray(shapes).T
     amp_values = np.linalg.lstsq(shapes, cluster.data, rcond=None)[0]
 
     return shapes, amp_values
 
 
-def residuals(params, cluster, noise):
+def residuals(params: lf.Parameters, cluster: Cluster, noise: float) -> np.ndarray:
     shapes, amplitudes = calculate_shape_heights(params, cluster)
     return np.ravel((cluster.data - shapes.dot(amplitudes)) / noise)
 
 
-def simulate_data(params, cluster):
+def simulate_data(params: lf.Parameters, cluster: Cluster) -> np.ndarray:
     shapes, amplitudes = calculate_shape_heights(params, cluster)
     return shapes.dot(amplitudes)
```

### Comparing `peakfit-0.5.0/peakfit/messages.py` & `peakfit-0.6.0/peakfit/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """Print the fitting message."""
     message = "\n — Fitting peaks..."
     console.print(message, style="bold yellow")
 
 
 def print_peaks(peaks) -> None:
     """Print the peak names that are being fitted."""
-    peak_list = ", ".join(f"{peak[0]:s}" for peak in peaks)
+    peak_list = ", ".join(f"{name:s}" for name in peaks["name"])
     message = f"Peak(s): {peak_list}"
     panel = Panel.fit(message, style="green")
     console.print(panel)
 
 
 def print_segmenting() -> None:
     """Print the segmenting message."""
```

### Comparing `peakfit-0.5.0/peakfit/peakfit.py` & `peakfit-0.6.0/peakfit/peakfit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,215 @@
 """Main module."""
 
-import random
 from collections.abc import Sequence
 from pathlib import Path
 
 import lmfit as lf
 import nmrglue as ng
 import numpy as np
-import numpy.random as nr
+from matplotlib.backends.backend_pdf import PdfPages
 
 from peakfit.cli import build_parser
 from peakfit.clustering import Cluster, Spectra, cluster_peaks
 from peakfit.computing import calculate_shape_heights, residuals, simulate_data
 from peakfit.messages import (
     export_html,
     print_estimated_noise,
     print_fit_report,
     print_fitting,
     print_logo,
     print_peaks,
 )
 from peakfit.noise import estimate_noise
+from peakfit.peaklist import read_list
+from peakfit.plots import plot_pdf
 from peakfit.shapes import create_params
 
 
 def read_spectra(
     paths_spectra: Sequence[Path],
     paths_z_values: Sequence[Path],
     exclude_list: Sequence[int],
 ) -> Spectra:
     """Read NMRPipe spectra and return a Spectra object."""
-    # Read NMRPipe spectra
-    dic_list = []
-    data_list = []
+    dic_list, data_list = [], []
+
     for path in paths_spectra:
         dic, data = ng.fileio.pipe.read(str(path))
         dic_list.append(dic)
         data_list.append(data)
     data = np.concatenate(data_list, axis=0)
 
-    # Read z values
-    z_list = [np.genfromtxt(path, dtype=None) for path in paths_z_values]
-    z_values = np.concatenate(z_list)
+    z_values = np.concatenate(
+        [np.genfromtxt(path, dtype=None) for path in paths_z_values]
+    )
 
-    # Exclude planes
     if exclude_list:
-        exclude_array = np.full_like(z_values, fill_value=False, dtype=np.bool_)
-        exclude_array[exclude_list] = True
-        data = data[~exclude_array]
-        z_values = z_values[~exclude_array]
+        data, z_values = exclude_planes(data, z_values, exclude_list)
 
-    # Create unit conversion object for indirect and direct dimension
     dic = dic_list[0]
-    ucy = ng.pipe.make_uc(dic, data, dim=1)
-    ucx = ng.pipe.make_uc(dic, data, dim=2)
+    ucy, ucx = ng.pipe.make_uc(dic, data, dim=1), ng.pipe.make_uc(dic, data, dim=2)
 
-    # Create and return 'Spectra' object
     return Spectra(data, ucx, ucy, z_values)
 
 
+def exclude_planes(
+    data: np.ndarray, z_values: np.ndarray, exclude_list: Sequence[int]
+) -> tuple[np.ndarray, np.ndarray]:
+    """Exclude specified planes from data and z_values."""
+    exclude_array = np.full_like(z_values, fill_value=False, dtype=np.bool_)
+    exclude_array[exclude_list] = True
+    return data[~exclude_array], z_values[~exclude_array]
+
+
 def write_profiles(
-    path,
-    z_values,
-    cluster,
-    params,
-    heights,
-    params_err,
-    height_err,
+    path: Path,
+    z_values: np.ndarray,
+    cluster: Cluster,
+    params: lf.Parameters,
+    heights: np.ndarray,
+    params_err: dict,
+    height_err: np.ndarray,
 ) -> None:
-    for i, peak in enumerate(cluster.peaks):
-        vals = params.valuesdict()
-        errs = {k: v if v is not None else 0.0 for k, v in params_err.items()}
-
-        x_ppm = vals[f"p{i}_x0"]
-        y_ppm = vals[f"p{i}_y0"]
-        x_ppm_e = errs[f"p{i}_x0"]
-        y_ppm_e = errs[f"p{i}_y0"]
-
-        xw_hz = vals[f"p{i}_x_fwhm"]
-        yw_hz = vals[f"p{i}_y_fwhm"]
-        xw_hz_e = errs[f"p{i}_x_fwhm"]
-        yw_hz_e = errs[f"p{i}_y_fwhm"]
-
-        x_eta = vals[f"p{i}_x_eta"]
-        y_eta = vals[f"p{i}_y_eta"]
-        x_eta_e = errs[f"p{i}_x_eta"]
-        y_eta_e = errs[f"p{i}_y_eta"]
-
-        ampl_e = np.mean(height_err[i])
-
-        with (path / f"{peak.name}.out").open("w") as f:
-            f.write(f"# Name: {peak.name}\n")
-            f.write(f"# y_ppm: {y_ppm:10.5f} {y_ppm_e:10.5f}\n")
-            f.write(f"# yw_hz: {yw_hz:10.5f} {yw_hz_e:10.5f}\n")
-            f.write(f"# y_eta: {y_eta:10.5f} {y_eta_e:10.5f}\n")
-            f.write(f"# x_ppm: {x_ppm:10.5f} {x_ppm_e:10.5f}\n")
-            f.write(f"# xw_hz: {xw_hz:10.5f} {xw_hz_e:10.5f}\n")
-            f.write(f"# x_eta: {x_eta:10.5f} {x_eta_e:10.5f}\n")
-            f.write("#---------------------------------------------\n")
-            f.write(f"# {'Z':>10s}  {'I':>14s}  {'I_err':>14s}\n")
-            f.write(
-                "\n".join(
-                    f"  {z!s:>10s}  {ampl:14.6e}  {ampl_e:14.6e}"
-                    for z, ampl in zip(z_values, heights[i], strict=False)
-                ),
-            )
+    """Write profile information to output files."""
+    for i, peak in enumerate(cluster.peaks.itertuples()):
+        vals, errs = (
+            params.valuesdict(),
+            {k: v if v is not None else 0.0 for k, v in params_err.items()},
+        )
 
+        profile_data = {
+            "x_ppm:": f'{vals[f"p{i}_x0"]:10.5f} {errs[f"p{i}_x0"]:10.5f}',
+            "y_ppm:": f'{vals[f"p{i}_y0"]:10.5f} {errs[f"p{i}_y0"]:10.5f}',
+            "xw_hz:": f'{vals[f"p{i}_x_fwhm"]:10.5f} {errs[f"p{i}_x_fwhm"]:10.5f}',
+            "yw_hz:": f'{vals[f"p{i}_y_fwhm"]:10.5f} {errs[f"p{i}_y_fwhm"]:10.5f}',
+            "x_eta:": f'{vals[f"p{i}_x_eta"]:10.5f} {errs[f"p{i}_x_eta"]:10.5f}',
+            "y_eta:": f'{vals[f"p{i}_y_eta"]:10.5f} {errs[f"p{i}_y_eta"]:10.5f}',
+        }
+
+        write_profile(
+            path / f"{peak.name}.out",
+            peak.name,
+            profile_data,
+            z_values,
+            heights[i],
+            height_err[i],
+        )
 
-def get_some_noise(spectra, noise, x_pt, y_pt):
-    nr.shuffle(noise)
 
-    nz_noise, ny_noise, nx_noise = noise.shape
+def write_profile(
+    filepath: Path,
+    name: str,
+    profile_data: dict,
+    z_values: np.ndarray,
+    heights: np.ndarray,
+    heights_err: np.ndarray,
+) -> None:
+    """Write individual profile data to a file."""
+    with filepath.open("w") as f:
+        f.write(f"# Name: {name}\n")
+        for key, value in profile_data.items():
+            f.write(f"# {key:<10s} {value}\n")
+        f.write("#---------------------------------------------\n")
+        f.write(f"# {'Z':>10s}  {'I':>14s}  {'I_err':>14s}\n")
+        f.write(
+            "\n".join(
+                f"  {z!s:>10s}  {ampl:14.6e}  {ampl_e:14.6e}"
+                for z, ampl, ampl_e in zip(z_values, heights, heights_err, strict=False)
+            )
+        )
 
-    x_off = random.randint(0, nx_noise - 1)
-    y_off = random.randint(0, ny_noise - 1)
 
-    x_noise = (x_pt + x_off) % nx_noise
-    y_noise = (y_pt + y_off) % ny_noise
+def get_some_noise(
+    spectra: Spectra, noise: np.ndarray, x_pt: np.ndarray, y_pt: np.ndarray
+) -> np.ndarray:
+    """Retrieve some noise from spectra data."""
+    rng = np.random.default_rng()
+    rng.shuffle(noise)
+    nz_noise, ny_noise, nx_noise = noise.shape
+
+    x_off, y_off = rng.integers(0, nx_noise - 1), rng.integers(0, ny_noise - 1)
+    x_noise, y_noise = (x_pt + x_off) % nx_noise, (y_pt + y_off) % ny_noise
 
     return spectra.data[:, y_noise, x_noise].reshape((nz_noise, x_noise.size)).T
 
 
-def extract_noise_spectra(mc, spectra):
+def extract_noise_spectra(
+    mc: Sequence[int], spectra: Spectra
+) -> tuple[int, np.ndarray]:
+    """Extract noise spectra based on monte carlo parameters."""
     x1, x2, y1, y2, n_iter = mc
-
     x1_pt, x2_pt = sorted((spectra.ucx.i(x1), spectra.ucx.i(x2)))
     y1_pt, y2_pt = sorted((spectra.ucy.i(y1), spectra.ucy.i(y2)))
 
     noise = spectra.data[:, y1_pt:y2_pt, x1_pt:x2_pt]
     return n_iter, noise
 
 
-def calc_err_from_mc(params_list, heights_list):
+def calc_err_from_mc(
+    params_list: Sequence[dict], heights_list: np.ndarray
+) -> tuple[dict, np.ndarray]:
+    """Calculate errors from monte carlo simulations."""
     params_dict = {}
 
     for params_mc in params_list:
         for name, param in params_mc.items():
             params_dict.setdefault(name, []).append(param.value)
 
     params_err = {name: np.std(values) for name, values in params_dict.items()}
     height_err = np.std(heights_list, axis=0, ddof=1)
 
     return params_err, height_err
 
 
-def monte_carlo(mc, spectra, cluster, result, noise):
+def monte_carlo(
+    mc: Sequence[int],
+    spectra: Spectra,
+    cluster: Cluster,
+    result: lf.minimizer.MinimizerResult,
+    noise: float,
+) -> tuple[dict, np.ndarray]:
+    """Perform monte carlo simulation for error estimation."""
     n_iter, spectra_noise = extract_noise_spectra(mc, spectra)
-
     x_pt = np.rint(spectra.ucx.f(cluster.x, "ppm")).astype(int)
     y_pt = np.rint(spectra.ucy.f(cluster.y, "ppm")).astype(int)
 
     data_sim = simulate_data(result.params, cluster)
-
     mc_list = []
 
     for _ in range(int(n_iter)):
         data_noise = get_some_noise(spectra, spectra_noise, x_pt, y_pt)
         data_mc = data_sim + data_noise
         cluster_mc = Cluster(cluster.peaks, cluster.x, cluster.y, data_mc)
 
         params_mc = lf.minimize(
             residuals,
             result.params,
             args=(cluster_mc, noise),
             method="least_squares",
         ).params
 
-        _shapes, heights = calculate_shape_heights(params_mc, cluster_mc)
-
+        _, heights = calculate_shape_heights(params_mc, cluster_mc)
         mc_list.append((params_mc, heights))
 
     params_list, heights_list = zip(*mc_list, strict=False)
-
     params_err, height_err = calc_err_from_mc(params_list, heights_list)
 
     return params_err, height_err
 
 
-def run_fit(clargs, spectra, clusters):
+def run_fit(clargs, spectra: Spectra, clusters: Sequence[Cluster]) -> dict:
+    """Run the fitting process for all clusters."""
     print_fitting()
-
     shifts = {}
 
+    pdf = PdfPages(clargs.path_output / "clusters.pdf")
+
     for cluster in clusters:
         print_peaks(cluster.peaks)
-
         params = create_params(cluster.peaks, spectra, clargs)
 
         out = lf.minimize(
             residuals,
             params,
             args=(cluster, clargs.noise),
             method="least_squares",
@@ -198,49 +219,48 @@
         _, heights = calculate_shape_heights(out.params, cluster)
 
         print_fit_report(out)
 
         params_err = {param.name: param.stderr for param in out.params.values()}
         height_err = np.full_like(heights, clargs.noise)
 
+        plot_pdf(pdf, spectra, cluster, clargs.contour_level, out)
+
         shifts.update(
             {
-                peak.name: (out.params[f"p{i}_x0"].value, out.params[f"p{i}_y0"].value)
-                for i, peak in enumerate(cluster.peaks)
-            },
+                name: (out.params[f"p{i}_x0"].value, out.params[f"p{i}_y0"].value)
+                for i, name in enumerate(cluster.peaks["name"])
+            }
         )
 
-        # Monte-Carlo
         if clargs.mc and int(clargs.mc[4]) > 1:
             params_err, height_err = monte_carlo(
-                clargs.mc,
-                spectra,
-                cluster,
-                out,
-                clargs.noise,
+                clargs.mc, spectra, cluster, out, clargs.noise
             )
 
         write_profiles(
             clargs.path_output,
             spectra.z_values,
             cluster,
             out.params,
             heights,
             params_err,
             height_err,
         )
 
+    pdf.close()
+
     return shifts
 
 
-def write_shifts(names, shifts, file_shifts) -> None:
-    for name in names:
-        file_shifts.write(
-            f"{name:>15s} {shifts[name][1]:10.5f} {shifts[name][0]:10.5f}\n",
-        )
+def write_shifts(names: Sequence[str], shifts: dict, file_shifts: Path) -> None:
+    """Write the shifts to the output file."""
+    with file_shifts.open("w") as f:
+        for name in names:
+            f.write(f"{name:>15s} {shifts[name][1]:10.5f} {shifts[name][0]:10.5f}\n")
 
 
 def main() -> None:
     """Run peakfit."""
     print_logo()
 
     parser = build_parser()
@@ -251,34 +271,22 @@
     if clargs.noise is not None and clargs.noise < 0.0:
         clargs.noise = None
 
     if clargs.noise is None:
         clargs.noise = estimate_noise(spectra.data)
         print_estimated_noise(clargs.noise)
 
-    # Read peak list
-    lines = clargs.path_list.read_text().replace("Ass", "#").splitlines()
-    peaks = np.genfromtxt(
-        lines,
-        dtype=None,
-        encoding="utf-8",
-        names=("names", "y", "x"),
-    )
-
-    # Create the output directory
+    peaks = read_list(clargs.path_list, spectra)
     clargs.path_output.mkdir(parents=True, exist_ok=True)
 
-    # Cluster peaks
     if clargs.contour_level is None:
         clargs.contour_level = 5.0 * clargs.noise
-    clusters = cluster_peaks(spectra, peaks, clargs.contour_level)
 
+    clusters = cluster_peaks(spectra, peaks, clargs.contour_level)
     shifts = run_fit(clargs, spectra, clusters)
 
     export_html(clargs.path_output / "logs.html")
-
-    with (clargs.path_output / "shifts.list").open("w") as file_shifts:
-        write_shifts(peaks["names"], shifts, file_shifts)
+    write_shifts(peaks["name"], shifts, clargs.path_output / "shifts.list")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `peakfit-0.5.0/peakfit/plot_cest.py` & `peakfit-0.6.0/peakfit/plot_cest.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.5.0/peakfit/plot_cpmg.py` & `peakfit-0.6.0/peakfit/plot_cpmg.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.5.0/peakfit/plot_intensities.py` & `peakfit-0.6.0/peakfit/plot_intensities.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.5.0/peakfit/shapes.py` & `peakfit-0.6.0/peakfit/shapes.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,35 +9,43 @@
     return shapex * shapey
 
 
 def create_params(peaks, spectra, clargs):
     ucx = spectra.ucx
     ucy = spectra.ucy
 
+    nz, ny, nx = spectra.data.shape
+
+    hz2pt_x = abs(ucx.f(1, "hz") - ucx.f(0, "hz"))
+    hz2pt_y = abs(ucy.f(1, "hz") - ucy.f(0, "hz"))
+
     hz2ppm_x = abs(ucx.ppm(ucx.f(1, "hz")))
     hz2ppm_y = abs(ucy.ppm(ucy.f(1, "hz")))
 
     vary_position = not clargs.fixed
 
     params = lf.Parameters(usersyms={"ucx": ucx, "ucy": ucy})
 
-    for index, peak in enumerate(peaks):
+    for index, (x0_ppm, y0_ppm) in enumerate(peaks[["x0_ppm", "y0_ppm"]].values):
         pre = f"p{index}_"
 
-        x0, x0min, x0max = peak.x0 + np.array([0.0, -10.0, 10.0]) * hz2ppm_x
-        y0, y0min, y0max = peak.y0 + np.array([0.0, -10.0, 10.0]) * hz2ppm_y
+        x0, x0min, x0max = x0_ppm + np.array([0.0, -10.0, 10.0]) * hz2ppm_x
+        y0, y0min, y0max = y0_ppm + np.array([0.0, -10.0, 10.0]) * hz2ppm_y
 
         params.add(f"{pre}x0", value=x0, min=x0min, max=x0max, vary=vary_position)
         params.add(f"{pre}y0", value=y0, min=y0min, max=y0max, vary=vary_position)
 
+        params.add(f"{pre}x0_pt", expr=f"ucx.f({pre}x0, 'ppm') % {nx}")
+        params.add(f"{pre}y0_pt", expr=f"ucy.f({pre}y0, 'ppm') % {ny}")
+
         params.add(f"{pre}x_fwhm", value=15.0, min=0.1, max=200.0)
         params.add(f"{pre}y_fwhm", value=15.0, min=0.1, max=200.0)
 
-        params.add(f"{pre}x_fwhm_ppm", expr=f"{pre}x_fwhm * {hz2ppm_x}")
-        params.add(f"{pre}y_fwhm_ppm", expr=f"{pre}y_fwhm * {hz2ppm_y}")
+        params.add(f"{pre}x_fwhm_pt", expr=f"{pre}x_fwhm * {hz2pt_x}")
+        params.add(f"{pre}y_fwhm_pt", expr=f"{pre}y_fwhm * {hz2pt_y}")
 
         # By default, the shape is gaussian (eta = 0.0)
         if clargs.pvoigt:
             vary_eta = True
             value_eta = 0.5
         elif clargs.lorentzian:
             vary_eta = False
```

### Comparing `peakfit-0.5.0/pyproject.toml` & `peakfit-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 ]
 dependencies = [
     "numpy>=1.26.4",
     "lmfit>=1.3.1",
     "matplotlib>=3.9.0",
     "rich>=13.7.1",
     "nmrglue>=0.10",
+    "pandas>=2.2.2",
+    "scipy>=1.13.1",
+    "openpyxl>=3.1.2",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dynamic = []
-version = "0.5.0"
+version = "0.6.0"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.scripts]
 peakfit = "peakfit.peakfit:main"
 plot_cpmg = "peakfit.plot_cpmg:main"
```

