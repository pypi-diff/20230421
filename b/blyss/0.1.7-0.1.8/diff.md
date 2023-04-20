# Comparing `tmp/blyss-0.1.7.tar.gz` & `tmp/blyss-0.1.8.tar.gz`

## Comparing `blyss-0.1.7.tar` & `blyss-0.1.8.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 blyss-0.1.7/local_dependencies/spiral-rs/Cargo.toml
--rw-r--r--   0     1001      123       82 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/.cargo/config.toml
--rw-r--r--   0     1001      123     2523 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/aligned_memory.rs
--rw-r--r--   0     1001      123    15010 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/arith.rs
--rw-r--r--   0     1001      123    31076 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/client.rs
--rw-r--r--   0     1001      123     5686 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/discrete_gaussian.rs
--rw-r--r--   0     1001      123     2882 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/gadget.rs
--rw-r--r--   0     1001      123     2358 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/key_value.rs
--rw-r--r--   0     1001      123      243 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/lib.rs
--rw-r--r--   0     1001      123    17652 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/ntt.rs
--rw-r--r--   0     1001      123     2386 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/number_theory.rs
--rw-r--r--   0     1001      123     7565 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/params.rs
--rw-r--r--   0     1001      123    22895 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/poly.rs
--rw-r--r--   0     1001      123    33066 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/server.rs
--rw-r--r--   0     1001      123    11526 2023-03-28 01:42:13.000000 blyss-0.1.7/local_dependencies/spiral-rs/src/util.rs
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 blyss-0.1.7/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-03-28 01:42:13.000000 blyss-0.1.7/.gitignore
--rw-r--r--   0     1001      123       19 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/__init__.py
--rw-r--r--   0     1001      123     9070 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/api.py
--rw-r--r--   0     1001      123     1275 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/bloom.py
--rw-r--r--   0     1001      123     3482 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/blyss_lib.py
--rw-r--r--   0     1001      123    11666 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/bucket.py
--rw-r--r--   0     1001      123     4126 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/bucket_service.py
--rw-r--r--   0     1001      123      139 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/main.py
--rw-r--r--   0     1001      123     2277 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/req_compression.py
--rw-r--r--   0     1001      123     1299 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/seed.py
--rw-r--r--   0     1001      123     1946 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/serializer.py
--rw-r--r--   0     1001      123     1520 2023-03-28 01:42:13.000000 blyss-0.1.7/blyss/varint.py
--rw-r--r--   0     1001      123      383 2023-03-28 01:42:13.000000 blyss-0.1.7/pyproject.toml
--rw-r--r--   0     1001      123     2160 2023-03-28 01:42:13.000000 blyss-0.1.7/src/lib.rs
--rw-r--r--   0     1001      123    13783 2023-03-28 01:42:13.000000 blyss-0.1.7/Cargo.lock
--rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 blyss-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 blyss-0.1.8/local_dependencies/spiral-rs/Cargo.toml
+-rw-r--r--   0     1001      123       82 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/.cargo/config.toml
+-rw-r--r--   0     1001      123      194 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/README.md
+-rw-r--r--   0     1001      123     2523 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/aligned_memory.rs
+-rw-r--r--   0     1001      123    15010 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/arith.rs
+-rw-r--r--   0     1001      123    32652 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/client.rs
+-rw-r--r--   0     1001      123     5686 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/discrete_gaussian.rs
+-rw-r--r--   0     1001      123     2882 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/gadget.rs
+-rw-r--r--   0     1001      123     2358 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/key_value.rs
+-rw-r--r--   0     1001      123      267 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/lib.rs
+-rw-r--r--   0     1001      123     5078 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/noise_estimate.rs
+-rw-r--r--   0     1001      123    17652 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/ntt.rs
+-rw-r--r--   0     1001      123     2386 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/number_theory.rs
+-rw-r--r--   0     1001      123     7852 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/params.rs
+-rw-r--r--   0     1001      123    23492 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/poly.rs
+-rw-r--r--   0     1001      123    36705 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/server.rs
+-rw-r--r--   0     1001      123    11665 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/util.rs
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 blyss-0.1.8/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-04-20 22:59:51.000000 blyss-0.1.8/.gitignore
+-rw-r--r--   0     1001      123       19 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/__init__.py
+-rw-r--r--   0     1001      123     9589 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/api.py
+-rw-r--r--   0     1001      123     1275 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/bloom.py
+-rw-r--r--   0     1001      123     3564 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/blyss_lib.py
+-rw-r--r--   0     1001      123    12241 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/bucket.py
+-rw-r--r--   0     1001      123     4155 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/bucket_service.py
+-rw-r--r--   0     1001      123      139 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/main.py
+-rw-r--r--   0     1001      123     2277 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/req_compression.py
+-rw-r--r--   0     1001      123     1299 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/seed.py
+-rw-r--r--   0     1001      123     1946 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/serializer.py
+-rw-r--r--   0     1001      123     1520 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/varint.py
+-rw-r--r--   0     1001      123      383 2023-04-20 22:59:51.000000 blyss-0.1.8/pyproject.toml
+-rw-r--r--   0     1001      123     2160 2023-04-20 22:59:51.000000 blyss-0.1.8/src/lib.rs
+-rw-r--r--   0     1001      123     3167 2023-04-20 22:59:51.000000 blyss-0.1.8/tests/test_service.py
+-rw-r--r--   0     1001      123    13791 2023-04-20 22:59:51.000000 blyss-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 blyss-0.1.8/PKG-INFO
```

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/aligned_memory.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/aligned_memory.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/arith.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/arith.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/client.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/client.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 use crate::{
     arith::*, discrete_gaussian::*, gadget::*, number_theory::*, params::*, poly::*, util::*,
 };
+use rand::seq::SliceRandom;
 use rand::{Rng, SeedableRng};
 use rand_chacha::ChaCha20Rng;
 use std::{iter::once, mem::size_of};
 use subtle::ConditionallySelectable;
 use subtle::ConstantTimeEq;
 
 pub type Seed = <ChaCha20Rng as SeedableRng>::Seed;
 pub const SEED_LENGTH: usize = 32;
+pub const HAMMING_WEIGHT: usize = 256;
+
+pub static mut CLIENT_TEST: Option<(PolyMatrixRaw, PolyMatrixRaw)> = None;
 
 pub const DEFAULT_PARAMS: &'static str = r#"
     {"n": 2,
     "nu_1": 10,
     "nu_2": 6,
     "p": 512,
     "q2_bits": 21,
@@ -119,14 +123,30 @@
     for i in 0..v_buf.len() {
         out.push(reg_cts_buf[2 * i]);
         out.push(v_buf[i]);
     }
     out
 }
 
+fn gen_ternary_mat(mat: &mut PolyMatrixRaw, hamming: usize, rng: &mut ChaCha20Rng) {
+    let modulus = mat.params.modulus;
+    for r in 0..mat.rows {
+        for c in 0..mat.cols {
+            let pol = mat.get_poly_mut(r, c);
+            for i in 0..hamming {
+                pol[i] = 1;
+            }
+            for i in hamming..2 * hamming {
+                pol[i] = modulus - 1;
+            }
+            pol.shuffle(rng);
+        }
+    }
+}
+
 pub struct PublicParameters<'a> {
     pub v_packing: Vec<PolyMatrixNTT<'a>>, // Ws
     pub v_expansion_left: Option<Vec<PolyMatrixNTT<'a>>>,
     pub v_expansion_right: Option<Vec<PolyMatrixNTT<'a>>>,
     pub v_conversion: Option<Vec<PolyMatrixNTT<'a>>>, // V
     pub seed: Option<Seed>,
 }
@@ -201,17 +221,25 @@
         let mut v_packing = new_vec_raw(params, params.n, params.n + 1, params.t_conv);
         idx += deserialize_vec_polymatrix_rng(&mut v_packing, &data[idx..], &mut rng);
 
         if params.expand_queries {
             let mut v_expansion_left = new_vec_raw(params, params.g(), 2, params.t_exp_left);
             idx += deserialize_vec_polymatrix_rng(&mut v_expansion_left, &data[idx..], &mut rng);
 
-            let mut v_expansion_right =
-                new_vec_raw(params, params.stop_round() + 1, 2, params.t_exp_right);
-            idx += deserialize_vec_polymatrix_rng(&mut v_expansion_right, &data[idx..], &mut rng);
+            let mut v_expansion_right = v_expansion_left.clone();
+            if params.version == 0 || params.t_exp_right != params.t_exp_left {
+                let mut v_expansion_right_tmp =
+                    new_vec_raw(params, params.stop_round() + 1, 2, params.t_exp_right);
+                idx += deserialize_vec_polymatrix_rng(
+                    &mut v_expansion_right_tmp,
+                    &data[idx..],
+                    &mut rng,
+                );
+                v_expansion_right = v_expansion_right_tmp;
+            }
 
             let mut v_conversion = new_vec_raw(params, 1, 2, 2 * params.t_conv);
             _ = deserialize_vec_polymatrix_rng(&mut v_conversion, &data[idx..], &mut rng);
 
             Self {
                 v_packing: Self::to_ntt_alloc_vec(&v_packing).unwrap(),
                 v_expansion_left: Self::to_ntt_alloc_vec(&v_expansion_left),
@@ -297,15 +325,15 @@
             deserialize_vec_polymatrix_rng(&mut v_ct, &data[v_buf_bytes..], &mut rng);
             out.v_ct = Some(v_ct);
         }
         out
     }
 }
 
-fn matrix_with_identity<'a>(p: &PolyMatrixRaw<'a>) -> PolyMatrixRaw<'a> {
+pub fn matrix_with_identity<'a>(p: &PolyMatrixRaw<'a>) -> PolyMatrixRaw<'a> {
     assert_eq!(p.cols, 1);
     let mut r = PolyMatrixRaw::zero(p.params, p.rows, p.rows + 1);
     r.copy_into(p, 0, 0);
     r.copy_into(&PolyMatrixRaw::identity(p.params, p.rows, p.rows), 0, 1);
     r
 }
 
@@ -322,14 +350,15 @@
         params.t_exp_right,
         params.t_gsw,
         params.expand_queries,
         params.db_dim_1,
         params.db_dim_2,
         params.instances,
         params.db_item_size,
+        params.version,
     )
 }
 
 pub struct Client<'a> {
     params: &'a Params,
     sk_gsw: PolyMatrixRaw<'a>,
     sk_reg: PolyMatrixRaw<'a>,
@@ -360,14 +389,19 @@
     }
 
     #[allow(dead_code)]
     pub(crate) fn get_sk_reg(&self) -> &PolyMatrixRaw<'a> {
         &self.sk_reg
     }
 
+    #[allow(dead_code)]
+    pub(crate) fn get_sk_gsw(&self) -> &PolyMatrixRaw<'a> {
+        &self.sk_gsw
+    }
+
     fn get_fresh_gsw_public_key(
         &self,
         m: usize,
         rng: &mut ChaCha20Rng,
         rng_pub: &mut ChaCha20Rng,
     ) -> PolyMatrixRaw<'a> {
         let params = self.params;
@@ -493,57 +527,71 @@
         } else {
             self.generate_secret_keys_from_seed(seed);
             None
         }
     }
 
     fn generate_secret_keys_impl(&mut self, rng: &mut ChaCha20Rng) {
-        self.dg.sample_matrix(&mut self.sk_gsw, rng);
-        self.dg.sample_matrix(&mut self.sk_reg, rng);
+        gen_ternary_mat(&mut self.sk_gsw, HAMMING_WEIGHT, rng);
+        gen_ternary_mat(&mut self.sk_reg, HAMMING_WEIGHT, rng);
         self.sk_gsw_full = matrix_with_identity(&self.sk_gsw);
         self.sk_reg_full = matrix_with_identity(&self.sk_reg);
     }
 
     fn generate_keys_impl(&mut self, rng: &mut ChaCha20Rng) -> PublicParameters<'a> {
         let params = self.params;
 
         self.generate_secret_keys_impl(rng);
         let sk_reg_ntt = to_ntt_alloc(&self.sk_reg);
+        let sk_gsw_ntt = to_ntt_alloc(&self.sk_gsw);
 
         let mut rng = ChaCha20Rng::from_entropy();
         let mut pp = PublicParameters::init(params);
         let pp_seed = rng.gen();
         pp.seed = Some(pp_seed);
         let mut rng_pub = ChaCha20Rng::from_seed(pp_seed);
 
         // Params for packing
         let gadget_conv = build_gadget(params, 1, params.t_conv);
         let gadget_conv_ntt = to_ntt_alloc(&gadget_conv);
-        for i in 0..params.n {
+        let num_packing_mats = if params.version == 0 { params.n } else { 1 };
+        for i in 0..num_packing_mats {
             let scaled = scalar_multiply_alloc(&sk_reg_ntt, &gadget_conv_ntt);
             let mut ag = PolyMatrixNTT::zero(params, params.n, params.t_conv);
             ag.copy_into(&scaled, i, 0);
             let w = self.encrypt_matrix_gsw(&ag, &mut rng, &mut rng_pub);
             pp.v_packing.push(w);
         }
 
+        if params.version > 0 {
+            let scaled = &sk_gsw_ntt * &gadget_conv_ntt;
+            let scaled_rotated = shift_rows_by_one(&scaled);
+            let w = self.encrypt_matrix_gsw(&scaled_rotated, &mut rng, &mut rng_pub);
+            pp.v_packing.push(w);
+        }
+
         if params.expand_queries {
             // Params for expansion
             pp.v_expansion_left = Some(self.generate_expansion_params(
                 params.g(),
                 params.t_exp_left,
                 &mut rng,
                 &mut rng_pub,
             ));
-            pp.v_expansion_right = Some(self.generate_expansion_params(
-                params.stop_round() + 1,
-                params.t_exp_right,
-                &mut rng,
-                &mut rng_pub,
-            ));
+
+            if params.version == 0 || params.t_exp_right != params.t_exp_left {
+                pp.v_expansion_right = Some(self.generate_expansion_params(
+                    params.stop_round() + 1,
+                    params.t_exp_right,
+                    &mut rng,
+                    &mut rng_pub,
+                ));
+            } else {
+                pp.v_expansion_right = None;
+            }
 
             // Params for converison
             let g_conv = build_gadget(params, 2, 2 * params.t_conv);
             let sk_reg_ntt = self.sk_reg.ntt();
             let sk_reg_squared_ntt = &sk_reg_ntt * &sk_reg_ntt;
             pp.v_conversion = Some(Vec::from_iter(once(PolyMatrixNTT::zero(
                 params,
@@ -799,17 +847,15 @@
 
     fn public_parameters_serialization_is_correct_for_params(params: Params) {
         let mut client = Client::init(&params);
         let pub_params = client.generate_keys();
 
         let serialized1 = pub_params.serialize();
         let deserialized1 = PublicParameters::deserialize(&params, &serialized1);
-        let serialized2 = deserialized1.serialize();
 
-        assert_eq!(serialized1, serialized2);
         assert_eq!(
             get_vec(&pub_params.v_packing),
             get_vec(&deserialized1.v_packing)
         );
 
         println!(
             "packing mats (bytes) {}",
```

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/discrete_gaussian.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/discrete_gaussian.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/gadget.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/gadget.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/key_value.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/key_value.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/ntt.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/ntt.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/number_theory.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/number_theory.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/params.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/params.rs`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,16 @@
     pub t_gsw: usize,
 
     pub expand_queries: bool,
     pub db_dim_1: usize,
     pub db_dim_2: usize,
     pub instances: usize,
     pub db_item_size: usize,
+
+    pub version: usize,
 }
 
 impl Params {
     pub fn get_ntt_forward_table(&self, i: usize) -> &[u64] {
         self.ntt_tables[i][0].as_slice()
     }
     pub fn get_ntt_forward_prime_table(&self, i: usize) -> &[u64] {
@@ -140,22 +142,27 @@
             2
         }
     }
 
     pub fn setup_bytes(&self) -> usize {
         let mut sz_polys = 0;
 
+        let num_packing_mats = if self.version == 0 { self.n } else { 2 };
         let packing_sz = ((self.n + 1) - 1) * self.t_conv;
-        sz_polys += self.n * packing_sz;
+        sz_polys += num_packing_mats * packing_sz;
 
         if self.expand_queries {
             let expansion_left_sz = self.g() * self.t_exp_left;
-            let expansion_right_sz = (self.stop_round() + 1) * self.t_exp_right;
+            let mut expansion_right_sz = (self.stop_round() + 1) * self.t_exp_right;
             let conversion_sz = 2 * self.t_conv;
 
+            if self.version > 0 && self.t_exp_left == self.t_exp_right {
+                expansion_right_sz = 0;
+            }
+
             sz_polys += expansion_left_sz + expansion_right_sz + conversion_sz;
         }
 
         let sz_bytes = sz_polys * self.poly_len * size_of::<u64>();
         SEED_LENGTH + sz_bytes
     }
 
@@ -226,14 +233,15 @@
         t_exp_right: usize,
         t_gsw: usize,
         expand_queries: bool,
         db_dim_1: usize,
         db_dim_2: usize,
         instances: usize,
         db_item_size: usize,
+        version: usize,
     ) -> Self {
         assert!(q2_bits >= MIN_Q2_BITS);
 
         let poly_len_log2 = log2(poly_len as u64) as usize;
         let crt_count = moduli.len();
         assert!(crt_count <= MAX_MODULI);
         let mut moduli_array = [0; MAX_MODULI];
@@ -279,10 +287,11 @@
             t_exp_right,
             t_gsw,
             expand_queries,
             db_dim_1,
             db_dim_2,
             instances,
             db_item_size,
+            version,
         }
     }
 }
```

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/poly.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/poly.rs`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,25 @@
 
 impl<'a> PolyMatrixNTT<'a> {
     pub fn raw(&self) -> PolyMatrixRaw<'a> {
         from_ntt_alloc(&self)
     }
 }
 
+pub fn shift_rows_by_one<'a>(inp: &PolyMatrixNTT<'a>) -> PolyMatrixNTT<'a> {
+    if inp.rows == 1 {
+        return inp.clone();
+    }
+
+    let all_but_last_row = inp.submatrix(0, 0, inp.rows - 1, inp.cols);
+    let last_row = inp.submatrix(inp.rows - 1, 0, 1, inp.cols);
+    let out = stack_ntt(&last_row, &all_but_last_row);
+    out
+}
+
 pub fn multiply_poly(params: &Params, res: &mut [u64], a: &[u64], b: &[u64]) {
     for c in 0..params.crt_count {
         for i in 0..params.poly_len {
             let idx = c * params.poly_len + i;
             res[idx] = multiply_modular(params, a[idx], b[idx], c);
         }
     }
@@ -549,14 +560,22 @@
     assert_eq!(a.cols, b.cols);
     let mut c = PolyMatrixRaw::zero(a.params, a.rows + b.rows, a.cols);
     c.copy_into(a, 0, 0);
     c.copy_into(b, a.rows, 0);
     c
 }
 
+pub fn stack_ntt<'a>(a: &PolyMatrixNTT<'a>, b: &PolyMatrixNTT<'a>) -> PolyMatrixNTT<'a> {
+    assert_eq!(a.cols, b.cols);
+    let mut c = PolyMatrixNTT::zero(a.params, a.rows + b.rows, a.cols);
+    c.copy_into(a, 0, 0);
+    c.copy_into(b, a.rows, 0);
+    c
+}
+
 pub fn scalar_multiply(res: &mut PolyMatrixNTT, a: &PolyMatrixNTT, b: &PolyMatrixNTT) {
     assert_eq!(a.rows, 1);
     assert_eq!(a.cols, 1);
 
     let params = res.params;
     let pol2 = a.get_poly(0, 0);
     for i in 0..b.rows {
```

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/server.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/server.rs`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 use std::io::Seek;
 use std::io::SeekFrom;
 
 use crate::aligned_memory::*;
 use crate::arith::*;
 use crate::client::PublicParameters;
 use crate::client::Query;
+use crate::client::CLIENT_TEST;
 use crate::gadget::*;
 use crate::params::*;
 use crate::poly::*;
 use crate::util::*;
 
 use rayon::prelude::*;
 
@@ -541,15 +542,15 @@
     for _ in 0..(1 << g) {
         v.push(PolyMatrixNTT::zero(params, 2, 1));
     }
     v[0].copy_into(&query.ct.as_ref().unwrap().ntt(), 0, 0);
 
     let v_conversion = &public_params.v_conversion.as_ref().unwrap()[0];
     let v_w_left = public_params.v_expansion_left.as_ref().unwrap();
-    let v_w_right = public_params.v_expansion_right.as_ref().unwrap();
+    let v_w_right = public_params.v_expansion_right.as_ref().unwrap_or(v_w_left);
     let v_neg1 = params.get_v_neg1();
 
     let mut v_reg_inp = Vec::with_capacity(dim0);
     let mut v_gsw_inp = Vec::with_capacity(right_expanded);
     if further_dims > 0 {
         coefficient_expansion(
             &mut v,
@@ -585,14 +586,71 @@
     }
 
     regev_to_gsw(&mut v_folding, &v_gsw_inp, &v_conversion, params, 1, 0);
 
     (v_reg_reoriented, v_folding)
 }
 
+pub fn variance(v: Vec<i64>) -> f64 {
+    let n = v.len();
+    let mean = v.iter().map(|x| *x as f64).sum::<f64>() / n as f64;
+    println!("mean: {}", mean.abs().log2());
+    let mut sum = 0.0;
+    for i in 0..n {
+        // println!(":: {}", (v[i] as f64).abs().log2());
+        sum += (v[i] as f64 - mean).powi(2);
+    }
+    sum / n as f64
+}
+
+fn dec_to_raw<'a>(
+    params: &'a Params,
+    poly: &PolyMatrixRaw<'a>,
+    target: &PolyMatrixRaw<'a>,
+) -> PolyMatrixRaw<'a> {
+    let mut out = PolyMatrixRaw::zero(params, poly.rows, poly.cols);
+    let scale_k = params.modulus / params.pt_modulus;
+    let mut noises = Vec::new();
+    for z in 0..poly.data.len() {
+        let mut val = poly.data[z] as i64;
+        if val > (params.modulus / 2) as i64 {
+            val -= params.modulus as i64;
+        }
+        let mut val_rounded = f64::round(val as f64 / scale_k as f64) as i64;
+
+        let mut target_val = target.data[z] as i64;
+        if target_val >= (params.pt_modulus / 2) as i64 {
+            target_val -= params.pt_modulus as i64;
+        }
+        let target_val_scaled = target_val * scale_k as i64;
+
+        let mut noise = val - target_val_scaled;
+        // this seems fragile
+        if noise.abs() >= (params.pt_modulus * scale_k / 2) as i64 {
+            noise -= (params.pt_modulus * scale_k) as i64;
+        }
+        noises.push(noise);
+
+        if val_rounded < 0 {
+            val_rounded += params.pt_modulus as i64;
+        }
+
+        let result_val = (val_rounded as u64) % params.modulus;
+
+        out.data[z] = result_val;
+    }
+
+    println!(
+        "Noise width (s^2, log2): {}",
+        (2.0 * std::f64::consts::PI * variance(noises)).log2()
+    );
+
+    out
+}
+
 pub fn process_query(
     params: &Params,
     public_params: &PublicParameters,
     query: &Query,
     db: &[u64],
 ) -> Vec<u8> {
     let dim0 = 1 << params.db_dim_1;
@@ -617,15 +675,15 @@
             .unwrap()
             .iter()
             .map(|x| x.ntt())
             .collect();
     }
     let v_folding_neg = get_v_folding_neg(params, &v_folding);
 
-    let v_packed_ct = (0..params.instances)
+    let v_packed_ct: Vec<PolyMatrixRaw> = (0..params.instances)
         .into_par_iter()
         .map(|instance| {
             let mut intermediate = Vec::with_capacity(num_per);
             let mut intermediate_raw = Vec::with_capacity(num_per);
             for _ in 0..num_per {
                 intermediate.push(PolyMatrixNTT::zero(params, 2, 1));
                 intermediate_raw.push(PolyMatrixRaw::zero(params, 2, 1));
@@ -648,14 +706,32 @@
 
                 for i in 0..intermediate.len() {
                     from_ntt(&mut intermediate_raw[i], &intermediate[i]);
                 }
 
                 fold_ciphertexts(params, &mut intermediate_raw, &v_folding, &v_folding_neg);
 
+                if instance == 0 && trial == 0 {
+                    unsafe {
+                        if let Some((sk_reg, target)) = &CLIENT_TEST {
+                            let ct = intermediate_raw[0].ntt();
+                            let ct_subset = ct.submatrix(0, 0, 2, 1);
+                            let dec = (&sk_reg.ntt() * &ct_subset).raw();
+                            let dec_raw = dec_to_raw(params, &dec, target);
+                            for i in 0..params.poly_len {
+                                assert_eq!(
+                                    dec_raw.data[i], target.data[i],
+                                    "{} != {} at {}",
+                                    dec_raw.data[i], target.data[i], i
+                                );
+                            }
+                        }
+                    }
+                }
+
                 v_ct.push(intermediate_raw[0].clone());
             }
 
             let packed_ct = pack(params, &v_ct, &v_packing);
 
             packed_ct.raw()
         })
@@ -915,31 +991,55 @@
             1
         );
     }
 
     fn full_protocol_is_correct_for_params(params: &Params) {
         let mut seeded_rng = get_seeded_rng();
 
-        let target_idx = seeded_rng.gen::<usize>() % (params.db_dim_1 + params.db_dim_2);
+        let target_idx = seeded_rng.gen::<usize>() % (1 << (params.db_dim_1 + params.db_dim_2));
+        println!("target_idx: {}", target_idx);
 
         let mut client = Client::init(&params);
 
         let public_params = client.generate_keys();
+        let pp_serialized = public_params.serialize();
+        println!("pp size: {}", pp_serialized.len());
+        let pp = PublicParameters::deserialize(params, &pp_serialized);
         let query = client.generate_query(target_idx);
 
         let (corr_item, db) = generate_random_db_and_get_item(params, target_idx);
 
-        let response = process_query(params, &public_params, &query, db.as_slice());
+        unsafe {
+            let params_static = Box::leak(Box::new(params.clone()));
+            let mut corr_item_static =
+                PolyMatrixRaw::zero(params_static, corr_item.rows, corr_item.cols);
+            corr_item_static
+                .data
+                .as_mut_slice()
+                .copy_from_slice(corr_item.data.as_slice());
+            let sk_reg_full = matrix_with_identity(client.get_sk_reg());
+            let mut sk_reg_static =
+                PolyMatrixRaw::zero(params_static, sk_reg_full.rows, sk_reg_full.cols);
+            sk_reg_static
+                .data
+                .as_mut_slice()
+                .copy_from_slice(sk_reg_full.as_slice());
+            CLIENT_TEST = Some((sk_reg_static, corr_item_static));
+        }
+
+        let response = process_query(params, &pp, &query, db.as_slice());
+        println!("response size: {}", response.len());
 
         let result = client.decode_response(response.as_slice());
 
         let p_bits = log2_ceil(params.pt_modulus) as usize;
         let corr_result = corr_item.to_vec(p_bits, params.modp_words_per_chunk());
 
         assert_eq!(result.len(), corr_result.len());
+        println!("res len: {}", result.len());
 
         for z in 0..corr_result.len() {
             assert_eq!(result[z], corr_result[z], "at {:?}", z);
         }
     }
 
     #[test]
@@ -947,28 +1047,27 @@
         full_protocol_is_correct_for_params(&get_params());
     }
 
     #[test]
     #[ignore]
     fn larger_full_protocol_is_correct() {
         let cfg_expand = r#"
-            {
-            'n': 2,
-            'nu_1': 10,
-            'nu_2': 6,
-            'p': 512,
-            'q2_bits': 21,
-            's_e': 85.83255142749422,
-            't_gsw': 10,
-            't_conv': 4,
-            't_exp_left': 16,
-            't_exp_right': 56,
-            'instances': 1,
-            'db_item_size': 9000 }
+        {
+            "n": 2,
+            "nu_1": 9,
+            "nu_2": 5,
+            "p": 256,
+            "q2_bits": 22,
+            "t_gsw": 7,
+            "t_conv": 3,
+            "t_exp_left": 5,
+            "t_exp_right": 5,
+            "instances": 4,
+            "db_item_size": 32768
+        }
         "#;
         let cfg = cfg_expand;
-        let cfg = cfg.replace("'", "\"");
         let params = params_from_json(&cfg);
 
         full_protocol_is_correct_for_params(&params);
     }
 }
```

