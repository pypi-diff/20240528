# Comparing `tmp/gradio_clickabletextbox-0.0.5.tar.gz` & `tmp/gradio_clickabletextbox-0.0.6.tar.gz`

## Comparing `gradio_clickabletextbox-0.0.5.tar` & `gradio_clickabletextbox-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/__init__.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/clickabletextbox.py
--rw-r--r--   0        0        0    37561 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/clickabletextbox.pyi
--rw-r--r--   0        0        0    97496 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/templates/component/index.js
--rw-r--r--   0        0        0    16051 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/templates/component/style.css
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/demo/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/demo/css.css
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/demo/requirements.txt
--rw-r--r--   0        0        0    10461 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/demo/space.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/frontend/Example.svelte
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/frontend/Index.svelte
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/frontend/gradio.config.js
--rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/frontend/package-lock.json
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/frontend/package.json
--rw-r--r--   0        0        0    15554 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/frontend/shared/Textbox.svelte
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/frontend/shared/transitions.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/.gitignore
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/README.md
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/__init__.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/clickabletextbox.py
+-rw-r--r--   0        0        0    37561 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/clickabletextbox.pyi
+-rw-r--r--   0        0        0    97509 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/component/index.js
+-rw-r--r--   0        0        0    16635 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/component/style.css
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/css.css
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/requirements.txt
+-rw-r--r--   0        0        0    10461 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/space.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/Example.svelte
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/Index.svelte
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/gradio.config.js
+-rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/package-lock.json
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/package.json
+-rw-r--r--   0        0        0    16137 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/shared/Textbox.svelte
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/shared/transitions.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/.gitignore
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/README.md
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/PKG-INFO
```

### Comparing `gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/clickabletextbox.py` & `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/clickabletextbox.py`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/clickabletextbox.pyi` & `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/clickabletextbox.pyi`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/templates/component/index.js` & `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/component/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     element: Tl,
     get_all_dirty_from_scope: Nl,
     get_slot_changes: Bl,
     get_spread_update: Al,
     init: Dl,
     insert: Il,
     safe_not_equal: jl,
-    set_dynamic_element_data: qt,
+    set_dynamic_element_data: Mt,
     set_style: U,
     toggle_class: fe,
     transition_in: _l,
     transition_out: cl,
     update_slot_base: Pl
 } = window.__gradio__svelte__internal;
 
