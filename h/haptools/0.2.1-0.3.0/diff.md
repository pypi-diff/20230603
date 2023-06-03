# Comparing `tmp/haptools-0.2.1.tar.gz` & `tmp/haptools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haptools-0.2.1.tar", max compression
+gzip compressed data, was "haptools-0.3.0.tar", max compression
```

## Comparing `haptools-0.2.1.tar` & `haptools-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-03-22 21:16:34.231399 haptools-0.2.1/LICENSE
--rw-r--r--   0        0        0     1443 2023-03-22 21:16:34.231399 haptools-0.2.1/README.md
--rw-r--r--   0        0        0      340 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/__init__.py
--rwxr-xr-x   0        0        0    22656 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/__main__.py
--rw-r--r--   0        0        0     2121 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/admix_storage.py
--rw-r--r--   0        0        0      265 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/data/__init__.py
--rw-r--r--   0        0        0    14450 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/data/breakpoints.py
--rw-r--r--   0        0        0      867 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/data/covariates.py
--rw-r--r--   0        0        0     2862 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/data/data.py
--rw-r--r--   0        0        0    51250 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/data/genotypes.py
--rw-r--r--   0        0        0    42541 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/data/haplotypes.py
--rw-r--r--   0        0        0    10403 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/data/phenotypes.py
--rw-r--r--   0        0        0     2911 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/index.py
--rw-r--r--   0        0        0    13845 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/karyogram.py
--rw-r--r--   0        0        0     8587 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/ld.py
--rw-r--r--   0        0        0      963 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/logging.py
--rw-r--r--   0        0        0    37181 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/sim_genotype.py
--rw-r--r--   0        0        0    12172 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/sim_phenotype.py
--rw-r--r--   0        0        0    27697 2023-03-22 21:16:34.235399 haptools-0.2.1/haptools/transform.py
--rw-r--r--   0        0        0     2243 2023-03-22 21:16:50.320751 haptools-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 haptools-0.2.1/setup.py
--rw-r--r--   0        0        0     2755 1970-01-01 00:00:00.000000 haptools-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-03 05:01:11.393974 haptools-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1443 2023-06-03 05:01:11.393974 haptools-0.3.0/README.md
+-rw-r--r--   0        0        0      340 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/__init__.py
+-rwxr-xr-x   0        0        0    26750 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/__main__.py
+-rw-r--r--   0        0        0     2121 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/admix_storage.py
+-rw-r--r--   0        0        0    20659 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/clump.py
+-rw-r--r--   0        0        0      286 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/data/__init__.py
+-rw-r--r--   0        0        0    14450 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/data/breakpoints.py
+-rw-r--r--   0        0        0      851 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/data/covariates.py
+-rw-r--r--   0        0        0     2862 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/data/data.py
+-rw-r--r--   0        0        0    59017 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/data/genotypes.py
+-rw-r--r--   0        0        0    48987 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/data/haplotypes.py
+-rw-r--r--   0        0        0    15519 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/data/phenotypes.py
+-rw-r--r--   0        0        0    62120 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/data/tr_harmonizer.py
+-rw-r--r--   0        0        0     2911 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/index.py
+-rw-r--r--   0        0        0    13845 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/karyogram.py
+-rw-r--r--   0        0        0     9001 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/ld.py
+-rw-r--r--   0        0        0     1056 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/logging.py
+-rw-r--r--   0        0        0    37434 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/sim_genotype.py
+-rw-r--r--   0        0        0    16539 2023-06-03 05:01:11.397974 haptools-0.3.0/haptools/sim_phenotype.py
+-rw-r--r--   0        0        0    27987 2023-06-03 05:01:11.401974 haptools-0.3.0/haptools/transform.py
+-rw-r--r--   0        0        0     2261 2023-06-03 05:01:27.178111 haptools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 haptools-0.3.0/setup.py
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 haptools-0.3.0/PKG-INFO
```

### Comparing `haptools-0.2.1/LICENSE` & `haptools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `haptools-0.2.1/README.md` & `haptools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `haptools-0.2.1/haptools/__main__.py` & `haptools-0.3.0/haptools/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import click
 
 # AVOID IMPORTING ANYTHING ABOVE
 # any imports we put here will make it slower to use the command line client
 # a basic "haptools --help" should be quick and require very few imports, for example
 
+
 ################### Haptools ##################
 @click.group()
 @click.version_option(message="%(version)s")
 def main():
     """
     haptools: A toolkit for simulating and analyzing genotypes and
     phenotypes while taking into account haplotype information
@@ -322,19 +323,26 @@
     "--replications",
     type=click.IntRange(min=1),
     default=1,
     show_default=True,
     help="Number of rounds of simulation to perform",
 )
 @click.option(
+    "--environment",
+    type=click.FloatRange(min=0),
+    default=None,
+    show_default=True,
+    help="Variance of environmental term; inferred if not specified",
+)
+@click.option(
     "-h",
     "--heritability",
     type=click.FloatRange(min=0, max=1),
     default=None,
-    show_default=True,
+    show_default="0.5",
     help="Trait heritability",
 )
 @click.option(
     "-p",
     "--prevalence",
     type=click.FloatRange(min=0, max=1, min_open=False, max_open=True),
     show_default="quantitative trait",
@@ -408,14 +416,23 @@
     "--chunk-size",
     type=int,
     default=None,
     show_default="all variants",
     help="If using a PGEN file, read genotypes in chunks of X variants; reduces memory",
 )
 @click.option(
+    "--repeats",
+    type=click.Path(exists=True, path_type=Path),
+    default=None,
+    help=(
+        "Path to a genotypes file containing tandem repeats. This is only necessary "
+        "when simulating both haplotypes *and* repeats as causal effects"
+    ),
+)
+@click.option(
     "--seed",
     type=int,
     default=None,
     show_default="chosen randomly",
     help="Use this option across executions to make the output reproducible",
 )
 @click.option(
@@ -434,23 +451,25 @@
     show_default=True,
     help="The level of verbosity desired",
 )
 def simphenotype(
     genotypes: Path,
     haplotypes: Path,
     replications: int = 1,
+    environment: float = None,
     heritability: float = None,
     prevalence: float = None,
     normalize: bool = True,
     region: str = None,
     samples: tuple[str] = tuple(),
     samples_file: Path = None,
     ids: tuple[str] = tuple(),
     ids_file: Path = None,
     chunk_size: int = None,
+    repeats: Path = None,
     seed: int = None,
     output: Path = Path("-"),
     verbosity: str = "INFO",
 ):
     """
     Haplotype-aware phenotype simulation. Create a set of simulated phenotypes from a
     set of haplotypes.
@@ -483,26 +502,33 @@
         with ids_file as id_file:
             ids = set(id_file.read().splitlines())
     elif ids:
         ids = set(ids)
     else:
         ids = None
 
+    if heritability is None and environment is None and not normalize:
+        # in this case, the assumptions of the model break
+        # The variances of both sides of the equation will no longer properly sum to 1
+        log.error("A --heritability value should be specified with --no-normalize")
+
     # Run simulation
     simulate_pt(
         genotypes,
         haplotypes,
         replications,
+        environment,
         heritability,
         prevalence,
         normalize,
         region,
         samples,
         ids,
         chunk_size,
+        repeats,
         seed,
         output,
         log,
     )
 
 
 @main.command(short_help="Transform a genotypes matrix via a set of haplotypes")
@@ -855,15 +881,15 @@
     type=click.Choice(["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"]),
     default="INFO",
     show_default=True,
     help="The level of verbosity desired",
 )
 def index(
     haplotypes: Path,
-    sort: bool = False,
+    sort: bool = True,
     output: Path = None,
     verbosity: str = "INFO",
 ):
     """
     Takes in an unsorted .hap file and outputs it as a .gz and a .tbi file
     """
 
@@ -871,10 +897,134 @@
     from .logging import getLogger
 
     log = getLogger(name="index", level=verbosity)
 
     index_haps(haplotypes, sort, output, log)
 
 
+@main.command(short_help="Clump summary stat files.")
+@click.option(
+    "--summstats-snps",
+    type=click.Path(path_type=Path),
+    help="File to load snps summary statistics",
+)
+@click.option(
+    "--summstats-strs",
+    type=click.Path(path_type=Path),
+    help="File to load strs summary statistics",
+)
+@click.option(
+    "--gts-snps", type=click.Path(path_type=Path), help="SNP genotypes (VCF or PGEN)"
+)
+@click.option("--gts-strs", type=click.Path(path_type=Path), help="STR genotypes (VCF)")
+@click.option(
+    "--clump-p1", type=float, default=0.0001, help="Max pval to start a new clump"
+)
+@click.option(
+    "--clump-p2", type=float, default=0.01, help="Filter for pvalue less than"
+)
+@click.option(
+    "--clump-id-field", type=str, default="SNP", help="Column header of the variant ID"
+)
+@click.option(
+    "--clump-field", type=str, default="P", help="Column header of the p-values"
+)
+@click.option(
+    "--clump-chrom-field",
+    type=str,
+    default="CHR",
+    help="Column header of the chromosome",
+)
+@click.option(
+    "--clump-pos-field", type=str, default="POS", help="Column header of the position"
+)
+@click.option(
+    "--clump-kb",
+    type=float,
+    default=250,
+    help="clump kb radius",
+)
+@click.option(
+    "--clump-r2",
+    type=float,
+    default=0.5,
+    help="r^2 threshold",
+)
+@click.option(
+    "--ld",
+    type=click.Choice(["Exact", "Pearson"]),
+    default="Pearson",
+    show_default=True,
+    help=(
+        "Calculation type to infer LD, Exact Solution or "
+        "Pearson R. (Exact|Pearson). Note the Exact Solution "
+        "works best when all three genotypes are present (0,1,2) in "
+        "the variants being compared."
+    ),
+)
+@click.option(
+    "--out",
+    type=click.Path(path_type=Path),
+    required=True,
+    help="Output filename",
+)
+@click.option(
+    "-v",
+    "--verbosity",
+    type=click.Choice(["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"]),
+    default="INFO",
+    show_default=True,
+    help="The level of verbosity desired",
+)
+def clump(
+    summstats_snps: Path,
+    summstats_strs: Path,
+    gts_snps: Path,
+    gts_strs: Path,
+    clump_p1: float,
+    clump_p2: float,
+    clump_id_field: str,
+    clump_field: str,
+    clump_chrom_field: str,
+    clump_pos_field: str,
+    clump_kb: float,
+    clump_r2: float,
+    ld: str,
+    out: Path,
+    verbosity: str = "INFO",
+):
+    """
+    Performs clumping on datasets with SNPs, SNPs and STRs, and STRs.
+    Clumping is the process of identifying SNPs or STRs that are highly
+    correlated with one another and concatenating them all together into
+    a single "clump" in order to not repeat the same effect size due to
+    LD.
+    """
+    from .logging import getLogger
+    from .clump import clumpstr
+
+    log = getLogger(name="clump", level=verbosity)
+    log.debug(f"Loading SNPs from {summstats_snps} {gts_snps}")
+    log.debug(f"Loading STRs from {summstats_strs} {gts_strs}")
+
+    clumpstr(
+        summstats_snps,
+        summstats_strs,
+        gts_snps,
+        gts_strs,
+        clump_p1,
+        clump_p2,
+        clump_id_field,
+        clump_field,
+        clump_chrom_field,
+        clump_pos_field,
+        clump_kb,
+        clump_r2,
+        ld,
+        out,
+        log,
+    )
+
+
 if __name__ == "__main__":
     # run the CLI if someone tries 'python -m haptools' on the command line
     main(prog_name="haptools")
