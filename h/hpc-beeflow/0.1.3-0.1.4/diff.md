# Comparing `tmp/hpc-beeflow-0.1.3.tar.gz` & `tmp/hpc_beeflow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpc-beeflow-0.1.3.tar", max compression
+gzip compressed data, was "hpc_beeflow-0.1.4.tar", max compression
```

## Comparing `hpc-beeflow-0.1.3.tar` & `hpc_beeflow-0.1.4.tar`

### file list

```diff
@@ -1,211 +1,259 @@
--rw-r--r--   0        0        0     1477 2022-12-16 21:16:44.512906 hpc-beeflow-0.1.3/LICENSE
--rw-r--r--   0        0        0     4108 2022-12-16 21:16:44.513055 hpc-beeflow-0.1.3/README.rst
--rwxr-xr-x   0        0        0    12933 2022-12-16 21:16:44.513463 hpc-beeflow-0.1.3/beeflow/cli.py
--rw-r--r--   0        0        0      122 2022-12-16 21:16:44.513653 hpc-beeflow-0.1.3/beeflow/client/README.md
--rw-r--r--   0        0        0    15932 2022-12-21 21:24:29.022589 hpc-beeflow-0.1.3/beeflow/client/bee_client.py
--rw-r--r--   0        0        0     8239 2022-12-16 21:16:44.514042 hpc-beeflow-0.1.3/beeflow/cloud_launcher.py
--rw-r--r--   0        0        0      234 2022-12-16 21:16:44.514236 hpc-beeflow-0.1.3/beeflow/common/README.md
--rw-r--r--   0        0        0      459 2022-12-16 21:16:44.514382 hpc-beeflow-0.1.3/beeflow/common/api.py
--rw-r--r--   0        0        0    11597 2022-12-16 21:16:44.514604 hpc-beeflow-0.1.3/beeflow/common/build/README.md
--rw-r--r--   0        0        0     5734 2022-12-16 21:16:44.514764 hpc-beeflow-0.1.3/beeflow/common/build/build_driver.py
--rw-r--r--   0        0        0    19070 2022-12-16 21:16:44.514966 hpc-beeflow-0.1.3/beeflow/common/build/container_drivers.py
--rw-r--r--   0        0        0     3366 2022-12-16 21:16:44.515146 hpc-beeflow-0.1.3/beeflow/common/build_interfaces.py
--rw-r--r--   0        0        0      285 2022-12-16 21:16:44.515276 hpc-beeflow-0.1.3/beeflow/common/cli.py
--rw-r--r--   0        0        0     3023 2022-12-16 21:16:44.515408 hpc-beeflow-0.1.3/beeflow/common/cli_connection.py
--rw-r--r--   0        0        0     2542 2022-12-16 21:16:44.515601 hpc-beeflow-0.1.3/beeflow/common/cloud/README.md
--rw-r--r--   0        0        0      830 2022-12-16 21:16:44.515735 hpc-beeflow-0.1.3/beeflow/common/cloud/__init__.py
--rw-r--r--   0        0        0     1166 2022-12-16 21:16:44.515889 hpc-beeflow-0.1.3/beeflow/common/cloud/chameleoncloud.py
--rw-r--r--   0        0        0      315 2022-12-16 21:16:44.516077 hpc-beeflow-0.1.3/beeflow/common/cloud/cloud.py
--rw-r--r--   0        0        0       42 2022-12-16 21:16:44.516283 hpc-beeflow-0.1.3/beeflow/common/cloud/constants.py
--rw-r--r--   0        0        0     1694 2022-12-16 21:16:44.516478 hpc-beeflow-0.1.3/beeflow/common/cloud/google.py
--rw-r--r--   0        0        0     1093 2022-12-16 21:16:44.516673 hpc-beeflow-0.1.3/beeflow/common/cloud/openstack.py
--rw-r--r--   0        0        0      784 2022-12-16 21:16:44.516864 hpc-beeflow-0.1.3/beeflow/common/cloud/provider.py
--rw-r--r--   0        0        0    25345 2022-12-16 21:16:44.517195 hpc-beeflow-0.1.3/beeflow/common/config_driver.py
--rw-r--r--   0        0        0     5779 2022-12-16 21:16:44.517456 hpc-beeflow-0.1.3/beeflow/common/config_validator.py
--rw-r--r--   0        0        0     2420 2022-12-16 21:16:44.517637 hpc-beeflow-0.1.3/beeflow/common/connection.py
--rw-r--r--   0        0        0      947 2022-12-16 21:16:44.517850 hpc-beeflow-0.1.3/beeflow/common/container_path.py
--rw-r--r--   0        0        0     6264 2022-12-16 21:16:44.518122 hpc-beeflow-0.1.3/beeflow/common/crt/charliecloud_driver.py
--rw-r--r--   0        0        0     1166 2022-12-16 21:16:44.518328 hpc-beeflow-0.1.3/beeflow/common/crt/crt_driver.py
--rw-r--r--   0        0        0     1713 2022-12-16 21:16:44.518489 hpc-beeflow-0.1.3/beeflow/common/crt/singularity_driver.py
--rw-r--r--   0        0        0     1551 2022-12-16 21:16:44.518664 hpc-beeflow-0.1.3/beeflow/common/crt_interface.py
--rw-r--r--   0        0        0     1901 2022-12-16 21:16:44.518968 hpc-beeflow-0.1.3/beeflow/common/db/sched.py
--rw-r--r--   0        0        0     5327 2022-12-16 21:16:44.519138 hpc-beeflow-0.1.3/beeflow/common/db/tm.py
--rw-r--r--   0        0        0     2133 2022-12-16 21:16:44.519327 hpc-beeflow-0.1.3/beeflow/common/expr.py
--rw-r--r--   0        0        0     5924 2022-12-16 21:16:44.519579 hpc-beeflow-0.1.3/beeflow/common/gdb/DESIGN.md
--rw-r--r--   0        0        0     8239 2022-12-16 21:16:44.519741 hpc-beeflow-0.1.3/beeflow/common/gdb/gdb_driver.py
--rw-r--r--   0        0        0    23333 2022-12-16 21:16:44.519950 hpc-beeflow-0.1.3/beeflow/common/gdb/neo4j_cypher.py
--rw-r--r--   0        0        0    22672 2022-12-16 21:16:44.520177 hpc-beeflow-0.1.3/beeflow/common/gdb/neo4j_driver.py
--rw-r--r--   0        0        0     9736 2022-12-16 21:16:44.520502 hpc-beeflow-0.1.3/beeflow/common/gdb_interface.py
--rw-r--r--   0        0        0      642 2022-12-16 21:16:44.520716 hpc-beeflow-0.1.3/beeflow/common/log.py
--rw-r--r--   0        0        0       16 2022-12-16 21:16:44.520996 hpc-beeflow-0.1.3/beeflow/common/parser/.gitignore
--rw-r--r--   0        0        0     2614 2022-12-16 21:16:44.521226 hpc-beeflow-0.1.3/beeflow/common/parser/README.md
--rw-r--r--   0        0        0      102 2022-12-16 21:16:44.521419 hpc-beeflow-0.1.3/beeflow/common/parser/__init__.py
--rw-r--r--   0        0        0    14476 2022-12-16 21:16:44.521682 hpc-beeflow-0.1.3/beeflow/common/parser/parser.py
--rw-r--r--   0        0        0    11021 2022-12-16 21:16:44.521952 hpc-beeflow-0.1.3/beeflow/common/wf_data.py
--rw-r--r--   0        0        0    13026 2022-12-16 21:16:44.522136 hpc-beeflow-0.1.3/beeflow/common/wf_interface.py
--rw-r--r--   0        0        0     1522 2022-12-16 21:16:44.522319 hpc-beeflow-0.1.3/beeflow/common/wf_profiler.py
--rw-r--r--   0        0        0      493 2022-12-16 21:16:44.522632 hpc-beeflow-0.1.3/beeflow/common/worker/README.md
--rw-r--r--   0        0        0      516 2022-12-16 21:16:44.522800 hpc-beeflow-0.1.3/beeflow/common/worker/__init__.py
--rw-r--r--   0        0        0     2570 2022-12-16 21:16:44.523071 hpc-beeflow-0.1.3/beeflow/common/worker/lsf_worker.py
--rw-r--r--   0        0        0     1731 2022-12-16 21:16:44.523265 hpc-beeflow-0.1.3/beeflow/common/worker/simple_worker.py
--rw-r--r--   0        0        0     4991 2022-12-21 21:24:29.022919 hpc-beeflow-0.1.3/beeflow/common/worker/slurm_worker.py
--rw-r--r--   0        0        0     4022 2022-12-21 21:24:29.023249 hpc-beeflow-0.1.3/beeflow/common/worker/worker.py
--rw-r--r--   0        0        0     1794 2022-12-16 21:16:44.523960 hpc-beeflow-0.1.3/beeflow/common/worker_interface.py
--rw-r--r--   0        0        0     4301 2022-12-16 21:16:44.524441 hpc-beeflow-0.1.3/beeflow/data/cloud_templates/dora.jinja
--rw-r--r--   0        0        0      866 2022-12-16 21:16:44.524596 hpc-beeflow-0.1.3/beeflow/data/cloud_templates/dora.yaml
--rw-r--r--   0        0        0      414 2022-12-16 21:16:44.524819 hpc-beeflow-0.1.3/beeflow/data/cwl/README.md
--rw-r--r--   0        0        0     1281 2022-12-16 21:16:44.525022 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/README.md
--rw-r--r--   0        0        0      315 2022-12-16 21:16:44.525245 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/README.md
--rw-r--r--   0        0        0      418 2022-12-16 21:16:44.525381 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast.yml
--rw-r--r--   0        0        0      423 2022-12-16 21:16:44.525509 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast_output.cwl
--rw-r--r--   0        0        0      300 2022-12-16 21:16:44.525663 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast_output_err.cwl
--rw-r--r--   0        0        0      410 2022-12-16 21:16:44.525782 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast_split.cwl
--rw-r--r--   0        0        0     2009 2022-12-16 21:16:44.525913 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl
--rw-r--r--   0        0        0      559 2022-12-16 21:16:44.526042 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl
--rw-r--r--   0        0        0      559 2022-12-16 21:16:44.526172 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl
--rwxr-xr-x   0        0        0   930997 2022-12-16 21:16:44.529619 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/input/small.fasta
--rw-r--r--   0        0        0      350 2022-12-16 21:16:44.529873 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-ci/README.md
--rw-r--r--   0        0        0     1968 2022-12-16 21:16:44.530017 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl
--rw-r--r--   0        0        0      302 2022-12-16 21:16:44.530157 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.json
--rw-r--r--   0        0        0      429 2022-12-16 21:16:44.530298 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.yml
--rw-r--r--   0        0        0     2228 2022-12-16 21:16:44.530443 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2022-12-16 21:16:44.530578 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl
--rw-r--r--   0        0        0      350 2022-12-16 21:16:44.538493 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf/README.md
--rw-r--r--   0        0        0     1977 2022-12-16 21:16:44.538644 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl
--rw-r--r--   0        0        0      302 2022-12-16 21:16:44.538788 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.json
--rw-r--r--   0        0        0      455 2022-12-16 21:16:44.538951 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.yml
--rw-r--r--   0        0        0     2145 2022-12-21 21:24:29.023606 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl
--rw-r--r--   0        0        0      815 2022-12-21 21:24:29.023882 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl
--rw-r--r--   0        0        0      350 2022-12-16 21:16:44.530858 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/README.md
--rw-r--r--   0        0        0     2077 2022-12-16 21:16:44.531014 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr.cwl
--rw-r--r--   0        0        0      339 2022-12-16 21:16:44.531146 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_job.json
--rw-r--r--   0        0        0      454 2022-12-16 21:16:44.531290 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_job.yml
--rw-r--r--   0        0        0      339 2022-12-16 21:16:44.531477 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_job_long.yml
--rw-r--r--   0        0        0     2430 2022-12-16 21:16:44.531659 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2022-12-16 21:16:44.531804 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/ffmpeg.cwl
--rw-r--r--   0        0        0      383 2022-12-16 21:16:44.532014 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/README.md
--rw-r--r--   0        0        0     1962 2022-12-16 21:16:44.532184 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl
--rw-r--r--   0        0        0      302 2022-12-16 21:16:44.532313 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.json
--rw-r--r--   0        0        0      411 2022-12-16 21:16:44.532442 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.yml
--rw-r--r--   0        0        0     2006 2022-12-16 21:16:44.532573 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl
--rw-r--r--   0        0        0      753 2022-12-16 21:16:44.532710 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl
--rw-r--r--   0        0        0      837 2022-12-16 21:16:44.532918 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md
--rw-r--r--   0        0        0      304 2022-12-16 21:16:44.533157 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/README.md
--rw-r--r--   0        0        0     1234 2022-12-16 21:16:44.533372 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl
--rw-r--r--   0        0        0      145 2022-12-16 21:16:44.533648 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/Dockerfile.clamr-lanl-x86_64
--rw-r--r--   0        0        0     3325 2022-12-16 21:16:44.533846 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md
--rw-r--r--   0        0        0     1127 2022-12-16 21:16:44.534090 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl
--rw-r--r--   0        0        0     1135 2022-12-16 21:16:44.534409 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl
--rw-r--r--   0        0        0     1137 2022-12-16 21:16:44.534670 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl
--rw-r--r--   0        0        0     1176 2022-12-16 21:16:44.534819 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl
--rw-r--r--   0        0        0     1137 2022-12-16 21:16:44.534959 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl
--rw-r--r--   0        0        0     1133 2022-12-16 21:16:44.535094 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl
--rw-r--r--   0        0        0      182 2022-12-16 21:16:44.535347 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/README.md
--rw-r--r--   0        0        0     1122 2022-12-16 21:16:44.535533 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl
--rw-r--r--   0        0        0      303 2022-12-16 21:16:44.535776 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/README.md
--rw-r--r--   0        0        0     1975 2022-12-16 21:16:44.535933 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl
--rw-r--r--   0        0        0      302 2022-12-16 21:16:44.536055 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.json
--rw-r--r--   0        0        0      418 2022-12-16 21:16:44.536188 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.yml
--rw-r--r--   0        0        0     2057 2022-12-16 21:16:44.536307 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl
--rw-r--r--   0        0        0      768 2022-12-16 21:16:44.536427 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl
--rw-r--r--   0        0        0      339 2022-12-16 21:16:44.536676 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-summit/README.md
--rw-r--r--   0        0        0     1962 2022-12-16 21:16:44.536815 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl
--rw-r--r--   0        0        0      302 2022-12-16 21:16:44.536938 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.json
--rw-r--r--   0        0        0      418 2022-12-16 21:16:44.537063 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.yml
--rw-r--r--   0        0        0     2103 2022-12-16 21:16:44.537205 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2022-12-16 21:16:44.537326 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl
--rw-r--r--   0        0        0      350 2022-12-16 21:16:44.537534 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/README.md
--rw-r--r--   0        0        0     1981 2022-12-16 21:16:44.537672 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl
--rw-r--r--   0        0        0      302 2022-12-16 21:16:44.537794 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.json
--rw-r--r--   0        0        0      430 2022-12-16 21:16:44.537922 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.yml
--rw-r--r--   0        0        0     1939 2022-12-16 21:16:44.538053 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2022-12-16 21:16:44.538183 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl
--rw-r--r--   0        0        0     2439 2022-12-16 21:16:44.538308 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf.tgz
--rw-r--r--   0        0        0      570 2022-12-16 21:16:44.539415 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl
--rw-r--r--   0        0        0      110 2022-12-16 21:16:44.539566 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/comd-mpi/comd.yml
--rw-r--r--   0        0        0      527 2022-12-16 21:16:44.539699 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/comd-mpi/comd_bin.cwl
--rw-r--r--   0        0        0      756 2022-12-16 21:16:44.539899 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl
--rw-r--r--   0        0        0       24 2022-12-16 21:16:44.540034 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.yml
--rw-r--r--   0        0        0     1282 2022-12-16 21:16:44.540273 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md
--rw-r--r--   0        0        0      590 2022-12-16 21:16:44.540402 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl
--rw-r--r--   0        0        0      161 2022-12-16 21:16:44.540519 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.yml
--rw-r--r--   0        0        0      199 2022-12-16 21:16:44.540640 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem_bin.cwl
--rw-r--r--   0        0        0       71 2022-12-16 21:16:44.540766 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/pytest.ini
--rw-r--r--   0        0        0      317 2022-12-16 21:16:44.540958 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/README.md
--rw-r--r--   0        0        0      986 2022-12-16 21:16:44.541094 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl
--rw-r--r--   0        0        0      217 2022-12-16 21:16:44.541327 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/README.md
--rw-r--r--   0        0        0     1083 2022-12-16 21:16:44.541540 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl
--rw-r--r--   0        0        0     1325 2022-12-16 21:16:44.541791 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl
--rw-r--r--   0        0        0     3776 2022-12-16 21:16:44.541978 hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt
--rw-r--r--   0        0        0      426 2022-12-16 21:16:44.542179 hpc-beeflow-0.1.3/beeflow/data/cwl/cwl_validation/README.md
--rwxr-xr-x   0        0        0      398 2022-12-16 21:16:44.542386 hpc-beeflow-0.1.3/beeflow/data/cwl/cwl_validation/builder/dockerFile.cwl
--rwxr-xr-x   0        0        0      317 2022-12-16 21:16:44.542518 hpc-beeflow-0.1.3/beeflow/data/cwl/cwl_validation/builder/dockerPull.cwl
--rw-r--r--   0        0        0     1202 2022-12-16 21:16:44.542740 hpc-beeflow-0.1.3/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl
--rw-r--r--   0        0        0     3776 2022-12-16 21:16:44.542909 hpc-beeflow-0.1.3/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt
--rwxr-xr-x   0        0        0      169 2022-12-16 21:16:44.543038 hpc-beeflow-0.1.3/beeflow/data/cwl/cwl_validation/helloworld.cwl
--rw-r--r--   0        0        0       19 2022-12-16 21:16:44.543158 hpc-beeflow-0.1.3/beeflow/data/cwl/cwl_validation/helloworld_input.yaml
--rw-r--r--   0        0        0       80 2022-12-16 21:16:44.543356 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.builder_demo
--rw-r--r--   0        0        0      411 2022-12-16 21:16:44.543491 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.clamr-ffmpeg
--rw-r--r--   0        0        0      145 2022-12-16 21:16:44.543627 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.clamr-lanl-x86_64
--rw-r--r--   0        0        0      724 2022-12-16 21:16:44.543783 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le
--rw-r--r--   0        0        0      391 2022-12-16 21:16:44.543923 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.comd-x86_64
--rw-r--r--   0        0        0      270 2022-12-16 21:16:44.544056 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.deb9ompi-x86_64
--rw-r--r--   0        0        0      592 2022-12-16 21:16:44.544178 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64
--rw-r--r--   0        0        0     1605 2022-12-16 21:16:44.544301 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le
--rw-r--r--   0        0        0     2489 2022-12-16 21:16:44.544432 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64
--rw-r--r--   0        0        0     3446 2022-12-16 21:16:44.544575 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64
--rw-r--r--   0        0        0      614 2022-12-16 21:16:44.544704 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/README.md
--rw-r--r--   0        0        0      331 2022-12-16 21:16:44.544931 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.comd-x86_64-wpmix
--rw-r--r--   0        0        0      573 2022-12-16 21:16:44.545079 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian
--rw-r--r--   0        0        0     3941 2022-12-16 21:16:44.545228 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5
--rw-r--r--   0        0        0      509 2022-12-16 21:16:44.545366 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/comd-pmix-support/README.md
--rw-r--r--   0        0        0      813 2022-12-16 21:16:44.545505 hpc-beeflow-0.1.3/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch
--rw-r--r--   0        0        0     1216 2022-12-16 21:16:44.545705 hpc-beeflow-0.1.3/beeflow/data/job_templates/README.md
--rw-r--r--   0        0        0      434 2022-12-16 21:16:44.545850 hpc-beeflow-0.1.3/beeflow/data/job_templates/lsf-submit.jinja
--rw-r--r--   0        0        0      760 2022-12-16 21:16:44.546028 hpc-beeflow-0.1.3/beeflow/data/job_templates/slurm-pmix_v3.jinja
--rw-r--r--   0        0        0      824 2022-12-16 21:16:44.546228 hpc-beeflow-0.1.3/beeflow/data/job_templates/slurm-submit-timelimit.jinja
--rw-r--r--   0        0        0      746 2022-12-16 21:16:44.546422 hpc-beeflow-0.1.3/beeflow/data/job_templates/slurm-submit.jinja
--rw-r--r--   0        0        0     1708 2022-12-16 21:16:44.546713 hpc-beeflow-0.1.3/beeflow/scheduler/README.md
--rw-r--r--   0        0        0    10485 2022-12-16 21:16:44.546957 hpc-beeflow-0.1.3/beeflow/scheduler/algorithms.py
--rw-r--r--   0        0        0     9336 2022-12-16 21:16:44.547161 hpc-beeflow-0.1.3/beeflow/scheduler/resource_allocation.py
--rw-r--r--   0        0        0     4344 2022-12-16 21:16:44.547393 hpc-beeflow-0.1.3/beeflow/scheduler/scheduler.py
--rw-r--r--   0        0        0     2890 2022-12-16 21:16:44.547606 hpc-beeflow-0.1.3/beeflow/scheduler/scheduler.yaml
--rw-r--r--   0        0        0      708 2022-12-16 21:16:44.547887 hpc-beeflow-0.1.3/beeflow/scheduler/serializable.py
--rw-r--r--   0        0        0     2296 2022-12-16 21:16:44.548092 hpc-beeflow-0.1.3/beeflow/scheduler/task.py
--rwxr-xr-x   0        0        0    13008 2022-12-16 21:16:44.548398 hpc-beeflow-0.1.3/beeflow/task_manager.py
--rw-r--r--   0        0        0    34925 2022-12-16 21:16:44.548841 hpc-beeflow-0.1.3/beeflow/tests/42.tgz
--rw-r--r--   0        0        0      236 2022-12-16 21:16:44.549027 hpc-beeflow-0.1.3/beeflow/tests/README.md
--rw-r--r--   0        0        0     1139 2022-12-16 21:16:44.549156 hpc-beeflow-0.1.3/beeflow/tests/cf.cwl
--rw-r--r--   0        0        0     1093 2022-12-16 21:16:44.549475 hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/clamr.cwl
--rw-r--r--   0        0        0      302 2022-12-16 21:16:44.549639 hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/clamr_job.json
--rw-r--r--   0        0        0      424 2022-12-16 21:16:44.549774 hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/clamr_job.yml
--rw-r--r--   0        0        0     1320 2022-12-16 21:16:44.549906 hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/clamr_wf.cwl
--rw-r--r--   0        0        0      680 2022-12-16 21:16:44.550045 hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/ffmpeg.cwl
--rw-r--r--   0        0        0      273 2022-12-16 21:16:44.550170 hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/mv_script.cwl
--rwxr-xr-x   0        0        0      324 2022-12-16 21:16:44.550304 hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/mv_script.sh
--rw-r--r--   0        0        0     2401 2022-12-16 21:16:44.549284 hpc-beeflow-0.1.3/beeflow/tests/clamr-wf.tgz
--rw-r--r--   0        0        0      774 2022-12-16 21:16:44.550448 hpc-beeflow-0.1.3/beeflow/tests/gdb.py
--rw-r--r--   0        0        0    12378 2022-12-16 21:16:44.550606 hpc-beeflow-0.1.3/beeflow/tests/mocks.py
--rw-r--r--   0        0        0      267 2022-12-16 21:16:44.550747 hpc-beeflow-0.1.3/beeflow/tests/test_cloud.py
--rw-r--r--   0        0        0     6006 2022-12-16 21:16:44.550905 hpc-beeflow-0.1.3/beeflow/tests/test_config_validator.py
--rw-r--r--   0        0        0      807 2022-12-16 21:16:44.551050 hpc-beeflow-0.1.3/beeflow/tests/test_container_path.py
--rw-r--r--   0        0        0      819 2022-12-16 21:16:44.551200 hpc-beeflow-0.1.3/beeflow/tests/test_db_sched.py
--rw-r--r--   0        0        0     4427 2022-12-16 21:16:44.551364 hpc-beeflow-0.1.3/beeflow/tests/test_db_tm.py
--rw-r--r--   0        0        0     2350 2022-12-16 21:16:44.551520 hpc-beeflow-0.1.3/beeflow/tests/test_parser.py
--rw-r--r--   0        0        0    15134 2022-12-16 21:16:44.551675 hpc-beeflow-0.1.3/beeflow/tests/test_scheduler.py
--rw-r--r--   0        0        0     2630 2022-12-16 21:16:44.551818 hpc-beeflow-0.1.3/beeflow/tests/test_scheduler_resource_allocation.py
--rw-r--r--   0        0        0     6558 2022-12-16 21:16:44.551991 hpc-beeflow-0.1.3/beeflow/tests/test_scheduler_rest.py
--rw-r--r--   0        0        0     5113 2022-12-16 21:16:44.552146 hpc-beeflow-0.1.3/beeflow/tests/test_slurm_worker.py
--rw-r--r--   0        0        0     3390 2022-12-16 21:16:44.552313 hpc-beeflow-0.1.3/beeflow/tests/test_tm.py
--rw-r--r--   0        0        0    30859 2022-12-16 21:16:44.552571 hpc-beeflow-0.1.3/beeflow/tests/test_wf_interface.py
--rw-r--r--   0        0        0     7524 2022-12-16 21:16:44.552753 hpc-beeflow-0.1.3/beeflow/tests/test_wf_manager.py
--rwxr-xr-x   0        0        0     7935 2022-12-16 21:16:44.553039 hpc-beeflow-0.1.3/beeflow/wf_manager/common/dep_manager.py
--rw-r--r--   0        0        0     9282 2022-12-16 21:16:44.553206 hpc-beeflow-0.1.3/beeflow/wf_manager/common/wf_db.py
--rw-r--r--   0        0        0     4050 2022-12-16 21:16:44.553432 hpc-beeflow-0.1.3/beeflow/wf_manager/resources/wf_actions.py
--rw-r--r--   0        0        0     8264 2022-12-16 21:16:44.553698 hpc-beeflow-0.1.3/beeflow/wf_manager/resources/wf_list.py
--rw-r--r--   0        0        0     5215 2022-12-16 21:16:44.553880 hpc-beeflow-0.1.3/beeflow/wf_manager/resources/wf_update.py
--rw-r--r--   0        0        0     7714 2022-12-16 21:16:44.554045 hpc-beeflow-0.1.3/beeflow/wf_manager/resources/wf_utils.py
--rw-r--r--   0        0        0     1051 2022-12-16 21:16:44.554180 hpc-beeflow-0.1.3/beeflow/wf_manager/wf_manager.py
--rw-r--r--   0        0        0     2523 2022-12-22 21:03:41.844763 hpc-beeflow-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7519 2022-12-22 21:04:06.026183 hpc-beeflow-0.1.3/setup.py
--rw-r--r--   0        0        0     6058 2022-12-22 21:04:06.026592 hpc-beeflow-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1477 2023-04-25 21:47:28.980995 hpc_beeflow-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4903 2023-04-25 21:47:28.981096 hpc_beeflow-0.1.4/README.rst
+-rwxr-xr-x   0        0        0    14754 2023-05-05 17:47:06.278273 hpc_beeflow-0.1.4/beeflow/cli.py
+-rw-r--r--   0        0        0      122 2023-04-25 21:47:28.981520 hpc_beeflow-0.1.4/beeflow/client/README.md
+-rw-r--r--   0        0        0    18282 2023-05-05 17:47:06.278602 hpc_beeflow-0.1.4/beeflow/client/bee_client.py
+-rw-r--r--   0        0        0     8036 2023-04-25 21:47:28.981805 hpc_beeflow-0.1.4/beeflow/cloud_launcher.py
+-rw-r--r--   0        0        0      234 2023-04-25 21:47:28.981918 hpc_beeflow-0.1.4/beeflow/common/README.md
+-rw-r--r--   0        0        0      459 2023-04-25 21:47:28.982000 hpc_beeflow-0.1.4/beeflow/common/api.py
+-rw-r--r--   0        0        0    11597 2023-04-25 21:47:28.982148 hpc_beeflow-0.1.4/beeflow/common/build/README.md
+-rw-r--r--   0        0        0     5734 2023-04-25 21:47:28.982334 hpc_beeflow-0.1.4/beeflow/common/build/build_driver.py
+-rw-r--r--   0        0        0    18962 2023-05-05 17:47:06.278843 hpc_beeflow-0.1.4/beeflow/common/build/container_drivers.py
+-rw-r--r--   0        0        0     3456 2023-04-25 21:47:28.982535 hpc_beeflow-0.1.4/beeflow/common/build_interfaces.py
+-rw-r--r--   0        0        0      285 2023-04-25 21:47:28.982612 hpc_beeflow-0.1.4/beeflow/common/cli.py
+-rw-r--r--   0        0        0     3023 2023-04-25 21:47:28.983190 hpc_beeflow-0.1.4/beeflow/common/cli_connection.py
+-rw-r--r--   0        0        0     2542 2023-04-25 21:47:28.983324 hpc_beeflow-0.1.4/beeflow/common/cloud/README.md
+-rw-r--r--   0        0        0      830 2023-04-25 21:47:28.983420 hpc_beeflow-0.1.4/beeflow/common/cloud/__init__.py
+-rw-r--r--   0        0        0     1166 2023-04-25 21:47:28.983503 hpc_beeflow-0.1.4/beeflow/common/cloud/chameleoncloud.py
+-rw-r--r--   0        0        0      175 2023-04-25 21:47:28.983588 hpc_beeflow-0.1.4/beeflow/common/cloud/cloud.py
+-rw-r--r--   0        0        0       42 2023-04-25 21:47:28.983663 hpc_beeflow-0.1.4/beeflow/common/cloud/constants.py
+-rw-r--r--   0        0        0     1599 2023-04-25 21:47:28.983758 hpc_beeflow-0.1.4/beeflow/common/cloud/google.py
+-rw-r--r--   0        0        0     1093 2023-04-25 21:47:28.983846 hpc_beeflow-0.1.4/beeflow/common/cloud/openstack.py
+-rw-r--r--   0        0        0      784 2023-04-25 21:47:28.983934 hpc_beeflow-0.1.4/beeflow/common/cloud/provider.py
+-rw-r--r--   0        0        0    24102 2023-05-09 22:30:18.856061 hpc_beeflow-0.1.4/beeflow/common/config_driver.py
+-rw-r--r--   0        0        0     5891 2023-04-25 21:47:28.984324 hpc_beeflow-0.1.4/beeflow/common/config_validator.py
+-rw-r--r--   0        0        0     2420 2023-04-25 21:47:28.984426 hpc_beeflow-0.1.4/beeflow/common/connection.py
+-rw-r--r--   0        0        0      947 2023-04-25 21:47:28.984512 hpc_beeflow-0.1.4/beeflow/common/container_path.py
+-rw-r--r--   0        0        0     6515 2023-04-25 21:47:28.984665 hpc_beeflow-0.1.4/beeflow/common/crt/charliecloud_driver.py
+-rw-r--r--   0        0        0     1487 2023-04-25 21:47:28.984782 hpc_beeflow-0.1.4/beeflow/common/crt/crt_driver.py
+-rw-r--r--   0        0        0     1767 2023-04-25 21:47:28.984875 hpc_beeflow-0.1.4/beeflow/common/crt/singularity_driver.py
+-rw-r--r--   0        0        0     1551 2023-04-25 21:47:28.985006 hpc_beeflow-0.1.4/beeflow/common/crt_interface.py
+-rw-r--r--   0        0        0     2553 2023-04-25 21:47:28.985129 hpc_beeflow-0.1.4/beeflow/common/db/bdb.py
+-rw-r--r--   0        0        0     1675 2023-04-25 21:47:28.985202 hpc_beeflow-0.1.4/beeflow/common/db/sched_db.py
+-rw-r--r--   0        0        0     5075 2023-04-25 21:47:28.985280 hpc_beeflow-0.1.4/beeflow/common/db/tm_db.py
+-rw-r--r--   0        0        0     8324 2023-04-25 21:47:28.985378 hpc_beeflow-0.1.4/beeflow/common/db/wfm_db.py
+-rw-r--r--   0        0        0     2133 2023-04-25 21:47:28.985469 hpc_beeflow-0.1.4/beeflow/common/expr.py
+-rw-r--r--   0        0        0     5924 2023-04-25 21:47:28.985612 hpc_beeflow-0.1.4/beeflow/common/gdb/DESIGN.md
+-rw-r--r--   0        0        0     8239 2023-04-25 21:47:28.985717 hpc_beeflow-0.1.4/beeflow/common/gdb/gdb_driver.py
+-rw-r--r--   0        0        0    23333 2023-04-25 21:47:28.985845 hpc_beeflow-0.1.4/beeflow/common/gdb/neo4j_cypher.py
+-rw-r--r--   0        0        0    22756 2023-04-25 21:47:28.985994 hpc_beeflow-0.1.4/beeflow/common/gdb/neo4j_driver.py
+-rw-r--r--   0        0        0     9736 2023-04-25 21:47:28.989071 hpc_beeflow-0.1.4/beeflow/common/gdb_interface.py
+-rw-r--r--   0        0        0      642 2023-04-25 21:47:28.989144 hpc_beeflow-0.1.4/beeflow/common/log.py
+-rw-r--r--   0        0        0       16 2023-04-25 21:47:28.989234 hpc_beeflow-0.1.4/beeflow/common/parser/.gitignore
+-rw-r--r--   0        0        0     2614 2023-04-25 21:47:28.989307 hpc_beeflow-0.1.4/beeflow/common/parser/README.md
+-rw-r--r--   0        0        0      102 2023-04-25 21:47:28.989397 hpc_beeflow-0.1.4/beeflow/common/parser/__init__.py
+-rw-r--r--   0        0        0    14476 2023-04-25 21:47:28.989535 hpc_beeflow-0.1.4/beeflow/common/parser/parser.py
+-rw-r--r--   0        0        0      493 2023-04-25 21:47:28.989613 hpc_beeflow-0.1.4/beeflow/common/tab_completion.py
+-rw-r--r--   0        0        0     1643 2023-05-05 17:47:06.279186 hpc_beeflow-0.1.4/beeflow/common/validation.py
+-rw-r--r--   0        0        0    11382 2023-04-25 21:47:28.989727 hpc_beeflow-0.1.4/beeflow/common/wf_data.py
+-rw-r--r--   0        0        0    13026 2023-04-25 21:47:28.989821 hpc_beeflow-0.1.4/beeflow/common/wf_interface.py
+-rw-r--r--   0        0        0     1522 2023-04-25 21:47:28.989906 hpc_beeflow-0.1.4/beeflow/common/wf_profiler.py
+-rw-r--r--   0        0        0      493 2023-04-25 21:47:28.990038 hpc_beeflow-0.1.4/beeflow/common/worker/README.md
+-rw-r--r--   0        0        0      516 2023-04-25 21:47:28.990130 hpc_beeflow-0.1.4/beeflow/common/worker/__init__.py
+-rw-r--r--   0        0        0     2570 2023-04-25 21:47:28.990261 hpc_beeflow-0.1.4/beeflow/common/worker/lsf_worker.py
+-rw-r--r--   0        0        0     1731 2023-04-25 21:47:28.990365 hpc_beeflow-0.1.4/beeflow/common/worker/simple_worker.py
+-rw-r--r--   0        0        0     9859 2023-05-09 22:30:18.856646 hpc_beeflow-0.1.4/beeflow/common/worker/slurm_worker.py
+-rw-r--r--   0        0        0     2899 2023-05-05 17:47:06.279519 hpc_beeflow-0.1.4/beeflow/common/worker/worker.py
+-rw-r--r--   0        0        0     1794 2023-04-25 21:47:28.990669 hpc_beeflow-0.1.4/beeflow/common/worker_interface.py
+-rw-r--r--   0        0        0     4301 2023-04-25 21:47:28.990832 hpc_beeflow-0.1.4/beeflow/data/cloud_templates/dora.jinja
+-rw-r--r--   0        0        0      866 2023-04-25 21:47:28.990917 hpc_beeflow-0.1.4/beeflow/data/cloud_templates/dora.yaml
+-rw-r--r--   0        0        0      414 2023-04-25 21:47:28.991033 hpc_beeflow-0.1.4/beeflow/data/cwl/README.md
+-rw-r--r--   0        0        0     1281 2023-04-25 21:47:28.991144 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/README.md
+-rw-r--r--   0        0        0      315 2023-04-25 21:47:28.991254 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/README.md
+-rw-r--r--   0        0        0      418 2023-04-25 21:47:28.991479 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast.yml
+-rw-r--r--   0        0        0      423 2023-04-25 21:47:28.991551 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast_output.cwl
+-rw-r--r--   0        0        0      300 2023-04-25 21:47:28.991624 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast_output_err.cwl
+-rw-r--r--   0        0        0      410 2023-04-25 21:47:28.991690 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast_split.cwl
+-rw-r--r--   0        0        0     2009 2023-04-25 21:47:28.991763 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl
+-rw-r--r--   0        0        0      559 2023-04-25 21:47:28.991833 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl
+-rw-r--r--   0        0        0      559 2023-04-25 21:47:28.991901 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl
+-rwxr-xr-x   0        0        0   930997 2023-04-25 21:47:28.994579 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/input/small.fasta
+-rw-r--r--   0        0        0      350 2023-04-25 21:47:28.994706 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-ci/README.md
+-rw-r--r--   0        0        0     1968 2023-04-25 21:47:28.994777 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl
+-rw-r--r--   0        0        0      302 2023-04-25 21:47:28.994847 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.json
+-rw-r--r--   0        0        0      429 2023-04-25 21:47:28.994926 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.yml
+-rw-r--r--   0        0        0     2228 2023-04-25 21:47:28.995018 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2023-04-25 21:47:28.995094 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl
+-rw-r--r--   0        0        0      350 2023-04-25 21:47:28.999935 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf/README.md
+-rw-r--r--   0        0        0     1977 2023-04-25 21:47:29.000007 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl
+-rw-r--r--   0        0        0      302 2023-04-25 21:47:29.000067 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.json
+-rw-r--r--   0        0        0      455 2023-04-25 21:47:29.000130 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.yml
+-rw-r--r--   0        0        0     2145 2023-04-25 21:47:29.000192 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl
+-rw-r--r--   0        0        0      815 2023-04-25 21:47:29.000252 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl
+-rw-r--r--   0        0        0      411 2023-05-05 17:47:06.279682 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/Dockerfile.clamr-ffmpeg
+-rw-r--r--   0        0        0      350 2023-04-25 21:47:28.995216 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/README.md
+-rw-r--r--   0        0        0     2064 2023-05-05 17:47:06.279832 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr.cwl
+-rw-r--r--   0        0        0      339 2023-04-25 21:47:28.995402 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_job.json
+-rw-r--r--   0        0        0      454 2023-04-25 21:47:28.995475 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_job.yml
+-rw-r--r--   0        0        0      339 2023-04-25 21:47:28.995543 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_job_long.yml
+-rw-r--r--   0        0        0     2524 2023-05-05 17:47:06.279976 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2023-04-25 21:47:28.995695 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/ffmpeg.cwl
+-rw-r--r--   0        0        0      383 2023-04-25 21:47:28.995807 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/README.md
+-rw-r--r--   0        0        0     1962 2023-04-25 21:47:28.995893 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl
+-rw-r--r--   0        0        0      302 2023-04-25 21:47:28.995962 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.json
+-rw-r--r--   0        0        0      411 2023-04-25 21:47:28.996043 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.yml
+-rw-r--r--   0        0        0     2006 2023-04-25 21:47:28.996110 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl
+-rw-r--r--   0        0        0      753 2023-04-25 21:47:28.996179 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl
+-rw-r--r--   0        0        0      837 2023-04-25 21:47:28.996296 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md
+-rw-r--r--   0        0        0      304 2023-04-25 21:47:28.996464 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/README.md
+-rw-r--r--   0        0        0     1234 2023-04-25 21:47:28.996562 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl
+-rw-r--r--   0        0        0      145 2023-04-25 21:47:28.996681 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/Dockerfile.clamr-lanl-x86_64
+-rw-r--r--   0        0        0     3325 2023-04-25 21:47:28.996775 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md
+-rw-r--r--   0        0        0     1127 2023-04-25 21:47:28.996851 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl
+-rw-r--r--   0        0        0     1135 2023-04-25 21:47:28.996921 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl
+-rw-r--r--   0        0        0     1137 2023-04-25 21:47:28.996990 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl
+-rw-r--r--   0        0        0     1176 2023-04-25 21:47:28.997063 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl
+-rw-r--r--   0        0        0     1137 2023-04-25 21:47:28.997136 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl
+-rw-r--r--   0        0        0     1133 2023-04-25 21:47:28.997217 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl
+-rw-r--r--   0        0        0      182 2023-04-25 21:47:28.997348 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/README.md
+-rw-r--r--   0        0        0     1122 2023-04-25 21:47:28.997441 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl
+-rw-r--r--   0        0        0      303 2023-04-25 21:47:28.997562 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/README.md
+-rw-r--r--   0        0        0     1975 2023-04-25 21:47:28.997639 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl
+-rw-r--r--   0        0        0      302 2023-04-25 21:47:28.997705 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.json
+-rw-r--r--   0        0        0      418 2023-04-25 21:47:28.997783 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.yml
+-rw-r--r--   0        0        0     2057 2023-04-25 21:47:28.997856 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl
+-rw-r--r--   0        0        0      768 2023-04-25 21:47:28.997935 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl
+-rw-r--r--   0        0        0      339 2023-04-25 21:47:28.998055 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-summit/README.md
+-rw-r--r--   0        0        0     1962 2023-04-25 21:47:28.998134 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl
+-rw-r--r--   0        0        0      302 2023-04-25 21:47:28.998270 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.json
+-rw-r--r--   0        0        0      418 2023-04-25 21:47:28.998350 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.yml
+-rw-r--r--   0        0        0     2103 2023-04-25 21:47:28.998435 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2023-04-25 21:47:28.998522 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl
+-rw-r--r--   0        0        0      350 2023-04-25 21:47:28.998645 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/README.md
+-rw-r--r--   0        0        0     1981 2023-04-25 21:47:28.998789 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl
+-rw-r--r--   0        0        0      302 2023-04-25 21:47:28.999069 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.json
+-rw-r--r--   0        0        0      430 2023-04-25 21:47:28.999155 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.yml
+-rw-r--r--   0        0        0     1939 2023-04-25 21:47:28.999246 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2023-04-25 21:47:28.999771 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl
+-rw-r--r--   0        0        0      527 2023-04-25 21:47:29.000349 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl
+-rw-r--r--   0        0        0      110 2023-04-25 21:47:29.000417 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/comd-mpi/comd_job.yml
+-rw-r--r--   0        0        0      555 2023-04-25 21:47:29.000482 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl
+-rw-r--r--   0        0        0      831 2023-04-25 21:47:29.000913 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl
+-rw-r--r--   0        0        0       24 2023-04-25 21:47:29.001008 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.yml
+-rw-r--r--   0        0        0      264 2023-04-25 21:47:29.000577 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh.cwl
+-rw-r--r--   0        0        0       24 2023-04-25 21:47:29.000669 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_job.yml
+-rw-r--r--   0        0        0      469 2023-04-25 21:47:29.000773 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_wf.cwl
+-rw-r--r--   0        0        0     1282 2023-04-25 21:47:29.001147 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md
+-rw-r--r--   0        0        0      590 2023-04-25 21:47:29.001253 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl
+-rw-r--r--   0        0        0      161 2023-04-25 21:47:29.001325 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.yml
+-rw-r--r--   0        0        0      199 2023-04-25 21:47:29.001386 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem_bin.cwl
+-rw-r--r--   0        0        0       71 2023-04-25 21:47:29.001443 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/pytest.ini
+-rw-r--r--   0        0        0      317 2023-04-25 21:47:29.001539 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/README.md
+-rw-r--r--   0        0        0      986 2023-04-25 21:47:29.001615 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl
+-rw-r--r--   0        0        0      217 2023-04-25 21:47:29.001709 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/README.md
+-rw-r--r--   0        0        0     1083 2023-04-25 21:47:29.001774 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl
+-rw-r--r--   0        0        0     1325 2023-04-25 21:47:29.001854 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl
+-rw-r--r--   0        0        0     3776 2023-04-25 21:47:29.001951 hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt
+-rw-r--r--   0        0        0      426 2023-04-25 21:47:29.002093 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/README.md
+-rwxr-xr-x   0        0        0      398 2023-04-25 21:47:29.002238 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/builder/dockerFile.cwl
+-rwxr-xr-x   0        0        0      317 2023-04-25 21:47:29.002333 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/builder/dockerPull.cwl
+-rw-r--r--   0        0        0     1202 2023-04-25 21:47:29.002463 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl
+-rw-r--r--   0        0        0     3776 2023-04-25 21:47:29.002550 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt
+-rwxr-xr-x   0        0        0      169 2023-04-25 21:47:29.002620 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/helloworld.cwl
+-rw-r--r--   0        0        0       19 2023-04-25 21:47:29.002681 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/helloworld_input.yaml
+-rw-r--r--   0        0        0    59407 2023-04-25 21:47:29.003142 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/DAG_example-1.png
+-rw-r--r--   0        0        0      833 2023-04-25 21:47:29.003262 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/README.md
+-rw-r--r--   0        0        0      254 2023-04-25 21:47:29.003333 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add.cwl
+-rw-r--r--   0        0        0      351 2023-04-25 21:47:29.003405 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_multiply_example_workflow.cwl
+-rw-r--r--   0        0        0      245 2023-04-25 21:47:29.003482 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_step1.py
+-rw-r--r--   0        0        0      386 2023-04-25 21:47:29.003555 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/isolated test.cwl
+-rw-r--r--   0        0        0       21 2023-04-25 21:47:29.003622 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/job.yaml
+-rw-r--r--   0        0        0      304 2023-04-25 21:47:29.003687 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply.cwl
+-rw-r--r--   0        0        0      267 2023-04-25 21:47:29.003759 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply_step2.py
+-rw-r--r--   0        0        0      407 2023-04-25 21:47:29.003840 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/workflow_generater_python.py
+-rw-r--r--   0        0        0     3496 2023-04-25 21:47:29.003994 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/README.md
+-rw-r--r--   0        0        0      901 2023-04-25 21:47:29.004107 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree.py
+-rw-r--r--   0        0        0      443 2023-04-25 21:47:29.004204 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_output.txt
+-rw-r--r--   0        0        0      234 2023-04-25 21:47:29.004308 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_tool.cwl
+-rw-r--r--   0        0        0      178 2023-04-25 21:47:29.004411 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/expectedValue.txt
+-rw-r--r--   0        0        0      157 2023-04-25 21:47:29.004497 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/hiring1.txt
+-rw-r--r--   0        0        0      467 2023-04-25 21:47:29.004576 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regress_output.txt
+-rw-r--r--   0        0        0     1203 2023-04-25 21:47:29.004690 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regression.py
+-rw-r--r--   0        0        0      692 2023-04-25 21:47:29.004786 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/machinelearning_pipeline.cwl
+-rw-r--r--   0        0        0    12405 2023-04-25 21:47:29.004908 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/out.PNG
+-rw-r--r--   0        0        0     1517 2023-04-25 21:47:29.005030 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_code.py
+-rw-r--r--   0        0        0      336 2023-04-25 21:47:29.005110 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_tool.cwl
+-rw-r--r--   0        0        0     1054 2023-04-25 21:47:29.005209 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset.py
+-rw-r--r--   0        0        0      235 2023-04-25 21:47:29.005315 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset_tool.cwl
+-rw-r--r--   0        0        0      239 2023-04-25 21:47:29.005398 hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/regress_tool.cwl
+-rw-r--r--   0        0        0       80 2023-04-25 21:47:29.005519 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.builder_demo
+-rw-r--r--   0        0        0      411 2023-04-25 21:47:29.005642 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.clamr-ffmpeg
+-rw-r--r--   0        0        0      145 2023-04-25 21:47:29.005725 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.clamr-lanl-x86_64
+-rw-r--r--   0        0        0      724 2023-04-25 21:47:29.005802 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le
+-rw-r--r--   0        0        0     2303 2023-04-25 21:47:29.005907 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.comd-x86_64
+-rw-r--r--   0        0        0      270 2023-04-25 21:47:29.005992 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.deb9ompi-x86_64
+-rw-r--r--   0        0        0     2592 2023-04-25 21:47:29.006062 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64
+-rw-r--r--   0        0        0     1605 2023-04-25 21:47:29.006164 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le
+-rw-r--r--   0        0        0     2489 2023-04-25 21:47:29.006269 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64
+-rw-r--r--   0        0        0     3446 2023-04-25 21:47:29.006374 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64
+-rw-r--r--   0        0        0      614 2023-04-25 21:47:29.006482 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/README.md
+-rw-r--r--   0        0        0      331 2023-04-25 21:47:29.006618 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.comd-x86_64-wpmix
+-rw-r--r--   0        0        0      573 2023-04-25 21:47:29.006711 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian
+-rw-r--r--   0        0        0     3941 2023-04-25 21:47:29.006821 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5
+-rw-r--r--   0        0        0      509 2023-04-25 21:47:29.006927 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/comd-pmix-support/README.md
+-rw-r--r--   0        0        0      813 2023-04-25 21:47:29.007028 hpc_beeflow-0.1.4/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch
+-rw-r--r--   0        0        0      640 2023-04-25 21:47:29.007462 hpc_beeflow-0.1.4/beeflow/enhanced_client/README.rst
+-rw-r--r--   0        0        0        0 2023-04-25 21:47:29.007581 hpc_beeflow-0.1.4/beeflow/enhanced_client/data/.gitkeep
+-rw-r--r--   0        0        0      386 2023-04-25 21:47:29.007687 hpc_beeflow-0.1.4/beeflow/enhanced_client/forge.config.js
+-rw-r--r--   0        0        0     1682 2023-04-25 21:47:29.007800 hpc_beeflow-0.1.4/beeflow/enhanced_client/main.js
+-rw-r--r--   0        0        0   277089 2023-04-25 21:47:29.008549 hpc_beeflow-0.1.4/beeflow/enhanced_client/package-lock.json
+-rw-r--r--   0        0        0     1078 2023-04-25 21:47:29.008694 hpc_beeflow-0.1.4/beeflow/enhanced_client/package.json
+-rw-r--r--   0        0        0     1219 2023-04-25 21:47:29.008916 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/app.js
+-rw-r--r--   0        0        0     5151 2023-04-25 21:47:29.009061 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/client.js
+-rw-r--r--   0        0        0      872 2023-04-25 21:47:29.009162 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/config.js
+-rw-r--r--   0        0        0     2013 2023-04-25 21:47:29.009273 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/control.js
+-rw-r--r--   0        0        0     3610 2023-04-25 21:47:29.009393 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/database.js
+-rw-r--r--   0        0        0    12140 2023-04-25 21:47:29.009519 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/display.js
+-rw-r--r--   0        0        0      455 2023-04-25 21:47:29.009613 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/gdb.js
+-rw-r--r--   0        0        0    33601 2023-04-25 21:47:29.009934 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/img/logo.png
+-rw-r--r--   0        0        0     2751 2023-04-25 21:47:29.010080 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/main.html
+-rw-r--r--   0        0        0   206620 2023-04-25 21:47:29.010757 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/styles/bulma.min.css
+-rw-r--r--   0        0        0      374 2023-04-25 21:47:29.010868 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/styles/main.css
+-rw-r--r--   0        0        0      498 2023-04-25 21:47:29.010960 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/tunnel.js
+-rw-r--r--   0        0        0      428 2023-04-25 21:47:29.011047 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/viz.html
+-rw-r--r--   0        0        0     1071 2023-04-25 21:47:29.011146 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/viz.js
+-rw-r--r--   0        0        0     7603 2023-04-25 21:47:29.011257 hpc_beeflow-0.1.4/beeflow/enhanced_client/renderer/workflows.js
+-rw-r--r--   0        0        0     1708 2023-04-25 21:47:29.011551 hpc_beeflow-0.1.4/beeflow/scheduler/README.md
+-rw-r--r--   0        0        0    10098 2023-04-25 21:47:29.011762 hpc_beeflow-0.1.4/beeflow/scheduler/algorithms.py
+-rw-r--r--   0        0        0     9347 2023-04-25 21:47:29.011888 hpc_beeflow-0.1.4/beeflow/scheduler/resource_allocation.py
+-rw-r--r--   0        0        0     3984 2023-04-25 21:47:29.011986 hpc_beeflow-0.1.4/beeflow/scheduler/scheduler.py
+-rw-r--r--   0        0        0     2890 2023-04-25 21:47:29.012145 hpc_beeflow-0.1.4/beeflow/scheduler/scheduler.yaml
+-rw-r--r--   0        0        0      708 2023-04-25 21:47:29.012263 hpc_beeflow-0.1.4/beeflow/scheduler/serializable.py
+-rw-r--r--   0        0        0     2296 2023-04-25 21:47:29.012364 hpc_beeflow-0.1.4/beeflow/scheduler/task.py
+-rwxr-xr-x   0        0        0    12841 2023-05-09 22:30:18.857330 hpc_beeflow-0.1.4/beeflow/task_manager.py
+-rw-r--r--   0        0        0    34925 2023-04-25 21:47:29.012805 hpc_beeflow-0.1.4/beeflow/tests/42.tgz
+-rw-r--r--   0        0        0      236 2023-04-25 21:47:29.012980 hpc_beeflow-0.1.4/beeflow/tests/README.md
+-rw-r--r--   0        0        0     1139 2023-04-25 21:47:29.013070 hpc_beeflow-0.1.4/beeflow/tests/cf.cwl
+-rw-r--r--   0        0        0     1093 2023-04-25 21:47:29.013282 hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/clamr.cwl
+-rw-r--r--   0        0        0      302 2023-04-25 21:47:29.013394 hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/clamr_job.json
+-rw-r--r--   0        0        0      424 2023-04-25 21:47:29.013478 hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/clamr_job.yml
+-rw-r--r--   0        0        0     1320 2023-04-25 21:47:29.013567 hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/clamr_wf.cwl
+-rw-r--r--   0        0        0      680 2023-04-25 21:47:29.013641 hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/ffmpeg.cwl
+-rw-r--r--   0        0        0      273 2023-04-25 21:47:29.013735 hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/mv_script.cwl
+-rwxr-xr-x   0        0        0      324 2023-04-25 21:47:29.013817 hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/mv_script.sh
+-rw-r--r--   0        0        0     2401 2023-04-25 21:47:29.013156 hpc_beeflow-0.1.4/beeflow/tests/clamr-wf.tgz
+-rw-r--r--   0        0        0      774 2023-04-25 21:47:29.013918 hpc_beeflow-0.1.4/beeflow/tests/gdb.py
+-rw-r--r--   0        0        0    12378 2023-04-25 21:47:29.014045 hpc_beeflow-0.1.4/beeflow/tests/mocks.py
+-rw-r--r--   0        0        0      267 2023-04-25 21:47:29.014151 hpc_beeflow-0.1.4/beeflow/tests/test_cloud.py
+-rw-r--r--   0        0        0     6006 2023-04-25 21:47:29.014267 hpc_beeflow-0.1.4/beeflow/tests/test_config_validator.py
+-rw-r--r--   0        0        0      807 2023-04-25 21:47:29.014348 hpc_beeflow-0.1.4/beeflow/tests/test_container_path.py
+-rw-r--r--   0        0        0      946 2023-04-25 21:47:29.014440 hpc_beeflow-0.1.4/beeflow/tests/test_db_sched.py
+-rw-r--r--   0        0        0     4410 2023-04-25 21:47:29.014548 hpc_beeflow-0.1.4/beeflow/tests/test_db_tm.py
+-rw-r--r--   0        0        0     2286 2023-04-25 21:47:29.014659 hpc_beeflow-0.1.4/beeflow/tests/test_parser.py
+-rw-r--r--   0        0        0    15134 2023-04-25 21:47:29.014766 hpc_beeflow-0.1.4/beeflow/tests/test_scheduler.py
+-rw-r--r--   0        0        0     2630 2023-04-25 21:47:29.014849 hpc_beeflow-0.1.4/beeflow/tests/test_scheduler_resource_allocation.py
+-rw-r--r--   0        0        0     6557 2023-04-25 21:47:29.014958 hpc_beeflow-0.1.4/beeflow/tests/test_scheduler_rest.py
+-rw-r--r--   0        0        0     4840 2023-05-05 17:47:06.280350 hpc_beeflow-0.1.4/beeflow/tests/test_slurm_worker.py
+-rw-r--r--   0        0        0     3704 2023-04-25 21:47:29.015183 hpc_beeflow-0.1.4/beeflow/tests/test_tm.py
+-rw-r--r--   0        0        0    30958 2023-04-25 21:47:29.015358 hpc_beeflow-0.1.4/beeflow/tests/test_wf_interface.py
+-rw-r--r--   0        0        0     8850 2023-04-25 21:47:29.015504 hpc_beeflow-0.1.4/beeflow/tests/test_wf_manager.py
+-rwxr-xr-x   0        0        0     7935 2023-04-25 21:47:29.015709 hpc_beeflow-0.1.4/beeflow/wf_manager/common/dep_manager.py
+-rw-r--r--   0        0        0     9282 2023-04-25 21:47:29.015817 hpc_beeflow-0.1.4/beeflow/wf_manager/common/wf_db.py
+-rw-r--r--   0        0        0     4286 2023-04-25 21:47:29.015970 hpc_beeflow-0.1.4/beeflow/wf_manager/resources/wf_actions.py
+-rw-r--r--   0        0        0     8423 2023-04-25 21:47:29.016143 hpc_beeflow-0.1.4/beeflow/wf_manager/resources/wf_list.py
+-rw-r--r--   0        0        0      560 2023-04-25 21:47:29.016239 hpc_beeflow-0.1.4/beeflow/wf_manager/resources/wf_metadata.py
+-rw-r--r--   0        0        0     5477 2023-05-05 17:47:06.280542 hpc_beeflow-0.1.4/beeflow/wf_manager/resources/wf_update.py
+-rw-r--r--   0        0        0     7938 2023-04-25 21:47:29.016450 hpc_beeflow-0.1.4/beeflow/wf_manager/resources/wf_utils.py
+-rw-r--r--   0        0        0     1192 2023-04-25 21:47:29.016542 hpc_beeflow-0.1.4/beeflow/wf_manager/wf_manager.py
+-rw-r--r--   0        0        0     2699 2023-05-11 21:24:08.023456 hpc_beeflow-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6989 1970-01-01 00:00:00.000000 hpc_beeflow-0.1.4/PKG-INFO
```

### Comparing `hpc-beeflow-0.1.3/LICENSE` & `hpc_beeflow-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/README.rst` & `hpc_beeflow-0.1.4/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -31,14 +31,37 @@
 Contact
 =======
 
 
 For bugs and problems report, suggestions and other general questions regarding the BEE project, email questions to `bee-dev@lanl.gov <bee-dev@lanl.gov>`_.
 
 