### Comparing `blyss-0.1.7/local_dependencies/spiral-rs/src/util.rs` & `blyss-0.1.8/local_dependencies/spiral-rs/src/util.rs`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         56,
         8,
         true,
         9,
         6,
         1,
         2048,
+        0,
     )
 }
 
 pub fn get_short_keygen_params() -> Params {
     Params::init(
         2048,
         &vec![268369921u64, 249561089u64],
@@ -93,14 +94,15 @@
         4,
         4,
         true,
         9,
         6,
         1,
         2048,
+        0,
     )
 }
 
 pub fn get_expansion_testing_params() -> Params {
     let cfg = r#"
         {'n': 2,
         'nu_1': 9,
@@ -206,14 +208,15 @@
         t_exp_right: 0,
         t_gsw: 0,
         expand_queries: false,
         db_dim_1: 0,
         db_dim_2: 0,
         instances: 0,
         db_item_size: 0,
+        version: 0,
     }
 }
 
 pub fn params_from_json(cfg: &str) -> Params {
     let v: Value = serde_json::from_str(cfg).unwrap();
     params_from_json_obj(&v)
 }
@@ -232,14 +235,17 @@
     let do_expansion = v.get("direct_upload").is_none();
 
     let mut db_item_size = v["db_item_size"].as_u64().unwrap_or(0) as usize;
     if db_item_size == 0 {
         db_item_size = instances * n * n;
         db_item_size = db_item_size * 2048 * log2_ceil(p) as usize / 8;
     }