```

### Comparing `haptools-0.2.1/haptools/admix_storage.py` & `haptools-0.3.0/haptools/admix_storage.py`

 * *Files identical despite different names*

### Comparing `haptools-0.2.1/haptools/data/breakpoints.py` & `haptools-0.3.0/haptools/data/breakpoints.py`

 * *Files identical despite different names*

### Comparing `haptools-0.2.1/haptools/data/covariates.py` & `haptools-0.3.0/haptools/data/covariates.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 
     Examples
     --------
     >>> covariates = Covariates.load('tests/data/simple.covar')
     """
 
     def __init__(self, fname: Path | str, log: Logger = None):
-        super(Phenotypes, self).__init__(fname, log)
+        super().__init__(fname, log)
         self._ext = "covar"
```

### Comparing `haptools-0.2.1/haptools/data/data.py` & `haptools-0.3.0/haptools/data/data.py`

 * *Files identical despite different names*

### Comparing `haptools-0.2.1/haptools/data/genotypes.py` & `haptools-0.3.0/haptools/data/genotypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from collections import namedtuple, Counter
 
 import numpy as np
 import numpy.typing as npt
 from cyvcf2 import VCF, Variant
 from pysam import VariantFile, TabixFile
 
+try:
+    import trtools.utils.tr_harmonizer as trh
+except ModuleNotFoundError:
+    from . import tr_harmonizer as trh
+
 from .data import Data
 
 
 class Genotypes(Data):
     """
     A class for processing genotypes from a file
 
@@ -192,15 +197,15 @@
                 self.data = self.data[:num_seen]
         if 0 in self.data.shape:
             self.log.warning(
                 "Failed to load genotypes. If you specified a region, check that the"
                 " contig name matches! For example, double-check the 'chr' prefix."
             )
         # transpose the GT matrix so that samples are rows and variants are columns
-        self.log.info(f"Transposing genotype matrix of size {self.data.shape}.")
+        self.log.info(f"Transposing genotype matrix of size {self.data.shape}")
         self.data = self.data.transpose((1, 0, 2))
 
     def _variant_arr(self, record: Variant):
         """
         Construct a np array from the metadata in a line of the VCF
 
         This is a helper function for :py:meth:`~.Genotypes._iterate`. It's separate
@@ -217,14 +222,48 @@
             A row from the :py:attr:`~.Genotypes.variants` array
         """
         return np.array(
             (record.ID, record.CHROM, record.POS),
             dtype=self.variants.dtype,
         )
 
+    def _vcf_iter(self, vcf: cyvcf2.VCF, region: str):
+        """
+        Yield all variants within a region in the VCF file.
+
+        Parameters
+        ----------
+        vcf: VCF
+            The cyvcf2.VCF object from which to fetch variant records
+        region : str, optional
+            See documentation for :py:meth:`~.Genotypes.read`
+
+        Returns
+        -------
+        vcffile : cyvcf2.VCF
+            Iterable cyvcf2 instance.
+        """
+        return vcf(region)
+
+    def _return_data(self, variant: Variant):
+        """
+        Collect genotypes from current variant
+
+        Parameters
+        ----------
+        variant: cyvcf2.Variant
+            A cyvcf2.Variant object from which to fetch genotypes
+
+        Returns
+        -------
+        data: npt.NDArray[np.uint8]
+            Numpy array storing all genotypes
+        """
+        return np.array(variant.genotypes, dtype=np.uint8)
+
     def _iterate(self, vcf: VCF, region: str = None, variants: set[str] = None):
         """
         A generator over the lines of a VCF
 
         This is a helper function for :py:meth:`~.Genotypes.__iter__`
 
         Parameters
@@ -243,28 +282,28 @@
             namedtuple containing each of the class properties
         """
         self.log.info(f"Loading genotypes from {len(self.samples)} samples")
         Record = namedtuple("Record", "data variants")
         num_seen = 0
         # iterate over each line in the VCF
         # note, this can take a lot of time if there are many samples
-        for variant in vcf(region):
+        for variant in self._vcf_iter(vcf, region):
             if variants is not None and variant.ID not in variants:
                 if num_seen >= len(variants):
                     # exit early if we've already found all the variants
                     break
                 continue
             # save meta information about each variant
             variant_arr = self._variant_arr(variant)
             # extract the genotypes to a matrix of size n x 3
             # the last dimension has three items:
             # 1) presence of REF in strand one
             # 2) presence of REF in strand two
             # 3) whether the genotype is phased (if self._prephased is False)