+Contributors:
+==========================
+
+* Steven Anaya - `Boogie3D <https://github.com/Boogie3D>`_
+* Paul Bryant - `paulbry <https://github.com/paulbry>`_
+* Rusty Davis - `rstyd <https://github.com/rstyd>`_
+* Jieyang Chen - `JieyangChen7 <https://github.com/JieyangChen7>`_
+* Patricia Grubel - `pagrubel <https://github.com/pagrubel>`_
+* Qiang Guan - `guanxyz <https://github.com/guanxyz>`_
+* Ragini Gupta - `raginigupta6 <https://github.com/raginigupta6>`_
+* Andres Quan - `aquan9 <https://github.com/aquan9>`_
+* Quincy Wofford - `qwofford <https://github.com/qwofford>`_
+* Tim Randles - `trandles-lanl <https://github.com/trandles-lanl>`_
+* Jacob Tronge - `jtronge <https://github.com/jtronge>`_
+
+Concept and Design Contributors
+
+* James Ahrens
+* Allen McPherson
+* Li-Ta Lo
+* Louis Vernon
+
+
 Contributing
 ==========================
 
 The BEE project adheres to style guidelines specified in `setup.cfg <https://github.com/lanl/BEE/blob/master/setup\.cfg>`_. Before attempting to commit and push changes, please install our pre-commit githooks by running the following command in project root:
 
 If using `git --version` >= 2.9:
     git config core.hooksPath .githooks