@@ -49,15 +49,15 @@
     for (let r = 0; r < f.length; r += 1)
         a = Sl(a, f[r]);
     return {
         c() {
             e = Tl(
                 /*tag*/
                 l[14]
-            ), s && s.c(), qt(
+            ), s && s.c(), Mt(
                 /*tag*/
                 l[14]
             )(e, a), fe(
                 e,
                 "hidden",
                 /*visible*/
                 l[10] === !1
@@ -129,15 +129,15 @@
                         o,
                         null
                     ) : Nl(
                         /*$$scope*/
                         r[17]
                     ),
                     null
-                ), qt(
+                ), Mt(
                     /*tag*/
                     r[14]
                 )(e, a = Al(f, [
                     (!n || o & /*test_id*/
                         128) && {
                         "data-testid": (
                             /*test_id*/
@@ -282,43 +282,43 @@
     } = e, {
         explicit_call: v = !1
     } = e, {
         container: L = !0
     } = e, {
         visible: w = !0
     } = e, {
-        allow_overflow: V = !0
+        allow_overflow: H = !0
     } = e, {
         scale: b = null
     } = e, {
         min_width: h = 0
     } = e, p = c === "fieldset" ? "fieldset" : "div";
     const T = (k) => {
         if (k !== void 0) {
             if (typeof k == "number")
                 return k + "px";
             if (typeof k == "string")
                 return k;
         }
     };
     return l.$$set = (k) => {
-        "height" in k && t(0, s = k.height), "width" in k && t(1, f = k.width), "elem_id" in k && t(2, a = k.elem_id), "elem_classes" in k && t(3, r = k.elem_classes), "variant" in k && t(4, o = k.variant), "border_mode" in k && t(5, u = k.border_mode), "padding" in k && t(6, _ = k.padding), "type" in k && t(16, c = k.type), "test_id" in k && t(7, m = k.test_id), "explicit_call" in k && t(8, v = k.explicit_call), "container" in k && t(9, L = k.container), "visible" in k && t(10, w = k.visible), "allow_overflow" in k && t(11, V = k.allow_overflow), "scale" in k && t(12, b = k.scale), "min_width" in k && t(13, h = k.min_width), "$$scope" in k && t(17, i = k.$$scope);
+        "height" in k && t(0, s = k.height), "width" in k && t(1, f = k.width), "elem_id" in k && t(2, a = k.elem_id), "elem_classes" in k && t(3, r = k.elem_classes), "variant" in k && t(4, o = k.variant), "border_mode" in k && t(5, u = k.border_mode), "padding" in k && t(6, _ = k.padding), "type" in k && t(16, c = k.type), "test_id" in k && t(7, m = k.test_id), "explicit_call" in k && t(8, v = k.explicit_call), "container" in k && t(9, L = k.container), "visible" in k && t(10, w = k.visible), "allow_overflow" in k && t(11, H = k.allow_overflow), "scale" in k && t(12, b = k.scale), "min_width" in k && t(13, h = k.min_width), "$$scope" in k && t(17, i = k.$$scope);
     }, [
         s,
         f,
         a,
         r,
         o,
         u,
         _,
         m,
         v,
         L,
         w,
-        V,
+        H,
         b,
         h,
         p,
         T,
         c,
         i,
         n
@@ -426,15 +426,15 @@
 class an extends Xl {
     constructor(e) {
         super(), $l(this, e, on, fn, tn, {});
     }
 }
 const {
     SvelteComponent: rn,
-    attr: Mt,
+    attr: Vt,
     check_outros: un,
     create_component: _n,
     create_slot: cn,
     destroy_component: dn,
     detach: Ue,
     element: mn,
     empty: hn,
@@ -447,23 +447,23 @@
     safe_not_equal: pn,
     set_data: Cn,
     space: yn,
     text: Ln,
     toggle_class: Le,
     transition_in: De,
     transition_out: Ge,
-    update_slot_base: qn
+    update_slot_base: Mn
 } = window.__gradio__svelte__internal;
 
-function Vt(l) {
+function Ht(l) {
     let e, t;
     return e = new an({
         props: {
             $$slots: {
-                default: [Mn]
+                default: [Vn]
             },
             $$scope: {
                 ctx: l
             }
         }
     }), {
         c() {
@@ -488,15 +488,15 @@
         },
         d(n) {
             dn(e, n);
         }
     };
 }
 
-function Mn(l) {
+function Vn(l) {
     let e;
     return {
         c() {
             e = Ln(
                 /*info*/
                 l[1]
             );
@@ -514,48 +514,48 @@
         },
         d(t) {
             t && Ue(e);
         }
     };
 }
 
-function Vn(l) {
+function Hn(l) {
     let e, t, n, i;
     const s = (
             /*#slots*/
             l[2].default
         ),
         f = cn(
             s,
             l,
             /*$$scope*/
             l[3],
             null
         );
     let a = (
         /*info*/
-        l[1] && Vt(l)
+        l[1] && Ht(l)
     );
     return {
         c() {
-            e = mn("span"), f && f.c(), t = yn(), a && a.c(), n = hn(), Mt(e, "data-testid", "block-info"), Mt(e, "class", "svelte-22c38v"), Le(e, "sr-only", ! /*show_label*/
+            e = mn("span"), f && f.c(), t = yn(), a && a.c(), n = hn(), Vt(e, "data-testid", "block-info"), Vt(e, "class", "svelte-22c38v"), Le(e, "sr-only", ! /*show_label*/
                 l[0]), Le(e, "hide", ! /*show_label*/
                 l[0]), Le(
                 e,
                 "has-info",
                 /*info*/
                 l[1] != null
             );
         },
         m(r, o) {
             Xe(r, e, o), f && f.m(e, null), Xe(r, t, o), a && a.m(r, o), Xe(r, n, o), i = !0;
         },
         p(r, [o]) {
             f && f.p && (!i || o & /*$$scope*/
-                    8) && qn(
+                    8) && Mn(
                     f,
                     s,
                     r,
                     /*$$scope*/
                     r[3],
                     i ? gn(
                         s,
@@ -576,15 +576,15 @@
                     2) && Le(
                     e,
                     "has-info",
                     /*info*/
                     r[1] != null
                 ), /*info*/
                 r[1] ? a ? (a.p(r, o), o & /*info*/
-                    2 && De(a, 1)) : (a = Vt(r), a.c(), De(a, 1), a.m(n.parentNode, n)) : a && (wn(), Ge(a, 1, 1, () => {
+                    2 && De(a, 1)) : (a = Ht(r), a.c(), De(a, 1), a.m(n.parentNode, n)) : a && (wn(), Ge(a, 1, 1, () => {
                     a = null;
                 }), un());
         },
         i(r) {
             i || (De(f, r), De(a), i = !0);
         },
         o(r) {
@@ -592,30 +592,30 @@
         },
         d(r) {
             r && (Ue(e), Ue(t), Ue(n)), f && f.d(r), a && a.d(r);
         }
     };
 }
 
-function Hn(l, e, t) {
+function qn(l, e, t) {
     let {
         $$slots: n = {},
         $$scope: i
     } = e, {
         show_label: s = !0
     } = e, {
         info: f = void 0
     } = e;
     return l.$$set = (a) => {
         "show_label" in a && t(0, s = a.show_label), "info" in a && t(1, f = a.info), "$$scope" in a && t(3, i = a.$$scope);
     }, [s, f, n, i];
 }
 class Fn extends rn {
     constructor(e) {
-        super(), vn(this, e, Hn, Vn, pn, {
+        super(), vn(this, e, qn, Hn, pn, {
             show_label: 0,
             info: 1
         });
     }
 }
 const {
     SvelteComponent: Zn,
@@ -628,23 +628,23 @@
     element: ct,
     init: Tn,
     insert: ml,
     listen: Nn,
     mount_component: Bn,
     safe_not_equal: An,
     set_data: Dn,
-    set_style: qe,
+    set_style: Me,
     space: In,
     text: jn,
     toggle_class: j,
     transition_in: Pn,
     transition_out: Yn
 } = window.__gradio__svelte__internal;
 
-function Ht(l) {
+function qt(l) {
     let e, t;
     return {
         c() {
             e = ct("span"), t = jn(
                 /*label*/
                 l[1]
             ), _e(e, "class", "svelte-1lrphxw");
@@ -665,15 +665,15 @@
         }
     };
 }
 
 function Kn(l) {
     let e, t, n, i, s, f, a, r = (
         /*show_label*/
-        l[2] && Ht(l)
+        l[2] && qt(l)
     );
     return i = new /*Icon*/
     l[0]({}), {
         c() {
             e = ct("button"), r && r.c(), t = In(), n = ct("div"), zn(i.$$.fragment), _e(n, "class", "svelte-1lrphxw"), j(
                     n,
                     "small",
@@ -721,24 +721,24 @@
                     /*highlight*/
                     l[6]
                 ), j(
                     e,
                     "transparent",
                     /*transparent*/
                     l[9]
-                ), qe(e, "color", ! /*disabled*/
+                ), Me(e, "color", ! /*disabled*/
                     l[7] && /*_color*/
                     l[12] ? (
                         /*_color*/
                         l[12]
-                    ) : "var(--block-label-text-color)"), qe(e, "--bg-color", /*disabled*/
+                    ) : "var(--block-label-text-color)"), Me(e, "--bg-color", /*disabled*/
                     l[7] ? "auto" : (
                         /*background*/
                         l[10]
-                    )), qe(
+                    )), Me(
                     e,
                     "margin-left",
                     /*offset*/
                     l[11] + "px"
                 );
         },
         m(o, u) {
@@ -747,15 +747,15 @@
                 "click",
                 /*click_handler*/
                 l[14]
             ), f = !0);
         },
         p(o, [u]) {
             /*show_label*/
-            o[2] ? r ? r.p(o, u) : (r = Ht(o), r.c(), r.m(e, t)) : r && (r.d(1), r = null), (!s || u & /*size*/
+            o[2] ? r ? r.p(o, u) : (r = qt(o), r.c(), r.m(e, t)) : r && (r.d(1), r = null), (!s || u & /*size*/
                     16) && j(
                     n,
                     "small",
                     /*size*/
                     o[4] === "small"
                 ), (!s || u & /*size*/
                     16) && j(
@@ -810,26 +810,26 @@
                 ), (!s || u & /*transparent*/
                     512) && j(
                     e,
                     "transparent",
                     /*transparent*/
                     o[9]
                 ), u & /*disabled, _color*/
-                4224 && qe(e, "color", ! /*disabled*/
+                4224 && Me(e, "color", ! /*disabled*/
                     o[7] && /*_color*/
                     o[12] ? (
                         /*_color*/
                         o[12]
                     ) : "var(--block-label-text-color)"), u & /*disabled, background*/
-                1152 && qe(e, "--bg-color", /*disabled*/
+                1152 && Me(e, "--bg-color", /*disabled*/
                     o[7] ? "auto" : (
                         /*background*/
                         o[10]
                     )), u & /*offset*/
-                2048 && qe(
+                2048 && Me(
                     e,
                     "margin-left",
                     /*offset*/
                     o[11] + "px"
                 );
         },
         i(o) {
@@ -881,15 +881,15 @@
         {
             background: L = "var(--background-fill-primary)"
         } = e,
         {
             offset: w = 0
         } = e;
 
-    function V(b) {
+    function H(b) {
         Sn.call(this, l, b);
     }
     return l.$$set = (b) => {
         "Icon" in b && t(0, i = b.Icon), "label" in b && t(1, s = b.label), "show_label" in b && t(2, f = b.show_label), "pending" in b && t(3, a = b.pending), "size" in b && t(4, r = b.size), "padded" in b && t(5, o = b.padded), "highlight" in b && t(6, u = b.highlight), "disabled" in b && t(7, _ = b.disabled), "hasPopup" in b && t(8, c = b.hasPopup), "color" in b && t(13, m = b.color), "transparent" in b && t(9, v = b.transparent), "background" in b && t(10, L = b.background), "offset" in b && t(11, w = b.offset);
     }, l.$$.update = () => {
         l.$$.dirty & /*highlight, color*/
             8256 && t(12, n = u ? "var(--color-accent)" : m);
@@ -904,15 +904,15 @@
         _,
         c,
         v,
         L,
         w,
         n,
         m,
-        V
+        H
     ];
 }
 class Un extends Zn {
     constructor(e) {
         super(), Tn(this, e, On, Kn, An, {
             Icon: 0,
             label: 1,
@@ -1344,29 +1344,29 @@
     };
 }
 
 function li(l) {
     const e = l - 1;
     return e * e * e + 1;
 }
-const Me = [];
+const Ve = [];
 
 function ni(l, e = Re) {
     let t;
     const n = /* @__PURE__ */ new Set();
 
     function i(a) {
         if (ei(l, a) && (l = a, t)) {
-            const r = !Me.length;
+            const r = !Ve.length;
             for (const o of n)
-                o[1](), Me.push(o, l);
+                o[1](), Ve.push(o, l);
             if (r) {
-                for (let o = 0; o < Me.length; o += 2)
-                    Me[o][0](Me[o + 1]);
-                Me.length = 0;
+                for (let o = 0; o < Ve.length; o += 2)
+                    Ve[o][0](Ve[o + 1]);
+                Ve.length = 0;
             }
         }
     }
 
     function s(a) {
         i(a(l));
     }
@@ -1421,18 +1421,18 @@
         } = e;
     let f, a, r, o = l,
         u = l,
         _ = 1,
         c = 0,
         m = !1;
 
-    function v(w, V = {}) {
+    function v(w, H = {}) {
         u = w;
         const b = r = {};
-        return l == null || V.hard || L.stiffness >= 1 && L.damping >= 1 ? (m = !0, f = Zt(), o = w, t.set(l = u), Promise.resolve()) : (V.soft && (c = 1 / ((V.soft === !0 ? 0.5 : +V.soft) * 60), _ = 0), a || (f = Zt(), m = !1, a = ti((h) => {
+        return l == null || H.hard || L.stiffness >= 1 && L.damping >= 1 ? (m = !0, f = Zt(), o = w, t.set(l = u), Promise.resolve()) : (H.soft && (c = 1 / ((H.soft === !0 ? 0.5 : +H.soft) * 60), _ = 0), a || (f = Zt(), m = !1, a = ti((h) => {
             if (m)
                 return m = !1, a = null, !1;
             _ = Math.min(_ + c, 1);
             const p = {
                     inv_mass: _,
                     opts: L,
                     settled: !0,
@@ -1444,15 +1444,15 @@
             a.promise.then(() => {
                 b === r && h();
             });
         }));
     }
     const L = {
         set: v,
-        update: (w, V) => v(w(u, l), V),
+        update: (w, H) => v(w(u, l), H),
         subscribe: t.subscribe,
         stiffness: n,
         damping: i,
         precision: s
     };
     return L;
 }
@@ -1482,15 +1482,15 @@
 const {
     SvelteComponent: si,
     action_destroyer: gt,
     add_render_callback: fi,
     append: F,
     attr: y,
     binding_callbacks: at,
-    bubble: Ve,
+    bubble: He,
     create_component: oi,
     create_in_transition: ai,
     destroy_component: ri,
     destroy_each: wl,
     detach: te,
     element: z,
     ensure_array_like: We,
@@ -1552,15 +1552,15 @@
     };
 }
 
 function wi(l) {
     let e, t, n, i, s, f;
     return {
         c() {
-            e = z("textarea"), y(e, "data-testid", "textbox"), y(e, "class", "scroll-hide svelte-8lpwqk"), y(e, "dir", t = /*rtl*/
+            e = z("textarea"), y(e, "data-testid", "textbox"), y(e, "class", "scroll-hide svelte-ak29na"), y(e, "dir", t = /*rtl*/
                     l[10] ? "rtl" : "ltr"), y(
                     e,
                     "placeholder",
                     /*placeholder*/
                     l[2]
                 ), y(
                     e,
@@ -1667,30 +1667,30 @@
     };
 }
 
 function vi(l) {
     let e, t, n, i, s, f, a, r, o;
     return {
         c() {
-            e = z("div"), t = z("textarea"), f = ne(), a = z("button"), a.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-8lpwqk"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#CCCCCC" class="svelte-8lpwqk"></path></svg>', y(t, "data-testid", "textbox"), y(t, "class", "scroll-hide svelte-8lpwqk"), y(t, "dir", n = /*rtl*/
+            e = z("div"), t = z("textarea"), f = ne(), a = z("button"), a.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-ak29na"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#CCCCCC" class="svelte-ak29na"></path></svg>', y(t, "data-testid", "textbox"), y(t, "class", "scroll-hide svelte-ak29na"), y(t, "dir", n = /*rtl*/
                     l[10] ? "rtl" : "ltr"), y(
                     t,
                     "placeholder",
                     /*placeholder*/
                     l[2]
                 ), y(
                     t,
                     "rows",
                     /*lines*/
                     l[1]
                 ), t.disabled = /*disabled*/
                 l[5], t.autofocus = /*autofocus*/
                 l[11], y(t, "style", i = /*text_align*/
                     l[12] ? "text-align: " + /*text_align*/
-                    l[12] : ""), y(a, "class", "extend_button svelte-8lpwqk"), y(a, "aria-label", "Extend"), y(a, "aria-roledescription", "Extend text"), y(e, "class", "magic_container svelte-8lpwqk");
+                    l[12] : ""), y(a, "class", "extend_button svelte-ak29na"), y(a, "aria-label", "Extend"), y(a, "aria-roledescription", "Extend text"), y(e, "class", "magic_container svelte-ak29na");
         },
         m(u, _) {
             le(u, e, _), F(e, t), ze(
                     t,
                     /*value*/
                     l[0]
                 ), l[40](t), F(e, f), F(e, a), /*autofocus*/
@@ -1795,37 +1795,37 @@
         ),
         L = (
             /*suffixes*/
             l[9].length > 0 && It(l)
         );
     return {
         c() {
-            e = z("div"), t = z("textarea"), f = ne(), a = z("button"), a.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-8lpwqk"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#ff6700" class="svelte-8lpwqk"></path></svg>', r = ne(), o = z("div"), v && v.c(), u = ne(), L && L.c(), y(t, "data-testid", "textbox"), y(t, "class", "scroll-hide svelte-8lpwqk"), y(t, "dir", n = /*rtl*/
+            e = z("div"), t = z("textarea"), f = ne(), a = z("button"), a.innerHTML = '<svg width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg" class="svelte-ak29na"><path d="M23.0978 15.6987L23.5777 15.2188L21.7538 13.3952L21.2739 13.8751L23.0978 15.6987ZM11.1253 2.74873L10.6454 3.22809L12.4035 4.98733L12.8834 4.50769L11.1253 2.74873ZM25.5996 9.23801H22.885V9.91673H25.5996V9.23801ZM10.6692 9.23801H7.95457V9.91673H10.6692V9.23801ZM21.8008 5.01533L23.5982 3.21773L23.118 2.73781L21.3206 4.53541L21.8008 5.01533ZM17.2391 7.29845L18.6858 8.74521C18.7489 8.80822 18.7989 8.88303 18.8331 8.96538C18.8672 9.04773 18.8847 9.13599 18.8847 9.22513C18.8847 9.31427 18.8672 9.40254 18.8331 9.48488C18.7989 9.56723 18.7489 9.64205 18.6858 9.70505L3.00501 25.3859C2.74013 25.6511 2.31061 25.6511 2.04517 25.3859L0.598406 23.9391C0.535351 23.8761 0.485329 23.8013 0.4512 23.719C0.417072 23.6366 0.399506 23.5483 0.399506 23.4592C0.399506 23.3701 0.417072 23.2818 0.4512 23.1995C0.485329 23.1171 0.535351 23.0423 0.598406 22.9793L16.2792 7.29845C16.3422 7.23533 16.417 7.18525 16.4994 7.15108C16.5817 7.11691 16.67 7.09932 16.7592 7.09932C16.8483 7.09932 16.9366 7.11691 17.019 7.15108C17.1013 7.18525 17.1761 7.23533 17.2391 7.29845ZM14.4231 13.2042L18.3792 9.24893L16.746 7.61541L12.7899 11.5713L14.4231 13.2042ZM17.4555 0.415771H16.7768V3.13037H17.4555V0.415771ZM17.4555 15.3462H16.7768V18.0608H17.4555V15.3462Z" fill="#ff6700" class="svelte-ak29na"></path></svg>', r = ne(), o = z("div"), v && v.c(), u = ne(), L && L.c(), y(t, "data-testid", "textbox"), y(t, "class", "scroll-hide svelte-ak29na"), y(t, "dir", n = /*rtl*/
                     l[10] ? "rtl" : "ltr"), y(
                     t,
                     "placeholder",
                     /*placeholder*/
                     l[2]
                 ), y(
                     t,
                     "rows",
                     /*lines*/
                     l[1]
                 ), t.disabled = /*disabled*/
                 l[5], t.autofocus = /*autofocus*/
                 l[11], y(t, "style", i = /*text_align*/
                     l[12] ? "text-align: " + /*text_align*/
-                    l[12] : ""), y(a, "class", "extend_button svelte-8lpwqk"), y(a, "aria-label", "Extend"), y(a, "aria-roledescription", "Extend text"), y(e, "class", "magic_container svelte-8lpwqk"), y(o, "class", "menu svelte-8lpwqk");
+                    l[12] : ""), y(a, "class", "extend_button svelte-ak29na"), y(a, "aria-label", "Extend"), y(a, "aria-roledescription", "Extend text"), y(e, "class", "magic_container svelte-ak29na"), y(o, "class", "menu svelte-ak29na");
         },
-        m(w, V) {
-            le(w, e, V), F(e, t), ze(
+        m(w, H) {
+            le(w, e, H), F(e, t), ze(
                     t,
                     /*value*/
                     l[0]
-                ), l[34](t), F(e, f), F(e, a), le(w, r, V), le(w, o, V), v && v.m(o, null), F(o, u), L && L.m(o, null), /*autofocus*/
+                ), l[34](t), F(e, f), F(e, a), le(w, r, H), le(w, o, H), v && v.m(o, null), F(o, u), L && L.m(o, null), /*autofocus*/
                 l[11] && t.focus(), c || (m = [
                     gt(s = /*text_area_resize*/
                         l[23].call(
                             null,
                             t,
                             /*value*/
                             l[0]
@@ -1882,49 +1882,49 @@
                         o,
                         "transitionend",
                         /*transitionend_handler*/
                         l[38]
                     )
                 ], c = !0);
         },
-        p(w, V) {
-            V[0] & /*rtl*/
+        p(w, H) {
+            H[0] & /*rtl*/
                 1024 && n !== (n = /*rtl*/
-                    w[10] ? "rtl" : "ltr") && y(t, "dir", n), V[0] & /*placeholder*/
+                    w[10] ? "rtl" : "ltr") && y(t, "dir", n), H[0] & /*placeholder*/
                 4 && y(
                     t,
                     "placeholder",
                     /*placeholder*/
                     w[2]
-                ), V[0] & /*lines*/
+                ), H[0] & /*lines*/
                 2 && y(
                     t,
                     "rows",
                     /*lines*/
                     w[1]
-                ), V[0] & /*disabled*/
+                ), H[0] & /*disabled*/
                 32 && (t.disabled = /*disabled*/
-                    w[5]), V[0] & /*autofocus*/
+                    w[5]), H[0] & /*autofocus*/
                 2048 && (t.autofocus = /*autofocus*/
-                    w[11]), V[0] & /*text_align*/
+                    w[11]), H[0] & /*text_align*/
                 4096 && i !== (i = /*text_align*/
                     w[12] ? "text-align: " + /*text_align*/
-                    w[12] : "") && y(t, "style", i), s && wt(s.update) && V[0] & /*value*/
+                    w[12] : "") && y(t, "style", i), s && wt(s.update) && H[0] & /*value*/
                 1 && s.update.call(
                     null,
                     /*value*/
                     w[0]
-                ), V[0] & /*value*/
+                ), H[0] & /*value*/
                 1 && ze(
                     t,
                     /*value*/
                     w[0]
                 ), /*prompts*/
-                w[8].length > 0 ? v ? v.p(w, V) : (v = At(w), v.c(), v.m(o, u)) : v && (v.d(1), v = null), /*suffixes*/
-                w[9].length > 0 ? L ? L.p(w, V) : (L = It(w), L.c(), L.m(o, null)) : L && (L.d(1), L = null);
+                w[8].length > 0 ? v ? v.p(w, H) : (v = At(w), v.c(), v.m(o, u)) : v && (v.d(1), v = null), /*suffixes*/
+                w[9].length > 0 ? L ? L.p(w, H) : (L = It(w), L.c(), L.m(o, null)) : L && (L.d(1), L = null);
         },
         i(w) {
             w && (_ || fi(() => {
                 _ = ai(o, ii, {
                     duration: 500
                 }), _.start();
             }));
@@ -1945,15 +1945,15 @@
     for (let a = 0; a < s.length; a += 1)
         f[a] = Dt(Bt(l, s, a));
     return {
         c() {
             e = z("div"), t = z("span"), t.textContent = "A few prompt inspirations", n = ne(), i = z("ul");
             for (let a = 0; a < f.length; a += 1)
                 f[a].c();
-            y(i, "class", "svelte-8lpwqk"), y(e, "class", "menu_section svelte-8lpwqk");
+            y(i, "class", "svelte-ak29na"), y(e, "class", "menu_section_prompt svelte-ak29na");
         },
         m(a, r) {
             le(a, e, r), F(e, t), F(e, n), F(e, i);
             for (let o = 0; o < f.length; o += 1)
                 f[o] && f[o].m(i, null);
         },
         p(a, r) {
@@ -1993,15 +1993,15 @@
                 /*word*/
                 l[51]
             )
         );
     }
     return {
         c() {
-            e = z("li"), t = z("button"), n = z("div"), s = pt(i), f = ne(), a = z("div"), a.innerHTML = '<svg xmlns="http://www.w3.org/2000/svg" width="11" height="12" viewBox="0 0 11 12" fill="none" class="svelte-8lpwqk"><path d="M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z" fill="#FF9A57" class="svelte-8lpwqk"></path></svg>', r = ne(), y(t, "class", "text_extension_button_prompt svelte-8lpwqk"), y(e, "class", "svelte-8lpwqk");
+            e = z("li"), t = z("button"), n = z("div"), s = pt(i), f = ne(), a = z("div"), a.innerHTML = '<svg xmlns="http://www.w3.org/2000/svg" width="11" height="12" viewBox="0 0 11 12" fill="none" class="svelte-ak29na"><path d="M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z" fill="#FF9A57" class="svelte-ak29na"></path></svg>', r = ne(), y(t, "class", "text_extension_button_prompt svelte-ak29na"), y(e, "class", "svelte-ak29na");
         },
         m(c, m) {
             le(c, e, m), F(e, t), F(t, n), F(n, s), F(t, f), F(t, a), F(e, r), o || (u = S(t, "click", _), o = !0);
         },
         p(c, m) {
             l = c, m[0] & /*prompts*/
                 256 && i !== (i = /*word*/
@@ -2022,15 +2022,15 @@
     for (let a = 0; a < s.length; a += 1)
         f[a] = jt(Nt(l, s, a));
     return {
         c() {
             e = z("div"), t = z("span"), t.textContent = "Add keywords to guide style", n = ne(), i = z("ul");
             for (let a = 0; a < f.length; a += 1)
                 f[a].c();
-            y(i, "class", "svelte-8lpwqk"), y(e, "class", "menu_section svelte-8lpwqk");
+            y(i, "class", "svelte-ak29na"), y(e, "class", "menu_section_style svelte-ak29na");
         },
         m(a, r) {
             le(a, e, r), F(e, t), F(e, n), F(e, i);
             for (let o = 0; o < f.length; o += 1)
                 f[o] && f[o].m(i, null);
         },
         p(a, r) {
@@ -2070,15 +2070,15 @@
                 /*word*/
                 l[51]
             )
         );
     }
     return {
         c() {
-            e = z("li"), t = z("button"), n = z("div"), s = pt(i), f = ne(), a = z("div"), a.innerHTML = '<svg xmlns="http://www.w3.org/2000/svg" width="11" height="12" viewBox="0 0 11 12" fill="none" class="svelte-8lpwqk"><path d="M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z" fill="#FF9A57" class="svelte-8lpwqk"></path></svg>', r = ne(), y(t, "class", "text_extension_button svelte-8lpwqk"), y(e, "class", "svelte-8lpwqk");
+            e = z("li"), t = z("button"), n = z("div"), s = pt(i), f = ne(), a = z("div"), a.innerHTML = '<svg xmlns="http://www.w3.org/2000/svg" width="11" height="12" viewBox="0 0 11 12" fill="none" class="svelte-ak29na"><path d="M8.70801 5.51112H5.95801V2.57779C5.95801 2.44813 5.90972 2.32377 5.82376 2.23209C5.73781 2.14041 5.62123 2.0889 5.49967 2.0889C5.37812 2.0889 5.26154 2.14041 5.17558 2.23209C5.08963 2.32377 5.04134 2.44813 5.04134 2.57779V5.51112H2.29134C2.16978 5.51112 2.0532 5.56263 1.96725 5.65431C1.8813 5.746 1.83301 5.87035 1.83301 6.00001C1.83301 6.12967 1.8813 6.25402 1.96725 6.34571C2.0532 6.43739 2.16978 6.4889 2.29134 6.4889H5.04134V9.42223C5.04134 9.55189 5.08963 9.67624 5.17558 9.76793C5.26154 9.85961 5.37812 9.91112 5.49967 9.91112C5.62123 9.91112 5.73781 9.85961 5.82376 9.76793C5.90972 9.67624 5.95801 9.55189 5.95801 9.42223V6.4889H8.70801C8.82956 6.4889 8.94614 6.43739 9.0321 6.34571C9.11805 6.25402 9.16634 6.12967 9.16634 6.00001C9.16634 5.87035 9.11805 5.746 9.0321 5.65431C8.94614 5.56263 8.82956 5.51112 8.70801 5.51112Z" fill="#FF9A57" class="svelte-ak29na"></path></svg>', r = ne(), y(t, "class", "text_extension_button svelte-ak29na"), y(e, "class", "svelte-ak29na");
         },
         m(c, m) {
             le(c, e, m), F(e, t), F(t, n), F(n, s), F(t, f), F(t, a), F(e, r), o || (u = S(t, "click", _), o = !0);
         },
         p(c, m) {
             l = c, m[0] & /*suffixes*/
                 512 && i !== (i = /*word*/
@@ -2126,15 +2126,15 @@
             o[15])
             return wi;
     }
     let a = f(l),
         r = a && a(l);
     return {
         c() {
-            e = z("label"), oi(t.$$.fragment), n = ne(), i = z("div"), r && r.c(), y(i, "class", "input-container"), y(e, "class", "svelte-8lpwqk"), Et(
+            e = z("label"), oi(t.$$.fragment), n = ne(), i = z("div"), r && r.c(), y(i, "class", "input-container"), y(e, "class", "svelte-ak29na"), Et(
                 e,
                 "container",
                 /*container*/
                 l[7]
             );
         },
         m(o, u) {
@@ -2175,15 +2175,15 @@
     var n = this && this.__awaiter || function(d, A, O, D) {
         function me(Ae) {
             return Ae instanceof O ? Ae : new O(function(Pe) {
                 Pe(Ae);
             });
         }
         return new(O || (O = Promise))(function(Ae, Pe) {
-            function Hl(he) {
+            function ql(he) {
                 try {
                     it(D.next(he));
                 } catch (st) {
                     Pe(st);
                 }
             }
 
@@ -2192,15 +2192,15 @@
                     it(D.throw(he));
                 } catch (st) {
                     Pe(st);
                 }
             }
 
             function it(he) {
-                he.done ? Ae(he.value) : me(he.value).then(Hl, Fl);
+                he.done ? Ae(he.value) : me(he.value).then(ql, Fl);
             }
             it((D = D.apply(d, A || [])).next());
         });
     };
     let {
         value: i = ""
     } = e, {
@@ -2224,15 +2224,15 @@
     } = e, {
         prompts: v = []
     } = e, {
         suffixes: L = []
     } = e, {
         rtl: w = !1
     } = e, {
-        autofocus: V = !1
+        autofocus: H = !1
     } = e, {
         text_align: b = void 0
     } = e, {
         autoscroll: h = !0
     } = e, p, T = !1, k, N = 0, B = !1, P = !1, Y = !P && (v.length > 0 || L.length > 0);
     const I = bi();
     mi(() => {
@@ -2242,15 +2242,15 @@
         k && h && !B && p.scrollTo(0, p.scrollHeight);
     };
 
     function ge() {
         I("change", i), s || I("input");
     }
     hi(() => {
-        V && p.focus(), k && h && ie(), t(24, s = !1), t(16, Y = !P && (v.length > 0 || L.length > 0));
+        H && p.focus(), k && h && ie(), t(24, s = !1), t(16, Y = !P && (v.length > 0 || L.length > 0));
     });
 
     function W() {
         return n(this, void 0, void 0, function*() {
             t(14, T = !T);
         });
     }
@@ -2306,35 +2306,35 @@
                 target: d
             }), {
                 destroy: () => d.removeEventListener("input", g)
             };
     }
 
     function Qe(d) {
-        Ve.call(this, l, d);
+        He.call(this, l, d);
     }
 
     function xe(d) {
-        Ve.call(this, l, d);
+        He.call(this, l, d);
     }
 
     function $e(d) {
-        Ve.call(this, l, d);
+        He.call(this, l, d);
     }
 
     function C(d) {
-        Ve.call(this, l, d);
+        He.call(this, l, d);
     }
 
     function et(d) {
-        Ve.call(this, l, d);
+        He.call(this, l, d);
     }
 
     function pe(d) {
-        Ve.call(this, l, d);
+        He.call(this, l, d);
     }
 
     function Ce() {
         i = this.value, t(0, i);
     }
 
     function tt(d) {
@@ -2357,21 +2357,21 @@
         });
     }
 
     function Be() {
         i = this.value, t(0, i);
     }
 
-    function Vl(d) {
+    function Hl(d) {
         at[d ? "unshift" : "push"](() => {
             p = d, t(13, p);
         });
     }
     return l.$$set = (d) => {
-        "value" in d && t(0, i = d.value), "value_is_output" in d && t(24, s = d.value_is_output), "lines" in d && t(1, f = d.lines), "placeholder" in d && t(2, a = d.placeholder), "label" in d && t(3, r = d.label), "info" in d && t(4, o = d.info), "disabled" in d && t(5, u = d.disabled), "show_label" in d && t(6, _ = d.show_label), "container" in d && t(7, c = d.container), "max_lines" in d && t(25, m = d.max_lines), "prompts" in d && t(8, v = d.prompts), "suffixes" in d && t(9, L = d.suffixes), "rtl" in d && t(10, w = d.rtl), "autofocus" in d && t(11, V = d.autofocus), "text_align" in d && t(12, b = d.text_align), "autoscroll" in d && t(26, h = d.autoscroll);
+        "value" in d && t(0, i = d.value), "value_is_output" in d && t(24, s = d.value_is_output), "lines" in d && t(1, f = d.lines), "placeholder" in d && t(2, a = d.placeholder), "label" in d && t(3, r = d.label), "info" in d && t(4, o = d.info), "disabled" in d && t(5, u = d.disabled), "show_label" in d && t(6, _ = d.show_label), "container" in d && t(7, c = d.container), "max_lines" in d && t(25, m = d.max_lines), "prompts" in d && t(8, v = d.prompts), "suffixes" in d && t(9, L = d.suffixes), "rtl" in d && t(10, w = d.rtl), "autofocus" in d && t(11, H = d.autofocus), "text_align" in d && t(12, b = d.text_align), "autoscroll" in d && t(26, h = d.autoscroll);
     }, l.$$.update = () => {
         l.$$.dirty[0] & /*value*/
             1 && i === null && t(0, i = ""), l.$$.dirty[0] & /*value, el, lines, max_lines*/
             33562627 && p && f !== m && g({
                 target: p
             }), l.$$.dirty[0] & /*value*/
             1 && ge();
@@ -2383,15 +2383,15 @@
         o,
         u,
         _,
         c,
         v,
         L,
         w,
-        V,
+        H,
         b,
         p,
         T,
         P,
         Y,
         W,
         se,
@@ -2414,15 +2414,15 @@
         de,
         ye,
         lt,
         nt,
         Ne,
         ue,
         Be,
-        Vl
+        Hl
     ];
 }
 class yi extends si {
     constructor(e) {
         super(), ui(
             this,
             e,
@@ -2459,46 +2459,46 @@
         l /= 1e3, t++;
     let n = e[t];
     return (Number.isInteger(l) ? l : l.toFixed(1)) + n;
 }
 const {
     SvelteComponent: Li,
     append: Q,
-    attr: H,
+    attr: q,
     component_subscribe: Pt,
-    detach: qi,
-    element: Mi,
-    init: Vi,
-    insert: Hi,
+    detach: Mi,
+    element: Vi,
+    init: Hi,
+    insert: qi,
     noop: Yt,
     safe_not_equal: Fi,
     set_style: Ke,
     svg_element: x,
     toggle_class: Kt
 } = window.__gradio__svelte__internal, {
     onMount: Zi
 } = window.__gradio__svelte__internal;
 
 function Si(l) {
     let e, t, n, i, s, f, a, r, o, u, _, c;
     return {
         c() {
-            e = Mi("div"), t = x("svg"), n = x("g"), i = x("path"), s = x("path"), f = x("path"), a = x("path"), r = x("g"), o = x("path"), u = x("path"), _ = x("path"), c = x("path"), H(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), H(i, "fill", "#FF7C00"), H(i, "fill-opacity", "0.4"), H(i, "class", "svelte-43sxxs"), H(s, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), H(s, "fill", "#FF7C00"), H(s, "class", "svelte-43sxxs"), H(f, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), H(f, "fill", "#FF7C00"), H(f, "fill-opacity", "0.4"), H(f, "class", "svelte-43sxxs"), H(a, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), H(a, "fill", "#FF7C00"), H(a, "class", "svelte-43sxxs"), Ke(n, "transform", "translate(" + /*$top*/
+            e = Vi("div"), t = x("svg"), n = x("g"), i = x("path"), s = x("path"), f = x("path"), a = x("path"), r = x("g"), o = x("path"), u = x("path"), _ = x("path"), c = x("path"), q(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(i, "fill", "#FF7C00"), q(i, "fill-opacity", "0.4"), q(i, "class", "svelte-43sxxs"), q(s, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(s, "fill", "#FF7C00"), q(s, "class", "svelte-43sxxs"), q(f, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(f, "fill", "#FF7C00"), q(f, "fill-opacity", "0.4"), q(f, "class", "svelte-43sxxs"), q(a, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(a, "fill", "#FF7C00"), q(a, "class", "svelte-43sxxs"), Ke(n, "transform", "translate(" + /*$top*/
                 l[1][0] + "px, " + /*$top*/
-                l[1][1] + "px)"), H(o, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), H(o, "fill", "#FF7C00"), H(o, "fill-opacity", "0.4"), H(o, "class", "svelte-43sxxs"), H(u, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), H(u, "fill", "#FF7C00"), H(u, "class", "svelte-43sxxs"), H(_, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), H(_, "fill", "#FF7C00"), H(_, "fill-opacity", "0.4"), H(_, "class", "svelte-43sxxs"), H(c, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), H(c, "fill", "#FF7C00"), H(c, "class", "svelte-43sxxs"), Ke(r, "transform", "translate(" + /*$bottom*/
+                l[1][1] + "px)"), q(o, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(o, "fill", "#FF7C00"), q(o, "fill-opacity", "0.4"), q(o, "class", "svelte-43sxxs"), q(u, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(u, "fill", "#FF7C00"), q(u, "class", "svelte-43sxxs"), q(_, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(_, "fill", "#FF7C00"), q(_, "fill-opacity", "0.4"), q(_, "class", "svelte-43sxxs"), q(c, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(c, "fill", "#FF7C00"), q(c, "class", "svelte-43sxxs"), Ke(r, "transform", "translate(" + /*$bottom*/
                 l[2][0] + "px, " + /*$bottom*/
-                l[2][1] + "px)"), H(t, "viewBox", "-1200 -1200 3000 3000"), H(t, "fill", "none"), H(t, "xmlns", "http://www.w3.org/2000/svg"), H(t, "class", "svelte-43sxxs"), H(e, "class", "svelte-43sxxs"), Kt(
+                l[2][1] + "px)"), q(t, "viewBox", "-1200 -1200 3000 3000"), q(t, "fill", "none"), q(t, "xmlns", "http://www.w3.org/2000/svg"), q(t, "class", "svelte-43sxxs"), q(e, "class", "svelte-43sxxs"), Kt(
                 e,
                 "margin",
                 /*margin*/
                 l[0]
             );
         },
         m(m, v) {
-            Hi(m, e, v), Q(e, t), Q(t, n), Q(n, i), Q(n, s), Q(n, f), Q(n, a), Q(t, r), Q(r, o), Q(r, u), Q(r, _), Q(r, c);
+            qi(m, e, v), Q(e, t), Q(t, n), Q(n, i), Q(n, s), Q(n, f), Q(n, a), Q(t, r), Q(r, o), Q(r, u), Q(r, _), Q(r, c);
         },
         p(m, [v]) {
             v & /*$top*/
                 2 && Ke(n, "transform", "translate(" + /*$top*/
                     m[1][0] + "px, " + /*$top*/
                     m[1][1] + "px)"), v & /*$bottom*/
                 4 && Ke(r, "transform", "translate(" + /*$bottom*/
@@ -2510,23 +2510,23 @@
                     /*margin*/
                     m[0]
                 );
         },
         i: Yt,
         o: Yt,
         d(m) {
-            m && qi(e);
+            m && Mi(e);
         }
     };
 }
 
 function zi(l, e, t) {
     let n, i;
     var s = this && this.__awaiter || function(m, v, L, w) {
-        function V(b) {
+        function H(b) {
             return b instanceof L ? b : new L(function(h) {
                 h(b);
             });
         }
         return new(L || (L = Promise))(function(b, h) {
             function p(N) {
                 try {
@@ -2541,15 +2541,15 @@
                     k(w.throw(N));
                 } catch (B) {
                     h(B);
                 }
             }
 
             function k(N) {
-                N.done ? b(N.value) : V(N.value).then(p, T);
+                N.done ? b(N.value) : H(N.value).then(p, T);
             }
             k((w = w.apply(m, v || [])).next());
         });
     };
     let {
         margin: f = !0
     } = e;
@@ -2578,49 +2578,49 @@
     }
     return Zi(() => (c(), () => o = !0)), l.$$set = (m) => {
         "margin" in m && t(0, f = m.margin);
     }, [f, n, i, a, r];
 }
 class Ei extends Li {
     constructor(e) {
-        super(), Vi(this, e, zi, Si, Fi, {
+        super(), Hi(this, e, zi, Si, Fi, {
             margin: 0
         });
     }
 }
 const {
     SvelteComponent: Ti,
     append: be,
     attr: ee,
     binding_callbacks: Ot,
     check_outros: mt,
     create_component: vl,
     create_slot: kl,
     destroy_component: pl,
     destroy_each: Cl,
-    detach: q,
+    detach: M,
     element: ae,
     empty: Ee,
     ensure_array_like: Je,
     get_all_dirty_from_scope: yl,
     get_slot_changes: Ll,
     group_outros: ht,
     init: Ni,
-    insert: M,
-    mount_component: ql,
+    insert: V,
+    mount_component: Ml,
     noop: bt,
     safe_not_equal: Bi,
     set_data: R,
     set_style: ce,
     space: G,
     text: E,
     toggle_class: X,
     transition_in: $,
     transition_out: re,
-    update_slot_base: Ml
+    update_slot_base: Vl
 } = window.__gradio__svelte__internal, {
     tick: Ai
 } = window.__gradio__svelte__internal, {
     onDestroy: Di
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: Ii
 } = window.__gradio__svelte__internal, ji = (l) => ({}), Ut = (l) => ({}), Pi = (l) => ({}), Xt = (l) => ({});
@@ -2667,24 +2667,24 @@
             Ut
         );
     return {
         c() {
             e = ae("div"), vl(t.$$.fragment), n = G(), i = ae("span"), f = E(s), a = G(), u && u.c(), ee(e, "class", "clear-status svelte-vopvsi"), ee(i, "class", "error svelte-vopvsi");
         },
         m(_, c) {
-            M(_, e, c), ql(t, e, null), M(_, n, c), M(_, i, c), be(i, f), M(_, a, c), u && u.m(_, c), r = !0;
+            V(_, e, c), Ml(t, e, null), V(_, n, c), V(_, i, c), be(i, f), V(_, a, c), u && u.m(_, c), r = !0;
         },
         p(_, c) {
             const m = {};
             c[0] & /*i18n*/
                 2 && (m.label = /*i18n*/
                     _[1]("common.clear")), t.$set(m), (!r || c[0] & /*i18n*/
                     2) && s !== (s = /*i18n*/
                     _[1]("common.error") + "") && R(f, s), u && u.p && (!r || c[0] & /*$$scope*/
-                    536870912) && Ml(
+                    536870912) && Vl(
                     u,
                     o,
                     _,
                     /*$$scope*/
                     _[29],
                     r ? Ll(
                         o,
@@ -2702,15 +2702,15 @@
         i(_) {
             r || ($(t.$$.fragment, _), $(u, _), r = !0);
         },
         o(_) {
             re(t.$$.fragment, _), re(u, _), r = !1;
         },
         d(_) {
-            _ && (q(e), q(n), q(i), q(a)), pl(t), u && u.d(_);
+            _ && (M(e), M(n), M(i), M(a)), pl(t), u && u.d(_);
         }
     };
 }
 
 function Ki(l) {
     let e, t, n, i, s, f, a, r, o, u = (
         /*variant*/
@@ -2743,24 +2743,24 @@
         v = (
             /*timer*/
             l[5] && xt(l)
         );
     const L = [Ji, Wi],
         w = [];
 
-    function V(h, p) {
+    function H(h, p) {
         return (
             /*last_progress_level*/
             h[15] != null ? 0 : (
                 /*show_progress*/
                 h[6] === "full" ? 1 : -1
             )
         );
     }
-    ~(s = V(l)) && (f = w[s] = L[s](l));
+    ~(s = H(l)) && (f = w[s] = L[s](l));
     let b = ! /*timer*/
         l[5] && sl(l);
     return {
         c() {
             u && u.c(), e = G(), t = ae("div"), m && m.c(), n = G(), v && v.c(), i = G(), f && f.c(), a = G(), b && b.c(), r = Ee(), ee(t, "class", "progress-text svelte-vopvsi"), X(
                 t,
                 "meta-text-center",
@@ -2770,15 +2770,15 @@
                 t,
                 "meta-text",
                 /*variant*/
                 l[8] === "default"
             );
         },
         m(h, p) {
-            u && u.m(h, p), M(h, e, p), M(h, t, p), m && m.m(t, null), be(t, n), v && v.m(t, null), M(h, i, p), ~s && w[s].m(h, p), M(h, a, p), b && b.m(h, p), M(h, r, p), o = !0;
+            u && u.m(h, p), V(h, e, p), V(h, t, p), m && m.m(t, null), be(t, n), v && v.m(t, null), V(h, i, p), ~s && w[s].m(h, p), V(h, a, p), b && b.m(h, p), V(h, r, p), o = !0;
         },
         p(h, p) {
             /*variant*/
             h[8] === "default" && /*show_eta_bar*/
                 h[18] && /*show_progress*/
                 h[6] === "full" ? u ? u.p(h, p) : (u = Wt(h), u.c(), u.m(e.parentNode, e)) : u && (u.d(1), u = null), c === (c = _(h)) && m ? m.p(h, p) : (m && m.d(1), m = c && c(h), m && (m.c(), m.m(t, n))), /*timer*/
                 h[5] ? v ? v.p(h, p) : (v = xt(h), v.c(), v.m(t, null)) : v && (v.d(1), v = null), (!o || p[0] & /*variant*/
@@ -2791,67 +2791,67 @@
                     256) && X(
                     t,
                     "meta-text",
                     /*variant*/
                     h[8] === "default"
                 );
             let T = s;
-            s = V(h), s === T ? ~s && w[s].p(h, p) : (f && (ht(), re(w[T], 1, 1, () => {
+            s = H(h), s === T ? ~s && w[s].p(h, p) : (f && (ht(), re(w[T], 1, 1, () => {
                     w[T] = null;
                 }), mt()), ~s ? (f = w[s], f ? f.p(h, p) : (f = w[s] = L[s](h), f.c()), $(f, 1), f.m(a.parentNode, a)) : f = null), /*timer*/
                 h[5] ? b && (ht(), re(b, 1, 1, () => {
                     b = null;
                 }), mt()) : b ? (b.p(h, p), p[0] & /*timer*/
                     32 && $(b, 1)) : (b = sl(h), b.c(), $(b, 1), b.m(r.parentNode, r));
         },
         i(h) {
             o || ($(f), $(b), o = !0);
         },
         o(h) {
             re(f), re(b), o = !1;
         },
         d(h) {
-            h && (q(e), q(t), q(i), q(a), q(r)), u && u.d(h), m && m.d(), v && v.d(), ~s && w[s].d(h), b && b.d(h);
+            h && (M(e), M(t), M(i), M(a), M(r)), u && u.d(h), m && m.d(), v && v.d(), ~s && w[s].d(h), b && b.d(h);
         }
     };
 }
 
 function Wt(l) {
     let e, t = `translateX(${/*eta_level*/
   (l[17] || 0) * 100 - 100}%)`;
     return {
         c() {
             e = ae("div"), ee(e, "class", "eta-bar svelte-vopvsi"), ce(e, "transform", t);
         },
         m(n, i) {
-            M(n, e, i);
+            V(n, e, i);
         },
         p(n, i) {
             i[0] & /*eta_level*/
                 131072 && t !== (t = `translateX(${/*eta_level*/
       (n[17] || 0) * 100 - 100}%)`) && ce(e, "transform", t);
         },
         d(n) {
-            n && q(e);
+            n && M(e);
         }
     };
 }
 
 function Oi(l) {
     let e;
     return {
         c() {
             e = E("processing |");
         },
         m(t, n) {
-            M(t, e, n);
+            V(t, e, n);
         },
         p: bt,
         d(t) {
-            t && q(e);
+            t && M(e);
         }
     };
 }
 
 function Ui(l) {
     let e, t = (
             /*queue_position*/
@@ -2862,28 +2862,28 @@
         c() {
             e = E("queue: "), n = E(t), i = E("/"), s = E(
                 /*queue_size*/
                 l[3]
             ), f = E(" |");
         },
         m(a, r) {
-            M(a, e, r), M(a, n, r), M(a, i, r), M(a, s, r), M(a, f, r);
+            V(a, e, r), V(a, n, r), V(a, i, r), V(a, s, r), V(a, f, r);
         },
         p(a, r) {
             r[0] & /*queue_position*/
                 4 && t !== (t = /*queue_position*/
                     a[2] + 1 + "") && R(n, t), r[0] & /*queue_size*/
                 8 && R(
                     s,
                     /*queue_size*/
                     a[3]
                 );
         },
         d(a) {
-            a && (q(e), q(n), q(i), q(s), q(f));
+            a && (M(e), M(n), M(i), M(s), M(f));
         }
     };
 }
 
 function Xi(l) {
     let e, t = Je(
             /*progress*/
@@ -2897,15 +2897,15 @@
             for (let i = 0; i < n.length; i += 1)
                 n[i].c();
             e = Ee();
         },
         m(i, s) {
             for (let f = 0; f < n.length; f += 1)
                 n[f] && n[f].m(i, s);
-            M(i, e, s);
+            V(i, e, s);
         },
         p(i, s) {
             if (s[0] & /*progress*/
                 128) {
                 t = Je(
                     /*progress*/
                     i[7]
@@ -2917,15 +2917,15 @@
                 }
                 for (; f < n.length; f += 1)
                     n[f].d(1);
                 n.length = t.length;
             }
         },
         d(i) {
-            i && q(e), Cl(n, i);
+            i && M(e), Cl(n, i);
         }
     };
 }
 
 function Jt(l) {
     let e, t = (
             /*p*/
@@ -2943,23 +2943,23 @@
     let r = a(l),
         o = r(l);
     return {
         c() {
             o.c(), e = G(), n = E(t), i = E(" | "), f = E(s);
         },
         m(u, _) {
-            o.m(u, _), M(u, e, _), M(u, n, _), M(u, i, _), M(u, f, _);
+            o.m(u, _), V(u, e, _), V(u, n, _), V(u, i, _), V(u, f, _);
         },
         p(u, _) {
             r === (r = a(u)) && o ? o.p(u, _) : (o.d(1), o = r(u), o && (o.c(), o.m(e.parentNode, e))), _[0] & /*progress*/
                 128 && t !== (t = /*p*/
                     u[41].unit + "") && R(n, t);
         },
         d(u) {
-            u && (q(e), q(n), q(i), q(f)), o.d(u);
+            u && (M(e), M(n), M(i), M(f)), o.d(u);
         }
     };
 }
 
 function Gi(l) {
     let e = Fe(
             /*p*/
@@ -2967,25 +2967,25 @@
         ) + "",
         t;
     return {
         c() {
             t = E(e);
         },
         m(n, i) {
-            M(n, t, i);
+            V(n, t, i);
         },
         p(n, i) {
             i[0] & /*progress*/
                 128 && e !== (e = Fe(
                     /*p*/
                     n[41].index || 0
                 ) + "") && R(t, e);
         },
         d(n) {
-            n && q(t);
+            n && M(t);
         }
     };
 }
 
 function Ri(l) {
     let e = Fe(
             /*p*/
@@ -2997,51 +2997,51 @@
         ) + "",
         s;
     return {
         c() {
             t = E(e), n = E("/"), s = E(i);
         },
         m(f, a) {
-            M(f, t, a), M(f, n, a), M(f, s, a);
+            V(f, t, a), V(f, n, a), V(f, s, a);
         },
         p(f, a) {
             a[0] & /*progress*/
                 128 && e !== (e = Fe(
                     /*p*/
                     f[41].index || 0
                 ) + "") && R(t, e), a[0] & /*progress*/
                 128 && i !== (i = Fe(
                     /*p*/
                     f[41].length
                 ) + "") && R(s, i);
         },
         d(f) {
-            f && (q(t), q(n), q(s));
+            f && (M(t), M(n), M(s));
         }
     };
 }
 
 function Qt(l) {
     let e, t = (
         /*p*/
         l[41].index != null && Jt(l)
     );
     return {
         c() {
             t && t.c(), e = Ee();
         },
         m(n, i) {
-            t && t.m(n, i), M(n, e, i);
+            t && t.m(n, i), V(n, e, i);
         },
         p(n, i) {
             /*p*/
             n[41].index != null ? t ? t.p(n, i) : (t = Jt(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(n) {
-            n && q(e), t && t.d(n);
+            n && M(e), t && t.d(n);
         }
     };
 }
 
 function xt(l) {
     let e, t = (
             /*eta*/
@@ -3053,29 +3053,29 @@
         c() {
             e = E(
                 /*formatted_timer*/
                 l[20]
             ), n = E(t), i = E("s");
         },
         m(s, f) {
-            M(s, e, f), M(s, n, f), M(s, i, f);
+            V(s, e, f), V(s, n, f), V(s, i, f);
         },
         p(s, f) {
             f[0] & /*formatted_timer*/
                 1048576 && R(
                     e,
                     /*formatted_timer*/
                     s[20]
                 ), f[0] & /*eta, formatted_eta*/
                 524289 && t !== (t = /*eta*/
                     s[0] ? `/${/*formatted_eta*/
       s[19]}` : "") && R(n, t);
         },
         d(s) {
-            s && (q(e), q(n), q(i));
+            s && (M(e), M(n), M(i));
         }
     };
 }
 
 function Wi(l) {
     let e, t;
     return e = new Ei({
@@ -3086,15 +3086,15 @@
             )
         }
     }), {
         c() {
             vl(e.$$.fragment);
         },
         m(n, i) {
-            ql(e, n, i), t = !0;
+            Ml(e, n, i), t = !0;
         },
         p(n, i) {
             const s = {};
             i[0] & /*variant*/
                 256 && (s.margin = /*variant*/
                     n[8] === "default"), e.$set(s);
         },
@@ -3118,26 +3118,26 @@
             l[7] != null && $t(l)
         );
     return {
         c() {
             e = ae("div"), t = ae("div"), a && a.c(), n = G(), i = ae("div"), s = ae("div"), ee(t, "class", "progress-level-inner svelte-vopvsi"), ee(s, "class", "progress-bar svelte-vopvsi"), ce(s, "width", f), ee(i, "class", "progress-bar-wrap svelte-vopvsi"), ee(e, "class", "progress-level svelte-vopvsi");
         },
         m(r, o) {
-            M(r, e, o), be(e, t), a && a.m(t, null), be(e, n), be(e, i), be(i, s), l[31](s);
+            V(r, e, o), be(e, t), a && a.m(t, null), be(e, n), be(e, i), be(i, s), l[31](s);
         },
         p(r, o) {
             /*progress*/
             r[7] != null ? a ? a.p(r, o) : (a = $t(r), a.c(), a.m(t, null)) : a && (a.d(1), a = null), o[0] & /*last_progress_level*/
                 32768 && f !== (f = `${/*last_progress_level*/
       r[15] * 100}%`) && ce(s, "width", f);
         },
         i: bt,
         o: bt,
         d(r) {
-            r && q(e), a && a.d(), l[31](null);
+            r && M(e), a && a.d(), l[31](null);
         }
     };
 }
 
 function $t(l) {
     let e, t = Je(
             /*progress*/
@@ -3151,15 +3151,15 @@
             for (let i = 0; i < n.length; i += 1)
                 n[i].c();
             e = Ee();
         },
         m(i, s) {
             for (let f = 0; f < n.length; f += 1)
                 n[f] && n[f].m(i, s);
-            M(i, e, s);
+            V(i, e, s);
         },
         p(i, s) {
             if (s[0] & /*progress_level, progress*/
                 16512) {
                 t = Je(
                     /*progress*/
                     i[7]
@@ -3171,15 +3171,15 @@
                 }
                 for (; f < n.length; f += 1)
                     n[f].d(1);
                 n.length = t.length;
             }
         },
         d(i) {
-            i && q(e), Cl(n, i);
+            i && M(e), Cl(n, i);
         }
     };
 }
 
 function el(l) {
     let e, t, n, i, s = (
             /*i*/
@@ -3203,44 +3203,44 @@
             l[14] != null && nl(l)
         );
     return {
         c() {
             s && s.c(), e = G(), f && f.c(), t = G(), a && a.c(), n = G(), r && r.c(), i = Ee();
         },
         m(o, u) {
-            s && s.m(o, u), M(o, e, u), f && f.m(o, u), M(o, t, u), a && a.m(o, u), M(o, n, u), r && r.m(o, u), M(o, i, u);
+            s && s.m(o, u), V(o, e, u), f && f.m(o, u), V(o, t, u), a && a.m(o, u), V(o, n, u), r && r.m(o, u), V(o, i, u);
         },
         p(o, u) {
             /*p*/
             o[41].desc != null ? f ? f.p(o, u) : (f = tl(o), f.c(), f.m(t.parentNode, t)) : f && (f.d(1), f = null), /*p*/
                 o[41].desc != null && /*progress_level*/
                 o[14] && /*progress_level*/
                 o[14][
                     /*i*/
                     o[43]
                 ] != null ? a || (a = ll(), a.c(), a.m(n.parentNode, n)) : a && (a.d(1), a = null), /*progress_level*/
                 o[14] != null ? r ? r.p(o, u) : (r = nl(o), r.c(), r.m(i.parentNode, i)) : r && (r.d(1), r = null);
         },
         d(o) {
-            o && (q(e), q(t), q(n), q(i)), s && s.d(o), f && f.d(o), a && a.d(o), r && r.d(o);
+            o && (M(e), M(t), M(n), M(i)), s && s.d(o), f && f.d(o), a && a.d(o), r && r.d(o);
         }
     };
 }
 
 function Qi(l) {
     let e;
     return {
         c() {
             e = E(" /");
         },
         m(t, n) {
-            M(t, e, n);
+            V(t, e, n);
         },
         d(t) {
-            t && q(e);
+            t && M(e);
         }
     };
 }
 
 function tl(l) {
     let e = (
             /*p*/
@@ -3248,38 +3248,38 @@
         ),
         t;
     return {
         c() {
             t = E(e);
         },
         m(n, i) {
-            M(n, t, i);
+            V(n, t, i);
         },
         p(n, i) {
             i[0] & /*progress*/
                 128 && e !== (e = /*p*/
                     n[41].desc + "") && R(t, e);
         },
         d(n) {
-            n && q(t);
+            n && M(t);
         }
     };
 }
 
 function ll(l) {
     let e;
     return {
         c() {
             e = E("-");
         },
         m(t, n) {
-            M(t, e, n);
+            V(t, e, n);
         },
         d(t) {
-            t && q(e);
+            t && M(e);
         }
     };
 }
 
 function nl(l) {
     let e = (100 * /*progress_level*/
             (l[14][
@@ -3288,26 +3288,26 @@
             ] || 0)).toFixed(1) + "",
         t, n;
     return {
         c() {
             t = E(e), n = E("%");
         },
         m(i, s) {
-            M(i, t, s), M(i, n, s);
+            V(i, t, s), V(i, n, s);
         },
         p(i, s) {
             s[0] & /*progress_level*/
                 16384 && e !== (e = (100 * /*progress_level*/
                     (i[14][
                         /*i*/
                         i[43]
                     ] || 0)).toFixed(1) + "") && R(t, e);
         },
         d(i) {
-            i && (q(t), q(n));
+            i && (M(t), M(n));
         }
     };
 }
 
 function il(l) {
     let e, t = (
         /*p*/
@@ -3319,27 +3319,27 @@
             ] != null) && el(l)
     );
     return {
         c() {
             t && t.c(), e = Ee();
         },
         m(n, i) {
-            t && t.m(n, i), M(n, e, i);
+            t && t.m(n, i), V(n, e, i);
         },
         p(n, i) {
             /*p*/
             n[41].desc != null || /*progress_level*/
                 n[14] && /*progress_level*/
                 n[14][
                     /*i*/
                     n[43]
                 ] != null ? t ? t.p(n, i) : (t = el(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(n) {
-            n && q(e), t && t.d(n);
+            n && M(e), t && t.d(n);
         }
     };
 }
 
 function sl(l) {
     let e, t, n, i;
     const s = (
@@ -3357,24 +3357,24 @@
         c() {
             e = ae("p"), t = E(
                 /*loading_text*/
                 l[9]
             ), n = G(), f && f.c(), ee(e, "class", "loading svelte-vopvsi");
         },
         m(a, r) {
-            M(a, e, r), be(e, t), M(a, n, r), f && f.m(a, r), i = !0;
+            V(a, e, r), be(e, t), V(a, n, r), f && f.m(a, r), i = !0;
         },
         p(a, r) {
             (!i || r[0] & /*loading_text*/
                 512) && R(
                 t,
                 /*loading_text*/
                 a[9]
             ), f && f.p && (!i || r[0] & /*$$scope*/
-                536870912) && Ml(
+                536870912) && Vl(
                 f,
                 s,
                 a,
                 /*$$scope*/
                 a[29],
                 i ? Ll(
                     s,
@@ -3392,15 +3392,15 @@
         i(a) {
             i || ($(f, a), i = !0);
         },
         o(a) {
             re(f, a), i = !1;
         },
         d(a) {
-            a && (q(e), q(n)), f && f.d(a);
+            a && (M(e), M(n)), f && f.d(a);
         }
     };
 }
 
 function xi(l) {
     let e, t, n, i, s;
     const f = [Ki, Yi],
@@ -3450,15 +3450,15 @@
                 e,
                 "padding",
                 /*absolute*/
                 l[10] ? "0" : "var(--size-8) 0"
             );
         },
         m(o, u) {
-            M(o, e, u), ~t && a[t].m(e, null), l[33](e), s = !0;
+            V(o, e, u), ~t && a[t].m(e, null), l[33](e), s = !0;
         },
         p(o, u) {
             let _ = t;
             t = r(o), t === _ ? ~t && a[t].p(o, u) : (n && (ht(), re(a[_], 1, 1, () => {
                     a[_] = null;
                 }), mt()), ~t ? (n = a[t], n ? n.p(o, u) : (n = a[t] = f[t](o), n.c()), $(n, 1), n.m(e, null)) : n = null), (!s || u[0] & /*variant, show_progress*/
                     320 && i !== (i = "wrap " + /*variant*/
@@ -3506,15 +3506,15 @@
         i(o) {
             s || ($(n), s = !0);
         },
         o(o) {
             re(n), s = !1;
         },
         d(o) {
-            o && q(e), ~t && a[t].d(), l[33](null);
+            o && M(e), ~t && a[t].d(), l[33](null);
         }
     };
 }
 var $i = function(l, e, t, n) {
     function i(s) {
         return s instanceof t ? s : new t(function(f) {
             f(s);
@@ -3592,15 +3592,15 @@
     } = e, {
         show_progress: v = "full"
     } = e, {
         message: L = null
     } = e, {
         progress: w = null
     } = e, {
-        variant: V = "default"
+        variant: H = "default"
     } = e, {
         loading_text: b = "Loading..."
     } = e, {
         absolute: h = !0
     } = e, {
         translucent: p = !1
     } = e, {
@@ -3637,15 +3637,15 @@
 
     function $e(C) {
         Ot[C ? "unshift" : "push"](() => {
             N = C, t(13, N);
         });
     }
     return l.$$set = (C) => {
-        "i18n" in C && t(1, a = C.i18n), "eta" in C && t(0, r = C.eta), "queue_position" in C && t(2, o = C.queue_position), "queue_size" in C && t(3, u = C.queue_size), "status" in C && t(4, _ = C.status), "scroll_to_output" in C && t(22, c = C.scroll_to_output), "timer" in C && t(5, m = C.timer), "show_progress" in C && t(6, v = C.show_progress), "message" in C && t(23, L = C.message), "progress" in C && t(7, w = C.progress), "variant" in C && t(8, V = C.variant), "loading_text" in C && t(9, b = C.loading_text), "absolute" in C && t(10, h = C.absolute), "translucent" in C && t(11, p = C.translucent), "border" in C && t(12, T = C.border), "autoscroll" in C && t(24, k = C.autoscroll), "$$scope" in C && t(29, s = C.$$scope);
+        "i18n" in C && t(1, a = C.i18n), "eta" in C && t(0, r = C.eta), "queue_position" in C && t(2, o = C.queue_position), "queue_size" in C && t(3, u = C.queue_size), "status" in C && t(4, _ = C.status), "scroll_to_output" in C && t(22, c = C.scroll_to_output), "timer" in C && t(5, m = C.timer), "show_progress" in C && t(6, v = C.show_progress), "message" in C && t(23, L = C.message), "progress" in C && t(7, w = C.progress), "variant" in C && t(8, H = C.variant), "loading_text" in C && t(9, b = C.loading_text), "absolute" in C && t(10, h = C.absolute), "translucent" in C && t(11, p = C.translucent), "border" in C && t(12, T = C.border), "autoscroll" in C && t(24, k = C.autoscroll), "$$scope" in C && t(29, s = C.$$scope);
     }, l.$$.update = () => {
         l.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
             436207617 && (r === null && t(0, r = I), r != null && I !== r && (t(28, ie = (performance.now() - P) / 1e3 + r), t(19, ke = ie.toFixed(1)), t(27, I = r))), l.$$.dirty[0] & /*eta_from_start, timer_diff*/
             335544320 && t(17, ge = ie === null || ie <= 0 || !Y ? null : Math.min(Y / ie, 1)), l.$$.dirty[0] & /*progress*/
             128 && w != null && t(18, we = !1), l.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
             114816 && (w != null ? t(14, W = w.map((C) => {
                 if (C.index != null && C.length != null)
@@ -3662,15 +3662,15 @@
         a,
         o,
         u,
         _,
         m,
         v,
         w,
-        V,
+        H,
         b,
         h,
         p,
         T,
         N,
         W,
         se,
@@ -3735,15 +3735,15 @@
     element: us,
     init: _s,
     insert: cs,
     noop: fl,
     safe_not_equal: ds,
     set_data: ms,
     text: hs,
-    toggle_class: He
+    toggle_class: qe
 } = window.__gradio__svelte__internal, {
     onMount: bs
 } = window.__gradio__svelte__internal;
 
 function gs(l) {
     let e, t = (
             /*value*/
@@ -3754,25 +3754,25 @@
         ),
         n, i;
     return {
         c() {
             e = us("div"), n = hs(t), os(e, "class", "svelte-84cxb8"), ss(() => (
                 /*div_elementresize_handler*/
                 l[5].call(e)
-            )), He(
+            )), qe(
                 e,
                 "table",
                 /*type*/
                 l[1] === "table"
-            ), He(
+            ), qe(
                 e,
                 "gallery",
                 /*type*/
                 l[1] === "gallery"
-            ), He(
+            ), qe(
                 e,
                 "selected",
                 /*selected*/
                 l[2]
             );
         },
         m(s, f) {
@@ -3785,27 +3785,27 @@
         p(s, [f]) {
             f & /*value*/
                 1 && t !== (t = /*value*/
                     (s[0] ? (
                         /*value*/
                         s[0]
                     ) : "") + "") && ms(n, t), f & /*type*/
-                2 && He(
+                2 && qe(
                     e,
                     "table",
                     /*type*/
                     s[1] === "table"
                 ), f & /*type*/
-                2 && He(
+                2 && qe(
                     e,
                     "gallery",
                     /*type*/
                     s[1] === "gallery"
                 ), f & /*selected*/
-                4 && He(
+                4 && qe(
                     e,
                     "selected",
                     /*selected*/
                     s[2]
                 );
         },
         i: fl,
@@ -3863,19 +3863,19 @@
     check_outros: ps,
     create_component: Ct,
     destroy_component: yt,
     detach: Cs,
     flush: Z,
     get_spread_object: ys,
     get_spread_update: Ls,
-    group_outros: qs,
-    init: Ms,
-    insert: Vs,
+    group_outros: Ms,
+    init: Vs,
+    insert: Hs,
     mount_component: Lt,
-    safe_not_equal: Hs,
+    safe_not_equal: qs,
     space: Fs,
     transition_in: Ze,
     transition_out: Ie
 } = window.__gradio__svelte__internal;
 
 function ul(l) {
     let e, t;
@@ -4054,20 +4054,20 @@
             /*focus_handler*/
             l[32]
         ), {
             c() {
                 f && f.c(), e = Fs(), Ct(t.$$.fragment);
             },
             m(u, _) {
-                f && f.m(u, _), Vs(u, e, _), Lt(t, u, _), s = !0;
+                f && f.m(u, _), Hs(u, e, _), Lt(t, u, _), s = !0;
             },
             p(u, _) {
                 /*loading_status*/
                 u[18] ? f ? (f.p(u, _), _[0] & /*loading_status*/
-                    262144 && Ze(f, 1)) : (f = ul(u), f.c(), Ze(f, 1), f.m(e.parentNode, e)) : f && (qs(), Ie(f, 1, 1, () => {
+                    262144 && Ze(f, 1)) : (f = ul(u), f.c(), Ze(f, 1), f.m(e.parentNode, e)) : f && (Ms(), Ie(f, 1, 1, () => {
                     f = null;
                 }), ps());
                 const c = {};
                 _[0] & /*label*/
                     8 && (c.label = /*label*/
                         u[3]), _[0] & /*info*/
                     16 && (c.info = /*info*/
@@ -4224,15 +4224,15 @@
     } = e, {
         prompts: v = []
     } = e, {
         suffixes: L = []
     } = e, {
         type: w = "text"
     } = e, {
-        container: V = !0
+        container: H = !0
     } = e, {
         scale: b = null
     } = e, {
         min_width: h = void 0
     } = e, {
         loading_status: p = void 0
     } = e, {
@@ -4260,15 +4260,15 @@
     const W = () => n.dispatch("change", o),
         se = () => n.dispatch("input"),
         K = () => n.dispatch("submit"),
         we = () => n.dispatch("blur"),
         Te = (g) => n.dispatch("select", g.detail),
         ve = () => n.dispatch("focus");
     return l.$$set = (g) => {
-        "gradio" in g && t(2, n = g.gradio), "label" in g && t(3, i = g.label), "info" in g && t(4, s = g.info), "elem_id" in g && t(5, f = g.elem_id), "elem_classes" in g && t(6, a = g.elem_classes), "visible" in g && t(7, r = g.visible), "value" in g && t(0, o = g.value), "lines" in g && t(8, u = g.lines), "placeholder" in g && t(9, _ = g.placeholder), "show_label" in g && t(10, c = g.show_label), "max_lines" in g && t(11, m = g.max_lines), "prompts" in g && t(12, v = g.prompts), "suffixes" in g && t(13, L = g.suffixes), "type" in g && t(14, w = g.type), "container" in g && t(15, V = g.container), "scale" in g && t(16, b = g.scale), "min_width" in g && t(17, h = g.min_width), "loading_status" in g && t(18, p = g.loading_status), "value_is_output" in g && t(1, T = g.value_is_output), "rtl" in g && t(19, k = g.rtl), "text_align" in g && t(20, N = g.text_align), "autofocus" in g && t(21, B = g.autofocus), "autoscroll" in g && t(22, P = g.autoscroll), "interactive" in g && t(23, Y = g.interactive);
+        "gradio" in g && t(2, n = g.gradio), "label" in g && t(3, i = g.label), "info" in g && t(4, s = g.info), "elem_id" in g && t(5, f = g.elem_id), "elem_classes" in g && t(6, a = g.elem_classes), "visible" in g && t(7, r = g.visible), "value" in g && t(0, o = g.value), "lines" in g && t(8, u = g.lines), "placeholder" in g && t(9, _ = g.placeholder), "show_label" in g && t(10, c = g.show_label), "max_lines" in g && t(11, m = g.max_lines), "prompts" in g && t(12, v = g.prompts), "suffixes" in g && t(13, L = g.suffixes), "type" in g && t(14, w = g.type), "container" in g && t(15, H = g.container), "scale" in g && t(16, b = g.scale), "min_width" in g && t(17, h = g.min_width), "loading_status" in g && t(18, p = g.loading_status), "value_is_output" in g && t(1, T = g.value_is_output), "rtl" in g && t(19, k = g.rtl), "text_align" in g && t(20, N = g.text_align), "autofocus" in g && t(21, B = g.autofocus), "autoscroll" in g && t(22, P = g.autoscroll), "interactive" in g && t(23, Y = g.interactive);
     }, [
         o,
         T,
         n,
         i,
         s,
         f,
@@ -4277,15 +4277,15 @@
         u,
         _,
         c,
         m,
         v,
         L,
         w,
-        V,
+        H,
         b,
         h,
         p,
         k,
         N,
         B,
         P,
@@ -4299,20 +4299,20 @@
         we,
         Te,
         ve
     ];
 }
 class Ts extends vs {
     constructor(e) {
-        super(), Ms(
+        super(), Vs(
             this,
             e,
             zs,
             Ss,
-            Hs, {
+            qs, {
                 gradio: 2,
                 label: 3,
                 info: 4,
                 elem_id: 5,
                 elem_classes: 6,
                 visible: 7,
                 value: 0,
```

### Comparing `gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/templates/component/style.css` & `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/component/style.css`

 * *Files 9% similar despite different names*

```diff
@@ -1 +1 @@
-.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-1lrphxw{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-1lrphxw{opacity:.5;box-shadow:none}button[disabled].svelte-1lrphxw:hover{cursor:not-allowed}.padded.svelte-1lrphxw{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-1lrphxw:hover,button.highlight.svelte-1lrphxw{cursor:pointer;color:var(--color-accent)}.padded.svelte-1lrphxw:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-1lrphxw{padding:0 1px;font-size:10px}div.svelte-1lrphxw{padding:2px;display:flex;align-items:flex-end}.small.svelte-1lrphxw{width:14px;height:14px}.medium.svelte-1lrphxw{width:20px;height:20px}.large.svelte-1lrphxw{width:22px;height:22px}.pending.svelte-1lrphxw{animation:svelte-1lrphxw-flash .5s infinite}@keyframes svelte-1lrphxw-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-1lrphxw{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-q32hvf{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;align-items:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;color:var(--block-label-text-color);flex-shrink:0}.show_border.svelte-q32hvf{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}label.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk{display:block;width:100%}textarea.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk{display:block;position:relative;outline:none!important;box-shadow:var(--input-shadow);background:var(--input-background-fill);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none}label.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk:not(.container),textarea.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk:disabled{-webkit-text-fill-color:var(--body-text-color);-webkit-opacity:1;opacity:1}textarea.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk::placeholder{color:var(--input-placeholder-color)}.extend_button.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk{display:flex;position:relative;align-items:center;width:20px;height:20px;overflow:hidden;color:var(--block-label-color);font:var(--font-sans);font-size:var(--button-small-text-size)}.extend_button.svelte-8lpwqk:hover path.svelte-8lpwqk.svelte-8lpwqk{--ring-color:var(--color-accent);filter:brightness(1.1);fill:#ff6700}.menu_section.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk{padding:12px 0 0;align-items:center;color:#100700;font-family:Inter;font-size:13px;font-style:normal;font-weight:300;line-height:24px;display:flex;flex-direction:column;align-items:flex-start;gap:8px}.menu.svelte-8lpwqk ul.svelte-8lpwqk.svelte-8lpwqk{list-style-type:none;display:flex;align-items:flex-start;align-content:flex-start;gap:4px 12px;flex-wrap:wrap;flex-direction:column;width:100%}.menu.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk{border-radius:0 0 15px 15px;background:#cccccc1a;margin:0 16px;padding:0 14px 12px}.menu.svelte-8lpwqk li.svelte-8lpwqk.svelte-8lpwqk{width:100%}.text_extension_button.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk{border-radius:15px;border:.5px solid #ff9a57;background:#fff4ea;cursor:pointer;display:flex;padding:4px 12px;align-items:center;gap:4px}.text_extension_button_prompt.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk{display:flex;width:100%;padding:8px 12px;justify-content:space-between;align-items:center;border-radius:10px;border:.5px solid #ff9a57;background:#fff4ea;color:#101111;text-align:left;font-size:13px;font-style:normal;font-weight:300;line-height:normal;gap:4px;flex-wrap:nowrap;flex-direction:row}.text_extension_button_prompt.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk:hover{color:#fff;fill:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button_prompt.svelte-8lpwqk:hover svg.svelte-8lpwqk path.svelte-8lpwqk{fill:#fff}.text_extension_button.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk:hover{color:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button.svelte-8lpwqk:hover svg.svelte-8lpwqk path.svelte-8lpwqk{fill:#fff}.magic_container.svelte-8lpwqk.svelte-8lpwqk.svelte-8lpwqk{display:flex;position:relative;outline:none!important;box-shadow:var(--input-shadow);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none;scrollbar-width:none;resize:none;align-items:center}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden}.wrap.center.svelte-vopvsi.svelte-vopvsi{top:0;right:0;left:0}.wrap.default.svelte-vopvsi.svelte-vopvsi{top:0;right:0;bottom:0;left:0}.hide.svelte-vopvsi.svelte-vopvsi{opacity:0;pointer-events:none}.generating.svelte-vopvsi.svelte-vopvsi{animation:svelte-vopvsi-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1);pointer-events:none}.translucent.svelte-vopvsi.svelte-vopvsi{background:none}@keyframes svelte-vopvsi-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-vopvsi.svelte-vopvsi{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-vopvsi.svelte-vopvsi{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-vopvsi.svelte-vopvsi{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-vopvsi.svelte-vopvsi{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-vopvsi.svelte-vopvsi{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-vopvsi .progress-text.svelte-vopvsi{background:var(--block-background-fill)}.border.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary)}.clear-status.svelte-vopvsi.svelte-vopvsi{position:absolute;display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-84cxb8{padding:var(--size-1) var(--size-2)}div.svelte-84cxb8{overflow:hidden;min-width:var(--local-text-width);white-space:nowrap}
+.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-1lrphxw{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-1lrphxw{opacity:.5;box-shadow:none}button[disabled].svelte-1lrphxw:hover{cursor:not-allowed}.padded.svelte-1lrphxw{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-1lrphxw:hover,button.highlight.svelte-1lrphxw{cursor:pointer;color:var(--color-accent)}.padded.svelte-1lrphxw:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-1lrphxw{padding:0 1px;font-size:10px}div.svelte-1lrphxw{padding:2px;display:flex;align-items:flex-end}.small.svelte-1lrphxw{width:14px;height:14px}.medium.svelte-1lrphxw{width:20px;height:20px}.large.svelte-1lrphxw{width:22px;height:22px}.pending.svelte-1lrphxw{animation:svelte-1lrphxw-flash .5s infinite}@keyframes svelte-1lrphxw-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-1lrphxw{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-q32hvf{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;align-items:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;color:var(--block-label-text-color);flex-shrink:0}.show_border.svelte-q32hvf{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}label.svelte-ak29na.svelte-ak29na.svelte-ak29na{display:block;width:100%}textarea.svelte-ak29na.svelte-ak29na.svelte-ak29na{display:block;position:relative;outline:none!important;box-shadow:var(--input-shadow);background:var(--input-background-fill);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none}label.svelte-ak29na.svelte-ak29na.svelte-ak29na:not(.container),textarea.svelte-ak29na.svelte-ak29na.svelte-ak29na:disabled{-webkit-text-fill-color:var(--body-text-color);-webkit-opacity:1;opacity:1}textarea.svelte-ak29na.svelte-ak29na.svelte-ak29na::placeholder{color:var(--input-placeholder-color)}.extend_button.svelte-ak29na.svelte-ak29na.svelte-ak29na{display:flex;position:relative;align-items:center;width:20px;height:20px;overflow:hidden;color:var(--block-label-color);font:var(--font-sans);font-size:var(--button-small-text-size)}.extend_button.svelte-ak29na:hover path.svelte-ak29na.svelte-ak29na{--ring-color:var(--color-accent);filter:brightness(1.1);fill:#ff6700}.menu_section_prompt.svelte-ak29na.svelte-ak29na.svelte-ak29na{padding:12px 0 0;align-items:center;color:#100700;font-family:Inter;font-size:13px;font-style:normal;font-weight:300;line-height:24px;display:flex;flex-direction:column;align-items:flex-start;gap:8px}.menu_section_style.svelte-ak29na.svelte-ak29na.svelte-ak29na{padding:12px 0 0;align-items:center;color:#100700;font-family:Inter;font-size:13px;font-style:normal;font-weight:300;line-height:24px;display:flex;align-items:flex-start;flex-wrap:none;flex-direction:column;gap:8px}.menu_section_prompt.svelte-ak29na ul.svelte-ak29na.svelte-ak29na{list-style-type:none;display:flex;align-items:flex-start;align-content:flex-start;gap:4px 12px;flex-wrap:wrap;flex-direction:column;width:100%}.menu_section_style.svelte-ak29na ul.svelte-ak29na.svelte-ak29na{list-style-type:none;display:flex;align-items:flex-start;align-content:flex-start;gap:4px 12px;flex-wrap:wrap;flex-direction:row}.menu_section_style.svelte-ak29na li.svelte-ak29na.svelte-ak29na{width:auto}.menu.svelte-ak29na.svelte-ak29na.svelte-ak29na{border-radius:0 0 15px 15px;background:#cccccc1a;margin:0 16px;padding:0 14px 12px}.menu_section_prompt.svelte-ak29na li.svelte-ak29na.svelte-ak29na{width:100%}.text_extension_button.svelte-ak29na.svelte-ak29na.svelte-ak29na{border-radius:15px;border:.5px solid #ff9a57;background:#fff4ea;cursor:pointer;display:flex;padding:4px 12px;align-items:center;gap:4px}.text_extension_button_prompt.svelte-ak29na.svelte-ak29na.svelte-ak29na{display:flex;width:100%;padding:8px 12px;justify-content:space-between;align-items:center;border-radius:10px;border:.5px solid #ff9a57;background:#fff4ea;color:#101111;text-align:left;font-size:13px;font-style:normal;font-weight:300;line-height:normal;gap:4px;flex-wrap:nowrap;flex-direction:row}.text_extension_button_prompt.svelte-ak29na.svelte-ak29na.svelte-ak29na:hover{color:#fff;fill:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button_prompt.svelte-ak29na:hover svg.svelte-ak29na path.svelte-ak29na{fill:#fff}.text_extension_button.svelte-ak29na.svelte-ak29na.svelte-ak29na:hover{color:#fff;background:var(--Light-Orange, #ff9a57)}.text_extension_button.svelte-ak29na:hover svg.svelte-ak29na path.svelte-ak29na{fill:#fff}.magic_container.svelte-ak29na.svelte-ak29na.svelte-ak29na{display:flex;position:relative;outline:none!important;box-shadow:var(--input-shadow);padding:var(--input-padding);width:100%;color:var(--body-text-color);font-weight:var(--input-text-weight);font-size:var(--input-text-size);line-height:var(--line-sm);border:none;scrollbar-width:none;resize:none;align-items:center}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden}.wrap.center.svelte-vopvsi.svelte-vopvsi{top:0;right:0;left:0}.wrap.default.svelte-vopvsi.svelte-vopvsi{top:0;right:0;bottom:0;left:0}.hide.svelte-vopvsi.svelte-vopvsi{opacity:0;pointer-events:none}.generating.svelte-vopvsi.svelte-vopvsi{animation:svelte-vopvsi-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1);pointer-events:none}.translucent.svelte-vopvsi.svelte-vopvsi{background:none}@keyframes svelte-vopvsi-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-vopvsi.svelte-vopvsi{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-vopvsi.svelte-vopvsi{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-vopvsi.svelte-vopvsi{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-vopvsi.svelte-vopvsi{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-vopvsi.svelte-vopvsi{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-vopvsi.svelte-vopvsi{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-vopvsi.svelte-vopvsi{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-vopvsi .progress-text.svelte-vopvsi{background:var(--block-background-fill)}.border.svelte-vopvsi.svelte-vopvsi{border:1px solid var(--border-color-primary)}.clear-status.svelte-vopvsi.svelte-vopvsi{position:absolute;display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-84cxb8{padding:var(--size-1) var(--size-2)}div.svelte-84cxb8{overflow:hidden;min-width:var(--local-text-width);white-space:nowrap}
```

### Comparing `gradio_clickabletextbox-0.0.5/backend/gradio_clickabletextbox/templates/example/index.js` & `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/demo/app.py` & `gradio_clickabletextbox-0.0.6/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/demo/css.css` & `gradio_clickabletextbox-0.0.6/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/demo/space.py` & `gradio_clickabletextbox-0.0.6/demo/space.py`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/frontend/Example.svelte` & `gradio_clickabletextbox-0.0.6/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/frontend/Index.svelte` & `gradio_clickabletextbox-0.0.6/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/frontend/package-lock.json` & `gradio_clickabletextbox-0.0.6/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/frontend/package.json` & `gradio_clickabletextbox-0.0.6/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/frontend/shared/Textbox.svelte` & `gradio_clickabletextbox-0.0.6/frontend/shared/Textbox.svelte`

 * *Files 4% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 			<div
 				class="menu"
 				in:fadeSlide={{ duration: 500 }}
 				on:transitionstart={() => (ongoing_animation = true)}
 				on:transitionend={() => (ongoing_animation = false)}
 			>
 				{#if prompts.length > 0}
-					<div class="menu_section">
+					<div class="menu_section_prompt">
 						<span> A few prompt inspirations </span>
 						<ul>
 							{#each prompts as word}
 								<li>
 									<button
 										class="text_extension_button_prompt"
 										on:click={() => loadPrompt(word)}
@@ -263,15 +263,15 @@
 									>
 								</li>
 							{/each}
 						</ul>
 					</div>
 				{/if}
 				{#if suffixes.length > 0}
-					<div class="menu_section">
+					<div class="menu_section_style">
 						<span> Add keywords to guide style </span>
 						<ul>
 							{#each suffixes as word}
 								<li>
 									<button
 										class="text_extension_button"
 										on:click={() => addSuffix(word)}
@@ -404,48 +404,77 @@
 
 	.extend_button:hover path {
 		--ring-color: var(--color-accent);
 		filter: brightness(1.1);
 		fill: #ff6700;
 	}
 
-	.menu_section {
+	.menu_section_prompt {
 		padding: 12px 0px 0px 0px;
 		align-items: center;
 		color: #100700;
 		font-family: Inter;
 		font-size: 13px;
 		font-style: normal;
 		font-weight: 300;
 		line-height: 24px;
 		display: flex;
 		flex-direction: column;
 		align-items: flex-start;
 		gap: 8px;
 	}
 
-	.menu ul {
+	.menu_section_style {
+		padding: 12px 0px 0px 0px;
+		align-items: center;
+		color: #100700;
+		font-family: Inter;
+		font-size: 13px;
+		font-style: normal;
+		font-weight: 300;
+		line-height: 24px;
+		display: flex;
+		align-items: flex-start;
+		flex-wrap: none;
+		flex-direction: column;
+		gap: 8px;
+	}
+
+	.menu_section_prompt ul {
 		list-style-type: none;
 		display: flex;
 		align-items: flex-start;
 		align-content: flex-start;
 		gap: 4px 12px;
 		flex-wrap: wrap;
 		flex-direction: column;
 		width: 100%;
 	}
 
+	.menu_section_style ul {
+		list-style-type: none;
+		display: flex;
+		align-items: flex-start;
+		align-content: flex-start;
+		gap: 4px 12px;
+		flex-wrap: wrap;
+		flex-direction: row;
+	}
+	.menu_section_style li {
+		width: auto;
+	}
+
 	.menu {
 		border-radius: 0px 0px 15px 15px;
 		background: rgba(204, 204, 204, 0.1);
 		margin: 0px 16px;
 		padding: 0px 14px 12px 14px;
 	}
 
-	.menu li {
+	.menu_section_prompt li {
 		width: 100%;
 	}
 
 	.text_extension_button {
 		border-radius: 15px;
 		border: 0.5px solid #ff9a57;
 		background: #fff4ea;
```

### Comparing `gradio_clickabletextbox-0.0.5/frontend/shared/transitions.js` & `gradio_clickabletextbox-0.0.6/frontend/shared/transitions.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/README.md` & `gradio_clickabletextbox-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.5/pyproject.toml` & `gradio_clickabletextbox-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_clickabletextbox"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python library for easily interacting with trained machine learning models"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Textbox"]
 # Add dependencies here
```

### Comparing `gradio_clickabletextbox-0.0.5/PKG-INFO` & `gradio_clickabletextbox-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_clickabletextbox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library for easily interacting with trained machine learning models
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: Apache-2.0
 Keywords: gradio-custom-component,gradio-template-Textbox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

