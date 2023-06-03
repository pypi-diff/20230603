# Comparing `tmp/PySupercell-0.0.2.tar.gz` & `tmp/PySupercell-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySupercell-0.0.2.tar", last modified: Sat Jun  3 11:43:53 2023, max compression
+gzip compressed data, was "PySupercell-0.0.3.tar", last modified: Sat Jun  3 14:08:26 2023, max compression
```

## Comparing `PySupercell-0.0.2.tar` & `PySupercell-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,49 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/
--rwxrw-r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 11:10:34.000000 PySupercell-0.0.2/LICENSE.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      294 2023-06-03 11:24:12.000000 PySupercell-0.0.2/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      474 2023-06-03 11:43:53.111161 PySupercell-0.0.2/PKG-INFO
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.107161 PySupercell-0.0.2/PySupercell.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      474 2023-06-03 11:43:52.000000 PySupercell-0.0.2/PySupercell.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      547 2023-06-03 11:43:53.000000 PySupercell-0.0.2/PySupercell.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-03 11:43:52.000000 PySupercell-0.0.2/PySupercell.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       33 2023-06-03 11:43:52.000000 PySupercell-0.0.2/PySupercell.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-03 11:43:52.000000 PySupercell-0.0.2/PySupercell.egg-info/top_level.txt
--rw-r--r--   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 10:06:26.000000 PySupercell-0.0.2/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.107161 PySupercell-0.0.2/bin/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9840 2023-06-03 10:18:05.000000 PySupercell-0.0.2/bin/pysc.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.107161 PySupercell-0.0.2/examples/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       53 2023-06-03 11:23:33.000000 PySupercell-0.0.2/examples/README
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      364 2023-06-03 11:32:21.000000 PySupercell-0.0.2/examples/example1/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      704 2023-06-03 11:32:28.000000 PySupercell-0.0.2/examples/example1/POSCAR_redefine
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-06-03 11:35:47.000000 PySupercell-0.0.2/examples/example1/README
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      948 2023-06-03 11:15:37.000000 PySupercell-0.0.2/examples/example3/POSCAR_redefine
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 11:37:17.000000 PySupercell-0.0.2/examples/example3/make_screw_diamond.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/pysupercell/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     8621 2023-06-03 10:12:44.000000 PySupercell-0.0.2/pysupercell/QE_ibrav_lib.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      293 2023-06-03 11:39:40.000000 PySupercell-0.0.2/pysupercell/__init__.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     4587 2023-06-03 10:16:44.000000 PySupercell-0.0.2/pysupercell/arguments.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)    44205 2023-06-03 11:30:54.000000 PySupercell-0.0.2/pysupercell/pysupercell.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-03 11:43:53.111161 PySupercell-0.0.2/setup.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3609 2023-06-03 11:43:48.000000 PySupercell-0.0.2/setup.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 11:43:53.111161 PySupercell-0.0.2/tests_basic/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 10:27:02.000000 PySupercell-0.0.2/tests_basic/README
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       72 2023-06-03 10:30:27.000000 PySupercell-0.0.2/tests_basic/test_1.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.642947 PySupercell-0.0.3/
+-rwxrw-r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 11:10:34.000000 PySupercell-0.0.3/LICENSE.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      294 2023-06-03 11:24:12.000000 PySupercell-0.0.3/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-03 14:08:26.642947 PySupercell-0.0.3/PKG-INFO
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.634947 PySupercell-0.0.3/PySupercell.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-03 14:08:26.000000 PySupercell-0.0.3/PySupercell.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      951 2023-06-03 14:08:26.000000 PySupercell-0.0.3/PySupercell.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-03 14:08:26.000000 PySupercell-0.0.3/PySupercell.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       33 2023-06-03 14:08:26.000000 PySupercell-0.0.3/PySupercell.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-03 14:08:26.000000 PySupercell-0.0.3/PySupercell.egg-info/top_level.txt
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 13:25:16.000000 PySupercell-0.0.3/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.634947 PySupercell-0.0.3/bin/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9714 2023-06-03 14:04:58.000000 PySupercell-0.0.3/bin/pysc.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.634947 PySupercell-0.0.3/examples/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-06-03 13:05:58.000000 PySupercell-0.0.3/examples/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.634947 PySupercell-0.0.3/examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      364 2023-06-03 11:32:21.000000 PySupercell-0.0.3/examples/example1/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      611 2023-06-03 12:57:50.000000 PySupercell-0.0.3/examples/example1/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.638947 PySupercell-0.0.3/examples/example1/reference/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      704 2023-06-03 11:32:28.000000 PySupercell-0.0.3/examples/example1/reference/POSCAR_redefine
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1312 2023-06-03 12:58:44.000000 PySupercell-0.0.3/examples/example1/reference/POSCAR_slab
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.638947 PySupercell-0.0.3/examples/example2/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      437 2023-06-03 13:07:30.000000 PySupercell-0.0.3/examples/example2/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 13:09:42.000000 PySupercell-0.0.3/examples/example2/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.638947 PySupercell-0.0.3/examples/example2/reference/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     9732 2023-06-03 13:09:46.000000 PySupercell-0.0.3/examples/example2/reference/POSCAR_sc
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     9738 2023-06-03 13:09:46.000000 PySupercell-0.0.3/examples/example2/reference/POSCAR_tube
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.638947 PySupercell-0.0.3/examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1695 2023-06-03 13:49:18.000000 PySupercell-0.0.3/examples/example3/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)    44136 2023-06-03 14:01:17.000000 PySupercell-0.0.3/examples/example3/POSCAR_redefine
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)    54957 2023-06-03 14:06:32.000000 PySupercell-0.0.3/examples/example3/POSCAR_screw
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      555 2023-06-03 14:04:16.000000 PySupercell-0.0.3/examples/example3/README
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 14:03:09.000000 PySupercell-0.0.3/examples/example3/make_screw_diamond.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.638947 PySupercell-0.0.3/examples/example4/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      534 2023-06-03 13:02:08.000000 PySupercell-0.0.3/examples/example4/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      124 2023-06-03 13:04:39.000000 PySupercell-0.0.3/examples/example4/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.638947 PySupercell-0.0.3/examples/example4/reference/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     2176 2023-06-03 13:02:46.000000 PySupercell-0.0.3/examples/example4/reference/POSCAR_bending
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     2168 2023-06-03 13:02:46.000000 PySupercell-0.0.3/examples/example4/reference/POSCAR_flat
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.642947 PySupercell-0.0.3/pysupercell/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     8621 2023-06-03 10:12:44.000000 PySupercell-0.0.3/pysupercell/QE_ibrav_lib.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      293 2023-06-03 14:07:35.000000 PySupercell-0.0.3/pysupercell/__init__.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     4589 2023-06-03 13:26:30.000000 PySupercell-0.0.3/pysupercell/arguments.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)    44615 2023-06-03 14:06:49.000000 PySupercell-0.0.3/pysupercell/pysupercell.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-03 14:08:26.642947 PySupercell-0.0.3/setup.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3621 2023-06-03 14:07:28.000000 PySupercell-0.0.3/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:08:26.642947 PySupercell-0.0.3/tests_basic/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 10:27:02.000000 PySupercell-0.0.3/tests_basic/README
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       72 2023-06-03 10:30:27.000000 PySupercell-0.0.3/tests_basic/test_1.py
```

### Comparing `PySupercell-0.0.2/LICENSE.txt` & `PySupercell-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.2/README.md` & `PySupercell-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.2/bin/pysc.py` & `PySupercell-0.0.3/bin/pysc.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,22 +68,21 @@
     print ('{0}'.format('-'*60))
     print ('{0:14s}'.format('Total dist : ')+'   {:8.4f}'.format(np.sum(diff)))
     print ('{0:14s}'.format('Max   dist : ')+'   {:8.4f}\n'.format(np.max(diff)))
     return diff
 
 
 task_list=[
-'latt_info',
+'crystal_info',
 'redefine',
 'slab',
 'tube',
 'strain',
 'bond',
 'rotate_z',
-'molar_mass',
 'kmesh',
 'reset_vacuum',
 'bending',
 'screw_dislocation',
 'None']
 
 