```

### Comparing `hpc-beeflow-0.1.3/beeflow/cli.py` & `hpc_beeflow-0.1.4/beeflow/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 import daemon
 import typer
 
 from beeflow.common.config_driver import BeeConfig as bc
 from beeflow.common import cli_connection
 
 
+bc.init()
+# Max number of times a component can be restarted
+MAX_RESTARTS = bc.get('DEFAULT', 'max_restarts')
+
+
 class ComponentManager:
     """Component manager class."""
 
     def __init__(self):
         """Construct the component manager."""
         self.components = {}
         self.procs = {}
@@ -36,14 +41,16 @@
         """Return a decorator function to be called."""
 
         def wrap(fn):
             """Add the component to the list."""
             self.components[name] = {
                 'fn': fn,
                 'deps': deps,
+                'restart_count': 0,
+                'failed': False,
             }
 
         return wrap
 
     def _validate(self, base_components):
         """Make sure that the components all exist and have valid deps."""
         missing = [name for name in base_components if name not in self.components]
@@ -83,20 +90,32 @@
         print(f'Launching components in order: {order}')
         # Now launch the components
         for name in order:
             component = self.components[name]
             self.procs[name] = component['fn']()
 
     def poll(self):
-        """Poll each process to check for errors."""
-        for name, proc in self.procs.items():
-            returncode = proc.poll()
+        """Poll each process to check for errors, restart failed processes."""
+        for name in self.procs:  # noqa no need to iterate with items() since self.procs may be set
+            component = self.components[name]
+            if component['failed']:
+                continue
+            returncode = self.procs[name].poll()
             if returncode is not None:
                 log = log_fname(name)
                 print(f'Component "{name}" failed, check log "{log}"')
+                if component['restart_count'] >= MAX_RESTARTS:
+                    print(f'Component "{name}" has been restarted {MAX_RESTARTS} '
+                          'times, not restarting again')
+                    component['failed'] = True
+                else:
+                    restart_count = component['restart_count']
+                    print(f'Attempting restart {restart_count} of "{name}"...')
+                    self.procs[name] = component['fn']()
+                    component['restart_count'] += 1
 
     def status(self):
         """Return the statuses for each process in a dict."""
         return {
             name: 'RUNNING' if proc.poll() is None else 'FAILED'
             for name, proc in self.procs.items()
         }
@@ -136,24 +155,35 @@
 
 def open_log(component):
     """Determine the log for the component, open and return it."""
     log = log_fname(component)
     return open(log, 'a', encoding='utf-8')
 
 
+# Slurmrestd will be started only if we're running with Slurm and
+# slurm::use_commands is not True
+NEED_SLURMRESTD = (bc.get('DEFAULT', 'workload_scheduler') == 'Slurm'
+                   and not bc.get('slurm', 'use_commands'))
+
+
 @MGR.component('wf_manager', ('scheduler',))
 def start_wfm():
     """Start the WFM."""
     fp = open_log('wf_manager')
     sock_path = bc.get('workflow_manager', 'socket')
     return launch_with_gunicorn('beeflow.wf_manager.wf_manager:create_app()',
                                 sock_path, stdout=fp, stderr=fp)
 
 
-@MGR.component('task_manager', ('slurmrestd',))
+TM_DEPS = []
+if NEED_SLURMRESTD:
+    TM_DEPS.append('slurmrestd')
+
+
+@MGR.component('task_manager', TM_DEPS)
 def start_task_manager():
     """Start the TM."""
     fp = open_log('task_manager')
     sock_path = bc.get('task_manager', 'socket')
     return launch_with_gunicorn('beeflow.task_manager:flask_app', sock_path, stdout=fp, stderr=fp)
 
 
@@ -164,39 +194,40 @@
     sock_path = bc.get('scheduler', 'socket')
     # Using a function here because of the funny way that the scheduler's written
     return launch_with_gunicorn('beeflow.scheduler.scheduler:create_app()', sock_path, stdout=fp,
                                 stderr=fp)
 
 
 # Workflow manager and task manager need to be opened with PIPE for their stdout/stderr
-@MGR.component('slurmrestd')
-def start_slurm_restd():
-    """Start BEESlurmRestD. Returns a Popen process object."""
-    bee_workdir = bc.get('DEFAULT', 'bee_workdir')
-    slurmrestd_log = '/'.join([bee_workdir, 'logs', 'restd.log'])
-    slurm_socket = bc.get('slurmrestd', 'slurm_socket')
-    slurm_args = bc.get('slurmrestd', 'slurm_args')
-    slurm_args = slurm_args if slurm_args is not None else ''
-    subprocess.run(['rm', '-f', slurm_socket], check=True)
-    # log.info("Attempting to open socket: {}".format(slurm_socket))
-    fp = open(slurmrestd_log, 'w', encoding='utf-8') # noqa
-    cmd = ['slurmrestd']
-    cmd.extend(slurm_args.split())
-    cmd.append(f'unix:{slurm_socket}')
-    return subprocess.Popen(cmd, stdout=fp, stderr=fp)
+if NEED_SLURMRESTD:
+    @MGR.component('slurmrestd')
+    def start_slurm_restd():
+        """Start BEESlurmRestD. Returns a Popen process object."""
+        bee_workdir = bc.get('DEFAULT', 'bee_workdir')
+        slurmrestd_log = '/'.join([bee_workdir, 'logs', 'restd.log'])
+        slurm_socket = bc.get('slurm', 'slurmrestd_socket')
+        openapi_version = bc.get('slurm', 'openapi_version')
+        slurm_args = f'-s openapi/{openapi_version}'
+        subprocess.run(['rm', '-f', slurm_socket], check=True)
+        # log.info("Attempting to open socket: {}".format(slurm_socket))
+        fp = open(slurmrestd_log, 'w', encoding='utf-8') # noqa
+        cmd = ['slurmrestd']
+        cmd.extend(slurm_args.split())
+        cmd.append(f'unix:{slurm_socket}')
+        return subprocess.Popen(cmd, stdout=fp, stderr=fp)
 
 
 def handle_terminate(signum, stack): # noqa
     """Handle a terminate signal."""
     # Kill all subprocesses
     MGR.kill()
     sys.exit(1)
 
 
-MIN_CHARLIECLOUD_VERSION = (0, 27)
+MIN_CHARLIECLOUD_VERSION = (0, 32)
 
 
 def version_str(version):
     """Convert a version tuple to a string."""
     return '.'.join([str(part) for part in version])
 
 
@@ -284,21 +315,29 @@
 @app.command()
 def start(foreground: bool = typer.Option(False, '--foreground', '-F',
           help='run in the foreground')):
     """Attempt to daemonize if not in debug and start all BEE components."""
     beeflow_log = log_fname('beeflow')
     check_dependencies()
     sock_path = bc.get('DEFAULT', 'beeflow_socket')
+    if bc.get('DEFAULT', 'workload_scheduler') == 'Slurm' and not NEED_SLURMRESTD:
+        warn('Not using slurmrestd. Command-line interface will be used.')
     # Note: there is a possible race condition here, however unlikely
     if os.path.exists(sock_path):
         # Try to contact for a status
-        resp = cli_connection.send(sock_path, {'type': 'status'})
+        try:
+            resp = cli_connection.send(sock_path, {'type': 'status'})
+        except (ConnectionResetError, ConnectionRefusedError):
+            resp = None
         if resp is None:
             # Must be dead, so remove the socket path
-            os.remove(sock_path)
+            try:
+                os.remove(sock_path)
+            except FileNotFoundError:
+                pass
         else:
             # It's already running, so print an error and exit
             warn(f'Beeflow appears to be running. Check the beeflow log: "{beeflow_log}"')
             sys.exit(1)
     print('Starting beeflow...')
     if not foreground:
         print(f'Check "{beeflow_log}" or run `beeflow status` for more information.')
@@ -348,25 +387,32 @@
              f'       Check the beeflow log: "{beeflow_log}".')
         sys.exit(1)
     # As long as it returned something, we should be good
     beeflow_log = log_fname('beeflow')
     print(f'Beeflow has stopped. Check the log at "{beeflow_log}".')
 
 
+@app.command()
+def restart(foreground: bool = typer.Option(False, '--foreground', '-F',
+            help='run in the foreground')):
+    """Attempt to stop and restart the beeflow daemon."""
+    stop()
+    start(foreground)
+
+
 @app.callback(invoke_without_command=True)
 def version_callback(version: bool = False):
     """Beeflow."""
     # Print out the current version of the app, and then exit
     # Note above docstring gets used in the help menu
     if version:
         version = importlib.metadata.version("hpc-beeflow")
         print(version)
 
 
 def main():
     """Start the beeflow app."""