-            data = np.array(variant.genotypes, dtype=np.uint8)
+            data = self._return_data(variant)
             data = data[:, : (2 + (not self._prephased))]
             yield Record(data, variant_arr)
             num_seen += 1
         vcf.close()
 
     def __iter__(
         self, region: str = None, samples: list[str] = None, variants: set[str] = None
@@ -402,16 +441,17 @@
         Parameters
         ----------
         discard_also : bool, optional
             If True, discard any samples that are missing genotypes without raising a
             ValueError
         """
         # check: are there any samples that have genotype values that are empty?
-        # A genotype value equal to the max for uint8 indicates the value was missing
-        missing = np.any(self.data[:, :, :2] == np.iinfo(np.uint8).max, axis=2)
+        # A genotype value equal to the max or one less than max for uint8 indicates
+        #   the value was missing
+        missing = np.any(self.data[:, :, :2] >= np.iinfo(np.uint8).max - 1, axis=2)
         if np.any(missing):
             samp_idx, variant_idx = np.nonzero(missing)
             if discard_also:
                 original_num_samples = len(self.samples)
                 self.data = np.delete(self.data, samp_idx, axis=0)
                 self.samples = tuple(np.delete(self.samples, samp_idx))
                 self.log.warning(
@@ -589,24 +629,85 @@
         for chrom in chroms:
             positions = self.variants["pos"][self.variants["chrom"] == chrom]
             if not np.all(positions[:-1] <= positions[1:]):
                 raise ValueError(
                     f"The variants in chromosome '{chrom}' are not sorted by position"
                 )
 
+    @classmethod
+    def merge_variants(
+        cls, objs: tuple[Genotypes], check_samples: bool = True, **kwargs
+    ) -> Genotypes:
+        """
+        Merge genotypes objects with different sets of variants together
+
+        .. note::
+            The input genotypes objects are not expected to have any overlapping sets
+            of variants. Also, all samples in the input genotypes must be the same.
+
+        Parameters
+        ----------
+        objs: tuple[Genotypes]
+            The objects that should be merged together
+        check_samples: bool, optional
+            Whether to check that the set of provided samples is *exactly* the same
+            for all genotypes. This can take a while so you may want to avoid it
+        **kwargs
+            Any parameters to pass to :py:meth:`~.Genotypes._init__`
+
+        Raises
+        ------
+        ValueError
+            If the set of samples in each input object is not the same
+
+        Returns
+        -------
+        Genotypes
+            A new object containing merged versions of the properties in each object
+        """
+        gts = cls(**kwargs)
+        if check_samples:
+            for obj in objs[1:]:
+                if objs[0].samples != obj.samples:
+                    raise ValueError("Samples must be shared among all Genotypes")
+        else:
+            num_samps = [len(obj.samples) for obj in objs]
+            if all(num_samps[0] == num_samps[1:]):
+                gts.samples = tuple(samp for obj in objs for samp in obj.samples)
+            else:
+                raise ValueError("Samples must be shared among all Genotypes")
+        gts.samples = objs[0].samples
+        dtypes = list(gts.variants.dtype.names)
+        gts.variants = np.concatenate(tuple(obj.variants[dtypes] for obj in objs))
+        unphased = [obj.data.shape[2] == 3 for obj in objs]
+        # check: do we have a mix of phased and unphased objects?
+        if any(unphased) and not all(unphased):
+            data = (
+                obj.data if phase else np.insert(obj.data, 2, 1, axis=2)
+                for phase, obj in zip(unphased, objs)
+            )
+        else:
+            data = (obj.data for obj in objs)
+        # TODO: fix Genotypes.check_biallelic so it always keeps data as np.uint8 and then adjust this code accordingly
+        dtype = (
+            np.bool_ if all(obj.data.dtype == np.bool_ for obj in objs) else np.uint8
+        )
+        gts.data = np.concatenate(tuple(data), axis=1, dtype=dtype)
+        return gts
+
 
 class GenotypesVCF(Genotypes):
     """
     A class for processing genotypes from a file
     Unlike the base Genotypes class, this class also includes REF and ALT alleles as
     a list of alleles in the variants array
 
     Attributes
     ----------
-    data : np.array
+    data : npt.NDArray
         See documentation for :py:attr:`~.Genotypes.data`
     fname : Path | str
         See documentation for :py:attr:`~.Genotypes.fname`
     samples : tuple[str]
         See documentation for :py:attr:`~.Genotypes.samples`
     variants : np.array
         Variant-level meta information:
@@ -691,21 +792,155 @@
                 else:
                     record.samples[sample].phased = self.data[samp_idx, var_idx, 2]
             # write the record to a file
             vcf.write(record)
         vcf.close()
 
 
+class GenotypesTR(Genotypes):
+    """
+    A class for processing TR genotypes from a file
+    Unlike the base Genotypes class, this class genotypes will be repeat number
+    in the variants array
+
+    Attributes
+    ----------
+    data : npt.NDArray
+        See documentation for :py:attr:`~.Genotypes.data`
+    fname : Path | str
+        See documentation for :py:attr:`~.Genotypes.fname`
+    samples : tuple[str]
+        See documentation for :py:attr:`~.Genotypes.samples`
+    variants : np.array
+        Variant-level meta information:
+            1. ID
+            2. CHROM
+            3. POS
+    log: Logger
+        See documentation for :py:attr:`~.Genotypes.log`
+    vcftype: str
+        TR vcf type currently being read.
+        {'auto', 'gangstr', 'advntr', 'hipstr', 'eh', 'popstr'}
+    """
+
+    def __init__(self, fname: Path | str, log: Logger = None, vcftype: str = "auto"):
+        super().__init__(fname, log)
+        self.vcftype = vcftype
+
+    @classmethod
+    def load(
+        cls: GenotypesTR,
+        fname: Path | str,
+        region: str = None,
+        samples: list[str] = None,
+        variants: set[str] = None,
+        vcftype: str = "auto",
+    ) -> Genotypes:
+        """
+        Load STR genotypes from a VCF file
+
+        Read the file contents, check the genotype phase, and create the MAC matrix
+
+        Parameters
+        ----------
+        fname
+            See documentation for :py:attr:`~.Data.fname`
+        region : str, optional
+            See documentation for :py:meth:`~.Genotypes.read`
+        samples : list[str], optional
+            See documentation for :py:meth:`~.Genotypes.read`
+        variants : set[str], optional
+            See documentation for :py:meth:`~.Genotypes.read`
+
+        Returns
+        -------
+        Genotypes
+            A Genotypes object with the data loaded into its properties
+        """
+        genotypes = cls(fname, vcftype=vcftype)
+        genotypes.read(region, samples, variants)
+        genotypes.check_phase()
+        return genotypes
+
+    def _vcf_iter(self, vcf: cyvcf2.VCF, region: str = None):
+        """
+        Collect GTs (trh.TRRecord objects) to iterate over
+
+        Parameters
+        ----------
+        vcf: VCF
+            The cyvcf2.VCF object from which to fetch variant records
+        region : str, optional
+            See documentation for :py:meth:`~.Genotypes.read`
+
+        Returns
+        -------
+        tr_records: trh.TRRecord
+            TRRecord objects yielded from TRRecordHarmonizer
+        """
+        for record in trh.TRRecordHarmonizer(
+            vcffile=vcf, vcfiter=vcf(region), region=region, vcftype=self.vcftype
+        ):
+            record.ID = record.record_id
+            record.CHROM = record.chrom
+            record.POS = record.pos
+            yield record
+
+    def _return_data(self, variant: trh.TRRecord):
+        """
+        Collect Genotypes, transform them to copy number, and return them.
+
+        Parameters
+        ----------
+        variant: trh.TRRecord
+            A trh.TRRecord object from which to collect copy number genotypes using the
+            GetLengthGenotypes() function
+
+        Returns
+        -------
+        data: npt.NDArray[np.uint8]
+            Numpy array storing all genotypes
+        """
+        # Grab GT Lengths and round to lowest integer
+        gts = np.rint(variant.GetLengthGenotypes())
+
+        # If only one GT present fill rest with empty gts (-1)
+        if gts.shape[1] == 2:
+            self.log.warning(
+                "The current variant in the VCF only has one allele per sample."
+            )
+            data = []
+            # Only one GT so phase will always be 0
+            zeros = np.zeros((gts.shape[0], 1))
+            missing = -1 * np.ones((gts.shape[0],))
+            gts = np.concatenate((gts, zeros), axis=1)
+            gts[:, 1] = missing
+
+        return gts.astype(np.uint8)
+
+    def check_biallelic(self):
+        """
+        See documentation for :py:meth:`~.Genotypes.check_biallelic`
+        """
+        raise NotImplementedError
+
+    def check_maf(self):
+        """
+        See documentation for :py:meth:`~.Genotypes.check_maf`
+        """
+        raise NotImplementedError
+
+
 class GenotypesPLINK(GenotypesVCF):
     """
     A class for processing genotypes from a PLINK ``.pgen`` file
 
     Attributes
     ----------
-    data : np.array
+    data : npt.NDArray
         See documentation for :py:attr:`~.GenotypesVCF.data`
     samples : tuple
         See documentation for :py:attr:`~.GenotypesVCF.data`
     variants : np.array
         See documentation for :py:attr:`~.GenotypesVCF.data`
     log: Logger
         See documentation for :py:attr:`~.GenotypesVCF.data`
@@ -1061,26 +1296,26 @@
                     )
                     # missing alleles will have a value of -9
                     # let's make them be -1 to be consistent with cyvcf2
                     data[data == -9] = -1
                     # add phase info, then transpose the GT matrix so that samples are
                     # rows and variants are columns
                     self.data[:, start:end, :2] = data.reshape(
-                        (chunks, mat_shape[0], 2)
+                        (size, mat_shape[0], 2)
                     ).transpose((1, 0, 2))
                     self.data[:, start:end, 2] = phasing.transpose()
                 else:
                     # ...each row is a different chromosomal strand
                     data = np.empty((size, len(sample_idxs) * 2), dtype=np.int32)
                     pgen.read_alleles_list(indices[start:end], data)
                     # missing alleles will have a value of -9
                     # let's make them be -1 to be consistent with cyvcf2
                     data[data == -9] = -1
                     self.data[:, start:end] = data.reshape(
-                        (chunks, mat_shape[0], 2)
+                        (size, mat_shape[0], 2)
                     ).transpose((1, 0, 2))
                 del data
                 gc.collect()
 
     def _iterate(
         self,
         pgen: pgenlib.PgenReader,
@@ -1216,15 +1451,15 @@
         :py:attr:`~.GenotypesPLINK.fname`
         """
         import pgenlib
 
         # write the psam and pvar files
         self.write_samples()
         self.write_variants()
-        self.log.debug(f"Transposing genotype matrix of size {self.data.shape}.")
+        self.log.debug(f"Transposing genotype matrix of size {self.data.shape}")
         # transpose the data b/c pgenwriter expects things in "variant-major" order
         # (ie where variants are rows instead of samples)
         data = self.data.transpose((1, 0, 2))[:, :, :2]
         # how many variants should we write at once?
         chunks = self.chunk_size
         if chunks is None or chunks > len(self.variants):
             chunks = len(self.variants)
```

### Comparing `haptools-0.2.1/haptools/data/haplotypes.py` & `haptools-0.3.0/haptools/data/haplotypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
-import os
 from pathlib import Path
 from functools import total_ordering
 from logging import getLogger, Logger
 from dataclasses import dataclass, field, fields
 from typing import Iterator, get_type_hints, Generator, Callable
 
 import numpy as np
 import numpy.typing as npt
 from pysam import TabixFile
 
 from .data import Data
 from .genotypes import GenotypesVCF
 
 
+# the current version of the hap format spec
+HAP_VERSION = "0.2.0"
+
+
 @dataclass
 class Extra:
     """
     An extra field on a line in the .hap file
 
     Attributes
     ----------
@@ -493,15 +496,15 @@
                     [int(var.allele != gts.variants[i]["alleles"][0])]
                     for i, var in enumerate(self.variants)
                 ]
             ]
         )
         # look for the presence of each allele in each chromosomal strand
         # and then just AND them together
-        return np.all(allele_arr == gts.data, axis=1)
+        return np.all(allele_arr == gts.data[:, :, :2], axis=1)
 
     def __lt__(self, other: Haplotype):
         """
         Defines ordering for sort() method when dealing with variants.
 
         This function will sort first by start followed by end and lastly ID
 
@@ -532,28 +535,205 @@
         Sorts the variants within this Haplotype instance
 
         """
 
         self.variants = tuple(sorted(self.variants))
 
 
+@total_ordering
+@dataclass
+class Repeat:
+    """
+    A tandem repeat within the .hap format spec
+
+    In order to use this class with the Haplotypes class, you should
+    1) add properties to the class for each of extra fields
+    2) override the _extras property to describe the header declaration
+
+    Attributes
+    ----------
+    chrom: str
+        The contig to which this tandem repeat belongs
+    start: int
+        The chromosomal start position of the tandem repeat
+    end: int
+        The chromosomal end position of the tandem repeat
+    id: str
+        The tandem repeat's unique ID
+    _extras: tuple[Extra]
+        Extra fields for the tandem repeat
+
+    Examples
+    --------
+    Let's extend this class and add an extra field called "ancestry"
+
+    >>> from dataclasses import dataclass, field
+    >>> @dataclass
+    >>> class CustomRepeat(Repeat):
+    ...     ancestry: str
+    ...     _extras: tuple = field(
+    ...         repr=False,
+    ...         init=False,
+    ...         default = (
+    ...             Extra("ancestry", "s", "Local ancestry"),
+    ...         ),
+    ...     )
+    """
+
+    chrom: str
+    start: int
+    end: int
+    id: str
+    _extras: tuple = field(default=tuple(), init=False, repr=False)
+
+    @property
+    def ID(self):
+        """
+        Create an alias for the id property
+        """
+        return self.id
+
+    @property
+    # TODO: use @cached_property in py3.8
+    def _fmt(self):
+        extras = ""
+        if len(self._extras):
+            extras = "\t" + "\t".join(extra.fmt_str for extra in self._extras)
+        return "R\t{chrom:s}\t{start:d}\t{end:d}\t{id:s}" + extras
+
+    @classproperty
+    # TODO: use @cached_property in py3.8
+    def types(cls) -> dict[str, type]:
+        """
+        Obtain the types of each property in the object
+
+        Returns
+        -------
+        dict[str, type]
+            A mapping of each property in the object to its type
+        """
+        return {k: v for k, v in get_type_hints(cls).items() if not k.startswith("_")}
+
+    @classmethod
+    def from_hap_spec(
+        cls: Repeat,
+        line: str,
+        types: dict[str, type] = None,
+    ) -> Repeat:
+        """
+        Convert a tandem repeat line into a tandem repeat object in the .hap format spec
+
+        Note that this implementation does NOT support having more extra fields than
+        appear in the header
+
+        Parameters
+        ----------
+        line: str
+            A tandem repeat (R) line from the .hap file
+        types: dict[str, type], optional
+            The types of each property in the object
+
+        Returns
+        -------
+        Repeat
+            The repeat object line.
+        """
+        assert line[0] == "R", "Attempting to init a Repeat with a non-R line"
+        line = line[2:].split("\t")
+        types = types or cls.types
+        tr_fields = {
+            name: val(line[idx])
+            for idx, (name, val) in enumerate(types.items())
+            if val is not None
+        }
+        return cls(**tr_fields)
+
+    def to_hap_spec(self) -> str:
+        """
+        Convert a Repeat object into a repeat line in the .hap format spec
+
+        Returns
+        -------
+        str
+            A valid Repeat line (R) in the .hap format spec
+        """
+        return self._fmt.format(**self.__dict__)
+
+    @classmethod
+    def extras_head(cls) -> set:
+        """
+        Return the header lines of the extra fields that are supported
+
+        Returns
+        -------
+        tuple
+            The header lines of the extra fields
+        """
+        return set(extra.to_hap_spec("R") for extra in cls._extras)
+
+    @classmethod
+    def extras_order(cls) -> tuple[str]:
+        """
+        The names of the extra fields in order
+
+        Returns
+        -------
+        tuple[str]
+            The names of the extra fields in the order in which they are stored
+        """
+        return tuple(extra.name for extra in cls._extras)
+
+    def __lt__(self, other: Haplotype | Repeat):
+        """
+        Defines ordering for sort() method when dealing with variants.
+
+        This function will sort first by start followed by end and lastly ID
+
+        Parameters
+        ----------
+        other: Haplotype|Repeat
+            A haplotype or repeat line from the .hap file
+
+        Returns
+        -------
+        bool
+            True if other is less than this instance, and False otherwise
+        """
+
+        if self.chrom == other.chrom:
+            if self.start == other.start:
+                if self.end == other.end:
+                    return self.id < other.id
+                else:
+                    return self.end < other.end
+            else:
+                return self.start < other.start
+        else:
+            return self.chrom < other.chrom
+
+
 class Haplotypes(Data):
     """
     A class for processing haplotypes from a file
 
     Attributes
     ----------
     fname: Path | str
         The path to the file containing the data
