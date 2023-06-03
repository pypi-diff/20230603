# Comparing `tmp/MarsGT-0.1.3.tar.gz` & `tmp/MarsGT-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MarsGT-0.1.3.tar", last modified: Sat Jun  3 07:35:29 2023, max compression
+gzip compressed data, was "dist/MarsGT-0.1.4.tar", last modified: Sat Jun  3 08:51:34 2023, max compression
```

## Comparing `MarsGT-0.1.3.tar` & `MarsGT-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:35:29.373832 MarsGT-0.1.3/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.3/MANIFEST.in
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:35:29.349812 MarsGT-0.1.3/MarsGT/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.3/MarsGT/__init__.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 06:21:55.000000 MarsGT-0.1.3/MarsGT/conv.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6007 2023-06-03 06:21:56.000000 MarsGT-0.1.3/MarsGT/egrn.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21321 2023-06-03 06:21:56.000000 MarsGT-0.1.3/MarsGT/marsgt_model.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7786 2023-06-03 06:21:57.000000 MarsGT-0.1.3/MarsGT/utils.py
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 07:35:29.367813 MarsGT-0.1.3/MarsGT.egg-info/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/SOURCES.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/dependency_links.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      317 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/requires.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-06-03 07:35:29.000000 MarsGT-0.1.3/MarsGT.egg-info/top_level.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 07:35:29.371821 MarsGT-0.1.3/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      730 2023-06-03 06:21:54.000000 MarsGT-0.1.3/README.md
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-06-03 07:35:29.374813 MarsGT-0.1.3/setup.cfg
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1071 2023-06-03 07:33:41.000000 MarsGT-0.1.3/setup.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 08:51:34.314496 MarsGT-0.1.4/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.4/MANIFEST.in
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 08:51:34.262496 MarsGT-0.1.4/MarsGT/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.4/MarsGT/__init__.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 08:36:23.000000 MarsGT-0.1.4/MarsGT/conv.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     5909 2023-06-03 08:36:23.000000 MarsGT-0.1.4/MarsGT/egrn.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21360 2023-06-03 08:36:23.000000 MarsGT-0.1.4/MarsGT/marsgt_model.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7786 2023-06-03 08:36:23.000000 MarsGT-0.1.4/MarsGT/utils.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-06-03 08:51:34.290496 MarsGT-0.1.4/MarsGT.egg-info/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 08:51:34.000000 MarsGT-0.1.4/MarsGT.egg-info/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-06-03 08:51:34.000000 MarsGT-0.1.4/MarsGT.egg-info/SOURCES.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-06-03 08:51:34.000000 MarsGT-0.1.4/MarsGT.egg-info/dependency_links.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      335 2023-06-03 08:51:34.000000 MarsGT-0.1.4/MarsGT.egg-info/requires.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-06-03 08:51:34.000000 MarsGT-0.1.4/MarsGT.egg-info/top_level.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1024 2023-06-03 08:51:34.313493 MarsGT-0.1.4/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      730 2023-06-03 06:21:54.000000 MarsGT-0.1.4/README.md
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-06-03 08:51:34.315498 MarsGT-0.1.4/setup.cfg
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1099 2023-06-03 08:51:21.000000 MarsGT-0.1.4/setup.py
```

### Comparing `MarsGT-0.1.3/MarsGT/conv.py` & `MarsGT-0.1.4/MarsGT/conv.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.3/MarsGT/egrn.py` & `MarsGT-0.1.4/MarsGT/egrn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-import numpy as np
-import scipy.sparse as sp
-import anndata as ad
-from collections import Counter
-import pandas as pd
-
-
-def peak_Sparse(peak_feature, gene_feature, device):
-    # Find the non-zero elements in peak_feature
-    peak_row = torch.where(peak_feature != 0)[0].to(device)
-    peak_col = torch.where(peak_feature != 0)[1].to(device)
-    peak_data = peak_feature[torch.where(peak_feature != 0)]
-
-    # Initialize tensors for combined peak data
-    peak_combine_row = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]), dtype=torch.int32)
-    peak_combine_col = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]), dtype=torch.int32)
-    peak_combine_data = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]))
-
-    non_count = 0
-    for peak_num in range(peak_feature.shape[0]):
-        # Calculate the peak sum
-        peak_sum = len(peak_row[peak_row == peak_num])
-
-        # Initialize a tensor for peak indices
-        peak_init = torch.zeros((gene_feature.shape[0], peak_sum), dtype=torch.int32).to(device)
-        for id in range(gene_feature.shape[0]):
-            peak_init[id,] = id + peak_num * gene_feature.shape[0]
-
-        # Update the combined peak data tensors
-        peak_combine_row[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_row[peak_row == peak_num] + peak_init - peak_num).reshape(1, -1)
-        peak_combine_col[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_col[peak_row == peak_num]).repeat(gene_feature.shape[0])
-        peak_combine_data[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_data[peak_row == peak_num]).repeat(gene_feature.shape[0])
-
-        non_count += peak_sum * gene_feature.shape[0]
-
-    # Create the final sparse peak_feature tensor
-    peak_feature_ori = torch.sparse.FloatTensor(torch.vstack((peak_combine_row, peak_combine_col)).long(), peak_combine_data, torch.Size((gene_feature.shape[0] * peak_feature.shape[0], peak_feature.shape[1])))
-    return peak_feature_ori.to(device)
-
-
-def gene_Sparse(peak_feature, gene_feature, device):
-    # Find the non-zero elements in gene_feature
-    gene_row = torch.where(gene_feature != 0)[0].to(device)
-    gene_col = torch.where(gene_feature != 0)[1].to(device)
-    gene_data = gene_feature[torch.where(gene_feature != 0)]
-
-    # Initialize a tensor for gene indices
-    gene_init = torch.zeros((peak_feature.shape[0], len(gene_row)), dtype=torch.int32).to(device)
-    for peak_id in range(peak_feature.shape[0]):
-        gene_init[peak_id] = gene_row + peak_id * gene_feature.shape[0]
-
-    # Update the combined gene data tensors
-    gene_combine_row = gene_init.reshape(1, -1)[0]
-    gene_combine_col = gene_col.repeat(1, peak_feature.shape[0])[0]
-    gene_combine_data = gene_data.repeat(peak_feature.shape[0])
-
-    # Create the final sparse gene_feature tensor
-    gene_feature_ori = torch.sparse.FloatTensor(torch.vstack((gene_combine_row, gene_combine_col)), gene_combine_data, torch.Size((gene_feature.shape[0] * peak_feature.shape[0], gene_feature.shape[1])))
-    return gene_feature_ori
-
-
-def gene_Peak_Score(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names):
-    y = ad.AnnData(RNA_matrix.transpose(), dtype='int32')
-    y.var_names=gene_names[0]
-    y.obs['pred'] = np.array(pred_label,dtype='int64')
-    y.obs['pred'] = y.obs['pred'].astype("category")
-    # Store the prediction results as a sparse matrix, where rows represent cells and columns represent cluster labels. A value of 1 at the corresponding position indicates that the cell belongs to that cluster.
-    cell_emb_binary = sp.coo_matrix((np.ones(len(y.obs['pred'])),(np.array(range(len(y.obs['pred']))),list(y.obs['pred']))))
-    cell_emb_binary.todense()
-
-    adata_atac_all = ATAC_matrix[:,nodes_id]
-    adata_rna_all = RNA_matrix[:,nodes_id]
-
-    ATAC_matrix_ct = adata_atac_all*(cell_emb_binary)
-    RNA_matrix_ct = adata_rna_all*(cell_emb_binary)
-    RNA_matrix_ct = RNA_matrix_ct/np.sum(cell_emb_binary,axis=0)
-    ATAC_matrix_ct = ATAC_matrix_ct/np.sum(cell_emb_binary,axis=0)
-
-    rna_matrix = RNA_matrix_ct
-    m = range(rna_matrix.shape[0])
-    gene_peak = RP_matrix
-    gp = gene_peak.reshape(gene_peak.shape[1]*rna_matrix.shape[0],1).todense()
-    gene_emb_enh = ATAC_matrix_ct[list(range (ATAC_matrix_ct.shape[0]))*rna_matrix.shape[0]]
-    peak_emb_enh = RNA_matrix_ct[[v for v in m for i in range(ATAC_matrix_ct.shape[0])]]
-    egrn = np.multiply(gene_emb_enh, peak_emb_enh)
-    egrn = np.multiply(egrn,gp)
-    return egrn
-
-def egrn_calculate(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names,peak_names,threshold=0):
-    print('We are currently performing calculations for EGRN. Please bear with us as this process will take approximately around 10 minutes.')
-    egrn = gene_Peak_Score(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names)
-    label_num = len(Counter(pred_label))
-    print('class_num:',label_num)
-    gn = np.array(gene_names[0])[[v for v in range(RNA_matrix.shape[0]) for i in range(ATAC_matrix.shape[0])]]
-    pn = np.array(peak_names[0])[list(range (ATAC_matrix.shape[0]))*RNA_matrix.shape[0]]
-    egrn_df = pd.DataFrame(columns=['gene', 'peak', 'score', 'class'])
-    print('We are currently conducting filtering and categorization operations.')
-    for i in range(label_num):
-        data = np.array(np.squeeze(egrn[:,i]))[0]
-        gene_peak_score_Dict = {'gene': gn, 'peak': pn, 'score':data}
-        gene_peak_score_df = pd.DataFrame(data = gene_peak_score_Dict)
-        gene_peak_score = gene_peak_score_df[gene_peak_score_df['score'] >threshold]
-        gene_peak_score = gene_peak_score.drop_duplicates(['gene','peak'])
-        gene_peak_score = gene_peak_score.sort_values(by="score",ascending=False)
-        gene_peak_score['class'] = i
-        egrn_df = egrn_df.append(gene_peak_score)
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+import numpy as np
+import scipy.sparse as sp
+import anndata as ad
+from collections import Counter
+import pandas as pd
+
+
+def peak_Sparse(peak_feature, gene_feature, device):
+    # Find the non-zero elements in peak_feature
+    peak_row = torch.where(peak_feature != 0)[0].to(device)
+    peak_col = torch.where(peak_feature != 0)[1].to(device)
+    peak_data = peak_feature[torch.where(peak_feature != 0)]
+
+    # Initialize tensors for combined peak data
+    peak_combine_row = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]), dtype=torch.int32)
+    peak_combine_col = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]), dtype=torch.int32)
+    peak_combine_data = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]))
+
+    non_count = 0
+    for peak_num in range(peak_feature.shape[0]):
+        # Calculate the peak sum
+        peak_sum = len(peak_row[peak_row == peak_num])
+
+        # Initialize a tensor for peak indices
+        peak_init = torch.zeros((gene_feature.shape[0], peak_sum), dtype=torch.int32).to(device)
+        for id in range(gene_feature.shape[0]):
+            peak_init[id,] = id + peak_num * gene_feature.shape[0]
+
+        # Update the combined peak data tensors
+        peak_combine_row[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_row[peak_row == peak_num] + peak_init - peak_num).reshape(1, -1)
+        peak_combine_col[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_col[peak_row == peak_num]).repeat(gene_feature.shape[0])
+        peak_combine_data[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_data[peak_row == peak_num]).repeat(gene_feature.shape[0])
+
+        non_count += peak_sum * gene_feature.shape[0]
+
+    # Create the final sparse peak_feature tensor
+    peak_feature_ori = torch.sparse.FloatTensor(torch.vstack((peak_combine_row, peak_combine_col)).long(), peak_combine_data, torch.Size((gene_feature.shape[0] * peak_feature.shape[0], peak_feature.shape[1])))
+    return peak_feature_ori.to(device)
+
+
+def gene_Sparse(peak_feature, gene_feature, device):
+    # Find the non-zero elements in gene_feature
+    gene_row = torch.where(gene_feature != 0)[0].to(device)
+    gene_col = torch.where(gene_feature != 0)[1].to(device)
+    gene_data = gene_feature[torch.where(gene_feature != 0)]
+
+    # Initialize a tensor for gene indices
+    gene_init = torch.zeros((peak_feature.shape[0], len(gene_row)), dtype=torch.int32).to(device)
+    for peak_id in range(peak_feature.shape[0]):
+        gene_init[peak_id] = gene_row + peak_id * gene_feature.shape[0]
+
+    # Update the combined gene data tensors
+    gene_combine_row = gene_init.reshape(1, -1)[0]
+    gene_combine_col = gene_col.repeat(1, peak_feature.shape[0])[0]
+    gene_combine_data = gene_data.repeat(peak_feature.shape[0])
+
+    # Create the final sparse gene_feature tensor
+    gene_feature_ori = torch.sparse.FloatTensor(torch.vstack((gene_combine_row, gene_combine_col)), gene_combine_data, torch.Size((gene_feature.shape[0] * peak_feature.shape[0], gene_feature.shape[1])))
+    return gene_feature_ori.to(device)
+
+
+def gene_Peak_Score(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names):
+    y = ad.AnnData(RNA_matrix.transpose(), dtype='int32')
+    y.var_names=gene_names[0]
+    y.obs['pred'] = np.array(pred_label,dtype='int64')
+    y.obs['pred'] = y.obs['pred'].astype("category")
+    # Store the prediction results as a sparse matrix, where rows represent cells and columns represent cluster labels. A value of 1 at the corresponding position indicates that the cell belongs to that cluster.
+    cell_emb_binary = sp.coo_matrix((np.ones(len(y.obs['pred'])),(np.array(range(len(y.obs['pred']))),list(y.obs['pred']))))
+    cell_emb_binary.todense()
+
+    adata_atac_all = ATAC_matrix[:,nodes_id]
+    adata_rna_all = RNA_matrix[:,nodes_id]
+
+    ATAC_matrix_ct = adata_atac_all*(cell_emb_binary)
+    RNA_matrix_ct = adata_rna_all*(cell_emb_binary)
+    RNA_matrix_ct = RNA_matrix_ct/np.sum(cell_emb_binary,axis=0)
+    ATAC_matrix_ct = ATAC_matrix_ct/np.sum(cell_emb_binary,axis=0)
+
+    rna_matrix = RNA_matrix_ct
+    m = range(rna_matrix.shape[0])
+    gene_peak = RP_matrix
+    gp = gene_peak.reshape(gene_peak.shape[1]*rna_matrix.shape[0],1).todense()
+    gene_emb_enh = ATAC_matrix_ct[list(range (ATAC_matrix_ct.shape[0]))*rna_matrix.shape[0]]
+    peak_emb_enh = RNA_matrix_ct[[v for v in m for i in range(ATAC_matrix_ct.shape[0])]]
+    egrn = np.multiply(gene_emb_enh, peak_emb_enh)
+    egrn = np.multiply(egrn,gp)
+    return egrn
+
+def egrn_calculate(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names,peak_names,threshold=0):
+    print('We are currently performing calculations for EGRN. Please bear with us as this process will take approximately around 10 minutes.')
+    egrn = gene_Peak_Score(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names)
+    label_num = len(Counter(pred_label))
+    print('class_num:',label_num)
+    gn = np.array(gene_names[0])[[v for v in range(RNA_matrix.shape[0]) for i in range(ATAC_matrix.shape[0])]]
+    pn = np.array(peak_names[0])[list(range (ATAC_matrix.shape[0]))*RNA_matrix.shape[0]]
+    egrn_df = pd.DataFrame(columns=['gene', 'peak', 'score', 'class'])
+    print('We are currently conducting filtering and categorization operations.')
+    for i in range(label_num):
+        data = np.array(np.squeeze(egrn[:,i]))[0]
+        gene_peak_score_Dict = {'gene': gn, 'peak': pn, 'score':data}
+        gene_peak_score_df = pd.DataFrame(data = gene_peak_score_Dict)
+        gene_peak_score = gene_peak_score_df[gene_peak_score_df['score'] >threshold]
+        gene_peak_score = gene_peak_score.drop_duplicates(['gene','peak'])
+        gene_peak_score = gene_peak_score.sort_values(by="score",ascending=False)
+        gene_peak_score['class'] = i
+        egrn_df = egrn_df.append(gene_peak_score)
     return egrn_df
