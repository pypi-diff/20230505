# Comparing `tmp/GenBioX-0.3.tar.gz` & `tmp/GenBioX-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenBioX-0.3.tar", last modified: Thu May  4 03:39:29 2023, max compression
+gzip compressed data, was "GenBioX-0.3.1.tar", last modified: Fri May  5 13:32:40 2023, max compression
```

## Comparing `GenBioX-0.3.tar` & `GenBioX-0.3.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.053618 GenBioX-0.3/
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.046660 GenBioX-0.3/GenBioX/
--rw-r--r--   0 li         (501) staff       (20)        0 2023-03-12 06:16:05.000000 GenBioX-0.3/GenBioX/__init__.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.047949 GenBioX-0.3/GenBioX/alignment/
--rw-r--r--   0 li         (501) staff       (20)      247 2023-05-02 09:24:07.000000 GenBioX-0.3/GenBioX/alignment/__init__.py
--rw-r--r--   0 li         (501) staff       (20)      803 2023-03-29 11:45:13.000000 GenBioX-0.3/GenBioX/alignment/align.py
--rw-r--r--   0 li         (501) staff       (20)      720 2023-04-28 11:19:37.000000 GenBioX-0.3/GenBioX/alignment/evaluate_alignment_quality.py
--rw-r--r--   0 li         (501) staff       (20)     1316 2023-04-28 11:13:12.000000 GenBioX-0.3/GenBioX/alignment/extract_conserved_regions.py
--rw-r--r--   0 li         (501) staff       (20)      810 2023-04-28 11:09:16.000000 GenBioX-0.3/GenBioX/alignment/merge_alignments.py
--rw-r--r--   0 li         (501) staff       (20)      740 2023-04-28 11:39:45.000000 GenBioX-0.3/GenBioX/alignment/read_alignment.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.048887 GenBioX-0.3/GenBioX/annotation/
--rw-r--r--   0 li         (501) staff       (20)      155 2023-05-02 09:26:59.000000 GenBioX-0.3/GenBioX/annotation/__init__.py
--rw-r--r--   0 li         (501) staff       (20)     2719 2023-03-13 06:47:14.000000 GenBioX-0.3/GenBioX/annotation/annotation.py
--rw-r--r--   0 li         (501) staff       (20)        0 2023-03-13 05:42:34.000000 GenBioX-0.3/GenBioX/annotation/ap_qualityCheck.py
--rw-r--r--   0 li         (501) staff       (20)     1270 2023-04-28 11:23:02.000000 GenBioX-0.3/GenBioX/annotation/extract_annotations.py
--rw-r--r--   0 li         (501) staff       (20)      772 2023-04-28 11:23:46.000000 GenBioX-0.3/GenBioX/annotation/filter_annotations.py
--rw-r--r--   0 li         (501) staff       (20)      670 2023-04-28 11:24:17.000000 GenBioX-0.3/GenBioX/annotation/search_annotations.py
--rw-r--r--   0 li         (501) staff       (20)      577 2023-03-13 07:19:41.000000 GenBioX-0.3/GenBioX/annotation/test_annotation.py
--rw-r--r--   0 li         (501) staff       (20)      914 2023-03-13 06:38:01.000000 GenBioX-0.3/GenBioX/annotation/test_annotation_processing.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.049453 GenBioX-0.3/GenBioX/comparative_genomics/
--rw-r--r--   0 li         (501) staff       (20)      226 2023-05-02 09:35:31.000000 GenBioX-0.3/GenBioX/comparative_genomics/__init__.py
--rw-r--r--   0 li         (501) staff       (20)      627 2023-04-28 12:27:36.000000 GenBioX-0.3/GenBioX/comparative_genomics/compare_genome_size.py
--rw-r--r--   0 li         (501) staff       (20)     1003 2023-04-28 12:29:13.000000 GenBioX-0.3/GenBioX/comparative_genomics/identify_conserved_regions.py
--rw-r--r--   0 li         (501) staff       (20)     1091 2023-04-28 12:33:31.000000 GenBioX-0.3/GenBioX/comparative_genomics/pairwise_identity.py
--rw-r--r--   0 li         (501) staff       (20)      865 2023-05-02 09:34:26.000000 GenBioX-0.3/GenBioX/comparative_genomics/phylogenetic_distance.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.051253 GenBioX-0.3/GenBioX/data_preprocessing/
--rw-r--r--   0 li         (501) staff       (20)      498 2023-05-02 09:16:54.000000 GenBioX-0.3/GenBioX/data_preprocessing/__init__.py
--rw-r--r--   0 li         (501) staff       (20)     1269 2023-03-21 11:47:30.000000 GenBioX-0.3/GenBioX/data_preprocessing/extract_annotation.py
--rw-r--r--   0 li         (501) staff       (20)      994 2023-03-12 11:10:50.000000 GenBioX-0.3/GenBioX/data_preprocessing/fasta_quality_check.py
--rw-r--r--   0 li         (501) staff       (20)     1670 2023-03-15 07:48:07.000000 GenBioX-0.3/GenBioX/data_preprocessing/fetch_seq.py
--rw-r--r--   0 li         (501) staff       (20)      735 2023-03-21 12:36:47.000000 GenBioX-0.3/GenBioX/data_preprocessing/filter_contaminants.py
--rw-r--r--   0 li         (501) staff       (20)      819 2023-05-02 09:10:07.000000 GenBioX-0.3/GenBioX/data_preprocessing/filter_low_quality_read.py
--rw-r--r--   0 li         (501) staff       (20)      696 2023-05-02 09:07:31.000000 GenBioX-0.3/GenBioX/data_preprocessing/quality_score.py
--rw-r--r--   0 li         (501) staff       (20)      719 2023-05-01 09:51:28.000000 GenBioX-0.3/GenBioX/data_preprocessing/read_fasta.py
--rw-r--r--   0 li         (501) staff       (20)      516 2023-03-21 12:32:15.000000 GenBioX-0.3/GenBioX/data_preprocessing/remove_duplicates.py
--rw-r--r--   0 li         (501) staff       (20)      492 2023-03-12 11:43:35.000000 GenBioX-0.3/GenBioX/data_preprocessing/test2.py
--rw-r--r--   0 li         (501) staff       (20)      202 2023-03-15 07:46:06.000000 GenBioX-0.3/GenBioX/data_preprocessing/test_fetch_seq.py
--rw-r--r--   0 li         (501) staff       (20)      301 2023-03-15 07:15:50.000000 GenBioX-0.3/GenBioX/data_preprocessing/test_read_fasta.py
--rw-r--r--   0 li         (501) staff       (20)      845 2023-03-21 12:31:53.000000 GenBioX-0.3/GenBioX/data_preprocessing/trim_adapters.py
--rw-r--r--   0 li         (501) staff       (20)      466 2023-03-12 10:13:01.000000 GenBioX-0.3/GenBioX/data_preprocessing/vcf.py
--rw-r--r--   0 li         (501) staff       (20)     1725 2023-03-21 12:38:00.000000 GenBioX-0.3/GenBioX/data_preprocessing/visualise_quality_metrics.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.051858 GenBioX-0.3/GenBioX/gene_expression/
--rw-r--r--   0 li         (501) staff       (20)      306 2023-05-02 09:33:24.000000 GenBioX-0.3/GenBioX/gene_expression/__init__.py
--rw-r--r--   0 li         (501) staff       (20)     2381 2023-04-28 12:15:59.000000 GenBioX-0.3/GenBioX/gene_expression/differential_gene_expression_analysis.py
--rw-r--r--   0 li         (501) staff       (20)      857 2023-04-28 12:19:43.000000 GenBioX-0.3/GenBioX/gene_expression/gene_expression_correlation.py
--rw-r--r--   0 li         (501) staff       (20)      968 2023-04-28 12:13:21.000000 GenBioX-0.3/GenBioX/gene_expression/gene_expression_normalization.py
--rw-r--r--   0 li         (501) staff       (20)      834 2023-04-28 12:18:09.000000 GenBioX-0.3/GenBioX/gene_expression/gene_expression_quantification.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.052478 GenBioX-0.3/GenBioX/statistical_analysis/
--rw-r--r--   0 li         (501) staff       (20)      189 2023-05-02 09:20:21.000000 GenBioX-0.3/GenBioX/statistical_analysis/__init__.py
--rw-r--r--   0 li         (501) staff       (20)      313 2023-03-29 10:45:48.000000 GenBioX-0.3/GenBioX/statistical_analysis/calculate_gc_content.py
--rw-r--r--   0 li         (501) staff       (20)      638 2023-03-29 11:26:06.000000 GenBioX-0.3/GenBioX/statistical_analysis/count_nucleotides.py
--rw-r--r--   0 li         (501) staff       (20)      606 2023-03-29 11:13:34.000000 GenBioX-0.3/GenBioX/statistical_analysis/reverse_complement.py
--rw-r--r--   0 li         (501) staff       (20)      911 2023-03-29 11:07:19.000000 GenBioX-0.3/GenBioX/statistical_analysis/translate.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.053193 GenBioX-0.3/GenBioX/variant_analysis/
--rw-r--r--   0 li         (501) staff       (20)      275 2023-05-02 09:30:22.000000 GenBioX-0.3/GenBioX/variant_analysis/__init__.py
--rw-r--r--   0 li         (501) staff       (20)      993 2023-05-02 09:29:28.000000 GenBioX-0.3/GenBioX/variant_analysis/phenotype_prediction.py
--rw-r--r--   0 li         (501) staff       (20)     1041 2023-04-28 11:57:24.000000 GenBioX-0.3/GenBioX/variant_analysis/splice_site_prediction.py
--rw-r--r--   0 li         (501) staff       (20)      673 2023-04-28 11:53:06.000000 GenBioX-0.3/GenBioX/variant_analysis/variant_annotation.py
--rw-r--r--   0 li         (501) staff       (20)      437 2023-04-28 11:51:00.000000 GenBioX-0.3/GenBioX/variant_analysis/variant_calling.py
--rw-r--r--   0 li         (501) staff       (20)      608 2023-04-28 11:54:44.000000 GenBioX-0.3/GenBioX/variant_analysis/variant_effect_prediction.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-04 03:39:29.047212 GenBioX-0.3/GenBioX.egg-info/
--rw-r--r--   0 li         (501) staff       (20)      940 2023-05-04 03:39:28.000000 GenBioX-0.3/GenBioX.egg-info/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)     2465 2023-05-04 03:39:29.000000 GenBioX-0.3/GenBioX.egg-info/SOURCES.txt
--rw-r--r--   0 li         (501) staff       (20)        1 2023-05-04 03:39:28.000000 GenBioX-0.3/GenBioX.egg-info/dependency_links.txt
--rw-r--r--   0 li         (501) staff       (20)       64 2023-05-04 03:39:28.000000 GenBioX-0.3/GenBioX.egg-info/requires.txt
--rw-r--r--   0 li         (501) staff       (20)        8 2023-05-04 03:39:28.000000 GenBioX-0.3/GenBioX.egg-info/top_level.txt
--rw-r--r--   0 li         (501) staff       (20)     1072 2023-05-03 10:52:48.000000 GenBioX-0.3/LICENSE.txt
--rw-r--r--   0 li         (501) staff       (20)      940 2023-05-04 03:39:29.053374 GenBioX-0.3/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)      134 2023-05-03 10:57:36.000000 GenBioX-0.3/README.md
--rw-r--r--   0 li         (501) staff       (20)       38 2023-05-04 03:39:29.053667 GenBioX-0.3/setup.cfg
--rw-r--r--   0 li         (501) staff       (20)     1231 2023-05-04 03:38:49.000000 GenBioX-0.3/setup.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.248195 GenBioX-0.3.1/
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.232493 GenBioX-0.3.1/GenBioX/
+-rw-r--r--   0 li         (501) staff       (20)        0 2023-03-12 06:16:05.000000 GenBioX-0.3.1/GenBioX/__init__.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.234980 GenBioX-0.3.1/GenBioX/alignment/
+-rw-r--r--   0 li         (501) staff       (20)      298 2023-05-05 08:12:11.000000 GenBioX-0.3.1/GenBioX/alignment/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)      207 2023-05-04 13:31:47.000000 GenBioX-0.3.1/GenBioX/alignment/align.py
+-rw-r--r--   0 li         (501) staff       (20)      720 2023-05-04 13:49:09.000000 GenBioX-0.3.1/GenBioX/alignment/evaluate_alignment_quality.py
+-rw-r--r--   0 li         (501) staff       (20)     1316 2023-05-05 08:40:55.000000 GenBioX-0.3.1/GenBioX/alignment/extract_conserved_regions.py
+-rw-r--r--   0 li         (501) staff       (20)      810 2023-04-28 11:09:16.000000 GenBioX-0.3.1/GenBioX/alignment/merge_alignments.py
+-rw-r--r--   0 li         (501) staff       (20)      583 2023-05-05 08:11:27.000000 GenBioX-0.3.1/GenBioX/alignment/pairwise_alignment.py
+-rw-r--r--   0 li         (501) staff       (20)     1186 2023-05-05 07:32:38.000000 GenBioX-0.3.1/GenBioX/alignment/read_alignment.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.236832 GenBioX-0.3.1/GenBioX/annotation/
+-rw-r--r--   0 li         (501) staff       (20)      261 2023-05-05 10:45:02.000000 GenBioX-0.3.1/GenBioX/annotation/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)     1270 2023-04-28 11:23:02.000000 GenBioX-0.3.1/GenBioX/annotation/extract_annotations.py
+-rw-r--r--   0 li         (501) staff       (20)      474 2023-05-05 10:38:51.000000 GenBioX-0.3.1/GenBioX/annotation/extract_locations.py
+-rw-r--r--   0 li         (501) staff       (20)      264 2023-05-05 09:11:10.000000 GenBioX-0.3.1/GenBioX/annotation/filter_annotations.py
+-rw-r--r--   0 li         (501) staff       (20)      292 2023-05-05 09:08:39.000000 GenBioX-0.3.1/GenBioX/annotation/search_annotations.py
+-rw-r--r--   0 li         (501) staff       (20)     1062 2023-05-05 10:44:34.000000 GenBioX-0.3.1/GenBioX/annotation/visualize_annotations.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.238308 GenBioX-0.3.1/GenBioX/comparative_genomics/
+-rw-r--r--   0 li         (501) staff       (20)      226 2023-05-02 09:35:31.000000 GenBioX-0.3.1/GenBioX/comparative_genomics/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)      627 2023-04-28 12:27:36.000000 GenBioX-0.3.1/GenBioX/comparative_genomics/compare_genome_size.py
+-rw-r--r--   0 li         (501) staff       (20)     1003 2023-04-28 12:29:13.000000 GenBioX-0.3.1/GenBioX/comparative_genomics/identify_conserved_regions.py
+-rw-r--r--   0 li         (501) staff       (20)     1091 2023-04-28 12:33:31.000000 GenBioX-0.3.1/GenBioX/comparative_genomics/pairwise_identity.py
+-rw-r--r--   0 li         (501) staff       (20)      334 2023-05-05 12:13:45.000000 GenBioX-0.3.1/GenBioX/comparative_genomics/phylogenetic_distance.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.242570 GenBioX-0.3.1/GenBioX/data_preprocessing/
+-rw-r--r--   0 li         (501) staff       (20)      498 2023-05-02 09:16:54.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)     1269 2023-03-21 11:47:30.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/extract_annotation.py
+-rw-r--r--   0 li         (501) staff       (20)     1072 2023-05-04 11:48:45.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/fasta_quality_check.py
+-rw-r--r--   0 li         (501) staff       (20)     1670 2023-03-15 07:48:07.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/fetch_seq.py
+-rw-r--r--   0 li         (501) staff       (20)      735 2023-03-21 12:36:47.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/filter_contaminants.py
+-rw-r--r--   0 li         (501) staff       (20)      819 2023-05-02 09:10:07.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/filter_low_quality_read.py
+-rw-r--r--   0 li         (501) staff       (20)      389 2023-05-04 11:47:37.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/quality_score.py
+-rw-r--r--   0 li         (501) staff       (20)      442 2023-05-04 11:36:04.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/read_fasta.py
+-rw-r--r--   0 li         (501) staff       (20)      516 2023-03-21 12:32:15.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/remove_duplicates.py
+-rw-r--r--   0 li         (501) staff       (20)      492 2023-03-12 11:43:35.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/test2.py
+-rw-r--r--   0 li         (501) staff       (20)      202 2023-03-15 07:46:06.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/test_fetch_seq.py
+-rw-r--r--   0 li         (501) staff       (20)      301 2023-03-15 07:15:50.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/test_read_fasta.py
+-rw-r--r--   0 li         (501) staff       (20)      369 2023-05-04 12:06:13.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/trim_adapters.py
+-rw-r--r--   0 li         (501) staff       (20)      466 2023-03-12 10:13:01.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/vcf.py
+-rw-r--r--   0 li         (501) staff       (20)     1725 2023-03-21 12:38:00.000000 GenBioX-0.3.1/GenBioX/data_preprocessing/visualise_quality_metrics.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.244579 GenBioX-0.3.1/GenBioX/gene_expression/
+-rw-r--r--   0 li         (501) staff       (20)      418 2023-05-05 11:46:13.000000 GenBioX-0.3.1/GenBioX/gene_expression/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)     2381 2023-05-05 11:43:41.000000 GenBioX-0.3.1/GenBioX/gene_expression/differential_gene_expression_analysis.py
+-rw-r--r--   0 li         (501) staff       (20)      857 2023-04-28 12:19:43.000000 GenBioX-0.3.1/GenBioX/gene_expression/gene_expression_correlation.py
+-rw-r--r--   0 li         (501) staff       (20)      968 2023-05-05 11:24:32.000000 GenBioX-0.3.1/GenBioX/gene_expression/gene_expression_normalization.py
+-rw-r--r--   0 li         (501) staff       (20)      834 2023-04-28 12:18:09.000000 GenBioX-0.3.1/GenBioX/gene_expression/gene_expression_quantification.py
+-rw-r--r--   0 li         (501) staff       (20)     1121 2023-05-05 11:45:43.000000 GenBioX-0.3.1/GenBioX/gene_expression/get_group_labels.py
+-rw-r--r--   0 li         (501) staff       (20)      633 2023-05-05 11:17:30.000000 GenBioX-0.3.1/GenBioX/gene_expression/read_gene_expression_file.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.245926 GenBioX-0.3.1/GenBioX/statistical_analysis/
+-rw-r--r--   0 li         (501) staff       (20)      189 2023-05-02 09:20:21.000000 GenBioX-0.3.1/GenBioX/statistical_analysis/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)      313 2023-03-29 10:45:48.000000 GenBioX-0.3.1/GenBioX/statistical_analysis/calculate_gc_content.py
+-rw-r--r--   0 li         (501) staff       (20)      254 2023-05-04 13:10:07.000000 GenBioX-0.3.1/GenBioX/statistical_analysis/count_nucleotides.py
+-rw-r--r--   0 li         (501) staff       (20)      606 2023-03-29 11:13:34.000000 GenBioX-0.3.1/GenBioX/statistical_analysis/reverse_complement.py
+-rw-r--r--   0 li         (501) staff       (20)      312 2023-05-04 13:00:35.000000 GenBioX-0.3.1/GenBioX/statistical_analysis/translate.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.247583 GenBioX-0.3.1/GenBioX/variant_analysis/
+-rw-r--r--   0 li         (501) staff       (20)      275 2023-05-02 09:30:22.000000 GenBioX-0.3.1/GenBioX/variant_analysis/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)      993 2023-05-02 09:29:28.000000 GenBioX-0.3.1/GenBioX/variant_analysis/phenotype_prediction.py
+-rw-r--r--   0 li         (501) staff       (20)     1041 2023-04-28 11:57:24.000000 GenBioX-0.3.1/GenBioX/variant_analysis/splice_site_prediction.py
+-rw-r--r--   0 li         (501) staff       (20)      673 2023-04-28 11:53:06.000000 GenBioX-0.3.1/GenBioX/variant_analysis/variant_annotation.py
+-rw-r--r--   0 li         (501) staff       (20)      437 2023-04-28 11:51:00.000000 GenBioX-0.3.1/GenBioX/variant_analysis/variant_calling.py
+-rw-r--r--   0 li         (501) staff       (20)      608 2023-04-28 11:54:44.000000 GenBioX-0.3.1/GenBioX/variant_analysis/variant_effect_prediction.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-05 13:32:40.233068 GenBioX-0.3.1/GenBioX.egg-info/
+-rw-r--r--   0 li         (501) staff       (20)      942 2023-05-05 13:32:40.000000 GenBioX-0.3.1/GenBioX.egg-info/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)     2528 2023-05-05 13:32:40.000000 GenBioX-0.3.1/GenBioX.egg-info/SOURCES.txt
+-rw-r--r--   0 li         (501) staff       (20)        1 2023-05-05 13:32:40.000000 GenBioX-0.3.1/GenBioX.egg-info/dependency_links.txt
+-rw-r--r--   0 li         (501) staff       (20)       64 2023-05-05 13:32:40.000000 GenBioX-0.3.1/GenBioX.egg-info/requires.txt
+-rw-r--r--   0 li         (501) staff       (20)        8 2023-05-05 13:32:40.000000 GenBioX-0.3.1/GenBioX.egg-info/top_level.txt
+-rw-r--r--   0 li         (501) staff       (20)     1072 2023-05-03 10:52:48.000000 GenBioX-0.3.1/LICENSE.txt
+-rw-r--r--   0 li         (501) staff       (20)      942 2023-05-05 13:32:40.247918 GenBioX-0.3.1/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)      134 2023-05-03 10:57:36.000000 GenBioX-0.3.1/README.md
+-rw-r--r--   0 li         (501) staff       (20)       38 2023-05-05 13:32:40.248242 GenBioX-0.3.1/setup.cfg
+-rw-r--r--   0 li         (501) staff       (20)     1233 2023-05-05 13:19:11.000000 GenBioX-0.3.1/setup.py
```

### Comparing `GenBioX-0.3/GenBioX/alignment/evaluate_alignment_quality.py` & `GenBioX-0.3.1/GenBioX/alignment/evaluate_alignment_quality.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/alignment/extract_conserved_regions.py` & `GenBioX-0.3.1/GenBioX/alignment/extract_conserved_regions.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/alignment/merge_alignments.py` & `GenBioX-0.3.1/GenBioX/alignment/merge_alignments.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/annotation/extract_annotations.py` & `GenBioX-0.3.1/GenBioX/annotation/extract_annotations.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/comparative_genomics/compare_genome_size.py` & `GenBioX-0.3.1/GenBioX/comparative_genomics/compare_genome_size.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/comparative_genomics/identify_conserved_regions.py` & `GenBioX-0.3.1/GenBioX/comparative_genomics/identify_conserved_regions.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/comparative_genomics/pairwise_identity.py` & `GenBioX-0.3.1/GenBioX/comparative_genomics/pairwise_identity.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/data_preprocessing/extract_annotation.py` & `GenBioX-0.3.1/GenBioX/data_preprocessing/extract_annotation.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/data_preprocessing/fetch_seq.py` & `GenBioX-0.3.1/GenBioX/data_preprocessing/fetch_seq.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/data_preprocessing/filter_contaminants.py` & `GenBioX-0.3.1/GenBioX/data_preprocessing/filter_contaminants.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/data_preprocessing/filter_low_quality_read.py` & `GenBioX-0.3.1/GenBioX/data_preprocessing/filter_low_quality_read.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/data_preprocessing/remove_duplicates.py` & `GenBioX-0.3.1/GenBioX/data_preprocessing/remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/data_preprocessing/visualise_quality_metrics.py` & `GenBioX-0.3.1/GenBioX/data_preprocessing/visualise_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/gene_expression/differential_gene_expression_analysis.py` & `GenBioX-0.3.1/GenBioX/gene_expression/differential_gene_expression_analysis.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/gene_expression/gene_expression_correlation.py` & `GenBioX-0.3.1/GenBioX/gene_expression/gene_expression_correlation.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/gene_expression/gene_expression_normalization.py` & `GenBioX-0.3.1/GenBioX/gene_expression/gene_expression_normalization.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/gene_expression/gene_expression_quantification.py` & `GenBioX-0.3.1/GenBioX/gene_expression/gene_expression_quantification.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/statistical_analysis/reverse_complement.py` & `GenBioX-0.3.1/GenBioX/statistical_analysis/reverse_complement.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/variant_analysis/phenotype_prediction.py` & `GenBioX-0.3.1/GenBioX/variant_analysis/phenotype_prediction.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/variant_analysis/splice_site_prediction.py` & `GenBioX-0.3.1/GenBioX/variant_analysis/splice_site_prediction.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/variant_analysis/variant_annotation.py` & `GenBioX-0.3.1/GenBioX/variant_analysis/variant_annotation.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX/variant_analysis/variant_effect_prediction.py` & `GenBioX-0.3.1/GenBioX/variant_analysis/variant_effect_prediction.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/GenBioX.egg-info/PKG-INFO` & `GenBioX-0.3.1/GenBioX.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenBioX
-Version: 0.3
+Version: 0.3.1
 Summary: A Comprehensive Bioinformatics Package for Genome Analysis
 Home-page: https://github.com/SayaGarud/GenBioX.git
 Author: Sayali Garud
 Author-email: sayaligrud@gmail.com
 License: MIT
 Keywords: bioinformatics,genomics,genome analysis,quality control,preprocessing,sequencing,annotation,variant analysis,gene expression,comparative genomics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `GenBioX-0.3/GenBioX.egg-info/SOURCES.txt` & `GenBioX-0.3.1/GenBioX.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 GenBioX.egg-info/requires.txt
 GenBioX.egg-info/top_level.txt
 GenBioX/alignment/__init__.py
 GenBioX/alignment/align.py
 GenBioX/alignment/evaluate_alignment_quality.py
 GenBioX/alignment/extract_conserved_regions.py
 GenBioX/alignment/merge_alignments.py
+GenBioX/alignment/pairwise_alignment.py
 GenBioX/alignment/read_alignment.py
 GenBioX/annotation/__init__.py
-GenBioX/annotation/annotation.py
-GenBioX/annotation/ap_qualityCheck.py
 GenBioX/annotation/extract_annotations.py
+GenBioX/annotation/extract_locations.py
 GenBioX/annotation/filter_annotations.py
 GenBioX/annotation/search_annotations.py
-GenBioX/annotation/test_annotation.py
-GenBioX/annotation/test_annotation_processing.py
+GenBioX/annotation/visualize_annotations.py
 GenBioX/comparative_genomics/__init__.py
 GenBioX/comparative_genomics/compare_genome_size.py
 GenBioX/comparative_genomics/identify_conserved_regions.py
 GenBioX/comparative_genomics/pairwise_identity.py
 GenBioX/comparative_genomics/phylogenetic_distance.py
 GenBioX/data_preprocessing/__init__.py
 GenBioX/data_preprocessing/extract_annotation.py
@@ -42,14 +41,16 @@
 GenBioX/data_preprocessing/vcf.py
 GenBioX/data_preprocessing/visualise_quality_metrics.py
 GenBioX/gene_expression/__init__.py
 GenBioX/gene_expression/differential_gene_expression_analysis.py
 GenBioX/gene_expression/gene_expression_correlation.py
 GenBioX/gene_expression/gene_expression_normalization.py
 GenBioX/gene_expression/gene_expression_quantification.py
+GenBioX/gene_expression/get_group_labels.py
+GenBioX/gene_expression/read_gene_expression_file.py
 GenBioX/statistical_analysis/__init__.py
 GenBioX/statistical_analysis/calculate_gc_content.py
 GenBioX/statistical_analysis/count_nucleotides.py
 GenBioX/statistical_analysis/reverse_complement.py
 GenBioX/statistical_analysis/translate.py
 GenBioX/variant_analysis/__init__.py
 GenBioX/variant_analysis/phenotype_prediction.py
```

### Comparing `GenBioX-0.3/LICENSE.txt` & `GenBioX-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GenBioX-0.3/PKG-INFO` & `GenBioX-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenBioX
-Version: 0.3
+Version: 0.3.1
 Summary: A Comprehensive Bioinformatics Package for Genome Analysis
 Home-page: https://github.com/SayaGarud/GenBioX.git
 Author: Sayali Garud
 Author-email: sayaligrud@gmail.com
 License: MIT
 Keywords: bioinformatics,genomics,genome analysis,quality control,preprocessing,sequencing,annotation,variant analysis,gene expression,comparative genomics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `GenBioX-0.3/setup.py` & `GenBioX-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GenBioX',
-    version='0.3',
+    version='0.3.1',
     packages=find_packages(),
     license='MIT',
     description='A Comprehensive Bioinformatics Package for Genome Analysis',
     long_description='''For documentation, please visit http://genbiox.readthedocs.io/''',
     keywords=['bioinformatics', 'genomics', 'genome analysis', 'quality control', 'preprocessing',  'sequencing', 'annotation','variant analysis', 'gene expression', 'comparative genomics'],
     install_requires=[
         'pandas>=1.3.0',
```