+
+    let version = v["version"].as_u64().unwrap_or(0) as usize;
+
     Params::init(
         2048,
         &vec![268369921u64, 249561089u64],
         6.4,
         n,
         p,
         q2_bits,
@@ -248,14 +254,15 @@
         t_exp_right,
         t_gsw,
         do_expansion,
         db_dim_1,
         db_dim_2,
         instances,
         db_item_size,
+        version,
     )
 }
 
 static ALL_PARAMS_STORE_FNAME: &str = "../params_store.json";
 
 pub fn get_params_from_store(target_num_log2: usize, item_size: usize) -> Params {
     let params_store_str = fs::read_to_string(ALL_PARAMS_STORE_FNAME).unwrap();
@@ -381,14 +388,15 @@
             56,
             8,
             true,
             9,
             6,
             1,
             2048,
+            0,
         );
         assert_eq!(b, c);
     }
 
     #[test]
     fn test_decompose_calc_correct() {
         let lengths = [5, 4, 3];
```

### Comparing `blyss-0.1.7/.gitignore` & `blyss-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/blyss/api.py` & `blyss-0.1.8/blyss/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 import logging
 import base64
 
 from blyss.req_compression import get_session
 from blyss.bloom import BloomFilter
 
 CREATE_PATH = "/create"
+MODIFY_PATH = "/modify"
 DESTROY_PATH = "/destroy"
+CLEAR_PATH = "/clear"
 CHECK_PATH = "/check"
 LIST_BUCKETS_PATH = "/list-buckets"
 DELETE_PATH = "/delete"
 META_PATH = "/meta"
 BLOOM_PATH = "/bloom"
 LIST_KEYS_PATH = "/list-keys"
 SETUP_PATH = "/setup"
@@ -204,14 +206,24 @@
         """
         return _get_data_json(self.api_key, self._service_url_for(LIST_BUCKETS_PATH))
 
     # Bucket-specific methods
     def _url_for(self, bucket_name: str, path: str) -> str:
         return self.service_endpoint + "/" + bucket_name + path
 
+    def modify(self, bucket_name: str, data_json: str) -> dict[Any, Any]:
+        """Modify existing bucket.
+         
+        Args:
+            data_json (str): same as create.
+        """
+        return _post_data_json(
+            self.api_key, self._url_for(bucket_name, MODIFY_PATH), data_json
+        )
+
     def meta(self, bucket_name: str) -> dict[Any, Any]:
         """Get metadata about a bucket.
 
         Returns:
             dict: Metadata about a bucket.
         """
         return _get_data_json(self.api_key, self._url_for(bucket_name, META_PATH))
@@ -254,14 +266,18 @@
         """List all keys in this bucket."""
         return _get_data_json(self.api_key, self._url_for(bucket_name, LIST_KEYS_PATH))
 
     def destroy(self, bucket_name: str):
         """Destroy this bucket."""
         _post_data(self.api_key, self._url_for(bucket_name, DESTROY_PATH), "")
 
+    def clear(self, bucket_name: str):
+        """Delete all keys in this bucket."""
+        _post_data(self.api_key, self._url_for(bucket_name, CLEAR_PATH), "")
+
     def write(self, bucket_name: str, data: bytes):
         """Write some data to this bucket."""
         _post_data(self.api_key, self._url_for(bucket_name, WRITE_PATH), data)
 
     async def async_write(self, bucket_name: str, data: str):
         """Write JSON payload to this bucket."""
         await _async_post_data(
```

### Comparing `blyss-0.1.7/blyss/bloom.py` & `blyss-0.1.8/blyss/bloom.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/blyss/blyss_lib.py` & `blyss-0.1.8/blyss/blyss_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 INTERNAL
 
 This Python module is the *only* code that interfaces with
 the compiled Rust code.
 """
 
 
-from typing import Any
+from typing import Any, Optional
 from . import blyss, seed  # type: ignore
 
 # NB:   There are many "type: ignore"s on purpose. Type information
 #       for the maturin output is difficult to include nicely, so we just wrap it here.
 
 
 class BlyssLib:
@@ -78,25 +78,29 @@
             response (bytes): The raw PIR response from the server.
 
         Returns:
             bytes: The plaintext data in the response.
         """
         return bytes(blyss.decode_response(self.inner_client, response))  # type: ignore
 
-    def extract_result(self, key: str, data: bytes) -> bytes:
+    def extract_result(self, key: str, data: bytes) -> Optional[bytes]:
         """Extracts the value for a given key, given the plaintext data from a response.
 
         Args:
             key (str): The key the client is looking up.
             data (bytes): The plaintext data from the PIR response.
 
         Returns:
             bytes: The plaintext data corresponding to the given key.
         """
-        return bytes(blyss.extract_result(self.inner_client, key, data))  # type: ignore
+        r = blyss.extract_result(self.inner_client, key, data)
+        if r is None:
+            return None
+        else:
+            return bytes(r)
 
     def __init__(self, params: str, secret_seed: str):
         """Initializes a new BlyssLib instance.
 
         Args:
             params (str): The set of JSON parameters for the underlying PIR scheme.
             secret_seed (str): A base64-encoded secret seed that is used to derive all client secrets.
```

### Comparing `blyss-0.1.7/blyss/bucket.py` & `blyss-0.1.8/blyss/bucket.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 value_str = base64.b64encode(value).decode("utf-8")
                 fmt = {
                     "key": key,
                     "value": value_str,
                     "content-type": "application/octet-stream",
                 }
                 row.append(fmt)
-                row_size += int(72 + len(key) + len(value_str))
+                row_size += int(24 + len(key) + len(value_str) + 48)
 
             # if the new row doesn't fit into the current chunk, start a new one
             if current_chunk_size + row_size > _MAX_PAYLOAD:
                 kv_chunks.append(current_chunk)
                 current_chunk = row
                 current_chunk_size = row_size
             else:
@@ -207,14 +207,22 @@
     def info(self) -> dict[Any, Any]:
         """Gets info on this bucket from the service."""
         return self.api.meta(self.name)
 
     def list_keys(self) -> dict[str, Any]:
         """Gets info on all keys in this bucket."""
         return self.api.list_keys(self.name)
+    
+    def rename(self, new_name: str):
+        """Renames this bucket."""
+        bucket_create_req = {
+            "name": new_name,
+        }
+        self.api.modify(self.name, json.dumps(bucket_create_req))
+        self.name = new_name
 
     def write(self, kv_pairs: dict[str, Union[tuple[Any, Optional[Any]], Any]]):
         """Writes the supplied key-value pair(s) into the bucket.
 
         To supply metadata for a key, set the value in
         the dict to a tuple of (value_to_write, metadata).
 
@@ -247,14 +255,22 @@
         """
         self.api.delete_key(self.name, key)
 
     def destroy_entire_bucket(self):
         """Destroys the entire bucket. This action is permanent and irreversible."""
         self.api.destroy(self.name)
 
+    def clear_entire_bucket(self):
+        """Deletes all keys in this bucket. This action is permanent and irreversible.
+        
+        Differs from destroy in that the bucket's metadata 
+        (e.g. permissions, PIR scheme parameters, and clients' setup data) are preserved.
+        """
+        self.api.clear(self.name)
+
     def private_read(self, keys: Union[str, list[str]]) -> Union[bytes, list[bytes]]:
         """Privately reads the supplied key from the bucket,
         returning the value corresponding to the key.
 
         No entity, including the Blyss service, should be able to
         determine which key(s) this method was called for.
```

### Comparing `blyss-0.1.7/blyss/bucket_service.py` & `blyss-0.1.8/blyss/bucket_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Optional, Union
 from . import bucket, api, seed
 import json
 
 BLYSS_BUCKET_URL = "https://beta.api.blyss.dev"
-DEFAULT_BUCKET_PARAMETERS = {"maxItemSize": 1000}
+DEFAULT_BUCKET_PARAMETERS = {"maxItemSize": 1000, "keyStoragePolicy": "bloom"}
 
 ApiConfig = dict[str, str]
 
 
 class BucketService:
     """A class representing a client to the Blyss bucket service."""
```

### Comparing `blyss-0.1.7/blyss/req_compression.py` & `blyss-0.1.8/blyss/req_compression.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/blyss/seed.py` & `blyss-0.1.8/blyss/seed.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/blyss/serializer.py` & `blyss-0.1.8/blyss/serializer.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/blyss/varint.py` & `blyss-0.1.8/blyss/varint.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/src/lib.rs` & `blyss-0.1.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.7/Cargo.lock` & `blyss-0.1.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "blyss-client-python"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "pyo3",
  "spiral-rs",
 ]
 
 [[package]]
 name = "bumpalo"
@@ -346,15 +346,15 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "spiral-rs"
-version = "0.2.0"
+version = "0.2.1-alpha.2"
 dependencies = [
  "getrandom",
  "rand",
  "rand_chacha",
  "serde_json",
  "sha2",
  "subtle",
```