-    data: dict[str, Haplotype]
-        A dict of Haplotype objects keyed by their IDs
+    data: dict[str, Haplotype|Repeat]
+        A dict of Haplotype/Repeat objects keyed by their IDs
     types: dict
         A dict of class names keyed by the symbol denoting their line type
 
-        Ex: {'H': Haplotype, 'V': Variant}
+        Ex: {'H': Haplotype, 'V': Variant, 'R': Repeat}
+    type_ids: dict[str, list]
+        A dict of class names keyed by the symbol denoting line type.
+        Stores all haplotype and repeat IDs.
+
+        Ex: {'H': ["H1", "H2", "H3"], 'R': ["STR_1", "STR_2"]}
     version: str
         A string denoting the current file format version
     log: Logger
         A logging instance for recording debug statements.
 
     Examples
     --------
@@ -568,27 +748,30 @@
     Haplotypes object:
 
     >>> haplotypes = Haplotypes('tests/data/simphenotype.hap', HaptoolsHaplotype)
     >>> haplotypes.read()
     >>> haps = haplotypes.data # a dictionary of Haplotype objects
     """
 
+    version = HAP_VERSION
+
     def __init__(
         self,
         fname: Path | str,
         haplotype: type[Haplotype] = Haplotype,
         variant: type[Variant] = Variant,
+        repeat: type[Repeat] = Repeat,
         log: Logger = None,
     ):
         super().__init__(fname, log)
         self.data = None
         # note: it's important that self.types is created such that its keys are sorted
         # otherwise, the write() method might create unsorted files
-        self.types = {"H": haplotype, "V": variant}
-        self.version = "0.1.0"
+        self.types = {"H": haplotype, "V": variant, "R": repeat}
+        self.type_ids = None
 
     @classmethod
     def load(
         cls: Haplotypes,
         fname: Path | str,
         region: str = None,
         haplotypes: set[str] = None,
@@ -651,15 +834,15 @@
             self.log.warning("There have been fixes to the .hap spec")
         return o_major, o_minor, o_patch
 
     def check_header(
         self,
         lines: list[str],
         check_version=True,
-        softly=False,
+        softly=True,
     ) -> tuple[dict, dict[str, tuple[str]]]:
         """
         1) Check and parse any metadata and 2) check that any extra fields declared in
         the .haps file can be handled by the Variant and Haplotype classes
         provided in __init__()
 
         This function is called automatically by other methods that read .hap files
@@ -769,14 +952,30 @@
         line_types = self.types.keys()
         if line[0] in line_types:
             return line[0]
         else:
             # if none of the lines matched, return None
             return None
 
+    def index(self, force=False):
+        """
+        Reset the type_ids parameter
+
+        You should call this method after any changes to the data property
+        """
+        if not (force or self.type_ids is None):
+            # do not remap IDs if they've already been mapped
+            return
+        self.type_ids = {"H": [], "R": []}
+        for key, value in self.data.items():
+            if isinstance(value, Haplotype):
+                self.type_ids["H"].append(key)
+            if isinstance(value, Repeat):
+                self.type_ids["R"].append(key)
+
     def read(self, region: str = None, haplotypes: set[str] = None):
         """
         Read haplotypes from a .hap file into a list stored in :py:attr:`~.Haplotypes.data`
 
         Parameters
         ----------
         region: str, optional
@@ -791,24 +990,27 @@
 
             Defaults to loading haplotypes from all samples
         """
         super().read()
         self.data = {}
         var_haps = {}
         for line in self.__iter__(region, haplotypes):
-            if isinstance(line, Haplotype):
+            if isinstance(line, Haplotype) or isinstance(line, Repeat):
+                # store Haplotype object and Repeat object the same way
                 self.data[line.id] = line
             elif isinstance(line, Variant):
                 hap_id = line.hap
                 del line.hap
                 # store the variant for later
                 var_haps.setdefault(hap_id, []).append(line)
         for hap in var_haps:
             self.data[hap].variants = tuple(var_haps[hap])
-        self.log.info(f"Loaded {len(self.data)} haplotypes from .hap file")
+        self.index()
+        num_haps = len(self.type_ids["H"])
+        self.log.info(f"Loaded {num_haps} haplotypes from .hap file")
 
     def _get_field_types(
         self,
         extras: dict[str, tuple[str]],
         order: dict[str, tuple] = None,
     ) -> dict[str, dict[str.type]]:
         """
@@ -890,39 +1092,43 @@
                 region = []
             else:
                 region = region[1].split("-", maxsplit=1)
                 if len(region) > 1 and region[1] == "":
                     region = [region[0]]
                 region = list(map(int, region))
             # fetch region
-            # we already know that each line will start with an H, so we don't
-            # need to check that
             for line in haps_file.fetch(region=region_str, multiple_iterators=True):
-                hap = self.types["H"].from_hap_spec(line, types=line_types)
+                # hap can either be a Repeat or Haplotype
+                line_type = self._line_type(line)
+                hap = self.types[line_type].from_hap_spec(
+                    line, types=line_types[line_type]
+                )
                 if haplotypes is not None:
                     if hap.id not in haplotypes:
                         continue
                 # also exclude haplotypes that overlap but don't fit perfectly
                 if len(region) >= 2 and (hap.start < region[0] or hap.end > region[1]):
                     continue
                 elif len(region) == 1 and hap.start < region[0]:
                     continue
                 yield hap
         else:
+            count = 0
             for line in haps_file.fetch(multiple_iterators=True):
                 # we only want lines that start with an H
                 line_type = self._line_type(line)
-                if line_type == "H":
-                    hap = self.types["H"].from_hap_spec(line, types=line_types)
+                if line_type == "H" or line_type == "R":
+                    hap = self.types[line_type].from_hap_spec(
+                        line, types=line_types[line_type]
+                    )
                     if hap.id in haplotypes:
+                        count += 1
                         yield hap
-                elif line_type > "H":
-                    # if we've already passed all of the H's, we can just exit
-                    # We assume the file has been sorted so that all of the H lines
-                    # come before the V lines
+                # exit prematurely if we've seen all of the requested haplotypes
+                if count == len(haplotypes):
                     break
 
     def __iter__(
         self, region: str = None, haplotypes: set[str] = None
     ) -> Iterator[Variant | Haplotype]:
         """
         Read haplotypes from a .hap file line by line without storing anything
@@ -944,17 +1150,17 @@
             A list of haplotype IDs corresponding to a subset of the haplotypes to
             extract
 
             Defaults to loading haplotypes from all samples
 
         Yields
         ------
-        Iterator[Variant|Haplotype]
+        Iterator[Variant|Repeat|Haplotype]
             An iterator over each line in the file, where each line is encoded as a
-            Variant or Haplotype containing each of the class properties
+            Variant, Repeat, or Haplotype containing each of the class properties
 
         Examples
         --------
         If you're worried that the contents of the .hap file will be large, you may
         opt to parse the file line-by-line instead of loading it all into memory at
         once. In cases like these, you can use the __iter__() method in a for-loop:
 
@@ -979,16 +1185,21 @@
         # is indexed, then we should handle it using tabix
         # else, we use a regular text opener - b/c there's no benefit to using tabix
         if region or (haplotypes and indexed):
             haps_file = TabixFile(str(self.fname))
             metas, extras = self.check_header(list(haps_file.header))
             types = self._get_field_types(extras, metas.get("order"))
             # query for the variants of each haplotype
-            for hap in self._iter_haps(haps_file, types["H"], region, haplotypes):
+            for hap in self._iter_haps(haps_file, types, region, haplotypes):
                 yield hap
+
+                # If the haplotype is a repeat it will not have variants so continue
+                if isinstance(hap, Repeat):
+                    continue
+
                 # fetch region
                 # we already know that each line will start with a V, so we don't
                 # need to check that
                 for line in haps_file.fetch(reference=hap.id, multiple_iterators=True):
                     line_type = self._line_type(line)
                     if line_type == "V":
                         var = self.types["V"].from_hap_spec(line, types=types["V"])[1]
@@ -1021,17 +1232,17 @@
                             pass
                     else:
                         if header_lines:
                             metas, extras = self.check_header(header_lines)
                             types = self._get_field_types(extras, metas.get("order"))
                             header_lines = None
                             self.log.info("Finished reading header.")
