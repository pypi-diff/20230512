# Comparing `tmp/ontogpt-0.2.4.tar.gz` & `tmp/ontogpt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontogpt-0.2.4.tar", max compression
+gzip compressed data, was "ontogpt-0.2.5.tar", max compression
```

## Comparing `ontogpt-0.2.4.tar` & `ontogpt-0.2.5.tar`

### file list

```diff
@@ -1,107 +1,110 @@
--rw-r--r--   0        0        0     1485 2023-05-04 00:13:25.772353 ontogpt-0.2.4/LICENSE
--rw-r--r--   0        0        0    11172 2023-05-04 00:13:25.772353 ontogpt-0.2.4/README.md
--rw-r--r--   0        0        0     2356 2023-05-04 00:14:29.715690 ontogpt-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/__init__.py
--rw-r--r--   0        0        0    32662 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/cli.py
--rw-r--r--   0        0        0      244 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/__init__.py
--rw-r--r--   0        0        0     6962 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/openai_client.py
--rw-r--r--   0        0        0     2921 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/pubmed_client.py
--rw-r--r--   0        0        0      617 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/soup_client.py
--rw-r--r--   0        0        0     1122 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/wikipedia_client.py
--rw-r--r--   0        0        0      684 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/conf/synonymizer-conf.yaml
--rw-r--r--   0        0        0       81 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/converters/__init__.py
--rw-r--r--   0        0        0     5289 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/converters/ontology_converter.py
--rw-r--r--   0        0        0       59 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/__init__.py
--rw-r--r--   0        0        0     3748 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/embedding_similarity_engine.py
--rw-r--r--   0        0        0    12334 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/enrichment.py
--rw-r--r--   0        0        0    19185 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/halo_engine.py
--rw-r--r--   0        0        0    24067 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/knowledge_engine.py
--rw-r--r--   0        0        0      752 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/resolver.py
--rw-r--r--   0        0        0    18520 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/spires_engine.py
--rw-r--r--   0        0        0      719 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/synonym_engine.py
--rw-r--r--   0        0        0       70 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/__init__.py
--rw-r--r--   0        0        0   425228 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
--rw-r--r--   0        0        0   409439 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
--rw-r--r--   0        0        0   413985 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/synonyms.yaml
--rw-r--r--   0        0        0    10390 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/eval_ctd.py
--rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/__init__.py
--rw-r--r--   0        0        0     2145 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
--rw-r--r--   0        0        0     2027 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
--rw-r--r--   0        0        0    10670 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
--rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/enrichment/__init__.py
--rw-r--r--   0        0        0    13679 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/enrichment/eval_enrichment.py
--rw-r--r--   0        0        0     2950 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/evaluation_engine.py
--rw-r--r--   0        0        0     6164 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/go/eval_go.py
--rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/hpoa/__init__.py
--rw-r--r--   0        0        0     8973 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/hpoa/eval_hpoa.py
--rw-r--r--   0        0        0     1191 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
--rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
--rw-r--r--   0        0        0     4791 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
--rwxr-xr-x   0        0        0       95 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/run.sh
--rwxr-xr-x   0        0        0       99 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/run.sh~
--rw-r--r--   0        0        0      586 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/resolver.py
--rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/__init__.py
--rw-r--r--   0        0        0      386 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/exporter.py
--rw-r--r--   0        0        0     4329 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/html_exporter.py
--rw-r--r--   0        0        0     3255 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/markdown_exporter.py
--rw-r--r--   0        0        0     2350 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/owl_exporter.py
--rw-r--r--   0        0        0     1440 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/rdf_exporter.py
--rw-r--r--   0        0        0      899 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/yaml_wrapper.py
--rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/__init__.py
--rw-r--r--   0        0        0      159 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
--rw-r--r--   0        0        0     1016 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
--rw-r--r--   0        0        0      993 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
--rw-r--r--   0        0        0      994 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
--rw-r--r--   0        0        0      995 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
--rw-r--r--   0        0        0      560 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/similarity/connections.jinja2
--rw-r--r--   0        0        0       68 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/__init__.py
--rw-r--r--   0        0        0      401 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/all.yaml
--rw-r--r--   0        0        0     5942 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/biological_process.py
--rw-r--r--   0        0        0     2027 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/biological_process.yaml
--rw-r--r--   0        0        0     2938 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/class_enrichment.yaml
--rw-r--r--   0        0        0     3593 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/core.py
--rw-r--r--   0        0        0     3098 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/core.yaml
--rw-r--r--   0        0        0     6210 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/ctd.py
--rw-r--r--   0        0        0     6683 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/ctd.yaml
--rw-r--r--   0        0        0     5466 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/drug.py
--rw-r--r--   0        0        0     1856 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/drug.yaml
--rw-r--r--   0        0        0     6092 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/environmental_sample.py
--rw-r--r--   0        0        0     2880 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/environmental_sample.yaml
--rw-r--r--   0        0        0     4709 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/gene_description_term.py
--rw-r--r--   0        0        0     1614 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/gene_description_term.yaml
--rw-r--r--   0        0        0     8172 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/gocam.py
--rw-r--r--   0        0        0     4871 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/gocam.yaml
--rw-r--r--   0        0        0     6813 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/halo.py
--rw-r--r--   0        0        0     2367 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/halo.yaml
--rw-r--r--   0        0        0     8165 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ibd.py
--rw-r--r--   0        0        0     4869 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ibd.yaml
--rw-r--r--   0        0        0     6097 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/mendelian_disease.py
--rw-r--r--   0        0        0     3130 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/mendelian_disease.yaml
--rw-r--r--   0        0        0     5384 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/metabolic_process.py
--rw-r--r--   0        0        0     1633 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/metabolic_process.yaml
--rw-r--r--   0        0        0     7156 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/metagenome_study.py
--rw-r--r--   0        0        0     3910 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/metagenome_study.yaml
--rw-r--r--   0        0        0     5072 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ontology_class.py
--rw-r--r--   0        0        0     2686 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ontology_class.yaml
--rw-r--r--   0        0        0     6136 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ontology_issue.py
--rw-r--r--   0        0        0     3383 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ontology_issue.yaml
--rw-r--r--   0        0        0     4887 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/phenotype.py
--rw-r--r--   0        0        0     1532 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/phenotype.yaml
--rw-r--r--   0        0        0     7501 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/reaction.py
--rw-r--r--   0        0        0     3187 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/reaction.yaml
--rw-r--r--   0        0        0     7222 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/recipe.py
--rw-r--r--   0        0        0     5792 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/recipe.yaml
--rw-r--r--   0        0        0     7847 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/treatment.py
--rw-r--r--   0        0        0     4485 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/treatment.yaml
--rw-r--r--   0        0        0        0 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/utils/__init__.py
--rw-r--r--   0        0        0     7510 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/utils/gene_set_utils.py
--rw-r--r--   0        0        0        0 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/__init__.py
--rw-r--r--   0        0        0      861 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/html/form.html
--rw-r--r--   0        0        0      201 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/html/results.html
--rw-r--r--   0        0        0      819 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/html/spindoctor/form.html
--rw-r--r--   0        0        0      205 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/html/spindoctor/results.html
--rw-r--r--   0        0        0     2722 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/main.py
--rw-r--r--   0        0        0    13469 1970-01-01 00:00:00.000000 ontogpt-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-05-12 21:38:29.111857 ontogpt-0.2.5/LICENSE
+-rw-r--r--   0        0        0    11651 2023-05-12 21:38:29.111857 ontogpt-0.2.5/README.md
+-rw-r--r--   0        0        0     2356 2023-05-12 21:39:44.607110 ontogpt-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/__init__.py
+-rw-r--r--   0        0        0    32676 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/cli.py
+-rw-r--r--   0        0        0      244 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/__init__.py
+-rw-r--r--   0        0        0     6962 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/openai_client.py
+-rw-r--r--   0        0        0     2921 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/pubmed_client.py
+-rw-r--r--   0        0        0      617 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/soup_client.py
+-rw-r--r--   0        0        0     1122 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/wikipedia_client.py
+-rw-r--r--   0        0        0      684 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/conf/synonymizer-conf.yaml
+-rw-r--r--   0        0        0       81 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/converters/__init__.py
+-rw-r--r--   0        0        0     5289 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/converters/ontology_converter.py
+-rw-r--r--   0        0        0       59 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/__init__.py
+-rw-r--r--   0        0        0     3748 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/embedding_similarity_engine.py
+-rw-r--r--   0        0        0    12456 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/enrichment.py
+-rw-r--r--   0        0        0    19185 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/halo_engine.py
+-rw-r--r--   0        0        0    24102 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/knowledge_engine.py
+-rw-r--r--   0        0        0      752 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/resolver.py
+-rw-r--r--   0        0        0    18520 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/spires_engine.py
+-rw-r--r--   0        0        0      719 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/synonym_engine.py
+-rw-r--r--   0        0        0       70 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/__init__.py
+-rw-r--r--   0        0        0   425228 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
+-rw-r--r--   0        0        0   409439 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
+-rw-r--r--   0        0        0   413985 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/synonyms.yaml
+-rw-r--r--   0        0        0    10390 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/eval_ctd.py
+-rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
+-rw-r--r--   0        0        0     2027 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
+-rw-r--r--   0        0        0    10670 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
+-rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/enrichment/__init__.py
+-rw-r--r--   0        0        0    13705 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/enrichment/eval_enrichment.py
+-rw-r--r--   0        0        0     2950 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/evaluation_engine.py
+-rw-r--r--   0        0        0     6164 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/go/eval_go.py
+-rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/hpoa/__init__.py
+-rw-r--r--   0        0        0     8973 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/hpoa/eval_hpoa.py
+-rw-r--r--   0        0        0     1191 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
+-rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
+-rw-r--r--   0        0        0     4791 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
+-rwxr-xr-x   0        0        0       95 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/run.sh
+-rwxr-xr-x   0        0        0       99 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/run.sh~
+-rw-r--r--   0        0        0      586 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/resolver.py
+-rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/exporter.py
+-rw-r--r--   0        0        0     4329 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/html_exporter.py
+-rw-r--r--   0        0        0     3255 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/markdown_exporter.py
+-rw-r--r--   0        0        0     2350 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/owl_exporter.py
+-rw-r--r--   0        0        0     1440 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/rdf_exporter.py
+-rw-r--r--   0        0        0      899 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/yaml_wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
+-rw-r--r--   0        0        0     1016 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
+-rw-r--r--   0        0        0      993 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
+-rw-r--r--   0        0        0      994 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
+-rw-r--r--   0        0        0      995 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
+-rw-r--r--   0        0        0      560 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/similarity/connections.jinja2
+-rw-r--r--   0        0        0       68 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/templates/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/templates/all.yaml
+-rw-r--r--   0        0        0     5942 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/biological_process.py
+-rw-r--r--   0        0        0     2027 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/biological_process.yaml
+-rw-r--r--   0        0        0     2938 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/class_enrichment.yaml
+-rw-r--r--   0        0        0     4519 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/composite_disease.yaml
+-rw-r--r--   0        0        0     3593 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/core.py
+-rw-r--r--   0        0        0     3098 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/core.yaml
+-rw-r--r--   0        0        0     6210 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ctd.py
+-rw-r--r--   0        0        0     6683 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ctd.yaml
+-rw-r--r--   0        0        0     8825 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/diagnostic_procedure.py
+-rw-r--r--   0        0        0     4774 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/diagnostic_procedure.yaml
+-rw-r--r--   0        0        0     5466 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/drug.py
+-rw-r--r--   0        0        0     1856 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/drug.yaml
+-rw-r--r--   0        0        0     6092 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/environmental_sample.py
+-rw-r--r--   0        0        0     2880 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/environmental_sample.yaml
+-rw-r--r--   0        0        0     4709 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/gene_description_term.py
+-rw-r--r--   0        0        0     1614 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/gene_description_term.yaml
+-rw-r--r--   0        0        0     8172 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/gocam.py
+-rw-r--r--   0        0        0     4871 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/gocam.yaml
+-rw-r--r--   0        0        0     6813 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/halo.py
+-rw-r--r--   0        0        0     2367 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/halo.yaml
+-rw-r--r--   0        0        0     8165 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ibd.py
+-rw-r--r--   0        0        0     4869 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ibd.yaml
+-rw-r--r--   0        0        0     6097 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/mendelian_disease.py
+-rw-r--r--   0        0        0     3130 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/mendelian_disease.yaml
+-rw-r--r--   0        0        0     5384 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/metabolic_process.py
+-rw-r--r--   0        0        0     1633 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/metabolic_process.yaml
+-rw-r--r--   0        0        0     7156 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/metagenome_study.py
+-rw-r--r--   0        0        0     3910 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/metagenome_study.yaml
+-rw-r--r--   0        0        0     5072 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ontology_class.py
+-rw-r--r--   0        0        0     2686 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ontology_class.yaml
+-rw-r--r--   0        0        0     6136 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ontology_issue.py
+-rw-r--r--   0        0        0     3383 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ontology_issue.yaml
+-rw-r--r--   0        0        0     4887 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/phenotype.py
+-rw-r--r--   0        0        0     1532 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/phenotype.yaml
+-rw-r--r--   0        0        0     7501 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/reaction.py
+-rw-r--r--   0        0        0     3187 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/reaction.yaml
+-rw-r--r--   0        0        0     7222 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/recipe.py
+-rw-r--r--   0        0        0     5792 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/recipe.yaml
+-rw-r--r--   0        0        0     7847 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/treatment.py
+-rw-r--r--   0        0        0     4485 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/treatment.yaml
+-rw-r--r--   0        0        0        0 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/utils/__init__.py
+-rw-r--r--   0        0        0     8788 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/utils/gene_set_utils.py
+-rw-r--r--   0        0        0        0 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/__init__.py
+-rw-r--r--   0        0        0      861 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/html/form.html
+-rw-r--r--   0        0        0      201 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/html/results.html
+-rw-r--r--   0        0        0      819 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/html/spindoctor/form.html
+-rw-r--r--   0        0        0      205 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/html/spindoctor/results.html
+-rw-r--r--   0        0        0     2767 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/main.py
+-rw-r--r--   0        0        0    13948 1970-01-01 00:00:00.000000 ontogpt-0.2.5/PKG-INFO
```

### Comparing `ontogpt-0.2.4/LICENSE` & `ontogpt-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/README.md` & `ontogpt-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![DOI](https://zenodo.org/badge/13996/monarch-initiative/ontogpt.svg)](https://zenodo.org/badge/latestdoi/13996/monarch-initiative/ontogpt)
+
 # OntoGPT
 
 Generation of Ontologies and Knowledge Bases using GPT
 
 A knowledge extraction tool that uses a large language model to extract semantic information from text.
 
 This makes use of so-called *instruction prompts* in Large Language Models (LLMs) such as GPT-4.
@@ -196,15 +198,22 @@
 
 ```
 ontogpt extract -t mendelian_disease.MendelianDisease -i marfan-wikipedia.txt
 ```
 
 ## Web Application
 
-There is a bare bones web application
+There is a bare bones web application for running OntoGPT and viewing results.
+
+Install the required dependencies first with the following command:
+```
+poetry install -E web
+```
+
+Then run the following command to start the web application:
 
 ```
 poetry run web-ontogpt
 ```
 
 Note that the agent running uvicorn must have the API key set, so for obvious reasons
 don't host this publicly without authentication, unless you want your credits drained.
@@ -338,27 +347,25 @@
 
 
 ## Gene Enrichment using SPINDOCTOR
 
 Given a set of genes, OntoGPT can find similarities among them.
 
 Example:
+
 ```
-ontogpt  enrichment -r sqlite:obo:hgnc  -U tests/input/genesets/sensory-ataxia.yaml
+ontogpt  enrichment -U tests/input/genesets/sensory-ataxia.yaml
 ```
 
-This gives both a narrative summary:
-
-__
+The default is to use ontological gene function synopses (via the Alliance API).
 
-and structured term list:
+To use narrative/RefSeq summaries, use the `--no-ontological-synopses` flag.
 
-```
+To run without any gene descriptions, use the `--no-annotations` flag.
 
-```
 
 ## OntoGPT Limitations
 
 ### Non-deterministic
 
 This relies on an existing LLM, and LLMs can be fickle in their responses.
```

### Comparing `ontogpt-0.2.4/pyproject.toml` & `ontogpt-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontogpt"
-version = "0.2.4"
+version = "0.2.5"
 description = "OntoGPT"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 license = "BSD-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `ontogpt-0.2.4/src/ontogpt/cli.py` & `ontogpt-0.2.5/src/ontogpt/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,19 +580,19 @@
 
     Limitations:
 
     It is very easy to exceed the max token length; resolved in GPT-4?
 
     Usage:
 
-        ontogpt enrichment -r sqlite:obo:hgnc -U tests/input/human-genes.txt
+        ontogpt enrichment -r sqlite:obo:hgnc -U tests/input/genesets/dopamine.yaml
 
     Usage:
 
-        ontogpt enrichment -r sqlite:obo:hgnc -U tests/input/human-genes.txt
+        ontogpt enrichment -r sqlite:obo:hgnc -U tests/input/genesets/dopamine.yaml
 
     """
     if not genes and not input_file:
         raise ValueError("Either genes or input file must be passed")
     if genes:
         gene_set = GeneSet(name="TEMP", gene_symbols=genes)
     if input_file:
```

### Comparing `ontogpt-0.2.4/src/ontogpt/clients/openai_client.py` & `ontogpt-0.2.5/src/ontogpt/clients/openai_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/clients/pubmed_client.py` & `ontogpt-0.2.5/src/ontogpt/clients/pubmed_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/clients/soup_client.py` & `ontogpt-0.2.5/src/ontogpt/clients/soup_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/clients/wikipedia_client.py` & `ontogpt-0.2.5/src/ontogpt/clients/wikipedia_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/conf/synonymizer-conf.yaml` & `ontogpt-0.2.5/src/ontogpt/conf/synonymizer-conf.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/converters/ontology_converter.py` & `ontogpt-0.2.5/src/ontogpt/converters/ontology_converter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/engines/embedding_similarity_engine.py` & `ontogpt-0.2.5/src/ontogpt/engines/embedding_similarity_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/engines/enrichment.py` & `ontogpt-0.2.5/src/ontogpt/engines/enrichment.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 from jinja2 import Template
 from oaklib import BasicOntologyInterface, get_adapter
 from pydantic import BaseModel
 
-from ontogpt.engines.knowledge_engine import KnowledgeEngine
+from ontogpt.engines.knowledge_engine import KnowledgeEngine, MODEL_GPT_4
 from ontogpt.prompts.enrichment import DEFAULT_ENRICHMENT_PROMPT
 from ontogpt.templates.class_enrichment import ClassEnrichmentResult
 from ontogpt.templates.gene_description_term import GeneDescriptionTerm
 from ontogpt.utils.gene_set_utils import (
     ENTITY_ID,
     GENE_TUPLE,
     GeneSet,
@@ -244,15 +244,18 @@
             ENRICHED_TERMS_KEYWORD=ENRICHED_TERMS_KEYWORD,
             END_MARKER=self.end_marker,
         )
         logging.debug(f"Prompt from template: {prompt}")
         logging.info(f"Prompt [{truncation_factor}] Length: {len(prompt)}")
         # https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them
         prompt_length = len(self.encoding.encode(prompt)) + 10
-        max_len = 4097 - self.completion_length
+        max_len_total = 4097
+        if self.model == MODEL_GPT_4:
+            max_len_total = 8193
+        max_len = max_len_total - self.completion_length
         logging.info(
             f"Prompt [{truncation_factor}] Toks: {prompt_length} / {max_len} Str={len(prompt)}"
         )
         if prompt_length > max_len:  # TODO: check this
             logging.warning(f"Prompt is too long; toks: {prompt_length} len: {len(prompt)}")
             return self._prompt_from_template(
                 genes,
```

### Comparing `ontogpt-0.2.4/src/ontogpt/engines/halo_engine.py` & `ontogpt-0.2.5/src/ontogpt/engines/halo_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/engines/knowledge_engine.py` & `ontogpt-0.2.5/src/ontogpt/engines/knowledge_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 ANNOTATION_KEY_PROMPT_SKIP = "prompt.skip"
 ANNOTATION_KEY_ANNOTATORS = "annotators"
 ANNOTATION_KEY_RECURSE = "ner.recurse"
 ANNOTATION_KEY_EXAMPLES = "prompt.examples"
 
 MODEL_GPT_3_5_TURBO = "gpt-3.5-turbo"
 MODEL_TEXT_DAVINCI_003 = "text-davinci-003"
-MODELS = [MODEL_GPT_3_5_TURBO, MODEL_TEXT_DAVINCI_003]
+MODEL_GPT_4 = "gpt-4"
+MODELS = [MODEL_GPT_3_5_TURBO, MODEL_TEXT_DAVINCI_003, MODEL_GPT_4]
 
 DEFAULT_MODEL = MODEL_GPT_3_5_TURBO
 
 # TODO: introspect
 DATAMODELS = [
     "treatment.DiseaseTreatmentSummary",
     "gocam.GoCamAnnotations",
```

### Comparing `ontogpt-0.2.4/src/ontogpt/engines/resolver.py` & `ontogpt-0.2.5/src/ontogpt/engines/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/engines/spires_engine.py` & `ontogpt-0.2.5/src/ontogpt/engines/spires_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/engines/synonym_engine.py` & `ontogpt-0.2.5/src/ontogpt/engines/synonym_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz` & `ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz` & `ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/synonyms.yaml` & `ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/synonyms.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/ctd/eval_ctd.py` & `ontogpt-0.2.5/src/ontogpt/evaluation/ctd/eval_ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py` & `ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml` & `ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py` & `ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/enrichment/eval_enrichment.py` & `ontogpt-0.2.5/src/ontogpt/evaluation/enrichment/eval_enrichment.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.parsers.association_parser_factory import get_association_parser
 from pydantic import BaseModel
 from tiktoken import Encoding
 
 from ontogpt.engines import create_engine
 from ontogpt.engines.enrichment import ENTITY_ID, EnrichmentEngine, EnrichmentPayload
-from ontogpt.engines.knowledge_engine import MODEL_GPT_3_5_TURBO, MODEL_NAME, MODEL_TEXT_DAVINCI_003
+from ontogpt.engines.knowledge_engine import MODEL_GPT_3_5_TURBO, MODEL_NAME, MODEL_TEXT_DAVINCI_003, MODEL_GPT_4
 from ontogpt.evaluation.evaluation_engine import EvaluationEngine
 from ontogpt.templates.class_enrichment import ClassEnrichmentResult
 from ontogpt.utils.gene_set_utils import SYMBOL, GeneSet, drop_genes_from_gene_set, gene_info
 
 THIS_DIR = Path(__file__).parent
 DATABASE_DIR = Path(__file__).parent / "database"
 
@@ -38,15 +38,15 @@
 NO_SYNOPSIS = "no_synopsis"
 STANDARD = "standard"
 STANDARD_NO_ONTOLOGY = "standard_no_ontology"
 RANDOM = "random"
 RANK_BASED = "rank_based"
 CLOSURE = "closure"
 
-ENRICHMENT_MODELS = [MODEL_GPT_3_5_TURBO, MODEL_TEXT_DAVINCI_003]
+ENRICHMENT_MODELS = [MODEL_GPT_4, MODEL_GPT_3_5_TURBO, MODEL_TEXT_DAVINCI_003]
 
 
 logger = logging.getLogger(__name__)
 
 
 class Overlap(BaseModel):
     """Overlap between two sets."""
```

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/evaluation_engine.py` & `ontogpt-0.2.5/src/ontogpt/evaluation/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/go/eval_go.py` & `ontogpt-0.2.5/src/ontogpt/evaluation/go/eval_go.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/hpoa/eval_hpoa.py` & `ontogpt-0.2.5/src/ontogpt/evaluation/hpoa/eval_hpoa.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt` & `ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml` & `ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/evaluation/resolver.py` & `ontogpt-0.2.5/src/ontogpt/evaluation/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/io/html_exporter.py` & `ontogpt-0.2.5/src/ontogpt/io/html_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/io/markdown_exporter.py` & `ontogpt-0.2.5/src/ontogpt/io/markdown_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/io/owl_exporter.py` & `ontogpt-0.2.5/src/ontogpt/io/owl_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/io/rdf_exporter.py` & `ontogpt-0.2.5/src/ontogpt/io/rdf_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/io/yaml_wrapper.py` & `ontogpt-0.2.5/src/ontogpt/io/yaml_wrapper.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2` & `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2` & `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2` & `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2` & `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2` & `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/prompts/similarity/connections.jinja2` & `ontogpt-0.2.5/src/ontogpt/prompts/similarity/connections.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/biological_process.py` & `ontogpt-0.2.5/src/ontogpt/templates/biological_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/biological_process.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/biological_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/class_enrichment.py` & `ontogpt-0.2.5/src/ontogpt/templates/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/class_enrichment.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/core.py` & `ontogpt-0.2.5/src/ontogpt/templates/core.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/core.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/core.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/ctd.py` & `ontogpt-0.2.5/src/ontogpt/templates/ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/ctd.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/ctd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/drug.py` & `ontogpt-0.2.5/src/ontogpt/templates/drug.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/drug.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/drug.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/environmental_sample.py` & `ontogpt-0.2.5/src/ontogpt/templates/environmental_sample.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/environmental_sample.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/environmental_sample.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/gene_description_term.py` & `ontogpt-0.2.5/src/ontogpt/templates/gene_description_term.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/gene_description_term.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/gene_description_term.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/gocam.py` & `ontogpt-0.2.5/src/ontogpt/templates/gocam.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/gocam.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/gocam.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/halo.py` & `ontogpt-0.2.5/src/ontogpt/templates/halo.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/halo.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/halo.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/ibd.py` & `ontogpt-0.2.5/src/ontogpt/templates/ibd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/ibd.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/ibd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/mendelian_disease.py` & `ontogpt-0.2.5/src/ontogpt/templates/mendelian_disease.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/mendelian_disease.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/mendelian_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/metabolic_process.py` & `ontogpt-0.2.5/src/ontogpt/templates/metabolic_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/metabolic_process.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/metabolic_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/metagenome_study.py` & `ontogpt-0.2.5/src/ontogpt/templates/metagenome_study.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/metagenome_study.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/metagenome_study.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/ontology_class.py` & `ontogpt-0.2.5/src/ontogpt/templates/ontology_class.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/ontology_class.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/ontology_class.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/ontology_issue.py` & `ontogpt-0.2.5/src/ontogpt/templates/ontology_issue.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/ontology_issue.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/ontology_issue.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/phenotype.py` & `ontogpt-0.2.5/src/ontogpt/templates/phenotype.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/phenotype.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/phenotype.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/reaction.py` & `ontogpt-0.2.5/src/ontogpt/templates/reaction.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/reaction.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/reaction.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/recipe.py` & `ontogpt-0.2.5/src/ontogpt/templates/recipe.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/recipe.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/recipe.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/treatment.py` & `ontogpt-0.2.5/src/ontogpt/templates/treatment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/templates/treatment.yaml` & `ontogpt-0.2.5/src/ontogpt/templates/treatment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/utils/gene_set_utils.py` & `ontogpt-0.2.5/src/ontogpt/utils/gene_set_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for handling gene sets."""
+import csv
 import glob
 import json
 import logging
 from copy import deepcopy
 from pathlib import Path
 from random import sample
 from typing import Dict, List, Optional, Tuple, Union
@@ -81,31 +82,72 @@
     - txt (one gene symbol per line)
 
     This does no normalization of gene symbols or ids.
     """
     if isinstance(input_path, Path):
         input_path = str(input_path)
     if format is None:
-        format = input_path.split(".")[-1]
+        if "gene_export_geneset" in input_path:
+            format = "geneweaver"
+        else:
+            format = input_path.split(".")[-1]
     if format == "yaml":
         with open(input_path, "r") as f:
             gene_set = GeneSet(**yaml.safe_load(f))
     elif format == "json" or format == "msigdb":
         with open(input_path, "r") as f:
             name, msig = list(json.load(f).items())[0]
             gene_set = GeneSet(name=name, gene_symbols=msig["geneSymbols"])
+    elif format == "geneweaver":
+        gene_set = parse_geneweaver(input_path)
     elif format == "txt":
         with open(input_path, "r") as f:
             gene_symbols = [line.strip() for line in f.readlines()]
             gene_set = GeneSet(name=input_path, gene_symbols=gene_symbols)
     else:
         raise ValueError(f"Unknown format {format}")
     return gene_set
 
 
+def parse_geneweaver(path: str) -> GeneSet:
+    gene_set = GeneSet(name=Path(path).stem, source="geneweaver", gene_ids=[], gene_symbols=[])
+    col2sp = {
+        "Wormbase": "C elegans",
+        "ZFIN": "Danio rerio",
+    }
+    fix = {
+        "Wormbase": "WB",
+    }
+    with open(path, "r") as f:
+        reader = csv.DictReader(f, delimiter="\t")
+        col = None
+        sp = None
+        for row in reader:
+            sym = row["Gene Symbol"]
+            if not col:
+                for k, v in col2sp.items():
+                    if row.get(k, None):
+                        col = k
+                        db = col
+                        gene_set.taxon = v
+                        if col in fix:
+                            db = fix[col]
+                        break
+            if not col:
+                raise ValueError("Unknown column")
+
+            id = f"{db}:{row[col]}"
+            gene = Gene(id=id, symbol=sym)
+            gene_set.gene_ids.append(id)
+            gene_set.gene_symbols.append(sym)
+            gene_set.gene_ids.append(id)
+    return gene_set
+
+
+
 def load_gene_sets(
     path: str, ontology_adapter: BasicOntologyInterface = None, strict=False, fill_missing=True,
 ) -> GeneSetCollection:
     """Load collection of gene sets from a folder.
 
     If ontology_adapter is provided, gene symbols will be converted to gene ids and vice versa.
     """
```

### Comparing `ontogpt-0.2.4/src/ontogpt/webapp/html/form.html` & `ontogpt-0.2.5/src/ontogpt/webapp/html/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/webapp/html/spindoctor/form.html` & `ontogpt-0.2.5/src/ontogpt/webapp/html/spindoctor/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.4/src/ontogpt/webapp/main.py` & `ontogpt-0.2.5/src/ontogpt/webapp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class Query(BaseModel):
     text: str
     datamodel: str
 
 
 app = FastAPI()
-
+static_dir.mkdir(parents=True, exist_ok=True)
 app.mount("/static", StaticFiles(directory=str(static_dir)), name="static")
 templates = Jinja2Templates(directory=str(html_dir))
 
 html_exporter = HTMLExporter()
 engines: Dict[str, SPIRESEngine] = {}
```

### Comparing `ontogpt-0.2.4/PKG-INFO` & `ontogpt-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontogpt
-Version: 0.2.4
+Version: 0.2.5
 Summary: OntoGPT
 License: BSD-3
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -49,14 +49,16 @@
 Requires-Dist: sphinx[docs] (>=5.3.0,<6.0.0) ; extra == "docs"
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0) ; extra == "web"
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Requires-Dist: wikipedia-api (>=0.5.8,<0.6.0)
 Description-Content-Type: text/markdown
 
+[![DOI](https://zenodo.org/badge/13996/monarch-initiative/ontogpt.svg)](https://zenodo.org/badge/latestdoi/13996/monarch-initiative/ontogpt)
+
 # OntoGPT
 
 Generation of Ontologies and Knowledge Bases using GPT
 
 A knowledge extraction tool that uses a large language model to extract semantic information from text.
 
 This makes use of so-called *instruction prompts* in Large Language Models (LLMs) such as GPT-4.
@@ -251,15 +253,22 @@
 
 ```
 ontogpt extract -t mendelian_disease.MendelianDisease -i marfan-wikipedia.txt
 ```
 
 ## Web Application
 
-There is a bare bones web application
+There is a bare bones web application for running OntoGPT and viewing results.
+
+Install the required dependencies first with the following command:
+```
+poetry install -E web
+```
+
+Then run the following command to start the web application:
 
 ```
 poetry run web-ontogpt
 ```
 
 Note that the agent running uvicorn must have the API key set, so for obvious reasons
 don't host this publicly without authentication, unless you want your credits drained.
@@ -393,27 +402,25 @@
 
 
 ## Gene Enrichment using SPINDOCTOR
 
 Given a set of genes, OntoGPT can find similarities among them.
 
 Example:
+
 ```
-ontogpt  enrichment -r sqlite:obo:hgnc  -U tests/input/genesets/sensory-ataxia.yaml
+ontogpt  enrichment -U tests/input/genesets/sensory-ataxia.yaml
 ```
 
-This gives both a narrative summary:
-
-__
+The default is to use ontological gene function synopses (via the Alliance API).
 
-and structured term list:
+To use narrative/RefSeq summaries, use the `--no-ontological-synopses` flag.
 
-```
+To run without any gene descriptions, use the `--no-annotations` flag.
 
-```
 
 ## OntoGPT Limitations
 
 ### Non-deterministic
 
 This relies on an existing LLM, and LLMs can be fickle in their responses.
```