-    bc.init()
     app()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `hpc-beeflow-0.1.3/beeflow/client/bee_client.py` & `hpc_beeflow-0.1.4/beeflow/client/bee_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import sys
 import logging
 import inspect
 import pathlib
 import shutil
 import subprocess
+import tempfile
 import textwrap
 import time
 import jsonpickle
 import requests
 import typer
 
 from beeflow.common.config_driver import BeeConfig as bc
@@ -53,15 +54,15 @@
         typer.secho(msg, fg=typer.colors.RED, file=sys.stderr)
         sys.exit(1)
     else:
         # Raise an error so that client libraries can handle it
         raise ClientError(msg) from None
 
 
-def error_handler(resp): # noqa (this is an error handler, it doesn't need to return an expression)
+def error_handler(resp):  # noqa (this is an error handler, it doesn't need to return an expression)
     """Handle a 500 error in a response."""
     if resp.status_code != 500:
         return resp
     data = resp.json()
     if 'error' not in data:
         return resp
     error = data['error']
@@ -162,30 +163,60 @@
     return None
 
 
 app = typer.Typer(no_args_is_help=True, add_completion=False, cls=NaturalOrderGroup)
 
 
 @app.command()
-def submit(wf_name: str = typer.Argument(..., help='The workflow name'),
-           wf_path: pathlib.Path = typer.Argument(..., help='Path to the workflow .tgz or dir'),
+def submit(wf_name: str = typer.Argument(..., help='the workflow name'),  # pylint:disable=R0915
+           wf_path: pathlib.Path = typer.Argument(..., help='path to the workflow .tgz or dir'),
            main_cwl: str = typer.Argument(..., help='filename of main CWL file'),
            yaml: str = typer.Argument(..., help='filename of YAML file'),
            workdir: pathlib.Path = typer.Argument(...,
-           help='working directory for workflow containing input + output files',)):
+           help='working directory for workflow containing input + output files',),
+           no_start: bool = typer.Option(False, '--no-start', '-n',
+                                         help='do not start the workflow')):
     """Submit a new workflow."""
+    def is_parent(parent, path):
+        """Return true if the path is a child of the other path."""
+        parent = os.path.abspath(parent)
+        path = os.path.abspath(path)
+        return os.path.commonpath([parent]) == os.path.commonpath([parent, path])
+
     tarball_path = ""
     if os.path.exists(wf_path):
         # Check to see if the wf_path is a tarball or a directory. Run package() if directory
         if os.path.isdir(wf_path):
             print("Detected directory instead of packaged workflow. Packaging Directory...")
-            bee_workdir = bc.get('DEFAULT', 'bee_workdir')
-            package(wf_path, pathlib.Path(bee_workdir))
-            tarball_path = pathlib.Path(bee_workdir + "/" + str(wf_path.name) + ".tgz")
-            wf_tarball = open(tarball_path, 'rb')
+            main_cwl_path = pathlib.Path(main_cwl).resolve()
+            yaml_path = pathlib.Path(yaml).resolve()
+
+            if not main_cwl_path.exists():
+                error_exit(f'Main CWL file {main_cwl} does not exist')
+            if not yaml_path.exists():
+                error_exit(f'YAML file {yaml} does not exist')
+
+            cwl_indir = is_parent(wf_path, main_cwl_path)
+            yaml_indir = is_parent(wf_path, yaml_path)
+            # The CWL and YAML file are already in the workflow directory
+            # so we don't need to do anything
+            tempdir_path = pathlib.Path(tempfile.mkdtemp())
+            if cwl_indir and yaml_indir:
+                package_path = package(wf_path, tempdir_path)
+            else:
+                # Create a temp wf directory
+                tempdir_wf_path = pathlib.Path(tempdir_path / wf_path.name)
+                shutil.copytree(wf_path, tempdir_wf_path, dirs_exist_ok=False)
+                if not cwl_indir:
+                    shutil.copy2(main_cwl, tempdir_wf_path)
+                if not yaml_indir:
+                    shutil.copy2(yaml, tempdir_wf_path)
+                package_path = package(tempdir_wf_path, tempdir_path)
+            wf_tarball = open(package_path, 'rb')
+            shutil.rmtree(tempdir_path)
         else:
             wf_tarball = open(wf_path, 'rb')
     else:
         error_exit(f'Workflow tarball {wf_path} cannot be found')
 
     # Make sure the workdir is an absolute path and exists
     workdir = os.path.expanduser(workdir)
@@ -193,16 +224,16 @@
     if not os.path.exists(workdir):
         error_exit(f"Workflow working directory \"{workdir}\" doesn't exist")
 
     # TODO: Can all of this information be sent as a file?
     data = {
         'wf_name': wf_name.encode(),
         'wf_filename': os.path.basename(wf_path).encode(),
-        'main_cwl': main_cwl,
-        'yaml': yaml,
+        'main_cwl': os.path.basename(main_cwl),
+        'yaml': os.path.basename(yaml),
         'workdir': workdir
     }
     files = {
         'workflow_archive': wf_tarball
     }
     try:
         conn = _wfm_conn()
@@ -223,28 +254,36 @@
     typer.secho("Workflow submitted! Your workflow id is "
                 f"{_short_id(wf_id)}.", fg=typer.colors.GREEN)
     logging.info('Sumit workflow:  {resp.text}')
 
     # Cleanup code
     if tarball_path:
         os.remove(tarball_path)
+
+    # Start the workflow
+    if not no_start:
+        start(wf_id)
+
     return wf_id
 
 
 @app.command()
 def start(wf_id: str = typer.Argument(..., callback=match_short_id)):
     """Start a workflow with a workflow ID."""
     long_wf_id = wf_id
     try:
         conn = _wfm_conn()
         resp = conn.post(_resource(long_wf_id), timeout=60)
     except requests.exceptions.ConnectionError:
         error_exit('Could not reach WF Manager.')
 
-    if resp.status_code != requests.codes.okay:  # pylint: disable=no-member
+    if resp.status_code == 400:
+        error_exit("Could not start workflow. It may have already been started "
+                   "and ran to completion (or failure).")
+    elif resp.status_code != requests.codes.okay:  # pylint: disable=no-member
         error_exit(f"Starting {long_wf_id} failed."
                    f" Returned {resp.status_code}")
 
     typer.echo(f"{resp.json()['msg']}")
     logging.info('Started  {resp.text}')
 
 
@@ -276,14 +315,16 @@
         shutil.move(tarball_path, package_path)
 
     if return_code != 0:
         error_exit("Package failed")
     else:
         print(f"Package {tarball} created successfully")
 
+    return package_path
+
 
 @app.command()
 def listall():
     """List all worklfows."""
     try:
         conn = _wfm_conn()
         resp = conn.get(_url(), timeout=60)
@@ -314,29 +355,48 @@
     try:
         conn = _wfm_conn()
         resp = conn.get(_resource(long_wf_id), timeout=60)
     except requests.exceptions.ConnectionError:
         error_exit('Could not reach WF Manager.')
 
     if resp.status_code != requests.codes.okay:  # pylint: disable=no-member
-        error_exit('Could sucessfully query workflow manager')
+        error_exit('Could not successfully query workflow manager')
 
     tasks_status = resp.json()['tasks_status']
     wf_status = resp.json()['wf_status']
     if tasks_status == 'Unavailable':
         typer.echo(wf_status)
     else:
         typer.echo(wf_status)
         typer.echo(tasks_status)
 
     logging.info('Query workflow:  {resp.text}')
     return wf_status, tasks_status
 
 
 @app.command()
+def metadata(wf_id: str = typer.Argument(..., callback=match_short_id)):
+    """Get metadata about a given workflow."""
+    try:
+        conn = _wfm_conn()
+        resp = conn.get(_resource(wf_id) + '/metadata', timeout=60)
+    except requests.exceptions.ConnectionError:
+        error_exit('Could not reach WF Manager.')
+
+    if resp.status_code != requests.codes.okay:  # noqa (pylama doesn't know about the okay member)
+        error_exit('Could not successfully query workflow manager')
+
+    # Print and or return the metadata
+    data = resp.json()
+    for key, value in data.items():
+        typer.echo(f'{key} = {value}')
+    return data
+
+
+@app.command()
 def pause(wf_id: str = typer.Argument(..., callback=match_short_id)):
     """Pause a workflow (Running tasks will finish)."""
     long_wf_id = wf_id
     try:
         conn = _wfm_conn()
         resp = conn.patch(_resource(long_wf_id), json={'option': 'pause'},
                           timeout=60)
@@ -437,12 +497,10 @@
     bc.init()
     app()
 
 
 if __name__ == "__main__":
     app()
 
-# Pylint is reporting no member for requests.codes even when they exist
-#     ignoring them line by line
-# Ignore using with for open files; used to send command.
-# Ignore W0511: This is a TODO that should be addressed later
-# pylama:ignore=R1732,W0511
+# Ignore W0511: This allows us to have TODOs in the code
+# Ignore R1732: Significant code restructuring required to fix
+# pylama:ignore=W0511,R1732
```

### Comparing `hpc-beeflow-0.1.3/beeflow/cloud_launcher.py` & `hpc_beeflow-0.1.4/beeflow/cloud_launcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -201,12 +201,10 @@
                 bee_user=bee_user, head_node=head_node,
                 wfm_listen_port=wfm_listen_port, tm_listen_port=tm_listen_port,
                 max_retries=args.max_retries)
 
 
 if __name__ == '__main__':
     main()
-# Ignore R1732: Using a 'with' statement for resource allocation doesn't really apply here. We'd
-#               need to completely restructure the code to use it, but it's something to think
-#               about later on.
-# Ignore W0511: This TODO needs to be addressed later on, perhaps with a restructure of this code.
-# pylama:ignore=R1732,W0511
+# Ignore R1732: Significant code restructuring required to fix
+# Ignore W0511: This allows us to have TODOs in the code
+# pylama:ignore=W0511,R1732
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/build/README.md` & `hpc_beeflow-0.1.4/beeflow/common/build/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/build/build_driver.py` & `hpc_beeflow-0.1.4/beeflow/common/build/build_driver.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/build/container_drivers.py` & `hpc_beeflow-0.1.4/beeflow/common/build/container_drivers.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,16 @@
 
     def __init__(self, task):
         """Begin build request.
 
         Parse hints and requirements to determine target build
         system. Harvest relevant BeeConfig params in kwargs.
 
-        :param requirements: the workflow requirements
-        :type requirements: set of Requirement instances
-        :param hints: the workflow hints (optional requirements)
-        :type hints: set of Requirement instances
-        :param kwargs: Dictionary of build system config options
-        :type kwargs: set of build system parameters
+        :param task: the task to build for
+        :type task: Task
         """
         # Store build container archive pased on config file or relative to bee_workdir if not set.
         container_archive = bc.get('builder', 'container_archive')
         self.container_archive = bc.resolve_path(container_archive)
         os.makedirs(self.container_archive, exist_ok=True)
         # Deploy build tarballs relative to /var/tmp/username/beeflow by default
         deployed_image_root = bc.get('builder', 'deployed_image_root')
@@ -218,23 +214,26 @@
             except FileNotFoundError:
                 pass
             try:
                 shutil.rmtree('/var/tmp/' + os.getlogin() + '/ch-image/' + ch_build_addr)
             except FileNotFoundError:
                 pass
 
+        # Get the force type (uses seccomp by default)
+        force_type = self.task.get_requirement('DockerRequirement', 'beeflow:forceType', 'seccomp')
+
         # Out of excuses. Build the image.
         with tempfile.NamedTemporaryFile(mode='w+', encoding='utf-8') as tmp:
             # Write the dockerfile to the tempfile
             tmp.write(task_dockerfile)
             tmp.flush()
             dockerfile_path = tmp.name
             # Build and run the command
             log.info('Context directory configured. Beginning build.')