-                        if line_type == "H":
-                            temp_hap = self.types["H"].from_hap_spec(
-                                line, types=types["H"]
+                        if line_type == "H" or line_type == "R":
+                            temp_hap = self.types[line_type].from_hap_spec(
+                                line, types=types[line_type]
                             )
                             if haplotypes is None or temp_hap.id in haplotypes:
                                 yield temp_hap
                         elif line_type == "V":
                             hap_id, var = self.types["V"].from_hap_spec(
                                 line, types=types["V"]
                             )
@@ -1048,34 +1259,40 @@
     def to_str(self, sort: bool = True) -> Generator[str, None, None]:
         """
         Create a string representation of this Haplotype
 
         Parameters
         ----------
         sort: bool, optional
-            Whether to attempt to output lines in sorted order
+            Whether to attempt to sort variant lines by their haplotype IDs
 
         Yields
         ------
         Generator[str, None, None]
             A list of lines (strings) to include in the output
         """
+        self.index()
         for symbol, line_instance in self.types.items():
             extras_order = line_instance.extras_order()
             if extras_order:
                 yield f"#\torder{symbol}\t" + "\t".join(extras_order)
         yield "#\tversion\t" + self.version
         for line_instance in self.types.values():
             yield from sorted(line_instance.extras_head())
+
         for hap in self.data.values():
-            yield self.types["H"].to_hap_spec(hap)
-        sorted_hap_ids = sorted(self.data.keys()) if sort else self.data.keys()
-        for hap_id in sorted_hap_ids:
-            for var in self.data[hap_id].variants:
-                yield self.types["V"].to_hap_spec(var, hap_id)
+            if isinstance(hap, Haplotype):
+                yield self.types["H"].to_hap_spec(hap)
+            elif isinstance(hap, Repeat):
+                yield self.types["R"].to_hap_spec(hap)
+
+        sorted_hap_ids = sorted(self.type_ids["H"]) if sort else self.type_ids["H"]
+        for hap in sorted_hap_ids:
+            for var in self.data[hap].variants:
+                yield self.types["V"].to_hap_spec(var, hap)
 
     def __repr__(self):
         return "\n".join(self.to_str())
 
     def write(self):
         """
         Write the contents of this Haplotypes object to the file at
@@ -1117,29 +1334,31 @@
             be stored
 
         Returns
         -------
         GenotypesVCF
             A Genotypes object composed of haplotypes instead of regular variants.
         """
+        self.index()
+        haps = [self.data[hap] for hap in self.type_ids["H"]]
         # Initialize GenotypesVCF return value
         if hap_gts is None:
             hap_gts = GenotypesVCF(fname=None, log=self.log)
         hap_gts.samples = gts.samples
         hap_gts.variants = np.array(
-            [(hap.id, hap.chrom, hap.start, ("A", "T")) for hap in self.data.values()],
+            [(hap.id, hap.chrom, hap.start, ("A", "T")) for hap in haps],
             dtype=hap_gts.variants.dtype,
         )
         # build a fast data structure for querying the alleles in each haplotype:
         # a dict mapping (variant ID, allele) -> a unique index
         alleles = {}
         # and a list of arrays containing the indices of each hap's alleles
-        idxs = [None] * len(self.data)
+        idxs = [None] * len(haps)
         count = 0
-        for i, hap in enumerate(self.data.values()):
+        for i, hap in enumerate(haps):
             idxs[i] = np.empty(len(hap.variants), dtype=np.uintc)
             for j, variant in enumerate(hap.variants):
                 key = (variant.id, variant.allele)
                 if key not in alleles:
                     alleles[key] = count
                     count += 1
                 idxs[i][j] = alleles[key]
@@ -1152,35 +1371,36 @@
             [
                 int(allele != gts.variants[i]["alleles"][0])
                 for i, (vID, allele) in enumerate(alleles)
             ],
             dtype=gts.data.dtype,
         )[np.newaxis, :, np.newaxis]
         # finally, obtain and merge the haplotype genotypes
-        self.log.info(f"Transforming genotypes for {len(self.data)} haplotypes")
-        equality_arr = np.equal(allele_arr, gts.data)
+        self.log.info(f"Transforming genotypes for {len(haps)} haplotypes")
+        equality_arr = np.equal(allele_arr, gts.data[:, :, :2])
         self.log.debug(
             f"Allocating array with dtype {gts.data.dtype} and size "
-            f"{(len(gts.samples), len(self.data), 2)}"
+            f"{(len(gts.samples), len(haps), 2)}"
         )
-        hap_gts.data = np.empty((gts.data.shape[0], len(self.data), 2), dtype=np.bool_)
+        hap_gts.data = np.empty((gts.data.shape[0], len(haps), 2), dtype=np.bool_)
         self.log.debug("Computing haplotype genotypes. This may take a while")
-        for i in range(len(self.data)):
+        for i in range(len(haps)):
             hap_gts.data[:, i] = np.all(equality_arr[:, idxs[i]], axis=1)
         return hap_gts
 
     def sort(self):
         """
         Sorts .hap files first by chrom, followed by start, end, and lastly ID
 
         Also sorts the variants within each haplotype
         """
         self.data = dict(sorted(self.data.items(), key=lambda item: item[1]))
-        for hap in self.data.values():
-            hap.sort()
+        self.index(force=True)
+        for hap in self.type_ids["H"]:
+            self.data[hap].sort()
 
     def subset(self, haplotypes: tuple[str], inplace: bool = False):
         """
         Subset these haplotypes to a smaller set of haplotypes
 
         The order of the haplotypes in the subsetted instance will match the order in
         the provided tuple parameters.
@@ -1212,9 +1432,10 @@
                 missing.add(hap_id)
         if len(missing):
             self.log.warning(
                 f"Saw {len(missing)} fewer haplotypes than requested. Proceeding with "
                 f"{len(hps.data)} haplotypes."
             )
         hps.data = data
+        hps.index(force=True)
         if not inplace:
             return hps
```

### Comparing `haptools-0.2.1/haptools/data/phenotypes.py` & `haptools-0.3.0/haptools/data/phenotypes.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     """
 
     def __init__(self, fname: Path | str, log: Logger = None):
         super().__init__(fname, log)
         self.samples = tuple()
         self.names = tuple()
         self._ext = "pheno"
+        self._samp_idx = None
+        self._name_idx = None
 
     @classmethod
     def load(
         cls: Phenotypes, fname: Path | str, samples: set[str] = None
     ) -> Phenotypes:
         """
         Load phenotypes from a pheno file
@@ -172,34 +174,38 @@
 
         Examples
         --------
         To write to a file, you must first initialize a Phenotypes object and then
         fill out the names, data, and samples properties:
         >>> phenotypes = Phenotypes('tests/data/simple.pheno')
         >>> phenotypes.names = ('height',)
-        >>> phenotypes.data = np.array([1, 1, 2], dtype='float64')
+        >>> phenotypes.data = np.array([[1, 1, 2]], dtype='float64')
         >>> phenotypes.samples = ('HG00096', 'HG00097', 'HG00099')
         >>> phenotypes.write()
         """
         # make sure the names are unique
         uniq_names = Counter()
         names = [None] * len(self.names)
         for idx, name in enumerate(self.names):
             suffix = ""
             if uniq_names[name]:
                 suffix = f"-{uniq_names[name]}"
             names[idx] = name + suffix
             uniq_names[name] += 1