```

### Comparing `MarsGT-0.1.3/MarsGT/marsgt_model.py` & `MarsGT-0.1.4/MarsGT/marsgt_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from conv import *
-from utils import *
-from egrn import *
+from .conv import *
+from .utils import *
+from .egrn import *
 
 
 class GNN_from_raw(nn.Module):
     def __init__(self, in_dim, n_hid, num_types, num_relations, n_heads, n_layers, dropout=0.2, conv_name='hgt',
                  prev_norm=True, last_norm=True):
         super(GNN_from_raw, self).__init__()
         self.gcs = nn.ModuleList()
@@ -72,15 +72,15 @@
     def forward(self, x):
         x = F.relu(self.fc1(x))
         return x
 
 
 class NodeDimensionReduction(nn.Module):
     def __init__(self, RNA_matrix, ATAC_matrix, indices, ini_p1, n_hid, n_heads,
-                 n_layers, labsm, lr, wd, device, num_types=3, num_relations=2):
+                 n_layers, labsm, lr, wd, device, num_types=3, num_relations=2, epochs=1):
         super(NodeDimensionReduction, self).__init__()
         self.RNA_matrix = RNA_matrix
         self.ATAC_matrix = ATAC_matrix
         self.indices = indices
         self.ini_p1 = ini_p1
         self.in_dim = [RNA_matrix.shape[0], RNA_matrix.shape[1], ATAC_matrix.shape[1]]
         self.n_hid = n_hid