-            cmd = (f'ch-image build -t {self.container_name} --force '
+            cmd = (f'ch-image build -t {self.container_name} --force {force_type} '
                    f'-f {dockerfile_path} {context_dir}\n'
                    f'ch-convert -i ch-image -o tar {ch_build_addr} '
                    f'{self.container_archive}/{ch_build_addr}.tar.gz'
                    )
             log.info(f'Executing: {cmd}')
             return subprocess.run(cmd, check=True, shell=True)
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/build_interfaces.py` & `hpc_beeflow-0.1.4/beeflow/common/build_interfaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,8 +78,9 @@
         local_task = arg2task(my_args)
     except Exception as err:
         log.info(f'{err}')
 
     build_main(local_task)
 
 # Ignore W0703: Catching generic exception isn't a problem if we just want a descriptive report
-# pylama:ignore=W0703
+# Ignore C901: "'build_main' is too complex" - this function is just around 40 lines
+# pylama:ignore=W0703,C901
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/cli_connection.py` & `hpc_beeflow-0.1.4/beeflow/common/cli_connection.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/cloud/README.md` & `hpc_beeflow-0.1.4/beeflow/common/cloud/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/cloud/__init__.py` & `hpc_beeflow-0.1.4/beeflow/common/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/cloud/chameleoncloud.py` & `hpc_beeflow-0.1.4/beeflow/common/cloud/chameleoncloud.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/cloud/google.py` & `hpc_beeflow-0.1.4/beeflow/common/cloud/google.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,30 +15,27 @@
         self.zone = zone
         self.project = project
         # Set defaults here for now
         self._api = googleapiclient.discovery.build('compute', 'v1')
 
     def get_ext_ip_addr(self, node_name):
         """Get the external IP of this node (or None if no IP)."""
-        res = self._api.instances().get(instance=node_name,
+        res = self._api.instances().get(instance=node_name,  # noqa (can't find instances member)
                                         project=self.project,
                                         zone=self.zone).execute()
         try:
             return res['networkInterfaces'][0]['accessConfigs'][0]['natIP']
         except (IndexError, KeyError):
             return None
 
     def setup_cloud(self, config):
         """Set up the cloud based on the config information."""
         # Load the YAML data
         config = yaml.load(config, Loader=yaml.Loader)
         # This just creates instances one-by-one. There may be a better API call
         # to just create everything at once.
         for instance in config['instances']:
-            call = self._api.instances().insert(project=self.project,
+            call = self._api.instances().insert(project=self.project,  # noqa (can't find instances member)
                                                 zone=self.zone, body=instance)
             res = call.execute()
             print(res)
             time.sleep(2)
-# Ignore E1101: Pylama notes that self._api doesn't have an 'instances' member.
-#               I believe this is set at runtime by googleapiclient.
-# pylama:ignore=E1101
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/cloud/openstack.py` & `hpc_beeflow-0.1.4/beeflow/common/cloud/openstack.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/cloud/provider.py` & `hpc_beeflow-0.1.4/beeflow/common/cloud/provider.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/config_driver.py` & `hpc_beeflow-0.1.4/beeflow/common/config_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import shutil
 import sys
 import textwrap
 import typer
 
 from beeflow.common.config_validator import ConfigValidator
 from beeflow.common.cli import NaturalOrderGroup
+from beeflow.common import validation
+from beeflow.common.tab_completion import filepath_completion
 
 
 # System specific path set up
 HOME_DIR = os.path.expanduser('~/')
 _SYSTEM = platform.system()
 if _SYSTEM == 'Linux':
     CONF_DIR = os.path.join(HOME_DIR, '.config/beeflow')
@@ -158,61 +160,14 @@
 
 def check_yes(msg):
     """Check for a y/n answer."""
     res = input(f'{msg} [y/n] ')
     return res.lower() == 'y'
 
 
-# Specialized functions for validation and config initialization
-
-def validate_path(path):
-    """Check that the path exists."""
-    path = os.path.expanduser(path)
-    if not os.path.exists(path):
-        raise ValueError(f'path "{path}" does not exist')
-    return path
-
-
-def validate_dir(path):
-    """Check that the path exists and is a directory."""
-    path = validate_path(path)
-    if not os.path.isdir(path):
-        raise ValueError('path "{path}" is not a directory')
-    return path
-
-
-def validate_make_dir(path):
-    """Check if the dir exists and if not create it."""
-    os.makedirs(path, exist_ok=True)
-    if not os.path.isdir(path):
-        raise ValueError('path "{path}" is not a directory')
-    return path
-
-
-def validate_file(path):
-    """Check that the path exists and is a file."""
-    path = validate_path(path)
-    if not os.path.isfile(path):
-        raise ValueError(f'path "{path}" is not a file')
-    return path
-
-
-def validate_nonnegative_int(value):
-    """Validate that the input is nonnegative."""
-    i = int(value)
-    if i < 0:
-        raise ValueError('the value must be nonnegative')
-    return i
-
-
-def validate_bool(value):
-    """Validate a boolean value."""
-    return str(value).lower() == 'true'
-
-
 def check_choice(msg, opts):
     """Ask the user to pick from opts."""
     while True:
         value = input(f'{msg} ({",".join(opts)})')
         if value in opts:
             return value
         print(f'ERROR: invalid option: {value}')
@@ -222,50 +177,14 @@
     """Join multiple dirnames together to form a path."""
     path = pargs[0]
     for part in pargs[1:]:
         path = os.path.join(path, part)
     return path
 
 
-def job_template_init(path, cur_opts):
-    """Job template init function.
-
-    :param path: chosen path of Jinja job template file
-    :param cur_opts: current chosen options from the config generator
-    :return: initialized Jinja template path
-    """
-    path = os.path.expanduser(path)
-    if os.path.exists(path):
-        return path
-    print('Check that options (like accounts)for your particular system are satisfied.')
-    if not check_yes(f'Do you want to write a default job template to:\n "{path}"?'):
-        return path
-    # Check for workload_scheduler in cur_opts (NB: this will need to be updated
-    # if the option name changes later on)
-    if 'DEFAULT' in cur_opts and 'workload_scheduler' in cur_opts['DEFAULT']:
-        template = cur_opts['DEFAULT']['workload_scheduler']
-    else:
-        template = check_choice('What template should be generated?', ('Slurm', 'LSF', 'Simple'))
-    template_files = {
-        'Slurm': 'slurm-submit.jinja',
-        'LSF': 'lsf-submit.jinja',
-    }
-    if template not in template_files:
-        raise NotImplementedError(f'generation of template file "{template}" is not implemented')
-    fname = template_files[template]
-    # I don't like how this is done, but there seems to be some difficulties
-    # with using the pkgutil.get_data() method and the importlib.resources
-    # module.
-    common = os.path.dirname(__file__)
-    beeflow = os.path.dirname(common)
-    file_path = join_path(beeflow, 'data', 'job_templates', fname)
-    shutil.copy(file_path, path)
-    return path
-
-
 def bee_workdir_init(path, _cur_opts):
     """BEE workdir init function.
 
     :param path: chosen path for the bee workdir
     :param _cur_opts: current chosen options form the config generator
     :return: initialized bee workdir path
     """
@@ -274,14 +193,20 @@
         return path
     if not check_yes(f'Path "{path}" does not exist.\nWould you like to create it?'):
         return path
     os.makedirs(path)
     return path
 
 
+def filepath_completion_input(*pargs, **kwargs):
+    """Input files/paths with tab completion."""
+    with filepath_completion():
+        return input(*pargs, **kwargs)
+
+
 # Below is the definition of all bee config options, defaults and requirements.
 # This will be used to validate config files on loading them in the BeeConfig
 # singleton class above.
 #
 # Set up default ports, get parent's pid to offset ports.
 # Windows note: uid method better but not available in Windows
 if platform.system() == 'Windows':
@@ -294,137 +219,152 @@
 DEFAULT_HTTPS_PORT = 7473 + OFFSET
 
 DEFAULT_WFM_PORT = 5000 + OFFSET
 DEFAULT_TM_PORT = 5050 + OFFSET
 DEFAULT_SCHED_PORT = 5100 + OFFSET
 
 SOCKET_PATH = join_path(HOME_DIR, '.beeflow', 'sockets')
-os.makedirs(SOCKET_PATH, exist_ok=True)
 DEFAULT_WFM_SOCKET = join_path(SOCKET_PATH, 'wf_manager.sock')
 DEFAULT_TM_SOCKET = join_path(SOCKET_PATH, 'task_manager.sock')
 DEFAULT_SCHED_SOCKET = join_path(SOCKET_PATH, 'scheduler.sock')
 DEFAULT_BEEFLOW_SOCKET = join_path(SOCKET_PATH, 'beeflow.sock')
 
 DEFAULT_BEE_WORKDIR = join_path(HOME_DIR, '.beeflow')
 USER = getpass.getuser()
 # Create the validator
 VALIDATOR = ConfigValidator('BEE configuration file and validation information.')
 VALIDATOR.section('DEFAULT', info='Default bee.conf configuration section.')
 VALIDATOR.option('DEFAULT', 'bee_workdir', info='main BEE workdir',
-                 attrs={'default': DEFAULT_BEE_WORKDIR}, validator=validate_make_dir)
+                 attrs={'default': DEFAULT_BEE_WORKDIR}, validator=validation.make_dir)
 VALIDATOR.option('DEFAULT', 'workload_scheduler', choices=('Slurm', 'LSF', 'Simple'),
                  info='backend workload scheduler to interact with ')
-VALIDATOR.option('DEFAULT', 'use_archive', validator=validate_bool, attrs={'default': True},
+VALIDATOR.option('DEFAULT', 'use_archive', validator=validation.bool_, attrs={'default': True},
                  info='use the BEE archiving functinality')
-VALIDATOR.option('DEFAULT', 'bee_dep_image', validator=validate_file,
-                 info='container image with BEE dependencies')
+VALIDATOR.option('DEFAULT', 'bee_dep_image', validator=validation.file_,
+                 info='container image with BEE dependencies',
+                 attrs={'input': filepath_completion_input})
 VALIDATOR.option('DEFAULT', 'beeflow_pidfile',
                  attrs={'default': join_path(DEFAULT_BEE_WORKDIR, 'beeflow.pid')},
                  info='location of beeflow pidfile')
 VALIDATOR.option('DEFAULT', 'beeflow_socket',
+                 validator=validation.parent_dir,
                  attrs={'default': DEFAULT_BEEFLOW_SOCKET},
                  info='location of beeflow socket')
+VALIDATOR.option('DEFAULT', 'max_restarts', validator=int,
+                 attrs={'default': 3},
+                 info='max number of times beeflow will restart a component on failure')
 # Workflow Manager
 VALIDATOR.section('workflow_manager', info='Workflow manager section.')
-VALIDATOR.option('workflow_manager', 'socket',
-                 attrs={'default': DEFAULT_WFM_SOCKET}, validator=str,
+VALIDATOR.option('workflow_manager', 'socket', validator=validation.parent_dir,
+                 attrs={'default': DEFAULT_WFM_SOCKET},
                  info='workflow manager port')
 # Task manager
 VALIDATOR.section('task_manager',
                   info='Task manager configuration and config of container to use.')
-VALIDATOR.option('task_manager', 'socket', attrs={'default': DEFAULT_TM_SOCKET}, validator=str,
-                 info='task manager listen port')
+VALIDATOR.option('task_manager', 'socket',
+                 attrs={'default': DEFAULT_TM_SOCKET},
+                 validator=validation.parent_dir, info='task manager listen port')
 VALIDATOR.option('task_manager', 'container_runtime', attrs={'default': 'Charliecloud'},
                  choices=('Charliecloud', 'Singularity'),
                  info='container runtime to use for configuration')
-VALIDATOR.option('task_manager', 'runner_opts', validator=str, attrs={'default': ''},
+VALIDATOR.option('task_manager', 'runner_opts', attrs={'default': ''},
                  info='special runner options to pass to the runner opts')
-# Note: I've added a special attrs keyword which can include anything. In this
-# case it's being used to store a special 'init' function that can be used to
-# initialize the parameter when a user is generating a new configuration.
-VALIDATOR.option('task_manager', 'job_template',
-                 info='job template to use for generating submission scripts',
-                 validator=validate_file,
-                 attrs={'init': job_template_init, 'default': join_path(CONF_DIR, 'submit.jinja')})
+
+# Note: The special attrs keyword can include anything. One use case is for
+# storing a special 'init' function that can be used to initialize the
+# parameter when a user is generating a new configuration.
+
 # Charliecloud (depends on task_manager::container_runtime == Charliecloud)
 VALIDATOR.section('charliecloud', info='Charliecloud configuration section.',
                   depends_on=('task_manager', 'container_runtime', 'Charliecloud'))
 VALIDATOR.option('charliecloud', 'image_mntdir', attrs={'default': join_path('/tmp', USER)},
-                 info='Charliecloud mount directory', validator=validate_make_dir)
+                 info='Charliecloud mount directory', validator=validation.make_dir)
+# General job requirements
+VALIDATOR.section('job', info='General job requirements')
+VALIDATOR.option('job', 'default_account', validator=lambda val: val.strip(),
+                 info='default account to launch jobs with (leave blank if none)')
+VALIDATOR.option('job', 'default_time_limit', validator=validation.time_limit,
+                 info='default account time limit (leave blank if none)')
+VALIDATOR.option('job', 'default_partition', validator=lambda val: val.strip(),
+                 info='default partition to run jobs on (leave blank if none)')
 
 
 def validate_chrun_opts(opts):
     """Ensure that chrun_opts don't contain options that'll conflict with BEE."""
     args = opts.split()
     if '--cd' in args or '-c' in args:
         raise ValueError('Initial working directory option (-c or --cd) conflicts with BEE. '
                          'Please make sure that you choose the correct working directory on '
                          'workflow submission.')
     return opts
 
 
-VALIDATOR.option('charliecloud', 'chrun_opts', attrs={'default': ''},
+VALIDATOR.option('charliecloud', 'chrun_opts', attrs={'default': '--home'},
                  validator=validate_chrun_opts,
                  info='extra options to pass to ch-run')
-VALIDATOR.option('charliecloud', 'setup', attrs={'default': ''}, validator=str,
+VALIDATOR.option('charliecloud', 'setup', attrs={'default': ''},
                  info='extra Charliecloud setup to put in a job script')
 # Graph Database
 VALIDATOR.section('graphdb', info='Main graph database configuration section.')
 VALIDATOR.option('graphdb', 'hostname', attrs={'default': 'localhost'},
                  info='hostname of database')
 VALIDATOR.option('graphdb', 'dbpass', attrs={'default': 'password'}, info='password for database')
 VALIDATOR.option('graphdb', 'bolt_port', attrs={'default': DEFAULT_BOLT_PORT}, validator=int,
                  info='port used for the BOLT API')
 VALIDATOR.option('graphdb', 'http_port', attrs={'default': DEFAULT_HTTP_PORT}, validator=int,
                  info='HTTP port used for the graph database')
 VALIDATOR.option('graphdb', 'https_port', attrs={'default': DEFAULT_HTTPS_PORT},
                  info='HTTPS port used for the graph database')
 VALIDATOR.option('graphdb', 'gdb_image_mntdir', attrs={'default': join_path('/tmp', USER)},
-                 info='graph database image mount directory', validator=validate_make_dir)
+                 info='graph database image mount directory', validator=validation.make_dir)
 VALIDATOR.option('graphdb', 'sleep_time', validator=int, attrs={'default': 10},
                  info='how long to wait for the graph database to come up (this can take a while, '
                       'depending on the system)')
 # Builder
 VALIDATOR.section('builder', info='General builder configuration section.')
 VALIDATOR.option('builder', 'deployed_image_root', attrs={'default': '/tmp'},
-                 info='where to deploy container images', validator=validate_make_dir)
+                 info='where to deploy container images', validator=validation.make_dir)
 VALIDATOR.option('builder', 'container_output_path', attrs={'default': '/tmp'},
-                 info='container output path', validator=validate_make_dir)
+                 info='container output path', validator=validation.make_dir)
 VALIDATOR.option('builder', 'container_archive',
                  attrs={'default': join_path(DEFAULT_BEE_WORKDIR, 'container_archive')},
                  info='container archive location')
 VALIDATOR.option('builder', 'container_type', attrs={'default': 'charliecloud'},
                  info='container type to use')
 # Slurmrestd (depends on DEFAULT:workload_scheduler == Slurm)
-VALIDATOR.section('slurmrestd', info='Configuration section for Slurmrestd.',
+VALIDATOR.section('slurm', info='Configuration section for Slurm.',
                   depends_on=('DEFAULT', 'workload_scheduler', 'Slurm'))
+VALIDATOR.option('slurm', 'use_commands', validator=validation.bool_,
+                 attrs={'default': shutil.which('slurmrestd') is None},
+                 info='if set, use slurm cli commands instead of slurmrestd')
 DEFAULT_SLURMRESTD_SOCK = join_path('/tmp', f'slurm_{USER}_{random.randint(1, 10000)}.sock')
-VALIDATOR.option('slurmrestd', 'slurm_socket', attrs={'default': DEFAULT_SLURMRESTD_SOCK},
+VALIDATOR.option('slurm', 'slurmrestd_socket', validator=validation.parent_dir,
+                 attrs={'default': DEFAULT_SLURMRESTD_SOCK},
                  info='socket location')
-VALIDATOR.option('slurmrestd', 'slurm_args', attrs={'default': '-s openapi/v0.0.35'},
-                 info='arguments for the slurmrestd binary')
+VALIDATOR.option('slurm', 'openapi_version', attrs={'default': 'v0.0.37'},
+                 info='openapi version to use for slurmrestd')
 # Scheduler
 VALIDATOR.section('scheduler', info='Scheduler configuration section.')
 VALIDATOR.option('scheduler', 'log',
                  attrs={'default': join_path(DEFAULT_BEE_WORKDIR, 'logs', 'scheduler.log')},
-                 validator=str, info='scheduler log file')
-VALIDATOR.option('scheduler', 'socket', attrs={'default': DEFAULT_SCHED_SOCKET}, validator=str,
+                 info='scheduler log file')
+VALIDATOR.option('scheduler', 'socket', validator=validation.parent_dir,
+                 attrs={'default': DEFAULT_SCHED_SOCKET},
                  info='scheduler socket')
 VALIDATOR.option('scheduler', 'alloc_logfile',
                  attrs={'default': join_path(DEFAULT_BEE_WORKDIR, 'logs', 'scheduler_alloc.log')},
-                 validator=str, info='allocation logfile, to be used for later training')
+                 info='allocation logfile, to be used for later training')
 SCHEDULER_ALGORITHMS = ('fcfs', 'backfill', 'sjf')
 VALIDATOR.option('scheduler', 'algorithm', attrs={'default': 'fcfs'}, choices=SCHEDULER_ALGORITHMS,
                  info='scheduling algorithm to use')
 VALIDATOR.option('scheduler', 'default_algorithm', attrs={'default': 'fcfs'},
                  choices=SCHEDULER_ALGORITHMS,
                  info=('default algorithm to use'))
 VALIDATOR.option('scheduler', 'workdir',
                  attrs={'default': join_path(DEFAULT_BEE_WORKDIR, 'scheduler')},
-                 validator=str,
                  info='workdir to be used for the scheduler')
 
 
 def print_wrap(text, next_line_indent=''):
     """Print while wrapping lines to make the output easier to read."""
     for line in textwrap.wrap(text, width=80, subsequent_indent=next_line_indent):
         print(line)
@@ -464,43 +404,57 @@
                 if not printed:
                     print()
                     print(f'## {sec_name}')
                     print()
                     print_wrap(section.info)
                     print()
                     printed = True
+
+                # Check for a default value
                 if option.attrs is not None and 'default' in option.attrs:
                     default = option.attrs['default']
                     if option.attrs is not None and 'init' in option.attrs:
                         value = option.attrs['init'](default, self.sections)
                     else:
                         value = option.validate(default)
                     print(f'Setting option "{opt_name}" to default value "{value}".')
                     print()
                     self.sections[sec_name][opt_name] = value
                     continue
-                value = None
-                # Input and then validate the value
-                while value is None:
-                    print_wrap(f'{opt_name} - {option.info}')
-                    if option.choices is not None:
-                        print(f'(allowed values: {",".join(option.choices)})')
-                    value = input(f'{opt_name}: ')
-                    # Call the init function if there is one
-                    if option.attrs is not None and 'init' in option.attrs:
-                        option.attrs['init'](value, self.sections)
-                    try:
-                        option.validate(value)
-                    except ValueError as err:
-                        print('ERROR:', err)
-                        value = None
+
+                # Input and validate the value
+                value = self._input_loop(opt_name, option)
+
                 print()
                 self.sections[sec_name][opt_name] = value
         return self
 
+    def _input_loop(self, opt_name, option):
+        """Run the input-validation loop."""
+        # Check if there's a special input function (this allows for tab completion)
+        inp = (option.attrs['input'] if option.attrs is not None
+               and 'input' in option.attrs else input)
+        # Start of input loop
+        value = None
+        while value is None:
+            print_wrap(f'{opt_name} - {option.info}')
+            if option.choices is not None:
+                print(f'(allowed values: {",".join(option.choices)})')
+            value = inp(f'{opt_name}: ')
+            # Call the init function if there is one
+            if option.attrs is not None and 'init' in option.attrs:
+                option.attrs['init'](value, self.sections)
+            # Validate the input
+            try:
+                option.validate(value)
+            except ValueError as err:
+                print('ERROR:', err)
+                value = None
+        return value
+
     def save(self):
         """Save the config to a file."""
         print()
         print('The following configuration options were chosen:')
         for sec_name, section in self.sections.items():
             print()
             print(f'[{sec_name}]')
@@ -523,16 +477,14 @@
                         print(f'{opt_name} = {section[opt_name]}', file=fp)
         except FileNotFoundError:
             print('Configuration file does not exist!')
         print(70 * '#')
         print('Before running BEE, check defaults in the configuration file:',
               f'\n\t{self.fname}',
               '\n ** See documentation for values you should refrain from editing! **',
-              '\n\nThe job template configured is:',
-              f'\n\t{self.sections["task_manager"]["job_template"]}',
               '\n ** Include job options (such as account) required for this system.**')
         print('\n(Try `beecfg info` to see more about each option)')
         print(70 * '#')
 
 
 app = typer.Typer(no_args_is_help=False, add_completion=False, cls=NaturalOrderGroup)
 
@@ -599,7 +551,11 @@
 def main():
     """Entry point for config validation and help."""
     app()
 
 
 if __name__ == '__main__':
     app()
+# Ignore C901: "'ConfigGenerator.choose_values' is too complex" - I disagree, if
+#              it's just based on LOC, then there are a number `print()` functions
+#              that are increasing the line count
+# pylama:ignore=C901
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/config_validator.py` & `hpc_beeflow-0.1.4/beeflow/common/config_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,7 +143,9 @@
     def validate(self, value):
         """Validate the value and return it."""
         if self.choices is not None:
             if value not in self.choices:
                 raise ValueError(f"value must be one of {self.choices}; found '{value}'")
             return value
         return self._validator(value)
+# Ignore C901: "'ConfigValidator.validate' is too complex" - this function is under 40 LOC
+# pylama:ignore=C901
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/connection.py` & `hpc_beeflow-0.1.4/beeflow/common/connection.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/container_path.py` & `hpc_beeflow-0.1.4/beeflow/common/container_path.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/crt/charliecloud_driver.py` & `hpc_beeflow-0.1.4/beeflow/common/crt/charliecloud_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Charliecloud driver as the container runtime system for tasks.
 
 Creates text for tasks using Charliecloud.
 """
 
 import os
-from beeflow.common.crt.crt_driver import (ContainerRuntimeDriver, ContainerRuntimeResult)
+from beeflow.common.crt.crt_driver import (ContainerRuntimeDriver, ContainerRuntimeResult,
+                                           Command, CommandType)
 from beeflow.common.config_driver import BeeConfig as bc
 from beeflow.common.build.build_driver import task2arg
 from beeflow.common.container_path import convert_path
 from beeflow.common import log as bee_logging
 
 
 log = bee_logging.setup(__name__)
@@ -85,15 +86,15 @@
                 baremetal = False
 
         # Set the workdir with the env code
         task_workdir_env = f'cd {task.workdir}\n' if task.workdir is not None else ''
 
         if baremetal:
             return ContainerRuntimeResult(env_code=task_workdir_env, pre_commands=[],
-                                          main_command=[str(arg) for arg in task.command],
+                                          main_command=Command([str(arg) for arg in task.command]),
                                           post_commands=[])
 
         if task_container_name:
             container_path = '/'.join([self.container_archive, task_container_name]) + '.tar.gz'
 
         # If use_container is specified, no copying is done, the file  path is used
         if use_container:
@@ -108,31 +109,33 @@
 
         hints = dict(task.hints)
         mpi_opt = '--join' if 'beeflow:MPIRequirement' in hints else ''
         command = ' '.join(task.command)
         env_code = ''.join([self.cc_setup if self.cc_setup else '', task_workdir_env])
         deployed_path = deployed_image_root + '/' + task_container_name
         pre_commands = [
-            f'mkdir -p {deployed_image_root}\n'.split(),
-            f'ch-convert -i tar -o dir {container_path} {deployed_path}\n'.split()
+            Command(f'mkdir -p {deployed_image_root}\n'.split(), CommandType.ONE_PER_NODE),
+            Command(f'ch-convert -i tar -o dir {container_path} {deployed_path}\n'.split(),
+                    CommandType.ONE_PER_NODE),
         ]
         # Need to convert the path from inside to outside base on the bind mounts
         extra_opts = ''
         if task.workdir is not None:
             # Only setting it for $HOME right now
             bind_mounts = {
                 # Charliecloud bindmounts $HOME to /home/$USER by default
                 os.getenv('HOME'): os.path.join('/home', os.getenv('USER')),
             }
             ctr_workdir_path = convert_path(task.workdir, bind_mounts)
             extra_opts = f'--cd {ctr_workdir_path}'
         main_command = (f'ch-run {mpi_opt} {deployed_path} {self.chrun_opts} '
                         f'{extra_opts} -- {command}\n').split()
+        main_command = Command(main_command)
         post_commands = [
-            f'rm -rf {deployed_path}\n'.split(),
+            Command(f'rm -rf {deployed_path}\n'.split(), type_=CommandType.ONE_PER_NODE),
         ]
         return ContainerRuntimeResult(env_code, pre_commands, main_command, post_commands)
 
     def build_text(self, userconfig, task):
         """Build text for Charliecloud batch script."""
         task_args = task2arg(task)
         text = (f'beeflow --build {userconfig} {task_args}\n')
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/crt/crt_driver.py` & `hpc_beeflow-0.1.4/beeflow/common/crt/crt_driver.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,31 @@
         """Construct the result."""
         self.env_code = env_code
         self.pre_commands = pre_commands
         self.main_command = main_command
         self.post_commands = post_commands
 
 
+class CommandType:
+    """Command types."""
+
+    DEFAULT = 'default'
+    ONE_PER_NODE = 'one-per-node'
+    ENV = 'env'
+
+
+class Command:
+    """Command in a batch script."""
+
+    def __init__(self, args, type_=CommandType.DEFAULT):
+        """Construct the command."""
+        self.args = args
+        self.type = type_
+
+
 class ContainerRuntimeDriver(ABC):
     """ContainerRuntimeDriver interface for generic container runtime."""
 
     @abstractmethod
     def run_text(self, task):
         """Create commands for job using the container runtime.
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/crt/singularity_driver.py` & `hpc_beeflow-0.1.4/beeflow/common/crt/singularity_driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Singularity driver as the container runtime system for tasks.
 
 Creates text for tasks using Singularity.
 """
 
-from beeflow.common.crt.crt_driver import (ContainerRuntimeDriver, ContainerRuntimeResult)
+from beeflow.common.crt.crt_driver import (ContainerRuntimeDriver, ContainerRuntimeResult, Command)
 from beeflow.common.build.build_driver import task2arg
 
 
 class SingularityDriver(ContainerRuntimeDriver):
     """The ContainerRuntimeDriver for Singularity as container runtime system.
 
     Creates the text for the task for using Singularity to test abstract class.
@@ -26,14 +26,15 @@
                 if task.workdir is not None:
                     argv.extend(['--pwd', task.workdir])
                 argv.append(img)
                 argv.extend(cmd_tasks)
                 main_command = argv
             except (KeyError, TypeError):
                 pass
+        main_command = Command(main_command)
         # Change to the working directory
         env_code = ''
         if task.workdir is not None:
             env_code = f'cd {task.workdir}\n'
         return ContainerRuntimeResult(env_code=env_code, pre_commands=[],
                                       main_command=main_command, post_commands=[])
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/crt_interface.py` & `hpc_beeflow-0.1.4/beeflow/common/crt_interface.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/db/sched.py` & `hpc_beeflow-0.1.4/beeflow/common/db/sched_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,58 @@
 """Scheduler database code."""
-from contextlib import contextmanager
-import sqlite3
+
 import jsonpickle
+from beeflow.common.db import bdb
 
 
 class Resources:
     """Resources wrapper class."""
 
-    def __init__(self, conn):
+    def __init__(self, db_file):
         """Create the resources class."""
-        self._conn = conn
+        self.db_file = db_file
 
     def __iter__(self):
         """Create an iterator over the resources."""
-        cur = self._conn.cursor()
-        res = cur.execute('SELECT id, resource FROM resources')
-        while True:
-            item = res.fetchone()
-            if item is None:
-                break
-            resource = jsonpickle.decode(item['resource'])
+        stmt = 'SELECT id, resource FROM resources'
+        result = bdb.getall(self.db_file, stmt)
+        for rslt in result:
+            resource = jsonpickle.decode(rslt[1])
             yield resource
 
     def extend(self, resources):
         """Add a list of new resources."""
-        cur = self._conn.cursor()
         for resource in resources:
             data = jsonpickle.encode(resource)
-            cur.execute('INSERT INTO resources (resource) VALUES (:resource)', {'resource': data})
-        self._conn.commit()
+            stmt = 'INSERT INTO resources (resource) VALUES (?)'
+            bdb.run(self.db_file, stmt, [data])
 
     def clear(self):
         """Remove all resources."""
-        cur = self._conn.cursor()
-        cur.execute('DELETE FROM resources')
-        self._conn.commit()
+        clear_stmt = 'DELETE FROM resources'
+        bdb.run(self.db_file, clear_stmt)
 
 
 class SchedDB:
     """Scheduler database."""
 
-    def __init__(self, conn):
+    def __init__(self, db_file):
         """Construct a new scheduler database connection."""
-        self._conn = conn
+        self.db_file = db_file
         self._init_tables()
 
     def _init_tables(self):
         """Initialze the scheduler tables if they don't exist."""
-        script = """CREATE TABLE IF NOT EXISTS resources(
+        resource_stmt = """CREATE TABLE IF NOT EXISTS resources(
                         id INTEGER PRIMARY KEY ASC,
                         resource TEXT);"""
-        self._conn.executescript(script)
+        bdb.create_table(self.db_file, resource_stmt)
 
     @property
     def resources(self):
         """Get resources from the database."""
-        return Resources(self._conn)
+        return Resources(self.db_file)
 
 
-@contextmanager
-def open_db(fname):
+def open_db(db_file):
     """Open and return a new database."""
-    with sqlite3.connect(fname) as conn:
-        conn.row_factory = sqlite3.Row
-        yield SchedDB(conn)
+    return SchedDB(db_file)
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/expr.py` & `hpc_beeflow-0.1.4/beeflow/common/expr.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/gdb/DESIGN.md` & `hpc_beeflow-0.1.4/beeflow/common/gdb/DESIGN.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/gdb/gdb_driver.py` & `hpc_beeflow-0.1.4/beeflow/common/gdb/gdb_driver.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/gdb/neo4j_cypher.py` & `hpc_beeflow-0.1.4/beeflow/common/gdb/neo4j_cypher.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/gdb/neo4j_driver.py` & `hpc_beeflow-0.1.4/beeflow/common/gdb/neo4j_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,8 +573,9 @@
     :param keys: the metadata keys to retrieve from the record
     :type keys: iterable of str
     :rtype: dict
     """
     rec = metadata_record["m"]
     return {key: val for key, val in rec.items() if key != "state"}
 
+# Ignore E1129: External module is missing proper resource context manager methods.
 # pylama:ignore=E1129
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/gdb_interface.py` & `hpc_beeflow-0.1.4/beeflow/common/gdb_interface.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/log.py` & `hpc_beeflow-0.1.4/beeflow/common/log.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/parser/README.md` & `hpc_beeflow-0.1.4/beeflow/common/parser/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/parser/parser.py` & `hpc_beeflow-0.1.4/beeflow/common/parser/parser.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/wf_data.py` & `hpc_beeflow-0.1.4/beeflow/common/wf_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,27 +159,29 @@
         task_id = self.generate_task_id() if new_id else self.id
         return Task(name=self.name, base_command=self.base_command,
                     hints=deepcopy(self.hints), requirements=deepcopy(self.requirements),
                     inputs=deepcopy(self.inputs), outputs=deepcopy(self.outputs),
                     stdout=self.stdout, stderr=self.stderr, workflow_id=self.workflow_id,
                     task_id=task_id, workdir=self.workdir)
 
-    def get_requirement(self, req_type, req_param):
+    def get_requirement(self, req_type, req_param, default=None):
         """Get requirement from hints or requirements, prioritizing requirements over hints.
 
         :param req_type: the type of requirement (e.g. 'DockerRequirement')
         :type req_type: str
         :param req_param: the requirement parameter (e.g. 'dockerFile')
         :type req_param: str
+        :param default: default value if the requirement is not found
+        :type default: any
 
         When requirements are specified hints will be ignored.
         By default, tasks need not specify hints or requirements
         """
         requirements = dict(self.requirements)
-        requirement = None
+        requirement = default
         # Get value if specified in requirements
         try:
             # Try to get Requirement
             requirement = requirements[req_type][req_param]
         except (KeyError, TypeError):
             # Task Requirements are not mandatory. No docker_req_param specified in task reqs.
             requirement = None
@@ -188,15 +190,15 @@
             hints = dict(self.hints)
             # Get value if specified in hints
             try:
                 # Try to get Hints
                 requirement = hints[req_type][req_param]
             except (KeyError, TypeError):
                 # Task Hints are not mandatory. No docker_req_param specified in task hints.
-                requirement = None
+                requirement = default
         return requirement
 
     def __eq__(self, other):
         """Test the equality of two tasks.
 
         Task ID and dependencies do not factor into equality testing.
         :param other: the task with which to test equality
@@ -290,7 +292,11 @@
                     bind_mounts = {
                         os.getenv('HOME'): os.path.join('/home', os.getenv('USER')),
                     }
                     command.append(convert_path(checkpoint_file, bind_mounts))
                 break
 
         return command
+# Ignore C901: "'Task.command' is too complex" - right now this function is
+#              under 50 lines of code. If we add any more lines I think it
+#              might be best to break it up, but for now it seems fine.
+# pylama:ignore=C901
```

### Comparing `hpc-beeflow-0.1.3/beeflow/common/wf_interface.py` & `hpc_beeflow-0.1.4/beeflow/common/wf_interface.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/wf_profiler.py` & `hpc_beeflow-0.1.4/beeflow/common/wf_profiler.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/worker/__init__.py` & `hpc_beeflow-0.1.4/beeflow/common/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/worker/lsf_worker.py` & `hpc_beeflow-0.1.4/beeflow/common/worker/lsf_worker.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/worker/simple_worker.py` & `hpc_beeflow-0.1.4/beeflow/common/worker/simple_worker.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/common/worker_interface.py` & `hpc_beeflow-0.1.4/beeflow/common/worker_interface.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cloud_templates/dora.jinja` & `hpc_beeflow-0.1.4/beeflow/data/cloud_templates/dora.jinja`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cloud_templates/dora.yaml` & `hpc_beeflow-0.1.4/beeflow/data/cloud_templates/dora.yaml`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/README.md` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/blast/input/small.fasta` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/blast/input/small.fasta`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr.cwl`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- mode: YAML; -*-
 
 class: CommandLineTool
 cwlVersion: v1.0
 
-baseCommand: /clamr/CLAMR-master/clamr_cpuonly
+baseCommand: /CLAMR/clamr_cpuonly
 # This is the stdout field which makes all stdout be captured in this file
 # stderr is not currently implemented but it is also a thing
 stdout: clamr_stdout.txt
 # Arguments to the command
 inputs:
   amr_type:
     # ? means the argument is optional
```

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_wf.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # takes ID:Type syntax
   grid_resolution: int
   max_levels: int
   time_steps: int
   steps_between_outputs: int
   steps_between_graphics: int
   graphics_type: string
-  checkpoint_disk_interval: int
 ##### FFMPEG inputs #####
   input_format: string
   frame_rate: int
   frame_size: string
   pixel_format: string
   output_filename: string
 
@@ -46,30 +45,22 @@
     in:
       grid_res: grid_resolution
       max_levels: max_levels
       time_steps: time_steps
       output_steps: steps_between_outputs
       graphic_steps: steps_between_graphics
       graphics_type: graphics_type
-      checkpoint_disk_interval: checkpoint_disk_interval
-    out: [clamr_stdout, outdir, checkpoint_dir, time_log]
+    out: [clamr_stdout, outdir, time_log]
     hints:
         DockerRequirement:
             # TODO Sort this out
             #dockerImport: clamr_img.tar.gz
             #beeflow:copyContainer: clamr
-            beeflow:copyContainer: "/usr/projects/beedev/clamr/clamr-toss.tar.gz"
-        beeflow:CheckpointRequirement:
-            enabled: true
-            file_path: checkpoint_output
-            container_path: checkpoint_output
-            file_regex: backup[0-9]*.crx 
-            restart_parameters: -R
-            num_tries: 3
-            
+            beeflow:copyContainer: "/usr/projects/beedev/clamr/clamr-toss.simg"
+
   ffmpeg:
     run: ffmpeg.cwl
     in:
       input_format: input_format
       # input syntax is name: <step>/dependent_object
       ffmpeg_input: clamr/outdir
       frame_rate: frame_rate
```

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/ffmpeg.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl`

 * *Files 10% similar despite different names*

```diff
@@ -51,25 +51,25 @@
       graphics_type: graphics_type
     out: [clamr_stdout, outdir, time_log]
     hints:
         DockerRequirement:
             # TODO Sort this out
             #dockerImport: clamr_img.tar.gz
             #beeflow:copyContainer: clamr
-            beeflow:copyContainer: "/usr/projects/beedev/clamr/clamr-toss.simg"
+            beeflow:copyContainer: "/ccs/proj/csc420/BEE/clamr-ppc64le.tar.gz"
 
   ffmpeg:
     run: ffmpeg.cwl
     in:
-      input_format: input_format
-      # input syntax is name: <step>/dependent_object
+      input_format: input_format # input syntax is name: <step>/dependent_object
       ffmpeg_input: clamr/outdir
       frame_rate: frame_rate
       frame_size: frame_size
       pixel_format: pixel_format
       # Setting output file with file_name
       # output_filename set in wf inputs
       output_file: output_filename
     # Multiple outputs can be in array
     out: [movie]
-    requirements:
-        InlineJavascriptRequirement: {}
+    hints:
+      DockerRequirement:
+        beeflow:copyContainer: "/ccs/proj/csc420/BEE/clamr-ppc64le.tar.gz"
```

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl`

 * *Files 5% similar despite different names*

```diff
@@ -48,28 +48,25 @@
       time_steps: time_steps
       output_steps: steps_between_outputs
       graphic_steps: steps_between_graphics
       graphics_type: graphics_type
     out: [clamr_stdout, outdir, time_log]
     hints:
         DockerRequirement:
-            # TODO Sort this out
-            #dockerImport: clamr_img.tar.gz
-            #beeflow:copyContainer: clamr
-            beeflow:copyContainer: "/ccs/proj/csc420/BEE/clamr-ppc64le.tar.gz"
+            beeflow:useContainer: "/usr/projects/beedev/clamr/clamr-toss.tar.gz"
 
   ffmpeg:
     run: ffmpeg.cwl
     in:
-      input_format: input_format # input syntax is name: <step>/dependent_object
+      input_format: input_format
+      # input syntax is name: <step>/dependent_object
       ffmpeg_input: clamr/outdir
       frame_rate: frame_rate
       frame_size: frame_size
       pixel_format: pixel_format
       # Setting output file with file_name
       # output_filename set in wf inputs
       output_file: output_filename
     # Multiple outputs can be in array
     out: [movie]
-    hints:
-      DockerRequirement:
-        beeflow:copyContainer: "/ccs/proj/csc420/BEE/clamr-ppc64le.tar.gz"
+    requirements:
+        InlineJavascriptRequirement: {}
```

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-checkpoint/clamr_wf.cwl`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # takes ID:Type syntax
   grid_resolution: int
   max_levels: int
   time_steps: int
   steps_between_outputs: int
   steps_between_graphics: int
   graphics_type: string
+  checkpoint_disk_interval: int
 ##### FFMPEG inputs #####
   input_format: string
   frame_rate: int
   frame_size: string
   pixel_format: string
   output_filename: string
 
@@ -45,19 +46,29 @@
     in:
       grid_res: grid_resolution
       max_levels: max_levels
       time_steps: time_steps
       output_steps: steps_between_outputs
       graphic_steps: steps_between_graphics
       graphics_type: graphics_type
-    out: [clamr_stdout, outdir, time_log]
+      checkpoint_disk_interval: checkpoint_disk_interval
+    out: [clamr_stdout, outdir, checkpoint_dir, time_log]
     hints:
+        beeflow:CheckpointRequirement:
+            enabled: true
+            file_path: checkpoint_output
+            container_path: checkpoint_output
+            file_regex: backup[0-9]*.crx 
+            restart_parameters: -R
+            num_tries: 3
+        beeflow:SchedulerRequirement:
+            timeLimit: 00:00:10
         DockerRequirement:
-            beeflow:useContainer: "/usr/projects/beedev/clamr/clamr-toss.tar.gz"
-
+            dockerFile: "Dockerfile.clamr-ffmpeg"
+            beeflow:containerName: "clamr-ffmpeg"
   ffmpeg:
     run: ffmpeg.cwl
     in:
       input_format: input_format
       # input syntax is name: <step>/dependent_object
       ffmpeg_input: clamr/outdir
       frame_rate: frame_rate
@@ -66,7 +77,11 @@
       # Setting output file with file_name
       # output_filename set in wf inputs
       output_file: output_filename
     # Multiple outputs can be in array
     out: [movie]
     requirements:
         InlineJavascriptRequirement: {}
+    hints:
+        DockerRequirement:
+            dockerFile: "Dockerfile.clamr-ffmpeg"
+            beeflow:containerName: "clamr-ffmpeg"
```

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl`

 * *Files 20% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 outputs:
   comd_stdout:
     type: File
     outputSource: comd/comd_stdout
 
 steps:
   comd:
-    run: comd_bin.cwl
+    run: comd.cwl
     in:
       i: i
       j: j
       k: k
       x: x
       y: y
       z: z
       pot_dir: pot_dir
     out: [comd_stdout]
     hints:
       DockerRequirement:
-        # dockerPull: "jtronge/comd:latest"
-        beeflow:copyContainer: "/usr/projects/beedev/comd/comd-x86_64.tar.gz"
+        beeflow:copyContainer: "/usr/projects/beedev/mpi/comd-x86_64.tgz"
+        # See Dockerfile.comd-x86_64
       beeflow:MPIRequirement:
-        nodes: 8
+        nodes: 4
         ntasks: 8
```

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/comd-mpi/comd_bin.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl`

 * *Files 7% similar despite different names*

```diff
@@ -30,11 +30,12 @@
           type: stdout
     in:
       size: size
       iterations: iterations
     out: [lulesh_stdout]
     hints:
       DockerRequirement:
-        dockerPull: "jtronge/lulesh"
+        beeflow:useContainer: /usr/projects/beedev/mpi/lulesh-x86_64.tgz
+        # dockerPull: "jtronge/lulesh"
         # See Dockerfile.lulesh-x86_64
       beeflow:MPIRequirement:
         ntasks: 27
```

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt` & `hpc_beeflow-0.1.4/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl` & `hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt` & `hpc_beeflow-0.1.4/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le` & `hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le` & `hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64` & `hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64` & `hpc_beeflow-0.1.4/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/dockerfiles/README.md` & `hpc_beeflow-0.1.4/beeflow/data/dockerfiles/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian` & `hpc_beeflow-0.1.4/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5` & `hpc_beeflow-0.1.4/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch` & `hpc_beeflow-0.1.4/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/scheduler/README.md` & `hpc_beeflow-0.1.4/beeflow/scheduler/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/scheduler/algorithms.py` & `hpc_beeflow-0.1.4/beeflow/scheduler/algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,14 +258,10 @@
     """
     # Choose the default algorithm
     default = default_algorithm if default_algorithm is not None else 'fcfs'
     cls = algorithm_objects[default]
     if algorithm is not None:
         cls = algorithm_objects[algorithm]
     return AlgorithmLogWrapper(cls, **kwargs)
-# Ignoring E0211: This is how the class is designed right now, we should think about changing this
-#                 however.
-# Ignoring W0511: A number of these TODO's are hinted at in issue #333, but I don't want to remove
-#                 them from the code until this issue is fully addressed.
-# Ignoring R0903: Too few public methods, not sure how this calculated and this will be fixed with
-#                 issue #333
-# pylama:ignore=E0211,C0415,W0511,R0903
+
+# Ignore W0511: This allows us to have TODOs in the code
+# pylama:ignore=W0511
```

### Comparing `hpc-beeflow-0.1.3/beeflow/scheduler/resource_allocation.py` & `hpc_beeflow-0.1.4/beeflow/scheduler/resource_allocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,9 +255,10 @@
     def decode(data):
         """Decode the allocation.
 
         :param data: data representing the allocation
         :type data: dict
         """
         return Allocation(**data)
-# Ignore W0511: This is related to issue #333.
+
+# Ignore W0511: This allows us to have TODOs in the code
 # pylama:ignore=W0511
```

### Comparing `hpc-beeflow-0.1.3/beeflow/scheduler/scheduler.py` & `hpc_beeflow-0.1.4/beeflow/scheduler/scheduler.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,74 +7,58 @@
 from flask import Flask, request
 from flask_restful import Resource, Api
 
 from beeflow.scheduler import algorithms
 from beeflow.scheduler import task
 from beeflow.scheduler import resource_allocation
 from beeflow.common.config_driver import BeeConfig as bc
-from beeflow.common.db import sched
+from beeflow.common.db import sched_db
 from beeflow.common import log as bee_logging
 
+from beeflow.common.db.bdb import connect_db
 
 log = bee_logging.setup(__name__)
 
 flask_app = Flask(__name__)
 api = Api(flask_app)
 
 # We have to call bc.init() here due to how gunicorn works
 bc.init()
 
-
-def get_db_path():
-    """Get the database path."""
-    # Favor the environment variable if it exists
-    path = os.getenv('BEE_SCHED_DB_PATH')
-    if path is None:
-        workdir = bc.get('DEFAULT', 'bee_workdir')
-        path = os.path.join(workdir, 'sched.db')
-    return path
-
-
-def connect_db(fn):
-    """Decorate a function for connecting to a database."""
-    def wrap(*pargs, **kwargs):
-        """Decorate the function."""
-        with sched.open_db(get_db_path()) as db:
-            return fn(db, *pargs, **kwargs)
-
-    return wrap
+bee_workdir = bc.get('DEFAULT', 'bee_workdir')
+db_path = bee_workdir + '/' + 'sched.db'
 
 
 class ResourcesHandler(Resource):
     """Resources handler."""
 
     @staticmethod
-    @connect_db
-    def put(db):
+    def put():
         """Create a list of resources to use for allocation."""
+        db = connect_db(sched_db, db_path)
         db.resources.clear()
         resources = [resource_allocation.Resource.decode(r)
                      for r in request.json]
         db.resources.extend(resources)
         return f'created {len(resources)} resource(s)'
 
     @staticmethod
-    @connect_db
-    def get(db):
+    def get():
         """Get a list of all resources."""
+        db = connect_db(sched_db, db_path)
         return [r.encode() for r in db.resources]
 
 
 class WorkflowJobHandler(Resource):
     """Schedule jobs for a specific workflow with the current resources."""
 
     @staticmethod
-    @connect_db
-    def put(db, workflow_name):  # noqa ('workflow_name' may be used in the future)
+    def put(workflow_name):  # noqa ('workflow_name' may be used in the future)
         """Schedules a new list of independent tasks with available resources."""
+        db = connect_db(sched_db, db_path)
         data = request.json
         tasks = [task.Task.decode(t) for t in data]
         # Pick the scheduling algorithm
         algorithm = algorithms.choose(**vars(flask_app.sched_conf))
         algorithm.schedule_all(tasks, list(db.resources))
         return [t.encode() for t in tasks]
 
@@ -104,15 +88,14 @@
         'algorithm': None,
         'default_algorithm': None,
         'workdir': None,
     }
 
     for key in conf:
         conf[key] = bc.get('scheduler', key)
-    bee_workdir = bc.get('DEFAULT', 'bee_workdir')
     # Set some defaults
     if not conf['log']:
         conf['log'] = '/'.join([bee_workdir, 'logs', 'scheduler.log'])
     if not conf['workdir']:
         conf['workdir'] = os.path.join(bee_workdir, 'scheduler')
     if not conf['alloc_logfile']:
         conf['alloc_logfile'] = os.path.join(conf['workdir'],
@@ -138,9 +121,9 @@
 
     # Create the scheduler workdir, if necessary
     # sched_listen_port = wf_utils.get_open_port()
     # wf_db.set_sched_port(sched_listen_port)
     os.makedirs(conf.workdir, exist_ok=True)
     return flask_app
 
-# Ignore todo's or pylama fails
+# Ignore W0511: This allows us to have TODOs in the code
 # pylama:ignore=W0511
```

### Comparing `hpc-beeflow-0.1.3/beeflow/scheduler/scheduler.yaml` & `hpc_beeflow-0.1.4/beeflow/scheduler/scheduler.yaml`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/scheduler/serializable.py` & `hpc_beeflow-0.1.4/beeflow/scheduler/serializable.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/scheduler/task.py` & `hpc_beeflow-0.1.4/beeflow/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/task_manager.py` & `hpc_beeflow-0.1.4/beeflow/task_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,54 +16,38 @@
 from flask import Flask, jsonify, make_response
 from flask_restful import Resource, Api, reqparse
 
 from apscheduler.schedulers.background import BackgroundScheduler
 
 from beeflow.common.config_driver import BeeConfig as bc
 
+from beeflow.common.db.bdb import connect_db
+
 # This must be imported before calling other parts of BEE
 bc.init()
 
-print(sys.argv)
 
 from beeflow.common import log as bee_logging
 from beeflow.common.build_interfaces import build_main
 from beeflow.common.worker_interface import WorkerInterface
 from beeflow.common.connection import Connection
 import beeflow.common.worker as worker_pkg
-from beeflow.common.db import tm
+from beeflow.common.db import tm_db
 
 
 log = bee_logging.setup(__name__)
 
 runtime = bc.get('task_manager', 'container_runtime')
 
 
 flask_app = Flask(__name__)
 api = Api(flask_app)
 
-# submit_queue = []  # tasks ready to be submitted
-# job_queue = []  # jobs that are being monitored
-DB_PATH = os.path.join(bc.get('DEFAULT', 'bee_workdir'), 'tm.db')
-
-
-def connect_db(fn):
-    """Connect to the TM database."""
-
-    def wrap(*pargs, **kwargs):
-        """Wrap the function."""
-        # Check for the TESTING_DB_PATH for running the unit tests
-        try:
-            db_path = flask_app.config['TESTING_DB_PATH']
-        except KeyError:
-            db_path = DB_PATH
-        with tm.open_db(db_path) as db:
-            return fn(db, *pargs, **kwargs)
-
-    return wrap
+bee_workdir = bc.get('DEFAULT', 'bee_workdir')
+db_path = bee_workdir + '/' + 'tm.db'
 
 
 def _url():
     """Return  the url to the WFM."""
     # Saving this for whenever we need to run jobs across different machines
     # workflow_manager = 'bee_wfm/v1/jobs/'
     # #wfm_listen_port = bc.get('workflow_manager', 'listen_port')
@@ -133,17 +117,17 @@
 
 
 def resolve_environment(task):
     """Use build interface to create a valid environment."""
     build_main(task)
 
 
-@connect_db
-def submit_jobs(db):
+def submit_jobs():
     """Submit all jobs currently in submit queue to the workload scheduler."""
+    db = connect_db(tm_db, db_path)
     while db.submit_queue.count() >= 1:
         # Single value dictionary
         task = db.submit_queue.pop()
         try:
             log.info(f'Resolving environment for task {task.name}')
             resolve_environment(task)
             log.info(f'Environment preparation complete for task {task.name}')
@@ -206,76 +190,75 @@
     try:
         checkpoint_file = checkpoint_files[-1]
         return str(checkpoint_file)
     except IndexError:
         raise RuntimeError('Missing checkpoint file for task') from None
 
 
-@connect_db
-def update_jobs(db):
+def update_jobs():
     """Check and update states of jobs in queue, remove completed jobs."""
+    db = connect_db(tm_db, db_path)
     # Need to make a copy first
     job_q = list(db.job_queue)
     for job in job_q:
-        id_ = job['id']
-        task = job['task']
-        job_id = job['job_id']
-        job_state = worker.query_task(job_id)
+        id_ = job.id
+        task = job.task
+        job_id = job.job_id
+        job_state = job.job_state
+        new_job_state = worker.query_task(job_id)
 
         # If state changes update the WFM
-        if job_state != job['job_state']:
-            log.info(f'{task.name} {job["job_state"]} -> {job_state}')
-            # job['job_state'] = job_state
-            db.job_queue.update_job_state(id_, job_state)
-            if job_state in ('FAILED', 'TIMELIMIT', 'TIMEOUT'):
+        if job_state != new_job_state:
+            db.job_queue.update_job_state(id_, new_job_state)
+            if new_job_state in ('FAILED', 'TIMELIMIT', 'TIMEOUT'):
                 # Harvest lastest checkpoint file.
                 task_checkpoint = get_task_checkpoint(task)
+                log.info(f'state: {new_job_state}')
+                log.info(f'TIMELIMIT/TIMEOUT task_checkpoint: {task_checkpoint}')
                 if task_checkpoint:
                     checkpoint_file = get_restart_file(task_checkpoint, task.workdir)
                     task_info = {'checkpoint_file': checkpoint_file, 'restart': True}
-                    log.info(f'Restart: {task.name} task_info: {task_info}')
-                    update_task_state(task.workflow_id, task.id, job_state, task_info=task_info)
+                    update_task_state(task.workflow_id, task.id, new_job_state,
+                                      task_info=task_info)
                 else:
-                    update_task_state(task.workflow_id, task.id, job_state)
+                    update_task_state(task.workflow_id, task.id, new_job_state)
             else:
-                update_task_state(task.workflow_id, task.id, job_state)
+                update_task_state(task.workflow_id, task.id, new_job_state)
 
         if job_state in ('ZOMBIE', 'COMPLETED', 'CANCELLED', 'FAILED', 'TIMEOUT', 'TIMELIMIT'):
             # Remove from the job queue. Our job is finished
             db.job_queue.remove_by_id(id_)
-            # job_queue.remove(job)
-            log.info(f'Job {job_id} done {task.name}: removed from job status queue')
 
 
 def process_queues():
     """Look for newly submitted jobs and update status of scheduled jobs."""
     submit_jobs()  # noqa
     update_jobs()  # noqa
 
 
 if "pytest" not in sys.modules:
     scheduler = BackgroundScheduler({'apscheduler.timezone': 'UTC'})
-    scheduler.add_job(func=process_queues, trigger="interval", seconds=8)
+    scheduler.add_job(func=process_queues, trigger="interval", seconds=30)
     scheduler.start()
 
     # This kills the scheduler when the process terminates
     # so we don't accidentally leave a zombie process
     atexit.register(scheduler.shutdown)
 
 
 class TaskSubmit(Resource):
     """WFM sends tasks to the task manager."""
 
     def __init__(self):
         """Intialize request."""
 
     @staticmethod
-    @connect_db
-    def post(db):
+    def post():
         """Receives task from WFM."""
+        db = connect_db(tm_db, db_path)
         parser = reqparse.RequestParser()
         parser.add_argument('tasks', type=str, location='json')
         data = parser.parse_args()
         tasks = jsonpickle.decode(data['tasks'])
         for task in tasks:
             db.submit_queue.push(task)
             log.info(f"Added {task.name} task to the submit queue")
@@ -283,22 +266,22 @@
         return resp
 
 
 class TaskActions(Resource):
     """Actions to take for tasks."""
 
     @staticmethod
-    @connect_db
-    def delete(db):
+    def delete():
         """Cancel received from WFM to cancel job, update queue to monitor state."""
+        db = connect_db(tm_db, db_path)
         cancel_msg = ""
         for job in db.job_queue:
-            task_id = job['task'].id
-            job_id = job['job_id']
-            name = job['task'].name
+            task_id = job.task.id
+            job_id = job.job_id
+            name = job.task.name
             log.info(f"Cancelling {name} with job_id: {job_id}")
             try:
                 job_state = worker.cancel_task(job_id)
             except Exception as err:
                 log.error(err)
                 log.error(traceback.format_exc())
                 job_state = 'ZOMBIE'
@@ -322,20 +305,25 @@
 if worker_class is None:
     sys.exit(f'Workload scheduler {WLS}, not supported.\n'
              + f'Please check {bc.userconfig_path()} and restart TaskManager.')
 # Get the parameters for the worker classes
 worker_kwargs = {
     'bee_workdir': bc.get('DEFAULT', 'bee_workdir'),
     'container_runtime': bc.get('task_manager', 'container_runtime'),
-    'job_template': bc.get('task_manager', 'job_template'),
     # extra options to be passed to the runner (i.e. srun [RUNNER_OPTS] ... for Slurm)
     'runner_opts': bc.get('task_manager', 'runner_opts'),
 }
+# Job defaults
+for default_key in ['default_account', 'default_time_limit', 'default_partition']:
+    worker_kwargs[default_key] = bc.get('job', default_key)
+# Special slurm arguments
 if WLS == 'Slurm':
-    worker_kwargs['slurm_socket'] = bc.get('slurmrestd', 'slurm_socket')
+    worker_kwargs['use_commands'] = bc.get('slurm', 'use_commands')
+    worker_kwargs['slurm_socket'] = bc.get('slurm', 'slurmrestd_socket')
+    worker_kwargs['openapi_version'] = bc.get('slurm', 'openapi_version')
 worker = WorkerInterface(worker_class, **worker_kwargs)
 
 api.add_resource(TaskSubmit, '/bee_tm/v1/task/submit/')
 api.add_resource(TaskActions, '/bee_tm/v1/task/')
 
 # if __name__ == '__main__':
 #    hostname = socket.gethostname()
@@ -351,10 +339,11 @@
 #    werk_log.setLevel(logging.INFO)
 #    werk_log.addHandler(handler)
 #
 #    # Flask logging
 #    flask_app.logger.addHandler(handler)
 #    flask_app.run(debug=False, port=str(tm_listen_port))
 
-# Ignoring CO413 beeflow modules must be loaded after bc.init()
 # Ignoring W0703: Catching general exception is ok for failed submit and cancel.
-# pylama:ignore=C0413,W0703
+# Ignoring E402: "module level import is not at top of file" - this is required
+#                for the bee config
+# pylama:ignore=W0703,E402
```

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/42.tgz` & `hpc_beeflow-0.1.4/beeflow/tests/42.tgz`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/cf.cwl` & `hpc_beeflow-0.1.4/beeflow/tests/cf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/clamr.cwl` & `hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/clamr_wf.cwl` & `hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/clamr-wf/ffmpeg.cwl` & `hpc_beeflow-0.1.4/beeflow/tests/clamr-wf/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/clamr-wf.tgz` & `hpc_beeflow-0.1.4/beeflow/tests/clamr-wf.tgz`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/gdb.py` & `hpc_beeflow-0.1.4/beeflow/tests/gdb.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/mocks.py` & `hpc_beeflow-0.1.4/beeflow/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_config_validator.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_config_validator.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_container_path.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_container_path.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_db_sched.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_db_sched.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Tests of the scheduler database."""
 import tempfile
 import os
 
 import pytest
 
-from beeflow.common.db import sched
+from beeflow.common.db import sched_db
 
 
 @pytest.fixture
 def temp_db():
     """Create a fixture for making a temporary datbase."""
     fname = tempfile.mktemp()
-    with sched.open_db(fname) as db:
-        yield db
+    db = sched_db.open_db(fname)
+    yield db
     os.remove(fname)
 
 
 def test_empty(temp_db):
     """Test the empty database."""
     db = temp_db
 
@@ -34,8 +34,10 @@
 def test_clear(temp_db):
     """Test clearing the resources."""
     db = temp_db
     db.resources.extend([8, 9, 10, 11, 12, 13, 14])
 
     db.resources.clear()
     assert len(list(db.resources)) == 0
+# Ignore W0621: PyLama complains about redefining 'temp_db' from the outer
+#               scope. This is how pytest fixtures work.
 # pylama:ignore=W0621
```

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_db_tm.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_db_tm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Tests of the TM database."""
 import tempfile
 import os
 
 import pytest
 
-from beeflow.common.db import tm
+from beeflow.common.db import tm_db
 
 
 @pytest.fixture
 def temp_db():
     """Pytest fixture for creating a temporary database."""
     fname = tempfile.mktemp()
-    with tm.open_db(fname) as db:
-        yield db
+    db = tm_db.open_db(fname)
+    yield db
     os.remove(fname)
 
 
 def test_empty(temp_db):
     """Test an empty database."""
     db = temp_db
 
@@ -32,19 +32,18 @@
     # task
     db.submit_queue.push(3)
     db.job_queue.push(task=45, job_id=1289, job_state='READY')
 
     assert db.submit_queue.count() == 1
     assert db.job_queue.count() == 1
     assert db.submit_queue.pop() == 3
-    assert db.job_queue.pop() == {
-        'task': 45,
-        'job_id': 1289,
-        'job_state': 'READY',
-    }
+    popped_job = db.job_queue.pop()
+    assert popped_job.task == 45
+    assert popped_job.job_id == 1289
+    assert popped_job.job_state == 'READY'
     assert db.submit_queue.count() == 0
     assert db.job_queue.count() == 0
 
 
 def test_push_pop_many(temp_db):
     """Test pushing and popping many values."""
     db = temp_db
@@ -55,19 +54,18 @@
         job_state = 'READY' if (i % 2) == 0 else 'COMPLETED'
         db.job_queue.push(task=i, job_id=i + 1, job_state=job_state)
         assert db.submit_queue.count() == (i + 1)
         assert db.job_queue.count() == (i + 1)
     # Now pop 128 items
     for i in range(128):
         assert db.submit_queue.pop() == i
-        assert db.job_queue.pop() == {
-            'task': i,
-            'job_id': i + 1,
-            'job_state': 'READY' if (i % 2) == 0 else 'COMPLETED',
-        }
+        popped_job = db.job_queue.pop()
+        assert popped_job.task == i
+        assert popped_job.job_id == i + 1
+        assert popped_job.job_state == 'READY' if (i % 2) == 0 else 'COMPLETED'
         assert db.submit_queue.count() == (127 - i)
         assert db.job_queue.count() == (127 - i)
     assert db.submit_queue.count() == 0
     assert db.job_queue.count() == 0
 
 
 def test_clear(temp_db):
@@ -89,65 +87,64 @@
     assert db.submit_queue.count() == 0
 
 
 def test_iter(temp_db):
     """Test iterating over the values."""
     db = temp_db
 
-    values = (127, 16, 11999)
+    values = (127, 16)
     for val in values:
         db.submit_queue.push(val)
     for task, other in zip(db.submit_queue, values):
         assert task == other
 
     for val in values:
         db.job_queue.push(task=val, job_id=val, job_state='COMPLETED')
     for job, val in zip(db.job_queue, values):
-        assert 'id' in job
-        assert job['task'] == val
-        assert job['job_id'] == val
-        assert job['job_state'] == 'COMPLETED'
+        assert job.task == val
+        assert job.job_id == val
+        assert job.job_state == 'COMPLETED'
 
 
 def test_job_queue_remove_by_id(temp_db):
     """Test removing a job by ID for the job queue."""
     db = temp_db
 
     db.job_queue.push(task={8, 9, 10}, job_id=888, job_state='some-state0')
     db.job_queue.push(task={10}, job_id=999, job_state='some-state1')
     db.job_queue.push(task={46, 57}, job_id=111, job_state='some-state2')
 
     assert db.job_queue.count() == 3
 
     jobs = list(db.job_queue)
-    id_ = jobs[1]['id']
+    id_ = jobs[1].id
     db.job_queue.remove_by_id(id_)
 
     assert db.job_queue.count() == 2
     job = db.job_queue.pop()
-    assert job['task'] == {8, 9, 10}
-    assert job['job_id'] == 888
-    assert job['job_state'] == 'some-state0'
+    assert job.task == {8, 9, 10}
+    assert job.job_id == 888
+    assert job.job_state == 'some-state0'
     job = db.job_queue.pop()
-    assert job['task'] == {46, 57}
-    assert job['job_id'] == 111
-    assert job['job_state'] == 'some-state2'
+    assert job.task == {46, 57}
+    assert job.job_id == 111
+    assert job.job_state == 'some-state2'
     assert db.job_queue.count() == 0
 
 
 def test_job_queue_update_job_state(temp_db):
     """Test updating the job state for a job in the queue."""
     db = temp_db
 
     db.job_queue.push(task={8, 9, 10}, job_id='888', job_state='READY')
 
     jobs = list(db.job_queue)
-    id_ = jobs[0]['id']
+    id_ = jobs[0].id
     db.job_queue.update_job_state(id_, 'COMPLETED')
 
     job = db.job_queue.pop()
-    assert job['task'] == {8, 9, 10}
-    assert job['job_id'] == 888
-    assert job['job_state'] == 'COMPLETED'
+    assert job.task == {8, 9, 10}
+    assert job.job_id == 888
+    assert job.job_state == 'COMPLETED'
 # Ignore W0621: PyLama complains about redefining 'temp_db' from the outer
 #               scope. This is how pytest fixtures work.
 # pylama:ignore=W0621
```

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_parser.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 from pathlib import Path
 import unittest
 from beeflow.common.parser import CwlParser
 from beeflow.common.wf_data import generate_workflow_id
 from beeflow.tests.mocks import MockWFI
 
-# Disable protected member access warning
-# pylama:ignore=W0212
 
 REPO_PATH = Path(*Path(__file__).parts[:-3])
 
 
 def find(path):
     """Find a path relative to the root of the repo."""
     return str(Path(REPO_PATH, path))
```

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_scheduler.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_scheduler_resource_allocation.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_scheduler_resource_allocation.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_scheduler_rest.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_scheduler_rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Scheduler REST test cases.
 
 Tests of the REST interface for BEE Scheduler.
 """
+import os
 import tempfile
 import pytest
 
 from beeflow.scheduler.scheduler import create_app
 
-
 SCHEDULER_TEST_PORT = '5100'
 
 
 def endpoint(*pargs):
     """Return the endpoint url for a resource."""
     return '/'.join(['bee_sched/v1', *pargs])
 
@@ -22,17 +22,18 @@
 
     Start a new scheduler as a subprocess for each test function.
     """
     app = create_app()
     app.config.update({
         'TESTING': True,
     })
-    with tempfile.NamedTemporaryFile() as fp:
-        mocker.patch('beeflow.scheduler.scheduler.get_db_path', return_value=fp.name)
-        yield app.test_client()
+    fname = tempfile.mktemp(suffix='.db')
+    mocker.patch('beeflow.scheduler.scheduler.db_path', fname)
+    yield app.test_client()
+    os.remove(fname)
 
 
 def test_schedule_job_no_resources(scheduler):
     """Test scheduling a job with no resources.
 
     Test scheduling a job with no resources.
     :param scheduler: connection returned by fixture
```

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_slurm_worker.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_slurm_worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from beeflow.common.worker.slurm_worker import SlurmWorker
 from beeflow.common.wf_data import Task
 
 
 # Timeout (seconds) for waiting on tasks
 TIMEOUT = 150
 # Extra slurmrestd arguments. This may be something to take on the command line
-SLURMRESTD_ARGS = bc.get('slurmrestd', 'slurm_args')
+OPENAPI_VERSION = bc.get('slurm', 'openapi_version')
 GOOD_TASK = Task(name='good-task', base_command=['sleep', '3'], hints=[],
                  requirements=[], inputs=[], outputs=[], stdout='', stderr='',
                  workflow_id=uuid.uuid4().hex)
 BAD_TASK = Task(name='bad-task', base_command=['/this/is/not/a/command'], hints=[],
                 requirements=[], inputs=[], outputs=[], stdout='', stderr='',
                 workflow_id=uuid.uuid4().hex)
 
@@ -38,103 +38,88 @@
             raise RuntimeError(f'job timed out, still in state {state}')
         time.sleep(1)
         n += 1
         last_state = worker_iface.query_task(job_id)
     return last_state
 
 
-def setup_slurm_worker(fn):
-    """Add a decorator to set up the worker interface and slurmrestd."""
-
-    def decorator():
-        """Decorate the input function."""
-        slurm_socket = f'/tmp/{uuid.uuid4().hex}.sock'
-        bee_workdir = os.path.expanduser(f'~/{uuid.uuid4().hex}.tmp')
-        os.mkdir(bee_workdir)
-        proc = subprocess.Popen(f'slurmrestd {SLURMRESTD_ARGS} unix:{slurm_socket}', shell=True)
-        time.sleep(1)
-        worker_iface = WorkerInterface(worker=SlurmWorker, container_runtime='Charliecloud',
-                                       slurm_socket=slurm_socket, bee_workdir=bee_workdir,
-                                       job_template=bc.get('task_manager', 'job_template'))
-        fn(worker_iface)
-        time.sleep(1)
-        proc.kill()
-
-    return decorator
-
-
-def setup_worker_iface(fn):
-    """Add a decorator that creates the worker interface but not slurmrestd."""
+@pytest.fixture(params=[True, False], ids=['slurm-commands', 'slurmrestd'])
+def slurm_worker(request):
+    """Slurm worker fixture."""
+    slurm_socket = f'/tmp/{uuid.uuid4().hex}.sock'
+    bee_workdir = os.path.expanduser(f'~/{uuid.uuid4().hex}.tmp')
+    os.mkdir(bee_workdir)
+    proc = subprocess.Popen(f'slurmrestd -s openapi/{OPENAPI_VERSION} unix:{slurm_socket}',
+                            shell=True)
+    time.sleep(1)
+    worker_iface = WorkerInterface(worker=SlurmWorker, container_runtime='Charliecloud',
+                                   slurm_socket=slurm_socket, bee_workdir=bee_workdir,
+                                   openapi_version=OPENAPI_VERSION,
+                                   use_commands=request.param)
+    yield worker_iface
+    time.sleep(1)
+    proc.kill()
 
-    def decorator():
-        """Decorate the input function."""
-        slurm_socket = f'/tmp/{uuid.uuid4().hex}.sock'
-        bee_workdir = os.path.expanduser(f'~/{uuid.uuid4().hex}.tmp')
-        os.mkdir(bee_workdir)
-        worker_iface = WorkerInterface(worker=SlurmWorker, container_runtime='Charliecloud',
-                                       slurm_socket=slurm_socket, bee_workdir=bee_workdir,
-                                       job_template=bc.get('task_manager', 'job_template'))
-        fn(worker_iface)
 
-    return decorator
+@pytest.fixture
+def slurmrestd_worker_no_daemon():
+    """Fixture that creates the worker interface but not slurmrestd."""
+    slurm_socket = f'/tmp/{uuid.uuid4().hex}.sock'
+    bee_workdir = os.path.expanduser(f'~/{uuid.uuid4().hex}.tmp')
+    os.mkdir(bee_workdir)
+    yield WorkerInterface(worker=SlurmWorker, container_runtime='Charliecloud',
+                          slurm_socket=slurm_socket, bee_workdir=bee_workdir,
+                          openapi_version=OPENAPI_VERSION,
+                          use_commands=False)
 
 
-@setup_slurm_worker
-def test_good_task(worker_iface):
+def test_good_task(slurm_worker):
     """Test submission of a good task."""
-    job_id, last_state = worker_iface.submit_task(GOOD_TASK)
-    assert last_state == 'PENDING'
-    last_state = wait_state(worker_iface, job_id, 'PENDING')
+    job_id, last_state = slurm_worker.submit_task(GOOD_TASK)
+    if last_state == 'PENDING':
+        last_state = wait_state(slurm_worker, job_id, 'PENDING')
     if last_state == 'RUNNING':
-        last_state = wait_state(worker_iface, job_id, 'RUNNING')
+        last_state = wait_state(slurm_worker, job_id, 'RUNNING')
     if last_state == 'COMPLETING':
-        last_state = wait_state(worker_iface, job_id, 'COMPLETING')
+        last_state = wait_state(slurm_worker, job_id, 'COMPLETING')
     assert last_state == 'COMPLETED'
 
 
-@setup_slurm_worker
-def test_bad_task(worker_iface):
+def test_bad_task(slurm_worker):
     """Test submission of a bad task."""
-    job_id, last_state = worker_iface.submit_task(BAD_TASK)
-    assert last_state == 'PENDING'
-    last_state = wait_state(worker_iface, job_id, 'PENDING')
+    job_id, last_state = slurm_worker.submit_task(BAD_TASK)
+    if last_state == 'PENDING':
+        last_state = wait_state(slurm_worker, job_id, 'PENDING')
     if last_state == 'RUNNING':
-        last_state = wait_state(worker_iface, job_id, 'RUNNING')
+        last_state = wait_state(slurm_worker, job_id, 'RUNNING')
     if last_state == 'COMPLETING':
-        last_state = wait_state(worker_iface, job_id, 'COMPLETING')
+        last_state = wait_state(slurm_worker, job_id, 'COMPLETING')
     assert last_state == 'FAILED'
 
 
-@setup_slurm_worker
-def test_query_bad_job_id(worker_iface):
+def test_query_bad_job_id(slurm_worker):
     """Test querying a bad job ID."""
     with pytest.raises(WorkerError):
-        worker_iface.query_task(888)
+        slurm_worker.query_task(888)
 
 
-@setup_slurm_worker
-def test_cancel_good_job(worker_iface):
+def test_cancel_good_job(slurm_worker):
     """Cancel a good job."""
-    job_id, _ = worker_iface.submit_task(GOOD_TASK)
-    job_state = worker_iface.cancel_task(job_id)
+    job_id, _ = slurm_worker.submit_task(GOOD_TASK)
+    job_state = slurm_worker.cancel_task(job_id)
     assert job_state == 'CANCELLED'
 
 
-# This test is broken in CI, but works locally. I'm commenting it out for now
-# @setup_slurm_worker
-# def test_cancel_bad_job_id(worker_iface):
-#    """Cancel a non-existent job."""
-#    with pytest.raises(WorkerError):
-#        worker_iface.cancel_task(888)
-
-
-@setup_worker_iface
-def test_no_slurmrestd(worker_iface):
+def test_no_slurmrestd(slurmrestd_worker_no_daemon):
     """Test without running slurmrestd."""
-    job_id, state = worker_iface.submit_task(GOOD_TASK)
+    worker = slurmrestd_worker_no_daemon
+    job_id, state = worker.submit_task(GOOD_TASK)
     assert state == 'NOT_RESPONDING'
-    assert worker_iface.query_task(job_id) == 'NOT_RESPONDING'
-    assert worker_iface.cancel_task(job_id) == 'NOT_RESPONDING'
+    assert worker.query_task(job_id) == 'NOT_RESPONDING'
+    assert worker.cancel_task(job_id) == 'NOT_RESPONDING'
 # Ignoring R1732: This is not what we need to do with the Popen of slurmrestd above;
 #                 using a with statement doesn't kill the process immediately but just
 #                 waits for it to complete and slurmrestd never will unless we kill it.
-# pylama:ignore=R1732
+# Ignoring E402: "module level import not at top of file" - this is required for
+#                bee config
+# Ignoring W0621: Redefinition of names is required for pytest
+# pylama:ignore=R1732,E402,W0621
```

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_tm.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_tm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,57 @@
-"""This is a sample docstring."""
+"""Unit tests for the task manager."""
 
-import uuid
+import tempfile
 import os
+import uuid
 import pytest
 import jsonpickle
-from mocks import MockWorkerCompletion, MockWorkerSubmission
 from mocks import mock_put
+from mocks import MockWorkerCompletion, MockWorkerSubmission
 
+from beeflow.common.db.bdb import connect_db
+from beeflow.common.db import tm_db
 import beeflow.task_manager as tm
 from beeflow.common.wf_data import Task
 import beeflow
 
 
 @pytest.fixture
 def flask_client():
     """Client lets us run flask queries."""
     app = tm.flask_app
-    app.config['TESTING'] = True
-    db_path = f'/tmp/{uuid.uuid4().hex}.db'
-    app.config['TESTING_DB_PATH'] = db_path
     client = app.test_client()
     yield client
-    os.remove(db_path)
-
-
-@pytest.fixture
-@tm.connect_db
-def database(db):
-    """Fixture for connecting to the TM DB."""
-    return db
 
 
 def generate_tasks(n):
     """Generate n tasks for testing."""
     return [
         Task(f'task-{i}', base_command=['ls', '/'], hints=[], requirements=[],
              inputs=[], outputs=[], stdout=None, stderr=None,
              workflow_id=uuid.uuid4().hex)
         for i in range(n)
     ]
 
 
+@pytest.fixture
+def temp_db():
+    """Pytest fixture for creating a temporary database."""
+    fname = tempfile.mktemp(suffix='.db')
+    db = connect_db(tm_db, fname)
+    yield db
+    os.remove(fname)
+
+
 @pytest.mark.usefixtures('flask_client', 'mocker')
-def test_submit_task(flask_client, mocker, database):  # noqa
+def test_submit_task(flask_client, mocker, temp_db):  # noqa
     """Create a workflow and get the ID back."""
+    mocker.patch('beeflow.task_manager.worker',
+                 new_callable=MockWorkerSubmission)
+    mocker.patch('beeflow.task_manager.db_path', temp_db.db_file)
     # Generate a task
     tasks = generate_tasks(1)
     tasks_json = jsonpickle.encode(tasks)
 
     response = flask_client.post('/bee_tm/v1/task/submit/',
                                  json={'tasks': tasks_json})
 
@@ -56,55 +60,55 @@
 
     # Patch the connection object for WFM communication
     mocker.patch('beeflow.common.connection.Connection.put', mock_put)
     beeflow.task_manager.process_queues()
 
     msg = response.get_json()['msg']
     status = response.status_code
-
-    job_queue = list(database.job_queue)
+    job_queue = list(temp_db.job_queue)
 
     # We should only have a single job on the queue
     assert len(job_queue) == 1
     job = job_queue[0]
-    assert job['task'] == tasks[0]
-    assert job['job_id'] == 1
-    assert job['job_state'] == 'RUNNING'
+    assert job.task == tasks[0]
+    assert job.job_id == 1
+    assert job.job_state == 'RUNNING'
 
     assert status == 200
     assert msg == 'Tasks Added!'
 
 
 @pytest.mark.usefixtures('flask_client', 'mocker')
-def test_completed_task(flask_client, mocker, database): # noqa
+def test_completed_task(flask_client, mocker, temp_db): # noqa
     """Tests how the task manager processes a completed task."""
     # 42 is the sample task ID
     mocker.patch('beeflow.task_manager.worker',
                  new_callable=MockWorkerCompletion)
     # Patch the connection object for WFM communication
     mocker.patch('beeflow.common.connection.Connection.put', mock_put)
+    mocker.patch('beeflow.task_manager.db_path', temp_db.db_file)
 
     # This should notice the job is complete and empty the job_queue
     beeflow.task_manager.process_queues()
-    job_queue = list(database.job_queue)
+    job_queue = list(temp_db.job_queue)
     assert len(job_queue) == 0
 
 
 @pytest.mark.usefixtures('flask_client', 'mocker')
-def test_remove_task(flask_client, mocker, database):  # noqa
+def test_remove_task(flask_client, mocker, temp_db):  # noqa
     """Test cancelling a workflow and removing tasks."""
     task1, task2, task3 = generate_tasks(3)
     # Add a few tasks
-    database.job_queue.push(task=task1, job_id=1, job_state='RUNNING')
-    database.job_queue.push(task=task2, job_id=2, job_state='PENDING')
-    database.job_queue.push(task=task3, job_id=3, job_state='PENDING')
+    temp_db.job_queue.push(task=task1, job_id=1, job_state='RUNNING')
+    temp_db.job_queue.push(task=task2, job_id=2, job_state='PENDING')
+    temp_db.job_queue.push(task=task3, job_id=3, job_state='PENDING')
 
     mocker.patch('beeflow.task_manager.worker',
                  new_callable=MockWorkerCompletion)
+    mocker.patch('beeflow.task_manager.db_path', temp_db.db_file)
 
     response = flask_client.delete('/bee_tm/v1/task/')
 
     msg = response.get_json()['msg']
-    print(msg)
     status = response.status_code
     assert status == 200
     assert msg.count('CANCELLED') == 3
```

### Comparing `hpc-beeflow-0.1.3/beeflow/tests/test_wf_interface.py` & `hpc_beeflow-0.1.4/beeflow/tests/test_wf_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 #! /usr/bin/env python3
 """Unit test module for the BEE workflow interface module."""
 
-# Disable protected member access warning
-# pylama:ignore=W0212
-
 import unittest
 
 from beeflow.common.config_driver import BeeConfig as bc
 
 bc.init()
 
 from beeflow.common.wf_data import (Requirement, Hint, InputParameter, OutputParameter,
@@ -657,7 +654,10 @@
                 hints=[Hint("ResourceRequirement", {"ramMax": 2048})], stdout="viz_output.txt")
         ]
         return tasks
 
 
 if __name__ == "__main__":
     unittest.main()
+# Ignore W0212: Access required for unit tests
+# Ignore E402: "module level import not at top of file" - this is required for bee config
+# pylama:ignore=W0212,E402
```

### Comparing `hpc-beeflow-0.1.3/beeflow/wf_manager/common/dep_manager.py` & `hpc_beeflow-0.1.4/beeflow/wf_manager/common/dep_manager.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/wf_manager/common/wf_db.py` & `hpc_beeflow-0.1.4/beeflow/wf_manager/common/wf_db.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.3/beeflow/wf_manager/resources/wf_actions.py` & `hpc_beeflow-0.1.4/beeflow/wf_manager/resources/wf_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,104 @@
 """This module contains the workflow action endpoints."""
 
 from flask import make_response, jsonify
 from flask_restful import Resource, reqparse
-from beeflow.wf_manager.common import wf_db
 from beeflow.common import log as bee_logging
 from beeflow.wf_manager.resources import wf_utils
 
+from beeflow.common.db import wfm_db
+from beeflow.common.db.bdb import connect_db
 
 log = bee_logging.setup(__name__)
+db_path = wf_utils.get_db_path()
 
 
 class WFActions(Resource):
     """Class to perform actions on existing workflows."""
 
     def __init__(self):
         """Initialize with passed json object."""
         self.reqparse = reqparse.RequestParser()
 
     def post(self, wf_id):
         """Start workflow. Send ready tasks to the task manager."""
+        db = connect_db(wfm_db, db_path)
         wfi = wf_utils.get_workflow_interface(wf_id)
         state = wfi.get_workflow_state()
         if state in ('RUNNING', 'PAUSED', 'COMPLETED'):
             resp = make_response(jsonify(msg='Cannot start workflow it is '
                                  f'{state.lower()}.',
                                          status='ok'), 200)
             return resp
         wfi.execute_workflow()
         tasks = wfi.get_ready_tasks()
         wf_utils.schedule_submit_tasks(wf_id, tasks)
         wf_id = wfi.workflow_id
         wf_utils.update_wf_status(wf_id, 'Running')
-        wf_db.update_workflow_state(wf_id, 'Running')
+        db.workflows.update_workflow_state(wf_id, 'Running')
         resp = make_response(jsonify(msg='Started workflow!', status='ok'), 200)
         return resp
 
     @staticmethod
     def get(wf_id):
         """Check the database for the current status of all tasks."""
-        tasks = wf_db.get_tasks(wf_id)
+        db = connect_db(wfm_db, db_path)
+        tasks = db.workflows.get_tasks(wf_id)
         tasks_status = []
         if not tasks:
             log.info(f"Bad query for wf {wf_id}.")
             wf_status = 'No workflow with that ID is currently loaded'
             tasks_status.append('Unavailable')
             resp = make_response(jsonify(tasks_status=tasks_status,
                                  wf_status=wf_status, status='not found'), 404)
 
         for task in tasks:
-            tasks_status.append(f"{task.name}--{task.status}")
+            tasks_status.append(f"{task.name}--{task.state}")
         tasks_status = '\n'.join(tasks_status)
         wf_status = wf_utils.read_wf_status(wf_id)
 
         resp = make_response(jsonify(tasks_status=tasks_status,
                              wf_status=wf_status, status='ok'), 200)
         return resp
 
     @staticmethod
     def delete(wf_id):
         """Cancel the workflow. Lets current tasks finish running."""
+        db = connect_db(wfm_db, db_path)
         wfi = wf_utils.get_workflow_interface(wf_id)
         # Remove all tasks currently in the database
         if wfi.workflow_loaded():
             wfi.finalize_workflow()
         wf_utils.update_wf_status(wf_id, 'Cancelled')
-        wf_db.update_workflow_state(wf_id, 'Cancelled')
-        wf_db.delete_workflow(wf_id)
+        db.workflows.update_workflow_state(wf_id, 'Cancelled')
+        db.workflows.delete_workflow(wf_id)
         log.info("Workflow cancelled")
         resp = make_response(jsonify(status='Cancelled'), 202)
         return resp
 
     def patch(self, wf_id):
         """Pause or resume workflow."""
+        db = connect_db(wfm_db, db_path)
         self.reqparse.add_argument('option', type=str, location='json')
         option = self.reqparse.parse_args()['option']
 
         wfi = wf_utils.get_workflow_interface(wf_id)
         wf_state = wfi.get_workflow_state()
         if option == 'pause' and wf_state == 'RUNNING':
             wfi.pause_workflow()
             wf_utils.update_wf_status(wf_id, 'Paused')
-            wf_db.update_workflow_state(wf_id, 'Paused')
+            db.workflows.update_workflow_state(wf_id, 'Paused')
             log.info("Workflow Paused")
             resp = make_response(jsonify(status='Workflow Paused'), 200)
         elif option == 'resume' and wf_state == 'PAUSED':
             wfi.resume_workflow()
             tasks = wfi.get_ready_tasks()
             wf_utils.schedule_submit_tasks(wf_id, tasks)
             wf_utils.update_wf_status(wf_id, 'Running')
-            wf_db.update_workflow_state(wf_id, 'Running')
-            log.info("Workflow Paused")
+            db.workflows.update_workflow_state(wf_id, 'Running')
             log.info("Workflow Resumed")
             resp = make_response(jsonify(status='Workflow Resumed'), 200)
         else:
             resp_msg = f'Cannot {option} workflow. It is currently {wf_state.lower()}.'
             log.info(resp_msg)
             resp = make_response(jsonify(status=resp_msg), 200)
         return resp
```

### Comparing `hpc-beeflow-0.1.3/beeflow/wf_manager/resources/wf_list.py` & `hpc_beeflow-0.1.4/beeflow/wf_manager/resources/wf_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 
 from beeflow.common import log as bee_logging
 # from beeflow.common.wf_profiler import WorkflowProfiler
 from beeflow.common.parser import CwlParser, CwlParseError
 
 from beeflow.wf_manager.resources import wf_utils
 from beeflow.wf_manager.common import dep_manager
-from beeflow.wf_manager.common import wf_db
 from beeflow.common import wf_data
 
+from beeflow.common.db import wfm_db
+from beeflow.common.db.bdb import connect_db
+
 log = bee_logging.setup(__name__)
 
 
 def parse_workflow(wfi, wf_id, workflow_dir, main_cwl, yaml_file):
     """Run the parser."""
     parser = CwlParser(wfi)
     cwl_path = os.path.join(workflow_dir, main_cwl)
@@ -58,31 +60,36 @@
 
     subprocess.run(['tar', '-xf', archive_path, '--strip-components=1',
                     '-C', wf_dir], check=False)
     archive_dir = os.path.join(wf_dir, 'gdb')
     return archive_dir
 
 
+db_path = wf_utils.get_db_path()
+
+
 class WFList(Resource):
     """Interacts with existing workflows."""
 
     def get(self):
         """Return list of workflows to client."""
-        workflow_list = wf_db.get_workflows()
+        db = connect_db(wfm_db, db_path)
+        workflow_list = db.workflows.get_workflows()
         info = []
         for wf_info in workflow_list:
             wf_id = wf_info.workflow_id
-            wf_status = wf_info.status
+            wf_status = wf_info.state
             wf_name = wf_info.name
             info.append([wf_name, wf_id, wf_status])
         resp = make_response(jsonify(workflow_list=jsonpickle.encode(info)), 200)
         return resp
 
     def post(self):
         """Receive a workflow, parse it, and start up a neo4j instance for it."""
+        db = connect_db(wfm_db, db_path)
         reqparser = reqparse.RequestParser()
         reqparser.add_argument('wf_name', type=str, required=True,
                                location='form')
         reqparser.add_argument('main_cwl', type=str, required=True,
                                location='form')
         reqparser.add_argument('yaml', type=str, required=False,
                                location='form')
@@ -111,40 +118,40 @@
 
         wf_id = wf_data.generate_workflow_id()
         wf_dir = extract_wf(wf_id, wf_filename, wf_tarball)
         bolt_port = wf_utils.get_open_port()
         http_port = wf_utils.get_open_port()
         https_port = wf_utils.get_open_port()
         gdb_pid = dep_manager.start_gdb(wf_dir, bolt_port, http_port, https_port)
-        wf_db.add_workflow(wf_id, wf_name, 'Pending', wf_dir, bolt_port, gdb_pid)
+        db.workflows.add_workflow(wf_id, wf_name, 'Pending', wf_dir, bolt_port, gdb_pid)
         dep_manager.wait_gdb(log)
 
         try:
-            # wfi = parse_workflow(wf_path, main_cwl, yaml_file)
             wfi = wf_utils.get_workflow_interface(wf_id)
             parse_workflow(wfi, wf_id, wf_dir, main_cwl, yaml_file)
         except CwlParseError as err:
             traceback.print_exc()
             log.error('Failed to parse file')
             return make_response(jsonify(msg=f'Parser: {err.args[0]}', status='error'), 400)
         # initialize_wf_profiler(wf_name)
 
         wf_utils.create_wf_metadata(wf_id, wf_name)
         _, tasks = wfi.get_workflow()
         for task in tasks:
             metadata = wfi.get_task_metadata(task)
             metadata['workdir'] = wf_workdir
             wfi.set_task_metadata(task, metadata)
-            wf_db.add_task(task.id, wf_id, task.name, "WAITING")
+            db.workflows.add_task(task.id, wf_id, task.name, "WAITING")
         resp = make_response(jsonify(msg='Workflow uploaded', status='ok',
                              wf_id=wf_id), 201)
         return resp
 
     def put(self):
         """Reexecute a workflow."""
+        db = connect_db(wfm_db, db_path)
         reqparser = reqparse.RequestParser()
         reqparser.add_argument('wf_name', type=str, required=True,
                                location='form')
         reqparser.add_argument('wf_filename', type=str, required=True,
                                location='form')
         reqparser.add_argument('workdir', type=str, required=True,
                                location='form')
@@ -167,15 +174,15 @@
         wf_id = wf_data.generate_workflow_id()
         wf_dir = extract_wf(wf_id, wf_filename, workflow_archive, reexecute=True)
         bolt_port = wf_utils.get_open_port()
         http_port = wf_utils.get_open_port()
         https_port = wf_utils.get_open_port()
         gdb_pid = dep_manager.start_gdb(wf_dir, bolt_port, http_port,
                                         https_port, reexecute=True)
-        wf_db.add_workflow(wf_id, wf_name, 'Pending', wf_dir, bolt_port, gdb_pid)
+        db.workflows.add_workflow(wf_id, wf_name, 'Pending', wf_dir, bolt_port, gdb_pid)
         dep_manager.wait_gdb(log)
         wfi = wf_utils.get_workflow_interface(wf_id)
         wfi.reset_workflow(wf_id)
         wf_utils.create_wf_metadata(wf_id, wf_name)
 
         _, tasks = wfi.get_workflow()
         for task in tasks:
```

### Comparing `hpc-beeflow-0.1.3/beeflow/wf_manager/resources/wf_update.py` & `hpc_beeflow-0.1.4/beeflow/wf_manager/resources/wf_update.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,30 +5,34 @@
 import shutil
 import subprocess
 import time
 import jsonpickle
 
 from flask import make_response, jsonify
 from flask_restful import Resource, reqparse
-from beeflow.wf_manager.common import wf_db
 from beeflow.wf_manager.resources import wf_utils
 from beeflow.wf_manager.common import dep_manager
 from beeflow.common import log as bee_logging
 
+from beeflow.common.db import wfm_db
+from beeflow.common.db.bdb import connect_db
+
+
 log = bee_logging.setup(__name__)
+db_path = wf_utils.get_db_path()
 
 
-def archive_workflow(wf_id):
+def archive_workflow(db, wf_id):
     """Archive a workflow after completion."""
     # Archive Config
     workflow_dir = wf_utils.get_workflow_dir(wf_id)
     shutil.copyfile(os.path.expanduser("~") + '/.config/beeflow/bee.conf',
                     workflow_dir + '/' + 'bee.conf')
 
-    wf_db.update_workflow_state(wf_id, 'Archived')
+    db.workflows.update_workflow_state(wf_id, 'Archived')
     wf_utils.update_wf_status(wf_id, 'Archived')
 
     bee_workdir = wf_utils.get_bee_workdir()
     archive_dir = os.path.join(bee_workdir, 'archives')
     os.makedirs(archive_dir, exist_ok=True)
     archive_path = f'../archives/{wf_id}.tgz'
     # We use tar directly since tarfile is apparently very slow
@@ -52,24 +56,24 @@
                                    required=False)
         self.reqparse.add_argument('task_info', type=str, location='json',
                                    required=False)
         self.reqparse.add_argument('output', location='json', required=False)
 
     def put(self):
         """Update the state of a task from the task manager."""
+        db = connect_db(wfm_db, db_path)
         data = self.reqparse.parse_args()
         wf_id = data['wf_id']
         task_id = data['task_id']
         job_state = data['job_state']
 
         wfi = wf_utils.get_workflow_interface(wf_id)
         task = wfi.get_task_by_id(task_id)
         wfi.set_task_state(task, job_state)
-        wf_db.update_task_state(task_id, wf_id, job_state)
-        # wf_profiler.add_state_change(task, job_state)
+        db.workflows.update_task_state(task_id, wf_id, job_state)
 
         # Get metadata from update if available
         if 'metadata' in data:
             if data['metadata'] is not None:
                 metadata = jsonpickle.decode(data['metadata'])
                 wfi.set_task_metadata(task, metadata)
 
@@ -88,14 +92,15 @@
             with open(task_output_path, 'w', encoding='utf8') as fp:
                 json.dump(json.loads(data['output']), fp, indent=4)
 
         if 'task_info' in data and data['task_info'] is not None:
             task_info = jsonpickle.decode(data['task_info'])
             checkpoint_file = task_info['checkpoint_file']
             new_task = wfi.restart_task(task, checkpoint_file)
+            db.workflows.add_task(new_task.id, wf_id, new_task.name, "WAITING")
             if new_task is None:
                 log.info('No more restarts')
                 state = wfi.get_task_state(task)
                 return make_response(jsonify(status=f'Task {task_id} set to {job_state}'))
             # Submit the restart task
             tasks = [new_task]
             wf_utils.schedule_submit_tasks(wf_id, tasks)
@@ -110,17 +115,17 @@
             tasks = wfi.finalize_task(task)
             state = wfi.get_workflow_state()
             if tasks and state != 'PAUSED':
                 wf_utils.schedule_submit_tasks(wf_id, tasks)
 
             if wfi.workflow_completed():
                 log.info("Workflow Completed")
-                # Save the profile
-                # wf_profiler.save()
                 wf_id = wfi.workflow_id
-                archive_workflow(wf_id)
-                pid = wf_db.get_gdb_pid(wf_id)
+                archive_workflow(db, wf_id)
+                pid = db.workflows.get_gdb_pid(wf_id)
                 dep_manager.kill_gdb(pid)
-
         resp = make_response(jsonify(status=(f'Task {task_id} belonging to WF {wf_id} set to'
                                              f'{job_state}')), 200)
         return resp
+# Ignoring C901,R0915: "'WFUPdate.put' is too complex" - this requires a refactor
+#                      (or maybe the LOC limit is too low)
+# pylama:ignore=C901,R0915
```

### Comparing `hpc-beeflow-0.1.3/beeflow/wf_manager/resources/wf_utils.py` & `hpc_beeflow-0.1.4/beeflow/wf_manager/resources/wf_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,37 @@
 import os
 import shutil
 import socket
 import requests
 import jsonpickle
 
 from beeflow.common import log as bee_logging
-from beeflow.wf_manager.common import wf_db
 from beeflow.common.config_driver import BeeConfig as bc
 from beeflow.common.gdb_interface import GraphDatabaseInterface
 from beeflow.common.gdb.neo4j_driver import Neo4jDriver
 from beeflow.common.wf_interface import WorkflowInterface
 from beeflow.common.connection import Connection
 
+from beeflow.common.db import wfm_db
+from beeflow.common.db.bdb import connect_db
 
 log = bee_logging.setup(__name__)
 
 
+def get_db_path():
+    """Return db name."""
+    db_name = 'wfm.db'
+    bee_workdir = bc.get('DEFAULT', 'bee_workdir')
+    db_path = bee_workdir + '/' + db_name
+    return db_path
+
+
 def get_bee_workdir():
     """Get the bee workflow directory from the configuration file."""
-    return os.path.expanduser('~/.beeflow')
+    return bc.get('DEFAULT', 'bee_workdir')
 
 
 def get_workflows_dir():
     """Get the workflows script directory from beeflow."""
     bee_workdir = get_bee_workdir()
     workflows_dir = os.path.join(bee_workdir, 'workflows')
     return workflows_dir
@@ -57,22 +66,20 @@
 
 def remove_wf_dir(wf_id):
     """Remove a workflow directory."""
     bee_workdir = get_bee_workdir()
     workflows_dir = os.path.join(bee_workdir, 'workflows', wf_id)
     if os.path.exists(workflows_dir):
         shutil.rmtree(workflows_dir)
-    # wf_db.delete_workflow(wf_id)
 
 
 def create_wf_metadata(wf_id, wf_name):
     """Create workflow metadata files."""
     create_wf_name(wf_id, wf_name)
     create_wf_status(wf_id)
-    # wf_db.add_workflow(wf_id, wf_name, 'Pending')
 
 
 def create_wf_name(wf_id, wf_name):
     """Create workflow name metadata file."""
     bee_workdir = get_bee_workdir()
     workflows_dir = os.path.join(bee_workdir, 'workflows', wf_id)
     name_path = os.path.join(workflows_dir, 'bee_wf_name')
@@ -88,15 +95,14 @@
 def update_wf_status(wf_id, status_msg):
     """Update workflow status metadata file."""
     bee_workdir = get_bee_workdir()
     workflows_dir = os.path.join(bee_workdir, 'workflows', wf_id)
     status_path = os.path.join(workflows_dir, 'bee_wf_status')
     with open(status_path, 'w', encoding="utf8") as status:
         status.write(status_msg)
-    wf_db.update_workflow_state(wf_id, status_msg)
 
 
 def read_wf_status(wf_id):
     """Read workflow status metadata file."""
     bee_workdir = get_bee_workdir()
     workflows_dir = os.path.join(bee_workdir, 'workflows', wf_id)
     status_path = os.path.join(workflows_dir, 'bee_wf_status')
@@ -112,15 +118,16 @@
     name_path = os.path.join(workflows_dir, 'bee_wf_name')
     with open(name_path, 'w', encoding="utf8") as name:
         name.write(wf_name)
 
 
 def get_workflow_interface(wf_id):
     """Instantiate and return workflow interface object."""
-    bolt_port = wf_db.get_bolt_port(wf_id)
+    db = connect_db(wfm_db, get_db_path())
+    bolt_port = db.workflows.get_bolt_port(wf_id)
     try:
         driver = Neo4jDriver(user="neo4j", bolt_port=bolt_port,
                              db_hostname=bc.get("graphdb", "hostname"),
                              password=bc.get("graphdb", "dbpass"))
         iface = GraphDatabaseInterface(driver)
         wfi = WorkflowInterface(iface)
     except KeyError:
@@ -128,15 +135,16 @@
         # wfi = WorkflowInterface()
     return wfi
 
 
 def tm_url():
     """Get Task Manager url."""
     # tm_listen_port = bc.get('task_manager', 'listen_port')
-    tm_listen_port = wf_db.get_tm_port()
+    db = connect_db(wfm_db, get_db_path())
+    tm_listen_port = db.info.get_port('tm')
     task_manager = "bee_tm/v1/task/"
     return f'http://127.0.0.1:{tm_listen_port}/{task_manager}'
 
 
 # Base URLs for the TM and the Scheduler
 TM_URL = "bee_tm/v1/task/"
 SCHED_URL = "bee_sched/v1/"
@@ -145,17 +153,18 @@
 def _connect_tm():
     """Return a connection to the TM."""
     return Connection(bc.get('task_manager', 'socket'))
 
 
 def sched_url():
     """Get Scheduler url."""
+    db = connect_db(wfm_db, get_db_path())
     scheduler = "bee_sched/v1/"
     # sched_listen_port = bc.get('scheduler', 'listen_port')
-    sched_listen_port = wf_db.get_sched_port()
+    sched_listen_port = db.info.get_port('sched')
     return f'http://127.0.0.1:{sched_listen_port}/{scheduler}'
 
 
 def _connect_scheduler():
     """Return a connection to the Scheduler."""
     return Connection(bc.get('scheduler', 'socket'))
```

### Comparing `hpc-beeflow-0.1.3/beeflow/wf_manager/wf_manager.py` & `hpc_beeflow-0.1.4/beeflow/wf_manager/wf_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Start up the workflow manager connecting all of the endpoints."""
 
 from flask import Flask
 from beeflow.common.api import BeeApi
 
 from beeflow.wf_manager.resources.wf_list import WFList
 from beeflow.wf_manager.resources.wf_actions import WFActions
+from beeflow.wf_manager.resources.wf_metadata import WFMetadata
 from beeflow.wf_manager.resources.wf_update import WFUpdate
 
 from beeflow.wf_manager.resources import wf_utils
 
 
 def create_app():
     """Create flask app object and add REST endpoints."""
     app = Flask(__name__)
     api = BeeApi(app)
 
     # Add endpoints
     api.add_resource(WFList, '/bee_wfm/v1/jobs/')
     api.add_resource(WFActions, '/bee_wfm/v1/jobs/<string:wf_id>')
+    api.add_resource(WFMetadata, '/bee_wfm/v1/jobs/<string:wf_id>/metadata')
     api.add_resource(WFUpdate, '/bee_wfm/v1/jobs/update/')
     return app
 
 
 if __name__ == '__main__':
     flask_app = create_app()
     bee_workdir = wf_utils.get_bee_workdir()
```

### Comparing `hpc-beeflow-0.1.3/pyproject.toml` & `hpc_beeflow-0.1.4/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hpc-beeflow"
-version = "0.1.3"
+version = "0.1.4"
 description = "A software package for containerizing HPC applications and managing job workflow"
 
 
 authors = [
     "BEE-LANL Dev Team <bee-dev@lanl.gov>"
 ]
 
@@ -57,14 +57,16 @@
 Jinja2 = { version = "<3.1" }
 neo4j = { version = "^1.7.4" }
 PyYAML = { version = "^5.1.1" }
 flask_restful = "0.3.9"
 cwl-utils = "^0.16"
 APScheduler = "^3.6.3"
 jsonpickle = "^2.2.0"
+# Fix for urllib3 2.0 breaking change (similar error to this https://github.com/docker/docker-py/issues/3113)
+requests = "<2.29.0"
 requests-unixsocket = "^0.3.0"
 python-daemon = "^2.3.1"
 gunicorn = "^20.1.0"
 # typer version 0.6 and above seem to be throwing an AssertionError with no
 # attached info
 typer = "^0.5.0"
 
@@ -75,20 +77,22 @@
 
 [tool.poetry.extras]
 cloud_extras = ["google-api-python-client", "python-openstackclient", "python-heatclient"]
 
 [tool.poetry.dev-dependencies]
 # Developer dependencies
 pycodestyle = { version = ">=2.5.0" }
-pydocstyle = { version = ">=4.0.0" }
-pyflakes = { version = ">=2.1.1" }
-pylama = { version = ">=7.7.1" }
-pylint = { version = ">=2.3.1" }
-pytest = { version = ">=6.0.0" }
-pytest-mock = { version = ">=3.3.1" }
+# Newer version of pydocstyle break pylama
+pydocstyle = "6.1.1"
+pyflakes = "3.0.1"
+pylama = "8.4.1"
+pylint = "2.15.9"
+pytest = "7.2.0"
+pytest-mock = "3.3.1"
+# This is commented out until we can figure out why it's causing `poetry update` to loop forever
 sphinx = "^2.1"
 sphinx-rtd-theme = "^1.0"
 cwltool = "^3.0.20200324120055"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `hpc-beeflow-0.1.3/PKG-INFO` & `hpc_beeflow-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpc-beeflow
-Version: 0.1.3
+Version: 0.1.4
 Summary: A software package for containerizing HPC applications and managing job workflow
 Home-page: https://github.com/lanl/BEE
 Keywords: bee,hpc,workflow,cluster,computing
 Author: BEE-LANL Dev Team
 Author-email: bee-dev@lanl.gov
 Requires-Python: >=3.8.3,<=3.11
 Classifier: Environment :: Console
@@ -12,36 +12,39 @@
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Clustering
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
-Provides-Extra: cloud_extras
+Provides-Extra: cloud-extras
 Requires-Dist: APScheduler (>=3.6.3,<4.0.0)
 Requires-Dist: Flask (>=2.0,<3.0)
 Requires-Dist: Jinja2 (<3.1)
 Requires-Dist: PyYAML (>=5.1.1,<6.0.0)
 Requires-Dist: cwl-utils (>=0.16,<0.17)
 Requires-Dist: flask_restful (==0.3.9)
-Requires-Dist: google-api-python-client (>=2.66.0,<3.0.0); extra == "cloud_extras"
+Requires-Dist: google-api-python-client (>=2.66.0,<3.0.0) ; extra == "cloud-extras"
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: jsonpickle (>=2.2.0,<3.0.0)
 Requires-Dist: neo4j (>=1.7.4,<2.0.0)
 Requires-Dist: python-daemon (>=2.3.1,<3.0.0)
-Requires-Dist: python-heatclient (>=3.1.0,<4.0.0); extra == "cloud_extras"
-Requires-Dist: python-openstackclient (>=6.0.0,<7.0.0); extra == "cloud_extras"
+Requires-Dist: python-heatclient (>=3.1.0,<4.0.0) ; extra == "cloud-extras"
+Requires-Dist: python-openstackclient (>=6.0.0,<7.0.0) ; extra == "cloud-extras"
+Requires-Dist: requests (<2.29.0)
 Requires-Dist: requests-unixsocket (>=0.3.0,<0.4.0)
 Requires-Dist: typer (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://github.com/lanl/BEE
 Description-Content-Type: text/x-rst
 
 BEE: Build and Execution Environment
 ************************************
@@ -76,14 +79,37 @@
 Contact
 =======
 
 
 For bugs and problems report, suggestions and other general questions regarding the BEE project, email questions to `bee-dev@lanl.gov <bee-dev@lanl.gov>`_.
 
 
+Contributors:
+==========================
+
+* Steven Anaya - `Boogie3D <https://github.com/Boogie3D>`_
+* Paul Bryant - `paulbry <https://github.com/paulbry>`_
+* Rusty Davis - `rstyd <https://github.com/rstyd>`_
+* Jieyang Chen - `JieyangChen7 <https://github.com/JieyangChen7>`_
+* Patricia Grubel - `pagrubel <https://github.com/pagrubel>`_
+* Qiang Guan - `guanxyz <https://github.com/guanxyz>`_
+* Ragini Gupta - `raginigupta6 <https://github.com/raginigupta6>`_
+* Andres Quan - `aquan9 <https://github.com/aquan9>`_
+* Quincy Wofford - `qwofford <https://github.com/qwofford>`_
+* Tim Randles - `trandles-lanl <https://github.com/trandles-lanl>`_
+* Jacob Tronge - `jtronge <https://github.com/jtronge>`_
+
+Concept and Design Contributors
+
+* James Ahrens
+* Allen McPherson
+* Li-Ta Lo
+* Louis Vernon
+
+
 Contributing
 ==========================
 
 The BEE project adheres to style guidelines specified in `setup.cfg <https://github.com/lanl/BEE/blob/master/setup\.cfg>`_. Before attempting to commit and push changes, please install our pre-commit githooks by running the following command in project root:
 
 If using `git --version` >= 2.9:
     git config core.hooksPath .githooks
```