@@ -92,15 +91,15 @@
 input exmaple:
     {0}
     {0} --task=redefine --sc1=1,-1,0 --sc2=1,1,0 sc3=0,0,1
     {0} --task=slab --hkl=121
     {0} --task=tube --chiral_num=2,4
     {0} --task=bond --atom_index=0,1
     {0} --task=wien
-    {0} --task=latt_info
+    {0} --task=crystal_info
     {0} --task=cmp --poscar1=POSCAR --poscar2=CONTCAR
     {0} --task=strain --dirs=0,1 --strain=0.01
     {0} --task=kmesh
     {0} --task=bending --nn=8 --idir_per=1 --idir_bend=2
     {0} --task=shift --idir_shift=2 --shift=10
     {0} --task=screw_dislocation --burgers_vector=[0,0,1] --screw_idir=2 --display_structure=True
 '''.format(__file__.split('/')[-1])
@@ -110,130 +109,128 @@
 def main(task_list):
     parser, args = get_args(desc_str)
     print ('\nRunning the script: {0}\n'.format(__file__.lstrip('./')))
     if color_print: cprint (desc_str,'green')
     else: print (desc_str)
 
 
-    if args.source=='VASP' and args.task!='cmp':
+    if args.source=='VASP':
         struct = cryst_struct.load_poscar(args.poscar)
     elif args.source=='QE':
         struct = cryst_struct.load_pwscf_in(args.filpw)
     elif args.source=='cif':
         struct = cryst_struct.load_cif(args.filcif)
 
-   
-    if args.task: flpos='POSCAR_'+args.task
-    if args.task==None: pass
-    elif args.task=='latt_info': print_latt_param(struct.latt_param())
+    if args.task==None: 
+        pass
 
+    elif args.task=='crystal_info': 
+        struct.verbose_crystal_info()
 
     elif args.task=='redefine':
+        filpos = 'POSCAR_redefine'
         redef_struct = struct.redefine_lattice(args.sc1,args.sc2,args.sc3,args.cell_orientation)
-        redef_struct.write_poscar_head(filename=flpos)
-        redef_struct.write_poscar_atoms(filename=flpos,mode='a')
-
+        redef_struct.write_poscar_head(filename=filpos)
+        redef_struct.write_poscar_atoms(filename=filpos,mode='a')
 
     elif args.task=='reset_vacuum':
         redef_struct=copy.copy(struct)
         redef_struct._cell[2,2]=args.vacuum
         central_z = np.average(redef_struct._pos_cart[:,2])
         redef_struct._pos_cart[:,2] -= central_z + redef_struct._cell[2,2]/2
         redef_struct._pos=np.dot(redef_struct._pos_cart,np.linalg.inv(redef_struct._cell))
         redef_struct.shift_atoms_to_home()
         flpos='POSCAR_reset_vacuum'
         redef_struct.write_poscar_head(filename=flpos)
         redef_struct.write_poscar_atoms(filename=flpos,mode='a')
         
- 
     elif args.task=='rotate_z':
         a=struct.latt_param()['a']
         b=struct.latt_param()['b']
         gamma=struct.latt_param()['gamma']
         cell_1=[a*cos((args.angle)/180*np.pi),a*np.sin((args.angle)/180*np.pi),0]
         cell_2=[b*cos((gamma+args.angle)/180*np.pi),b*np.sin((gamma+args.angle)/180*np.pi),0]
         struct._cell=np.array([cell_1,cell_2,struct._cell[2]])
         struct._system='POSCAR_rotate_z'
         struct.write_poscar_head(filename=flpos)
         struct.write_poscar_atoms(filename=flpos,mode='add')
 
-
     elif args.task=='slab':
         hkl=args.hkl
         if len(hkl)>3:
             exit('we do not allow negative index!')
         h,k,l=list(map(int,hkl))
         struct_slab = struct.build_slab(h,k,l,args.thickness,args.vacuum,args.atom_shift)
         struct_slab._system='slab'
         struct_slab.write_poscar_head(filename=flpos)
         struct_slab.write_poscar_atoms(filename=flpos,mode='a')
 
-
     elif args.task=='tube':
         n,m=args.chiral_num
         struct_tube = struct.build_tube(n,m,negative_R=args.negative_R)
         fltube = "POSCAR_tube_{0}_{1}".format(n,m)
         struct_tube._system=system='{0}_{1}_nanotube'.format(n,m)
         struct_tube.write_poscar_head(filename=flpos)
         struct_tube.write_poscar_atoms(filename=flpos,mode='a')
 
-
     elif args.task=='bending':
         struct_bend = struct.build_bending_supercell(args.nn,args.amp,args.idir_per,args.idir_bend,args.central_z)
         struct_bend._system = 'bending struct'
         struct_bend.write_poscar_head(filename=flpos)
         struct_bend.write_poscar_atoms(filename=flpos,mode='a')
 
-
     elif args.task=='strain':
         for idir in args.strain_dirs:
             struct._cell[idir] *= 1+args.strain
         struct._pos_cart=np.dot(struct._pos,struct._cell)
         filpos='POSCAR_{0:5.3f}'.format(args.strain)
         struct.write_poscar_head(filename=filpos)
         struct.write_poscar_atoms(filename=filpos)
 
-
     elif args.task=='shift':        
         struct.shift_pos(args.idir_shift,args.shift,to_home=False)
         filpos='POSCAR_shifted'
         struct.write_poscar_head(filename=filpos)
         struct.write_poscar_atoms(filename=filpos)
 
-
     elif args.task=='bond':
         i,j=args.atom_index
         cc=np.append(0,np.cumsum(struct._counts))
         ic=i-cc[np.where(i-cc>=0)[0][-1]]+1
         jc=j-cc[np.where(j-cc>=0)[0][-1]]+1
         print ('\n{0}\natomic positions in the home cell\n{0}'.format('-'*80))
         print ('symbol  atom '+('{:>10s} '*6).format('x','y','z','x_cart','y_cart','z_cart'))
         for ii,jj in zip((i,j),(ic,jc)):
-            print ('{0:>6s} {1:5d} '.format(struct._symbols[ii],jj),end='')
-            print (' '.join(['{0:10.5f}'.format(item) for item in np.append(struct._pos[ii],struct._pos_cart[ii])]))
+            print ('{:>6s} {:5d} '.format(struct._symbols[ii],jj),end='')
+            print (' '.join(['{:10.5f}'.format(item) for item in np.append(struct._pos[ii],struct._pos_cart[ii])]))
         print ( '-'*80)
-        output='min distance between {0}{1} and {2}{3} is: {4:8.5f} Angstrom'
-        print (output.format(struct._symbols[i],ic,struct._symbols[j],jc,struct._bond_length(i,j)))
+        output='min distance between {}{} and {}{} is: {:8.5f} Angstrom'
+        print (output.format(struct._symbols[i],ic,struct._symbols[j],jc,struct.bond_length(i,j)))
 
     elif args.task=='screw_dislocation':
         burgers_vector = np.dot(args.burgers_vector,struct._cell)
         struct_screw = struct.make_screw_dislocation(burgers_vector,args.screw_center,args.screw_normal,args.screw_idir)
+        struct_screw._system = 'screw dislocation structure'
+        struct_screw.write_poscar_head(filename='POSCAR_screw')
+        struct_screw.write_poscar_atoms(filename='POSCAR_screw',mode='a')
         if args.display_structure: map_data(struct_screw._cell,struct_screw._pos)
 
-    elif args.task=='density':
-        print ('density = {0:10.5f} g/cm^3 = {1:10.5f} Angs^3/atom'.format(struct.get_mass_density(),struct.get_volume_density()))
     elif args.task=='Select_Dynamics' or args.task=='SD':
         struct.write_poscar_head(filename='POSCAR_sd')
         struct.write_poscar_atoms(selective_dynamics=True,fix_dirs=args.dirs,filename='POSCAR_sd')
-    elif args.task=='wien':         struct.write_wien2k_struct(args.case,symmprec=args.symmprec)
-    elif args.task=='cmp':          cmp_struct(args.poscar1,args.poscar2)
-    elif args.task=='molar_mass':   struct._molar_mass()
-    elif args.task=='kmesh':        struct.writekp(args.kgrid)
-    else:
-        print ('\n{0}\navailable tasks:'.format('-'*30))
-        print ('\n'.join(['{0}'.format(task) for task in task_list])+'\n{0}'.format('-'*30))
 
-    if args.display_structure: map_data(struct._cell,struct._pos)
+    elif args.task=='wien':         
+        struct.write_wien2k_struct(args.case,symmprec=args.symmprec)
+
+    elif args.task=='cmp':        
+        cmp_struct(args.poscar1,args.poscar2)
+
+    elif args.task=='kmesh':
+        struct.writekp(args.kgrid)
+
+    else:
+        print ('\n{}\navailable tasks:'.format('-'*30))
+        print ('\n'.join([task for task in task_list])+'\n{0}'.format('-'*30))
 
 
 if __name__=='__main__':
     main(task_list)
```

### Comparing `PySupercell-0.0.2/examples/example1/POSCAR_redefine` & `PySupercell-0.0.3/examples/example1/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.2/examples/example3/make_screw_diamond.py` & `PySupercell-0.0.3/examples/example3/make_screw_diamond.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.2/pysupercell/QE_ibrav_lib.py` & `PySupercell-0.0.3/pysupercell/QE_ibrav_lib.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.2/pysupercell/arguments.py` & `PySupercell-0.0.3/pysupercell/arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,13 +60,13 @@
     parser.add_argument('--idir_per',type=int,default=0,help='latt vector index, for repeation')
     parser.add_argument('--idir_bend',type=int,default=2,help='latt vector index, for bending')
     parser.add_argument('--central_z',type=float,default=0.5,help='height for the central layer of the film (for bending) in frac coord')
 
     parser.add_argument('--screw_center',type=eval,default=[0.5,0.5,0.5],help='center of a screw dislocation in fractional coord.')
     parser.add_argument('--screw_normal',type=eval,default=[0.,1.,0.],help='normal vector of the glide plane for a screw dislocation.')
     parser.add_argument('--screw_idir',type=int,default=2,help='direction of screw dislocation: 0/1/2 for x/y/z')
-    parser.add_argument('--burger_vector',type=eval,default=[0,0,1],help='Burger vector in fractional coord.')
+    parser.add_argument('--burgers_vector',type=eval,default=[0,0,1],help='Burgers vector in fractional coord.')
     parser.add_argument('--display_structure',type=str2bool,default=False,help='display the structure with screw dislocation')
 
 
 if __name__=='__main__':
     print ('\nthis is a collection of arguments')
```

### Comparing `PySupercell-0.0.2/pysupercell/pysupercell.py` & `PySupercell-0.0.3/pysupercell/pysupercell.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,30 +78,14 @@
 def gen_Rvecs(ncell=1,boundary_condition=[1,1,1]):
     Rvecs = np.mgrid[-ncell:ncell+1,-ncell:ncell+1,-ncell:ncell+1].reshape(3,-1).T
     for i in range(3): 
         if boundary_condition[i]==0: Rvecs = Rvecs[Rvecs[:,i]==0]
     return Rvecs
  
 
-# get the arc length of amp*sin(2*pi*omega*x) between [0,x]
-# here x is in range (0,1/omega]
-def get_sin_arc_length_scipy(x,amp=1,omega=1):
-    from scipy.special import ellipe,ellipeinc
-    fac = (2*np.pi*amp*omega)**2
-    aa = np.sqrt(1+fac)/(2*np.pi*omega)
-    cc = fac/(1+fac)
-    E = aa*ellipeinc(2*np.pi*omega*x,cc)
-    return E
-
-
-def get_element_info_phonopy(symbol):
-    import phonopy.structure.atoms as atoms
-    return atoms.atom_data[atoms.symbol_map[symbol]]
-
-
 # still under development
 def parse_cif(fil):
     import re
     lines=np.array(open(fil).readlines())
 
     idx=np.where([re.search('_cell_length',line) for line in lines])
     a,b,c=[float(item.split()[1]) for item in lines[idx]]
@@ -306,14 +290,30 @@
     if grid_y!=0: 
         for iy in np.arange(1,grid_y): ax.axhline(iy*latt[1,1]/grid_y,ls='--',c='gray',alpha=0.6,zorder=-1)
     fig.tight_layout()
     if show: plt.show()
     return fig
 
 
+def get_element_info_phonopy(symbol):
+    import phonopy.structure.atoms as atoms
+    return atoms.atom_data[atoms.symbol_map[symbol]]
+
+
+# get the arc length of amp*sin(2*pi*omega*x) between [0,x]
+# here x is in range (0,1/omega]
+def get_sin_arc_length_scipy(x,amp=1,omega=1):
+    from scipy.special import ellipe,ellipeinc
+    fac = (2*np.pi*amp*omega)**2
+    aa = np.sqrt(1+fac)/(2*np.pi*omega)
+    cc = fac/(1+fac)
+    E = aa*ellipeinc(2*np.pi*omega*x,cc)
+    return E
+
+
 def find_normal_vector(u,v,n1,m1,eps=1e-4,max_int=100):
     # Assume u and v are two noncollinear vectors, A=n1*u+m1*v.
     # Find B=n2*u+m2*v which is perpendicular to A. 
     # Here n1,n2,m1,m2 are all integers.
     A = n1*u + m1*v
     LA = np.linalg.norm(A)
     for (nn,mm) in itertools.product(range(max_int+1),range(max_int+1)):
@@ -375,19 +375,18 @@
         alpha, beta, gamma = np.rad2deg([alpha,beta,gamma])
         return {'a':a,'b':b,'c':c,'alpha':alpha,'beta':beta,'gamma':gamma}
 
     def real_cell_volume(self): return abs(np.linalg.det(self._cell))
 
     def reciprocal_cell(self):  return 2*np.pi*np.linalg.inv(self._cell).T
 
-    def bond_length(self,i,j,cell_idx=False,ncell=1):
+    def bond_length(self,i,j,cell_idx=False,ncell=1,boundary_condition=[1,1,1]):
         Rvecs = gen_Rvecs(ncell,boundary_condition)
         dists = np.linalg.norm( np.dot(self._pos[j]-self._pos[i]+Rvecs, self._cell), axis=-1)
         bond = np.min(dists)
-        print (dists)
         if cell_idx: return bond,np.where(dists==bond)
         return bond
 
 
     # get distance from atom iat to other atoms in home and neighboring cellls
     # boundary condition 1 and 0 are periodic and open, respectively, for three lattice vectors
     def get_dists_one_atom(self,iat=0,boundary_condition=[1,1,1],ncell=1,verbosity=0):
@@ -565,33 +564,35 @@
                 label_dic.setdefault('M',[0.5, 0.5, 0.0])
                 label_dic.setdefault('Z',[0.0, 0.0, 0.5])
                 if ibrav==8:
                    label_dic.setdefault('Y',[0.0, 0.5, 0.0])
             else:
                 print ( ('sorry! we do not have the label lib for this symmetry now!'))
 
+
     def write_poscar_head(self,filename = 'POSCAR'):
         cell_fmt=('{:20.12f}'*3+'\n')*3
         with open(filename,'w') as fpos:
             fpos.write('{0}\n'.format(self._system))
             fpos.write('{0:10.7f}\n'.format(self._scale))
             fpos.write(cell_fmt.format(*tuple(self._cell.flatten())))
 
+
     def write_poscar_atoms(self,filename='POSCAR',postype='Direct',mode='a',selective_dynamics=False,fix_dirs=None):
         with open(filename,mode) as fpos:
             fpos.write(' '.join(['{0:3s}'.format(item) for item in self._species])+'\n')
             fpos.write(' '.join(['{0:3d}'.format(item) for item in self._counts])+'\n')
             if selective_dynamics: fpos.write('Selective_dynamics\n')
             fpos.write(postype+'\n')
             print_pos={'cartesian':self._pos_cart,'direct':self._pos}[postype.lower()]
             if selective_dynamics: 
                 dyn=[{True:'F',False:'T'}[i in fix_dirs] for i in range(3)]
-                print('\n'.join([' '.join(['{0:20.12f}'.format(item) for item in pos])+' '.join(['{0:>3s}'.format(L) for L in dyn]) for pos in print_pos]),file=fpos)
+                print('\n'.join([' '.join(['{0:25.18f}'.format(item) for item in pos])+' '.join(['{0:>3s}'.format(L) for L in dyn]) for pos in print_pos]),file=fpos)
             else:
-                print('\n'.join([('{:20.12f}'*3).format(*tuple(pos)) for pos in print_pos]),file=fpos)
+                print('\n'.join([('{:25.18f}'*3).format(*tuple(pos)) for pos in print_pos]),file=fpos)
 
     def write_pw_cell(self,ibrav,filename=None):
         celldm=self._find_celldm(ibrav)
         print ("ibrav=",ibrav, file=filename)
         #celldm=find_celldm(ibrav,latt)
         for i in range(1,7):
             if celldm[i]: print ('celldm({:1d}) = {:20.12f}'.format(i,celldm[i]), file=filename)
@@ -664,15 +665,15 @@
 
     def get_mass(self):
         amass=[get_element_info_phonopy(sym)[-1] for sym in self._symbols]
         return amass
 
     def get_mass_density(self):
         amass=self.get_mass()
-        return sum(mass)/(self.real_cell_volume()*1e-24*scipy.constants.Avogadro)
+        return sum(amass)/(self.real_cell_volume()*1e-24*scipy.constants.Avogadro)
 
     def get_volume_density(self):
         return self.real_cell_volume()/self._natom
 
 
     def visualize_struct(self):
         try: import matplotlib.pyplot as plt
@@ -709,17 +710,29 @@
         nfu=self._counts[0]
         for ispec in range(1,len(self._species)):
             nfu=gcd(self._counts[ispec],nfu)
         print ('no. of formula in unit cell: {0}'.format(nfu))
         try:
             amass=[get_element_info_phonopy(sym)[-1] for sym in self._species]
             molar_mass=sum(self._counts/nfu*amass)
-            print ('molar_mass={0:15.8f} g/mol = {1:15.8f} kg/mol'.format(molar_mass,molar_mass/1e3))
         except:
             exit('cannot calculate molar mass from phonopy')
+        return molar_mass
+
+
+    def verbose_crystal_info(self):
+        self.print_latt_param()
+        print ('Species  Natom')
+        for ispec,nat in zip(self._species,self._counts):
+            print ('{:7s}  {:5d}'.format(ispec,nat))
+        print ('\n')
+        print ('Molar_mass = {:15.8f} g/mol'.format(self.molar_mass()))
+        print ('Mass density   = {:10.5f}'.format(self.get_mass_density()))
+        print ('Volume density = {:10.5f} Atom/Angstrom^3'.format(self.get_volume_density()))
+
           
              
     def build_supercell(self,sc,eps=1e-4,nr=1,verbosity=0):
         sc_scale=np.linalg.det(sc)
         if verbosity:
             print ('Supercell scale = {:10.5f}'.format(sc_scale))
             if sc_scale==0:  warnings.warn('The supercell size is zero!','red')
```

### Comparing `PySupercell-0.0.2/setup.py` & `PySupercell-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,20 +67,20 @@
 
 core_modules = ['pysupercell/{}'.format(item) for item in core_modules]
 
 
 
 kwargs_setup=dict(
 name='PySupercell',
-version='0.0.2',
+version='0.0.3',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://to_be_posted',
 download_url='https://on_request',
-keywords=['Python','Crystal structure'],
+keywords=['Python','Crystal structure','supercell'],
 py_modules=core_modules,
 license="MIT License",
 description='Python library for creating and manipulating crystal structures',
 long_description="A Open-source Python library for playing with crystal structures, such as supercell, dislocation, slab, and nanotube",
 platforms=[platform.system()],
 install_requires=['numpy','matplotlib','scipy','termcolor'],
 )
```