@@ -88,14 +88,15 @@
         self.num_relations = num_relations
         self.n_heads = n_heads
         self.n_layers = n_layers
         self.labsm = labsm
         self.lr = lr
         self.wd = wd
         self.device = device
+        self.epochs = epochs
 
         self.LabSm = LabelSmoothing(self.labsm)
 
         self.gnn = GNN_from_raw(in_dim=self.in_dim,
                                 n_hid=self.n_hid,
                                 num_types=self.num_types,
                                 num_relations=self.num_relations,
@@ -103,17 +104,17 @@
                                 n_layers=self.n_layers,
                                 dropout=0.3).to(self.device)
 
         self.optimizer = torch.optim.AdamW(self.gnn.parameters(), lr=self.lr, weight_decay=self.wd)
         self.scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(self.optimizer, 'min', factor=0.5, patience=5,
                                                                     verbose=True)
 
-    def train_model(self, epochs, n_batch):
+    def train_model(self, n_batch):
         print('The training process for the NodeDimensionReduction model has started. Please wait.')
-        for epoch in tqdm(range(epochs)):
+        for epoch in tqdm(range(self.epochs)):
             for batch_id in np.arange(n_batch):
                 gene_index = self.indices[batch_id]['gene_index']
                 cell_index = self.indices[batch_id]['cell_index']
                 peak_index = self.indices[batch_id]['peak_index']
                 gene_feature = self.RNA_matrix[list(gene_index),]
                 cell_feature = self.RNA_matrix[:, list(cell_index)].T
                 peak_feature = self.ATAC_matrix[list(peak_index),]
```

### Comparing `MarsGT-0.1.3/MarsGT/utils.py` & `MarsGT-0.1.4/MarsGT/utils.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.3/MarsGT.egg-info/PKG-INFO` & `MarsGT-0.1.4/MarsGT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.3
+Version: 0.1.4
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ==3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: torch_sparse
 Provides-Extra: torch_scatter
```

### Comparing `MarsGT-0.1.3/PKG-INFO` & `MarsGT-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.3
+Version: 0.1.4
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ==3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: torch_sparse
 Provides-Extra: torch_scatter
```

### Comparing `MarsGT-0.1.3/README.md` & `MarsGT-0.1.4/README.md`

 * *Files identical despite different names*