+        # check that the phenotypes aren't a single vector; they must have a 2D shape!
+        # otherwise, negative signs won't get written correctly to the output
+        if len(self.data.shape) <= 1:
+            raise ValueError("The data property must have a 2D shape.")
         # now we can finally write the file
         with self.hook_compressed(self.fname, mode="w") as phens:
             phens.write("#IID\t" + "\t".join(names) + "\n")
             for samp, phen in zip(self.samples, self.data):
                 line = np.array2string(
                     phen,
-                    sign=" ",
+                    sign="-",
                     legacy=False,
                     separator="\t",
                     threshold=np.inf,
                     edgeitems=np.inf,
                     floatmode="unique",
                     suppress_small=False,
                     max_line_width=np.inf,
@@ -217,28 +223,31 @@
 
         Parameters
         ----------
         discard_also : bool, optional
             If True, discard any samples that are missing phenotypes without raising a
             ValueError
         """
+        if len(self.data.shape) <= 1:
+            raise ValueError("The data property must have a 2D shape.")
         # check: are there any samples that have phenotypes values that are -9?
         mask = self.data == -9
         missing = np.any(mask, axis=1)
         if np.any(missing):
             samp_idx = np.nonzero(missing)[0]
             missing_phens = np.nonzero(np.any(mask, axis=0))[0]
             if discard_also:
                 original_num_samples = len(self.samples)
                 self.data = np.delete(self.data, samp_idx, axis=0)
                 self.samples = tuple(np.delete(self.samples, samp_idx))
                 self.log.warning(
                     "Ignoring missing phenotypes from "
                     f"{original_num_samples - len(self.samples)} samples"
                 )
+                self._samp_idx = None
             else:
                 raise ValueError(
                     "Sample with ID {} for phenotype '{}' is missing".format(
                         self.samples[samp_idx[0]],
                         self.names[missing_phens[0]],
                     )
                 )
@@ -250,14 +259,16 @@
 
     def standardize(self):
         """
         Standardize phenotypes so they have a mean of 0 and a stdev of 1
 
         This function modifies :py:attr:`~.Phenotypes.data` in-place
         """
+        if len(self.data.shape) <= 1:
+            raise ValueError("The data property must have a 2D shape.")
         std = np.std(self.data, axis=0)
         self.data = (self.data - np.mean(self.data, axis=0)) / std
         # for phenotypes where the stdev is 0, just set all values to 0 instead of nan
         zero_elements = std == 0
         self.data[:, zero_elements] = np.zeros(
             (self.data.shape[0], np.sum(zero_elements))
         )
@@ -271,23 +282,127 @@
         name: str
             The name of the new phenotype
         data: npt.NDArray
             A 1D np array of the same length as :py:attr:`~.Phenotypes.samples`,
             containing the phenotype values for each sample. Must have the same dtype
             as :py:attr:`~.Phenotypes.data.`
         """
+        if len(data.shape) != 1:
+            raise ValueError("The data argument must have a 1D shape.")
         if len(self.samples):
             if len(self.samples) != len(data):
                 self.log.error(
                     "The data provided to the add() method is not of the appropriate"
                     "length"
                 )
         else:
             self.log.warning(
                 "Set the samples property of the Phenotypes instance before calling "
                 "the add() method"
             )
         if self.unset():
             self.data = data[:, np.newaxis]
         else:
+            if len(self.data.shape) <= 1:
+                raise ValueError("The data property must have a 2D shape.")
             self.data = np.concatenate((self.data, data[:, np.newaxis]), axis=1)
+        if self._name_idx is not None:
+            self._name_idx[name] = len(self.names)
         self.names = self.names + (name,)
+
+    def index(self, samples: bool = True, names: bool = True):
+        """
+        Call this function once to improve the amortized time-complexity of look-ups of
+        samples and names by their ID. This is useful if you intend to later subset
+        by a set of samples or name IDs.
+        The time complexity of this function should be roughly O(n+p) if both
+        parameters are True. Otherwise, it will be either O(n) or O(p).
+
+        Parameters
+        ----------
+        samples: bool, optional
+            Whether to index the samples for fast loop-up. Adds complexity O(n).
+        names: bool, optional
+            Whether to index the names for fast look-up. Adds complexity O(p).
+
+        Raises
+        ------
+        ValueError
+            If any samples or names appear more than once
+        """
+        if samples and self._samp_idx is None:
+            self._samp_idx = dict(zip(self.samples, range(len(self.samples))))
+            if len(self._samp_idx) < len(self.samples):
+                duplicates = Counter(self.samples).items()
+                duplicates = [samp_id for samp_id, count in duplicates if count > 1]
+                a_few = 5 if len(duplicates) > 5 else len(duplicates)
+                raise ValueError(f"Found duplicate sample IDs: {duplicates[:a_few]}")
+        if names and self._name_idx is None:
+            self._name_idx = dict(zip(self.names, range(len(self.names))))
+            if len(self._name_idx) < len(self.names):
+                duplicates = Counter(self.names).items()
+                duplicates = [name_id for name_id, count in duplicates if count > 1]
+                a_few = 5 if len(duplicates) > 5 else len(duplicates)
+                raise ValueError(f"Found duplicate name IDs: {duplicates[:a_few]}")
+
+    def subset(
+        self,
+        samples: tuple[str] = None,
+        names: tuple[str] = None,
+        inplace: bool = False,
+    ):
+        """
+        Subset these phenotypes to a smaller set of samples or a smaller set of names
+
+        The order of the samples and names in the subsetted instance will match
+        the order in the provided tuple parameters.
+
+        Parameters
+        ----------
+        samples: tuple[str]
+            A subset of samples to keep
+        names: tuple[str]
+            A subset of phenotype IDs to keep
+        inplace: bool, optional
+            If False, return a new Phenotypes object; otherwise, alter the current one
+
+        Returns
+        -------
+            A new Phenotypes object if inplace is set to False, else returns None
+        """
+        # First, initialize variables
+        pts = self
+        if not inplace:
+            pts = self.__class__(self.fname, self.log)
+        pts.samples = self.samples
+        pts.names = self.names
+        pts.data = self.data
+        # Index the current set of samples and names so we can have fast look-up
+        self.index(samples=(samples is not None), names=(names is not None))
+        # Subset the samples
+        if samples is not None:
+            pts.samples = tuple(samp for samp in samples if samp in self._samp_idx)
+            if len(pts.samples) < len(samples):
+                diff = len(samples) - len(pts.samples)
+                self.log.warning(
+                    f"Saw {diff} fewer samples than requested. Proceeding with "
+                    f"{len(pts.samples)} samples."
+                )
+            samp_idx = tuple(self._samp_idx[samp] for samp in pts.samples)
+            if inplace:
+                self._samp_idx = None
+            pts.data = pts.data[samp_idx, :]
+        # Subset the names
+        if names is not None:
+            pts.names = tuple(name for name in names if name in self._name_idx)
+            if len(pts.names) < len(names):
+                diff = len(names) - len(pts.names)
+                self.log.warning(
+                    f"Saw {diff} fewer names than requested. Proceeding with "
+                    f"{len(pts.names)} names."
+                )
+            name_idx = tuple(self._name_idx[name] for name in pts.names)
+            if inplace:
+                self._pts.names = None
+            pts.data = pts.data[:, name_idx]
+        if not inplace:
+            return pts
```

### Comparing `haptools-0.2.1/haptools/index.py` & `haptools-0.3.0/haptools/index.py`

 * *Files identical despite different names*

### Comparing `haptools-0.2.1/haptools/karyogram.py` & `haptools-0.3.0/haptools/karyogram.py`

 * *Files identical despite different names*

### Comparing `haptools-0.2.1/haptools/ld.py` & `haptools-0.3.0/haptools/ld.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,28 +108,41 @@
     haplotype_ids = None
     if not from_gts:
         haplotype_ids = ids
         if haplotype_ids is not None:
             haplotype_ids.add(target)
     hp.read(region=region, haplotypes=haplotype_ids)
 
+    # remove all repeats from the haplotypes object since we don't yet support them
+    for repeat_id in hp.type_ids["R"]:
+        del hp.data[repeat_id]
+    num_repeats = len(hp.type_ids["R"])
+    if num_repeats:
+        log.info(f"Ignoring {num_repeats} repeats in .hap file")
+        hp.type_ids["R"] = []
+
     if from_gts:
         variants = None
         if target in hp.data and ids:
             variants = ids.copy()
             log.info("Extracting variants from haplotypes")
             variants.update(var.id for var in hp.data[target].variants)
     else:
         log.info("Extracting variants from haplotypes")
-        variants = {var.id for hap in hp.data.values() for var in hap.variants}
+        variants = {var.id for h in hp.type_ids["H"] for var in hp.data[h].variants}
 
     # check to see whether the target was a haplotype
-    if target in hp.data:
-        log.info(f"Identified target '{target}' as a haplotype")
+    try:
         target = hp.data.pop(target)
+    except:
+        # the target is a variant, instead
+        pass
+    else:
+        log.info(f"Identified target '{target}' as a haplotype")
+        hp.index(force=True)
         if len(hp.data) == 0 and not from_gts:
             log.error(
                 "There must be at least one more haplotype in the .hap file "
                 "than the TARGET haplotype specified."
             )
 
     # check that all of the haplotypes were loaded successfully and warn otherwise
@@ -202,15 +215,15 @@
                 variant_ld = pearson_corr_ld(target_gts, variant_gts)
                 ld_file.write(f"{var_chr}\t{var_bp}\t{var_snp}\t{variant_ld:.3f}\n")
     else:
         log.info("Computing LD between haplotypes and the target")
         # construct a new Haplotypes object that also stores the LD values
         hp_out = data.Haplotypes(fname=output, haplotype=Haplotype, log=log)
         hp_out.data = {}
-        for hap_id in hp.data:
+        for hap_id in hp.type_ids["H"]:
             # break the BaseHaplotype instance up into its properties
             hapd = hp.data[hap_id].__dict__
             hapd_variants = hapd.pop("variants")
             # obtain genotypes for the current haplotype
             hap_gts = hp_gt.subset(variants=(hap_id,)).data[:, 0, :2].sum(axis=1)
             # compute the LD between the current haplotype and the target
             hapd["ld"] = pearson_corr_ld(target_gts, hap_gts)
```

### Comparing `haptools-0.2.1/haptools/logging.py` & `haptools-0.3.0/haptools/logging.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import logging
 
 
-def getLogger(name: str = None, level: str = "ERROR"):
+def getLogger(name: str = None, level: str = "ERROR", exact_time=False):
     """
     Retrieve a Logger object
 
     Parameters
     ----------
     name : str, optional
         The name of the logging object
@@ -23,15 +23,19 @@
     logger.setLevel(level)
 
     # create console handler and set level to debug
     ch = logging.StreamHandler()
     ch.setLevel(level)
 
     # create formatter
-    db_time = "|%(asctime)s" if level == "DEBUG" else ""
+    db_time = (
+        ("|%(asctime)s" + (".%(msecs)03d" if exact_time else ""))
+        if level == "DEBUG"
+        else ""
+    )
     formatter = logging.Formatter(
         fmt="[%(levelname)8s" + db_time + "] %(message)s (%(filename)s:%(lineno)s)",
         datefmt="%H:%M:%S",
     )
 
     # add formatter to ch
     ch.setFormatter(formatter)
```

### Comparing `haptools-0.2.1/haptools/sim_genotype.py` & `haptools-0.3.0/haptools/sim_genotype.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,16 @@
         else:
             return int(chrom)
 
     # sort coordinate files to ensure coords read are in sorted order
     # remove all chr files not found in chroms list
     all_coord_files = glob.glob(f'{coords_dir}/*.map')
     all_coord_files = [coord_file for coord_file in all_coord_files \
-                if re.search(r'(?<=chr)(X|\d+)', coord_file).group() in chroms]
+                if re.search(r'(?<=chr)(X|\d+)', coord_file) and \
+                   re.search(r'(?<=chr)(X|\d+)', coord_file).group() in chroms]
     all_coord_files.sort(key=numeric_alpha)
 
     if len(all_coord_files) != len(chroms):
         raise Exception(f"Unable to find all chromosomes {chroms} in map file directory.")
     
     # coords list has form chroms x coords
     coords = []
@@ -864,20 +865,23 @@
         if chrom not in valid_chroms:
             raise Exception(f"Chromosome {chrom} in the list given is not valid.")
 
     # Validate mapdir ensuring it contains proper files.
     try:
         all_coord_files = glob.glob(f'{mapdir}/*.map')
         all_coord_files = [coord_file for coord_file in all_coord_files \
-            if re.search(r'(?<=chr)(X|\d+)', coord_file).group() in chroms]
+            if re.search(r'(?<=chr)(X|\d+)', coord_file) and \
+               re.search(r'(?<=chr)(X|\d+)', coord_file).group() in chroms]
     except:
-        raise Exception("Could not parse map directory files.")
+        raise Exception("No valid coordinate files found. Must contain chr{1-22,X} in the file name"
+                        " and end in .map")
     
     if not all_coord_files:
-        raise Exception("No valid coordinate files found. Must contain chr{1-22,X} in the file name.")
+        raise Exception("No valid coordinate files found. Must contain chr{1-22,X} in the file name"
+                        " and end in .map")
     
     # validate popsize
     if not isinstance(popsize, int):
         raise Exception("Popsize is not an Integer.")
     if popsize <= 0:
         raise Exception("Popsize must be greater than 0.")
```

### Comparing `haptools-0.2.1/haptools/sim_phenotype.py` & `haptools-0.3.0/haptools/sim_phenotype.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,62 @@
 from pathlib import Path
 from dataclasses import dataclass, field
 
 import numpy as np
 import numpy.typing as npt
 
 from .logging import getLogger
-from .data import Haplotype as HaplotypeBase
 from .data import (
     Extra,
     Genotypes,
     Phenotypes,
     Haplotypes,
+    GenotypesTR,
     GenotypesPLINK,
+    Repeat as RepeatBase,
+    Haplotype as HaplotypeBase,
 )
 
 
 @dataclass
+class Effect:
+    """
+    A variable in the simphenotype linear model
+
+    Attributes
+    ----------
+    id : str
+        The ID of the variable; corresponds to a variant in a Genotypes object
+    beta : float
+        The effect size of the variable
+    """
+
+    id: str
+    beta: float
+
+    @classmethod
+    def from_hap_spec(cls: Effect, line: str) -> Effect:
+        """
+        Convert a .snplist line into an Effect object
+
+        Parameters
+        ----------
+        line: str
+            A line from a .snplist file
+
+        Returns
+        -------
+        Effect
+            The converted Effect instance
+        """
+        ID, beta = line.split("\t")[:2]
+        return cls(id=ID, beta=float(beta))
+
+
+@dataclass
 class Haplotype(HaplotypeBase):
     """
     A haplotype with sufficient fields for simphenotype
 
     Properties and functions are shared with the base Haplotype object, "HaplotypeBase"
     """
 
@@ -29,32 +66,49 @@
     _extras: tuple = field(
         repr=False,
         init=False,
         default=(Extra("beta", ".2f", "Effect size in linear model"),),
     )
 
 
+@dataclass
+class Repeat(RepeatBase):
+    """
+    A repeat with sufficient fields for simphenotype
+
+    Properties and functions are shared with the base Repeat object, "RepeatBeta"
+    """
+
+    beta: float
+    _extras: tuple = field(
+        repr=False,
+        init=False,
+        default=(Extra("beta", ".2f", "Effect size in linear model"),),
+    )
+
+
 class PhenoSimulator:
     """
     Simulate phenotypes from genotypes
 
     Attributes
     ----------
-    gens: Genotypes
+    gens: dict[Genotypes]
         Genotypes to simulate
     phens: Phenotypes
         Simulated phenotypes; filled by :py:meth:`~.PhenoSimular.run`
     rng: np.random.Generator, optional
         A numpy random number generator
     log: logging.Logger
         A logging instance for recording debug statements
 
     Examples
     --------
     >>> gens = Genotypes.load("tests/data/example.vcf.gz")
+    >>> tr_gens = GenotypesTR.load("tests/data/simple_tr.vcf")
     >>> haps = Haplotypes.load("tests/data/basic.hap")
     >>> haps_gts = haps.transform(gens)
     >>> phenosim = PhenoSimulator(haps_gts)
     >>> phenosim.run(haps.data.values())
     >>> phenotypes = phenosim.phens
     """
 
@@ -89,91 +143,90 @@
         self.phens.data = None
         self.phens.samples = self.gens.samples
         self.rng = np.random.default_rng(seed)
         self.log = log or logging.getLogger(self.__class__.__name__)
 
     def run(
         self,
-        effects: list[Haplotype],
+        effects: list[Effect | Haplotype | Repeat],
         heritability: float = None,
         prevalence: float = None,
         normalize: bool = True,
+        environment: float = None,
     ) -> npt.NDArray:
         """
         Simulate phenotypes for an entry in the Genotypes object
 
         The generated phenotypes will also be added to
         :py:attr:`~.PhenoSimulator.output`
 
         Parameters
         ----------
-        effects: list[Haplotype]
+        effects: list[Effect|Haplotype|Repeat]
             A list of Haplotypes to use in an additive fashion within the simulations
         heritability: float, optional
             The simulated heritability of the trait
 
             If not provided, this will default to the sum of the squared effect sizes
         prevalence: float, optional
             How common should the disease be within the population?
 
             If this value is specified, case/control phenotypes will be generated
             instead of quantitative traits.
         normalize: bool, optional
             If True, normalize the genotypes before using them to simulate the
             phenotypes. Otherwise, use the raw values.
+        environment: float, optional
+            The variance (aka strength) of the environmental contribution to the trait.
+            This is inferred from the betas if it isn't specified.
 
         Returns
         -------
         npt.NDArray
             The simulated phenotypes, as a np array of shape num_samples x 1
         """
         # extract the relevant haplotype info from the Haplotype objects
-        ids = [hap.id for hap in effects]
-        betas = np.array([hap.beta for hap in effects])
-        self.log.debug(f"Extracting haplotype genotypes for haps: {ids}")
+        ids = [effect.id for effect in effects]
+        betas = np.array([effect.beta for effect in effects])
         self.log.debug(f"Beta values are {betas}")
-        # extract the haplotype "genotypes" and compute the phenotypes
+        self.log.debug(f"Extracting haplotype genotypes for haps: {ids}")
         gts = self.gens.subset(variants=ids).data[:, :, :2].sum(axis=2)
-        self.log.info(f"Computing genetic component w/ {gts.shape[1]} causal effects")
-        # standardize the genotypes
+
         if normalize:
-            std = gts.std(axis=0)
-            gts = (gts - gts.mean(axis=0)) / std
-            # when the stdev is 0, just set all values to 0 instead of nan
-            zero_elements = std == 0
-            num_zero_elements = np.sum(zero_elements)
-            if num_zero_elements:
-                # get the first five causal variables with variances == 0
-                zero_elements_ids = np.array(ids)[zero_elements]
-                if len(zero_elements_ids) > 5:
-                    zero_elements_ids = zero_elements_ids[:5]
-                self.log.warning(
-                    "Some of your causal variables have genotypes with variance 0. "
-                    f"Here are the first few few: {zero_elements_ids}"
-                )
-            gts[:, zero_elements] = np.zeros((gts.shape[0], num_zero_elements))
+            gts = self.normalize_gts(gts, ids)
+
+        self.log.info(f"Computing genetic component w/ {gts.shape[1]} causal effects")
+
         # generate the genetic component
         pt = (betas * gts).sum(axis=1)
         # compute the heritability
-        if heritability is None:
+        if heritability is None and environment is None:
             self.log.debug("Computing heritability as the sum of the squared betas")
             heritability = np.power(betas, 2).sum()
             if heritability > 1:
+                self.log.warning(
+                    "Variance of error term exceeds 1. Check your betas! Capping at 1 "
+                    "for now."
+                )
                 heritability = 1
             # compute the environmental effect
             noise = 1 - heritability
         else:
-            # compute the environmental effect
-            noise = np.var(pt)
-            if noise == 0:
-                self.log.warning(
-                    "Your genotypes have a variance of 0. Creating artificial noise..."
-                )
-                noise = 1
-            # TODO: handle a heritability of 0 somehow
+            noise = environment
+            if environment is None:
+                # compute the environmental effect
+                noise = np.var(pt)
+                if noise == 0:
+                    self.log.warning(
+                        "Your genotypes have 0 variance. Creating artificial noise..."
+                    )
+                    noise = 1
+            elif heritability is None:
+                heritability = 0.5
+            # TODO: handle a heritability of 0 somehow?
             noise *= np.reciprocal(heritability) - 1
         self.log.info(f"Adding environmental component {noise} for h^2 {heritability}")
         # finally, add everything together to get the simulated phenotypes
         pt_noise = self.rng.normal(0, np.sqrt(noise), size=pt.shape)
         if self.log.getEffectiveLevel() == logging.DEBUG:
             # if we're in debug mode, compute the pearson correlation and report it
             # but don't do this otherwise to keep things fast
@@ -195,33 +248,68 @@
                 bool_pt[max_indices] = True
             pt = bool_pt
             name_suffix = "-cc"
         # now, save the archived phenotypes for later
         self.phens.append(name="-".join(ids) + name_suffix, data=pt.astype(np.float64))
         return pt
 
+    def normalize_gts(self, gts, ids):
+        """
+        Normalize variant or repeats genotypes
+
+        Parameters
+        ----------
+        gts: np.array
+            Genotypes variant array stored in data.
+        ids: list[str]
+            IDs for variants
+
+        Returns
+        -------
+        normalized_gts: np.array
+            Normalized Genotypes variant array.
+        """
+        std = gts.std(axis=0)
+        gts = (gts - gts.mean(axis=0)) / std
+        # when the stdev is 0, just set all values to 0 instead of nan
+        zero_elements = std == 0
+        num_zero_elements = np.sum(zero_elements)
+        if num_zero_elements:
+            # get the first five causal variables with variances == 0
+            zero_elements_ids = np.array(ids)[zero_elements]
+            if len(zero_elements_ids) > 5:
+                zero_elements_ids = zero_elements_ids[:5]
+            self.log.warning(
+                "Some of your causal variables have genotypes with variance 0. "
+                f"Here are the first few: {zero_elements_ids}"
+            )
+        gts[:, zero_elements] = np.zeros((gts.shape[0], num_zero_elements))
+        return gts
+
     def write(self):
         """
         Write the generated phenotypes to the file specified in
         :py:meth:`~.PhenoSimular.__init__`
         """
         self.phens.write()
 
 
 def simulate_pt(
     genotypes: Path,
     haplotypes: Path,
     num_replications: int = 1,
+    environment: float = None,
     heritability: float = None,
     prevalence: float = None,
     normalize: bool = True,
     region: str = None,
     samples: list[str] = None,
     haplotype_ids: set[str] = None,
     chunk_size: int = None,
+    repeats: Path = None,
     seed: int = None,
     output: Path = Path("-"),
     log: logging.Logger = None,
 ):
     """
     Haplotype-aware phenotype simulation. Create a set of simulated phenotypes from a
     set of haplotypes.
@@ -276,51 +364,97 @@
         If not provided, all haplotypes will be used.
     chunk_size: int, optional
         The max number of variants to fetch from the PGEN file at any given time
 
         If this value is provided, variants from the PGEN file will be loaded in
         chunks so as to use less memory. This argument is ignored if the genotypes are
         not in PGEN format.
+    repeats: Path, optional
+        The path to a genotypes file containing tandem repeats. This is only necessary
+        when simulating both haplotypes *and* repeats as causal effects
+    environment: float, optional
+        The variance (aka strength) of the environmental term. This will be inferred if
+        it isn't specified.
+    seed: int, optional
+        Seed for random processes
     output : Path, optional
         The location to which to write the simulated phenotypes
     log : logging.Logger, optional
         The logging module for this task
     """
     if log is None:
         log = getLogger(name="simphenotype", level="ERROR")
 
-    log.info("Loading haplotypes")
-    hp = Haplotypes(haplotypes, haplotype=Haplotype, log=log)
-    hp.read(region=region, haplotypes=haplotype_ids)
-
-    if haplotype_ids is None:
-        haplotype_ids = set(hp.data.keys())
-
-    if genotypes.suffix == ".pgen":
-        log.info("Loading genotypes from PGEN file")
-        gt = GenotypesPLINK(fname=genotypes, log=log, chunk_size=chunk_size)
+    load_as_haps = True
+    # either load SNPs from the snplist file or load haps/repeats from the hap file
+    if haplotypes.suffix == ".snplist":
+        log.info("Loading from .snplist")
+        with open(haplotypes) as snplist_file:
+            effects = map(Effect.from_hap_spec, snplist_file.readlines())
+        if haplotype_ids is None:
+            effects = list(effects)
+            haplotype_ids = set(effect.id for effect in effects)
+        else:
+            effects = list(filter(lambda e: e.id in haplotype_ids, effects))
     else:
-        log.info("Loading genotypes from VCF/BCF file")
-        gt = Genotypes(fname=genotypes, log=log)
+        log.info("Loading from .hap")
+        hp = Haplotypes(haplotypes, haplotype=Haplotype, repeat=Repeat, log=log)
+        hp.read(region=region, haplotypes=haplotype_ids)
+        effects = hp.data.values()
+
+        if haplotype_ids is None:
+            haplotype_ids = set(hp.data.keys())
+
+        # check if these are all repeat IDs, haplotype IDs, or a mix of them
+        if len(hp.type_ids["R"]) >= len(haplotype_ids) and repeats is None:
+            # if they're all repeat IDs or --repeats was specified
+            log.info("Loading TR genotypes")
+            gt = GenotypesTR(fname=genotypes, log=log)
+            load_as_haps = False
+        else:
+            # the genotypes variable must contain haplotype genotypes
+            # but first, check if they're a mix but --repeats wasn't specified
+            if len(hp.type_ids["H"]) < len(haplotype_ids) and repeats is None:
+                raise ValueError(
+                    "The --repeats option must be specified when simulating a mix of"
+                    " both haplotypes and repeats as causal effects."
+                )
+
+    if load_as_haps:
+        # load these as haplotype pseudo-genotypes
+        if genotypes.suffix == ".pgen":
+            log.info("Loading haplotype genotypes from PGEN file")
+            gt = GenotypesPLINK(fname=genotypes, log=log, chunk_size=chunk_size)
+        else:
+            log.info("Loading haplotype genotypes from VCF/BCF file")
+            gt = Genotypes(fname=genotypes, log=log)
+
     # gt._prephased = True
     gt.read(region=region, samples=samples, variants=haplotype_ids)
     log.info("QC-ing genotypes")
     gt.check_missing()
-    gt.check_biallelic()
+
+    if repeats:
+        log.info("Merging with TR genotypes")
+        tr_gt = GenotypesTR(fname=repeats, log=log)
+        tr_gt.read(region=region, samples=samples, variants=haplotype_ids)
+        tr_gt.check_missing()
+        gt = Genotypes.merge_variants((gt, tr_gt), fname=None)
 
     # check that all of the genotypes were loaded successfully and warn otherwise
     if len(haplotype_ids) < len(gt.variants):
         diff = list(haplotype_ids.difference(gt.variants["id"]))
         first_few = 5 if len(diff) > 5 else len(diff)
         log.warning(
-            f"{len(diff)} haplotypes could not be found in the genotypes file. Check "
-            "that the hap IDs in your .hap file correspond with those in the genotypes"
-            f" file. Here are the first few missing variants: {diff[:first_few]}"
+            f"{len(diff)} effects could not be found in the genotypes file. Check "
+            "that the IDs in your .snplist or .hap file correspond with those in the "
+            "genotypes file. Here are the first few missing variants: "
+            f"{diff[:first_few]}"
         )
 
     # Initialize phenotype simulator (haptools simphenotype)
     log.info("Simulating phenotypes")
     pt_sim = PhenoSimulator(gt, output=output, seed=seed, log=log)
     for i in range(num_replications):
-        pt_sim.run(hp.data.values(), heritability, prevalence, normalize)
+        pt_sim.run(effects, heritability, prevalence, normalize, environment)
     log.info("Writing phenotypes")
     pt_sim.write()
```

### Comparing `haptools-0.2.1/haptools/transform.py` & `haptools-0.3.0/haptools/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,31 +89,33 @@
         super().__init__(fname, haplotype=haplotype, variant=variant, log=log)
 
     def transform(
         self,
         gts: data.GenotypesAncestry,
         hap_gts: data.GenotypesVCF = None,
     ) -> data.GenotypesVCF:
+        self.index()
+        haps = [self.data[hap] for hap in self.type_ids["H"]]
         # Initialize GenotypesVCF return value
         if hap_gts is None:
             hap_gts = data.GenotypesVCF(fname=None, log=self.log)
         hap_gts.samples = gts.samples
         hap_gts.variants = np.array(
-            [(hap.id, hap.chrom, hap.start, ("A", "T")) for hap in self.data.values()],
+            [(hap.id, hap.chrom, hap.start, ("A", "T")) for hap in haps],
             dtype=hap_gts.variants.dtype,
         )
         # build a fast data structure for querying the alleles in each haplotype:
         # a dict mapping (variant ID, allele) -> a unique index
         alleles = {}
         # and a list of arrays containing the indices of each hap's alleles
-        idxs = [None] * len(self.data)
+        idxs = [None] * len(haps)
         # and lastly, a list of ancestral population labels for each hap
-        ancestries = np.empty(len(self.data), dtype=np.uint8)
+        ancestries = np.empty(len(haps), dtype=np.uint8)
         count = 0
-        for i, hap in enumerate(self.data.values()):
+        for i, hap in enumerate(haps):
             ancestries[i] = gts.ancestry_labels.get(hap.ancestry, -1)
             idxs[i] = np.empty(len(hap.variants), dtype=np.uintc)
             for j, variant in enumerate(hap.variants):
                 key = (variant.id, variant.allele)
                 if key not in alleles:
                     alleles[key] = count
                     count += 1
@@ -127,23 +129,23 @@
             [
                 int(allele != gts.variants[i]["alleles"][0])
                 for i, (vID, allele) in enumerate(alleles)
             ],
             dtype=gts.data.dtype,
         )[np.newaxis, :, np.newaxis]
         # finally, obtain and merge the haplotype genotypes
-        self.log.info(f"Transforming genotypes for {len(self.data)} haplotypes")
+        self.log.info(f"Transforming genotypes for {len(haps)} haplotypes")
         equality_arr = np.equal(allele_arr, gts.data)
         self.log.debug(
             f"Allocating array with dtype {gts.data.dtype} and size "
-            f"{(len(gts.samples), len(self.data), 2)}"
+            f"{(len(gts.samples), len(haps), 2)}"
         )
-        hap_gts.data = np.empty((gts.data.shape[0], len(self.data), 2), dtype=np.bool_)
+        hap_gts.data = np.empty((gts.data.shape[0], len(haps), 2), dtype=np.bool_)
         self.log.debug("Computing haplotype genotypes. This may take a while")
-        for i in range(len(self.data)):
+        for i in range(len(haps)):
             hap_gts.data[:, i] = np.logical_and(
                 np.all(gts.ancestry[:, idxs[i]] == ancestries[i], axis=1),
                 np.all(equality_arr[:, idxs[i]], axis=1),
             )
         return hap_gts
 
 
@@ -513,14 +515,22 @@
                     record.samples[sample].phased = True
                 else:
                     record.samples[sample].phased = self.data[samp_idx, var_idx, 2]
             # write the record to a file
             vcf.write(record)
         vcf.close()
 
+    def merge_variants(
+        cls, objs: tuple[data.Genotypes], check_samples: bool = True, **kwargs
+    ) -> data.Genotypes:
+        """
+        See documentation for :py:meth:`~.data.Genotypes.merge_variants`
+        """
+        raise NotImplementedError
+
 
 def transform_haps(
     genotypes: Path,
     haplotypes: Path,
     region: str = None,
     samples: list[str] = None,
     haplotype_ids: set[str] = None,
@@ -581,15 +591,15 @@
         log.warning(
             f"{len(diff)} haplotypes could not be found in the .hap file. Check "
             "that the IDs in your .hap file correspond with those you provided. "
             f"Here are the first few missing haplotypes: {diff[:first_few]}"
         )
 
     log.info("Extracting variants from haplotypes")
-    variants = {var.id for hap in hp.data.values() for var in hap.variants}
+    variants = {vr.id for id in hp.type_ids["H"] for vr in hp.data[id].variants}
 
     # load the genotypes, but first get the path to the breakpoints file
     if genotypes.suffix == ".gz":
         bps_file = genotypes.with_suffix("").with_suffix(".bp")
     else:
         bps_file = genotypes.with_suffix(".bp")
     # now, get the genotypes
```

### Comparing `haptools-0.2.1/pyproject.toml` & `haptools-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "haptools"
-version = "v0.2.1"
+version = "v0.3.0"
 description = "Ancestry and haplotype aware simulation of genotypes and phenotypes for complex trait analysis"
 authors = ["Arya Massarat", "Michael Lamkin"]
 license = "MIT"
 repository = "https://github.com/cast-genomics/haptools"
 homepage = "https://github.com/cast-genomics/haptools"
 documentation = "https://haptools.readthedocs.io"
 readme = "README.md"
@@ -12,15 +12,15 @@
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 numpy = ">=1.20.0"
 click = ">=8.0.3"
 pysam = ">=0.19.0"
 cyvcf2 = ">=0.30.14"
 matplotlib = ">=3.5.1"
-Pgenlib = { version = ">=0.81.3", optional = true }
+Pgenlib = {version = ">=0.81.3", optional = true, extras = ["files"]}
 
 # docs
 # these belong in dev-dependencies, but RTD doesn't support that yet -- see
 # https://github.com/readthedocs/readthedocs.org/issues/4912
 Sphinx = { version = ">=4.3.2", optional = true }
 sphinx-autodoc-typehints = { version = ">=1.12.0", optional = true }
 sphinx-rtd-theme = { version = ">=1.0.0", optional = true }
```

### Comparing `haptools-0.2.1/setup.py` & `haptools-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 
 extras_require = \
 {'docs': ['Sphinx>=4.3.2',
           'sphinx-autodoc-typehints>=1.12.0',
           'sphinx-rtd-theme>=1.0.0',
           'numpydoc>=1.1.0',
           'sphinx-click>=3.0.2'],
- 'files': ['Pgenlib>=0.81.3']}
+ 'files': ['Pgenlib[files]>=0.81.3']}
 
 entry_points = \
 {'console_scripts': ['haptools = haptools.__main__:main']}
 
 setup_kwargs = {
     'name': 'haptools',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Ancestry and haplotype aware simulation of genotypes and phenotypes for complex trait analysis',
     'long_description': '# haptools\n[![pypi version](https://img.shields.io/pypi/v/haptools)](https://pypi.org/project/haptools)\n[![image](https://anaconda.org/bioconda/haptools/badges/version.svg)](https://anaconda.org/bioconda/haptools)\n[![license](https://img.shields.io/pypi/l/haptools)](LICENSE)\n![status](https://github.com/CAST-genomics/haptools/workflows/Tests/badge.svg)\n\nHaptools is a collection of tools for simulating and analyzing genotypes and phenotypes while taking into account haplotype information. Haptools supports fast simulation of admixed genomes (with `simgenotype`), visualization of admixture tracks (with `karyogram`), simulating haplotype- and local ancestry-specific phenotype effects (with `transform` and `simphenotype`), and computing a variety of common file operations and statistics in a haplotype-aware manner.\n\nHomepage: [https://haptools.readthedocs.io/](https://haptools.readthedocs.io/)\n\nVisit our homepage for installation and usage instructions.\n\n![haptools commands](https://drive.google.com/uc?id=1c0i_Hjms7579s24zRsKp5yMs7BxNHed_)\n\n## citation\nThere is an option to _"Cite this repository"_ on the right sidebar of [the repository homepage](https://github.com/CAST-genomics/haptools)\n\n> Arya R Massarat, Michael Lamkin, Ciara Reeve, Amy L Williams, Matteo D’Antonio, Melissa Gymrek, Haptools: a toolkit for admixture and haplotype analysis, Bioinformatics, 2023;, btad104, https://doi.org/10.1093/bioinformatics/btad104\n',
     'author': 'Arya Massarat',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cast-genomics/haptools',
```

### Comparing `haptools-0.2.1/PKG-INFO` & `haptools-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: haptools
-Version: 0.2.1
+Version: 0.3.0
 Summary: Ancestry and haplotype aware simulation of genotypes and phenotypes for complex trait analysis
 Home-page: https://github.com/cast-genomics/haptools
 License: MIT
 Author: Arya Massarat
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: docs
 Provides-Extra: files
 Provides-Extra: tests
-Requires-Dist: Pgenlib (>=0.81.3) ; extra == "files"
+Requires-Dist: Pgenlib[files] (>=0.81.3) ; extra == "files"
 Requires-Dist: Sphinx (>=4.3.2) ; extra == "docs"
 Requires-Dist: click (>=8.0.3)
 Requires-Dist: cyvcf2 (>=0.30.14)
 Requires-Dist: matplotlib (>=3.5.1)
 Requires-Dist: numpy (>=1.20.0)
 Requires-Dist: numpydoc (>=1.1.0) ; extra == "docs"
 Requires-Dist: pysam (>=0.19.0)
```

