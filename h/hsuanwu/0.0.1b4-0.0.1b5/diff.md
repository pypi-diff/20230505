# Comparing `tmp/hsuanwu-0.0.1b4.tar.gz` & `tmp/hsuanwu-0.0.1b5.tar.gz`

## Comparing `hsuanwu-0.0.1b4.tar` & `hsuanwu-0.0.1b5.tar`

### file list

```diff
@@ -1,227 +1,576 @@
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/ACKNOWLEDGMENT.md
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/CONTRIBUTING.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/Makefile
--rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/mkdocs.yml
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/FUNDING.yml
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/documentation.yml
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/question.yml
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/deployment/__init__.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/CNAME
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/benchmarks.md
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/changelog.md
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/contributing.md
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/generate_mkgendocs.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/getting_started.md
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/index.md
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/license.md
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/mkgendocs.yml
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/trigger.yml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/verification.md
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/contributing.md
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/index.md
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/logger.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/timer.md
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/__init__.md
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/base_policy_trainer.md
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/distributed_trainer.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/off_policy_trainer.md
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/on_policy_trainer.md
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/utils.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/atari/__init__.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/bullet/__init__.md
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/dmc/__init__.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/minigrid/__init__.md
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/procgen/__init__.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/evaluation/comparison.md
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/evaluation/performance.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/base.md
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/drqv2.md
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/impala.md
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/ppg.md
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/ppo.md
--rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/sac.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/base.md
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/espeholt_residual_encoder.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/identity_encoder.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/mnih_cnn_encoder.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/tassa_cnn_encoder.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/vanilla_mlp_encoder.md
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/distributed_storage.md
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/nstep_replay_storage.md
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/prioritized_replay_storage.md
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/vanilla_replay_storage.md
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/vanilla_rollout_storage.md
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/auto_augment.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/base.md
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/elastic_transform.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/gaussian_noise.md
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/grayscale.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_adjustsharpness.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_amplitude_scaling.md
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_augment.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_autocontrast.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_colorjitter.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_convolution.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_crop.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_cutout.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_cutoutcolor.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_equalize.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_flip.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_invert.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_perspective.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_rotate.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_shift.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_translate.md
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/base.md
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/categorical.md
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/diagonal_gaussian.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/kl.md
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/normal_noise.md
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/ornstein_uhlenbeck_noise.md
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/squashed_normal.md
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/truncated_normal_noise.md
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/base.md
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/girm.md
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/icm.md
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/ngu.md
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/pseudo_counts.md
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/re3.md
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/revd.md
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/ride.md
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/rise.md
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/rnd.md
--rw-r--r--   0        0        0    81827 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/github_issues.png
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/icon.svg
--rw-r--r--   0        0        0    94410 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/logo.png
--rw-r--r--   0        0        0   152927 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/qq.jpg
--rw-r--r--   0        0        0    70288 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/rl_training.png
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/roadmap.svg
--rw-r--r--   0        0        0    81227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/slack.png
--rw-r--r--   0        0        0    17517 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/structure.svg
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/stylesheets/extra.css
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/api.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/common_index/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/deployment_index/index.md
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/env_index/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/evaluation_index/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/pretraining_index/index.md
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/xploit_index/index.md
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/xplore_index/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/tutorials/configuration.md
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/tutorials/index.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/tutorials/quick_start.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/__init__.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/verification.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/__init__.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/logger.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/timer.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/__init__.py
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/base_policy_trainer.py
--rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/distributed_trainer.py
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/off_policy_trainer.py
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/on_policy_trainer.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/utils.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/__init__.py
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/utils.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/atari/__init__.py
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/atari/wrappers.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/bullet/__init__.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/dmc/__init__.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/dmc/natural_imgsource.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/dmc/wrappers.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/minigrid/__init__.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/procgen/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/__init__.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/comparison.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/performance.py
--rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/visualization.py
--rw-r--r--   0        0        0    16422 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/experimental/npu_ppo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/__init__.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/__init__.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/base.py
--rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/drqv2.py
--rw-r--r--   0        0        0    12307 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/impala.py
--rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/network.py
--rw-r--r--   0        0        0    15125 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/ppg.py
--rw-r--r--   0        0        0    10240 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/ppo.py
--rw-r--r--   0        0        0    13609 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/sac.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/utils.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/__init__.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/base.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/espeholt_residual_encoder.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/identity_encoder.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/mnih_cnn_encoder.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/tassa_cnn_encoder.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/vanilla_mlp_encoder.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/__init__.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/base.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/distributed_storage.py
--rw-r--r--   0        0        0     8793 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/nstep_replay_storage.py
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/prioritized_replay_storage.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/utils.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/vanilla_replay_storage.py
--rw-r--r--   0        0        0     7960 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/vanilla_rollout_storage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/__init__.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/auto_augment.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/base.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/elastic_transform.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/gaussian_noise.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/grayscale.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_adjustsharpness.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_amplitude_scaling.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_augment.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_autocontrast.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_colorjitter.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_convolution.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_crop.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_cutout.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_cutoutcolor.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_equalize.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_flip.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_invert.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_perspective.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_rotate.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_shift.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_translate.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/__init__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/base.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/categorical.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/diagonal_gaussian.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/kl.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/normal_noise.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/squashed_normal.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/truncated_normal_noise.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/utils.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/__init__.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/base.py
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/girm.py
--rw-r--r--   0        0        0     9843 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/icm.py
--rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/ngu.py
--rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/pseudo_counts.py
--rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/re3.py
--rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/revd.py
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/ride.py
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/rise.py
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/rnd.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/scripts/run_tests.sh
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_aug.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_dist.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_env.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_eval.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_logger.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_mp.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_reward.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_torch.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.gitignore
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/LICENSE
--rw-r--r--   0        0        0    12440 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/README.md
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/pyproject.toml
--rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/PKG-INFO
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/ACKNOWLEDGMENT.md
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/Makefile
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/mkdocs.yml
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.github/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.github/ISSUE_TEMPLATE/question.yml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/.gitignore
+-rw-r--r--   0        0        0    20667 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/.ninja_log
+-rw-r--r--   0        0        0    53272 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/build.ninja
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/default.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.__init__.imports
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.common.__init__.imports
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.common.engine.__init__.imports
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.common.engine.base_policy_trainer.imports
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.common.engine.distributed_trainer.imports
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.common.engine.off_policy_trainer.imports
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.common.engine.on_policy_trainer.imports
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.common.engine.utils.imports
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.common.logger.imports
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.common.timer.imports
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.__init__.imports
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.atari.__init__.imports
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.atari.wrappers.imports
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.bullet.__init__.imports
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.dmc.__init__.imports
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.dmc.natural_imgsource.imports
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.dmc.wrappers.imports
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.minigrid.__init__.imports
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.multibinary.__init__.imports
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.procgen.__init__.imports
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.env.utils.imports
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.evaluation.__init__.imports
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.evaluation.comparison.imports
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.evaluation.performance.imports
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.evaluation.utils.imports
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.evaluation.visualization.imports
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.verification.imports
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.__init__.imports
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.__init__.imports
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.base.imports
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.daac.imports
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.drqv2.imports
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.impala.imports
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.network.imports
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.ppg.imports
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.ppo.imports
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.sac.imports
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.agent.utils.imports
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.encoder.__init__.imports
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.encoder.base.imports
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.encoder.espeholt_residual_encoder.imports
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.encoder.identity_encoder.imports
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.encoder.mnih_cnn_encoder.imports
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.encoder.tassa_cnn_encoder.imports
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.encoder.vanilla_mlp_encoder.imports
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.storage.__init__.imports
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.storage.base.imports
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.storage.decoupled_rollout_storage.imports
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.storage.distributed_storage.imports
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.storage.nstep_replay_storage.imports
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.storage.prioritized_replay_storage.imports
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.storage.utils.imports
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.storage.vanilla_replay_storage.imports
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xploit.storage.vanilla_rollout_storage.imports
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.__init__.imports
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.__init__.imports
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.auto_augment.imports
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.base.imports
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.elastic_transform.imports
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.gaussian_noise.imports
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.grayscale.imports
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_adjustsharpness.imports
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_amplitude_scaling.imports
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_augment.imports
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_autocontrast.imports
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_colorjitter.imports
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_convolution.imports
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_crop.imports
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_cutout.imports
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_cutoutcolor.imports
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_equalize.imports
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_flip.imports
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_invert.imports
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_perspective.imports
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_rotate.imports
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_shift.imports
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.augmentation.random_translate.imports
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.__init__.imports
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.__init__.imports-1
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.base.imports
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.bernoulli.imports
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.bernoulli.imports-1
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.categorical.imports
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.categorical.imports-1
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.diagonal_gaussian.imports
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.kl.imports
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.kl.imports-1
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.normal_noise.imports
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.ornstein_uhlenbeck_noise.imports
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.squashed_normal.imports
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.truncated_normal_noise.imports
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.distribution.utils.imports
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.__init__.imports
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.__init__.imports-1
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.base.imports
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.girm.imports
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.icm.imports
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.ngu.imports
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.pseudo_counts.imports
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.pseudo_counts.imports-1
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.re3.imports
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.revd.imports
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.ride.imports
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.rise.imports
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/hsuanwu.xplore.reward.rnd.imports
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/imports/npu_ppo.imports
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/npu_ppo.pyi
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/__init__.pyi
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/verification.pyi
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/common/__init__.pyi
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/common/logger.pyi
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/common/timer.pyi
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/common/engine/__init__.pyi
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/common/engine/base_policy_trainer.pyi
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/common/engine/distributed_trainer.pyi
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/common/engine/off_policy_trainer.pyi
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/common/engine/on_policy_trainer.pyi
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/common/engine/utils.pyi
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/__init__.pyi
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/utils.pyi
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/atari/__init__.pyi
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/atari/wrappers.pyi
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/bullet/__init__.pyi
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/dmc/__init__.pyi
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/dmc/natural_imgsource.pyi
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/dmc/wrappers.pyi
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/minigrid/__init__.pyi
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/multibinary/__init__.pyi
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/env/procgen/__init__.pyi
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/evaluation/__init__.pyi
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/evaluation/comparison.pyi
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/evaluation/performance.pyi
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/evaluation/utils.pyi
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/evaluation/visualization.pyi
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/__init__.pyi
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/__init__.pyi
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/base.pyi
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/daac.pyi
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/drqv2.pyi
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/impala.pyi
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/network.pyi
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/ppg.pyi
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/ppo.pyi
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/sac.pyi
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/agent/utils.pyi
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/encoder/__init__.pyi
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/encoder/base.pyi
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/encoder/espeholt_residual_encoder.pyi
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/encoder/identity_encoder.pyi
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/encoder/mnih_cnn_encoder.pyi
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/encoder/tassa_cnn_encoder.pyi
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/encoder/vanilla_mlp_encoder.pyi
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/storage/__init__.pyi
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/storage/base.pyi
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/storage/decoupled_rollout_storage.pyi
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/storage/distributed_storage.pyi
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/storage/nstep_replay_storage.pyi
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/storage/prioritized_replay_storage.pyi
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/storage/utils.pyi
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/storage/vanilla_replay_storage.pyi
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xploit/storage/vanilla_rollout_storage.pyi
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/__init__.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/__init__.pyi
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/auto_augment.pyi
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/base.pyi
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/elastic_transform.pyi
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/gaussian_noise.pyi
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/grayscale.pyi
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_adjustsharpness.pyi
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_amplitude_scaling.pyi
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_augment.pyi
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_autocontrast.pyi
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_colorjitter.pyi
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_convolution.pyi
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_crop.pyi
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_cutout.pyi
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_cutoutcolor.pyi
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_equalize.pyi
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_flip.pyi
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_invert.pyi
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_perspective.pyi
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_rotate.pyi
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_shift.pyi
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/augmentation/random_translate.pyi
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/__init__.pyi
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/__init__.pyi-1
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/base.pyi
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/bernoulli.pyi
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/bernoulli.pyi-1
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/categorical.pyi
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/categorical.pyi-1
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/diagonal_gaussian.pyi
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/kl.pyi
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/kl.pyi-1
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/normal_noise.pyi
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.pyi
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/squashed_normal.pyi
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/truncated_normal_noise.pyi
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/distribution/utils.pyi
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/__init__.pyi
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/__init__.pyi-1
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/base.pyi
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/girm.pyi
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/icm.pyi
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/ngu.pyi
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/pseudo_counts.pyi
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/pseudo_counts.pyi-1
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/re3.pyi
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/revd.pyi
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/ride.pyi
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/rise.pyi
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.pytype/pyi/hsuanwu/xplore/reward/rnd.pyi
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/11a127456e8f30c6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/1371cdf75b5e614f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/1378ebcbf13907f7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/18c6c454bd09c6f4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/1928ebe40ed4d3e6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/19b01ebee9a847fc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/1ac3f1dff5514509
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/20f72ffab9266d40
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/2402c4b97d3f09cc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/25703fb8e0d412ed
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/26e9a832810a16e8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/2a834dddb817788d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/2b6abbe406fa41fa
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/2dbfcf93f6bdd315
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/2e983c5ee8042cc8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/30748b9b20c06f04
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/34a08899c82ea283
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/3523ddd70c69d114
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/3a2aeb401aa5991f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/3abebd99f5ad47a4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/40c1dbddc37b04fe
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/441fcc61aff03e1b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/4441d81b3e661991
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/445ea04da2a3bacc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/44b43d2630fd9430
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/4847c4aec4aaa172
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/4bd4eaff4992a4c4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/59723800dc929b59
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/5b53c8e441565201
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/5c4f9fd9cbb78abf
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/5c669560030d3a67
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/5c807d8515274d50
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/5ef70803f15d1104
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/60b3d436eec6030f
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/64636d41a5675c77
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/6606b0d7e42d048
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/69d0ebcf92933aa8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/6b6948608aedd884
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/6dadca91a3179b9f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/6e84dfb3d4996d6d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/6ed18032fcba04b6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/6f6c2abfb5b6777
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/72db8d8e3e62ae69
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/7346bb5817ff2b5d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/73980ebb0b054e20
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/75f7ae405e877754
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/771f44c75a7bfd7c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/7a3cb5faa7c3c0ed
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/7bc26babb9a80c14
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/7d3cfe104f8a504a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/7d5b5fa180e8d244
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/7fcdef529cb44e03
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/80fc0e1707464180
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/821aea47628edad
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/83125fbbf4fe5b2b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/84c1d6dfcb730d5e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/886def4e361bd39a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/8a2719f00eaae50c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/8d42d4741c5bb027
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/8e902be760538c4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/8f2fe811d3e35c80
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/8f817df801121b80
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/9144a7867bb3d059
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/9160d8fb873586ce
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/944359001305e29b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/94cd4cda5ef8a21
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/967617b29d420fad
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/97943038ba436d65
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/98bc2921877ecf8b
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/9b90c90ae6c659bb
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/a3d326c798befc0b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/a44e62719257af3c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/a56a52995c867c5d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/a7e529d7b1771bcf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/a8a6e9a44a28f421
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/a953ed284a246da3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/aab32152d4b6b5d5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/aad15c106c2fc98c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/ac1f46e25ff511e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/acdddd39ceae7e93
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/ad403a104ff7287f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/ad80e4b4d528c9ce
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/ae81fae1451238d5
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/b001523a9e6018cc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/b25dc6116e39efc4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/b34a7d80a1ebe835
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/b487473f3137324a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/b5b554889849c8b7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/b9cbfaaa63bb7e4b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/bafb69720f6f9ad
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/bba4ec6251c724ba
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/c0d467f210fb4818
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/c1fc77283d3629b0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/c27d95f344071688
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/c85305cbf817b695
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/c9bf0a3e1fdf3020
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/ca2344d18c07346b
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/ccbc3f26b049cd02
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/ccf9738ec3ed3b2b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/cdf980c872c4e39f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/cfef12ad0596f62c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/d32fe21965ece9b9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/d41b50d1d2b410f9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/d525cc7d3eac6a2b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/d6c3486270bc4595
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/d786538181238260
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/d7f7db139957a176
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/d924c5911df09674
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/dac5ca535e90a84c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/dbbac2ac859a29ee
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/e06608a8b7921615
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/e23fd6bcc5addced
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/e28d3058d69c2ed
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/ef87298fe9f7004e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/f2b82a7004ba2b58
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/f3c605b03f54e27e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/f4ed4f5ea102c073
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/f6146503e815a129
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/f732c3bf7137fcaa
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/f9edefbc5e4306ad
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/fa00f96ba1317110
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/fa105088cfed0718
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/fb49bbd32c9da8c5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.ruff_cache/content/ff0ba5f05bb815cf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/deployment/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/CNAME
+-rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api.md
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/benchmarks.md
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/changelog.md
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/contributing.md
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/generate_mkgendocs.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/getting_started.md
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/index.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/license.md
+-rw-r--r--   0        0        0    10057 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/mkgendocs.yml
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/trigger.yml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/verification.md
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/common/logger.md
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/common/timer.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/common/engine/__init__.md
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/common/engine/base_policy_trainer.md
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/common/engine/distributed_trainer.md
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/common/engine/off_policy_trainer.md
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/common/engine/on_policy_trainer.md
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/env/utils.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/env/atari/__init__.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/env/bullet/__init__.md
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/env/dmc/__init__.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/env/minigrid/__init__.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/env/multibinary/__init__.md
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/env/procgen/__init__.md
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/evaluation/comparison.md
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/evaluation/performance.md
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/evaluation/utils.md
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/base.md
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/daac.md
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/drqv2.md
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/impala.md
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/ppg.md
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/ppo.md
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/sac.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/base.md
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/espeholt_residual_encoder.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/identity_encoder.md
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/mnih_cnn_encoder.md
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/tassa_cnn_encoder.md
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/vanilla_mlp_encoder.md
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/base.md
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/decoupled_rollout_storage.md
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/distributed_storage.md
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/nstep_replay_storage.md
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/prioritized_replay_storage.md
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/vanilla_replay_storage.md
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/vanilla_rollout_storage.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/auto_augment.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/base.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/elastic_transform.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/gaussian_noise.md
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/grayscale.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_adjustsharpness.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_amplitude_scaling.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_augment.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_autocontrast.md
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_colorjitter.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_convolution.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_crop.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_cutout.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_cutoutcolor.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_equalize.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_flip.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_invert.md
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_perspective.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_rotate.md
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_shift.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_translate.md
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/base.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/bernoulli.md
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/categorical.md
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/diagonal_gaussian.md
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/kl.md
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/normal_noise.md
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/ornstein_uhlenbeck_noise.md
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/squashed_normal.md
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/truncated_normal_noise.md
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/base.md
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/girm.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/icm.md
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/ngu.md
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/pseudo_counts.md
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/re3.md
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/revd.md
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/ride.md
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/rise.md
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/rnd.md
+-rw-r--r--   0        0        0    81827 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/assets/images/github_issues.png
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/assets/images/icon.svg
+-rw-r--r--   0        0        0    94410 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/assets/images/logo.png
+-rw-r--r--   0        0        0   152927 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/assets/images/qq.jpg
+-rw-r--r--   0        0        0    81306 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/assets/images/rl_training.png
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/assets/images/roadmap.svg
+-rw-r--r--   0        0        0    81227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/assets/images/slack.png
+-rw-r--r--   0        0        0    17517 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/assets/images/structure.svg
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/assets/stylesheets/extra.css
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/tutorials/configuration.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/tutorials/custom_environment.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/tutorials/custom_module.md
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/tutorials/data_augmentation.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/tutorials/deployment.md
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/tutorials/evaluation.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/tutorials/index.md
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/tutorials/pre-training.md
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/docs/tutorials/quick_start.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/verification.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/common/__init__.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/common/logger.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/common/timer.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/common/engine/__init__.py
+-rw-r--r--   0        0        0    10028 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/common/engine/base_policy_trainer.py
+-rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/common/engine/distributed_trainer.py
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/common/engine/off_policy_trainer.py
+-rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/common/engine/on_policy_trainer.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/common/engine/utils.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/utils.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/atari/__init__.py
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/atari/wrappers.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/bullet/__init__.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/dmc/__init__.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/dmc/natural_imgsource.py
+-rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/dmc/wrappers.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/minigrid/__init__.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/multibinary/__init__.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/env/procgen/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/evaluation/__init__.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/evaluation/comparison.py
+-rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/evaluation/performance.py
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/evaluation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/evaluation/visualization.py
+-rw-r--r--   0        0        0    16422 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/experimental/npu_ppo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/__init__.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/__init__.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/base.py
+-rw-r--r--   0        0        0    13969 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/daac.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/drqv2.py
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/impala.py
+-rw-r--r--   0        0        0    23293 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/network.py
+-rw-r--r--   0        0        0    16866 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/ppg.py
+-rw-r--r--   0        0        0    11094 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/ppo.py
+-rw-r--r--   0        0        0    15469 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/sac.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/agent/utils.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/__init__.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/base.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/espeholt_residual_encoder.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/identity_encoder.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/mnih_cnn_encoder.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/tassa_cnn_encoder.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/vanilla_mlp_encoder.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/storage/__init__.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/storage/base.py
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/storage/decoupled_rollout_storage.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/storage/distributed_storage.py
+-rw-r--r--   0        0        0    10736 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/storage/nstep_replay_storage.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/storage/prioritized_replay_storage.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/storage/utils.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/storage/vanilla_replay_storage.py
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xploit/storage/vanilla_rollout_storage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/__init__.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/auto_augment.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/base.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/elastic_transform.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/gaussian_noise.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/grayscale.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_adjustsharpness.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_amplitude_scaling.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_augment.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_autocontrast.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_colorjitter.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_convolution.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_crop.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_cutout.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_cutoutcolor.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_equalize.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_flip.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_invert.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_perspective.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_rotate.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_shift.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_translate.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/base.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/bernoulli.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/categorical.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/diagonal_gaussian.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/kl.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/normal_noise.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/squashed_normal.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/truncated_normal_noise.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/utils.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/__init__.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/base.py
+-rw-r--r--   0        0        0    13143 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/girm.py
+-rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/icm.py
+-rw-r--r--   0        0        0    11038 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/ngu.py
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/pseudo_counts.py
+-rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/re3.py
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/revd.py
+-rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/ride.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/rise.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/hsuanwu/xplore/reward/rnd.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/scripts/run_tests.sh
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/tests/test_aug.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/tests/test_dist.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/tests/test_env.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/tests/test_eval.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/tests/test_logger.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/tests/test_mp.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/tests/test_reward.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/tests/test_torch.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/.gitignore
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/LICENSE
+-rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/README.md
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0    14255 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b5/PKG-INFO
```

### Comparing `hsuanwu-0.0.1b4/ACKNOWLEDGMENT.md` & `hsuanwu-0.0.1b5/ACKNOWLEDGMENT.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 - [auto-drac](https://github.com/rraileanu/auto-drac)
 - [pytorch-a2c-ppo-acktr-gail](https://github.com/ikostrikov/pytorch-a2c-ppo-acktr-gail)
 - [impact-driven-exploration](https://github.com/facebookresearch/impact-driven-exploration)
 - [deep_bisim4control](https://github.com/facebookresearch/deep_bisim4control)
 - [dm_control](https://github.com/deepmind/dm_control)
 - [gym](https://github.com/openai/gym)
 - [procgen](https://github.com/openai/procgen)
-- [bullet3](https://github.com/bulletphysics/bullet3)
+- [bullet3](https://github.com/bulletphysics/bullet3)
+- [rliable](Borrowed from: https://github.com/google-research/rliable)
```

### Comparing `hsuanwu-0.0.1b4/CODE_OF_CONDUCT.md` & `hsuanwu-0.0.1b5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/CONTRIBUTING.md` & `hsuanwu-0.0.1b5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/Makefile` & `hsuanwu-0.0.1b5/Makefile`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/.github/FUNDING.yml` & `hsuanwu-0.0.1b5/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/.github/PULL_REQUEST_TEMPLATE.md` & `hsuanwu-0.0.1b5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/bug_report.yml` & `hsuanwu-0.0.1b5/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/documentation.yml` & `hsuanwu-0.0.1b5/.github/ISSUE_TEMPLATE/documentation.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/feature_request.yml` & `hsuanwu-0.0.1b5/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/question.yml` & `hsuanwu-0.0.1b5/.github/ISSUE_TEMPLATE/question.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/.github/workflows/ci.yml` & `hsuanwu-0.0.1b5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/contributing.md` & `hsuanwu-0.0.1b5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/getting_started.md` & `hsuanwu-0.0.1b5/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/index.md` & `hsuanwu-0.0.1b5/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 - ⏱️ Latest algorithms and tricks;
 - 🧱 Highly modularized design for complete decoupling of RL algorithms;
 - 🚀 Optimized workflow for full hardware acceleration;
 - ⚙️ Support for custom environments;
 - 🖥️ Support for multiple computing devices like GPU and NPU;
 - 🛠️ Support for RL model engineering deployment (TensorRT, CANN, ...);
-- 💾 Large number of reusable bechmarks ([See HsuanwuHub](hub.hsuanwu.dev));
+- 💾 Large number of reusable bechmarks ([See HsuanwuHub](https://hub.hsuanwu.dev/));
 - 📋 Elegant experimental management powered by [Hydra](https://hydra.cc/).
 
 See the project structure below:
 <div align=center>
 <img src='./assets/images/structure.svg' style="width: 100%">
 </div>
```

#### html2text {}

```diff
@@ -18,16 +18,16 @@
 Hsuanwu, you can find everything you need in RL, such as training, evaluation,
 deployment, etc. The highlight features of Hsuanwu: - â±ï¸ Latest algorithms
 and tricks; - ð§± Highly modularized design for complete decoupling of RL
 algorithms; - ð Optimized workflow for full hardware acceleration; - âï¸
 Support for custom environments; - ð¥ï¸ Support for multiple computing
 devices like GPU and NPU; - ð ï¸ Support for RL model engineering deployment
 (TensorRT, CANN, ...); - ð¾ Large number of reusable bechmarks ([See
-HsuanwuHub](hub.hsuanwu.dev)); - ð Elegant experimental management powered
-by [Hydra](https://hydra.cc/). See the project structure below:
+HsuanwuHub](https://hub.hsuanwu.dev/)); - ð Elegant experimental management
+powered by [Hydra](https://hydra.cc/). See the project structure below:
                         [./assets/images/structure.svg]
 Hsuanwu evolves based on reinforcement learning algorithms and integrates
 latest tricks. The following figure demonstrates the main evolution roadmap of
 Hsuanwu:
                          [./assets/images/roadmap.svg]
 Join the developer community for issues and discussions: |Slack|QQ|GitHub| |:-:
 |:-:|:-:| |[./assets/images/slack.png]|[./assets/images/qq.jpg]|[./assets/
```

### Comparing `hsuanwu-0.0.1b4/docs/license.md` & `hsuanwu-0.0.1b5/docs/license.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/mkgendocs.yml` & `hsuanwu-0.0.1b5/docs/mkgendocs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,289 +1,314 @@
-sources_dir: docs/api
-templates_dir:
-repo: https://github.com/RLE-Foundation/Hsuanwu
-version: main
-pages:
-  - page: common/engine/base_policy_trainer.md
-    source: hsuanwu/common/engine/base_policy_trainer.py
-    classes:
-      - BasePolicyTrainer
-  - page: common/engine/distributed_trainer.md
-    source: hsuanwu/common/engine/distributed_trainer.py
-    classes:
-      - DistributedTrainer
-  - page: common/engine/__init__.md
-    source: hsuanwu/common/engine/__init__.py
-    classes:
-      - HsuanwuEngine
-  - page: common/engine/off_policy_trainer.md
-    source: hsuanwu/common/engine/off_policy_trainer.py
-    classes:
-      - OffPolicyTrainer
-  - page: common/engine/on_policy_trainer.md
-    source: hsuanwu/common/engine/on_policy_trainer.py
-    classes:
-      - OnPolicyTrainer
-  - page: common/logger.md
-    source: hsuanwu/common/logger.py
-    classes:
-      - Logger
-  - page: common/timer.md
-    source: hsuanwu/common/timer.py
-    classes:
-      - Timer
-  - page: xploit/encoder/base.md
-    source: hsuanwu/xploit/encoder/base.py
-    classes:
-      - BaseEncoder
-  - page: xploit/encoder/espeholt_residual_encoder.md
-    source: hsuanwu/xploit/encoder/espeholt_residual_encoder.py
-    classes:
-      - EspeholtResidualEncoder
-  - page: xploit/encoder/identity_encoder.md
-    source: hsuanwu/xploit/encoder/identity_encoder.py
-    classes:
-      - IdentityEncoder
-  - page: xploit/encoder/mnih_cnn_encoder.md
-    source: hsuanwu/xploit/encoder/mnih_cnn_encoder.py
-    classes:
-      - MnihCnnEncoder
-  - page: xploit/encoder/tassa_cnn_encoder.md
-    source: hsuanwu/xploit/encoder/tassa_cnn_encoder.py
-    classes:
-      - TassaCnnEncoder
-  - page: xploit/encoder/vanilla_mlp_encoder.md
-    source: hsuanwu/xploit/encoder/vanilla_mlp_encoder.py
-    classes:
-      - VanillaMlpEncoder
-  - page: xploit/agent/base.md
-    source: hsuanwu/xploit/agent/base.py
-    classes:
-      - BaseAgent
-  - page: xploit/agent/drqv2.md
-    source: hsuanwu/xploit/agent/drqv2.py
-    classes:
-      - DrQv2
-  - page: xploit/agent/impala.md
-    source: hsuanwu/xploit/agent/impala.py
-    classes:
-      - IMPALA
-  - page: xploit/agent/ppg.md
-    source: hsuanwu/xploit/agent/ppg.py
-    classes:
-      - PPG
-  - page: xploit/agent/ppo.md
-    source: hsuanwu/xploit/agent/ppo.py
-    classes:
-      - PPO
-  - page: xploit/agent/sac.md
-    source: hsuanwu/xploit/agent/sac.py
-    classes:
-      - SAC
-  - page: xploit/storage/distributed_storage.md
-    source: hsuanwu/xploit/storage/distributed_storage.py
-    classes:
-      - DistributedStorage
-  - page: xploit/storage/nstep_replay_storage.md
-    source: hsuanwu/xploit/storage/nstep_replay_storage.py
-    classes:
-      - NStepReplayStorage
-  - page: xploit/storage/prioritized_replay_storage.md
-    source: hsuanwu/xploit/storage/prioritized_replay_storage.py
-    classes:
-      - PrioritizedReplayStorage
-  - page: xploit/storage/vanilla_replay_storage.md
-    source: hsuanwu/xploit/storage/vanilla_replay_storage.py
-    classes:
-      - VanillaReplayStorage
-  - page: xploit/storage/vanilla_rollout_storage.md
-    source: hsuanwu/xploit/storage/vanilla_rollout_storage.py
-    classes:
-      - VanillaRolloutStorage
-  - page: xplore/reward/base.md
-    source: hsuanwu/xplore/reward/base.py
-    classes:
-      - BaseIntrinsicRewardModule
-  - page: xplore/reward/girm.md
-    source: hsuanwu/xplore/reward/girm.py
-    classes:
-      - GIRM
-  - page: xplore/reward/icm.md
-    source: hsuanwu/xplore/reward/icm.py
-    classes:
-      - ICM
-  - page: xplore/reward/ngu.md
-    source: hsuanwu/xplore/reward/ngu.py
-    classes:
-      - NGU
-  - page: xplore/reward/pseudo_counts.md
-    source: hsuanwu/xplore/reward/pseudo_counts.py
-    classes:
-      - PseudoCounts
-  - page: xplore/reward/re3.md
-    source: hsuanwu/xplore/reward/re3.py
-    classes:
-      - RE3
-  - page: xplore/reward/revd.md
-    source: hsuanwu/xplore/reward/revd.py
-    classes:
-      - REVD
-  - page: xplore/reward/ride.md
-    source: hsuanwu/xplore/reward/ride.py
-    classes:
-      - RIDE
-  - page: xplore/reward/rise.md
-    source: hsuanwu/xplore/reward/rise.py
-    classes:
-      - RISE
-  - page: xplore/reward/rnd.md
-    source: hsuanwu/xplore/reward/rnd.py
-    classes:
-      - RND
-  - page: xplore/augmentation/auto_augment.md
-    source: hsuanwu/xplore/augmentation/auto_augment.py
-    classes:
-      - AutoAugment
-  - page: xplore/augmentation/base.md
-    source: hsuanwu/xplore/augmentation/base.py
-    classes:
-      - BaseAugmentation
-  - page: xplore/augmentation/elastic_transform.md
-    source: hsuanwu/xplore/augmentation/elastic_transform.py
-    classes:
-      - ElasticTransform
-  - page: xplore/augmentation/gaussian_noise.md
-    source: hsuanwu/xplore/augmentation/gaussian_noise.py
-    classes:
-      - GaussianNoise
-  - page: xplore/augmentation/grayscale.md
-    source: hsuanwu/xplore/augmentation/grayscale.py
-    classes:
-      - GrayScale
-  - page: xplore/augmentation/random_adjustsharpness.md
-    source: hsuanwu/xplore/augmentation/random_adjustsharpness.py
-    classes:
-      - RandomAdjustSharpness
-  - page: xplore/augmentation/random_amplitude_scaling.md
-    source: hsuanwu/xplore/augmentation/random_amplitude_scaling.py
-    classes:
-      - RandomAmplitudeScaling
-  - page: xplore/augmentation/random_augment.md
-    source: hsuanwu/xplore/augmentation/random_augment.py
-    classes:
-      - RandomAugment
-  - page: xplore/augmentation/random_autocontrast.md
-    source: hsuanwu/xplore/augmentation/random_autocontrast.py
-    classes:
-      - RandomAutocontrast
-  - page: xplore/augmentation/random_colorjitter.md
-    source: hsuanwu/xplore/augmentation/random_colorjitter.py
-    classes:
-      - RandomColorJitter
-  - page: xplore/augmentation/random_convolution.md
-    source: hsuanwu/xplore/augmentation/random_convolution.py
-    classes:
-      - RandomConvolution
-  - page: xplore/augmentation/random_crop.md
-    source: hsuanwu/xplore/augmentation/random_crop.py
-    classes:
-      - RandomCrop
-  - page: xplore/augmentation/random_cutout.md
-    source: hsuanwu/xplore/augmentation/random_cutout.py
-    classes:
-      - RandomCutout
-  - page: xplore/augmentation/random_cutoutcolor.md
-    source: hsuanwu/xplore/augmentation/random_cutoutcolor.py
-    classes:
-      - RandomCutoutColor
-  - page: xplore/augmentation/random_equalize.md
-    source: hsuanwu/xplore/augmentation/random_equalize.py
-    classes:
-      - RandomEqualize
-  - page: xplore/augmentation/random_flip.md
-    source: hsuanwu/xplore/augmentation/random_flip.py
-    classes:
-      - RandomFlip
-  - page: xplore/augmentation/random_invert.md
-    source: hsuanwu/xplore/augmentation/random_invert.py
-    classes:
-      - RandomInvert
-  - page: xplore/augmentation/random_perspective.md
-    source: hsuanwu/xplore/augmentation/random_perspective.py
-    classes:
-      - RandomPerspective
-  - page: xplore/augmentation/random_rotate.md
-    source: hsuanwu/xplore/augmentation/random_rotate.py
-    classes:
-      - RandomRotate
-  - page: xplore/augmentation/random_shift.md
-    source: hsuanwu/xplore/augmentation/random_shift.py
-    classes:
-      - RandomShift
-  - page: xplore/augmentation/random_translate.md
-    source: hsuanwu/xplore/augmentation/random_translate.py
-    classes:
-      - RandomTranslate
-  - page: xplore/distribution/base.md
-    source: hsuanwu/xplore/distribution/base.py
-    classes:
-      - BaseDistribution
-  - page: xplore/distribution/categorical.md
-    source: hsuanwu/xplore/distribution/categorical.py
-    classes:
-      - Categorical
-  - page: xplore/distribution/diagonal_gaussian.md
-    source: hsuanwu/xplore/distribution/diagonal_gaussian.py
-    classes:
-      - DiagonalGaussian
-  - page: xplore/distribution/normal_noise.md
-    source: hsuanwu/xplore/distribution/normal_noise.py
-    classes:
-      - NormalNoise
-  - page: xplore/distribution/ornstein_uhlenbeck_noise.md
-    source: hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py
-    classes:
-      - OrnsteinUhlenbeckNoise
-  - page: xplore/distribution/squashed_normal.md
-    source: hsuanwu/xplore/distribution/squashed_normal.py
-    classes:
-      - SquashedNormal
-  - page: xplore/distribution/truncated_normal_noise.md
-    source: hsuanwu/xplore/distribution/truncated_normal_noise.py
-    classes:
-      - TruncatedNormalNoise
-  - page: xplore/distribution/kl.md
-    source: hsuanwu/xplore/distribution/kl.py
-    functions:
-      - kl_categorical_categorical
-  - page: env/utils.md
-    source: hsuanwu/env/utils.py
-    classes:
-      - HsuanwuEnvWrapper
-  - page: env/atari/__init__.md
-    source: hsuanwu/env/atari/__init__.py
-    functions:
-      - make_atari_env
-  - page: env/bullet/__init__.md
-    source: hsuanwu/env/bullet/__init__.py
-    functions:
-      - make_bullet_env
-  - page: env/dmc/__init__.md
-    source: hsuanwu/env/dmc/__init__.py
-    functions:
-      - make_dmc_env
-  - page: env/minigrid/__init__.md
-    source: hsuanwu/env/minigrid/__init__.py
-    functions:
-      - make_minigrid_env
-  - page: env/procgen/__init__.md
-    source: hsuanwu/env/procgen/__init__.py
-    functions:
-      - make_procgen_env
-  - page: evaluation/comparison.md
-    source: hsuanwu/evaluation/comparison.py
-    classes:
-      - Comparison
-  - page: evaluation/performance.md
-    source: hsuanwu/evaluation/performance.py
-    classes:
-      - Performance
+sources_dir: docs/api_docs
+templates_dir:
+repo: https://github.com/RLE-Foundation/Hsuanwu
+version: main
+pages:
+  - page: common/engine/base_policy_trainer.md
+    source: hsuanwu/common/engine/base_policy_trainer.py
+    classes:
+      - BasePolicyTrainer
+  - page: common/engine/distributed_trainer.md
+    source: hsuanwu/common/engine/distributed_trainer.py
+    classes:
+      - DistributedTrainer
+  - page: common/engine/__init__.md
+    source: hsuanwu/common/engine/__init__.py
+    classes:
+      - HsuanwuEngine
+  - page: common/engine/off_policy_trainer.md
+    source: hsuanwu/common/engine/off_policy_trainer.py
+    classes:
+      - OffPolicyTrainer
+  - page: common/engine/on_policy_trainer.md
+    source: hsuanwu/common/engine/on_policy_trainer.py
+    classes:
+      - OnPolicyTrainer
+  - page: common/logger.md
+    source: hsuanwu/common/logger.py
+    classes:
+      - Logger
+  - page: common/timer.md
+    source: hsuanwu/common/timer.py
+    classes:
+      - Timer
+  - page: xploit/encoder/base.md
+    source: hsuanwu/xploit/encoder/base.py
+    classes:
+      - BaseEncoder
+  - page: xploit/encoder/espeholt_residual_encoder.md
+    source: hsuanwu/xploit/encoder/espeholt_residual_encoder.py
+    classes:
+      - EspeholtResidualEncoder
+  - page: xploit/encoder/identity_encoder.md
+    source: hsuanwu/xploit/encoder/identity_encoder.py
+    classes:
+      - IdentityEncoder
+  - page: xploit/encoder/mnih_cnn_encoder.md
+    source: hsuanwu/xploit/encoder/mnih_cnn_encoder.py
+    classes:
+      - MnihCnnEncoder
+  - page: xploit/encoder/tassa_cnn_encoder.md
+    source: hsuanwu/xploit/encoder/tassa_cnn_encoder.py
+    classes:
+      - TassaCnnEncoder
+  - page: xploit/encoder/vanilla_mlp_encoder.md
+    source: hsuanwu/xploit/encoder/vanilla_mlp_encoder.py
+    classes:
+      - VanillaMlpEncoder
+  - page: xploit/agent/base.md
+    source: hsuanwu/xploit/agent/base.py
+    classes:
+      - BaseAgent
+  - page: xploit/agent/daac.md
+    source: hsuanwu/xploit/agent/daac.py
+    classes:
+      - DAAC
+  - page: xploit/agent/drqv2.md
+    source: hsuanwu/xploit/agent/drqv2.py
+    classes:
+      - DrQv2
+  - page: xploit/agent/impala.md
+    source: hsuanwu/xploit/agent/impala.py
+    classes:
+      - IMPALA
+  - page: xploit/agent/ppg.md
+    source: hsuanwu/xploit/agent/ppg.py
+    classes:
+      - PPG
+  - page: xploit/agent/ppo.md
+    source: hsuanwu/xploit/agent/ppo.py
+    classes:
+      - PPO
+  - page: xploit/agent/sac.md
+    source: hsuanwu/xploit/agent/sac.py
+    classes:
+      - SAC
+  - page: xploit/storage/base.md
+    source: hsuanwu/xploit/storage/base.py
+    classes:
+      - BaseStorage
+  - page: xploit/storage/decoupled_rollout_storage.md
+    source: hsuanwu/xploit/storage/decoupled_rollout_storage.py
+    classes:
+      - DecoupledRolloutStorage
+  - page: xploit/storage/distributed_storage.md
+    source: hsuanwu/xploit/storage/distributed_storage.py
+    classes:
+      - DistributedStorage
+  - page: xploit/storage/nstep_replay_storage.md
+    source: hsuanwu/xploit/storage/nstep_replay_storage.py
+    classes:
+      - NStepReplayStorage
+  - page: xploit/storage/prioritized_replay_storage.md
+    source: hsuanwu/xploit/storage/prioritized_replay_storage.py
+    classes:
+      - PrioritizedReplayStorage
+  - page: xploit/storage/vanilla_replay_storage.md
+    source: hsuanwu/xploit/storage/vanilla_replay_storage.py
+    classes:
+      - VanillaReplayStorage
+  - page: xploit/storage/vanilla_rollout_storage.md
+    source: hsuanwu/xploit/storage/vanilla_rollout_storage.py
+    classes:
+      - VanillaRolloutStorage
+  - page: xplore/reward/base.md
+    source: hsuanwu/xplore/reward/base.py
+    classes:
+      - BaseIntrinsicRewardModule
+  - page: xplore/reward/girm.md
+    source: hsuanwu/xplore/reward/girm.py
+    classes:
+      - GIRM
+  - page: xplore/reward/icm.md
+    source: hsuanwu/xplore/reward/icm.py
+    classes:
+      - ICM
+  - page: xplore/reward/ngu.md
+    source: hsuanwu/xplore/reward/ngu.py
+    classes:
+      - NGU
+  - page: xplore/reward/pseudo_counts.md
+    source: hsuanwu/xplore/reward/pseudo_counts.py
+    classes:
+      - PseudoCounts
+  - page: xplore/reward/re3.md
+    source: hsuanwu/xplore/reward/re3.py
+    classes:
+      - RE3
+  - page: xplore/reward/revd.md
+    source: hsuanwu/xplore/reward/revd.py
+    classes:
+      - REVD
+  - page: xplore/reward/ride.md
+    source: hsuanwu/xplore/reward/ride.py
+    classes:
+      - RIDE
+  - page: xplore/reward/rise.md
+    source: hsuanwu/xplore/reward/rise.py
+    classes:
+      - RISE
+  - page: xplore/reward/rnd.md
+    source: hsuanwu/xplore/reward/rnd.py
+    classes:
+      - RND
+  - page: xplore/augmentation/auto_augment.md
+    source: hsuanwu/xplore/augmentation/auto_augment.py
+    classes:
+      - AutoAugment
+  - page: xplore/augmentation/base.md
+    source: hsuanwu/xplore/augmentation/base.py
+    classes:
+      - BaseAugmentation
+  - page: xplore/augmentation/elastic_transform.md
+    source: hsuanwu/xplore/augmentation/elastic_transform.py
+    classes:
+      - ElasticTransform
+  - page: xplore/augmentation/gaussian_noise.md
+    source: hsuanwu/xplore/augmentation/gaussian_noise.py
+    classes:
+      - GaussianNoise
+  - page: xplore/augmentation/grayscale.md
+    source: hsuanwu/xplore/augmentation/grayscale.py
+    classes:
+      - GrayScale
+  - page: xplore/augmentation/random_adjustsharpness.md
+    source: hsuanwu/xplore/augmentation/random_adjustsharpness.py
+    classes:
+      - RandomAdjustSharpness
+  - page: xplore/augmentation/random_amplitude_scaling.md
+    source: hsuanwu/xplore/augmentation/random_amplitude_scaling.py
+    classes:
+      - RandomAmplitudeScaling
+  - page: xplore/augmentation/random_augment.md
+    source: hsuanwu/xplore/augmentation/random_augment.py
+    classes:
+      - RandomAugment
+  - page: xplore/augmentation/random_autocontrast.md
+    source: hsuanwu/xplore/augmentation/random_autocontrast.py
+    classes:
+      - RandomAutocontrast
+  - page: xplore/augmentation/random_colorjitter.md
+    source: hsuanwu/xplore/augmentation/random_colorjitter.py
+    classes:
+      - RandomColorJitter
+  - page: xplore/augmentation/random_convolution.md
+    source: hsuanwu/xplore/augmentation/random_convolution.py
+    classes:
+      - RandomConvolution
+  - page: xplore/augmentation/random_crop.md
+    source: hsuanwu/xplore/augmentation/random_crop.py
+    classes:
+      - RandomCrop
+  - page: xplore/augmentation/random_cutout.md
+    source: hsuanwu/xplore/augmentation/random_cutout.py
+    classes:
+      - RandomCutout
+  - page: xplore/augmentation/random_cutoutcolor.md
+    source: hsuanwu/xplore/augmentation/random_cutoutcolor.py
+    classes:
+      - RandomCutoutColor
+  - page: xplore/augmentation/random_equalize.md
+    source: hsuanwu/xplore/augmentation/random_equalize.py
+    classes:
+      - RandomEqualize
+  - page: xplore/augmentation/random_flip.md
+    source: hsuanwu/xplore/augmentation/random_flip.py
+    classes:
+      - RandomFlip
+  - page: xplore/augmentation/random_invert.md
+    source: hsuanwu/xplore/augmentation/random_invert.py
+    classes:
+      - RandomInvert
+  - page: xplore/augmentation/random_perspective.md
+    source: hsuanwu/xplore/augmentation/random_perspective.py
+    classes:
+      - RandomPerspective
+  - page: xplore/augmentation/random_rotate.md
+    source: hsuanwu/xplore/augmentation/random_rotate.py
+    classes:
+      - RandomRotate
+  - page: xplore/augmentation/random_shift.md
+    source: hsuanwu/xplore/augmentation/random_shift.py
+    classes:
+      - RandomShift
+  - page: xplore/augmentation/random_translate.md
+    source: hsuanwu/xplore/augmentation/random_translate.py
+    classes:
+      - RandomTranslate
+  - page: xplore/distribution/base.md
+    source: hsuanwu/xplore/distribution/base.py
+    classes:
+      - BaseDistribution
+  - page: xplore/distribution/bernoulli.md
+    source: hsuanwu/xplore/distribution/bernoulli.py
+    classes:
+      - Bernoulli
+  - page: xplore/distribution/categorical.md
+    source: hsuanwu/xplore/distribution/categorical.py
+    classes:
+      - Categorical
+  - page: xplore/distribution/diagonal_gaussian.md
+    source: hsuanwu/xplore/distribution/diagonal_gaussian.py
+    classes:
+      - DiagonalGaussian
+  - page: xplore/distribution/normal_noise.md
+    source: hsuanwu/xplore/distribution/normal_noise.py
+    classes:
+      - NormalNoise
+  - page: xplore/distribution/ornstein_uhlenbeck_noise.md
+    source: hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py
+    classes:
+      - OrnsteinUhlenbeckNoise
+  - page: xplore/distribution/squashed_normal.md
+    source: hsuanwu/xplore/distribution/squashed_normal.py
+    classes:
+      - SquashedNormal
+  - page: xplore/distribution/truncated_normal_noise.md
+    source: hsuanwu/xplore/distribution/truncated_normal_noise.py
+    classes:
+      - TruncatedNormalNoise
+  - page: xplore/distribution/kl.md
+    source: hsuanwu/xplore/distribution/kl.py
+    functions:
+      - kl_categorical_categorical
+      - kl_diagonal_gaussian_diagonal_gaussian
+  - page: env/utils.md
+    source: hsuanwu/env/utils.py
+    classes:
+      - HsuanwuEnvWrapper
+  - page: env/atari/__init__.md
+    source: hsuanwu/env/atari/__init__.py
+    functions:
+      - make_atari_env
+  - page: env/bullet/__init__.md
+    source: hsuanwu/env/bullet/__init__.py
+    functions:
+      - make_bullet_env
+  - page: env/dmc/__init__.md
+    source: hsuanwu/env/dmc/__init__.py
+    functions:
+      - make_dmc_env
+  - page: env/minigrid/__init__.md
+    source: hsuanwu/env/minigrid/__init__.py
+    functions:
+      - make_minigrid_env
+  - page: env/multibinary/__init__.md
+    source: hsuanwu/env/multibinary/__init__.py
+    functions:
+      - make_multibinary_env
+  - page: env/procgen/__init__.md
+    source: hsuanwu/env/procgen/__init__.py
+    functions:
+      - make_procgen_env
+  - page: evaluation/comparison.md
+    source: hsuanwu/evaluation/comparison.py
+    classes:
+      - Comparison
+  - page: evaluation/performance.md
+    source: hsuanwu/evaluation/performance.py
+    classes:
+      - Performance
+  - page: evaluation/utils.md
+    source: hsuanwu/evaluation/utils.py
+    functions:
+      - min_max_normalize
```

### Comparing `hsuanwu-0.0.1b4/docs/verification.md` & `hsuanwu-0.0.1b5/docs/verification.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/api/index.md` & `hsuanwu-0.0.1b5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - 🚀 Optimized workflow for full hardware acceleration;
 - ⚙️ Support for custom environments;
 - 🖥️ Support for multiple computing devices like GPU and NPU;
 - 🛠️ Support for RL model engineering deployment (TensorRT, CANN, ...);
 - 💾 Large number of reusable bechmarks ([See HsuanwuHub](hub.hsuanwu.dev));
 - 📋 Elegant experimental management powered by [Hydra](https://hydra.cc/).
 
-Join the development community for issues and discussions:
+Join the developer community for issues and discussions:
 |Slack|QQ|GitHub|
 |:-:|:-:|:-:|
 |<a href="https://app.slack.com/client/T054J4NJXP0/C054T78QZ9A"><img src='./docs/assets/images/slack.png' style="width: 50%" ></a>|<img src='./docs/assets/images/qq.jpg' style="width: 65%">|<a href="https://github.com/RLE-Foundation/Hsuanwu/issues"><img src='./docs/assets/images/github_issues.png' style="width: 50%"></a>|
 
 
 
 <!-- Please cite the following paper if you use Hsuanwu in your work, thank you!
@@ -36,21 +36,24 @@
 - [Quick Start](#quick-start)
   - [Installation](#installation)
   - [Build your first Hsuanwu application](#build-your-first-hsuanwu-application)
 - [Implemented Modules](#implemented-modules)
   - [Roadmap](#roadmap)
   - [Project Structure](#project-structure)
   - [RL Agents](#rl-agents)
+  - [Intrinsic Reward Modules](#intrinsic-reward-modules)
 - [Model Zoo](#model-zoo)
 - [API Documentation](#api-documentation)
 - [How To Contribute](#how-to-contribute)
 - [Acknowledgment](#acknowledgment)
 
 # Quick Start
 ## Installation
+- Prerequisites
+
 Currently, Hsuanwu requires `Python>=3.8`, user can create an virtual environment by
 ``` sh
 conda create -n hsuanwu python=3.8
 ```
 
 - with pip `recommended`
 
@@ -130,60 +133,78 @@
 
 See the project structure below:
 <div align=center>
 <img src='./docs/assets/images/structure.svg' style="width: 90%">
 </div>
 
 - **[Common](https://docs.hsuanwu.dev/common_index/)**: Auxiliary modules like trainer and logger.
-    + **Engine**: Engine for building Hsuanwu application.
-    + **Logger**: Logger for managing output information.
+    + **Engine**: *Engine for building Hsuanwu application.*
+    + **Logger**: *Logger for managing output information.*
 
 - **[Xploit](https://docs.hsuanwu.dev/xploit_index/)**: Modules that focus on <font color="#B80000"><b>exploitation</b></font> in RL.
     + **Encoder**: *Neural nework-based encoder for processing observations.*
     + **Agent**: *Agent for interacting and learning.*
     + **Storage**: *Storage for storing collected experiences.*
 
 - **[Xplore](https://docs.hsuanwu.dev/xplore_index/)**: Modules that focus on <font color="#B80000"><b>exploration</b></font> in RL.
-    + **Augmentation**: PyTorch.nn-like modules for observation augmentation.
-    + **Distribution**: Distributions for sampling actions.
-    + **Reward**: Intrinsic reward modules for enhancing exploration.
+    + **Augmentation**: *PyTorch.nn-like modules for observation augmentation.*
+    + **Distribution**: *Distributions for sampling actions.*
+    + **Reward**: *Intrinsic reward modules for enhancing exploration.*
 
 - **[Evaluation](https://docs.hsuanwu.dev/evaluation_index/)**: Reasonable and reliable metrics for algorithm evaluation.
 
 - **[Env](https://docs.hsuanwu.dev/env_index/)**: Packaged environments (e.g., Atari games) for fast invocation.
 
 - **[Pre-training](https://docs.hsuanwu.dev/pretraining_index/)**: Methods of <font color="#B80000"><b>pre-training</b></font> in RL.
 
 - **[Deployment](https://docs.hsuanwu.dev/deployment_index/)**: Methods of <font color="#B80000"><b>model deployment</b></font> in RL.
 
-For more detiled descriptions of these modules, see [https://docs.hsuanwu.dev/api](https://docs.hsuanwu.dev/overview/api)
+For more detiled descriptions of these modules, see [https://docs.hsuanwu.dev/api](https://docs.hsuanwu.dev/api)
 
 ## RL Agents
 |Module|Recurrent|Box|Discrete|MultiBinary|Multi Processing|NPU|Paper|Citations|
 |:-|:-|:-|:-|:-|:-|:-|:-|:-|
 |SAC|❌| ✔️ |❌|❌|❌|🐌 | [Link](http://proceedings.mlr.press/v80/haarnoja18b/haarnoja18b.pdf) |5077⭐|
 |DrQ|❌| ✔️ |❌|❌|❌|🐌 | [Link](https://arxiv.org/pdf/2004.13649) |433⭐|
 |DDPG|❌| ✔️ |❌|❌|❌|🐌 | [Link](https://arxiv.org/pdf/1509.02971.pdf?source=post_page---------------------------) |11819⭐|
 |DrQ-v2|❌| ✔️ |❌|❌|❌|🐌 | [Link](https://arxiv.org/pdf/2107.09645.pdf?utm_source=morioh.com) |100⭐|
-|PPO|❌| ✔️ |✔️|🐌|✔️|🐌 | [Link](https://arxiv.org/pdf/1707.06347) |11155⭐|
-|DrAC|❌| ✔️ |✔️|🐌|✔️|🐌 | [Link](https://proceedings.neurips.cc/paper/2021/file/2b38c2df6a49b97f706ec9148ce48d86-Paper.pdf) |29⭐|
-|PPG|❌| ✔️ |✔️|🐌|✔️|🐌| [Link](http://proceedings.mlr.press/v139/cobbe21a/cobbe21a.pdf) |82⭐|
-|IMPALA|✔️| ✔️ |✔️|🐌|✔️|🐌| [Link](http://proceedings.mlr.press/v80/espeholt18a/espeholt18a.pdf) |1219⭐|
+|PPO|❌| ✔️ |✔️|✔️|✔️|🐌 | [Link](https://arxiv.org/pdf/1707.06347) |11155⭐|
+|DAAC|❌| ✔️ |✔️|✔️|✔️|🐌 | [Link](http://proceedings.mlr.press/v139/raileanu21a/raileanu21a.pdf) |56⭐|
+|DrAC|❌| ✔️ |✔️|✔️|✔️|🐌 | [Link](https://proceedings.neurips.cc/paper/2021/file/2b38c2df6a49b97f706ec9148ce48d86-Paper.pdf) |29⭐|
+|PPG|❌| ✔️ |✔️|❌|✔️|🐌| [Link](http://proceedings.mlr.press/v139/cobbe21a/cobbe21a.pdf) |82⭐|
+|IMPALA|✔️| ✔️ |✔️|❌|✔️|🐌| [Link](http://proceedings.mlr.press/v80/espeholt18a/espeholt18a.pdf) |1219⭐|
 
 > - 🐌: Developing.
 > - `NPU`: Support Neural-network processing unit.
 > - `Recurrent`: Support recurrent neural network.
 > - `Box`: A N-dimensional box that containes every point in the action space.
 > - `Discrete`: A list of possible actions, where each timestep only one of the actions can be used.
 > - `MultiBinary`: A list of possible actions, where each timestep any of the actions can be used in any combination.
 
+## Intrinsic Reward Modules
+| Module | Remark | Repr.  | Visual | Reference | 
+|:-|:-|:-|:-|:-|
+| PseudoCounts | Count-Based exploration |✔️|✔️|[Never Give Up: Learning Directed Exploration Strategies](https://arxiv.org/pdf/2002.06038) |
+| ICM  | Curiosity-driven exploration  | ✔️|✔️| [Curiosity-Driven Exploration by Self-Supervised Prediction](http://proceedings.mlr.press/v70/pathak17a/pathak17a.pdf) | 
+| RND  | Count-based exploration  | ❌|✔️| [Exploration by Random Network Distillation](https://arxiv.org/pdf/1810.12894.pdf) | 
+| GIRM | Curiosity-driven exploration  | ✔️ |✔️| [Intrinsic Reward Driven Imitation Learning via Generative Model](http://proceedings.mlr.press/v119/yu20d/yu20d.pdf)|
+| NGU | Memory-based exploration  | ✔️  |✔️| [Never Give Up: Learning Directed Exploration Strategies](https://arxiv.org/pdf/2002.06038) | 
+| RIDE| Procedurally-generated environment | ✔️ |✔️| [RIDE: Rewarding Impact-Driven Exploration for Procedurally-Generated Environments](https://arxiv.org/pdf/2002.12292)|
+| RE3  | Entropy Maximization | ❌ |✔️| [State Entropy Maximization with Random Encoders for Efficient Exploration](http://proceedings.mlr.press/v139/seo21a/seo21a.pdf) |
+| RISE  | Entropy Maximization  | ❌  |✔️| [Rényi State Entropy Maximization for Exploration Acceleration in Reinforcement Learning](https://ieeexplore.ieee.org/abstract/document/9802917/) | 
+| REVD  | Divergence Maximization | ❌  |✔️| [Rewarding Episodic Visitation Discrepancy for Exploration in Reinforcement Learning](https://openreview.net/pdf?id=V2pw1VYMrDo)|
+
+> - 🐌: Developing.
+> - `Repr.`: The method involves representation learning.
+> - `Visual`: The method works well in visual RL.
 
+See [Tutorials: Use intrinsic reward and observation augmentation](https://docs.hsuanwu.dev/tutorials/data_augmentation.md) for usage examples.
 
 # Model Zoo
-Hsuanwu provides a large number of reusable bechmarks, see [https://hub.hsuanwu.dev/](https://hub.hsuanwu.dev/)
+Hsuanwu provides a large number of reusable bechmarks, see [https://hub.hsuanwu.dev/](https://hub.hsuanwu.dev/) and [https://docs.hsuanwu.dev/benchmarks/](https://docs.hsuanwu.dev/benchmarks/)
 
 # API Documentation
 View our well-designed documentation: [https://docs.hsuanwu.dev/](https://docs.hsuanwu.dev/)
 
 # How To Contribute
 Welcome to contribute to this project! Before you begin writing code, please read [CONTRIBUTING.md](https://github.com/RLE-Foundation/Hsuanwu/blob/main/CONTRIBUTING.md) for guide first.
```

#### html2text {}

```diff
@@ -18,103 +18,132 @@
 deployment, etc. The highlight features of Hsuanwu: - â±ï¸ Latest algorithms
 and tricks; - ð§± Highly modularized design for complete decoupling of RL
 algorithms; - ð Optimized workflow for full hardware acceleration; - âï¸
 Support for custom environments; - ð¥ï¸ Support for multiple computing
 devices like GPU and NPU; - ð ï¸ Support for RL model engineering deployment
 (TensorRT, CANN, ...); - ð¾ Large number of reusable bechmarks ([See
 HsuanwuHub](hub.hsuanwu.dev)); - ð Elegant experimental management powered
-by [Hydra](https://hydra.cc/). Join the development community for issues and
+by [Hydra](https://hydra.cc/). Join the developer community for issues and
 discussions: |Slack|QQ|GitHub| |:-:|:-:|:-:| |[./docs/assets/images/slack.png]|
 [./docs/assets/images/qq.jpg]|[./docs/assets/images/github_issues.png]|  -
 [Quick Start](#quick-start) - [Installation](#installation) - [Build your first
 Hsuanwu application](#build-your-first-hsuanwu-application) - [Implemented
 Modules](#implemented-modules) - [Roadmap](#roadmap) - [Project Structure]
-(#project-structure) - [RL Agents](#rl-agents) - [Model Zoo](#model-zoo) - [API
-Documentation](#api-documentation) - [How To Contribute](#how-to-contribute) -
-[Acknowledgment](#acknowledgment) # Quick Start ## Installation Currently,
-Hsuanwu requires `Python>=3.8`, user can create an virtual environment by ```
-sh conda create -n hsuanwu python=3.8 ``` - with pip `recommended` Open up a
-terminal and install **Hsuanwu** with `pip`: ``` shell pip install hsuanwu #
-basic installation pip install hsuanwu[envs] # for pre-defined environments pip
-install hsuanwu[tests] # for project tests pip install hsuanwu[all] # install
-all the dependencies ``` - with git Open up a terminal and clone the repository
-from [GitHub](https://github.com/RLE-Foundation/Hsuanwu) with `git`: ``` sh git
-clone https://github.com/RLE-Foundation/Hsuanwu.git ``` After that, run the
-following command to install package and dependencies: ``` sh pip install -e .
-# basic installation pip install -e .[envs] # for pre-defined environments pip
-install -e .[tests] # for project tests pip install -e .[all] # install all the
-dependencies ``` For more detailed installation instruction, see [https://
-docs.hsuanwu.dev/getting_started](https://docs.hsuanwu.dev/getting_started). ##
-Build your first Hsuanwu application For example, we want to use [DrQ-v2]
-(https://openreview.net/forum?id=_SJ-_yyes8) to solve a task of [DeepMind
-Control Suite](https://github.com/deepmind/dm_control), and we only need the
-following two steps: 1. Write a `config.yaml` file in your working directory
-like: ``` yaml experiment: drqv2_dmc # Experiment ID. device: cuda:0 # Device
-(cpu, cuda, ...) on which the code should be run. seed: 1 # Random seed for
-reproduction. num_train_steps: 250000 # Number of training steps. agent: name:
-DrQv2 # The agent name. ``` 2. Write a `train.py` file like: ``` python import
-hydra # Use Hydra to manage experiments from hsuanwu.env import make_dmc_env #
-Import DeepMind Control Suite from hsuanwu.common.engine import HsuanwuEngine #
-Import Hsuanwu engine train_env = make_dmc_env(env_id='cartpole_balance') #
-Create train env test_env = make_dmc_env(env_id='cartpole_balance') # Create
-test env @hydra.main(version_base=None, config_path='./', config_name='config')
-def main(cfgs): engine = HsuanwuEngine(cfgs=cfgs, train_env=train_env,
+(#project-structure) - [RL Agents](#rl-agents) - [Intrinsic Reward Modules]
+(#intrinsic-reward-modules) - [Model Zoo](#model-zoo) - [API Documentation]
+(#api-documentation) - [How To Contribute](#how-to-contribute) -
+[Acknowledgment](#acknowledgment) # Quick Start ## Installation - Prerequisites
+Currently, Hsuanwu requires `Python>=3.8`, user can create an virtual
+environment by ``` sh conda create -n hsuanwu python=3.8 ``` - with pip
+`recommended` Open up a terminal and install **Hsuanwu** with `pip`: ``` shell
+pip install hsuanwu # basic installation pip install hsuanwu[envs] # for pre-
+defined environments pip install hsuanwu[tests] # for project tests pip install
+hsuanwu[all] # install all the dependencies ``` - with git Open up a terminal
+and clone the repository from [GitHub](https://github.com/RLE-Foundation/
+Hsuanwu) with `git`: ``` sh git clone https://github.com/RLE-Foundation/
+Hsuanwu.git ``` After that, run the following command to install package and
+dependencies: ``` sh pip install -e . # basic installation pip install -e .
+[envs] # for pre-defined environments pip install -e .[tests] # for project
+tests pip install -e .[all] # install all the dependencies ``` For more
+detailed installation instruction, see [https://docs.hsuanwu.dev/
+getting_started](https://docs.hsuanwu.dev/getting_started). ## Build your first
+Hsuanwu application For example, we want to use [DrQ-v2](https://
+openreview.net/forum?id=_SJ-_yyes8) to solve a task of [DeepMind Control Suite]
+(https://github.com/deepmind/dm_control), and we only need the following two
+steps: 1. Write a `config.yaml` file in your working directory like: ``` yaml
+experiment: drqv2_dmc # Experiment ID. device: cuda:0 # Device (cpu, cuda, ...)
+on which the code should be run. seed: 1 # Random seed for reproduction.
+num_train_steps: 250000 # Number of training steps. agent: name: DrQv2 # The
+agent name. ``` 2. Write a `train.py` file like: ``` python import hydra # Use
+Hydra to manage experiments from hsuanwu.env import make_dmc_env # Import
+DeepMind Control Suite from hsuanwu.common.engine import HsuanwuEngine # Import
+Hsuanwu engine train_env = make_dmc_env(env_id='cartpole_balance') # Create
+train env test_env = make_dmc_env(env_id='cartpole_balance') # Create test env
+@hydra.main(version_base=None, config_path='./', config_name='config') def main
+(cfgs): engine = HsuanwuEngine(cfgs=cfgs, train_env=train_env,
 test_env=test_env) # Initialize engine engine.invoke() # Start training if
 __name__ == '__main__': main() ``` Run `train.py` and you will see the
 following output:
                     [./docs/assets/images/rl_training.png]
 For more detailed tutorials, see [https://docs.hsuanwu.dev/tutorials](https://
 docs.hsuanwu.dev/tutorials). # Implemented Modules ## Roadmap Hsuanwu evolves
 based on reinforcement learning algorithms and integrates latest tricks. The
 following figure demonstrates the main evolution roadmap of Hsuanwu:
                       [./docs/assets/images/roadmap.svg]
 ## Project Structure See the project structure below:
                      [./docs/assets/images/structure.svg]
 - **[Common](https://docs.hsuanwu.dev/common_index/)**: Auxiliary modules like
-trainer and logger. + **Engine**: Engine for building Hsuanwu application. +
-**Logger**: Logger for managing output information. - **[Xploit](https://
+trainer and logger. + **Engine**: *Engine for building Hsuanwu application.* +
+**Logger**: *Logger for managing output information.* - **[Xploit](https://
 docs.hsuanwu.dev/xploit_index/)**: Modules that focus on exploitation in RL. +
 **Encoder**: *Neural nework-based encoder for processing observations.* +
 **Agent**: *Agent for interacting and learning.* + **Storage**: *Storage for
 storing collected experiences.* - **[Xplore](https://docs.hsuanwu.dev/
 xplore_index/)**: Modules that focus on exploration in RL. + **Augmentation**:
-PyTorch.nn-like modules for observation augmentation. + **Distribution**:
-Distributions for sampling actions. + **Reward**: Intrinsic reward modules for
-enhancing exploration. - **[Evaluation](https://docs.hsuanwu.dev/
+*PyTorch.nn-like modules for observation augmentation.* + **Distribution**:
+*Distributions for sampling actions.* + **Reward**: *Intrinsic reward modules
+for enhancing exploration.* - **[Evaluation](https://docs.hsuanwu.dev/
 evaluation_index/)**: Reasonable and reliable metrics for algorithm evaluation.
 - **[Env](https://docs.hsuanwu.dev/env_index/)**: Packaged environments (e.g.,
 Atari games) for fast invocation. - **[Pre-training](https://docs.hsuanwu.dev/
 pretraining_index/)**: Methods of pre-training in RL. - **[Deployment](https://
 docs.hsuanwu.dev/deployment_index/)**: Methods of model deployment in RL. For
 more detiled descriptions of these modules, see [https://docs.hsuanwu.dev/api]
-(https://docs.hsuanwu.dev/overview/api) ## RL Agents
+(https://docs.hsuanwu.dev/api) ## RL Agents
 |Module|Recurrent|Box|Discrete|MultiBinary|Multi
 Processing|NPU|Paper|Citations| |:-|:-|:-|:-|:-|:-|:-|:-|:-| |SAC|â| âï¸
 |â|â|â|ð | [Link](http://proceedings.mlr.press/v80/haarnoja18b/
 haarnoja18b.pdf) |5077â­| |DrQ|â| âï¸ |â|â|â|ð | [Link](https://
 arxiv.org/pdf/2004.13649) |433â­| |DDPG|â| âï¸ |â|â|â|ð | [Link]
 (https://arxiv.org/pdf/1509.02971.pdf?source=post_page-------------------------
 --) |11819â­| |DrQ-v2|â| âï¸ |â|â|â|ð | [Link](https://
 arxiv.org/pdf/2107.09645.pdf?utm_source=morioh.com) |100â­| |PPO|â| âï¸
-|âï¸|ð|âï¸|ð | [Link](https://arxiv.org/pdf/1707.06347) |11155â­|
-|DrAC|â| âï¸ |âï¸|ð|âï¸|ð | [Link](https://
-proceedings.neurips.cc/paper/2021/file/2b38c2df6a49b97f706ec9148ce48d86-
-Paper.pdf) |29â­| |PPG|â| âï¸ |âï¸|ð|âï¸|ð| [Link](http://
-proceedings.mlr.press/v139/cobbe21a/cobbe21a.pdf) |82â­| |IMPALA|âï¸|
-âï¸ |âï¸|ð|âï¸|ð| [Link](http://proceedings.mlr.press/v80/
-espeholt18a/espeholt18a.pdf) |1219â­| > - ð: Developing. > - `NPU`: Support
-Neural-network processing unit. > - `Recurrent`: Support recurrent neural
-network. > - `Box`: A N-dimensional box that containes every point in the
-action space. > - `Discrete`: A list of possible actions, where each timestep
-only one of the actions can be used. > - `MultiBinary`: A list of possible
-actions, where each timestep any of the actions can be used in any combination.
-# Model Zoo Hsuanwu provides a large number of reusable bechmarks, see [https:/
-/hub.hsuanwu.dev/](https://hub.hsuanwu.dev/) # API Documentation View our well-
-designed documentation: [https://docs.hsuanwu.dev/](https://docs.hsuanwu.dev/
-) # How To Contribute Welcome to contribute to this project! Before you begin
-writing code, please read [CONTRIBUTING.md](https://github.com/RLE-Foundation/
-Hsuanwu/blob/main/CONTRIBUTING.md) for guide first. # Acknowledgment This
-project is supported by [FUNDING.yml](https://github.com/RLE-Foundation/
-Hsuanwu/blob/main/.github/FUNDING.yml). Some code of this project is borrowed
-or inspired by several excellent projects, and we highly appreciate them. See
-[ACKNOWLEDGMENT.md](https://github.com/RLE-Foundation/Hsuanwu/blob/main/
-ACKNOWLEDGMENT.md).
+|âï¸|âï¸|âï¸|ð | [Link](https://arxiv.org/pdf/1707.06347)
+|11155â­| |DAAC|â| âï¸ |âï¸|âï¸|âï¸|ð | [Link](http://
+proceedings.mlr.press/v139/raileanu21a/raileanu21a.pdf) |56â­| |DrAC|â|
+âï¸ |âï¸|âï¸|âï¸|ð | [Link](https://proceedings.neurips.cc/
+paper/2021/file/2b38c2df6a49b97f706ec9148ce48d86-Paper.pdf) |29â­| |PPG|â|
+âï¸ |âï¸|â|âï¸|ð| [Link](http://proceedings.mlr.press/v139/
+cobbe21a/cobbe21a.pdf) |82â­| |IMPALA|âï¸| âï¸ |âï¸|â|âï¸|ð|
+[Link](http://proceedings.mlr.press/v80/espeholt18a/espeholt18a.pdf) |1219â­|
+> - ð: Developing. > - `NPU`: Support Neural-network processing unit. > -
+`Recurrent`: Support recurrent neural network. > - `Box`: A N-dimensional box
+that containes every point in the action space. > - `Discrete`: A list of
+possible actions, where each timestep only one of the actions can be used. > -
+`MultiBinary`: A list of possible actions, where each timestep any of the
+actions can be used in any combination. ## Intrinsic Reward Modules | Module |
+Remark | Repr. | Visual | Reference | |:-|:-|:-|:-|:-| | PseudoCounts | Count-
+Based exploration |âï¸|âï¸|[Never Give Up: Learning Directed Exploration
+Strategies](https://arxiv.org/pdf/2002.06038) | | ICM | Curiosity-driven
+exploration | âï¸|âï¸| [Curiosity-Driven Exploration by Self-Supervised
+Prediction](http://proceedings.mlr.press/v70/pathak17a/pathak17a.pdf) | | RND |
+Count-based exploration | â|âï¸| [Exploration by Random Network
+Distillation](https://arxiv.org/pdf/1810.12894.pdf) | | GIRM | Curiosity-driven
+exploration | âï¸ |âï¸| [Intrinsic Reward Driven Imitation Learning via
+Generative Model](http://proceedings.mlr.press/v119/yu20d/yu20d.pdf)| | NGU |
+Memory-based exploration | âï¸ |âï¸| [Never Give Up: Learning Directed
+Exploration Strategies](https://arxiv.org/pdf/2002.06038) | | RIDE|
+Procedurally-generated environment | âï¸ |âï¸| [RIDE: Rewarding Impact-
+Driven Exploration for Procedurally-Generated Environments](https://arxiv.org/
+pdf/2002.12292)| | RE3 | Entropy Maximization | â |âï¸| [State Entropy
+Maximization with Random Encoders for Efficient Exploration](http://
+proceedings.mlr.press/v139/seo21a/seo21a.pdf) | | RISE | Entropy Maximization |
+â |âï¸| [RÃ©nyi State Entropy Maximization for Exploration Acceleration in
+Reinforcement Learning](https://ieeexplore.ieee.org/abstract/document/9802917/
+) | | REVD | Divergence Maximization | â |âï¸| [Rewarding Episodic
+Visitation Discrepancy for Exploration in Reinforcement Learning](https://
+openreview.net/pdf?id=V2pw1VYMrDo)| > - ð: Developing. > - `Repr.`: The
+method involves representation learning. > - `Visual`: The method works well in
+visual RL. See [Tutorials: Use intrinsic reward and observation augmentation]
+(https://docs.hsuanwu.dev/tutorials/data_augmentation.md) for usage examples. #
+Model Zoo Hsuanwu provides a large number of reusable bechmarks, see [https://
+hub.hsuanwu.dev/](https://hub.hsuanwu.dev/) and [https://docs.hsuanwu.dev/
+benchmarks/](https://docs.hsuanwu.dev/benchmarks/) # API Documentation View our
+well-designed documentation: [https://docs.hsuanwu.dev/](https://
+docs.hsuanwu.dev/) # How To Contribute Welcome to contribute to this project!
+Before you begin writing code, please read [CONTRIBUTING.md](https://
+github.com/RLE-Foundation/Hsuanwu/blob/main/CONTRIBUTING.md) for guide first. #
+Acknowledgment This project is supported by [FUNDING.yml](https://github.com/
+RLE-Foundation/Hsuanwu/blob/main/.github/FUNDING.yml). Some code of this
+project is borrowed or inspired by several excellent projects, and we highly
+appreciate them. See [ACKNOWLEDGMENT.md](https://github.com/RLE-Foundation/
+Hsuanwu/blob/main/ACKNOWLEDGMENT.md).
```

### Comparing `hsuanwu-0.0.1b4/docs/api/common/engine/__init__.md` & `hsuanwu-0.0.1b5/docs/api_docs/common/engine/__init__.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-#
-
-
-## HsuanwuEngine
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/__init__.py\#L11)
-```python 
-HsuanwuEngine(
-   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
-)
-```
-
-
----
-Hsuanwu RL engine.
-
-
-**Args**
-
-* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
-* **train_env** (Env) : A Gym-like environment for training.
-* **test_env** (Env) : A Gym-like environment for testing.
-
-
-**Returns**
-
-Hsuanwu engine instance.
-
-
-**Methods:**
-
-
-### .invoke
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/__init__.py\#L38)
-```python
-.invoke()
-```
-
----
-Invoke the engine to perform training.
+#
+
+
+## HsuanwuEngine
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/__init__.py/#L12)
+```python 
+HsuanwuEngine(
+   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
+)
+```
+
+
+---
+Hsuanwu RL engine.
+
+
+**Args**
+
+* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
+* **train_env** (Env) : A Gym-like environment for training.
+* **test_env** (Env) : A Gym-like environment for testing.
+
+
+**Returns**
+
+Hsuanwu engine instance.
+
+
+**Methods:**
+
+
+### .invoke
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/__init__.py/#L39)
+```python
+.invoke()
+```
+
+---
+Invoke the engine to perform training.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/common/engine/base_policy_trainer.md` & `hsuanwu-0.0.1b5/docs/api_docs/common/engine/base_policy_trainer.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-#
-
-
-## BasePolicyTrainer
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/base_policy_trainer.py\#L48)
-```python 
-BasePolicyTrainer(
-   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
-)
-```
-
-
----
-Base class of policy trainer.
-
-
-**Args**
-
-* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
-* **train_env** (Env) : A Gym-like environment for training.
-* **test_env** (Env) : A Gym-like environment for testing.
-
-
-**Returns**
-
-Base policy trainer instance.
-
-
-**Methods:**
-
-
-### .global_step
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/base_policy_trainer.py\#L95)
-```python
-.global_step()
-```
-
----
-Get global training steps.
-
-### .global_episode
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/base_policy_trainer.py\#L100)
-```python
-.global_episode()
-```
-
----
-Get global training episodes.
-
-### .train
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/base_policy_trainer.py\#L269)
-```python
-.train()
-```
-
----
-Training function.
-
-### .test
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/base_policy_trainer.py\#L273)
-```python
-.test()
-```
-
----
-Testing function.
-
-### .save
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/base_policy_trainer.py\#L277)
-```python
-.save()
-```
-
----
-Save the trained model.
+#
+
+
+## BasePolicyTrainer
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/base_policy_trainer.py/#L49)
+```python 
+BasePolicyTrainer(
+   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
+)
+```
+
+
+---
+Base class of policy trainer.
+
+
+**Args**
+
+* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
+* **train_env** (Env) : A Gym-like environment for training.
+* **test_env** (Env) : A Gym-like environment for testing.
+
+
+**Returns**
+
+Base policy trainer instance.
+
+
+**Methods:**
+
+
+### .global_step
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/base_policy_trainer.py/#L96)
+```python
+.global_step()
+```
+
+---
+Get global training steps.
+
+### .global_episode
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/base_policy_trainer.py/#L101)
+```python
+.global_episode()
+```
+
+---
+Get global training episodes.
+
+### .train
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/base_policy_trainer.py/#L270)
+```python
+.train()
+```
+
+---
+Training function.
+
+### .test
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/base_policy_trainer.py/#L274)
+```python
+.test()
+```
+
+---
+Testing function.
+
+### .save
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/base_policy_trainer.py/#L278)
+```python
+.save()
+```
+
+---
+Save the trained model.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/common/engine/distributed_trainer.md` & `hsuanwu-0.0.1b5/docs/api_docs/common/engine/distributed_trainer.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-#
-
-
-## DistributedTrainer
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/distributed_trainer.py\#L112)
-```python 
-DistributedTrainer(
-   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
-)
-```
-
-
----
-Trainer for distributed algorithms.
-
-
-**Args**
-
-* **train_env** (Env) : A list of Gym-like environments for training.
-* **test_env** (Env) : A Gym-like environment for testing.
-* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
-
-
-**Returns**
-
-Distributed trainer instance.
-
-
-**Methods:**
-
-
-### .act
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/distributed_trainer.py\#L167)
-```python
-.act(
-   cfgs: omegaconf.DictConfig, logger: Logger, gym_env: gym.Env, actor_idx: int,
-   actor_model: nn.Module, free_queue: mp.SimpleQueue, full_queue: mp.SimpleQueue,
-   storages: Dict[str, List], init_actor_state_storages: List[th.Tensor]
-)
-```
-
----
-Sampling function for each actor.
-
-
-**Args**
-
-* **cfgs** (DictConfig) : Training configs.
-* **logger** (Logger) : Hsuanwu logger.
-* **gym_env** (Env) : A Gym-like environment.
-* **actor_idx** (int) : The index of actor.
-* **actor_model** (NNMoudle) : Actor network.
-* **free_queue** (Queue) : Free queue for communication.
-* **full_queue** (Queue) : Full queue for communication.
-* **storages** (List[Storage]) : A list of shared storages.
-* **init_actor_state_storages** (List[Tensor]) : Initial states for LSTM.
-
-
-**Returns**
-
-None.
-
-### .train
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/distributed_trainer.py\#L237)
-```python
-.train()
-```
-
----
-Training function
-
-### .test
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/distributed_trainer.py\#L347)
-```python
-.test()
-```
-
----
-Testing function.
-
-### .save
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/distributed_trainer.py\#L351)
-```python
-.save()
-```
-
----
-Save the trained model.
+#
+
+
+## DistributedTrainer
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/distributed_trainer.py/#L126)
+```python 
+DistributedTrainer(
+   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
+)
+```
+
+
+---
+Trainer for distributed algorithms.
+
+
+**Args**
+
+* **train_env** (Env) : A list of Gym-like environments for training.
+* **test_env** (Env) : A Gym-like environment for testing.
+* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
+
+
+**Returns**
+
+Distributed trainer instance.
+
+
+**Methods:**
+
+
+### .act
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/distributed_trainer.py/#L170)
+```python
+.act(
+   cfgs: omegaconf.DictConfig, logger: Logger, gym_env: gym.Env, actor_idx: int,
+   actor_model: nn.Module, free_queue: mp.SimpleQueue, full_queue: mp.SimpleQueue,
+   storages: Dict[str, List], init_actor_state_storages: List[th.Tensor]
+)
+```
+
+---
+Sampling function for each actor.
+
+
+**Args**
+
+* **cfgs** (DictConfig) : Training configs.
+* **logger** (Logger) : Hsuanwu logger.
+* **gym_env** (Env) : A Gym-like environment.
+* **actor_idx** (int) : The index of actor.
+* **actor_model** (NNMoudle) : Actor network.
+* **free_queue** (Queue) : Free queue for communication.
+* **full_queue** (Queue) : Full queue for communication.
+* **storages** (List[Storage]) : A list of shared storages.
+* **init_actor_state_storages** (List[Tensor]) : Initial states for LSTM.
+
+
+**Returns**
+
+None.
+
+### .train
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/distributed_trainer.py/#L240)
+```python
+.train()
+```
+
+---
+Training function
+
+### .test
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/distributed_trainer.py/#L362)
+```python
+.test()
+```
+
+---
+Testing function.
+
+### .save
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/distributed_trainer.py/#L383)
+```python
+.save()
+```
+
+---
+Save the trained model.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/common/engine/off_policy_trainer.md` & `hsuanwu-0.0.1b5/docs/api_docs/common/engine/on_policy_trainer.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,57 @@
-#
-
-
-## OffPolicyTrainer
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/off_policy_trainer.py\#L15)
-```python 
-OffPolicyTrainer(
-   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
-)
-```
-
-
----
-Trainer for off-policy algorithms.
-
-
-**Args**
-
-* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
-* **train_env** (Env) : A Gym-like environment for training.
-* **test_env** (Env) : A Gym-like environment for testing.
-
-
-**Returns**
-
-Off-policy trainer instance.
-
-
-**Methods:**
-
-
-### .replay_iter
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/off_policy_trainer.py\#L81)
-```python
-.replay_iter()
-```
-
----
-Create iterable dataloader.
-
-### .train
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/off_policy_trainer.py\#L87)
-```python
-.train()
-```
-
----
-Training function.
-
-### .test
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/off_policy_trainer.py\#L158)
-```python
-.test()
-```
-
----
-Testing function.
-
-### .save
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/off_policy_trainer.py\#L186)
-```python
-.save()
-```
-
----
-Save the trained model.
+#
+
+
+## OnPolicyTrainer
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/on_policy_trainer.py/#L16)
+```python 
+OnPolicyTrainer(
+   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
+)
+```
+
+
+---
+Trainer for on-policy algorithms.
+
+
+**Args**
+
+* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
+* **train_env** (Env) : A Gym-like environment for training.
+* **test_env** (Env) : A Gym-like environment for testing.
+
+
+**Returns**
+
+On-policy trainer instance.
+
+
+**Methods:**
+
+
+### .train
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/on_policy_trainer.py/#L62)
+```python
+.train()
+```
+
+---
+Training function.
+
+### .test
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/on_policy_trainer.py/#L140)
+```python
+.test()
+```
+
+---
+Testing function.
+
+### .save
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/on_policy_trainer.py/#L164)
+```python
+.save()
+```
+
+---
+Save the trained model.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/common/engine/on_policy_trainer.md` & `hsuanwu-0.0.1b5/docs/api_docs/common/engine/off_policy_trainer.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#
-
-
-## OnPolicyTrainer
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/on_policy_trainer.py\#L15)
-```python 
-OnPolicyTrainer(
-   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
-)
-```
-
-
----
-Trainer for on-policy algorithms.
-
-
-**Args**
-
-* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
-* **train_env** (Env) : A Gym-like environment for training.
-* **test_env** (Env) : A Gym-like environment for testing.
-
-
-**Returns**
-
-On-policy trainer instance.
-
-
-**Methods:**
-
-
-### .train
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/on_policy_trainer.py\#L64)
-```python
-.train()
-```
-
----
-Training function.
-
-### .test
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/on_policy_trainer.py\#L141)
-```python
-.test()
-```
-
----
-Testing function.
-
-### .save
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/common/engine/on_policy_trainer.py\#L165)
-```python
-.save()
-```
-
----
-Save the trained model.
+#
+
+
+## OffPolicyTrainer
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/off_policy_trainer.py/#L16)
+```python 
+OffPolicyTrainer(
+   cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None
+)
+```
+
+
+---
+Trainer for off-policy algorithms.
+
+
+**Args**
+
+* **cfgs** (DictConfig) : Dict config for configuring RL algorithms.
+* **train_env** (Env) : A Gym-like environment for training.
+* **test_env** (Env) : A Gym-like environment for testing.
+
+
+**Returns**
+
+Off-policy trainer instance.
+
+
+**Methods:**
+
+
+### .train
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/off_policy_trainer.py/#L64)
+```python
+.train()
+```
+
+---
+Training function.
+
+### .test
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/off_policy_trainer.py/#L130)
+```python
+.test()
+```
+
+---
+Testing function.
+
+### .save
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/common/engine/off_policy_trainer.py/#L158)
+```python
+.save()
+```
+
+---
+Save the trained model.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/env/atari/__init__.md` & `hsuanwu-0.0.1b5/docs/api_docs/env/bullet/__init__.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-#
-
-
-### make_atari_env
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/env/atari/__init__.py\#L12)
-```python
-.make_atari_env(
-   env_id: str = 'Alien-v5', num_envs: int = 8, device: str = 'cpu', seed: int = 0,
-   frame_stack: int = 4
-)
-```
-
----
-Build Atari environments.
-
-
-**Args**
-
-* **env_id** (str) : Name of environment.
-* **num_envs** (int) : Number of parallel environments.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **seed** (int) : Random seed.
-* **frame_stack** (int) : Number of stacked frames.
-
-
-**Returns**
-
-Environments instance.
+#
+
+
+### make_bullet_env
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/env/bullet/__init__.py/#L46)
+```python
+.make_bullet_env(
+   env_id: str = 'AntBulletEnv-v0', num_envs: int = 1, device: str = 'cpu', seed: int = 0
+)
+```
+
+---
+Build PyBullet robotics environments.
+
+
+**Args**
+
+* **env_id** (str) : Name of environment.
+* **num_envs** (int) : Number of parallel environments.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **seed** (int) : Random seed.
+
+
+**Returns**
+
+Environments instance.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/env/dmc/__init__.md` & `hsuanwu-0.0.1b5/docs/api_docs/env/dmc/__init__.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-#
-
-
-### make_dmc_env
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/env/dmc/__init__.py\#L12)
-```python
-.make_dmc_env(
-   env_id: str = 'cartpole_balance', num_envs: int = 1, device: str = 'cpu',
-   resource_files: Optional[List] = None, img_source: Optional[str] = None,
-   total_frames: Optional[int] = None, seed: int = 1, visualize_reward: bool = False,
-   from_pixels: bool = True, height: int = 84, width: int = 84, camera_id: int = 0,
-   frame_stack: int = 3, frame_skip: int = 2, episode_length: int = 1000,
-   environment_kwargs: Optional[Dict] = None
-)
-```
-
----
-Build DeepMind Control Suite environments.
-
-
-**Args**
-
-* **env_id** (str) : Name of environment.
-* **num_envs** (int) : Number of parallel environments.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **resource_files** (Optional[List]) : File path of the resource files.
-* **img_source** (Optional[str]) : Type of the background distractor, supported values: ['color', 'noise', 'images', 'video'].
-* **total_frames** (Optional[int]) : for 'images' or 'video' distractor.
-* **seed** (int) : Random seed.
-* **visualize_reward** (bool) : True when 'from_pixels' is False, False when 'from_pixels' is True.
-* **from_pixels** (bool) : Provide image-based observations or not.
-* **height** (int) : Image observation height.
-* **width** (int) : Image observation width.
-* **camera_id** (int) : Camera id for generating image-based observations.
-* **frame_stack** (int) : Number of stacked frames.
-* **frame_skip** (int) : Number of action repeat.
-* **episode_length** (int) : Maximum length of an episode.
-* **environment_kwargs** (Optional[Dict]) : Other environment arguments.
-
-
-**Returns**
-
-Environments instance.
+#
+
+
+### make_dmc_env
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/env/dmc/__init__.py/#L12)
+```python
+.make_dmc_env(
+   env_id: str = 'cartpole_balance', num_envs: int = 1, device: str = 'cpu',
+   resource_files: Optional[List] = None, img_source: Optional[str] = None,
+   total_frames: Optional[int] = None, seed: int = 1, visualize_reward: bool = False,
+   from_pixels: bool = True, height: int = 84, width: int = 84, camera_id: int = 0,
+   frame_stack: int = 3, frame_skip: int = 2, episode_length: int = 1000,
+   environment_kwargs: Optional[Dict] = None
+)
+```
+
+---
+Build DeepMind Control Suite environments.
+
+
+**Args**
+
+* **env_id** (str) : Name of environment.
+* **num_envs** (int) : Number of parallel environments.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **resource_files** (Optional[List]) : File path of the resource files.
+* **img_source** (Optional[str]) : Type of the background distractor, supported values: ['color', 'noise', 'images', 'video'].
+* **total_frames** (Optional[int]) : for 'images' or 'video' distractor.
+* **seed** (int) : Random seed.
+* **visualize_reward** (bool) : True when 'from_pixels' is False, False when 'from_pixels' is True.
+* **from_pixels** (bool) : Provide image-based observations or not.
+* **height** (int) : Image observation height.
+* **width** (int) : Image observation width.
+* **camera_id** (int) : Camera id for generating image-based observations.
+* **frame_stack** (int) : Number of stacked frames.
+* **frame_skip** (int) : Number of action repeat.
+* **episode_length** (int) : Maximum length of an episode.
+* **environment_kwargs** (Optional[Dict]) : Other environment arguments.
+
+
+**Returns**
+
+Environments instance.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/agent/base.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/base.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,146 @@
-#
-
-
-## BaseAgent
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/base.py\#L9)
-```python 
-BaseAgent(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str, feature_dim: int, lr: float, eps: float
-)
-```
-
-
----
-Base class of agent.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **feature_dim** (int) : Number of features extracted by the encoder.
-* **lr** (float) : The learning rate.
-* **eps** (float) : Term added to the denominator to improve numerical stability.
-
-
-**Returns**
-
-Base agent instance.
-
-
-**Methods:**
-
-
-### .train
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/base.py\#L74)
-```python
-.train(
-   training: bool = True
-)
-```
-
----
-Set the train mode.
-
-
-**Args**
-
-* **training** (bool) : True (training) or False (testing).
-
-
-**Returns**
-
-None.
-
-### .act
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/base.py\#L86)
-```python
-.act(
-   obs: th.Tensor, training: bool = True, step: int = 0
-)
-```
-
----
-Sample actions based on observations.
-
-
-**Args**
-
-* **obs** (Tensor) : Observations.
-* **training** (bool) : training mode, True or False.
-* **step** (int) : Global training step.
-
-
-**Returns**
-
-Sampled actions.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/base.py\#L99)
-```python
-.update(
-   *kwargs
-)
-```
-
----
-Update agent and return training metrics such as loss functions.
+#
+
+
+## BaseAgent
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/base.py/#L10)
+```python 
+BaseAgent(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str, feature_dim: int, lr: float, eps: float
+)
+```
+
+
+---
+Base class of agent.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **feature_dim** (int) : Number of features extracted by the encoder.
+* **lr** (float) : The learning rate.
+* **eps** (float) : Term added to the denominator to improve numerical stability.
+
+
+**Returns**
+
+Base agent instance.
+
+
+**Methods:**
+
+
+### .train
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/base.py/#L78)
+```python
+.train(
+   training: bool = True
+)
+```
+
+---
+Set the train mode.
+
+
+**Args**
+
+* **training** (bool) : True (training) or False (testing).
+
+
+**Returns**
+
+None.
+
+### .integrate
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/base.py/#L90)
+```python
+.integrate(
+   **kwargs
+)
+```
+
+---
+Integrate agent and other modules (encoder, reward, ...) together
+
+### .act
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/base.py/#L94)
+```python
+.act(
+   obs: th.Tensor, training: bool = True, step: int = 0
+)
+```
+
+---
+Sample actions based on observations.
+
+
+**Args**
+
+* **obs** (Tensor) : Observations.
+* **training** (bool) : training mode, True or False.
+* **step** (int) : Global training step.
+
+
+**Returns**
+
+Sampled actions.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/base.py/#L107)
+```python
+.update(
+   **kwargs
+)
+```
+
+---
+Update agent and return training metrics such as loss functions.
+
+### .save
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/base.py/#L111)
+```python
+.save(
+   path: Path
+)
+```
+
+---
+Save models.
+
+
+**Args**
+
+* **path** (path) : Storage path.
+
+
+**Returns**
+
+None.
+
+### .load
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/base.py/#L122)
+```python
+.load(
+   path: Path
+)
+```
+
+---
+Load initial parameters.
+
+
+**Args**
+
+* **path** (path) : Import path.
+
+
+**Returns**
+
+None.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/agent/drqv2.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/ppg.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,161 +1,197 @@
-#
-
-
-## DrQv2
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/drqv2.py\#L63)
-```python 
-DrQv2(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str, feature_dim: int, lr: float, eps: float,
-   hidden_dim: int, critic_target_tau: float, update_every_steps: int
-)
-```
-
-
----
-Data Regularized-Q v2 (DrQ-v2).
-When 'augmentation' module is deprecated, this agent will transform into
-    Deep Deterministic Policy Gradient (DDPG) agent.
-Based on: https://github.com/facebookresearch/drqv2/blob/main/drqv2.py
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **feature_dim** (int) : Number of features extracted by the encoder.
-* **lr** (float) : The learning rate.
-* **eps** (float) : Term added to the denominator to improve numerical stability.
-* **hidden_dim** (int) : The size of the hidden layers.
-* **critic_target_tau**  : The critic Q-function soft-update rate.
-* **update_every_steps** (int) : The agent update frequency.
-
-
-
-**Returns**
-
-DrQv2 agent instance.
-
-
-**Methods:**
-
-
-### .train
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/drqv2.py\#L122)
-```python
-.train(
-   training: bool = True
-)
-```
-
----
-Set the train mode.
-
-
-**Args**
-
-* **training** (bool) : True (training) or False (testing).
-
-
-**Returns**
-
-None.
-
-### .act
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/drqv2.py\#L137)
-```python
-.act(
-   obs: th.Tensor, training: bool = True, step: int = 0
-)
-```
-
----
-Sample actions based on observations.
-
-
-**Args**
-
-* **obs** (Tensor) : Observations.
-* **training** (bool) : training mode, True or False.
-* **step** (int) : Global training step.
-
-
-**Returns**
-
-Sampled actions.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/drqv2.py\#L158)
-```python
-.update(
-   replay_iter: Generator, step: int = 0
-)
-```
-
----
-Update the agent.
-
-
-**Args**
-
-* **replay_iter** (Generator) : Hsuanwu replay storage iterable dataloader.
-* **step** (int) : Global training step.
-
-
-**Returns**
-
-Training metrics such as actor loss, critic_loss, etc.
-
-### .update_critic
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/drqv2.py\#L212)
-```python
-.update_critic(
-   obs: th.Tensor, action: th.Tensor, reward: th.Tensor, discount: th.Tensor,
-   next_obs: th.Tensor, step: int
-)
-```
-
----
-Update the critic network.
-
-
-**Args**
-
-* **obs** (Tensor) : Observations.
-* **action** (Tensor) : Actions.
-* **reward** (Tensor) : Rewards.
-* **discount** (Tensor) : discounts.
-* **next_obs** (Tensor) : Next observations.
-* **step** (int) : Global training step.
-
-
-**Returns**
-
-Critic loss metrics.
-
-### .update_actor
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/drqv2.py\#L261)
-```python
-.update_actor(
-   obs: th.Tensor, step: int
-)
-```
-
----
-Update the actor network.
-
-
-**Args**
-
-* **obs** (Tensor) : Observations.
-* **step** (int) : Global training step.
-
-
-**Returns**
-
-Actor loss metrics.
+#
+
+
+## PPG
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppg.py/#L66)
+```python 
+PPG(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str, feature_dim: int = 256, lr: float = 0.0005,
+   eps: float = 1e-05, hidden_dim: int = 256, clip_range: float = 0.2,
+   num_policy_mini_batch: int = 8, num_aux_mini_batch: int = 4, vf_coef: float = 0.5,
+   ent_coef: float = 0.01, aug_coef: float = 0.1, max_grad_norm: float = 0.5,
+   policy_epochs: int = 32, aux_epochs: int = 6, kl_coef: float = 1.0,
+   num_aux_grad_accum: int = 1
+)
+```
+
+
+---
+Phasic Policy Gradient (PPG) agent.
+Based on: https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppg_procgen.py
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **feature_dim** (int) : Number of features extracted by the encoder.
+* **lr** (float) : The learning rate.
+* **eps** (float) : Term added to the denominator to improve numerical stability.
+* **hidden_dim** (int) : The size of the hidden layers.
+* **clip_range** (float) : Clipping parameter.
+* **num_policy_mini_batch** (int) : Number of mini-batches in policy phase.
+* **vf_coef** (float) : Weighting coefficient of value loss.
+* **ent_coef** (float) : Weighting coefficient of entropy bonus.
+* **aug_coef** (float) : Weighting coefficient of augmentation loss.
+* **max_grad_norm** (float) : Maximum norm of gradients.
+* **policy_epochs** (int) : Number of iterations in the policy phase.
+* **aux_epochs** (int) : Number of iterations in the auxiliary phase.
+* **kl_coef** (float) : Weighting coefficient of divergence loss.
+* **num_aux_grad_accum** (int) : Number of gradient accumulation for auxiliary phase update.
+
+num_aux_mini_batch (int) Number of mini-batches in auxiliary phase.
+
+
+**Returns**
+
+PPG agent instance.
+
+
+**Methods:**
+
+
+### .train
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppg.py/#L151)
+```python
+.train(
+   training: bool = True
+)
+```
+
+---
+Set the train mode.
+
+
+**Args**
+
+* **training** (bool) : True (training) or False (testing).
+
+
+**Returns**
+
+None.
+
+### .integrate
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppg.py/#L163)
+```python
+.integrate(
+   **kwargs
+)
+```
+
+---
+Integrate agent and other modules (encoder, reward, ...) together
+
+### .get_value
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppg.py/#L178)
+```python
+.get_value(
+   obs: th.Tensor
+)
+```
+
+---
+Get estimated values for observations.
+
+
+**Args**
+
+* **obs** (Tensor) : Observations.
+
+
+**Returns**
+
+Estimated values.
+
+### .act
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppg.py/#L189)
+```python
+.act(
+   obs: th.Tensor, training: bool = True, step: int = 0
+)
+```
+
+---
+Sample actions based on observations.
+
+
+**Args**
+
+* **obs**  : Observations.
+* **training**  : training mode, True or False.
+* **step**  : Global training step.
+
+
+**Returns**
+
+Sampled actions.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppg.py/#L211)
+```python
+.update(
+   rollout_storage: Storage, episode: int = 0
+)
+```
+
+---
+Update the agent.
+
+
+**Args**
+
+* **rollout_storage** (Storage) : Hsuanwu rollout storage.
+* **episode** (int) : Global training episode.
+
+
+**Returns**
+
+Training metrics such as actor loss, critic_loss, etc.
+
+### .save
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppg.py/#L412)
+```python
+.save(
+   path: Path
+)
+```
+
+---
+Save models.
+
+
+**Args**
+
+* **path** (Path) : Storage path.
+
+
+**Returns**
+
+None.
+
+### .load
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppg.py/#L427)
+```python
+.load(
+   path: str
+)
+```
+
+---
+Load initial parameters.
+
+
+**Args**
+
+* **path** (str) : Import path.
+
+
+**Returns**
+
+None.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/agent/ppg.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/agent/ppo.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,144 +1,191 @@
-#
-
-
-## PPG
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppg.py\#L64)
-```python 
-PPG(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str, feature_dim: int = 256, lr: float = 0.0005,
-   eps: float = 1e-05, hidden_dim: int = 256, clip_range: float = 0.2,
-   num_policy_mini_batch: int = 8, num_aux_mini_batch: int = 4, vf_coef: float = 0.5,
-   ent_coef: float = 0.01, aug_coef: float = 0.1, max_grad_norm: float = 0.5,
-   policy_epochs: int = 32, aux_epochs: int = 6, kl_coef: float = 1.0,
-   num_aux_grad_accum: int = 1
-)
-```
-
-
----
-Phasic Policy Gradient (PPG) agent.
-Based on: https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppg_procgen.py
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **feature_dim** (int) : Number of features extracted by the encoder.
-* **lr** (float) : The learning rate.
-* **eps** (float) : Term added to the denominator to improve numerical stability.
-* **hidden_dim** (int) : The size of the hidden layers.
-* **clip_range** (float) : Clipping parameter.
-* **num_policy_mini_batch** (int) : Number of mini-batches in policy phase.
-* **vf_coef** (float) : Weighting coefficient of value loss.
-* **ent_coef** (float) : Weighting coefficient of entropy bonus.
-* **aug_coef** (float) : Weighting coefficient of augmentation loss.
-* **max_grad_norm** (float) : Maximum norm of gradients.
-* **policy_epochs** (int) : Number of iterations in the policy phase.
-* **aux_epochs** (int) : Number of iterations in the auxiliary phase.
-* **kl_coef** (float) : Weighting coefficient of divergence loss.
-* **num_aux_grad_accum** (int) : Number of gradient accumulation for auxiliary phase update.
-
-num_aux_mini_batch (int) Number of mini-batches in auxiliary phase.
-
-
-**Returns**
-
-PPG agent instance.
-
-
-**Methods:**
-
-
-### .train
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppg.py\#L151)
-```python
-.train(
-   training: bool = True
-)
-```
-
----
-Set the train mode.
-
-
-**Args**
-
-* **training** (bool) : True (training) or False (testing).
-
-
-**Returns**
-
-None.
-
-### .get_value
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppg.py\#L165)
-```python
-.get_value(
-   obs: th.Tensor
-)
-```
-
----
-Get estimated values for observations.
-
-
-**Args**
-
-* **obs** (Tensor) : Observations.
-
-
-**Returns**
-
-Estimated values.
-
-### .act
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppg.py\#L177)
-```python
-.act(
-   obs: th.Tensor, training: bool = True, step: int = 0
-)
-```
-
----
-Sample actions based on observations.
-
-
-**Args**
-
-* **obs**  : Observations.
-* **training**  : training mode, True or False.
-* **step**  : Global training step.
-
-
-**Returns**
-
-Sampled actions.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppg.py\#L196)
-```python
-.update(
-   rollout_storage: Storage, episode: int = 0
-)
-```
-
----
-Update the agent.
-
-
-**Args**
-
-* **rollout_storage** (Storage) : Hsuanwu rollout storage.
-* **episode** (int) : Global training episode.
-
-
-**Returns**
-
-Training metrics such as actor loss, critic_loss, etc.
+#
+
+
+## PPO
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppo.py/#L62)
+```python 
+PPO(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str, feature_dim: int, lr: float, eps: float,
+   hidden_dim: int, clip_range: float, n_epochs: int, num_mini_batch: int,
+   vf_coef: float, ent_coef: float, aug_coef: float, max_grad_norm: float
+)
+```
+
+
+---
+Proximal Policy Optimization (PPO) agent.
+When 'augmentation' module is invoked, this learner will transform into Data Regularized Actor-Critic (DrAC) agent.
+Based on: https://github.com/yuanmingqi/pytorch-a2c-ppo-acktr-gail
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **feature_dim** (int) : Number of features extracted by the encoder.
+* **lr** (float) : The learning rate.
+* **eps** (float) : Term added to the denominator to improve numerical stability.
+* **hidden_dim** (int) : The size of the hidden layers.
+* **clip_range** (float) : Clipping parameter.
+* **n_epochs** (int) : Times of updating the policy.
+* **num_mini_batch** (int) : Number of mini-batches.
+* **vf_coef** (float) : Weighting coefficient of value loss.
+* **ent_coef** (float) : Weighting coefficient of entropy bonus.
+* **aug_coef** (float) : Weighting coefficient of augmentation loss.
+* **max_grad_norm** (float) : Maximum norm of gradients.
+
+
+
+**Returns**
+
+PPO learner instance.
+
+
+**Methods:**
+
+
+### .train
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppo.py/#L127)
+```python
+.train(
+   training: bool = True
+)
+```
+
+---
+Set the train mode.
+
+
+**Args**
+
+* **training** (bool) : True (training) or False (testing).
+
+
+**Returns**
+
+None.
+
+### .integrate
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppo.py/#L139)
+```python
+.integrate(
+   **kwargs
+)
+```
+
+---
+Integrate agent and other modules (encoder, reward, ...) together
+
+### .get_value
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppo.py/#L154)
+```python
+.get_value(
+   obs: th.Tensor
+)
+```
+
+---
+Get estimated values for observations.
+
+
+**Args**
+
+* **obs** (Tensor) : Observations.
+
+
+**Returns**
+
+Estimated values.
+
+### .act
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppo.py/#L165)
+```python
+.act(
+   obs: th.Tensor, training: bool = True, step: int = 0
+)
+```
+
+---
+Sample actions based on observations.
+
+
+**Args**
+
+* **obs**  : Observations.
+* **training**  : training mode, True or False.
+* **step**  : Global training step.
+
+
+**Returns**
+
+Sampled actions.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppo.py/#L187)
+```python
+.update(
+   rollout_storage: Storage, episode: int = 0
+)
+```
+
+---
+Update the learner.
+
+
+**Args**
+
+* **rollout_storage** (Storage) : Hsuanwu rollout storage.
+* **episode** (int) : Global training episode.
+
+
+**Returns**
+
+Training metrics such as actor loss, critic_loss, etc.
+
+### .save
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppo.py/#L285)
+```python
+.save(
+   path: Path
+)
+```
+
+---
+Save models.
+
+
+**Args**
+
+* **path** (Path) : Storage path.
+
+
+**Returns**
+
+None.
+
+### .load
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/agent/ppo.py/#L300)
+```python
+.load(
+   path: str
+)
+```
+
+---
+Load initial parameters.
+
+
+**Args**
+
+* **path** (str) : Import path.
+
+
+**Returns**
+
+None.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/agent/ppo.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/vanilla_rollout_storage.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,123 @@
-#
-
-
-## PPO
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppo.py\#L60)
-```python 
-PPO(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str, feature_dim: int, lr: float, eps: float,
-   hidden_dim: int, clip_range: float, n_epochs: int, num_mini_batch: int,
-   vf_coef: float, ent_coef: float, aug_coef: float, max_grad_norm: float
-)
-```
-
-
----
-Proximal Policy Optimization (PPO) agent.
-When 'augmentation' module is invoked, this learner will transform into Data Regularized Actor-Critic (DrAC) agent.
-Based on: https://github.com/yuanmingqi/pytorch-a2c-ppo-acktr-gail
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **feature_dim** (int) : Number of features extracted by the encoder.
-* **lr** (float) : The learning rate.
-* **eps** (float) : Term added to the denominator to improve numerical stability.
-* **hidden_dim** (int) : The size of the hidden layers.
-* **clip_range** (float) : Clipping parameter.
-* **n_epochs** (int) : Times of updating the policy.
-* **num_mini_batch** (int) : Number of mini-batches.
-* **vf_coef** (float) : Weighting coefficient of value loss.
-* **ent_coef** (float) : Weighting coefficient of entropy bonus.
-* **aug_coef** (float) : Weighting coefficient of augmentation loss.
-* **max_grad_norm** (float) : Maximum norm of gradients.
-
-
-
-**Returns**
-
-PPO learner instance.
-
-
-**Methods:**
-
-
-### .train
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppo.py\#L129)
-```python
-.train(
-   training: bool = True
-)
-```
-
----
-Set the train mode.
-
-
-**Args**
-
-* **training** (bool) : True (training) or False (testing).
-
-
-**Returns**
-
-None.
-
-### .get_value
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppo.py\#L143)
-```python
-.get_value(
-   obs: th.Tensor
-)
-```
-
----
-Get estimated values for observations.
-
-
-**Args**
-
-* **obs** (Tensor) : Observations.
-
-
-**Returns**
-
-Estimated values.
-
-### .act
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppo.py\#L155)
-```python
-.act(
-   obs: th.Tensor, training: bool = True, step: int = 0
-)
-```
-
----
-Sample actions based on observations.
-
-
-**Args**
-
-* **obs**  : Observations.
-* **training**  : training mode, True or False.
-* **step**  : Global training step.
-
-
-**Returns**
-
-Sampled actions.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/agent/ppo.py\#L174)
-```python
-.update(
-   rollout_storage: Storage, episode: int = 0
-)
-```
-
----
-Update the learner.
-
-
-**Args**
-
-* **rollout_storage** (Storage) : Hsuanwu rollout storage.
-* **episode** (int) : Global training episode.
-
-
-**Returns**
-
-Training metrics such as actor loss, critic_loss, etc.
+#
+
+
+## VanillaRolloutStorage
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/vanilla_rollout_storage.py/#L11)
+```python 
+VanillaRolloutStorage(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', num_steps: int = 256, num_envs: int = 8,
+   discount: float = 0.99, gae_lambda: float = 0.95
+)
+```
+
+
+---
+Vanilla rollout storage for on-policy algorithms.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **num_steps** (int) : The sample length of per rollout.
+* **num_envs** (int) : The number of parallel environments.
+* **discount** (float) : discount factor.
+* **gae_lambda** (float) : Weighting coefficient for generalized advantage estimation (GAE).
+
+
+**Returns**
+
+Vanilla rollout storage.
+
+
+**Methods:**
+
+
+### .add
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/vanilla_rollout_storage.py/#L90)
+```python
+.add(
+   obs: th.Tensor, actions: th.Tensor, rewards: th.Tensor, terminateds: th.Tensor,
+   truncateds: th.Tensor, next_obs: th.Tensor, log_probs: th.Tensor,
+   values: th.Tensor
+)
+```
+
+---
+Add sampled transitions into storage.
+
+
+**Args**
+
+* **obs** (Tensor) : Observations.
+* **actions** (Tensor) : Actions.
+* **rewards** (Tensor) : Rewards.
+* **terminateds** (Tensor) : Terminateds.
+* **truncateds** (Tensor) : Truncateds.
+* **next_obs** (Tensor) : Next observations.
+* **log_probs** (Tensor) : Log of the probability evaluated at `actions`.
+* **values** (Tensor) : Estimated values.
+
+
+**Returns**
+
+None.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/vanilla_rollout_storage.py/#L127)
+```python
+.update()
+```
+
+---
+Reset the terminal state of each env.
+
+### .compute_returns_and_advantages
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/vanilla_rollout_storage.py/#L132)
+```python
+.compute_returns_and_advantages(
+   last_values: th.Tensor
+)
+```
+
+---
+Perform generalized advantage estimation (GAE).
+
+
+**Args**
+
+* **last_values** (Tensor) : Estimated values of the last step.
+* **gamma** (float) : Discount factor.
+* **gae_lamdba** (float) : Coefficient of GAE.
+
+
+**Returns**
+
+None.
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/vanilla_rollout_storage.py/#L158)
+```python
+.sample(
+   num_mini_batch: int = 8
+)
+```
+
+---
+Sample data from storage.
+
+
+**Args**
+
+* **num_mini_batch** (int) : Number of mini-batches
+
+
+**Returns**
+
+Batch data.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/encoder/base.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/base.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#
-
-
-## BaseEncoder
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/base.py\#L20)
-```python 
-BaseEncoder(
-   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 0
-)
-```
-
-
----
-Base class that represents a features extractor.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **feature_dim** (int) : Number of features extracted.
-
-
-**Returns**
-
-The base encoder class
-
-
-**Methods:**
-
-
-### .feature_dim
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/base.py\#L39)
-```python
-.feature_dim()
-```
-
+#
+
+
+## BaseEncoder
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/base.py/#L20)
+```python 
+BaseEncoder(
+   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 0
+)
+```
+
+
+---
+Base class that represents a features extractor.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **feature_dim** (int) : Number of features extracted.
+
+
+**Returns**
+
+The base encoder class
+
+
+**Methods:**
+
+
+### .feature_dim
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/base.py/#L39)
+```python
+.feature_dim()
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/encoder/espeholt_residual_encoder.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/espeholt_residual_encoder.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-#
-
-
-## EspeholtResidualEncoder
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/espeholt_residual_encoder.py\#L68)
-```python 
-EspeholtResidualEncoder(
-   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 0,
-   net_arch: List[int] = [16, 32, 32]
-)
-```
-
-
----
-ResNet-like encoder for processing image-based observations.
-Proposed by Espeholt L, Soyer H, Munos R, et al. Impala: Scalable distributed deep-rl with importance
-weighted actor-learner architectures[C]//International conference on machine learning. PMLR, 2018: 1407-1416.
-Target task: Atari games and Procgen games.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **feature_dim** (int) : Number of features extracted.
-* **net_arch** (List) : Architecture of the network.
-    It represents the out channels of each residual layer.
-    The length of this list is the number of residual layers.
-
-
-**Returns**
-
-ResNet-like encoder instance.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/espeholt_residual_encoder.py\#L111)
-```python
-.forward(
-   obs: th.Tensor
-)
-```
-
+#
+
+
+## EspeholtResidualEncoder
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/espeholt_residual_encoder.py/#L68)
+```python 
+EspeholtResidualEncoder(
+   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 0,
+   net_arch: List[int] = [16, 32, 32]
+)
+```
+
+
+---
+ResNet-like encoder for processing image-based observations.
+Proposed by Espeholt L, Soyer H, Munos R, et al. Impala: Scalable distributed deep-rl with importance
+weighted actor-learner architectures[C]//International conference on machine learning. PMLR, 2018: 1407-1416.
+Target task: Atari games and Procgen games.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **feature_dim** (int) : Number of features extracted.
+* **net_arch** (List) : Architecture of the network.
+    It represents the out channels of each residual layer.
+    The length of this list is the number of residual layers.
+
+
+**Returns**
+
+ResNet-like encoder instance.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/espeholt_residual_encoder.py/#L111)
+```python
+.forward(
+   obs: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/encoder/identity_encoder.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/tassa_cnn_encoder.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-#
-
-
-## IdentityEncoder
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/identity_encoder.py\#L11)
-```python 
-IdentityEncoder(
-   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 64
-)
-```
-
-
----
-Identity encoder for state-based observations.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **feature_dim** (int) : Number of features extracted.
-
-
-**Returns**
-
-Identity encoder instance.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/identity_encoder.py\#L30)
-```python
-.forward(
-   obs: th.Tensor
-)
-```
-
+#
+
+
+## TassaCnnEncoder
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/tassa_cnn_encoder.py/#L11)
+```python 
+TassaCnnEncoder(
+   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 50
+)
+```
+
+
+---
+Convolutional neural network (CNN)-based encoder for processing image-based observations.
+Proposed by Tassa Y, Doron Y, Muldal A, et al. Deepmind control suite[J].
+arXiv preprint arXiv:1801.00690, 2018.
+Target task: DeepMind Control Suite.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **feature_dim** (int) : Number of features extracted.
+
+
+**Returns**
+
+CNN-based encoder instance.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/tassa_cnn_encoder.py/#L51)
+```python
+.forward(
+   obs: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/encoder/mnih_cnn_encoder.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/mnih_cnn_encoder.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-#
-
-
-## MnihCnnEncoder
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/mnih_cnn_encoder.py\#L11)
-```python 
-MnihCnnEncoder(
-   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 0
-)
-```
-
-
----
-Convolutional neural network (CNN)-based encoder for processing image-based observations.
-Proposed by Mnih V, Kavukcuoglu K, Silver D, et al. Playing atari with
-deep reinforcement learning[J]. arXiv preprint arXiv:1312.5602, 2013.
-Target task: Atari games.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **feature_dim** (int) : Number of features extracted.
-
-
-**Returns**
-
-CNN-based encoder instance.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/mnih_cnn_encoder.py\#L50)
-```python
-.forward(
-   obs: th.Tensor
-)
-```
-
+#
+
+
+## MnihCnnEncoder
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/mnih_cnn_encoder.py/#L11)
+```python 
+MnihCnnEncoder(
+   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 0
+)
+```
+
+
+---
+Convolutional neural network (CNN)-based encoder for processing image-based observations.
+Proposed by Mnih V, Kavukcuoglu K, Silver D, et al. Playing atari with
+deep reinforcement learning[J]. arXiv preprint arXiv:1312.5602, 2013.
+Target task: Atari games.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **feature_dim** (int) : Number of features extracted.
+
+
+**Returns**
+
+CNN-based encoder instance.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/mnih_cnn_encoder.py/#L49)
+```python
+.forward(
+   obs: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/encoder/tassa_cnn_encoder.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/encoder/identity_encoder.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-#
-
-
-## TassaCnnEncoder
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/tassa_cnn_encoder.py\#L11)
-```python 
-TassaCnnEncoder(
-   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 50
-)
-```
-
-
----
-Convolutional neural network (CNN)-based encoder for processing image-based observations.
-Proposed by Tassa Y, Doron Y, Muldal A, et al. Deepmind control suite[J].
-arXiv preprint arXiv:1801.00690, 2018.
-Target task: DeepMind Control Suite.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **feature_dim** (int) : Number of features extracted.
-
-
-**Returns**
-
-CNN-based encoder instance.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/encoder/tassa_cnn_encoder.py\#L52)
-```python
-.forward(
-   obs: th.Tensor
-)
-```
-
+#
+
+
+## IdentityEncoder
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/identity_encoder.py/#L11)
+```python 
+IdentityEncoder(
+   observation_space: Union[gym.Space, DictConfig], feature_dim: int = 64
+)
+```
+
+
+---
+Identity encoder for state-based observations.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **feature_dim** (int) : Number of features extracted.
+
+
+**Returns**
+
+Identity encoder instance.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/encoder/identity_encoder.py/#L31)
+```python
+.forward(
+   obs: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/storage/distributed_storage.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/distributed_storage.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,90 @@
-#
-
-
-## DistributedStorage
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/distributed_storage.py\#L11)
-```python 
-DistributedStorage(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', num_steps: int = 100, num_storages: int = 80,
-   batch_size: int = 32
-)
-```
-
-
----
-Distributed storage for distributed algorithms like IMPALA.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **num_steps** (int) : The sample steps of per rollout.
-* **num_storages** (int) : The number of shared-memory storages.
-* **batch_size** (int) : The batch size.
-
-
-**Returns**
-
-Vanilla rollout storage.
-
-
-**Methods:**
-
-
-### .add
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/distributed_storage.py\#L69)
-```python
-.add(
-   *args
-)
-```
-
----
-Add sampled transitions into storage.
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/distributed_storage.py\#L73)
-```python
-.sample(
-   device: th.device, batch_size: int, free_queue: th.multiprocessing.SimpleQueue,
-   full_queue: th.multiprocessing.SimpleQueue, storages: List,
-   init_actor_state_storages: List, lock = threading.Lock()
-)
-```
-
----
-Sample transitions from the storage.
-
-
-**Args**
-
-* **device** (Device) : Device (cpu, cuda, ...) on which the code should be run.
-* **batch_size** (int) : The batch size.
-* **free_queue** (Queue) : Free queue for communication.
-* **full_queue** (Queue) : Full queue for communication.
-* **storages** (List[Storage]) : A list of shared storages.
-* **init_actor_state_storages**  : (List[Tensor]): Initial states for LSTM.
-* **lock** (Lock) : Thread lock.
-
-
-**Returns**
-
-Batched samples.
+#
+
+
+## DistributedStorage
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/distributed_storage.py/#L11)
+```python 
+DistributedStorage(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', num_steps: int = 100, num_storages: int = 80,
+   batch_size: int = 32
+)
+```
+
+
+---
+Distributed storage for distributed algorithms like IMPALA.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **num_steps** (int) : The sample steps of per rollout.
+* **num_storages** (int) : The number of shared-memory storages.
+* **batch_size** (int) : The batch size.
+
+
+**Returns**
+
+Vanilla rollout storage.
+
+
+**Methods:**
+
+
+### .add
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/distributed_storage.py/#L85)
+```python
+.add(
+   *args
+)
+```
+
+---
+Add sampled transitions into storage.
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/distributed_storage.py/#L89)
+```python
+.sample(
+   device: th.device, batch_size: int, free_queue: th.multiprocessing.SimpleQueue,
+   full_queue: th.multiprocessing.SimpleQueue, storages: List,
+   init_actor_state_storages: List, lock = threading.Lock()
+)
+```
+
+---
+Sample transitions from the storage.
+
+
+**Args**
+
+* **device** (Device) : Device (cpu, cuda, ...) on which the code should be run.
+* **batch_size** (int) : The batch size.
+* **free_queue** (Queue) : Free queue for communication.
+* **full_queue** (Queue) : Full queue for communication.
+* **storages** (List[Storage]) : A list of shared storages.
+* **init_actor_state_storages**  : (List[Tensor]): Initial states for LSTM.
+* **lock** (Lock) : Thread lock.
+
+
+**Returns**
+
+Batched samples.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/distributed_storage.py/#L124)
+```python
+.update(
+   *args
+)
+```
+
+---
+Update the storage
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/storage/nstep_replay_storage.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/nstep_replay_storage.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,112 @@
-#
-
-
-## NStepReplayStorage
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/nstep_replay_storage.py\#L68)
-```python 
-NStepReplayStorage(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', storage_size: int = 500000, batch_size: int = 256,
-   num_workers: int = 4, pin_memory: bool = True, n_step: int = 3, discount: float = 0.99,
-   fetch_every: int = 1000, save_snapshot: bool = False
-)
-```
-
-
----
-Replay storage for off-policy algorithms (N-step returns supported).
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **storage_size** (int) : Max number of element in the storage.
-* **batch_size** (int) : Number of samples per batch to load.
-* **num_workers** (int) : Subprocesses to use for data loading.
-* **pin_memory** (bool) : Copy Tensors into device/CUDA pinned memory before returning them.
-* **discount** (float) : The discount factor for future rewards.
-* **fetch_every** (int) : Loading interval.
-* **save_snapshot** (bool) : Save loaded file or not.
-n_step (int) The number of transitions to consider when computing n-step returns
-
-
-**Returns**
-
-N-step replay storage.
-
-
-**Methods:**
-
-
-### .get_batch_size
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/nstep_replay_storage.py\#L126)
-```python
-.get_batch_size()
-```
-
-
-### .get_num_workers
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/nstep_replay_storage.py\#L130)
-```python
-.get_num_workers()
-```
-
-
-### .get_pin_memory
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/nstep_replay_storage.py\#L134)
-```python
-.get_pin_memory()
-```
-
-
-### .add
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/nstep_replay_storage.py\#L141)
-```python
-.add(
-   obs: Any, action: Any, reward: Any, terminated: Any, info: Any, next_obs: Any
-)
-```
-
----
-Add sampled transitions into storage.
-
-
-**Args**
-
-* **obs** (Any) : Observations.
-* **action** (Any) : Actions.
-* **reward** (Any) : Rewards.
-* **terminated** (Any) : Terminateds.
-* **info** (Any) : Infos.
-* **next_obs** (Any) : Next observations.
-
-
-**Returns**
-
-None.
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/nstep_replay_storage.py\#L214)
-```python
-.sample()
-```
-
----
-Generate samples.
-
-
-**Args**
-
-None.
-
-
-**Returns**
-
-Batched samples.
+#
+
+
+## NStepReplayStorage
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/nstep_replay_storage.py/#L191)
+```python 
+NStepReplayStorage(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', storage_size: int = 500000, batch_size: int = 256,
+   num_workers: int = 4, pin_memory: bool = True, n_step: int = 3, discount: float = 0.99,
+   fetch_every: int = 1000, save_snapshot: bool = False
+)
+```
+
+
+---
+Replay storage for off-policy algorithms (N-step returns supported).
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **storage_size** (int) : Max number of element in the storage.
+* **batch_size** (int) : Number of samples per batch to load.
+* **num_workers** (int) : Subprocesses to use for data loading.
+* **pin_memory** (bool) : Copy Tensors into device/CUDA pinned memory before returning them.
+* **discount** (float) : The discount factor for future rewards.
+* **fetch_every** (int) : Loading interval.
+* **save_snapshot** (bool) : Save loaded file or not.
+n_step (int) The number of transitions to consider when computing n-step returns
+
+
+**Returns**
+
+N-step replay storage.
+
+
+**Methods:**
+
+
+### .add
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/nstep_replay_storage.py/#L252)
+```python
+.add(
+   obs: Any, action: Any, reward: Any, terminated: Any, info: Any, next_obs: Any
+)
+```
+
+---
+Add sampled transitions into storage.
+
+
+**Args**
+
+* **obs** (Any) : Observations.
+* **action** (Any) : Actions.
+* **reward** (Any) : Rewards.
+* **terminated** (Any) : Terminateds.
+* **info** (Any) : Infos.
+* **next_obs** (Any) : Next observations.
+
+
+**Returns**
+
+None.
+
+### .replay_iter
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/nstep_replay_storage.py/#L284)
+```python
+.replay_iter()
+```
+
+---
+Create iterable dataloader.
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/nstep_replay_storage.py/#L290)
+```python
+.sample(
+   step: int
+)
+```
+
+---
+Generate samples.
+
+
+**Args**
+
+* **step** (int) : Global training step.
+
+
+**Returns**
+
+Batched samples.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/nstep_replay_storage.py/#L301)
+```python
+.update(
+   *args
+)
+```
+
+---
+Update the storage
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/storage/vanilla_replay_storage.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/vanilla_replay_storage.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,95 @@
-#
-
-
-## VanillaReplayStorage
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/vanilla_replay_storage.py\#L11)
-```python 
-VanillaReplayStorage(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', storage_size: int = 1000000, batch_size: int = 1024
-)
-```
-
-
----
-Vanilla replay storage for off-policy algorithms.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **storage_size** (int) : Max number of element in the buffer.
-* **batch_size** (int) : Batch size of samples.
-
-
-**Returns**
-
-Vanilla replay storage.
-
-
-**Methods:**
-
-
-### .add
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/vanilla_replay_storage.py\#L60)
-```python
-.add(
-   obs: Any, action: Any, reward: Any, terminated: Any, info: Any, next_obs: Any
-)
-```
-
----
-Add sampled transitions into storage.
-
-
-**Args**
-
-* **obs** (Any) : Observations.
-* **action** (Any) : Actions.
-* **reward** (Any) : Rewards.
-* **terminated** (Any) : Terminateds.
-* **info** (Any) : Infos.
-* **next_obs** (Any) : Next observations.
-
-
-**Returns**
-
-None.
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/vanilla_replay_storage.py\#L91)
-```python
-.sample(
-   step: int
-)
-```
-
----
-Sample from the storage.
-
-
-**Args**
-
-* **step** (int) : Global training step.
-
-
-**Returns**
-
-Batched samples.
+#
+
+
+## VanillaReplayStorage
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/vanilla_replay_storage.py/#L11)
+```python 
+VanillaReplayStorage(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', storage_size: int = 1000000, batch_size: int = 1024
+)
+```
+
+
+---
+Vanilla replay storage for off-policy algorithms.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **storage_size** (int) : Max number of element in the buffer.
+* **batch_size** (int) : Batch size of samples.
+
+
+**Returns**
+
+Vanilla replay storage.
+
+
+**Methods:**
+
+
+### .add
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/vanilla_replay_storage.py/#L60)
+```python
+.add(
+   obs: Any, action: Any, reward: Any, terminated: Any, info: Any, next_obs: Any
+)
+```
+
+---
+Add sampled transitions into storage.
+
+
+**Args**
+
+* **obs** (Any) : Observations.
+* **action** (Any) : Actions.
+* **reward** (Any) : Rewards.
+* **terminated** (Any) : Terminateds.
+* **info** (Any) : Infos.
+* **next_obs** (Any) : Next observations.
+
+
+**Returns**
+
+None.
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/vanilla_replay_storage.py/#L91)
+```python
+.sample(
+   step: int
+)
+```
+
+---
+Sample from the storage.
+
+
+**Args**
+
+* **step** (int) : Global training step.
+
+
+**Returns**
+
+Batched samples.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/vanilla_replay_storage.py/#L115)
+```python
+.update(
+   *args
+)
+```
+
+---
+Update the storage
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xploit/storage/vanilla_rollout_storage.md` & `hsuanwu-0.0.1b5/docs/api_docs/xploit/storage/decoupled_rollout_storage.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,123 +1,124 @@
-#
-
-
-## VanillaRolloutStorage
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/vanilla_rollout_storage.py\#L11)
-```python 
-VanillaRolloutStorage(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', num_steps: int = 256, num_envs: int = 8,
-   discount: float = 0.99, gae_lambda: float = 0.95
-)
-```
-
-
----
-Vanilla rollout storage for on-policy algorithms.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **num_steps** (int) : The sample length of per rollout.
-* **num_envs** (int) : The number of parallel environments.
-* **discount** (float) : discount factor.
-* **gae_lambda** (float) : Weighting coefficient for generalized advantage estimation (GAE).
-
-
-**Returns**
-
-Vanilla rollout storage.
-
-
-**Methods:**
-
-
-### .add
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/vanilla_rollout_storage.py\#L83)
-```python
-.add(
-   obs: th.Tensor, actions: th.Tensor, rewards: th.Tensor, terminateds: th.Tensor,
-   truncateds: th.Tensor, next_obs: th.Tensor, log_probs: th.Tensor,
-   values: th.Tensor
-)
-```
-
----
-Add sampled transitions into storage.
-
-
-**Args**
-
-* **obs** (Tensor) : Observations.
-* **actions** (Tensor) : Actions.
-* **rewards** (Tensor) : Rewards.
-* **terminateds** (Tensor) : Terminateds.
-* **truncateds** (Tensor) : Truncateds.
-* **next_obs** (Tensor) : Next observations.
-* **log_probs** (Tensor) : Log of the probability evaluated at `actions`.
-* **values** (Tensor) : Estimated values.
-
-
-**Returns**
-
-None.
-
-### .reset
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/vanilla_rollout_storage.py\#L120)
-```python
-.reset()
-```
-
----
-Reset the terminal state of each env.
-
-### .compute_returns_and_advantages
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/vanilla_rollout_storage.py\#L125)
-```python
-.compute_returns_and_advantages(
-   last_values: th.Tensor
-)
-```
-
----
-Perform generalized advantage estimation (GAE).
-
-
-**Args**
-
-* **last_values** (Tensor) : Estimated values of the last step.
-* **gamma** (float) : Discount factor.
-* **gae_lamdba** (float) : Coefficient of GAE.
-
-
-**Returns**
-
-None.
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xploit/storage/vanilla_rollout_storage.py\#L151)
-```python
-.sample(
-   num_mini_batch: int = 8
-)
-```
-
----
-Sample data from storage.
-
-
-**Args**
-
-* **num_mini_batch** (int) : Number of mini-batches
-
-
-**Returns**
-
-Batch data.
+#
+
+
+## DecoupledRolloutStorage
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/decoupled_rollout_storage.py/#L11)
+```python 
+DecoupledRolloutStorage(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', num_steps: int = 256, num_envs: int = 8,
+   discount: float = 0.99, gae_lambda: float = 0.95
+)
+```
+
+
+---
+Decoupled rollout storage for on-policy algorithms like DAAC.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **num_steps** (int) : The sample length of per rollout.
+* **num_envs** (int) : The number of parallel environments.
+* **discount** (float) : discount factor.
+* **gae_lambda** (float) : Weighting coefficient for generalized advantage estimation (GAE).
+
+
+**Returns**
+
+Vanilla rollout storage.
+
+
+**Methods:**
+
+
+### .add
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/decoupled_rollout_storage.py/#L91)
+```python
+.add(
+   obs: th.Tensor, actions: th.Tensor, rewards: th.Tensor, terminateds: th.Tensor,
+   truncateds: th.Tensor, next_obs: th.Tensor, log_probs: th.Tensor,
+   values: th.Tensor, adv_preds: th.Tensor
+)
+```
+
+---
+Add sampled transitions into storage.
+
+
+**Args**
+
+* **obs** (Tensor) : Observations.
+* **actions** (Tensor) : Actions.
+* **rewards** (Tensor) : Rewards.
+* **terminateds** (Tensor) : Terminateds.
+* **truncateds** (Tensor) : Truncateds.
+* **next_obs** (Tensor) : Next observations.
+* **log_probs** (Tensor) : Log of the probability evaluated at `actions`.
+* **values** (Tensor) : Estimated values.
+* **adv_preds** (Tensor) : Predicted advantages.
+
+
+**Returns**
+
+None.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/decoupled_rollout_storage.py/#L131)
+```python
+.update()
+```
+
+---
+Reset the terminal state of each env.
+
+### .compute_returns_and_advantages
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/decoupled_rollout_storage.py/#L136)
+```python
+.compute_returns_and_advantages(
+   last_values: th.Tensor
+)
+```
+
+---
+Perform generalized advantage estimation (GAE).
+
+
+**Args**
+
+* **last_values** (Tensor) : Estimated values of the last step.
+* **gamma** (float) : Discount factor.
+* **gae_lamdba** (float) : Coefficient of GAE.
+
+
+**Returns**
+
+None.
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xploit/storage/decoupled_rollout_storage.py/#L162)
+```python
+.sample(
+   num_mini_batch: int = 8
+)
+```
+
+---
+Sample data from storage.
+
+
+**Args**
+
+* **num_mini_batch** (int) : Number of mini-batches
+
+
+**Returns**
+
+Batch data.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/auto_augment.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/auto_augment.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#
-
-
-## AutoAugment
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/auto_augment.py\#L7)
-```python 
-AutoAugment(
-   augment_policy: str = T.AutoAugmentPolicy.IMAGENET
-)
-```
-
-
----
-Augmentation method based on “AutoAugment: Learning Augmentation Strategies from Data”.
-
-**Args**
-
-* **augment_policy** (str) : Desired policy enum defined by torchvision.transforms.autoaugment.AutoAugmentPolicy.
-    Default is AutoAugmentPolicy.IMAGENET.
-
-
-**Returns**
-
-Augmented images.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/auto_augment.py\#L24)
-```python
-.forward(
-   x: th.Tensor
-)
-```
-
+#
+
+
+## AutoAugment
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/auto_augment.py/#L7)
+```python 
+AutoAugment(
+   augment_policy: str = T.AutoAugmentPolicy.IMAGENET
+)
+```
+
+
+---
+Augmentation method based on “AutoAugment: Learning Augmentation Strategies from Data”.
+
+**Args**
+
+* **augment_policy** (str) : Desired policy enum defined by torchvision.transforms.autoaugment.AutoAugmentPolicy.
+    Default is AutoAugmentPolicy.IMAGENET.
+
+
+**Returns**
+
+Augmented images.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/auto_augment.py/#L24)
+```python
+.forward(
+   x: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/elastic_transform.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/elastic_transform.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#
-
-
-## ElasticTransform
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/elastic_transform.py\#L7)
-```python 
-ElasticTransform(
-   alpha: float = 50.0, sigma: float = 5.0, interpolation: int = 0, fill = 0
-)
-```
-
-
----
-ElasticTransform method based on “ElasticTransform: Transform a image with elastic transformations”.
-
-**Args**
-
-* **alpha** (float or sequence of python:floats) : Magnitude of displacements. Default is 50.0.
-* **sigma** (float or sequence of python:floats) : Smoothness of displacements. Default is 5.0.
-* **interpolation** (InterpolationMode) : Desired interpolation enum defined by torchvision.transforms.InterpolationMode.
-    Default is InterpolationMode.BILINEAR.
-* **fill** (sequence or int number) : Pixel fill value for the area outside the transformed image. Default is 0.
-
-
-**Returns**
-
-Augmented images.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/elastic_transform.py\#L39)
-```python
-.forward(
-   x: th.Tensor
-)
-```
-
+#
+
+
+## ElasticTransform
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/elastic_transform.py/#L7)
+```python 
+ElasticTransform(
+   alpha: float = 50.0, sigma: float = 5.0, interpolation: int = 0, fill = 0
+)
+```
+
+
+---
+ElasticTransform method based on “ElasticTransform: Transform a image with elastic transformations”.
+
+**Args**
+
+* **alpha** (float or sequence of python:floats) : Magnitude of displacements. Default is 50.0.
+* **sigma** (float or sequence of python:floats) : Smoothness of displacements. Default is 5.0.
+* **interpolation** (InterpolationMode) : Desired interpolation enum defined by torchvision.transforms.InterpolationMode.
+    Default is InterpolationMode.BILINEAR.
+* **fill** (sequence or int number) : Pixel fill value for the area outside the transformed image. Default is 0.
+
+
+**Returns**
+
+Augmented images.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/elastic_transform.py/#L39)
+```python
+.forward(
+   x: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_adjustsharpness.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_adjustsharpness.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-#
-
-
-## RandomAdjustSharpness
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_adjustsharpness.py\#L7)
-```python 
-RandomAdjustSharpness(
-   sharpness_factor: float = 50.0, p: float = 5.0
-)
-```
-
-
----
-RandomAdjustSharpness method based on “RandomAdjustSharpness: Adjust the
-sharpness of the image randomly with a given probability”.
-
-**Args**
-
-* **sharpness_factor** (float) : How much to adjust the sharpness. Can be any non-negative number. Default is 2.
-* **p** (float) : probability of the image being sharpened. Default value is 0.5
-
-
-**Returns**
-
-Augmented images.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_adjustsharpness.py\#L28)
-```python
-.forward(
-   x: th.Tensor
-)
-```
-
+#
+
+
+## RandomAdjustSharpness
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_adjustsharpness.py/#L7)
+```python 
+RandomAdjustSharpness(
+   sharpness_factor: float = 50.0, p: float = 5.0
+)
+```
+
+
+---
+RandomAdjustSharpness method based on “RandomAdjustSharpness: Adjust the
+sharpness of the image randomly with a given probability”.
+
+**Args**
+
+* **sharpness_factor** (float) : How much to adjust the sharpness. Can be any non-negative number. Default is 2.
+* **p** (float) : probability of the image being sharpened. Default value is 0.5
+
+
+**Returns**
+
+Augmented images.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_adjustsharpness.py/#L28)
+```python
+.forward(
+   x: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_amplitude_scaling.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_amplitude_scaling.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-#
-
-
-## RandomAmplitudeScaling
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_amplitude_scaling.py\#L7)
-```python 
-RandomAmplitudeScaling(
-   low: float = 0.6, high: float = 1.2
-)
-```
-
-
----
-Random amplitude scaling operation for processing state-based observations.
-
-
-**Args**
-
-* **low** (float) : lower range (inclusive).
-* **high** (float) : upper range (exclusive).
-
-
-**Returns**
-
-Augmented states.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_amplitude_scaling.py\#L22)
-```python
-.forward(
-   x: th.Tensor
-)
-```
-
+#
+
+
+## RandomAmplitudeScaling
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_amplitude_scaling.py/#L7)
+```python 
+RandomAmplitudeScaling(
+   low: float = 0.6, high: float = 1.2
+)
+```
+
+
+---
+Random amplitude scaling operation for processing state-based observations.
+
+
+**Args**
+
+* **low** (float) : lower range (inclusive).
+* **high** (float) : upper range (exclusive).
+
+
+**Returns**
+
+Augmented states.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_amplitude_scaling.py/#L22)
+```python
+.forward(
+   x: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_colorjitter.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_colorjitter.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-#
-
-
-## RandomColorJitter
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_colorjitter.py\#L7)
-```python 
-RandomColorJitter(
-   brightness: float = 0.4, contrast: float = 0.4, saturation: float = 0.4,
-   hue: float = 0.5
-)
-```
-
-
----
-Random ColorJitter operation for image augmentation.
-
-
-**Args**
-
-* **brightness** (float) : How much to jitter brightness. Should be non negative numbers.
-* **contrast** (float) : How much to jitter contrast. Should be non negative numbers.
-* **saturation** (float) : How much to jitter saturation. Should be non negative numbers.
-* **hue** (float) : How much to jitter hue. Should have 0<= hue <= 0.5 or -0.5 <= min <= max <= 0.5.
-
-
-**Returns**
-
-Augmented images.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_colorjitter.py\#L30)
-```python
-.forward(
-   x: th.Tensor
-)
-```
-
+#
+
+
+## RandomColorJitter
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_colorjitter.py/#L7)
+```python 
+RandomColorJitter(
+   brightness: float = 0.4, contrast: float = 0.4, saturation: float = 0.4,
+   hue: float = 0.5
+)
+```
+
+
+---
+Random ColorJitter operation for image augmentation.
+
+
+**Args**
+
+* **brightness** (float) : How much to jitter brightness. Should be non negative numbers.
+* **contrast** (float) : How much to jitter contrast. Should be non negative numbers.
+* **saturation** (float) : How much to jitter saturation. Should be non negative numbers.
+* **hue** (float) : How much to jitter hue. Should have 0<= hue <= 0.5 or -0.5 <= min <= max <= 0.5.
+
+
+**Returns**
+
+Augmented images.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_colorjitter.py/#L30)
+```python
+.forward(
+   x: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_cutout.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_cutoutcolor.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#
-
-
-## RandomCutout
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_cutout.py\#L6)
-```python 
-RandomCutout(
-   min_cut: int = 10, max_cut: int = 30
-)
-```
-
-
----
-Random Cutout operation for image augmentation.
-
-**Args**
-
-* **min_cut** (int) : Min size of the cut shape.
-* **max_cut** (int) : Max size of the cut shape.
-
-
-**Returns**
-
-Augmented images.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_cutout.py\#L21)
-```python
-.forward(
-   x: th.Tensor
-)
-```
-
+#
+
+
+## RandomCutoutColor
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_cutoutcolor.py/#L6)
+```python 
+RandomCutoutColor(
+   min_cut: int = 10, max_cut: int = 30
+)
+```
+
+
+---
+Random Cutout operation for image augmentation.
+
+**Args**
+
+* **min_cut** (int) : min size of the cut shape.
+* **max_cut** (int) : max size of the cut shape.
+
+
+**Returns**
+
+Augmented images.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_cutoutcolor.py/#L21)
+```python
+.forward(
+   x: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_cutoutcolor.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_cutout.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#
-
-
-## RandomCutoutColor
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_cutoutcolor.py\#L6)
-```python 
-RandomCutoutColor(
-   min_cut: int = 10, max_cut: int = 30
-)
-```
-
-
----
-Random Cutout operation for image augmentation.
-
-**Args**
-
-* **min_cut** (int) : min size of the cut shape.
-* **max_cut** (int) : max size of the cut shape.
-
-
-**Returns**
-
-Augmented images.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_cutoutcolor.py\#L21)
-```python
-.forward(
-   x: th.Tensor
-)
-```
-
+#
+
+
+## RandomCutout
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_cutout.py/#L6)
+```python 
+RandomCutout(
+   min_cut: int = 10, max_cut: int = 30
+)
+```
+
+
+---
+Random Cutout operation for image augmentation.
+
+**Args**
+
+* **min_cut** (int) : Min size of the cut shape.
+* **max_cut** (int) : Max size of the cut shape.
+
+
+**Returns**
+
+Augmented images.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_cutout.py/#L21)
+```python
+.forward(
+   x: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_perspective.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_perspective.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-#
-
-
-## RandomPerspective
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_perspective.py\#L7)
-```python 
-RandomPerspective(
-   distortion_scale: float = 0.5, p: float = 0.5, interpolation: int = 0, fill = 0
-)
-```
-
-
----
-RandomPerspective method based on “RandomPerspective: Performs
-a random perspective transformation of the given image with a given probability.”.
-
-**Args**
-
-* **distortion_scale** (float) : argument to control the degree of distortion and ranges from 0 to 1. Default is 0.5.
-* **p** (float) : Smoothness of displacements. Default is 5.0.
-* **interpolation** (Union, InterpolationMode) : Desired interpolation enum defined by
-    torchvision.transforms.InterpolationMode. Default is InterpolationMode.BILINEAR.
-* **fill** (sequence or int number) : Pixel fill value for the area outside the transformed image. Default is 0.
-
-
-**Returns**
-
-Augmented images.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_perspective.py\#L40)
-```python
-.forward(
-   x: th.Tensor
-)
-```
-
+#
+
+
+## RandomPerspective
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_perspective.py/#L7)
+```python 
+RandomPerspective(
+   distortion_scale: float = 0.5, p: float = 0.5, interpolation: int = 0, fill = 0
+)
+```
+
+
+---
+RandomPerspective method based on “RandomPerspective: Performs
+a random perspective transformation of the given image with a given probability.”.
+
+**Args**
+
+* **distortion_scale** (float) : argument to control the degree of distortion and ranges from 0 to 1. Default is 0.5.
+* **p** (float) : Smoothness of displacements. Default is 5.0.
+* **interpolation** (Union, InterpolationMode) : Desired interpolation enum defined by
+    torchvision.transforms.InterpolationMode. Default is InterpolationMode.BILINEAR.
+* **fill** (sequence or int number) : Pixel fill value for the area outside the transformed image. Default is 0.
+
+
+**Returns**
+
+Augmented images.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_perspective.py/#L40)
+```python
+.forward(
+   x: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_rotate.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/augmentation/random_rotate.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#
-
-
-## RandomRotate
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_rotate.py\#L6)
-```python 
-RandomRotate(
-   p: float = 0.2
-)
-```
-
-
----
-Random rotate operation for processing image-based observations.
-
-
-**Args**
-
-* **p** (float) : The image rotate problistily in a batch.
-
-
-**Returns**
-
-Random rotate image in a batch.
-
-
-**Methods:**
-
-
-### .forward
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/augmentation/random_rotate.py\#L20)
-```python
-.forward(
-   x: th.Tensor
-)
-```
-
+#
+
+
+## RandomRotate
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_rotate.py/#L6)
+```python 
+RandomRotate(
+   p: float = 0.2
+)
+```
+
+
+---
+Random rotate operation for processing image-based observations.
+
+
+**Args**
+
+* **p** (float) : The image rotate problistily in a batch.
+
+
+**Returns**
+
+Random rotate image in a batch.
+
+
+**Methods:**
+
+
+### .forward
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/augmentation/random_rotate.py/#L20)
+```python
+.forward(
+   x: th.Tensor
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/distribution/base.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/bernoulli.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,151 @@
-#
-
-
-## BaseDistribution
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/base.py\#L6)
-```python 
-
-```
-
-
----
-Abstract base class of distributions.
-
-
-**Methods:**
-
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/base.py\#L14)
-```python
-.sample(
-   sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped sample or sample_shape shaped batch of
-samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .rsample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/base.py\#L26)
-```python
-.rsample(
-   sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped sample or sample_shape shaped batch of
-samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .log_prob
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/base.py\#L38)
-```python
-.log_prob(
-   value: th.Tensor
-)
-```
-
----
-Returns the log of the probability density/mass function evaluated at `value`.
-
-
-**Args**
-
-* **value** (Tensor) : The value to be evaluated.
-
-
-**Returns**
-
-The log_prob value.
-
-### .entropy
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/base.py\#L49)
-```python
-.entropy()
-```
-
----
-Returns the Shannon entropy of distribution.
-
-### .reset
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/base.py\#L53)
-```python
-.reset()
-```
-
----
-Reset the distribution.
-
-### .mean
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/base.py\#L57)
-```python
-.mean()
-```
-
----
-Returns the mean of the distribution.
-
-### .mode
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/base.py\#L61)
-```python
-.mode()
-```
-
----
-Returns the mode of the distribution.
+#
+
+
+## Bernoulli
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L7)
+```python 
+Bernoulli(
+   logits: th.Tensor
+)
+```
+
+
+---
+Bernoulli distribution for sampling actions for 'MultiBinary' tasks.
+
+**Args**
+
+* **logits** (Tensor) : The event log probabilities (unnormalized).
+
+
+**Returns**
+
+Categorical distribution instance.
+
+
+**Methods:**
+
+
+### .probs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L24)
+```python
+.probs()
+```
+
+---
+Return probabilities.
+
+### .logits
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L29)
+```python
+.logits()
+```
+
+---
+Returns the unnormalized log probabilities.
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L33)
+```python
+.sample(
+   sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped sample or sample_shape shaped batch of
+samples if the distribution parameters are batched.
+
+
+**Args**
+
+* **sample_shape** (TorchSize) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .log_prob
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L45)
+```python
+.log_prob(
+   actions: th.Tensor
+)
+```
+
+---
+Returns the log of the probability density/mass function evaluated at actions.
+
+
+**Args**
+
+* **actions** (Tensor) : The actions to be evaluated.
+
+
+**Returns**
+
+The log_prob value.
+
+### .entropy
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L56)
+```python
+.entropy()
+```
+
+---
+Returns the Shannon entropy of distribution.
+
+### .mode
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L61)
+```python
+.mode()
+```
+
+---
+Returns the mode of the distribution.
+
+### .mean
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L66)
+```python
+.mean()
+```
+
+---
+Returns the mean of the distribution.
+
+### .stddev
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L71)
+```python
+.stddev()
+```
+
+---
+Returns the standard deviation of the distribution.
+
+### .variance
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L76)
+```python
+.variance()
+```
+
+---
+Returns the variance of the distribution.
+
+### .reset
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L80)
+```python
+.reset()
+```
+
+---
+Reset the distribution.
+
+### .rsample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/bernoulli.py/#L84)
+```python
+.rsample(
+   sample_shape: th.Size = ...
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/distribution/categorical.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/categorical.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,151 @@
-#
-
-
-## Categorical
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L7)
-```python 
-Categorical(
-   logits: th.Tensor
-)
-```
-
-
----
-Categorical distribution for sampling actions in discrete control tasks.
-
-**Args**
-
-* **logits** (Tensor) : The event log probabilities (unnormalized).
-
-
-**Returns**
-
-Categorical distribution instance.
-
-
-**Methods:**
-
-
-### .probs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L25)
-```python
-.probs()
-```
-
----
-Return probabilities.
-
-### .logits
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L30)
-```python
-.logits()
-```
-
----
-Returns the unnormalized log probabilities.
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L34)
-```python
-.sample(
-   sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped sample or sample_shape shaped batch of
-samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **sample_shape** (TorchSize) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .log_prob
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L46)
-```python
-.log_prob(
-   actions: th.Tensor
-)
-```
-
----
-Returns the log of the probability density/mass function evaluated at `value`.
-
-
-**Args**
-
-* **actions** (Tensor) : The actions to be evaluated.
-
-
-**Returns**
-
-The log_prob value.
-
-### .entropy
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L57)
-```python
-.entropy()
-```
-
----
-Returns the Shannon entropy of distribution.
-
-### .mode
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L62)
-```python
-.mode()
-```
-
----
-Returns the mode of the distribution.
-
-### .mean
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L67)
-```python
-.mean()
-```
-
----
-Returns the mean of the distribution.
-
-### .reset
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L71)
-```python
-.reset()
-```
-
----
-Reset the distribution.
-
-### .rsample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/categorical.py\#L75)
-```python
-.rsample(
-   sample_shape: th.Size = ...
-)
-```
-
+#
+
+
+## Categorical
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L7)
+```python 
+Categorical(
+   logits: th.Tensor
+)
+```
+
+
+---
+Categorical distribution for sampling actions for 'Discrete' tasks.
+
+**Args**
+
+* **logits** (Tensor) : The event log probabilities (unnormalized).
+
+
+**Returns**
+
+Categorical distribution instance.
+
+
+**Methods:**
+
+
+### .probs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L24)
+```python
+.probs()
+```
+
+---
+Return probabilities.
+
+### .logits
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L29)
+```python
+.logits()
+```
+
+---
+Returns the unnormalized log probabilities.
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L33)
+```python
+.sample(
+   sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped sample or sample_shape shaped batch of
+samples if the distribution parameters are batched.
+
+
+**Args**
+
+* **sample_shape** (TorchSize) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .log_prob
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L45)
+```python
+.log_prob(
+   actions: th.Tensor
+)
+```
+
+---
+Returns the log of the probability density/mass function evaluated at actions.
+
+
+**Args**
+
+* **actions** (Tensor) : The actions to be evaluated.
+
+
+**Returns**
+
+The log_prob value.
+
+### .entropy
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L56)
+```python
+.entropy()
+```
+
+---
+Returns the Shannon entropy of distribution.
+
+### .mode
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L61)
+```python
+.mode()
+```
+
+---
+Returns the mode of the distribution.
+
+### .mean
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L66)
+```python
+.mean()
+```
+
+---
+Returns the mean of the distribution.
+
+### .stddev
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L71)
+```python
+.stddev()
+```
+
+---
+Returns the standard deviation of the distribution.
+
+### .variance
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L76)
+```python
+.variance()
+```
+
+---
+Returns the variance of the distribution.
+
+### .reset
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L80)
+```python
+.reset()
+```
+
+---
+Reset the distribution.
+
+### .rsample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/categorical.py/#L84)
+```python
+.rsample(
+   sample_shape: th.Size = ...
+)
+```
+
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/distribution/diagonal_gaussian.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/diagonal_gaussian.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,148 @@
-#
-
-
-## DiagonalGaussian
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/diagonal_gaussian.py\#L7)
-```python 
-DiagonalGaussian(
-   mu: th.Tensor, sigma: th.Tensor
-)
-```
-
-
----
-Diagonal Gaussian distribution for 'Box' tasks.
-
-
-**Args**
-
-* **mu** (Tensor) : The mean of the distribution (often referred to as mu).
-* **sigma** (Tensor) : The standard deviation of the distribution (often referred to as sigma).
-
-
-**Returns**
-
-Squashed normal distribution instance.
-
-
-**Methods:**
-
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/diagonal_gaussian.py\#L25)
-```python
-.sample(
-   sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped sample or sample_shape shaped batch of
-samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .rsample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/diagonal_gaussian.py\#L37)
-```python
-.rsample(
-   sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped reparameterized sample or sample_shape shaped batch of
-reparameterized samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .mean
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/diagonal_gaussian.py\#L50)
-```python
-.mean()
-```
-
----
-Return the transformed mean.
-
-### .log_prob
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/diagonal_gaussian.py\#L54)
-```python
-.log_prob(
-   actions: th.Tensor
-)
-```
-
----
-Scores the sample by inverting the transform(s) and computing the score using the
-score of the base distribution and the log abs det jacobian.
-
-**Args**
-
-* **actions** (Tensor) : The actions to be evaluated.
-
-
-**Returns**
-
-The log_prob value.
-
-### .reset
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/diagonal_gaussian.py\#L65)
-```python
-.reset()
-```
-
----
-Reset the distribution.
-
-### .entropy
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/diagonal_gaussian.py\#L69)
-```python
-.entropy()
-```
-
----
-Returns the Shannon entropy of distribution.
-
-### .mode
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/diagonal_gaussian.py\#L73)
-```python
-.mode()
-```
-
----
-Returns the mode of the distribution.
+#
+
+
+## DiagonalGaussian
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L7)
+```python 
+DiagonalGaussian(
+   loc: th.Tensor, scale: th.Tensor
+)
+```
+
+
+---
+Diagonal Gaussian distribution for 'Box' tasks.
+
+
+**Args**
+
+* **loc** (Tensor) : The mean of the distribution (often referred to as mu).
+* **scale** (Tensor) : The standard deviation of the distribution (often referred to as sigma).
+
+
+**Returns**
+
+Squashed normal distribution instance.
+
+
+**Methods:**
+
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L25)
+```python
+.sample(
+   sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped sample or sample_shape shaped batch of
+samples if the distribution parameters are batched.
+
+
+**Args**
+
+* **sample_shape** (Size) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .rsample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L37)
+```python
+.rsample(
+   sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped reparameterized sample or sample_shape shaped batch of
+reparameterized samples if the distribution parameters are batched.
+
+
+**Args**
+
+* **sample_shape** (Size) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .mean
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L50)
+```python
+.mean()
+```
+
+---
+Returns the mean of the distribution.
+
+### .mode
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L55)
+```python
+.mode()
+```
+
+---
+Returns the mode of the distribution.
+
+### .stddev
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L60)
+```python
+.stddev()
+```
+
+---
+Returns the standard deviation of the distribution.
+
+### .variance
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L65)
+```python
+.variance()
+```
+
+---
+Returns the variance of the distribution.
+
+### .log_prob
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L69)
+```python
+.log_prob(
+   actions: th.Tensor
+)
+```
+
+---
+Returns the log of the probability density/mass function evaluated at actions.
+
+
+**Args**
+
+* **actions** (Tensor) : The actions to be evaluated.
+
+
+**Returns**
+
+The log_prob value.
+
+### .reset
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L80)
+```python
+.reset()
+```
+
+---
+Reset the distribution.
+
+### .entropy
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/diagonal_gaussian.py/#L84)
+```python
+.entropy()
+```
+
+---
+Returns the Shannon entropy of distribution.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/distribution/normal_noise.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/normal_noise.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,146 +1,164 @@
-#
-
-
-## NormalNoise
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/normal_noise.py\#L8)
-```python 
-NormalNoise(
-   mu: float = 0.0, sigma: float = 1.0, stddev_schedule: str = 'linear(1.0, 0.1,
-   100000)', stddev_clip: float = 0.3
-)
-```
-
-
----
-Gaussian action noise.
-
-
-**Args**
-
-* **mu** (float) : mean of the noise (often referred to as mu).
-* **sigma** (float) : standard deviation of the noise (often referred to as sigma).
-* **stddev_schedule** (str) : Use the exploration std schedule.
-
-
-**Returns**
-
-Gaussian action noise instance.
-
-
-**Methods:**
-
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/normal_noise.py\#L33)
-```python
-.sample(
-   clip: bool = False, sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped sample or sample_shape shaped batch of
-samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **clip** (bool) : Whether to perform noise truncation.
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .rsample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/normal_noise.py\#L52)
-```python
-.rsample(
-   sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped sample or sample_shape shaped batch of
-samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .log_prob
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/normal_noise.py\#L64)
-```python
-.log_prob(
-   value: th.Tensor
-)
-```
-
----
-Returns the log of the probability density/mass function evaluated at `value`.
-
-
-**Args**
-
-* **value** (Tensor) : The value to be evaluated.
-
-
-**Returns**
-
-The log_prob value.
-
-### .entropy
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/normal_noise.py\#L75)
-```python
-.entropy()
-```
-
----
-Returns the Shannon entropy of distribution.
-
-### .reset
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/normal_noise.py\#L79)
-```python
-.reset(
-   noiseless_action: th.Tensor, step: int = 0
-)
-```
-
----
-Reset the noise instance.
-
-
-**Args**
-
-* **noiseless_action** (Tensor) : Unprocessed actions.
-* **step** (int) : Global training step that can be None when there is no noise schedule.
-
-
-**Returns**
-
-None.
-
-### .mean
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/normal_noise.py\#L95)
-```python
-.mean()
-```
-
----
-Returns the mean of the distribution.
-
-### .mode
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/normal_noise.py\#L100)
-```python
-.mode()
-```
-
----
-Returns the mode of the distribution.
+#
+
+
+## NormalNoise
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L8)
+```python 
+NormalNoise(
+   loc: float = 0.0, scale: float = 1.0, stddev_schedule: str = 'linear(1.0, 0.1,
+   100000)', stddev_clip: float = 0.3
+)
+```
+
+
+---
+Gaussian action noise.
+
+
+**Args**
+
+* **loc** (float) : mean of the noise (often referred to as mu).
+* **scale** (float) : standard deviation of the noise (often referred to as sigma).
+* **stddev_schedule** (str) : Use the exploration std schedule.
+
+
+**Returns**
+
+Gaussian action noise instance.
+
+
+**Methods:**
+
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L35)
+```python
+.sample(
+   clip: bool = False, sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped sample or sample_shape shaped batch of
+samples if the distribution parameters are batched.
+
+
+**Args**
+
+* **clip** (bool) : Whether to perform noise truncation.
+* **sample_shape** (Size) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .rsample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L54)
+```python
+.rsample(
+   sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped sample or sample_shape shaped batch of
+samples if the distribution parameters are batched.
+
+
+**Args**
+
+* **sample_shape** (Size) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .log_prob
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L66)
+```python
+.log_prob(
+   value: th.Tensor
+)
+```
+
+---
+Returns the log of the probability density/mass function evaluated at `value`.
+
+
+**Args**
+
+* **value** (Tensor) : The value to be evaluated.
+
+
+**Returns**
+
+The log_prob value.
+
+### .entropy
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L77)
+```python
+.entropy()
+```
+
+---
+Returns the Shannon entropy of distribution.
+
+### .reset
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L81)
+```python
+.reset(
+   noiseless_action: th.Tensor, step: int = 0
+)
+```
+
+---
+Reset the noise instance.
+
+
+**Args**
+
+* **noiseless_action** (Tensor) : Unprocessed actions.
+* **step** (int) : Global training step that can be None when there is no noise schedule.
+
+
+**Returns**
+
+None.
+
+### .mean
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L97)
+```python
+.mean()
+```
+
+---
+Returns the mean of the distribution.
+
+### .mode
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L102)
+```python
+.mode()
+```
+
+---
+Returns the mode of the distribution.
+
+### .stddev
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L107)
+```python
+.stddev()
+```
+
+---
+Returns the standard deviation of the distribution.
+
+### .variance
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/normal_noise.py/#L112)
+```python
+.variance()
+```
+
+---
+Returns the variance of the distribution.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/distribution/ornstein_uhlenbeck_noise.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/ornstein_uhlenbeck_noise.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,147 +1,165 @@
-#
-
-
-## OrnsteinUhlenbeckNoise
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py\#L9)
-```python 
-OrnsteinUhlenbeckNoise(
-   mu: float = 0.0, sigma: float = 1.0, theta: float = 0.15, dt: float = 0.01,
-   stddev_schedule: str = 'linear(1.0, 0.1, 100000)'
-)
-```
-
-
----
-Ornstein Uhlenbeck action noise.
-Based on http://math.stackexchange.com/questions/1287634/implementing-ornstein-uhlenbeck-in-matlab
-
-
-**Args**
-
-* **mu** (float) : mean of the noise (often referred to as mu).
-* **sigma** (float) : standard deviation of the noise (often referred to as sigma).
-* **theta** (float) : Rate of mean reversion.
-* **dt** (float) : Timestep for the noise.
-
-
-**Returns**
-
-Ornstein-Uhlenbeck noise instance.
-
-
-**Methods:**
-
-
-### .reset
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py\#L42)
-```python
-.reset(
-   noiseless_action: th.Tensor, step: int = 0
-)
-```
-
----
-Reset the noise instance.
-
-
-**Args**
-
-* **noiseless_action** (Tensor) : Unprocessed actions.
-* **step** (int) : Global training step that can be None when there is no noise schedule.
-
-
-**Returns**
-
-None.
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py\#L59)
-```python
-.sample(
-   clip: bool = False, sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped sample
-
-
-**Args**
-
-* **clip** (bool) : Range for noise truncation operation.
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .mean
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py\#L90)
-```python
-.mean()
-```
-
----
-Returns the mean of the distribution.
-
-### .mode
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py\#L95)
-```python
-.mode()
-```
-
----
-Returns the mode of the distribution.
-
-### .rsample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py\#L99)
-```python
-.rsample(
-   sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped sample or sample_shape shaped batch of
-samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .log_prob
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py\#L111)
-```python
-.log_prob(
-   value: th.Tensor
-)
-```
-
----
-Returns the log of the probability density/mass function evaluated at `value`.
-
-
-**Args**
-
-* **value** (Tensor) : The value to be evaluated.
-
-
-**Returns**
-
-The log_prob value.
-
-### .entropy
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py\#L122)
-```python
-.entropy()
-```
-
----
-Returns the Shannon entropy of distribution.
+#
+
+
+## OrnsteinUhlenbeckNoise
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L9)
+```python 
+OrnsteinUhlenbeckNoise(
+   loc: float = 0.0, scale: float = 1.0, theta: float = 0.15, dt: float = 0.01,
+   stddev_schedule: str = 'linear(1.0, 0.1, 100000)'
+)
+```
+
+
+---
+Ornstein Uhlenbeck action noise.
+Based on http://math.stackexchange.com/questions/1287634/implementing-ornstein-uhlenbeck-in-matlab
+
+
+**Args**
+
+* **loc** (float) : mean of the noise (often referred to as mu).
+* **scale** (float) : standard deviation of the noise (often referred to as sigma).
+* **theta** (float) : Rate of mean reversion.
+* **dt** (float) : Timestep for the noise.
+
+
+**Returns**
+
+Ornstein-Uhlenbeck noise instance.
+
+
+**Methods:**
+
+
+### .reset
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L42)
+```python
+.reset(
+   noiseless_action: th.Tensor, step: int = 0
+)
+```
+
+---
+Reset the noise instance.
+
+
+**Args**
+
+* **noiseless_action** (Tensor) : Unprocessed actions.
+* **step** (int) : Global training step that can be None when there is no noise schedule.
+
+
+**Returns**
+
+None.
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L59)
+```python
+.sample(
+   clip: bool = False, sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped sample
+
+
+**Args**
+
+* **clip** (bool) : Range for noise truncation operation.
+* **sample_shape** (Size) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .mean
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L90)
+```python
+.mean()
+```
+
+---
+Returns the mean of the distribution.
+
+### .mode
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L95)
+```python
+.mode()
+```
+
+---
+Returns the mode of the distribution.
+
+### .rsample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L99)
+```python
+.rsample(
+   sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped sample or sample_shape shaped batch of
+samples if the distribution parameters are batched.
+
+
+**Args**
+
+* **sample_shape** (Size) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .log_prob
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L111)
+```python
+.log_prob(
+   value: th.Tensor
+)
+```
+
+---
+Returns the log of the probability density/mass function evaluated at `value`.
+
+
+**Args**
+
+* **value** (Tensor) : The value to be evaluated.
+
+
+**Returns**
+
+The log_prob value.
+
+### .entropy
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L122)
+```python
+.entropy()
+```
+
+---
+Returns the Shannon entropy of distribution.
+
+### .stddev
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L127)
+```python
+.stddev()
+```
+
+---
+Returns the standard deviation of the distribution.
+
+### .variance
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py/#L132)
+```python
+.variance()
+```
+
+---
+Returns the variance of the distribution.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/distribution/squashed_normal.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/distribution/squashed_normal.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,148 @@
-#
-
-
-## SquashedNormal
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/squashed_normal.py\#L39)
-```python 
-SquashedNormal(
-   mu: th.Tensor, sigma: th.Tensor
-)
-```
-
-
----
-Squashed normal distribution for Soft Actor-Critic learner.
-
-
-**Args**
-
-* **mu** (Tensor) : The mean of the distribution (often referred to as mu).
-* **sigma** (Tensor) : The standard deviation of the distribution (often referred to as sigma).
-
-
-**Returns**
-
-Squashed normal distribution instance.
-
-
-**Methods:**
-
-
-### .sample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/squashed_normal.py\#L60)
-```python
-.sample(
-   sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped sample or sample_shape shaped
-batch of samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .rsample
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/squashed_normal.py\#L72)
-```python
-.rsample(
-   sample_shape: th.Size = th.Size()
-)
-```
-
----
-Generates a sample_shape shaped reparameterized sample or sample_shape shaped
-batch of reparameterized samples if the distribution parameters are batched.
-
-
-**Args**
-
-* **sample_shape** (Size) : The size of the sample to be drawn.
-
-
-**Returns**
-
-A sample_shape shaped sample.
-
-### .mean
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/squashed_normal.py\#L85)
-```python
-.mean()
-```
-
----
-Return the transformed mean.
-
-### .log_prob
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/squashed_normal.py\#L92)
-```python
-.log_prob(
-   actions: th.Tensor
-)
-```
-
----
-Scores the sample by inverting the transform(s) and computing the score using
-the score of the base distribution and the log abs det jacobian.
-
-**Args**
-
-* **actions** (Tensor) : The actions to be evaluated.
-
-
-**Returns**
-
-The log_prob value.
-
-### .reset
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/squashed_normal.py\#L103)
-```python
-.reset()
-```
-
----
-Reset the distribution.
-
-### .entropy
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/squashed_normal.py\#L107)
-```python
-.entropy()
-```
-
----
-Returns the Shannon entropy of distribution.
-
-### .mode
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/distribution/squashed_normal.py\#L111)
-```python
-.mode()
-```
-
----
-Returns the mode of the distribution.
+#
+
+
+## SquashedNormal
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L39)
+```python 
+SquashedNormal(
+   loc: th.Tensor, scale: th.Tensor
+)
+```
+
+
+---
+Squashed normal distribution for Soft Actor-Critic learner.
+
+
+**Args**
+
+* **loc** (Tensor) : The mean of the distribution (often referred to as mu).
+* **scale** (Tensor) : The standard deviation of the distribution (often referred to as sigma).
+
+
+**Returns**
+
+Squashed normal distribution instance.
+
+
+**Methods:**
+
+
+### .sample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L60)
+```python
+.sample(
+   sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped sample or sample_shape shaped
+batch of samples if the distribution parameters are batched.
+
+
+**Args**
+
+* **sample_shape** (Size) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .rsample
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L72)
+```python
+.rsample(
+   sample_shape: th.Size = th.Size()
+)
+```
+
+---
+Generates a sample_shape shaped reparameterized sample or sample_shape shaped
+batch of reparameterized samples if the distribution parameters are batched.
+
+
+**Args**
+
+* **sample_shape** (Size) : The size of the sample to be drawn.
+
+
+**Returns**
+
+A sample_shape shaped sample.
+
+### .mean
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L85)
+```python
+.mean()
+```
+
+---
+Return the transformed mean.
+
+### .mode
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L93)
+```python
+.mode()
+```
+
+---
+Returns the mode of the distribution.
+
+### .log_prob
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L97)
+```python
+.log_prob(
+   actions: th.Tensor
+)
+```
+
+---
+Scores the sample by inverting the transform(s) and computing the score using
+the score of the base distribution and the log abs det jacobian.
+
+**Args**
+
+* **actions** (Tensor) : The actions to be evaluated.
+
+
+**Returns**
+
+The log_prob value.
+
+### .entropy
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L108)
+```python
+.entropy()
+```
+
+---
+Returns the Shannon entropy of distribution.
+
+### .stddev
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L113)
+```python
+.stddev()
+```
+
+---
+Returns the standard deviation of the distribution.
+
+### .variance
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L118)
+```python
+.variance()
+```
+
+---
+Returns the variance of the distribution.
+
+### .reset
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/distribution/squashed_normal.py/#L122)
+```python
+.reset()
+```
+
+---
+Reset the distribution.
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/reward/base.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/base.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-#
-
-
-## BaseIntrinsicRewardModule
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/base.py\#L9)
-```python 
-BaseIntrinsicRewardModule(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05
-)
-```
-
-
----
-Base class of intrinsic reward module.
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
-* **kappa** (float) : The decay rate.
-
-
-**Returns**
-
-Instance of the base intrinsic reward module.
-
-
-**Methods:**
-
-
-### .compute_irs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/base.py\#L59)
-```python
-.compute_irs(
-   samples: Dict, step: int = 0
-)
-```
-
----
-Compute the intrinsic rewards for current samples.
-
-
-**Args**
-
-* **samples** (Dict) : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-* **step** (int) : The global training step.
-
-
-**Returns**
-
-The intrinsic rewards.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/base.py\#L75)
-```python
-.update(
-   samples: Dict
-)
-```
-
----
-Update the intrinsic reward module if necessary.
-
-
-**Args**
-
-* **samples**  : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-
-
-**Returns**
-
-None
+#
+
+
+## BaseIntrinsicRewardModule
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/base.py/#L9)
+```python 
+BaseIntrinsicRewardModule(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05
+)
+```
+
+
+---
+Base class of intrinsic reward module.
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
+* **kappa** (float) : The decay rate.
+
+
+**Returns**
+
+Instance of the base intrinsic reward module.
+
+
+**Methods:**
+
+
+### .compute_irs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/base.py/#L61)
+```python
+.compute_irs(
+   samples: Dict, step: int = 0
+)
+```
+
+---
+Compute the intrinsic rewards for current samples.
+
+
+**Args**
+
+* **samples** (Dict) : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+* **step** (int) : The global training step.
+
+
+**Returns**
+
+The intrinsic rewards.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/base.py/#L77)
+```python
+.update(
+   samples: Dict
+)
+```
+
+---
+Update the intrinsic reward module if necessary.
+
+
+**Args**
+
+* **samples**  : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+
+
+**Returns**
+
+None
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/reward/girm.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/girm.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-#
-
-
-## GIRM
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/girm.py\#L169)
-```python 
-GIRM(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
-   latent_dim: int = 128, lr: float = 0.001, batch_size: int = 64, lambd: float = 0.5,
-   lambd_recon: float = 1.0, lambd_action: float = 1.0, kld_loss_beta: float = 1.0
-)
-```
-
-
----
-Intrinsic Reward Driven Imitation Learning via Generative Model (GIRM).
-See paper: http://proceedings.mlr.press/v119/yu20d/yu20d.pdf
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
-* **kappa** (float) : The decay rate.
-* **latent_dim** (int) : The dimension of encoding vectors.
-* **lr** (float) : The learning rate.
-* **batch_size** (int) : The batch size for update.
-* **lambd** (float) : The weighting coefficient for combining actions.
-* **lambd_recon** (float) : Weighting coefficient of the reconstruction loss.
-* **lambd_action** (float) : Weighting coefficient of the action loss.
-* **kld_loss_beta** (float) : Weighting coefficient of the divergence loss.
-
-
-**Returns**
-
-Instance of GIRM.
-
-
-**Methods:**
-
-
-### .get_vae_loss
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/girm.py\#L233)
-```python
-.get_vae_loss(
-   recon_x: th.Tensor, x: th.Tensor, mean: th.Tensor, logvar: th.Tensor
-)
-```
-
----
-Compute the vae loss.
-
-
-**Args**
-
-* **recon_x** (Tensor) : Reconstructed x.
-* **x** (Tensor) : Input x.
-* **mean** (Tensor) : Sample mean.
-* **logvar** (Tensor) : Log of the sample variance.
-
-
-**Returns**
-
-Loss values.
-
-### .compute_irs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/girm.py\#L250)
-```python
-.compute_irs(
-   samples: Dict, step: int = 0
-)
-```
-
----
-Compute the intrinsic rewards for current samples.
-
-
-**Args**
-
-* **samples** (Dict) : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-* **step** (int) : The global training step.
-
-
-**Returns**
-
-The intrinsic rewards.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/girm.py\#L299)
-```python
-.update(
-   samples: Dict
-)
-```
-
----
-Update the intrinsic reward module if necessary.
-
-
-**Args**
-
-* **samples**  : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-
-
-**Returns**
-
-None
+#
+
+
+## GIRM
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/girm.py/#L169)
+```python 
+GIRM(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
+   latent_dim: int = 128, lr: float = 0.001, batch_size: int = 64, lambd: float = 0.5,
+   lambd_recon: float = 1.0, lambd_action: float = 1.0, kld_loss_beta: float = 1.0
+)
+```
+
+
+---
+Intrinsic Reward Driven Imitation Learning via Generative Model (GIRM).
+See paper: http://proceedings.mlr.press/v119/yu20d/yu20d.pdf
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
+* **kappa** (float) : The decay rate.
+* **latent_dim** (int) : The dimension of encoding vectors.
+* **lr** (float) : The learning rate.
+* **batch_size** (int) : The batch size for update.
+* **lambd** (float) : The weighting coefficient for combining actions.
+* **lambd_recon** (float) : Weighting coefficient of the reconstruction loss.
+* **lambd_action** (float) : Weighting coefficient of the action loss.
+* **kld_loss_beta** (float) : Weighting coefficient of the divergence loss.
+
+
+**Returns**
+
+Instance of GIRM.
+
+
+**Methods:**
+
+
+### .get_vae_loss
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/girm.py/#L233)
+```python
+.get_vae_loss(
+   recon_x: th.Tensor, x: th.Tensor, mean: th.Tensor, logvar: th.Tensor
+)
+```
+
+---
+Compute the vae loss.
+
+
+**Args**
+
+* **recon_x** (Tensor) : Reconstructed x.
+* **x** (Tensor) : Input x.
+* **mean** (Tensor) : Sample mean.
+* **logvar** (Tensor) : Log of the sample variance.
+
+
+**Returns**
+
+Loss values.
+
+### .compute_irs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/girm.py/#L250)
+```python
+.compute_irs(
+   samples: Dict, step: int = 0
+)
+```
+
+---
+Compute the intrinsic rewards for current samples.
+
+
+**Args**
+
+* **samples** (Dict) : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+* **step** (int) : The global training step.
+
+
+**Returns**
+
+The intrinsic rewards.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/girm.py/#L299)
+```python
+.update(
+   samples: Dict
+)
+```
+
+---
+Update the intrinsic reward module if necessary.
+
+
+**Args**
+
+* **samples**  : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+
+
+**Returns**
+
+None
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/reward/icm.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/icm.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-#
-
-
-## ICM
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/icm.py\#L123)
-```python 
-ICM(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
-   latent_dim: int = 128, lr: float = 0.001, batch_size: int = 64
-)
-```
-
-
----
-Curiosity-Driven Exploration by Self-Supervised Prediction.
-See paper: http://proceedings.mlr.press/v70/pathak17a/pathak17a.pdf
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
-* **kappa** (float) : The decay rate.
-* **latent_dim** (int) : The dimension of encoding vectors.
-* **lr** (float) : The learning rate.
-* **batch_size** (int) : The batch size for update.
-
-
-**Returns**
-
-Instance of RND.
-
-
-**Methods:**
-
-
-### .compute_irs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/icm.py\#L176)
-```python
-.compute_irs(
-   samples: Dict, step: int = 0
-)
-```
-
----
-Compute the intrinsic rewards for current samples.
-
-
-**Args**
-
-* **samples** (Dict) : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-* **step** (int) : The global training step.
-
-
-**Returns**
-
-The intrinsic rewards.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/icm.py\#L214)
-```python
-.update(
-   samples: Dict
-)
-```
-
----
-Update the intrinsic reward module if necessary.
-
-
-**Args**
-
-* **samples**  : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-
-
-**Returns**
-
-None
+#
+
+
+## ICM
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/icm.py/#L123)
+```python 
+ICM(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
+   latent_dim: int = 128, lr: float = 0.001, batch_size: int = 64
+)
+```
+
+
+---
+Curiosity-Driven Exploration by Self-Supervised Prediction.
+See paper: http://proceedings.mlr.press/v70/pathak17a/pathak17a.pdf
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
+* **kappa** (float) : The decay rate.
+* **latent_dim** (int) : The dimension of encoding vectors.
+* **lr** (float) : The learning rate.
+* **batch_size** (int) : The batch size for update.
+
+
+**Returns**
+
+Instance of ICM.
+
+
+**Methods:**
+
+
+### .compute_irs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/icm.py/#L176)
+```python
+.compute_irs(
+   samples: Dict, step: int = 0
+)
+```
+
+---
+Compute the intrinsic rewards for current samples.
+
+
+**Args**
+
+* **samples** (Dict) : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+* **step** (int) : The global training step.
+
+
+**Returns**
+
+The intrinsic rewards.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/icm.py/#L214)
+```python
+.update(
+   samples: Dict
+)
+```
+
+---
+Update the intrinsic reward module if necessary.
+
+
+**Args**
+
+* **samples**  : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+
+
+**Returns**
+
+None
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/reward/ngu.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/ngu.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-#
-
-
-## NGU
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/ngu.py\#L81)
-```python 
-NGU(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
-   latent_dim: int = 128, lr: float = 0.001, batch_size: int = 64, capacity: int = 1000,
-   k: int = 10, kernel_cluster_distance: float = 0.008, kernel_epsilon: float = 0.0001,
-   c: float = 0.001, sm: float = 8.0, mrs: float = 5.0
-)
-```
-
-
----
-Never Give Up: Learning Directed Exploration Strategies (NGU).
-See paper: https://arxiv.org/pdf/2002.06038
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
-* **kappa** (float) : The decay rate.
-* **latent_dim** (int) : The dimension of encoding vectors.
-* **lr** (float) : The learning rate.
-* **batch_size** (int) : The batch size for update.
-* **capacity** (int) : The of capacity the episodic memory.
-* **k** (int) : Number of neighbors.
-* **kernel_cluster_distance** (float) : The kernel cluster distance.
-* **kernel_epsilon** (float) : The kernel constant.
-* **c** (float) : The pseudo-counts constant.
-* **sm** (float) : The kernel maximum similarity.
-* **mrs** (float) : The maximum reward scaling.
-
-
-**Returns**
-
-Instance of the base intrinsic reward module.
-
-
-**Methods:**
-
-
-### .pseudo_counts
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/ngu.py\#L171)
-```python
-.pseudo_counts(
-   e: th.Tensor
-)
-```
-
----
-Pseudo counts.
-
-
-**Args**
-
-* **e** (Tensor) : Encoded observations.
-
-
-**Returns**
-
-Conut values.
-
-### .compute_irs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/ngu.py\#L198)
-```python
-.compute_irs(
-   samples: Dict, step: int = 0
-)
-```
-
----
-Compute the intrinsic rewards for current samples.
-
-
-**Args**
-
-* **samples** (Dict) : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-* **step** (int) : The global training step.
-
-
-**Returns**
-
-The intrinsic rewards.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/ngu.py\#L244)
-```python
-.update(
-   samples: Dict
-)
-```
-
----
-Update the intrinsic reward module if necessary.
-
-
-**Args**
-
-* **samples**  : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-
-
-**Returns**
-
-None
+#
+
+
+## NGU
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/ngu.py/#L81)
+```python 
+NGU(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
+   latent_dim: int = 128, lr: float = 0.001, batch_size: int = 64, capacity: int = 1000,
+   k: int = 10, kernel_cluster_distance: float = 0.008, kernel_epsilon: float = 0.0001,
+   c: float = 0.001, sm: float = 8.0, mrs: float = 5.0
+)
+```
+
+
+---
+Never Give Up: Learning Directed Exploration Strategies (NGU).
+See paper: https://arxiv.org/pdf/2002.06038
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
+* **kappa** (float) : The decay rate.
+* **latent_dim** (int) : The dimension of encoding vectors.
+* **lr** (float) : The learning rate.
+* **batch_size** (int) : The batch size for update.
+* **capacity** (int) : The of capacity the episodic memory.
+* **k** (int) : Number of neighbors.
+* **kernel_cluster_distance** (float) : The kernel cluster distance.
+* **kernel_epsilon** (float) : The kernel constant.
+* **c** (float) : The pseudo-counts constant.
+* **sm** (float) : The kernel maximum similarity.
+* **mrs** (float) : The maximum reward scaling.
+
+
+**Returns**
+
+Instance of NGU.
+
+
+**Methods:**
+
+
+### .pseudo_counts
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/ngu.py/#L171)
+```python
+.pseudo_counts(
+   e: th.Tensor
+)
+```
+
+---
+Pseudo counts.
+
+
+**Args**
+
+* **e** (Tensor) : Encoded observations.
+
+
+**Returns**
+
+Conut values.
+
+### .compute_irs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/ngu.py/#L198)
+```python
+.compute_irs(
+   samples: Dict, step: int = 0
+)
+```
+
+---
+Compute the intrinsic rewards for current samples.
+
+
+**Args**
+
+* **samples** (Dict) : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+* **step** (int) : The global training step.
+
+
+**Returns**
+
+The intrinsic rewards.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/ngu.py/#L244)
+```python
+.update(
+   samples: Dict
+)
+```
+
+---
+Update the intrinsic reward module if necessary.
+
+
+**Args**
+
+* **samples**  : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+
+
+**Returns**
+
+None
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/reward/pseudo_counts.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/ride.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-#
-
-
-## PseudoCounts
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/pseudo_counts.py\#L81)
-```python 
-PseudoCounts(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
-   latent_dim: int = 32, lr: float = 0.001, batch_size: int = 64, capacity: int = 1000,
-   k: int = 10, kernel_cluster_distance: float = 0.008, kernel_epsilon: float = 0.0001,
-   c: float = 0.001, sm: float = 8.0
-)
-```
-
-
----
-Pseudo-counts based on "Never Give Up: Learning Directed Exploration Strategies (NGU)".
-See paper: https://arxiv.org/pdf/2002.06038
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
-* **kappa** (float) : The decay rate.
-* **latent_dim** (int) : The dimension of encoding vectors.
-* **lr** (float) : The learning rate.
-* **batch_size** (int) : The batch size for update.
-* **capacity** (int) : The of capacity the episodic memory.
-* **k** (int) : Number of neighbors.
-* **kernel_cluster_distance** (float) : The kernel cluster distance.
-* **kernel_epsilon** (float) : The kernel constant.
-* **c** (float) : The pseudo-counts constant.
-* **sm** (float) : The kernel maximum similarity.
-
-
-**Returns**
-
-Instance of the base intrinsic reward module.
-
-
-**Methods:**
-
-
-### .pseudo_counts
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/pseudo_counts.py\#L147)
-```python
-.pseudo_counts(
-   e: th.Tensor
-)
-```
-
----
-Pseudo counts.
-
-
-**Args**
-
-* **e** (Tensor) : Encoded observations.
-
-
-**Returns**
-
-Conut values.
-
-### .compute_irs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/pseudo_counts.py\#L174)
-```python
-.compute_irs(
-   samples: Dict, step: int = 0
-)
-```
-
----
-Compute the intrinsic rewards for current samples.
-
-
-**Args**
-
-* **samples** (Dict) : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-* **step** (int) : The global training step.
-
-
-**Returns**
-
-The intrinsic rewards.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/pseudo_counts.py\#L211)
-```python
-.update(
-   samples: Dict
-)
-```
-
----
-Update the intrinsic reward module if necessary.
-
-
-**Args**
-
-* **samples**  : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-
-
-**Returns**
-
-None
+#
+
+
+## RIDE
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/ride.py/#L124)
+```python 
+RIDE(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
+   latent_dim: int = 128, lr: float = 0.001, batch_size: int = 64, capacity: int = 1000,
+   k: int = 10, kernel_cluster_distance: float = 0.008, kernel_epsilon: float = 0.0001,
+   c: float = 0.001, sm: float = 8.0
+)
+```
+
+
+---
+RIDE: Rewarding Impact-Driven Exploration for Procedurally-Generated Environments.
+See paper: https://arxiv.org/pdf/2002.12292
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
+* **kappa** (float) : The decay rate.
+* **latent_dim** (int) : The dimension of encoding vectors.
+* **lr** (float) : The learning rate.
+* **batch_size** (int) : The batch size for update.
+* **capacity** (int) : The of capacity the episodic memory.
+* **k** (int) : Number of neighbors.
+* **kernel_cluster_distance** (float) : The kernel cluster distance.
+* **kernel_epsilon** (float) : The kernel constant.
+* **c** (float) : The pseudo-counts constant.
+* **sm** (float) : The kernel maximum similarity.
+
+
+**Returns**
+
+Instance of RIDE.
+
+
+**Methods:**
+
+
+### .pseudo_counts
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/ride.py/#L197)
+```python
+.pseudo_counts(
+   e: th.Tensor
+)
+```
+
+---
+Pseudo counts.
+
+
+**Args**
+
+* **e** (Tensor) : Encoded observations.
+
+
+**Returns**
+
+Conut values.
+
+### .compute_irs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/ride.py/#L224)
+```python
+.compute_irs(
+   samples: Dict, step: int = 0
+)
+```
+
+---
+Compute the intrinsic rewards for current samples.
+
+
+**Args**
+
+* **samples** (Dict) : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+* **step** (int) : The global training step.
+
+
+**Returns**
+
+The intrinsic rewards.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/ride.py/#L267)
+```python
+.update(
+   samples: Dict
+)
+```
+
+---
+Update the intrinsic reward module if necessary.
+
+
+**Args**
+
+* **samples**  : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+
+
+**Returns**
+
+None
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/reward/re3.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/rnd.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-#
-
-
-## RE3
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/re3.py\#L59)
-```python 
-RE3(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
-   latent_dim: int = 128, k: int = 5, average_entropy: bool = False
-)
-```
-
-
----
-State Entropy Maximization with Random Encoders for Efficient Exploration (RE3).
-See paper: http://proceedings.mlr.press/v139/seo21a/seo21a.pdf
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
-* **kappa** (float) : The decay rate.
-* **latent_dim** (int) : The dimension of encoding vectors.
-* **k** (int) : Use the k-th neighbors.
-* **average_entropy** (bool) : Use the average of entropy estimation.
-
-
-**Returns**
-
-Instance of RND.
-
-
-**Methods:**
-
-
-### .compute_irs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/re3.py\#L106)
-```python
-.compute_irs(
-   samples: Dict, step: int = 0
-)
-```
-
----
-Compute the intrinsic rewards for current samples.
-
-
-**Args**
-
-* **samples** (Dict) : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-* **step** (int) : The global training step.
-
-
-**Returns**
-
-The intrinsic rewards.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/re3.py\#L141)
-```python
-.update(
-   samples: Dict
-)
-```
-
----
-Update the intrinsic reward module if necessary.
-
-
-**Args**
-
-* **samples**  : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-
-
-**Returns**
-
-None
+#
+
+
+## RND
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/rnd.py/#L61)
+```python 
+RND(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
+   latent_dim: int = 128, lr: float = 0.001, batch_size: int = 64
+)
+```
+
+
+---
+Exploration by Random Network Distillation (RND).
+See paper: https://arxiv.org/pdf/1810.12894.pdf
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
+* **kappa** (float) : The decay rate.
+* **latent_dim** (int) : The dimension of encoding vectors.
+* **lr** (float) : The learning rate.
+* **batch_size** (int) : The batch size for update.
+
+
+**Returns**
+
+Instance of RND.
+
+
+**Methods:**
+
+
+### .compute_irs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/rnd.py/#L114)
+```python
+.compute_irs(
+   samples: Dict, step: int = 0
+)
+```
+
+---
+Compute the intrinsic rewards for current samples.
+
+
+**Args**
+
+* **samples** (Dict) : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+* **step** (int) : The global training step.
+
+
+**Returns**
+
+The intrinsic rewards.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/rnd.py/#L149)
+```python
+.update(
+   samples: Dict
+)
+```
+
+---
+Update the intrinsic reward module if necessary.
+
+
+**Args**
+
+* **samples**  : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+
+
+**Returns**
+
+None
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/reward/revd.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/revd.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-#
-
-
-## REVD
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/revd.py\#L59)
-```python 
-REVD(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
-   latent_dim: int = 128, alpha: float = 0.5, k: int = 5, average_divergence: bool = False
-)
-```
-
-
----
-Rewarding Episodic Visitation Discrepancy for Exploration in Reinforcement Learning (REVD).
-See paper: https://openreview.net/pdf?id=V2pw1VYMrDo
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
-* **kappa** (float) : The decay rate.
-* **latent_dim** (int) : The dimension of encoding vectors.
-* **alpha** (alpha) : The order of Rényi divergence.
-* **k** (int) : Use the k-th neighbors.
-* **average_divergence** (bool) : Use the average of divergence estimation.
-
-
-**Returns**
-
-Instance of REVD.
-
-
-**Methods:**
-
-
-### .compute_irs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/revd.py\#L112)
-```python
-.compute_irs(
-   samples: Dict, step: int = 0
-)
-```
-
----
-Compute the intrinsic rewards for current samples.
-
-
-**Args**
-
-* **samples** (Dict) : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-* **step** (int) : The global training step.
-
-
-**Returns**
-
-The intrinsic rewards.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/revd.py\#L167)
-```python
-.update(
-   samples: Dict
-)
-```
-
----
-Update the intrinsic reward module if necessary.
-
-
-**Args**
-
-* **samples**  : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-
-
-**Returns**
-
-None
+#
+
+
+## REVD
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/revd.py/#L59)
+```python 
+REVD(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
+   latent_dim: int = 128, alpha: float = 0.5, k: int = 5, average_divergence: bool = False
+)
+```
+
+
+---
+Rewarding Episodic Visitation Discrepancy for Exploration in Reinforcement Learning (REVD).
+See paper: https://openreview.net/pdf?id=V2pw1VYMrDo
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
+* **kappa** (float) : The decay rate.
+* **latent_dim** (int) : The dimension of encoding vectors.
+* **alpha** (alpha) : The order of Rényi divergence.
+* **k** (int) : Use the k-th neighbors.
+* **average_divergence** (bool) : Use the average of divergence estimation.
+
+
+**Returns**
+
+Instance of REVD.
+
+
+**Methods:**
+
+
+### .compute_irs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/revd.py/#L112)
+```python
+.compute_irs(
+   samples: Dict, step: int = 0
+)
+```
+
+---
+Compute the intrinsic rewards for current samples.
+
+
+**Args**
+
+* **samples** (Dict) : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+* **step** (int) : The global training step.
+
+
+**Returns**
+
+The intrinsic rewards.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/revd.py/#L167)
+```python
+.update(
+   samples: Dict
+)
+```
+
+---
+Update the intrinsic reward module if necessary.
+
+
+**Args**
+
+* **samples**  : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+
+
+**Returns**
+
+None
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/reward/rise.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/rise.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-#
-
-
-## RISE
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/rise.py\#L59)
-```python 
-RISE(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
-   latent_dim: int = 128, alpha: float = 0.5, k: int = 5, average_entropy: bool = False
-)
-```
-
-
----
-Rényi State Entropy Maximization for Exploration Acceleration in Reinforcement Learning (RISE).
-See paper: https://ieeexplore.ieee.org/abstract/document/9802917/
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
-* **kappa** (float) : The decay rate.
-* **latent_dim** (int) : The dimension of encoding vectors.
-* **alpha** (alpha) : The The order of Rényi entropy.
-* **k** (int) : Use the k-th neighbors.
-* **average_entropy** (bool) : Use the average of entropy estimation.
-
-
-**Returns**
-
-Instance of RND.
-
-
-**Methods:**
-
-
-### .compute_irs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/rise.py\#L109)
-```python
-.compute_irs(
-   samples: Dict, step: int = 0
-)
-```
-
----
-Compute the intrinsic rewards for current samples.
-
-
-**Args**
-
-* **samples** (Dict) : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-* **step** (int) : The global training step.
-
-
-**Returns**
-
-The intrinsic rewards.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/rise.py\#L145)
-```python
-.update(
-   samples: Dict
-)
-```
-
----
-Update the intrinsic reward module if necessary.
-
-
-**Args**
-
-* **samples**  : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-
-
-**Returns**
-
-None
+#
+
+
+## RISE
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/rise.py/#L59)
+```python 
+RISE(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
+   latent_dim: int = 128, alpha: float = 0.5, k: int = 5, average_entropy: bool = False
+)
+```
+
+
+---
+Rényi State Entropy Maximization for Exploration Acceleration in Reinforcement Learning (RISE).
+See paper: https://ieeexplore.ieee.org/abstract/document/9802917/
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
+* **kappa** (float) : The decay rate.
+* **latent_dim** (int) : The dimension of encoding vectors.
+* **alpha** (alpha) : The The order of Rényi entropy.
+* **k** (int) : Use the k-th neighbors.
+* **average_entropy** (bool) : Use the average of entropy estimation.
+
+
+**Returns**
+
+Instance of RISE.
+
+
+**Methods:**
+
+
+### .compute_irs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/rise.py/#L109)
+```python
+.compute_irs(
+   samples: Dict, step: int = 0
+)
+```
+
+---
+Compute the intrinsic rewards for current samples.
+
+
+**Args**
+
+* **samples** (Dict) : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+* **step** (int) : The global training step.
+
+
+**Returns**
+
+The intrinsic rewards.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/rise.py/#L145)
+```python
+.update(
+   samples: Dict
+)
+```
+
+---
+Update the intrinsic reward module if necessary.
+
+
+**Args**
+
+* **samples**  : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+
+
+**Returns**
+
+None
```

### Comparing `hsuanwu-0.0.1b4/docs/api/xplore/reward/rnd.md` & `hsuanwu-0.0.1b5/docs/api_docs/xplore/reward/re3.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-#
-
-
-## RND
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/rnd.py\#L61)
-```python 
-RND(
-   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
-   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
-   latent_dim: int = 128, lr: float = 0.001, batch_size: int = 64
-)
-```
-
-
----
-Exploration by Random Network Distillation (RND).
-See paper: https://arxiv.org/pdf/1810.12894.pdf
-
-
-**Args**
-
-* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
-    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
-    'action_space' is a 'DictConfig' like
-    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
-* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
-* **kappa** (float) : The decay rate.
-* **latent_dim** (int) : The dimension of encoding vectors.
-* **lr** (float) : The learning rate.
-* **batch_size** (int) : The batch size for update.
-
-
-**Returns**
-
-Instance of RND.
-
-
-**Methods:**
-
-
-### .compute_irs
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/rnd.py\#L114)
-```python
-.compute_irs(
-   samples: Dict, step: int = 0
-)
-```
-
----
-Compute the intrinsic rewards for current samples.
-
-
-**Args**
-
-* **samples** (Dict) : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-* **step** (int) : The global training step.
-
-
-**Returns**
-
-The intrinsic rewards.
-
-### .update
-[source](https://github.com/RLE-Foundation/Hsuanwu\blob\main\hsuanwu/xplore/reward/rnd.py\#L149)
-```python
-.update(
-   samples: Dict
-)
-```
-
----
-Update the intrinsic reward module if necessary.
-
-
-**Args**
-
-* **samples**  : The collected samples. A python dict like
-    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
-    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
-    rewards (n_steps, n_envs) <class 'th.Tensor'>,
-    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
-
-
-**Returns**
-
-None
+#
+
+
+## RE3
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/re3.py/#L59)
+```python 
+RE3(
+   observation_space: Union[gym.Space, DictConfig], action_space: Union[gym.Space,
+   DictConfig], device: str = 'cpu', beta: float = 0.05, kappa: float = 2.5e-05,
+   latent_dim: int = 128, k: int = 5, average_entropy: bool = False
+)
+```
+
+
+---
+State Entropy Maximization with Random Encoders for Efficient Exploration (RE3).
+See paper: http://proceedings.mlr.press/v139/seo21a/seo21a.pdf
+
+
+**Args**
+
+* **observation_space** (Space or DictConfig) : The observation space of environment. When invoked by Hydra,
+    'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+* **action_space** (Space or DictConfig) : The action space of environment. When invoked by Hydra,
+    'action_space' is a 'DictConfig' like
+    {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+    {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+* **device** (str) : Device (cpu, cuda, ...) on which the code should be run.
+* **beta** (float) : The initial weighting coefficient of the intrinsic rewards.
+* **kappa** (float) : The decay rate.
+* **latent_dim** (int) : The dimension of encoding vectors.
+* **k** (int) : Use the k-th neighbors.
+* **average_entropy** (bool) : Use the average of entropy estimation.
+
+
+**Returns**
+
+Instance of RE3.
+
+
+**Methods:**
+
+
+### .compute_irs
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/re3.py/#L106)
+```python
+.compute_irs(
+   samples: Dict, step: int = 0
+)
+```
+
+---
+Compute the intrinsic rewards for current samples.
+
+
+**Args**
+
+* **samples** (Dict) : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+* **step** (int) : The global training step.
+
+
+**Returns**
+
+The intrinsic rewards.
+
+### .update
+[source](https://github.com/RLE-Foundation/Hsuanwu/blob/main/hsuanwu/xplore/reward/re3.py/#L141)
+```python
+.update(
+   samples: Dict
+)
+```
+
+---
+Update the intrinsic reward module if necessary.
+
+
+**Args**
+
+* **samples**  : The collected samples. A python dict like
+    {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+    actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+    rewards (n_steps, n_envs) <class 'th.Tensor'>,
+    next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+
+
+**Returns**
+
+None
```

### Comparing `hsuanwu-0.0.1b4/docs/assets/images/github_issues.png` & `hsuanwu-0.0.1b5/docs/assets/images/github_issues.png`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/assets/images/icon.svg` & `hsuanwu-0.0.1b5/docs/assets/images/icon.svg`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/assets/images/logo.png` & `hsuanwu-0.0.1b5/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/assets/images/qq.jpg` & `hsuanwu-0.0.1b5/docs/assets/images/qq.jpg`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/assets/images/roadmap.svg` & `hsuanwu-0.0.1b5/docs/assets/images/roadmap.svg`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/assets/images/slack.png` & `hsuanwu-0.0.1b5/docs/assets/images/slack.png`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/docs/assets/images/structure.svg` & `hsuanwu-0.0.1b5/docs/assets/images/structure.svg`

 * *Files 20% similar despite different names*

```diff
@@ -1,1095 +1,1095 @@
-00000000: 3c73 7667 2068 6569 6768 743d 2235 3733  <svg height="573
-00000010: 2220 786d 6c6e 733a 6576 3d22 6874 7470  " xmlns:ev="http
-00000020: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-00000030: 3031 2f78 6d6c 2d65 7665 6e74 7322 2076  01/xml-events" v
-00000040: 6965 7742 6f78 3d22 3020 3020 3933 3720  iewBox="0 0 937 
-00000050: 3537 3322 2078 6d6c 6e73 3a78 6c69 6e6b  573" xmlns:xlink
-00000060: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-00000070: 6f72 672f 3139 3939 2f78 6c69 6e6b 2220  org/1999/xlink" 
-00000080: 7769 6474 683d 2239 3337 2220 786d 6c6e  width="937" xmln
-00000090: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
-000000a0: 2e6f 7267 2f32 3030 302f 7376 6722 3e3c  .org/2000/svg"><
-000000b0: 6465 6673 2f3e 3c67 2074 7261 6e73 666f  defs/><g transfo
-000000c0: 726d 3d22 7472 616e 736c 6174 6528 352e  rm="translate(5.
-000000d0: 352c 352e 3529 2220 6964 3d22 7061 6765  5,5.5)" id="page
-000000e0: 3122 3e3c 7265 6374 2078 3d22 3022 2068  1"><rect x="0" h
-000000f0: 6569 6768 743d 2235 3633 2220 793d 2230  eight="563" y="0
-00000100: 2220 7769 6474 683d 2239 3237 2220 6669  " width="927" fi
-00000110: 6c6c 3d22 6e6f 6e65 222f 3e3c 7061 7468  ll="none"/><path
-00000120: 2073 7472 6f6b 652d 6c69 6e65 6361 703d   stroke-linecap=
-00000130: 2272 6f75 6e64 2220 7472 616e 7366 6f72  "round" transfor
-00000140: 6d3d 2274 7261 6e73 6c61 7465 2835 3333  m="translate(533
-00000150: 2e36 392c 3238 372e 3530 2922 2069 643d  .69,287.50)" id=
-00000160: 2273 6861 7065 3122 2073 7472 6f6b 653d  "shape1" stroke=
-00000170: 2223 3435 3435 3435 2220 7374 726f 6b65  "#454545" stroke
-00000180: 2d77 6964 7468 3d22 3422 2066 696c 6c3d  -width="4" fill=
-00000190: 226e 6f6e 6522 2064 3d22 4d31 332e 312c  "none" d="M13.1,
-000001a0: 2e30 4c33 362e 372c 2e30 4333 382e 342c  .0L36.7,.0C38.4,
-000001b0: 2e30 2c34 302e 372c 2e30 2c34 322e 372c  .0,40.7,.0,42.7,
-000001c0: 2e30 4334 332e 362c 2e30 2c34 342e 362c  .0C43.6,.0,44.6,
-000001d0: 2e30 2c34 352e 372c 2e30 4c37 362e 312c  .0,45.7,.0L76.1,
-000001e0: 2e30 222f 3e3c 7061 7468 2073 7472 6f6b  .0"/><path strok
-000001f0: 652d 6c69 6e65 6361 703d 2272 6f75 6e64  e-linecap="round
-00000200: 2220 7472 616e 7366 6f72 6d3d 2274 7261  " transform="tra
-00000210: 6e73 6c61 7465 2835 3333 2e36 392c 3231  nslate(533.69,21
-00000220: 332e 3933 2922 2069 643d 2273 6861 7065  3.93)" id="shape
-00000230: 3222 2073 7472 6f6b 653d 2223 3435 3435  2" stroke="#4545
-00000240: 3435 2220 7374 726f 6b65 2d77 6964 7468  45" stroke-width
-00000250: 3d22 3422 2066 696c 6c3d 226e 6f6e 6522  ="4" fill="none"
-00000260: 2064 3d22 4d31 332e 312c 3733 2e36 4c33   d="M13.1,73.6L3
-00000270: 362e 372c 3733 2e36 4333 382e 342c 3733  6.7,73.6C38.4,73
-00000280: 2e36 2c33 392e 372c 3732 2e32 2c33 392e  .6,39.7,72.2,39.
-00000290: 372c 3730 2e36 4c33 392e 372c 2d36 342e  7,70.6L39.7,-64.
-000002a0: 3643 3339 2e37 2c2d 3636 2e32 2c33 392e  6C39.7,-66.2,39.
-000002b0: 352c 2d36 382e 372c 3430 2e34 2c2d 3730  5,-68.7,40.4,-70
-000002c0: 2e35 4334 312e 352c 2d37 322e 332c 3433  .5C41.5,-72.3,43
-000002d0: 2e34 2c2d 3733 2e36 2c34 352e 372c 2d37  .4,-73.6,45.7,-7
-000002e0: 332e 364c 3736 2e31 2c2d 3733 2e36 222f  3.6L76.1,-73.6"/
-000002f0: 3e3c 7061 7468 2073 7472 6f6b 652d 6c69  ><path stroke-li
-00000300: 6e65 6361 703d 2272 6f75 6e64 2220 7472  necap="round" tr
-00000310: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-00000320: 7465 2835 3333 2e36 392c 3336 312e 3038  te(533.69,361.08
-00000330: 2922 2069 643d 2273 6861 7065 3322 2073  )" id="shape3" s
-00000340: 7472 6f6b 653d 2223 3435 3435 3435 2220  troke="#454545" 
-00000350: 7374 726f 6b65 2d77 6964 7468 3d22 3422  stroke-width="4"
-00000360: 2066 696c 6c3d 226e 6f6e 6522 2064 3d22   fill="none" d="
-00000370: 4d31 332e 312c 2d37 332e 364c 3336 2e37  M13.1,-73.6L36.7
-00000380: 2c2d 3733 2e36 4333 382e 342c 2d37 332e  ,-73.6C38.4,-73.
-00000390: 362c 3339 2e37 2c2d 3732 2e32 2c33 392e  6,39.7,-72.2,39.
-000003a0: 372c 2d37 302e 364c 3339 2e37 2c36 342e  7,-70.6L39.7,64.
-000003b0: 3643 3339 2e37 2c36 362e 322c 3339 2e35  6C39.7,66.2,39.5
-000003c0: 2c36 382e 372c 3430 2e34 2c37 302e 3543  ,68.7,40.4,70.5C
-000003d0: 3431 2e35 2c37 322e 332c 3433 2e34 2c37  41.5,72.3,43.4,7
-000003e0: 332e 362c 3435 2e37 2c37 332e 364c 3736  3.6,45.7,73.6L76
-000003f0: 2e31 2c37 332e 3622 2f3e 3c70 6174 6820  .1,73.6"/><path 
-00000400: 7374 726f 6b65 2d6c 696e 6563 6170 3d22  stroke-linecap="
-00000410: 726f 756e 6422 2074 7261 6e73 666f 726d  round" transform
-00000420: 3d22 7472 616e 736c 6174 6528 3732 352e  ="translate(725.
-00000430: 3330 2c32 3637 2e30 3229 2220 6964 3d22  30,267.02)" id="
-00000440: 7368 6170 6534 2220 7374 726f 6b65 3d22  shape4" stroke="
-00000450: 2334 3534 3534 3522 2073 7472 6f6b 652d  #454545" stroke-
-00000460: 7769 6474 683d 2234 2220 6669 6c6c 3d22  width="4" fill="
-00000470: 6e6f 6e65 2220 643d 224d 2d31 322e 352c  none" d="M-12.5,
-00000480: 3230 2e35 4c2d 302e 332c 3230 2e35 4331  20.5L-0.3,20.5C1
-00000490: 2e34 2c32 302e 352c 322e 372c 3139 2e31  .4,20.5,2.7,19.1
-000004a0: 2c32 2e37 2c31 372e 354c 322e 372c 2d31  ,2.7,17.5L2.7,-1
-000004b0: 312e 3543 322e 372c 2d31 332e 312c 322e  1.5C2.7,-13.1,2.
-000004c0: 352c 2d31 352e 362c 332e 342c 2d31 372e  5,-15.6,3.4,-17.
-000004d0: 3443 342e 352c 2d31 392e 322c 362e 342c  4C4.5,-19.2,6.4,
-000004e0: 2d32 302e 352c 382e 372c 2d32 302e 354c  -20.5,8.7,-20.5L
-000004f0: 3132 2e35 2c2d 3230 2e35 222f 3e3c 7061  12.5,-20.5"/><pa
-00000500: 7468 2073 7472 6f6b 652d 6c69 6e65 6361  th stroke-lineca
-00000510: 703d 2272 6f75 6e64 2220 7472 616e 7366  p="round" transf
-00000520: 6f72 6d3d 2274 7261 6e73 6c61 7465 2837  orm="translate(7
-00000530: 3235 2e33 302c 3238 372e 3530 2922 2069  25.30,287.50)" i
-00000540: 643d 2273 6861 7065 3522 2073 7472 6f6b  d="shape5" strok
-00000550: 653d 2223 3435 3435 3435 2220 7374 726f  e="#454545" stro
-00000560: 6b65 2d77 6964 7468 3d22 3422 2066 696c  ke-width="4" fil
-00000570: 6c3d 226e 6f6e 6522 2064 3d22 4d2d 3132  l="none" d="M-12
-00000580: 2e35 2c2e 304c 2d30 2e33 2c2e 3043 312e  .5,.0L-0.3,.0C1.
-00000590: 342c 2e30 2c33 2e37 2c2e 302c 352e 372c  4,.0,3.7,.0,5.7,
-000005a0: 2e30 4336 2e36 2c2e 302c 372e 362c 2e30  .0C6.6,.0,7.6,.0
-000005b0: 2c38 2e37 2c2e 304c 3132 2e35 2c2e 3022  ,8.7,.0L12.5,.0"
-000005c0: 2f3e 3c70 6174 6820 7374 726f 6b65 2d6c  /><path stroke-l
-000005d0: 696e 6563 6170 3d22 726f 756e 6422 2074  inecap="round" t
-000005e0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-000005f0: 6174 6528 3732 352e 3330 2c33 3037 2e39  ate(725.30,307.9
-00000600: 3829 2220 6964 3d22 7368 6170 6536 2220  8)" id="shape6" 
-00000610: 7374 726f 6b65 3d22 2334 3534 3534 3522  stroke="#454545"
-00000620: 2073 7472 6f6b 652d 7769 6474 683d 2234   stroke-width="4
-00000630: 2220 6669 6c6c 3d22 6e6f 6e65 2220 643d  " fill="none" d=
-00000640: 224d 2d31 322e 352c 2d32 302e 354c 2d30  "M-12.5,-20.5L-0
-00000650: 2e33 2c2d 3230 2e35 4331 2e34 2c2d 3230  .3,-20.5C1.4,-20
-00000660: 2e35 2c32 2e37 2c2d 3139 2e31 2c32 2e37  .5,2.7,-19.1,2.7
-00000670: 2c2d 3137 2e35 4c32 2e37 2c31 312e 3543  ,-17.5L2.7,11.5C
-00000680: 322e 372c 3133 2e31 2c32 2e35 2c31 352e  2.7,13.1,2.5,15.
-00000690: 362c 332e 342c 3137 2e34 4334 2e35 2c31  6,3.4,17.4C4.5,1
-000006a0: 392e 322c 362e 342c 3230 2e35 2c38 2e37  9.2,6.4,20.5,8.7
-000006b0: 2c32 302e 354c 3132 2e35 2c32 302e 3522  ,20.5L12.5,20.5"
-000006c0: 2f3e 3c70 6174 6820 7374 726f 6b65 2d6c  /><path stroke-l
-000006d0: 696e 6563 6170 3d22 726f 756e 6422 2074  inecap="round" t
-000006e0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-000006f0: 6174 6528 3338 312e 3437 2c33 3834 2e37  ate(381.47,384.7
-00000700: 3729 2220 6964 3d22 7368 6170 6537 2220  7)" id="shape7" 
-00000710: 7374 726f 6b65 3d22 2334 3534 3534 3522  stroke="#454545"
-00000720: 2073 7472 6f6b 652d 7769 6474 683d 2234   stroke-width="4
-00000730: 2220 6669 6c6c 3d22 6e6f 6e65 2220 643d  " fill="none" d=
-00000740: 224d 2d31 332e 312c 2d39 372e 334c 2d33  "M-13.1,-97.3L-3
-00000750: 362e 372c 2d39 372e 3343 2d33 382e 342c  6.7,-97.3C-38.4,
-00000760: 2d39 372e 332c 2d33 392e 372c 2d39 352e  -97.3,-39.7,-95.
-00000770: 392c 2d33 392e 372c 2d39 342e 334c 2d33  9,-39.7,-94.3L-3
-00000780: 392e 372c 3838 2e33 432d 3339 2e37 2c38  9.7,88.3C-39.7,8
-00000790: 392e 392c 2d33 392e 352c 3932 2e34 2c2d  9.9,-39.5,92.4,-
-000007a0: 3430 2e34 2c39 342e 3143 2d34 312e 352c  40.4,94.1C-41.5,
-000007b0: 3936 2e30 2c2d 3433 2e34 2c39 372e 332c  96.0,-43.4,97.3,
-000007c0: 2d34 352e 372c 3937 2e33 4c2d 3736 2e31  -45.7,97.3L-76.1
-000007d0: 2c39 372e 3322 2f3e 3c70 6174 6820 7374  ,97.3"/><path st
-000007e0: 726f 6b65 2d6c 696e 6563 6170 3d22 726f  roke-linecap="ro
-000007f0: 756e 6422 2074 7261 6e73 666f 726d 3d22  und" transform="
-00000800: 7472 616e 736c 6174 6528 3338 312e 3437  translate(381.47
-00000810: 2c32 3435 2e35 3929 2220 6964 3d22 7368  ,245.59)" id="sh
-00000820: 6170 6538 2220 7374 726f 6b65 3d22 2334  ape8" stroke="#4
-00000830: 3534 3534 3522 2073 7472 6f6b 652d 7769  54545" stroke-wi
-00000840: 6474 683d 2234 2220 6669 6c6c 3d22 6e6f  dth="4" fill="no
-00000850: 6e65 2220 643d 224d 2d31 332e 312c 3431  ne" d="M-13.1,41
-00000860: 2e39 4c2d 3336 2e37 2c34 312e 3943 2d33  .9L-36.7,41.9C-3
-00000870: 382e 342c 3431 2e39 2c2d 3339 2e37 2c34  8.4,41.9,-39.7,4
-00000880: 302e 362c 2d33 392e 372c 3338 2e39 4c2d  0.6,-39.7,38.9L-
-00000890: 3339 2e37 2c2d 3332 2e39 432d 3339 2e37  39.7,-32.9C-39.7
-000008a0: 2c2d 3334 2e36 2c2d 3339 2e35 2c2d 3337  ,-34.6,-39.5,-37
-000008b0: 2e30 2c2d 3430 2e34 2c2d 3338 2e38 432d  .0,-40.4,-38.8C-
-000008c0: 3431 2e35 2c2d 3430 2e36 2c2d 3433 2e34  41.5,-40.6,-43.4
-000008d0: 2c2d 3431 2e39 2c2d 3435 2e37 2c2d 3431  ,-41.9,-45.7,-41
-000008e0: 2e39 4c2d 3736 2e31 2c2d 3431 2e39 222f  .9L-76.1,-41.9"/
-000008f0: 3e3c 7061 7468 2073 7472 6f6b 652d 6c69  ><path stroke-li
-00000900: 6e65 6361 703d 2272 6f75 6e64 2220 7472  necap="round" tr
-00000910: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-00000920: 7465 2833 3831 2e34 372c 3331 312e 3139  te(381.47,311.19
-00000930: 2922 2069 643d 2273 6861 7065 3922 2073  )" id="shape9" s
-00000940: 7472 6f6b 653d 2223 3435 3435 3435 2220  troke="#454545" 
-00000950: 7374 726f 6b65 2d77 6964 7468 3d22 3422  stroke-width="4"
-00000960: 2066 696c 6c3d 226e 6f6e 6522 2064 3d22   fill="none" d="
-00000970: 4d2d 3133 2e31 2c2d 3233 2e37 4c2d 3336  M-13.1,-23.7L-36
-00000980: 2e37 2c2d 3233 2e37 432d 3338 2e34 2c2d  .7,-23.7C-38.4,-
-00000990: 3233 2e37 2c2d 3339 2e37 2c2d 3232 2e33  23.7,-39.7,-22.3
-000009a0: 2c2d 3339 2e37 2c2d 3230 2e37 4c2d 3339  ,-39.7,-20.7L-39
-000009b0: 2e37 2c31 342e 3743 2d33 392e 372c 3136  .7,14.7C-39.7,16
-000009c0: 2e33 2c2d 3339 2e35 2c31 382e 382c 2d34  .3,-39.5,18.8,-4
-000009d0: 302e 342c 3230 2e36 432d 3431 2e35 2c32  0.4,20.6C-41.5,2
-000009e0: 322e 342c 2d34 332e 342c 3233 2e37 2c2d  2.4,-43.4,23.7,-
-000009f0: 3435 2e37 2c32 332e 374c 2d37 362e 312c  45.7,23.7L-76.1,
-00000a00: 3233 2e37 222f 3e3c 7061 7468 2073 7472  23.7"/><path str
-00000a10: 6f6b 652d 6c69 6e65 6361 703d 2272 6f75  oke-linecap="rou
-00000a20: 6e64 2220 7472 616e 7366 6f72 6d3d 2274  nd" transform="t
-00000a30: 7261 6e73 6c61 7465 2837 3330 2e33 302c  ranslate(730.30,
-00000a40: 3131 392e 3838 2922 2069 643d 2273 6861  119.88)" id="sha
-00000a50: 7065 3130 2220 7374 726f 6b65 3d22 2334  pe10" stroke="#4
-00000a60: 3534 3534 3522 2073 7472 6f6b 652d 7769  54545" stroke-wi
-00000a70: 6474 683d 2234 2220 6669 6c6c 3d22 6e6f  dth="4" fill="no
-00000a80: 6e65 2220 643d 224d 2d31 322e 352c 3230  ne" d="M-12.5,20
-00000a90: 2e35 4c2d 302e 332c 3230 2e35 4331 2e34  .5L-0.3,20.5C1.4
-00000aa0: 2c32 302e 352c 322e 372c 3139 2e31 2c32  ,20.5,2.7,19.1,2
-00000ab0: 2e37 2c31 372e 354c 322e 372c 2d31 312e  .7,17.5L2.7,-11.
-00000ac0: 3543 322e 372c 2d31 332e 312c 322e 352c  5C2.7,-13.1,2.5,
-00000ad0: 2d31 352e 362c 332e 342c 2d31 372e 3443  -15.6,3.4,-17.4C
-00000ae0: 342e 352c 2d31 392e 322c 362e 342c 2d32  4.5,-19.2,6.4,-2
-00000af0: 302e 352c 382e 372c 2d32 302e 354c 3132  0.5,8.7,-20.5L12
-00000b00: 2e35 2c2d 3230 2e35 222f 3e3c 7061 7468  .5,-20.5"/><path
-00000b10: 2073 7472 6f6b 652d 6c69 6e65 6361 703d   stroke-linecap=
-00000b20: 2272 6f75 6e64 2220 7472 616e 7366 6f72  "round" transfor
-00000b30: 6d3d 2274 7261 6e73 6c61 7465 2837 3330  m="translate(730
-00000b40: 2e33 302c 3134 302e 3335 2922 2069 643d  .30,140.35)" id=
-00000b50: 2273 6861 7065 3131 2220 7374 726f 6b65  "shape11" stroke
-00000b60: 3d22 2334 3534 3534 3522 2073 7472 6f6b  ="#454545" strok
-00000b70: 652d 7769 6474 683d 2234 2220 6669 6c6c  e-width="4" fill
-00000b80: 3d22 6e6f 6e65 2220 643d 224d 2d31 322e  ="none" d="M-12.
-00000b90: 352c 2e30 4c2d 302e 332c 2e30 4331 2e34  5,.0L-0.3,.0C1.4
-00000ba0: 2c2e 302c 332e 372c 2e30 2c35 2e37 2c2e  ,.0,3.7,.0,5.7,.
-00000bb0: 3043 362e 362c 2e30 2c37 2e36 2c2e 302c  0C6.6,.0,7.6,.0,
-00000bc0: 382e 372c 2e30 4c31 322e 352c 2e30 222f  8.7,.0L12.5,.0"/
-00000bd0: 3e3c 7061 7468 2073 7472 6f6b 652d 6c69  ><path stroke-li
-00000be0: 6e65 6361 703d 2272 6f75 6e64 2220 7472  necap="round" tr
-00000bf0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-00000c00: 7465 2837 3330 2e33 302c 3136 302e 3832  te(730.30,160.82
-00000c10: 2922 2069 643d 2273 6861 7065 3132 2220  )" id="shape12" 
-00000c20: 7374 726f 6b65 3d22 2334 3534 3534 3522  stroke="#454545"
-00000c30: 2073 7472 6f6b 652d 7769 6474 683d 2234   stroke-width="4
-00000c40: 2220 6669 6c6c 3d22 6e6f 6e65 2220 643d  " fill="none" d=
-00000c50: 224d 2d31 322e 352c 2d32 302e 354c 2d30  "M-12.5,-20.5L-0
-00000c60: 2e33 2c2d 3230 2e35 4331 2e34 2c2d 3230  .3,-20.5C1.4,-20
-00000c70: 2e35 2c32 2e37 2c2d 3139 2e31 2c32 2e37  .5,2.7,-19.1,2.7
-00000c80: 2c2d 3137 2e35 4c32 2e37 2c31 312e 3543  ,-17.5L2.7,11.5C
-00000c90: 322e 372c 3133 2e31 2c32 2e35 2c31 352e  2.7,13.1,2.5,15.
-00000ca0: 362c 332e 342c 3137 2e34 4334 2e35 2c31  6,3.4,17.4C4.5,1
-00000cb0: 392e 322c 362e 342c 3230 2e35 2c38 2e37  9.2,6.4,20.5,8.7
-00000cc0: 2c32 302e 354c 3132 2e35 2c32 302e 3522  ,20.5L12.5,20.5"
-00000cd0: 2f3e 3c70 6174 6820 7374 726f 6b65 2d6c  /><path stroke-l
-00000ce0: 696e 6563 6170 3d22 726f 756e 6422 2074  inecap="round" t
-00000cf0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00000d00: 6174 6528 3735 342e 3330 2c34 3134 2e31  ate(754.30,414.1
-00000d10: 3829 2220 6964 3d22 7368 6170 6531 3322  8)" id="shape13"
-00000d20: 2073 7472 6f6b 653d 2223 3435 3435 3435   stroke="#454545
-00000d30: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
-00000d40: 3422 2066 696c 6c3d 226e 6f6e 6522 2064  4" fill="none" d
-00000d50: 3d22 4d2d 3132 2e35 2c32 302e 354c 2d30  ="M-12.5,20.5L-0
-00000d60: 2e33 2c32 302e 3543 312e 342c 3230 2e35  .3,20.5C1.4,20.5
-00000d70: 2c32 2e37 2c31 392e 312c 322e 372c 3137  ,2.7,19.1,2.7,17
-00000d80: 2e35 4c32 2e37 2c2d 3131 2e35 4332 2e37  .5L2.7,-11.5C2.7
-00000d90: 2c2d 3133 2e31 2c32 2e35 2c2d 3135 2e36  ,-13.1,2.5,-15.6
-00000da0: 2c33 2e34 2c2d 3137 2e34 4334 2e35 2c2d  ,3.4,-17.4C4.5,-
-00000db0: 3139 2e32 2c36 2e34 2c2d 3230 2e35 2c38  19.2,6.4,-20.5,8
-00000dc0: 2e37 2c2d 3230 2e35 4c31 322e 352c 2d32  .7,-20.5L12.5,-2
-00000dd0: 302e 3522 2f3e 3c70 6174 6820 7374 726f  0.5"/><path stro
-00000de0: 6b65 2d6c 696e 6563 6170 3d22 726f 756e  ke-linecap="roun
-00000df0: 6422 2074 7261 6e73 666f 726d 3d22 7472  d" transform="tr
-00000e00: 616e 736c 6174 6528 3735 342e 3330 2c34  anslate(754.30,4
-00000e10: 3535 2e31 3329 2220 6964 3d22 7368 6170  55.13)" id="shap
-00000e20: 6531 3422 2073 7472 6f6b 653d 2223 3435  e14" stroke="#45
-00000e30: 3435 3435 2220 7374 726f 6b65 2d77 6964  4545" stroke-wid
-00000e40: 7468 3d22 3422 2066 696c 6c3d 226e 6f6e  th="4" fill="non
-00000e50: 6522 2064 3d22 4d2d 3132 2e35 2c2d 3230  e" d="M-12.5,-20
-00000e60: 2e35 4c2d 302e 332c 2d32 302e 3543 312e  .5L-0.3,-20.5C1.
-00000e70: 342c 2d32 302e 352c 322e 372c 2d31 392e  4,-20.5,2.7,-19.
-00000e80: 312c 322e 372c 2d31 372e 354c 322e 372c  1,2.7,-17.5L2.7,
-00000e90: 3131 2e35 4332 2e37 2c31 332e 312c 322e  11.5C2.7,13.1,2.
-00000ea0: 352c 3135 2e36 2c33 2e34 2c31 372e 3443  5,15.6,3.4,17.4C
-00000eb0: 342e 352c 3139 2e32 2c36 2e34 2c32 302e  4.5,19.2,6.4,20.
-00000ec0: 352c 382e 372c 3230 2e35 4c31 322e 352c  5,8.7,20.5L12.5,
-00000ed0: 3230 2e35 222f 3e3c 7061 7468 2073 7472  20.5"/><path str
-00000ee0: 6f6b 652d 6c69 6e65 6361 703d 2272 6f75  oke-linecap="rou
-00000ef0: 6e64 2220 7472 616e 7366 6f72 6d3d 2274  nd" transform="t
-00000f00: 7261 6e73 6c61 7465 2832 3133 2e38 362c  ranslate(213.86,
-00000f10: 3436 312e 3536 2922 2069 643d 2273 6861  461.56)" id="sha
-00000f20: 7065 3135 2220 7374 726f 6b65 3d22 2334  pe15" stroke="#4
-00000f30: 3534 3534 3522 2073 7472 6f6b 652d 7769  54545" stroke-wi
-00000f40: 6474 683d 2234 2220 6669 6c6c 3d22 6e6f  dth="4" fill="no
-00000f50: 6e65 2220 643d 224d 3132 2e35 2c32 302e  ne" d="M12.5,20.
-00000f60: 354c 2e33 2c32 302e 3543 2d31 2e34 2c32  5L.3,20.5C-1.4,2
-00000f70: 302e 352c 2d32 2e37 2c31 392e 312c 2d32  0.5,-2.7,19.1,-2
-00000f80: 2e37 2c31 372e 354c 2d32 2e37 2c2d 3131  .7,17.5L-2.7,-11
-00000f90: 2e35 432d 322e 372c 2d31 332e 312c 2d32  .5C-2.7,-13.1,-2
-00000fa0: 2e35 2c2d 3135 2e36 2c2d 332e 342c 2d31  .5,-15.6,-3.4,-1
-00000fb0: 372e 3443 2d34 2e35 2c2d 3139 2e32 2c2d  7.4C-4.5,-19.2,-
-00000fc0: 362e 342c 2d32 302e 352c 2d38 2e37 2c2d  6.4,-20.5,-8.7,-
-00000fd0: 3230 2e35 4c2d 3132 2e35 2c2d 3230 2e35  20.5L-12.5,-20.5
-00000fe0: 222f 3e3c 7061 7468 2073 7472 6f6b 652d  "/><path stroke-
-00000ff0: 6c69 6e65 6361 703d 2272 6f75 6e64 2220  linecap="round" 
-00001000: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00001010: 6c61 7465 2837 3534 2e33 302c 3433 342e  late(754.30,434.
-00001020: 3635 2922 2069 643d 2273 6861 7065 3136  65)" id="shape16
-00001030: 2220 7374 726f 6b65 3d22 2334 3534 3534  " stroke="#45454
-00001040: 3522 2073 7472 6f6b 652d 7769 6474 683d  5" stroke-width=
-00001050: 2234 2220 6669 6c6c 3d22 6e6f 6e65 2220  "4" fill="none" 
-00001060: 643d 224d 2d31 322e 352c 2e30 4c2d 302e  d="M-12.5,.0L-0.
-00001070: 332c 2e30 4331 2e34 2c2e 302c 332e 372c  3,.0C1.4,.0,3.7,
-00001080: 2e30 2c35 2e37 2c2e 3043 362e 362c 2e30  .0,5.7,.0C6.6,.0
-00001090: 2c37 2e36 2c2e 302c 382e 372c 2e30 4c31  ,7.6,.0,8.7,.0L1
-000010a0: 322e 352c 2e30 222f 3e3c 7061 7468 2073  2.5,.0"/><path s
-000010b0: 7472 6f6b 652d 6c69 6e65 6361 703d 2272  troke-linecap="r
-000010c0: 6f75 6e64 2220 7472 616e 7366 6f72 6d3d  ound" transform=
-000010d0: 2274 7261 6e73 6c61 7465 2831 3239 2e38  "translate(129.8
-000010e0: 362c 3139 332e 3435 2922 2069 643d 2273  6,193.45)" id="s
-000010f0: 6861 7065 3137 2220 7374 726f 6b65 3d22  hape17" stroke="
-00001100: 2334 3534 3534 3522 2073 7472 6f6b 652d  #454545" stroke-
-00001110: 7769 6474 683d 2234 2220 6669 6c6c 3d22  width="4" fill="
-00001120: 6e6f 6e65 2220 643d 224d 3132 2e35 2c31  none" d="M12.5,1
-00001130: 302e 324c 2e33 2c31 302e 3243 2d31 2e34  0.2L.3,10.2C-1.4
-00001140: 2c31 302e 322c 2d32 2e37 2c38 2e39 2c2d  ,10.2,-2.7,8.9,-
-00001150: 322e 372c 372e 324c 2d32 2e37 2c2d 312e  2.7,7.2L-2.7,-1.
-00001160: 3243 2d32 2e37 2c2d 322e 392c 2d32 2e35  2C-2.7,-2.9,-2.5
-00001170: 2c2d 352e 332c 2d33 2e34 2c2d 372e 3143  ,-5.3,-3.4,-7.1C
-00001180: 2d34 2e35 2c2d 392e 302c 2d36 2e34 2c2d  -4.5,-9.0,-6.4,-
-00001190: 3130 2e32 2c2d 382e 372c 2d31 302e 324c  10.2,-8.7,-10.2L
-000011a0: 2d31 322e 352c 2d31 302e 3222 2f3e 3c70  -12.5,-10.2"/><p
-000011b0: 6174 6820 7374 726f 6b65 2d6c 696e 6563  ath stroke-linec
-000011c0: 6170 3d22 726f 756e 6422 2074 7261 6e73  ap="round" trans
-000011d0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-000011e0: 3132 392e 3836 2c32 3133 2e39 3329 2220  129.86,213.93)" 
-000011f0: 6964 3d22 7368 6170 6531 3822 2073 7472  id="shape18" str
-00001200: 6f6b 653d 2223 3435 3435 3435 2220 7374  oke="#454545" st
-00001210: 726f 6b65 2d77 6964 7468 3d22 3422 2066  roke-width="4" f
-00001220: 696c 6c3d 226e 6f6e 6522 2064 3d22 4d31  ill="none" d="M1
-00001230: 322e 352c 2d31 302e 324c 2e33 2c2d 3130  2.5,-10.2L.3,-10
-00001240: 2e32 432d 312e 342c 2d31 302e 322c 2d32  .2C-1.4,-10.2,-2
-00001250: 2e37 2c2d 382e 392c 2d32 2e37 2c2d 372e  .7,-8.9,-2.7,-7.
-00001260: 324c 2d32 2e37 2c31 2e32 432d 322e 372c  2L-2.7,1.2C-2.7,
-00001270: 322e 392c 2d32 2e35 2c35 2e33 2c2d 332e  2.9,-2.5,5.3,-3.
-00001280: 342c 372e 3143 2d34 2e35 2c39 2e30 2c2d  4,7.1C-4.5,9.0,-
-00001290: 362e 342c 3130 2e32 2c2d 382e 372c 3130  6.4,10.2,-8.7,10
-000012a0: 2e32 4c2d 3132 2e35 2c31 302e 3222 2f3e  .2L-12.5,10.2"/>
-000012b0: 3c70 6174 6820 7374 726f 6b65 2d6c 696e  <path stroke-lin
-000012c0: 6563 6170 3d22 726f 756e 6422 2074 7261  ecap="round" tra
-000012d0: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-000012e0: 6528 3133 322e 3836 2c33 3134 2e34 3129  e(132.86,314.41)
-000012f0: 2220 6964 3d22 7368 6170 6531 3922 2073  " id="shape19" s
-00001300: 7472 6f6b 653d 2223 3435 3435 3435 2220  troke="#454545" 
-00001310: 7374 726f 6b65 2d77 6964 7468 3d22 3422  stroke-width="4"
-00001320: 2066 696c 6c3d 226e 6f6e 6522 2064 3d22   fill="none" d="
-00001330: 4d31 322e 352c 3230 2e35 4c2e 332c 3230  M12.5,20.5L.3,20
-00001340: 2e35 432d 312e 342c 3230 2e35 2c2d 322e  .5C-1.4,20.5,-2.
-00001350: 372c 3139 2e31 2c2d 322e 372c 3137 2e35  7,19.1,-2.7,17.5
-00001360: 4c2d 322e 372c 2d31 312e 3543 2d32 2e37  L-2.7,-11.5C-2.7
-00001370: 2c2d 3133 2e31 2c2d 322e 352c 2d31 352e  ,-13.1,-2.5,-15.
-00001380: 362c 2d33 2e34 2c2d 3137 2e34 432d 342e  6,-3.4,-17.4C-4.
-00001390: 352c 2d31 392e 322c 2d36 2e34 2c2d 3230  5,-19.2,-6.4,-20
-000013a0: 2e35 2c2d 382e 372c 2d32 302e 354c 2d31  .5,-8.7,-20.5L-1
-000013b0: 322e 352c 2d32 302e 3522 2f3e 3c70 6174  2.5,-20.5"/><pat
-000013c0: 6820 7374 726f 6b65 2d6c 696e 6563 6170  h stroke-linecap
-000013d0: 3d22 726f 756e 6422 2074 7261 6e73 666f  ="round" transfo
-000013e0: 726d 3d22 7472 616e 736c 6174 6528 3133  rm="translate(13
-000013f0: 322e 3836 2c33 3334 2e38 3929 2220 6964  2.86,334.89)" id
-00001400: 3d22 7368 6170 6532 3022 2073 7472 6f6b  ="shape20" strok
-00001410: 653d 2223 3435 3435 3435 2220 7374 726f  e="#454545" stro
-00001420: 6b65 2d77 6964 7468 3d22 3422 2066 696c  ke-width="4" fil
-00001430: 6c3d 226e 6f6e 6522 2064 3d22 4d31 322e  l="none" d="M12.
-00001440: 352c 2e30 4c2e 332c 2e30 432d 312e 342c  5,.0L.3,.0C-1.4,
-00001450: 2e30 2c2d 332e 372c 2e30 2c2d 352e 372c  .0,-3.7,.0,-5.7,
-00001460: 2e30 432d 362e 362c 2e30 2c2d 372e 362c  .0C-6.6,.0,-7.6,
-00001470: 2e30 2c2d 382e 372c 2e30 4c2d 3132 2e35  .0,-8.7,.0L-12.5
-00001480: 2c2e 3022 2f3e 3c70 6174 6820 7374 726f  ,.0"/><path stro
-00001490: 6b65 2d6c 696e 6563 6170 3d22 726f 756e  ke-linecap="roun
-000014a0: 6422 2074 7261 6e73 666f 726d 3d22 7472  d" transform="tr
-000014b0: 616e 736c 6174 6528 3133 322e 3836 2c33  anslate(132.86,3
-000014c0: 3535 2e33 3629 2220 6964 3d22 7368 6170  55.36)" id="shap
-000014d0: 6532 3122 2073 7472 6f6b 653d 2223 3435  e21" stroke="#45
-000014e0: 3435 3435 2220 7374 726f 6b65 2d77 6964  4545" stroke-wid
-000014f0: 7468 3d22 3422 2066 696c 6c3d 226e 6f6e  th="4" fill="non
-00001500: 6522 2064 3d22 4d31 322e 352c 2d32 302e  e" d="M12.5,-20.
-00001510: 354c 2e33 2c2d 3230 2e35 432d 312e 342c  5L.3,-20.5C-1.4,
-00001520: 2d32 302e 352c 2d32 2e37 2c2d 3139 2e31  -20.5,-2.7,-19.1
-00001530: 2c2d 322e 372c 2d31 372e 354c 2d32 2e37  ,-2.7,-17.5L-2.7
-00001540: 2c31 312e 3543 2d32 2e37 2c31 332e 312c  ,11.5C-2.7,13.1,
-00001550: 2d32 2e35 2c31 352e 362c 2d33 2e34 2c31  -2.5,15.6,-3.4,1
-00001560: 372e 3443 2d34 2e35 2c31 392e 322c 2d36  7.4C-4.5,19.2,-6
-00001570: 2e34 2c32 302e 352c 2d38 2e37 2c32 302e  .4,20.5,-8.7,20.
-00001580: 354c 2d31 322e 352c 3230 2e35 222f 3e3c  5L-12.5,20.5"/><
-00001590: 7061 7468 2073 7472 6f6b 652d 6c69 6e65  path stroke-line
-000015a0: 6361 703d 2272 6f75 6e64 2220 7472 616e  cap="round" tran
-000015b0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-000015c0: 2832 3133 2e38 362c 3438 322e 3034 2922  (213.86,482.04)"
-000015d0: 2069 643d 2273 6861 7065 3232 2220 7374   id="shape22" st
-000015e0: 726f 6b65 3d22 2334 3534 3534 3522 2073  roke="#454545" s
-000015f0: 7472 6f6b 652d 7769 6474 683d 2234 2220  troke-width="4" 
-00001600: 6669 6c6c 3d22 6e6f 6e65 2220 643d 224d  fill="none" d="M
-00001610: 3132 2e35 2c2e 304c 2e33 2c2e 3043 2d31  12.5,.0L.3,.0C-1
-00001620: 2e34 2c2e 302c 2d33 2e37 2c2e 302c 2d35  .4,.0,-3.7,.0,-5
-00001630: 2e37 2c2e 3043 2d36 2e36 2c2e 302c 2d37  .7,.0C-6.6,.0,-7
-00001640: 2e36 2c2e 302c 2d38 2e37 2c2e 304c 2d31  .6,.0,-8.7,.0L-1
-00001650: 322e 352c 2e30 222f 3e3c 7061 7468 2073  2.5,.0"/><path s
-00001660: 7472 6f6b 652d 6c69 6e65 6361 703d 2272  troke-linecap="r
-00001670: 6f75 6e64 2220 7472 616e 7366 6f72 6d3d  ound" transform=
-00001680: 2274 7261 6e73 6c61 7465 2832 3133 2e38  "translate(213.8
-00001690: 362c 3530 322e 3531 2922 2069 643d 2273  6,502.51)" id="s
-000016a0: 6861 7065 3233 2220 7374 726f 6b65 3d22  hape23" stroke="
-000016b0: 2334 3534 3534 3522 2073 7472 6f6b 652d  #454545" stroke-
-000016c0: 7769 6474 683d 2234 2220 6669 6c6c 3d22  width="4" fill="
-000016d0: 6e6f 6e65 2220 643d 224d 3132 2e35 2c2d  none" d="M12.5,-
-000016e0: 3230 2e35 4c2e 332c 2d32 302e 3543 2d31  20.5L.3,-20.5C-1
-000016f0: 2e34 2c2d 3230 2e35 2c2d 322e 372c 2d31  .4,-20.5,-2.7,-1
-00001700: 392e 312c 2d32 2e37 2c2d 3137 2e35 4c2d  9.1,-2.7,-17.5L-
-00001710: 322e 372c 3131 2e35 432d 322e 372c 3133  2.7,11.5C-2.7,13
-00001720: 2e31 2c2d 322e 352c 3135 2e36 2c2d 332e  .1,-2.5,15.6,-3.
-00001730: 342c 3137 2e34 432d 342e 352c 3139 2e32  4,17.4C-4.5,19.2
-00001740: 2c2d 362e 342c 3230 2e35 2c2d 382e 372c  ,-6.4,20.5,-8.7,
-00001750: 3230 2e35 4c2d 3132 2e35 2c32 302e 3522  20.5L-12.5,20.5"
-00001760: 2f3e 3c70 6174 6820 7374 726f 6b65 2d6c  /><path stroke-l
-00001770: 696e 6563 6170 3d22 726f 756e 6422 2074  inecap="round" t
-00001780: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00001790: 6174 6528 3338 312e 3437 2c31 3930 2e32  ate(381.47,190.2
-000017a0: 3329 2220 6964 3d22 7368 6170 6532 3422  3)" id="shape24"
-000017b0: 2073 7472 6f6b 653d 2223 3435 3435 3435   stroke="#454545
-000017c0: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
-000017d0: 3422 2066 696c 6c3d 226e 6f6e 6522 2064  4" fill="none" d
-000017e0: 3d22 4d2d 3133 2e31 2c39 372e 334c 2d33  ="M-13.1,97.3L-3
-000017f0: 362e 372c 3937 2e33 432d 3338 2e34 2c39  6.7,97.3C-38.4,9
-00001800: 372e 332c 2d33 392e 372c 3935 2e39 2c2d  7.3,-39.7,95.9,-
-00001810: 3339 2e37 2c39 342e 334c 2d33 392e 372c  39.7,94.3L-39.7,
-00001820: 2d38 382e 3343 2d33 392e 372c 2d38 392e  -88.3C-39.7,-89.
-00001830: 392c 2d33 392e 352c 2d39 322e 342c 2d34  9,-39.5,-92.4,-4
-00001840: 302e 342c 2d39 342e 3143 2d34 312e 352c  0.4,-94.1C-41.5,
-00001850: 2d39 362e 302c 2d34 332e 342c 2d39 372e  -96.0,-43.4,-97.
-00001860: 332c 2d34 352e 372c 2d39 372e 334c 2d37  3,-45.7,-97.3L-7
-00001870: 362e 312c 2d39 372e 3322 2f3e 3c70 6174  6.1,-97.3"/><pat
-00001880: 6820 7374 726f 6b65 2d6c 696e 6563 6170  h stroke-linecap
-00001890: 3d22 726f 756e 6422 2074 7261 6e73 666f  ="round" transfo
-000018a0: 726d 3d22 7472 616e 736c 6174 6528 3134  rm="translate(14
-000018b0: 372e 3836 2c38 322e 3733 2922 2069 643d  7.86,82.73)" id=
-000018c0: 2273 6861 7065 3235 2220 7374 726f 6b65  "shape25" stroke
-000018d0: 3d22 2334 3534 3534 3522 2073 7472 6f6b  ="#454545" strok
-000018e0: 652d 7769 6474 683d 2234 2220 6669 6c6c  e-width="4" fill
-000018f0: 3d22 6e6f 6e65 2220 643d 224d 3132 2e35  ="none" d="M12.5
-00001900: 2c31 302e 3243 2e31 2c31 302e 322c 2e35  ,10.2C.1,10.2,.5
-00001910: 2c2d 3130 2e32 2c2d 3132 2e35 2c2d 3130  ,-10.2,-12.5,-10
-00001920: 2e32 222f 3e3c 7061 7468 2073 7472 6f6b  .2"/><path strok
-00001930: 652d 6c69 6e65 6361 703d 2272 6f75 6e64  e-linecap="round
-00001940: 2220 7472 616e 7366 6f72 6d3d 2274 7261  " transform="tra
-00001950: 6e73 6c61 7465 2831 3437 2e38 362c 3130  nslate(147.86,10
-00001960: 332e 3230 2922 2069 643d 2273 6861 7065  3.20)" id="shape
-00001970: 3236 2220 7374 726f 6b65 3d22 2334 3534  26" stroke="#454
-00001980: 3534 3522 2073 7472 6f6b 652d 7769 6474  545" stroke-widt
-00001990: 683d 2234 2220 6669 6c6c 3d22 6e6f 6e65  h="4" fill="none
-000019a0: 2220 643d 224d 3132 2e35 2c2d 3130 2e32  " d="M12.5,-10.2
-000019b0: 432e 312c 2d31 302e 322c 2e35 2c31 302e  C.1,-10.2,.5,10.
-000019c0: 322c 2d31 322e 352c 3130 2e32 222f 3e3c  2,-12.5,10.2"/><
-000019d0: 6720 7472 616e 7366 6f72 6d3d 2274 7261  g transform="tra
-000019e0: 6e73 6c61 7465 2833 3638 2e33 3631 3030  nslate(368.36100
-000019f0: 302c 3235 332e 3030 3030 3030 2922 2069  0,253.000000)" i
-00001a00: 643d 2273 6861 7065 3237 223e 3c70 6174  d="shape27"><pat
-00001a10: 6820 6669 6c6c 2d72 756c 653d 226e 6f6e  h fill-rule="non
-00001a20: 7a65 726f 2220 7374 726f 6b65 3d22 2333  zero" stroke="#3
-00001a30: 3033 3033 3022 2073 7472 6f6b 652d 7769  03030" stroke-wi
-00001a40: 6474 683d 2234 2220 6669 6c6c 3d22 2330  dth="4" fill="#0
-00001a50: 3035 3364 3622 2064 3d22 4d33 342e 352c  053d6" d="M34.5,
-00001a60: 2e30 4c31 3433 2e39 2c2e 3043 3136 332e  .0L143.9,.0C163.
-00001a70: 302c 2e30 2c31 3738 2e34 2c31 352e 342c  0,.0,178.4,15.4,
-00001a80: 3137 382e 342c 3334 2e35 4331 3738 2e34  178.4,34.5C178.4
-00001a90: 2c35 332e 362c 3136 332e 302c 3639 2e30  ,53.6,163.0,69.0
-00001aa0: 2c31 3433 2e39 2c36 392e 304c 3334 2e35  ,143.9,69.0L34.5
-00001ab0: 2c36 392e 3043 3135 2e34 2c36 392e 302c  ,69.0C15.4,69.0,
-00001ac0: 2e30 2c35 332e 362c 2e30 2c33 342e 3543  .0,53.6,.0,34.5C
-00001ad0: 2e30 2c31 352e 342c 3135 2e34 2c2e 302c  .0,15.4,15.4,.0,
-00001ae0: 3334 2e35 2c2e 307a 222f 3e3c 7465 7874  34.5,.0z"/><text
-00001af0: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
-00001b00: 6572 7665 2220 7374 796c 653d 2266 696c  erve" style="fil
-00001b10: 6c3a 2366 6666 6666 663b 666f 6e74 2d66  l:#ffffff;font-f
-00001b20: 616d 696c 793a e5be aee8 bdaf e99b 85e9  amily:..........
-00001b30: bb91 3b66 6f6e 742d 7369 7a65 3a31 382e  ..;font-size:18.
-00001b40: 3030 7074 3b66 6f6e 742d 7765 6967 6874  00pt;font-weight
-00001b50: 3a62 6f6c 6422 3e3c 7473 7061 6e20 783d  :bold"><tspan x=
-00001b60: 2233 342e 3022 2079 3d22 3434 2e30 223e  "34.0" y="44.0">
+00000000: 3c73 7667 2077 6964 7468 3d22 3933 3722  <svg width="937"
+00000010: 2068 6569 6768 743d 2235 3733 2220 786d   height="573" xm
+00000020: 6c6e 733a 786c 696e 6b3d 2268 7474 703a  lns:xlink="http:
+00000030: 2f2f 7777 772e 7733 2e6f 7267 2f31 3939  //www.w3.org/199
+00000040: 392f 786c 696e 6b22 2078 6d6c 6e73 3d22  9/xlink" xmlns="
+00000050: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+00000060: 672f 3230 3030 2f73 7667 2220 786d 6c6e  g/2000/svg" xmln
+00000070: 733a 6576 3d22 6874 7470 3a2f 2f77 7777  s:ev="http://www
+00000080: 2e77 332e 6f72 672f 3230 3031 2f78 6d6c  .w3.org/2001/xml
+00000090: 2d65 7665 6e74 7322 2076 6965 7742 6f78  -events" viewBox
+000000a0: 3d22 3020 3020 3933 3720 3537 3322 3e3c  ="0 0 937 573"><
+000000b0: 6465 6673 2f3e 3c67 2069 643d 2270 6167  defs/><g id="pag
+000000c0: 6531 2220 7472 616e 7366 6f72 6d3d 2274  e1" transform="t
+000000d0: 7261 6e73 6c61 7465 2835 2e35 2c35 2e35  ranslate(5.5,5.5
+000000e0: 2922 3e3c 7265 6374 2077 6964 7468 3d22  )"><rect width="
+000000f0: 3932 3722 2068 6569 6768 743d 2235 3633  927" height="563
+00000100: 2220 793d 2230 2220 6669 6c6c 3d22 6e6f  " y="0" fill="no
+00000110: 6e65 2220 783d 2230 222f 3e3c 7061 7468  ne" x="0"/><path
+00000120: 2064 3d22 4d31 332e 312c 2e30 4c33 362e   d="M13.1,.0L36.
+00000130: 372c 2e30 4333 382e 342c 2e30 2c34 302e  7,.0C38.4,.0,40.
+00000140: 372c 2e30 2c34 322e 372c 2e30 4334 332e  7,.0,42.7,.0C43.
+00000150: 362c 2e30 2c34 342e 362c 2e30 2c34 352e  6,.0,44.6,.0,45.
+00000160: 372c 2e30 4c37 362e 312c 2e30 2220 7374  7,.0L76.1,.0" st
+00000170: 726f 6b65 2d6c 696e 6563 6170 3d22 726f  roke-linecap="ro
+00000180: 756e 6422 2069 643d 2273 6861 7065 3122  und" id="shape1"
+00000190: 2073 7472 6f6b 653d 2223 3435 3435 3435   stroke="#454545
+000001a0: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
+000001b0: 3422 2066 696c 6c3d 226e 6f6e 6522 2074  4" fill="none" t
+000001c0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+000001d0: 6174 6528 3533 332e 3639 2c32 3837 2e35  ate(533.69,287.5
+000001e0: 3029 222f 3e3c 7061 7468 2064 3d22 4d31  0)"/><path d="M1
+000001f0: 332e 312c 3733 2e36 4c33 362e 372c 3733  3.1,73.6L36.7,73
+00000200: 2e36 4333 382e 342c 3733 2e36 2c33 392e  .6C38.4,73.6,39.
+00000210: 372c 3732 2e32 2c33 392e 372c 3730 2e36  7,72.2,39.7,70.6
+00000220: 4c33 392e 372c 2d36 342e 3643 3339 2e37  L39.7,-64.6C39.7
+00000230: 2c2d 3636 2e32 2c33 392e 352c 2d36 382e  ,-66.2,39.5,-68.
+00000240: 372c 3430 2e34 2c2d 3730 2e35 4334 312e  7,40.4,-70.5C41.
+00000250: 352c 2d37 322e 332c 3433 2e34 2c2d 3733  5,-72.3,43.4,-73
+00000260: 2e36 2c34 352e 372c 2d37 332e 364c 3736  .6,45.7,-73.6L76
+00000270: 2e31 2c2d 3733 2e36 2220 7374 726f 6b65  .1,-73.6" stroke
+00000280: 2d6c 696e 6563 6170 3d22 726f 756e 6422  -linecap="round"
+00000290: 2069 643d 2273 6861 7065 3222 2073 7472   id="shape2" str
+000002a0: 6f6b 653d 2223 3435 3435 3435 2220 7374  oke="#454545" st
+000002b0: 726f 6b65 2d77 6964 7468 3d22 3422 2066  roke-width="4" f
+000002c0: 696c 6c3d 226e 6f6e 6522 2074 7261 6e73  ill="none" trans
+000002d0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+000002e0: 3533 332e 3639 2c32 3133 2e39 3329 222f  533.69,213.93)"/
+000002f0: 3e3c 7061 7468 2064 3d22 4d31 332e 312c  ><path d="M13.1,
+00000300: 2d37 332e 364c 3336 2e37 2c2d 3733 2e36  -73.6L36.7,-73.6
+00000310: 4333 382e 342c 2d37 332e 362c 3339 2e37  C38.4,-73.6,39.7
+00000320: 2c2d 3732 2e32 2c33 392e 372c 2d37 302e  ,-72.2,39.7,-70.
+00000330: 364c 3339 2e37 2c36 342e 3643 3339 2e37  6L39.7,64.6C39.7
+00000340: 2c36 362e 322c 3339 2e35 2c36 382e 372c  ,66.2,39.5,68.7,
+00000350: 3430 2e34 2c37 302e 3543 3431 2e35 2c37  40.4,70.5C41.5,7
+00000360: 322e 332c 3433 2e34 2c37 332e 362c 3435  2.3,43.4,73.6,45
+00000370: 2e37 2c37 332e 364c 3736 2e31 2c37 332e  .7,73.6L76.1,73.
+00000380: 3622 2073 7472 6f6b 652d 6c69 6e65 6361  6" stroke-lineca
+00000390: 703d 2272 6f75 6e64 2220 6964 3d22 7368  p="round" id="sh
+000003a0: 6170 6533 2220 7374 726f 6b65 3d22 2334  ape3" stroke="#4
+000003b0: 3534 3534 3522 2073 7472 6f6b 652d 7769  54545" stroke-wi
+000003c0: 6474 683d 2234 2220 6669 6c6c 3d22 6e6f  dth="4" fill="no
+000003d0: 6e65 2220 7472 616e 7366 6f72 6d3d 2274  ne" transform="t
+000003e0: 7261 6e73 6c61 7465 2835 3333 2e36 392c  ranslate(533.69,
+000003f0: 3336 312e 3038 2922 2f3e 3c70 6174 6820  361.08)"/><path 
+00000400: 643d 224d 2d31 322e 352c 3230 2e35 4c2d  d="M-12.5,20.5L-
+00000410: 302e 332c 3230 2e35 4331 2e34 2c32 302e  0.3,20.5C1.4,20.
+00000420: 352c 322e 372c 3139 2e31 2c32 2e37 2c31  5,2.7,19.1,2.7,1
+00000430: 372e 354c 322e 372c 2d31 312e 3543 322e  7.5L2.7,-11.5C2.
+00000440: 372c 2d31 332e 312c 322e 352c 2d31 352e  7,-13.1,2.5,-15.
+00000450: 362c 332e 342c 2d31 372e 3443 342e 352c  6,3.4,-17.4C4.5,
+00000460: 2d31 392e 322c 362e 342c 2d32 302e 352c  -19.2,6.4,-20.5,
+00000470: 382e 372c 2d32 302e 354c 3132 2e35 2c2d  8.7,-20.5L12.5,-
+00000480: 3230 2e35 2220 7374 726f 6b65 2d6c 696e  20.5" stroke-lin
+00000490: 6563 6170 3d22 726f 756e 6422 2069 643d  ecap="round" id=
+000004a0: 2273 6861 7065 3422 2073 7472 6f6b 653d  "shape4" stroke=
+000004b0: 2223 3435 3435 3435 2220 7374 726f 6b65  "#454545" stroke
+000004c0: 2d77 6964 7468 3d22 3422 2066 696c 6c3d  -width="4" fill=
+000004d0: 226e 6f6e 6522 2074 7261 6e73 666f 726d  "none" transform
+000004e0: 3d22 7472 616e 736c 6174 6528 3732 352e  ="translate(725.
+000004f0: 3330 2c32 3637 2e30 3229 222f 3e3c 7061  30,267.02)"/><pa
+00000500: 7468 2064 3d22 4d2d 3132 2e35 2c2e 304c  th d="M-12.5,.0L
+00000510: 2d30 2e33 2c2e 3043 312e 342c 2e30 2c33  -0.3,.0C1.4,.0,3
+00000520: 2e37 2c2e 302c 352e 372c 2e30 4336 2e36  .7,.0,5.7,.0C6.6
+00000530: 2c2e 302c 372e 362c 2e30 2c38 2e37 2c2e  ,.0,7.6,.0,8.7,.
+00000540: 304c 3132 2e35 2c2e 3022 2073 7472 6f6b  0L12.5,.0" strok
+00000550: 652d 6c69 6e65 6361 703d 2272 6f75 6e64  e-linecap="round
+00000560: 2220 6964 3d22 7368 6170 6535 2220 7374  " id="shape5" st
+00000570: 726f 6b65 3d22 2334 3534 3534 3522 2073  roke="#454545" s
+00000580: 7472 6f6b 652d 7769 6474 683d 2234 2220  troke-width="4" 
+00000590: 6669 6c6c 3d22 6e6f 6e65 2220 7472 616e  fill="none" tran
+000005a0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+000005b0: 2837 3235 2e33 302c 3238 372e 3530 2922  (725.30,287.50)"
+000005c0: 2f3e 3c70 6174 6820 643d 224d 2d31 322e  /><path d="M-12.
+000005d0: 352c 2d32 302e 354c 2d30 2e33 2c2d 3230  5,-20.5L-0.3,-20
+000005e0: 2e35 4331 2e34 2c2d 3230 2e35 2c32 2e37  .5C1.4,-20.5,2.7
+000005f0: 2c2d 3139 2e31 2c32 2e37 2c2d 3137 2e35  ,-19.1,2.7,-17.5
+00000600: 4c32 2e37 2c31 312e 3543 322e 372c 3133  L2.7,11.5C2.7,13
+00000610: 2e31 2c32 2e35 2c31 352e 362c 332e 342c  .1,2.5,15.6,3.4,
+00000620: 3137 2e34 4334 2e35 2c31 392e 322c 362e  17.4C4.5,19.2,6.
+00000630: 342c 3230 2e35 2c38 2e37 2c32 302e 354c  4,20.5,8.7,20.5L
+00000640: 3132 2e35 2c32 302e 3522 2073 7472 6f6b  12.5,20.5" strok
+00000650: 652d 6c69 6e65 6361 703d 2272 6f75 6e64  e-linecap="round
+00000660: 2220 6964 3d22 7368 6170 6536 2220 7374  " id="shape6" st
+00000670: 726f 6b65 3d22 2334 3534 3534 3522 2073  roke="#454545" s
+00000680: 7472 6f6b 652d 7769 6474 683d 2234 2220  troke-width="4" 
+00000690: 6669 6c6c 3d22 6e6f 6e65 2220 7472 616e  fill="none" tran
+000006a0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+000006b0: 2837 3235 2e33 302c 3330 372e 3938 2922  (725.30,307.98)"
+000006c0: 2f3e 3c70 6174 6820 643d 224d 2d31 332e  /><path d="M-13.
+000006d0: 312c 2d39 372e 334c 2d33 362e 372c 2d39  1,-97.3L-36.7,-9
+000006e0: 372e 3343 2d33 382e 342c 2d39 372e 332c  7.3C-38.4,-97.3,
+000006f0: 2d33 392e 372c 2d39 352e 392c 2d33 392e  -39.7,-95.9,-39.
+00000700: 372c 2d39 342e 334c 2d33 392e 372c 3838  7,-94.3L-39.7,88
+00000710: 2e33 432d 3339 2e37 2c38 392e 392c 2d33  .3C-39.7,89.9,-3
+00000720: 392e 352c 3932 2e34 2c2d 3430 2e34 2c39  9.5,92.4,-40.4,9
+00000730: 342e 3143 2d34 312e 352c 3936 2e30 2c2d  4.1C-41.5,96.0,-
+00000740: 3433 2e34 2c39 372e 332c 2d34 352e 372c  43.4,97.3,-45.7,
+00000750: 3937 2e33 4c2d 3736 2e31 2c39 372e 3322  97.3L-76.1,97.3"
+00000760: 2073 7472 6f6b 652d 6c69 6e65 6361 703d   stroke-linecap=
+00000770: 2272 6f75 6e64 2220 6964 3d22 7368 6170  "round" id="shap
+00000780: 6537 2220 7374 726f 6b65 3d22 2334 3534  e7" stroke="#454
+00000790: 3534 3522 2073 7472 6f6b 652d 7769 6474  545" stroke-widt
+000007a0: 683d 2234 2220 6669 6c6c 3d22 6e6f 6e65  h="4" fill="none
+000007b0: 2220 7472 616e 7366 6f72 6d3d 2274 7261  " transform="tra
+000007c0: 6e73 6c61 7465 2833 3831 2e34 372c 3338  nslate(381.47,38
+000007d0: 342e 3737 2922 2f3e 3c70 6174 6820 643d  4.77)"/><path d=
+000007e0: 224d 2d31 332e 312c 3431 2e39 4c2d 3336  "M-13.1,41.9L-36
+000007f0: 2e37 2c34 312e 3943 2d33 382e 342c 3431  .7,41.9C-38.4,41
+00000800: 2e39 2c2d 3339 2e37 2c34 302e 362c 2d33  .9,-39.7,40.6,-3
+00000810: 392e 372c 3338 2e39 4c2d 3339 2e37 2c2d  9.7,38.9L-39.7,-
+00000820: 3332 2e39 432d 3339 2e37 2c2d 3334 2e36  32.9C-39.7,-34.6
+00000830: 2c2d 3339 2e35 2c2d 3337 2e30 2c2d 3430  ,-39.5,-37.0,-40
+00000840: 2e34 2c2d 3338 2e38 432d 3431 2e35 2c2d  .4,-38.8C-41.5,-
+00000850: 3430 2e36 2c2d 3433 2e34 2c2d 3431 2e39  40.6,-43.4,-41.9
+00000860: 2c2d 3435 2e37 2c2d 3431 2e39 4c2d 3736  ,-45.7,-41.9L-76
+00000870: 2e31 2c2d 3431 2e39 2220 7374 726f 6b65  .1,-41.9" stroke
+00000880: 2d6c 696e 6563 6170 3d22 726f 756e 6422  -linecap="round"
+00000890: 2069 643d 2273 6861 7065 3822 2073 7472   id="shape8" str
+000008a0: 6f6b 653d 2223 3435 3435 3435 2220 7374  oke="#454545" st
+000008b0: 726f 6b65 2d77 6964 7468 3d22 3422 2066  roke-width="4" f
+000008c0: 696c 6c3d 226e 6f6e 6522 2074 7261 6e73  ill="none" trans
+000008d0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+000008e0: 3338 312e 3437 2c32 3435 2e35 3929 222f  381.47,245.59)"/
+000008f0: 3e3c 7061 7468 2064 3d22 4d2d 3133 2e31  ><path d="M-13.1
+00000900: 2c2d 3233 2e37 4c2d 3336 2e37 2c2d 3233  ,-23.7L-36.7,-23
+00000910: 2e37 432d 3338 2e34 2c2d 3233 2e37 2c2d  .7C-38.4,-23.7,-
+00000920: 3339 2e37 2c2d 3232 2e33 2c2d 3339 2e37  39.7,-22.3,-39.7
+00000930: 2c2d 3230 2e37 4c2d 3339 2e37 2c31 342e  ,-20.7L-39.7,14.
+00000940: 3743 2d33 392e 372c 3136 2e33 2c2d 3339  7C-39.7,16.3,-39
+00000950: 2e35 2c31 382e 382c 2d34 302e 342c 3230  .5,18.8,-40.4,20
+00000960: 2e36 432d 3431 2e35 2c32 322e 342c 2d34  .6C-41.5,22.4,-4
+00000970: 332e 342c 3233 2e37 2c2d 3435 2e37 2c32  3.4,23.7,-45.7,2
+00000980: 332e 374c 2d37 362e 312c 3233 2e37 2220  3.7L-76.1,23.7" 
+00000990: 7374 726f 6b65 2d6c 696e 6563 6170 3d22  stroke-linecap="
+000009a0: 726f 756e 6422 2069 643d 2273 6861 7065  round" id="shape
+000009b0: 3922 2073 7472 6f6b 653d 2223 3435 3435  9" stroke="#4545
+000009c0: 3435 2220 7374 726f 6b65 2d77 6964 7468  45" stroke-width
+000009d0: 3d22 3422 2066 696c 6c3d 226e 6f6e 6522  ="4" fill="none"
+000009e0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+000009f0: 736c 6174 6528 3338 312e 3437 2c33 3131  slate(381.47,311
+00000a00: 2e31 3929 222f 3e3c 7061 7468 2064 3d22  .19)"/><path d="
+00000a10: 4d2d 3132 2e35 2c32 302e 354c 2d30 2e33  M-12.5,20.5L-0.3
+00000a20: 2c32 302e 3543 312e 342c 3230 2e35 2c32  ,20.5C1.4,20.5,2
+00000a30: 2e37 2c31 392e 312c 322e 372c 3137 2e35  .7,19.1,2.7,17.5
+00000a40: 4c32 2e37 2c2d 3131 2e35 4332 2e37 2c2d  L2.7,-11.5C2.7,-
+00000a50: 3133 2e31 2c32 2e35 2c2d 3135 2e36 2c33  13.1,2.5,-15.6,3
+00000a60: 2e34 2c2d 3137 2e34 4334 2e35 2c2d 3139  .4,-17.4C4.5,-19
+00000a70: 2e32 2c36 2e34 2c2d 3230 2e35 2c38 2e37  .2,6.4,-20.5,8.7
+00000a80: 2c2d 3230 2e35 4c31 322e 352c 2d32 302e  ,-20.5L12.5,-20.
+00000a90: 3522 2073 7472 6f6b 652d 6c69 6e65 6361  5" stroke-lineca
+00000aa0: 703d 2272 6f75 6e64 2220 6964 3d22 7368  p="round" id="sh
+00000ab0: 6170 6531 3022 2073 7472 6f6b 653d 2223  ape10" stroke="#
+00000ac0: 3435 3435 3435 2220 7374 726f 6b65 2d77  454545" stroke-w
+00000ad0: 6964 7468 3d22 3422 2066 696c 6c3d 226e  idth="4" fill="n
+00000ae0: 6f6e 6522 2074 7261 6e73 666f 726d 3d22  one" transform="
+00000af0: 7472 616e 736c 6174 6528 3733 302e 3330  translate(730.30
+00000b00: 2c31 3139 2e38 3829 222f 3e3c 7061 7468  ,119.88)"/><path
+00000b10: 2064 3d22 4d2d 3132 2e35 2c2e 304c 2d30   d="M-12.5,.0L-0
+00000b20: 2e33 2c2e 3043 312e 342c 2e30 2c33 2e37  .3,.0C1.4,.0,3.7
+00000b30: 2c2e 302c 352e 372c 2e30 4336 2e36 2c2e  ,.0,5.7,.0C6.6,.
+00000b40: 302c 372e 362c 2e30 2c38 2e37 2c2e 304c  0,7.6,.0,8.7,.0L
+00000b50: 3132 2e35 2c2e 3022 2073 7472 6f6b 652d  12.5,.0" stroke-
+00000b60: 6c69 6e65 6361 703d 2272 6f75 6e64 2220  linecap="round" 
+00000b70: 6964 3d22 7368 6170 6531 3122 2073 7472  id="shape11" str
+00000b80: 6f6b 653d 2223 3435 3435 3435 2220 7374  oke="#454545" st
+00000b90: 726f 6b65 2d77 6964 7468 3d22 3422 2066  roke-width="4" f
+00000ba0: 696c 6c3d 226e 6f6e 6522 2074 7261 6e73  ill="none" trans
+00000bb0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+00000bc0: 3733 302e 3330 2c31 3430 2e33 3529 222f  730.30,140.35)"/
+00000bd0: 3e3c 7061 7468 2064 3d22 4d2d 3132 2e35  ><path d="M-12.5
+00000be0: 2c2d 3230 2e35 4c2d 302e 332c 2d32 302e  ,-20.5L-0.3,-20.
+00000bf0: 3543 312e 342c 2d32 302e 352c 322e 372c  5C1.4,-20.5,2.7,
+00000c00: 2d31 392e 312c 322e 372c 2d31 372e 354c  -19.1,2.7,-17.5L
+00000c10: 322e 372c 3131 2e35 4332 2e37 2c31 332e  2.7,11.5C2.7,13.
+00000c20: 312c 322e 352c 3135 2e36 2c33 2e34 2c31  1,2.5,15.6,3.4,1
+00000c30: 372e 3443 342e 352c 3139 2e32 2c36 2e34  7.4C4.5,19.2,6.4
+00000c40: 2c32 302e 352c 382e 372c 3230 2e35 4c31  ,20.5,8.7,20.5L1
+00000c50: 322e 352c 3230 2e35 2220 7374 726f 6b65  2.5,20.5" stroke
+00000c60: 2d6c 696e 6563 6170 3d22 726f 756e 6422  -linecap="round"
+00000c70: 2069 643d 2273 6861 7065 3132 2220 7374   id="shape12" st
+00000c80: 726f 6b65 3d22 2334 3534 3534 3522 2073  roke="#454545" s
+00000c90: 7472 6f6b 652d 7769 6474 683d 2234 2220  troke-width="4" 
+00000ca0: 6669 6c6c 3d22 6e6f 6e65 2220 7472 616e  fill="none" tran
+00000cb0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00000cc0: 2837 3330 2e33 302c 3136 302e 3832 2922  (730.30,160.82)"
+00000cd0: 2f3e 3c70 6174 6820 643d 224d 2d31 322e  /><path d="M-12.
+00000ce0: 352c 3230 2e35 4c2d 302e 332c 3230 2e35  5,20.5L-0.3,20.5
+00000cf0: 4331 2e34 2c32 302e 352c 322e 372c 3139  C1.4,20.5,2.7,19
+00000d00: 2e31 2c32 2e37 2c31 372e 354c 322e 372c  .1,2.7,17.5L2.7,
+00000d10: 2d31 312e 3543 322e 372c 2d31 332e 312c  -11.5C2.7,-13.1,
+00000d20: 322e 352c 2d31 352e 362c 332e 342c 2d31  2.5,-15.6,3.4,-1
+00000d30: 372e 3443 342e 352c 2d31 392e 322c 362e  7.4C4.5,-19.2,6.
+00000d40: 342c 2d32 302e 352c 382e 372c 2d32 302e  4,-20.5,8.7,-20.
+00000d50: 354c 3132 2e35 2c2d 3230 2e35 2220 7374  5L12.5,-20.5" st
+00000d60: 726f 6b65 2d6c 696e 6563 6170 3d22 726f  roke-linecap="ro
+00000d70: 756e 6422 2069 643d 2273 6861 7065 3133  und" id="shape13
+00000d80: 2220 7374 726f 6b65 3d22 2334 3534 3534  " stroke="#45454
+00000d90: 3522 2073 7472 6f6b 652d 7769 6474 683d  5" stroke-width=
+00000da0: 2234 2220 6669 6c6c 3d22 6e6f 6e65 2220  "4" fill="none" 
+00000db0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00000dc0: 6c61 7465 2837 3534 2e33 302c 3431 342e  late(754.30,414.
+00000dd0: 3138 2922 2f3e 3c70 6174 6820 643d 224d  18)"/><path d="M
+00000de0: 2d31 322e 352c 2d32 302e 354c 2d30 2e33  -12.5,-20.5L-0.3
+00000df0: 2c2d 3230 2e35 4331 2e34 2c2d 3230 2e35  ,-20.5C1.4,-20.5
+00000e00: 2c32 2e37 2c2d 3139 2e31 2c32 2e37 2c2d  ,2.7,-19.1,2.7,-
+00000e10: 3137 2e35 4c32 2e37 2c31 312e 3543 322e  17.5L2.7,11.5C2.
+00000e20: 372c 3133 2e31 2c32 2e35 2c31 352e 362c  7,13.1,2.5,15.6,
+00000e30: 332e 342c 3137 2e34 4334 2e35 2c31 392e  3.4,17.4C4.5,19.
+00000e40: 322c 362e 342c 3230 2e35 2c38 2e37 2c32  2,6.4,20.5,8.7,2
+00000e50: 302e 354c 3132 2e35 2c32 302e 3522 2073  0.5L12.5,20.5" s
+00000e60: 7472 6f6b 652d 6c69 6e65 6361 703d 2272  troke-linecap="r
+00000e70: 6f75 6e64 2220 6964 3d22 7368 6170 6531  ound" id="shape1
+00000e80: 3422 2073 7472 6f6b 653d 2223 3435 3435  4" stroke="#4545
+00000e90: 3435 2220 7374 726f 6b65 2d77 6964 7468  45" stroke-width
+00000ea0: 3d22 3422 2066 696c 6c3d 226e 6f6e 6522  ="4" fill="none"
+00000eb0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+00000ec0: 736c 6174 6528 3735 342e 3330 2c34 3535  slate(754.30,455
+00000ed0: 2e31 3329 222f 3e3c 7061 7468 2064 3d22  .13)"/><path d="
+00000ee0: 4d31 322e 352c 3230 2e35 4c2e 332c 3230  M12.5,20.5L.3,20
+00000ef0: 2e35 432d 312e 342c 3230 2e35 2c2d 322e  .5C-1.4,20.5,-2.
+00000f00: 372c 3139 2e31 2c2d 322e 372c 3137 2e35  7,19.1,-2.7,17.5
+00000f10: 4c2d 322e 372c 2d31 312e 3543 2d32 2e37  L-2.7,-11.5C-2.7
+00000f20: 2c2d 3133 2e31 2c2d 322e 352c 2d31 352e  ,-13.1,-2.5,-15.
+00000f30: 362c 2d33 2e34 2c2d 3137 2e34 432d 342e  6,-3.4,-17.4C-4.
+00000f40: 352c 2d31 392e 322c 2d36 2e34 2c2d 3230  5,-19.2,-6.4,-20
+00000f50: 2e35 2c2d 382e 372c 2d32 302e 354c 2d31  .5,-8.7,-20.5L-1
+00000f60: 322e 352c 2d32 302e 3522 2073 7472 6f6b  2.5,-20.5" strok
+00000f70: 652d 6c69 6e65 6361 703d 2272 6f75 6e64  e-linecap="round
+00000f80: 2220 6964 3d22 7368 6170 6531 3522 2073  " id="shape15" s
+00000f90: 7472 6f6b 653d 2223 3435 3435 3435 2220  troke="#454545" 
+00000fa0: 7374 726f 6b65 2d77 6964 7468 3d22 3422  stroke-width="4"
+00000fb0: 2066 696c 6c3d 226e 6f6e 6522 2074 7261   fill="none" tra
+00000fc0: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+00000fd0: 6528 3231 332e 3836 2c34 3631 2e35 3629  e(213.86,461.56)
+00000fe0: 222f 3e3c 7061 7468 2064 3d22 4d2d 3132  "/><path d="M-12
+00000ff0: 2e35 2c2e 304c 2d30 2e33 2c2e 3043 312e  .5,.0L-0.3,.0C1.
+00001000: 342c 2e30 2c33 2e37 2c2e 302c 352e 372c  4,.0,3.7,.0,5.7,
+00001010: 2e30 4336 2e36 2c2e 302c 372e 362c 2e30  .0C6.6,.0,7.6,.0
+00001020: 2c38 2e37 2c2e 304c 3132 2e35 2c2e 3022  ,8.7,.0L12.5,.0"
+00001030: 2073 7472 6f6b 652d 6c69 6e65 6361 703d   stroke-linecap=
+00001040: 2272 6f75 6e64 2220 6964 3d22 7368 6170  "round" id="shap
+00001050: 6531 3622 2073 7472 6f6b 653d 2223 3435  e16" stroke="#45
+00001060: 3435 3435 2220 7374 726f 6b65 2d77 6964  4545" stroke-wid
+00001070: 7468 3d22 3422 2066 696c 6c3d 226e 6f6e  th="4" fill="non
+00001080: 6522 2074 7261 6e73 666f 726d 3d22 7472  e" transform="tr
+00001090: 616e 736c 6174 6528 3735 342e 3330 2c34  anslate(754.30,4
+000010a0: 3334 2e36 3529 222f 3e3c 7061 7468 2064  34.65)"/><path d
+000010b0: 3d22 4d31 322e 352c 3130 2e32 4c2e 332c  ="M12.5,10.2L.3,
+000010c0: 3130 2e32 432d 312e 342c 3130 2e32 2c2d  10.2C-1.4,10.2,-
+000010d0: 322e 372c 382e 392c 2d32 2e37 2c37 2e32  2.7,8.9,-2.7,7.2
+000010e0: 4c2d 322e 372c 2d31 2e32 432d 322e 372c  L-2.7,-1.2C-2.7,
+000010f0: 2d32 2e39 2c2d 322e 352c 2d35 2e33 2c2d  -2.9,-2.5,-5.3,-
+00001100: 332e 342c 2d37 2e31 432d 342e 352c 2d39  3.4,-7.1C-4.5,-9
+00001110: 2e30 2c2d 362e 342c 2d31 302e 322c 2d38  .0,-6.4,-10.2,-8
+00001120: 2e37 2c2d 3130 2e32 4c2d 3132 2e35 2c2d  .7,-10.2L-12.5,-
+00001130: 3130 2e32 2220 7374 726f 6b65 2d6c 696e  10.2" stroke-lin
+00001140: 6563 6170 3d22 726f 756e 6422 2069 643d  ecap="round" id=
+00001150: 2273 6861 7065 3137 2220 7374 726f 6b65  "shape17" stroke
+00001160: 3d22 2334 3534 3534 3522 2073 7472 6f6b  ="#454545" strok
+00001170: 652d 7769 6474 683d 2234 2220 6669 6c6c  e-width="4" fill
+00001180: 3d22 6e6f 6e65 2220 7472 616e 7366 6f72  ="none" transfor
+00001190: 6d3d 2274 7261 6e73 6c61 7465 2831 3239  m="translate(129
+000011a0: 2e38 362c 3139 332e 3435 2922 2f3e 3c70  .86,193.45)"/><p
+000011b0: 6174 6820 643d 224d 3132 2e35 2c2d 3130  ath d="M12.5,-10
+000011c0: 2e32 4c2e 332c 2d31 302e 3243 2d31 2e34  .2L.3,-10.2C-1.4
+000011d0: 2c2d 3130 2e32 2c2d 322e 372c 2d38 2e39  ,-10.2,-2.7,-8.9
+000011e0: 2c2d 322e 372c 2d37 2e32 4c2d 322e 372c  ,-2.7,-7.2L-2.7,
+000011f0: 312e 3243 2d32 2e37 2c32 2e39 2c2d 322e  1.2C-2.7,2.9,-2.
+00001200: 352c 352e 332c 2d33 2e34 2c37 2e31 432d  5,5.3,-3.4,7.1C-
+00001210: 342e 352c 392e 302c 2d36 2e34 2c31 302e  4.5,9.0,-6.4,10.
+00001220: 322c 2d38 2e37 2c31 302e 324c 2d31 322e  2,-8.7,10.2L-12.
+00001230: 352c 3130 2e32 2220 7374 726f 6b65 2d6c  5,10.2" stroke-l
+00001240: 696e 6563 6170 3d22 726f 756e 6422 2069  inecap="round" i
+00001250: 643d 2273 6861 7065 3138 2220 7374 726f  d="shape18" stro
+00001260: 6b65 3d22 2334 3534 3534 3522 2073 7472  ke="#454545" str
+00001270: 6f6b 652d 7769 6474 683d 2234 2220 6669  oke-width="4" fi
+00001280: 6c6c 3d22 6e6f 6e65 2220 7472 616e 7366  ll="none" transf
+00001290: 6f72 6d3d 2274 7261 6e73 6c61 7465 2831  orm="translate(1
+000012a0: 3239 2e38 362c 3231 332e 3933 2922 2f3e  29.86,213.93)"/>
+000012b0: 3c70 6174 6820 643d 224d 3132 2e35 2c32  <path d="M12.5,2
+000012c0: 302e 354c 2e33 2c32 302e 3543 2d31 2e34  0.5L.3,20.5C-1.4
+000012d0: 2c32 302e 352c 2d32 2e37 2c31 392e 312c  ,20.5,-2.7,19.1,
+000012e0: 2d32 2e37 2c31 372e 354c 2d32 2e37 2c2d  -2.7,17.5L-2.7,-
+000012f0: 3131 2e35 432d 322e 372c 2d31 332e 312c  11.5C-2.7,-13.1,
+00001300: 2d32 2e35 2c2d 3135 2e36 2c2d 332e 342c  -2.5,-15.6,-3.4,
+00001310: 2d31 372e 3443 2d34 2e35 2c2d 3139 2e32  -17.4C-4.5,-19.2
+00001320: 2c2d 362e 342c 2d32 302e 352c 2d38 2e37  ,-6.4,-20.5,-8.7
+00001330: 2c2d 3230 2e35 4c2d 3132 2e35 2c2d 3230  ,-20.5L-12.5,-20
+00001340: 2e35 2220 7374 726f 6b65 2d6c 696e 6563  .5" stroke-linec
+00001350: 6170 3d22 726f 756e 6422 2069 643d 2273  ap="round" id="s
+00001360: 6861 7065 3139 2220 7374 726f 6b65 3d22  hape19" stroke="
+00001370: 2334 3534 3534 3522 2073 7472 6f6b 652d  #454545" stroke-
+00001380: 7769 6474 683d 2234 2220 6669 6c6c 3d22  width="4" fill="
+00001390: 6e6f 6e65 2220 7472 616e 7366 6f72 6d3d  none" transform=
+000013a0: 2274 7261 6e73 6c61 7465 2831 3332 2e38  "translate(132.8
+000013b0: 362c 3331 342e 3431 2922 2f3e 3c70 6174  6,314.41)"/><pat
+000013c0: 6820 643d 224d 3132 2e35 2c2e 304c 2e33  h d="M12.5,.0L.3
+000013d0: 2c2e 3043 2d31 2e34 2c2e 302c 2d33 2e37  ,.0C-1.4,.0,-3.7
+000013e0: 2c2e 302c 2d35 2e37 2c2e 3043 2d36 2e36  ,.0,-5.7,.0C-6.6
+000013f0: 2c2e 302c 2d37 2e36 2c2e 302c 2d38 2e37  ,.0,-7.6,.0,-8.7
+00001400: 2c2e 304c 2d31 322e 352c 2e30 2220 7374  ,.0L-12.5,.0" st
+00001410: 726f 6b65 2d6c 696e 6563 6170 3d22 726f  roke-linecap="ro
+00001420: 756e 6422 2069 643d 2273 6861 7065 3230  und" id="shape20
+00001430: 2220 7374 726f 6b65 3d22 2334 3534 3534  " stroke="#45454
+00001440: 3522 2073 7472 6f6b 652d 7769 6474 683d  5" stroke-width=
+00001450: 2234 2220 6669 6c6c 3d22 6e6f 6e65 2220  "4" fill="none" 
+00001460: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00001470: 6c61 7465 2831 3332 2e38 362c 3333 342e  late(132.86,334.
+00001480: 3839 2922 2f3e 3c70 6174 6820 643d 224d  89)"/><path d="M
+00001490: 3132 2e35 2c2d 3230 2e35 4c2e 332c 2d32  12.5,-20.5L.3,-2
+000014a0: 302e 3543 2d31 2e34 2c2d 3230 2e35 2c2d  0.5C-1.4,-20.5,-
+000014b0: 322e 372c 2d31 392e 312c 2d32 2e37 2c2d  2.7,-19.1,-2.7,-
+000014c0: 3137 2e35 4c2d 322e 372c 3131 2e35 432d  17.5L-2.7,11.5C-
+000014d0: 322e 372c 3133 2e31 2c2d 322e 352c 3135  2.7,13.1,-2.5,15
+000014e0: 2e36 2c2d 332e 342c 3137 2e34 432d 342e  .6,-3.4,17.4C-4.
+000014f0: 352c 3139 2e32 2c2d 362e 342c 3230 2e35  5,19.2,-6.4,20.5
+00001500: 2c2d 382e 372c 3230 2e35 4c2d 3132 2e35  ,-8.7,20.5L-12.5
+00001510: 2c32 302e 3522 2073 7472 6f6b 652d 6c69  ,20.5" stroke-li
+00001520: 6e65 6361 703d 2272 6f75 6e64 2220 6964  necap="round" id
+00001530: 3d22 7368 6170 6532 3122 2073 7472 6f6b  ="shape21" strok
+00001540: 653d 2223 3435 3435 3435 2220 7374 726f  e="#454545" stro
+00001550: 6b65 2d77 6964 7468 3d22 3422 2066 696c  ke-width="4" fil
+00001560: 6c3d 226e 6f6e 6522 2074 7261 6e73 666f  l="none" transfo
+00001570: 726d 3d22 7472 616e 736c 6174 6528 3133  rm="translate(13
+00001580: 322e 3836 2c33 3535 2e33 3629 222f 3e3c  2.86,355.36)"/><
+00001590: 7061 7468 2064 3d22 4d31 322e 352c 2e30  path d="M12.5,.0
+000015a0: 4c2e 332c 2e30 432d 312e 342c 2e30 2c2d  L.3,.0C-1.4,.0,-
+000015b0: 332e 372c 2e30 2c2d 352e 372c 2e30 432d  3.7,.0,-5.7,.0C-
+000015c0: 362e 362c 2e30 2c2d 372e 362c 2e30 2c2d  6.6,.0,-7.6,.0,-
+000015d0: 382e 372c 2e30 4c2d 3132 2e35 2c2e 3022  8.7,.0L-12.5,.0"
+000015e0: 2073 7472 6f6b 652d 6c69 6e65 6361 703d   stroke-linecap=
+000015f0: 2272 6f75 6e64 2220 6964 3d22 7368 6170  "round" id="shap
+00001600: 6532 3222 2073 7472 6f6b 653d 2223 3435  e22" stroke="#45
+00001610: 3435 3435 2220 7374 726f 6b65 2d77 6964  4545" stroke-wid
+00001620: 7468 3d22 3422 2066 696c 6c3d 226e 6f6e  th="4" fill="non
+00001630: 6522 2074 7261 6e73 666f 726d 3d22 7472  e" transform="tr
+00001640: 616e 736c 6174 6528 3231 332e 3836 2c34  anslate(213.86,4
+00001650: 3832 2e30 3429 222f 3e3c 7061 7468 2064  82.04)"/><path d
+00001660: 3d22 4d31 322e 352c 2d32 302e 354c 2e33  ="M12.5,-20.5L.3
+00001670: 2c2d 3230 2e35 432d 312e 342c 2d32 302e  ,-20.5C-1.4,-20.
+00001680: 352c 2d32 2e37 2c2d 3139 2e31 2c2d 322e  5,-2.7,-19.1,-2.
+00001690: 372c 2d31 372e 354c 2d32 2e37 2c31 312e  7,-17.5L-2.7,11.
+000016a0: 3543 2d32 2e37 2c31 332e 312c 2d32 2e35  5C-2.7,13.1,-2.5
+000016b0: 2c31 352e 362c 2d33 2e34 2c31 372e 3443  ,15.6,-3.4,17.4C
+000016c0: 2d34 2e35 2c31 392e 322c 2d36 2e34 2c32  -4.5,19.2,-6.4,2
+000016d0: 302e 352c 2d38 2e37 2c32 302e 354c 2d31  0.5,-8.7,20.5L-1
+000016e0: 322e 352c 3230 2e35 2220 7374 726f 6b65  2.5,20.5" stroke
+000016f0: 2d6c 696e 6563 6170 3d22 726f 756e 6422  -linecap="round"
+00001700: 2069 643d 2273 6861 7065 3233 2220 7374   id="shape23" st
+00001710: 726f 6b65 3d22 2334 3534 3534 3522 2073  roke="#454545" s
+00001720: 7472 6f6b 652d 7769 6474 683d 2234 2220  troke-width="4" 
+00001730: 6669 6c6c 3d22 6e6f 6e65 2220 7472 616e  fill="none" tran
+00001740: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00001750: 2832 3133 2e38 362c 3530 322e 3531 2922  (213.86,502.51)"
+00001760: 2f3e 3c70 6174 6820 643d 224d 2d31 332e  /><path d="M-13.
+00001770: 312c 3937 2e33 4c2d 3336 2e37 2c39 372e  1,97.3L-36.7,97.
+00001780: 3343 2d33 382e 342c 3937 2e33 2c2d 3339  3C-38.4,97.3,-39
+00001790: 2e37 2c39 352e 392c 2d33 392e 372c 3934  .7,95.9,-39.7,94
+000017a0: 2e33 4c2d 3339 2e37 2c2d 3838 2e33 432d  .3L-39.7,-88.3C-
+000017b0: 3339 2e37 2c2d 3839 2e39 2c2d 3339 2e35  39.7,-89.9,-39.5
+000017c0: 2c2d 3932 2e34 2c2d 3430 2e34 2c2d 3934  ,-92.4,-40.4,-94
+000017d0: 2e31 432d 3431 2e35 2c2d 3936 2e30 2c2d  .1C-41.5,-96.0,-
+000017e0: 3433 2e34 2c2d 3937 2e33 2c2d 3435 2e37  43.4,-97.3,-45.7
+000017f0: 2c2d 3937 2e33 4c2d 3736 2e31 2c2d 3937  ,-97.3L-76.1,-97
+00001800: 2e33 2220 7374 726f 6b65 2d6c 696e 6563  .3" stroke-linec
+00001810: 6170 3d22 726f 756e 6422 2069 643d 2273  ap="round" id="s
+00001820: 6861 7065 3234 2220 7374 726f 6b65 3d22  hape24" stroke="
+00001830: 2334 3534 3534 3522 2073 7472 6f6b 652d  #454545" stroke-
+00001840: 7769 6474 683d 2234 2220 6669 6c6c 3d22  width="4" fill="
+00001850: 6e6f 6e65 2220 7472 616e 7366 6f72 6d3d  none" transform=
+00001860: 2274 7261 6e73 6c61 7465 2833 3831 2e34  "translate(381.4
+00001870: 372c 3139 302e 3233 2922 2f3e 3c70 6174  7,190.23)"/><pat
+00001880: 6820 643d 224d 3132 2e35 2c31 302e 3243  h d="M12.5,10.2C
+00001890: 2e31 2c31 302e 322c 2e35 2c2d 3130 2e32  .1,10.2,.5,-10.2
+000018a0: 2c2d 3132 2e35 2c2d 3130 2e32 2220 7374  ,-12.5,-10.2" st
+000018b0: 726f 6b65 2d6c 696e 6563 6170 3d22 726f  roke-linecap="ro
+000018c0: 756e 6422 2069 643d 2273 6861 7065 3235  und" id="shape25
+000018d0: 2220 7374 726f 6b65 3d22 2334 3534 3534  " stroke="#45454
+000018e0: 3522 2073 7472 6f6b 652d 7769 6474 683d  5" stroke-width=
+000018f0: 2234 2220 6669 6c6c 3d22 6e6f 6e65 2220  "4" fill="none" 
+00001900: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00001910: 6c61 7465 2831 3437 2e38 362c 3832 2e37  late(147.86,82.7
+00001920: 3329 222f 3e3c 7061 7468 2064 3d22 4d31  3)"/><path d="M1
+00001930: 322e 352c 2d31 302e 3243 2e31 2c2d 3130  2.5,-10.2C.1,-10
+00001940: 2e32 2c2e 352c 3130 2e32 2c2d 3132 2e35  .2,.5,10.2,-12.5
+00001950: 2c31 302e 3222 2073 7472 6f6b 652d 6c69  ,10.2" stroke-li
+00001960: 6e65 6361 703d 2272 6f75 6e64 2220 6964  necap="round" id
+00001970: 3d22 7368 6170 6532 3622 2073 7472 6f6b  ="shape26" strok
+00001980: 653d 2223 3435 3435 3435 2220 7374 726f  e="#454545" stro
+00001990: 6b65 2d77 6964 7468 3d22 3422 2066 696c  ke-width="4" fil
+000019a0: 6c3d 226e 6f6e 6522 2074 7261 6e73 666f  l="none" transfo
+000019b0: 726d 3d22 7472 616e 736c 6174 6528 3134  rm="translate(14
+000019c0: 372e 3836 2c31 3033 2e32 3029 222f 3e3c  7.86,103.20)"/><
+000019d0: 6720 6964 3d22 7368 6170 6532 3722 2074  g id="shape27" t
+000019e0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+000019f0: 6174 6528 3336 382e 3336 3130 3030 2c32  ate(368.361000,2
+00001a00: 3533 2e30 3030 3030 3029 223e 3c70 6174  53.000000)"><pat
+00001a10: 6820 643d 224d 3334 2e35 2c2e 304c 3134  h d="M34.5,.0L14
+00001a20: 332e 392c 2e30 4331 3633 2e30 2c2e 302c  3.9,.0C163.0,.0,
+00001a30: 3137 382e 342c 3135 2e34 2c31 3738 2e34  178.4,15.4,178.4
+00001a40: 2c33 342e 3543 3137 382e 342c 3533 2e36  ,34.5C178.4,53.6
+00001a50: 2c31 3633 2e30 2c36 392e 302c 3134 332e  ,163.0,69.0,143.
+00001a60: 392c 3639 2e30 4c33 342e 352c 3639 2e30  9,69.0L34.5,69.0
+00001a70: 4331 352e 342c 3639 2e30 2c2e 302c 3533  C15.4,69.0,.0,53
+00001a80: 2e36 2c2e 302c 3334 2e35 432e 302c 3135  .6,.0,34.5C.0,15
+00001a90: 2e34 2c31 352e 342c 2e30 2c33 342e 352c  .4,15.4,.0,34.5,
+00001aa0: 2e30 7a22 2073 7472 6f6b 653d 2223 3330  .0z" stroke="#30
+00001ab0: 3330 3330 2220 7374 726f 6b65 2d77 6964  3030" stroke-wid
+00001ac0: 7468 3d22 3422 2066 696c 6c2d 7275 6c65  th="4" fill-rule
+00001ad0: 3d22 6e6f 6e7a 6572 6f22 2066 696c 6c3d  ="nonzero" fill=
+00001ae0: 2223 3030 3533 6436 222f 3e3c 7465 7874  "#0053d6"/><text
+00001af0: 2073 7479 6c65 3d22 6669 6c6c 3a23 6666   style="fill:#ff
+00001b00: 6666 6666 3b66 6f6e 742d 6661 6d69 6c79  ffff;font-family
+00001b10: 3ae5 beae e8bd afe9 9b85 e9bb 913b 666f  :............;fo
+00001b20: 6e74 2d73 697a 653a 3138 2e30 3070 743b  nt-size:18.00pt;
+00001b30: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
+00001b40: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
+00001b50: 7365 7276 6522 3e3c 7473 7061 6e20 793d  serve"><tspan y=
+00001b60: 2234 342e 3022 2078 3d22 3334 2e30 223e  "44.0" x="34.0">
 00001b70: 4873 7561 6e77 753c 2f74 7370 616e 3e3c  Hsuanwu</tspan><
-00001b80: 2f74 6578 743e 3c2f 673e 3c67 2074 7261  /text></g><g tra
-00001b90: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-00001ba0: 6528 3630 392e 3830 3130 3030 2c32 3632  e(609.801000,262
-00001bb0: 2e35 3030 3030 3029 2220 6964 3d22 7368  .500000)" id="sh
-00001bc0: 6170 6532 3822 3e3c 7061 7468 2066 696c  ape28"><path fil
-00001bd0: 6c2d 7275 6c65 3d22 6e6f 6e7a 6572 6f22  l-rule="nonzero"
-00001be0: 2073 7472 6f6b 653d 2223 3435 3435 3435   stroke="#454545
-00001bf0: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
-00001c00: 3422 2066 696c 6c3d 2223 6666 6666 6666  4" fill="#ffffff
-00001c10: 2220 643d 224d 342e 302c 2e30 4c39 392e  " d="M4.0,.0L99.
-00001c20: 302c 2e30 4331 3031 2e32 2c2e 302c 3130  0,.0C101.2,.0,10
-00001c30: 332e 302c 312e 382c 3130 332e 302c 342e  3.0,1.8,103.0,4.
-00001c40: 304c 3130 332e 302c 3436 2e30 4331 3033  0L103.0,46.0C103
-00001c50: 2e30 2c34 382e 322c 3130 312e 322c 3530  .0,48.2,101.2,50
-00001c60: 2e30 2c39 392e 302c 3530 2e30 4c34 2e30  .0,99.0,50.0L4.0
-00001c70: 2c35 302e 3043 312e 382c 3530 2e30 2c2e  ,50.0C1.8,50.0,.
-00001c80: 302c 3438 2e32 2c2e 302c 3436 2e30 4c2e  0,48.2,.0,46.0L.
-00001c90: 302c 342e 3043 2e30 2c31 2e38 2c31 2e38  0,4.0C.0,1.8,1.8
-00001ca0: 2c2e 302c 342e 302c 2e30 7a22 2f3e 3c74  ,.0,4.0,.0z"/><t
-00001cb0: 6578 7420 786d 6c3a 7370 6163 653d 2270  ext xml:space="p
-00001cc0: 7265 7365 7276 6522 2073 7479 6c65 3d22  reserve" style="
-00001cd0: 6669 6c6c 3a23 3330 3330 3330 3b66 6f6e  fill:#303030;fon
-00001ce0: 742d 6661 6d69 6c79 3ae5 beae e8bd afe9  t-family:.......
-00001cf0: 9b85 e9bb 913b 666f 6e74 2d73 697a 653a  .....;font-size:
-00001d00: 3134 2e30 3070 743b 666f 6e74 2d77 6569  14.00pt;font-wei
-00001d10: 6768 743a 626f 6c64 223e 3c74 7370 616e  ght:bold"><tspan
-00001d20: 2078 3d22 3234 2e33 2220 793d 2233 322e   x="24.3" y="32.
-00001d30: 3022 3e58 706c 6f69 743c 2f74 7370 616e  0">Xploit</tspan
-00001d40: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2074  ></text></g><g t
-00001d50: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00001d60: 6174 6528 3630 392e 3830 3130 3030 2c31  ate(609.801000,1
-00001d70: 3135 2e33 3530 3030 3029 2220 6964 3d22  15.350000)" id="
-00001d80: 7368 6170 6532 3922 3e3c 7061 7468 2066  shape29"><path f
-00001d90: 696c 6c2d 7275 6c65 3d22 6e6f 6e7a 6572  ill-rule="nonzer
-00001da0: 6f22 2073 7472 6f6b 653d 2223 3435 3435  o" stroke="#4545
-00001db0: 3435 2220 7374 726f 6b65 2d77 6964 7468  45" stroke-width
-00001dc0: 3d22 3422 2066 696c 6c3d 2223 6666 6666  ="4" fill="#ffff
-00001dd0: 6666 2220 643d 224d 342e 302c 2e30 4c31  ff" d="M4.0,.0L1
-00001de0: 3034 2e30 2c2e 3043 3130 362e 322c 2e30  04.0,.0C106.2,.0
-00001df0: 2c31 3038 2e30 2c31 2e38 2c31 3038 2e30  ,108.0,1.8,108.0
-00001e00: 2c34 2e30 4c31 3038 2e30 2c34 362e 3043  ,4.0L108.0,46.0C
-00001e10: 3130 382e 302c 3438 2e32 2c31 3036 2e32  108.0,48.2,106.2
-00001e20: 2c35 302e 302c 3130 342e 302c 3530 2e30  ,50.0,104.0,50.0
-00001e30: 4c34 2e30 2c35 302e 3043 312e 382c 3530  L4.0,50.0C1.8,50
-00001e40: 2e30 2c2e 302c 3438 2e32 2c2e 302c 3436  .0,.0,48.2,.0,46
-00001e50: 2e30 4c2e 302c 342e 3043 2e30 2c31 2e38  .0L.0,4.0C.0,1.8
-00001e60: 2c31 2e38 2c2e 302c 342e 302c 2e30 7a22  ,1.8,.0,4.0,.0z"
-00001e70: 2f3e 3c74 6578 7420 786d 6c3a 7370 6163  /><text xml:spac
-00001e80: 653d 2270 7265 7365 7276 6522 2073 7479  e="preserve" sty
-00001e90: 6c65 3d22 6669 6c6c 3a23 3330 3330 3330  le="fill:#303030
-00001ea0: 3b66 6f6e 742d 6661 6d69 6c79 3ae5 beae  ;font-family:...
-00001eb0: e8bd afe9 9b85 e9bb 913b 666f 6e74 2d73  .........;font-s
-00001ec0: 697a 653a 3134 2e30 3070 743b 666f 6e74  ize:14.00pt;font
-00001ed0: 2d77 6569 6768 743a 626f 6c64 223e 3c74  -weight:bold"><t
-00001ee0: 7370 616e 2078 3d22 3234 2e33 2220 793d  span x="24.3" y=
-00001ef0: 2233 322e 3022 3e58 706c 6f72 653c 2f74  "32.0">Xplore</t
+00001b80: 2f74 6578 743e 3c2f 673e 3c67 2069 643d  /text></g><g id=
+00001b90: 2273 6861 7065 3238 2220 7472 616e 7366  "shape28" transf
+00001ba0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2836  orm="translate(6
+00001bb0: 3039 2e38 3031 3030 302c 3236 322e 3530  09.801000,262.50
+00001bc0: 3030 3030 2922 3e3c 7061 7468 2064 3d22  0000)"><path d="
+00001bd0: 4d34 2e30 2c2e 304c 3939 2e30 2c2e 3043  M4.0,.0L99.0,.0C
+00001be0: 3130 312e 322c 2e30 2c31 3033 2e30 2c31  101.2,.0,103.0,1
+00001bf0: 2e38 2c31 3033 2e30 2c34 2e30 4c31 3033  .8,103.0,4.0L103
+00001c00: 2e30 2c34 362e 3043 3130 332e 302c 3438  .0,46.0C103.0,48
+00001c10: 2e32 2c31 3031 2e32 2c35 302e 302c 3939  .2,101.2,50.0,99
+00001c20: 2e30 2c35 302e 304c 342e 302c 3530 2e30  .0,50.0L4.0,50.0
+00001c30: 4331 2e38 2c35 302e 302c 2e30 2c34 382e  C1.8,50.0,.0,48.
+00001c40: 322c 2e30 2c34 362e 304c 2e30 2c34 2e30  2,.0,46.0L.0,4.0
+00001c50: 432e 302c 312e 382c 312e 382c 2e30 2c34  C.0,1.8,1.8,.0,4
+00001c60: 2e30 2c2e 307a 2220 7374 726f 6b65 3d22  .0,.0z" stroke="
+00001c70: 2334 3534 3534 3522 2073 7472 6f6b 652d  #454545" stroke-
+00001c80: 7769 6474 683d 2234 2220 6669 6c6c 2d72  width="4" fill-r
+00001c90: 756c 653d 226e 6f6e 7a65 726f 2220 6669  ule="nonzero" fi
+00001ca0: 6c6c 3d22 2366 6666 6666 6622 2f3e 3c74  ll="#ffffff"/><t
+00001cb0: 6578 7420 7374 796c 653d 2266 696c 6c3a  ext style="fill:
+00001cc0: 2333 3033 3033 303b 666f 6e74 2d66 616d  #303030;font-fam
+00001cd0: 696c 793a e5be aee8 bdaf e99b 85e9 bb91  ily:............
+00001ce0: 3b66 6f6e 742d 7369 7a65 3a31 342e 3030  ;font-size:14.00
+00001cf0: 7074 3b66 6f6e 742d 7765 6967 6874 3a62  pt;font-weight:b
+00001d00: 6f6c 6422 2078 6d6c 3a73 7061 6365 3d22  old" xml:space="
+00001d10: 7072 6573 6572 7665 223e 3c74 7370 616e  preserve"><tspan
+00001d20: 2079 3d22 3332 2e30 2220 783d 2232 342e   y="32.0" x="24.
+00001d30: 3322 3e58 706c 6f69 743c 2f74 7370 616e  3">Xploit</tspan
+00001d40: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2069  ></text></g><g i
+00001d50: 643d 2273 6861 7065 3239 2220 7472 616e  d="shape29" tran
+00001d60: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00001d70: 2836 3039 2e38 3031 3030 302c 3131 352e  (609.801000,115.
+00001d80: 3335 3030 3030 2922 3e3c 7061 7468 2064  350000)"><path d
+00001d90: 3d22 4d34 2e30 2c2e 304c 3130 342e 302c  ="M4.0,.0L104.0,
+00001da0: 2e30 4331 3036 2e32 2c2e 302c 3130 382e  .0C106.2,.0,108.
+00001db0: 302c 312e 382c 3130 382e 302c 342e 304c  0,1.8,108.0,4.0L
+00001dc0: 3130 382e 302c 3436 2e30 4331 3038 2e30  108.0,46.0C108.0
+00001dd0: 2c34 382e 322c 3130 362e 322c 3530 2e30  ,48.2,106.2,50.0
+00001de0: 2c31 3034 2e30 2c35 302e 304c 342e 302c  ,104.0,50.0L4.0,
+00001df0: 3530 2e30 4331 2e38 2c35 302e 302c 2e30  50.0C1.8,50.0,.0
+00001e00: 2c34 382e 322c 2e30 2c34 362e 304c 2e30  ,48.2,.0,46.0L.0
+00001e10: 2c34 2e30 432e 302c 312e 382c 312e 382c  ,4.0C.0,1.8,1.8,
+00001e20: 2e30 2c34 2e30 2c2e 307a 2220 7374 726f  .0,4.0,.0z" stro
+00001e30: 6b65 3d22 2334 3534 3534 3522 2073 7472  ke="#454545" str
+00001e40: 6f6b 652d 7769 6474 683d 2234 2220 6669  oke-width="4" fi
+00001e50: 6c6c 2d72 756c 653d 226e 6f6e 7a65 726f  ll-rule="nonzero
+00001e60: 2220 6669 6c6c 3d22 2366 6666 6666 6622  " fill="#ffffff"
+00001e70: 2f3e 3c74 6578 7420 7374 796c 653d 2266  /><text style="f
+00001e80: 696c 6c3a 2333 3033 3033 303b 666f 6e74  ill:#303030;font
+00001e90: 2d66 616d 696c 793a e5be aee8 bdaf e99b  -family:........
+00001ea0: 85e9 bb91 3b66 6f6e 742d 7369 7a65 3a31  ....;font-size:1
+00001eb0: 342e 3030 7074 3b66 6f6e 742d 7765 6967  4.00pt;font-weig
+00001ec0: 6874 3a62 6f6c 6422 2078 6d6c 3a73 7061  ht:bold" xml:spa
+00001ed0: 6365 3d22 7072 6573 6572 7665 223e 3c74  ce="preserve"><t
+00001ee0: 7370 616e 2079 3d22 3332 2e30 2220 783d  span y="32.0" x=
+00001ef0: 2232 342e 3322 3e58 706c 6f72 653c 2f74  "24.3">Xplore</t
 00001f00: 7370 616e 3e3c 2f74 6578 743e 3c2f 673e  span></text></g>
-00001f10: 3c67 2074 7261 6e73 666f 726d 3d22 7472  <g transform="tr
-00001f20: 616e 736c 6174 6528 3630 392e 3830 3130  anslate(609.8010
-00001f30: 3030 2c34 3039 2e36 3530 3030 3029 2220  00,409.650000)" 
-00001f40: 6964 3d22 7368 6170 6533 3022 3e3c 7061  id="shape30"><pa
-00001f50: 7468 2066 696c 6c2d 7275 6c65 3d22 6e6f  th fill-rule="no
-00001f60: 6e7a 6572 6f22 2073 7472 6f6b 653d 2223  nzero" stroke="#
-00001f70: 3435 3435 3435 2220 7374 726f 6b65 2d77  454545" stroke-w
-00001f80: 6964 7468 3d22 3422 2066 696c 6c3d 2223  idth="4" fill="#
-00001f90: 6666 6666 6666 2220 643d 224d 342e 302c  ffffff" d="M4.0,
-00001fa0: 2e30 4c31 3238 2e30 2c2e 3043 3133 302e  .0L128.0,.0C130.
-00001fb0: 322c 2e30 2c31 3332 2e30 2c31 2e38 2c31  2,.0,132.0,1.8,1
-00001fc0: 3332 2e30 2c34 2e30 4c31 3332 2e30 2c34  32.0,4.0L132.0,4
-00001fd0: 362e 3043 3133 322e 302c 3438 2e32 2c31  6.0C132.0,48.2,1
-00001fe0: 3330 2e32 2c35 302e 302c 3132 382e 302c  30.2,50.0,128.0,
-00001ff0: 3530 2e30 4c34 2e30 2c35 302e 3043 312e  50.0L4.0,50.0C1.
-00002000: 382c 3530 2e30 2c2e 302c 3438 2e32 2c2e  8,50.0,.0,48.2,.
-00002010: 302c 3436 2e30 4c2e 302c 342e 3043 2e30  0,46.0L.0,4.0C.0
-00002020: 2c31 2e38 2c31 2e38 2c2e 302c 342e 302c  ,1.8,1.8,.0,4.0,
-00002030: 2e30 7a22 2f3e 3c74 6578 7420 786d 6c3a  .0z"/><text xml:
-00002040: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
-00002050: 2073 7479 6c65 3d22 6669 6c6c 3a23 3330   style="fill:#30
-00002060: 3330 3330 3b66 6f6e 742d 6661 6d69 6c79  3030;font-family
-00002070: 3ae5 beae e8bd afe9 9b85 e9bb 913b 666f  :............;fo
-00002080: 6e74 2d73 697a 653a 3134 2e30 3070 743b  nt-size:14.00pt;
-00002090: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
-000020a0: 223e 3c74 7370 616e 2078 3d22 3234 2e33  "><tspan x="24.3
-000020b0: 2220 793d 2233 322e 3022 3e43 6f6d 6d6f  " y="32.0">Commo
+00001f10: 3c67 2069 643d 2273 6861 7065 3330 2220  <g id="shape30" 
+00001f20: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00001f30: 6c61 7465 2836 3039 2e38 3031 3030 302c  late(609.801000,
+00001f40: 3430 392e 3635 3030 3030 2922 3e3c 7061  409.650000)"><pa
+00001f50: 7468 2064 3d22 4d34 2e30 2c2e 304c 3132  th d="M4.0,.0L12
+00001f60: 382e 302c 2e30 4331 3330 2e32 2c2e 302c  8.0,.0C130.2,.0,
+00001f70: 3133 322e 302c 312e 382c 3133 322e 302c  132.0,1.8,132.0,
+00001f80: 342e 304c 3133 322e 302c 3436 2e30 4331  4.0L132.0,46.0C1
+00001f90: 3332 2e30 2c34 382e 322c 3133 302e 322c  32.0,48.2,130.2,
+00001fa0: 3530 2e30 2c31 3238 2e30 2c35 302e 304c  50.0,128.0,50.0L
+00001fb0: 342e 302c 3530 2e30 4331 2e38 2c35 302e  4.0,50.0C1.8,50.
+00001fc0: 302c 2e30 2c34 382e 322c 2e30 2c34 362e  0,.0,48.2,.0,46.
+00001fd0: 304c 2e30 2c34 2e30 432e 302c 312e 382c  0L.0,4.0C.0,1.8,
+00001fe0: 312e 382c 2e30 2c34 2e30 2c2e 307a 2220  1.8,.0,4.0,.0z" 
+00001ff0: 7374 726f 6b65 3d22 2334 3534 3534 3522  stroke="#454545"
+00002000: 2073 7472 6f6b 652d 7769 6474 683d 2234   stroke-width="4
+00002010: 2220 6669 6c6c 2d72 756c 653d 226e 6f6e  " fill-rule="non
+00002020: 7a65 726f 2220 6669 6c6c 3d22 2366 6666  zero" fill="#fff
+00002030: 6666 6622 2f3e 3c74 6578 7420 7374 796c  fff"/><text styl
+00002040: 653d 2266 696c 6c3a 2333 3033 3033 303b  e="fill:#303030;
+00002050: 666f 6e74 2d66 616d 696c 793a e5be aee8  font-family:....
+00002060: bdaf e99b 85e9 bb91 3b66 6f6e 742d 7369  ........;font-si
+00002070: 7a65 3a31 342e 3030 7074 3b66 6f6e 742d  ze:14.00pt;font-
+00002080: 7765 6967 6874 3a62 6f6c 6422 2078 6d6c  weight:bold" xml
+00002090: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
+000020a0: 223e 3c74 7370 616e 2079 3d22 3332 2e30  "><tspan y="32.0
+000020b0: 2220 783d 2232 342e 3322 3e43 6f6d 6d6f  " x="24.3">Commo
 000020c0: 6e3c 2f74 7370 616e 3e3c 2f74 6578 743e  n</tspan></text>
-000020d0: 3c2f 673e 3c67 2074 7261 6e73 666f 726d  </g><g transform
-000020e0: 3d22 7472 616e 736c 6174 6528 3733 372e  ="translate(737.
-000020f0: 3830 3130 3030 2c32 3134 2e33 3030 3030  801000,214.30000
-00002100: 3029 2220 6964 3d22 7368 6170 6533 3122  0)" id="shape31"
-00002110: 3e3c 7061 7468 2066 696c 6c2d 7275 6c65  ><path fill-rule
-00002120: 3d22 6e6f 6e7a 6572 6f22 2066 696c 6c3d  ="nonzero" fill=
-00002130: 2223 6666 6666 6666 2220 643d 224d 2e30  "#ffffff" d="M.0
-00002140: 2c2e 304c 3835 2e30 2c2e 304c 3835 2e30  ,.0L85.0,.0L85.0
-00002150: 2c33 322e 334c 2e30 2c33 322e 334c 2e30  ,32.3L.0,32.3L.0
-00002160: 2c2e 307a 222f 3e3c 7061 7468 2073 7472  ,.0z"/><path str
-00002170: 6f6b 653d 2223 3435 3435 3435 2220 7374  oke="#454545" st
-00002180: 726f 6b65 2d77 6964 7468 3d22 3422 2066  roke-width="4" f
-00002190: 696c 6c3d 226e 6f6e 6522 2064 3d22 4d2e  ill="none" d="M.
-000021a0: 302c 3332 2e33 4c38 352e 302c 3332 2e33  0,32.3L85.0,32.3
-000021b0: 222f 3e3c 7465 7874 2078 6d6c 3a73 7061  "/><text xml:spa
-000021c0: 6365 3d22 7072 6573 6572 7665 2220 7374  ce="preserve" st
-000021d0: 796c 653d 2266 696c 6c3a 2333 3033 3033  yle="fill:#30303
-000021e0: 303b 666f 6e74 2d66 616d 696c 793a e5be  0;font-family:..
-000021f0: aee8 bdaf e99b 85e9 bb91 3b66 6f6e 742d  ..........;font-
-00002200: 7369 7a65 3a31 312e 3030 7074 3b66 6f6e  size:11.00pt;fon
-00002210: 742d 7765 6967 6874 3a62 6f6c 6422 3e3c  t-weight:bold"><
-00002220: 7473 7061 6e20 783d 2231 322e 3922 2079  tspan x="12.9" y
-00002230: 3d22 3230 2e39 223e 456e 636f 6465 723c  ="20.9">Encoder<
+000020d0: 3c2f 673e 3c67 2069 643d 2273 6861 7065  </g><g id="shape
+000020e0: 3331 2220 7472 616e 7366 6f72 6d3d 2274  31" transform="t
+000020f0: 7261 6e73 6c61 7465 2837 3337 2e38 3031  ranslate(737.801
+00002100: 3030 302c 3231 342e 3330 3030 3030 2922  000,214.300000)"
+00002110: 3e3c 7061 7468 2064 3d22 4d2e 302c 2e30  ><path d="M.0,.0
+00002120: 4c38 352e 302c 2e30 4c38 352e 302c 3332  L85.0,.0L85.0,32
+00002130: 2e33 4c2e 302c 3332 2e33 4c2e 302c 2e30  .3L.0,32.3L.0,.0
+00002140: 7a22 2066 696c 6c2d 7275 6c65 3d22 6e6f  z" fill-rule="no
+00002150: 6e7a 6572 6f22 2066 696c 6c3d 2223 6666  nzero" fill="#ff
+00002160: 6666 6666 222f 3e3c 7061 7468 2064 3d22  ffff"/><path d="
+00002170: 4d2e 302c 3332 2e33 4c38 352e 302c 3332  M.0,32.3L85.0,32
+00002180: 2e33 2220 7374 726f 6b65 3d22 2334 3534  .3" stroke="#454
+00002190: 3534 3522 2073 7472 6f6b 652d 7769 6474  545" stroke-widt
+000021a0: 683d 2234 2220 6669 6c6c 3d22 6e6f 6e65  h="4" fill="none
+000021b0: 222f 3e3c 7465 7874 2073 7479 6c65 3d22  "/><text style="
+000021c0: 6669 6c6c 3a23 3330 3330 3330 3b66 6f6e  fill:#303030;fon
+000021d0: 742d 6661 6d69 6c79 3ae5 beae e8bd afe9  t-family:.......
+000021e0: 9b85 e9bb 913b 666f 6e74 2d73 697a 653a  .....;font-size:
+000021f0: 3131 2e30 3070 743b 666f 6e74 2d77 6569  11.00pt;font-wei
+00002200: 6768 743a 626f 6c64 2220 786d 6c3a 7370  ght:bold" xml:sp
+00002210: 6163 653d 2270 7265 7365 7276 6522 3e3c  ace="preserve"><
+00002220: 7473 7061 6e20 793d 2232 302e 3922 2078  tspan y="20.9" x
+00002230: 3d22 3132 2e39 223e 456e 636f 6465 723c  ="12.9">Encoder<
 00002240: 2f74 7370 616e 3e3c 2f74 6578 743e 3c2f  /tspan></text></
-00002250: 673e 3c67 2074 7261 6e73 666f 726d 3d22  g><g transform="
-00002260: 7472 616e 736c 6174 6528 3733 372e 3830  translate(737.80
-00002270: 3130 3030 2c32 3535 2e32 3530 3030 3029  1000,255.250000)
-00002280: 2220 6964 3d22 7368 6170 6533 3222 3e3c  " id="shape32"><
-00002290: 7061 7468 2066 696c 6c2d 7275 6c65 3d22  path fill-rule="
-000022a0: 6e6f 6e7a 6572 6f22 2066 696c 6c3d 2223  nonzero" fill="#
-000022b0: 6666 6666 6666 2220 643d 224d 2e30 2c2e  ffffff" d="M.0,.
-000022c0: 304c 3639 2e30 2c2e 304c 3639 2e30 2c33  0L69.0,.0L69.0,3
-000022d0: 322e 334c 2e30 2c33 322e 334c 2e30 2c2e  2.3L.0,32.3L.0,.
-000022e0: 307a 222f 3e3c 7061 7468 2073 7472 6f6b  0z"/><path strok
-000022f0: 653d 2223 3435 3435 3435 2220 7374 726f  e="#454545" stro
-00002300: 6b65 2d77 6964 7468 3d22 3422 2066 696c  ke-width="4" fil
-00002310: 6c3d 226e 6f6e 6522 2064 3d22 4d2e 302c  l="none" d="M.0,
-00002320: 3332 2e33 4c36 392e 302c 3332 2e33 222f  32.3L69.0,32.3"/
-00002330: 3e3c 7465 7874 2078 6d6c 3a73 7061 6365  ><text xml:space
-00002340: 3d22 7072 6573 6572 7665 2220 7374 796c  ="preserve" styl
-00002350: 653d 2266 696c 6c3a 2333 3033 3033 303b  e="fill:#303030;
-00002360: 666f 6e74 2d66 616d 696c 793a e5be aee8  font-family:....
-00002370: bdaf e99b 85e9 bb91 3b66 6f6e 742d 7369  ........;font-si
-00002380: 7a65 3a31 312e 3030 7074 3b66 6f6e 742d  ze:11.00pt;font-
-00002390: 7765 6967 6874 3a62 6f6c 6422 3e3c 7473  weight:bold"><ts
-000023a0: 7061 6e20 783d 2231 322e 3922 2079 3d22  pan x="12.9" y="
-000023b0: 3230 2e39 223e 4167 656e 743c 2f74 7370  20.9">Agent</tsp
+00002250: 673e 3c67 2069 643d 2273 6861 7065 3332  g><g id="shape32
+00002260: 2220 7472 616e 7366 6f72 6d3d 2274 7261  " transform="tra
+00002270: 6e73 6c61 7465 2837 3337 2e38 3031 3030  nslate(737.80100
+00002280: 302c 3235 352e 3235 3030 3030 2922 3e3c  0,255.250000)"><
+00002290: 7061 7468 2064 3d22 4d2e 302c 2e30 4c36  path d="M.0,.0L6
+000022a0: 392e 302c 2e30 4c36 392e 302c 3332 2e33  9.0,.0L69.0,32.3
+000022b0: 4c2e 302c 3332 2e33 4c2e 302c 2e30 7a22  L.0,32.3L.0,.0z"
+000022c0: 2066 696c 6c2d 7275 6c65 3d22 6e6f 6e7a   fill-rule="nonz
+000022d0: 6572 6f22 2066 696c 6c3d 2223 6666 6666  ero" fill="#ffff
+000022e0: 6666 222f 3e3c 7061 7468 2064 3d22 4d2e  ff"/><path d="M.
+000022f0: 302c 3332 2e33 4c36 392e 302c 3332 2e33  0,32.3L69.0,32.3
+00002300: 2220 7374 726f 6b65 3d22 2334 3534 3534  " stroke="#45454
+00002310: 3522 2073 7472 6f6b 652d 7769 6474 683d  5" stroke-width=
+00002320: 2234 2220 6669 6c6c 3d22 6e6f 6e65 222f  "4" fill="none"/
+00002330: 3e3c 7465 7874 2073 7479 6c65 3d22 6669  ><text style="fi
+00002340: 6c6c 3a23 3330 3330 3330 3b66 6f6e 742d  ll:#303030;font-
+00002350: 6661 6d69 6c79 3ae5 beae e8bd afe9 9b85  family:.........
+00002360: e9bb 913b 666f 6e74 2d73 697a 653a 3131  ...;font-size:11
+00002370: 2e30 3070 743b 666f 6e74 2d77 6569 6768  .00pt;font-weigh
+00002380: 743a 626f 6c64 2220 786d 6c3a 7370 6163  t:bold" xml:spac
+00002390: 653d 2270 7265 7365 7276 6522 3e3c 7473  e="preserve"><ts
+000023a0: 7061 6e20 793d 2232 302e 3922 2078 3d22  pan y="20.9" x="
+000023b0: 3132 2e39 223e 4167 656e 743c 2f74 7370  12.9">Agent</tsp
 000023c0: 616e 3e3c 2f74 6578 743e 3c2f 673e 3c67  an></text></g><g
-000023d0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
-000023e0: 736c 6174 6528 3733 372e 3830 3130 3030  slate(737.801000
-000023f0: 2c32 3936 2e32 3030 3030 3029 2220 6964  ,296.200000)" id
-00002400: 3d22 7368 6170 6533 3322 3e3c 7061 7468  ="shape33"><path
-00002410: 2066 696c 6c2d 7275 6c65 3d22 6e6f 6e7a   fill-rule="nonz
-00002420: 6572 6f22 2066 696c 6c3d 2223 6666 6666  ero" fill="#ffff
-00002430: 6666 2220 643d 224d 2e30 2c2e 304c 3832  ff" d="M.0,.0L82
-00002440: 2e30 2c2e 304c 3832 2e30 2c33 322e 334c  .0,.0L82.0,32.3L
-00002450: 2e30 2c33 322e 334c 2e30 2c2e 307a 222f  .0,32.3L.0,.0z"/
-00002460: 3e3c 7061 7468 2073 7472 6f6b 653d 2223  ><path stroke="#
-00002470: 3435 3435 3435 2220 7374 726f 6b65 2d77  454545" stroke-w
-00002480: 6964 7468 3d22 3422 2066 696c 6c3d 226e  idth="4" fill="n
-00002490: 6f6e 6522 2064 3d22 4d2e 302c 3332 2e33  one" d="M.0,32.3
-000024a0: 4c38 322e 302c 3332 2e33 222f 3e3c 7465  L82.0,32.3"/><te
-000024b0: 7874 2078 6d6c 3a73 7061 6365 3d22 7072  xt xml:space="pr
-000024c0: 6573 6572 7665 2220 7374 796c 653d 2266  eserve" style="f
-000024d0: 696c 6c3a 2333 3033 3033 303b 666f 6e74  ill:#303030;font
-000024e0: 2d66 616d 696c 793a e5be aee8 bdaf e99b  -family:........
-000024f0: 85e9 bb91 3b66 6f6e 742d 7369 7a65 3a31  ....;font-size:1
-00002500: 312e 3030 7074 3b66 6f6e 742d 7765 6967  1.00pt;font-weig
-00002510: 6874 3a62 6f6c 6422 3e3c 7473 7061 6e20  ht:bold"><tspan 
-00002520: 783d 2231 322e 3922 2079 3d22 3230 2e39  x="12.9" y="20.9
+000023d0: 2069 643d 2273 6861 7065 3333 2220 7472   id="shape33" tr
+000023e0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+000023f0: 7465 2837 3337 2e38 3031 3030 302c 3239  te(737.801000,29
+00002400: 362e 3230 3030 3030 2922 3e3c 7061 7468  6.200000)"><path
+00002410: 2064 3d22 4d2e 302c 2e30 4c38 322e 302c   d="M.0,.0L82.0,
+00002420: 2e30 4c38 322e 302c 3332 2e33 4c2e 302c  .0L82.0,32.3L.0,
+00002430: 3332 2e33 4c2e 302c 2e30 7a22 2066 696c  32.3L.0,.0z" fil
+00002440: 6c2d 7275 6c65 3d22 6e6f 6e7a 6572 6f22  l-rule="nonzero"
+00002450: 2066 696c 6c3d 2223 6666 6666 6666 222f   fill="#ffffff"/
+00002460: 3e3c 7061 7468 2064 3d22 4d2e 302c 3332  ><path d="M.0,32
+00002470: 2e33 4c38 322e 302c 3332 2e33 2220 7374  .3L82.0,32.3" st
+00002480: 726f 6b65 3d22 2334 3534 3534 3522 2073  roke="#454545" s
+00002490: 7472 6f6b 652d 7769 6474 683d 2234 2220  troke-width="4" 
+000024a0: 6669 6c6c 3d22 6e6f 6e65 222f 3e3c 7465  fill="none"/><te
+000024b0: 7874 2073 7479 6c65 3d22 6669 6c6c 3a23  xt style="fill:#
+000024c0: 3330 3330 3330 3b66 6f6e 742d 6661 6d69  303030;font-fami
+000024d0: 6c79 3ae5 beae e8bd afe9 9b85 e9bb 913b  ly:............;
+000024e0: 666f 6e74 2d73 697a 653a 3131 2e30 3070  font-size:11.00p
+000024f0: 743b 666f 6e74 2d77 6569 6768 743a 626f  t;font-weight:bo
+00002500: 6c64 2220 786d 6c3a 7370 6163 653d 2270  ld" xml:space="p
+00002510: 7265 7365 7276 6522 3e3c 7473 7061 6e20  reserve"><tspan 
+00002520: 793d 2232 302e 3922 2078 3d22 3132 2e39  y="20.9" x="12.9
 00002530: 223e 5374 6f72 6167 653c 2f74 7370 616e  ">Storage</tspan
-00002540: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2074  ></text></g><g t
-00002550: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00002560: 6174 6528 3232 362e 3336 3130 3030 2c34  ate(226.361000,4
-00002570: 3537 2e30 3337 3530 3029 2220 6964 3d22  57.037500)" id="
-00002580: 7368 6170 6533 3422 3e3c 7061 7468 2066  shape34"><path f
-00002590: 696c 6c2d 7275 6c65 3d22 6e6f 6e7a 6572  ill-rule="nonzer
-000025a0: 6f22 2073 7472 6f6b 653d 2223 3435 3435  o" stroke="#4545
-000025b0: 3435 2220 7374 726f 6b65 2d77 6964 7468  45" stroke-width
-000025c0: 3d22 3422 2066 696c 6c3d 2223 6666 6666  ="4" fill="#ffff
-000025d0: 6666 2220 643d 224d 342e 302c 2e30 4c37  ff" d="M4.0,.0L7
-000025e0: 352e 302c 2e30 4337 372e 322c 2e30 2c37  5.0,.0C77.2,.0,7
-000025f0: 392e 302c 312e 382c 3739 2e30 2c34 2e30  9.0,1.8,79.0,4.0
-00002600: 4c37 392e 302c 3436 2e30 4337 392e 302c  L79.0,46.0C79.0,
-00002610: 3438 2e32 2c37 372e 322c 3530 2e30 2c37  48.2,77.2,50.0,7
-00002620: 352e 302c 3530 2e30 4c34 2e30 2c35 302e  5.0,50.0L4.0,50.
-00002630: 3043 312e 382c 3530 2e30 2c2e 302c 3438  0C1.8,50.0,.0,48
-00002640: 2e32 2c2e 302c 3436 2e30 4c2e 302c 342e  .2,.0,46.0L.0,4.
-00002650: 3043 2e30 2c31 2e38 2c31 2e38 2c2e 302c  0C.0,1.8,1.8,.0,
-00002660: 342e 302c 2e30 7a22 2f3e 3c74 6578 7420  4.0,.0z"/><text 
-00002670: 786d 6c3a 7370 6163 653d 2270 7265 7365  xml:space="prese
-00002680: 7276 6522 2073 7479 6c65 3d22 6669 6c6c  rve" style="fill
-00002690: 3a23 3330 3330 3330 3b66 6f6e 742d 6661  :#303030;font-fa
-000026a0: 6d69 6c79 3ae5 beae e8bd afe9 9b85 e9bb  mily:...........
-000026b0: 913b 666f 6e74 2d73 697a 653a 3134 2e30  .;font-size:14.0
-000026c0: 3070 743b 666f 6e74 2d77 6569 6768 743a  0pt;font-weight:
-000026d0: 626f 6c64 223e 3c74 7370 616e 2078 3d22  bold"><tspan x="
-000026e0: 3234 2e33 2220 793d 2233 322e 3022 3e45  24.3" y="32.0">E
+00002540: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2069  ></text></g><g i
+00002550: 643d 2273 6861 7065 3334 2220 7472 616e  d="shape34" tran
+00002560: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00002570: 2832 3236 2e33 3631 3030 302c 3435 372e  (226.361000,457.
+00002580: 3033 3735 3030 2922 3e3c 7061 7468 2064  037500)"><path d
+00002590: 3d22 4d34 2e30 2c2e 304c 3735 2e30 2c2e  ="M4.0,.0L75.0,.
+000025a0: 3043 3737 2e32 2c2e 302c 3739 2e30 2c31  0C77.2,.0,79.0,1
+000025b0: 2e38 2c37 392e 302c 342e 304c 3739 2e30  .8,79.0,4.0L79.0
+000025c0: 2c34 362e 3043 3739 2e30 2c34 382e 322c  ,46.0C79.0,48.2,
+000025d0: 3737 2e32 2c35 302e 302c 3735 2e30 2c35  77.2,50.0,75.0,5
+000025e0: 302e 304c 342e 302c 3530 2e30 4331 2e38  0.0L4.0,50.0C1.8
+000025f0: 2c35 302e 302c 2e30 2c34 382e 322c 2e30  ,50.0,.0,48.2,.0
+00002600: 2c34 362e 304c 2e30 2c34 2e30 432e 302c  ,46.0L.0,4.0C.0,
+00002610: 312e 382c 312e 382c 2e30 2c34 2e30 2c2e  1.8,1.8,.0,4.0,.
+00002620: 307a 2220 7374 726f 6b65 3d22 2334 3534  0z" stroke="#454
+00002630: 3534 3522 2073 7472 6f6b 652d 7769 6474  545" stroke-widt
+00002640: 683d 2234 2220 6669 6c6c 2d72 756c 653d  h="4" fill-rule=
+00002650: 226e 6f6e 7a65 726f 2220 6669 6c6c 3d22  "nonzero" fill="
+00002660: 2366 6666 6666 6622 2f3e 3c74 6578 7420  #ffffff"/><text 
+00002670: 7374 796c 653d 2266 696c 6c3a 2333 3033  style="fill:#303
+00002680: 3033 303b 666f 6e74 2d66 616d 696c 793a  030;font-family:
+00002690: e5be aee8 bdaf e99b 85e9 bb91 3b66 6f6e  ............;fon
+000026a0: 742d 7369 7a65 3a31 342e 3030 7074 3b66  t-size:14.00pt;f
+000026b0: 6f6e 742d 7765 6967 6874 3a62 6f6c 6422  ont-weight:bold"
+000026c0: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
+000026d0: 6572 7665 223e 3c74 7370 616e 2079 3d22  erve"><tspan y="
+000026e0: 3332 2e30 2220 783d 2232 342e 3322 3e45  32.0" x="24.3">E
 000026f0: 6e76 3c2f 7473 7061 6e3e 3c2f 7465 7874  nv</tspan></text
-00002700: 3e3c 2f67 3e3c 6720 7472 616e 7366 6f72  ></g><g transfor
-00002710: 6d3d 2274 7261 6e73 6c61 7465 2831 3432  m="translate(142
-00002720: 2e33 3631 3030 302c 3137 382e 3638 3735  .361000,178.6875
-00002730: 3030 2922 2069 643d 2273 6861 7065 3335  00)" id="shape35
-00002740: 223e 3c70 6174 6820 6669 6c6c 2d72 756c  "><path fill-rul
-00002750: 653d 226e 6f6e 7a65 726f 2220 7374 726f  e="nonzero" stro
-00002760: 6b65 3d22 2334 3534 3534 3522 2073 7472  ke="#454545" str
-00002770: 6f6b 652d 7769 6474 683d 2234 2220 6669  oke-width="4" fi
-00002780: 6c6c 3d22 2366 6666 6666 6622 2064 3d22  ll="#ffffff" d="
-00002790: 4d34 2e30 2c2e 304c 3135 392e 302c 2e30  M4.0,.0L159.0,.0
-000027a0: 4331 3631 2e32 2c2e 302c 3136 332e 302c  C161.2,.0,163.0,
-000027b0: 312e 382c 3136 332e 302c 342e 304c 3136  1.8,163.0,4.0L16
-000027c0: 332e 302c 3436 2e30 4331 3633 2e30 2c34  3.0,46.0C163.0,4
-000027d0: 382e 322c 3136 312e 322c 3530 2e30 2c31  8.2,161.2,50.0,1
-000027e0: 3539 2e30 2c35 302e 304c 342e 302c 3530  59.0,50.0L4.0,50
-000027f0: 2e30 4331 2e38 2c35 302e 302c 2e30 2c34  .0C1.8,50.0,.0,4
-00002800: 382e 322c 2e30 2c34 362e 304c 2e30 2c34  8.2,.0,46.0L.0,4
-00002810: 2e30 432e 302c 312e 382c 312e 382c 2e30  .0C.0,1.8,1.8,.0
-00002820: 2c34 2e30 2c2e 307a 222f 3e3c 7465 7874  ,4.0,.0z"/><text
-00002830: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
-00002840: 6572 7665 2220 7374 796c 653d 2266 696c  erve" style="fil
-00002850: 6c3a 2333 3033 3033 303b 666f 6e74 2d66  l:#303030;font-f
-00002860: 616d 696c 793a e5be aee8 bdaf e99b 85e9  amily:..........
-00002870: bb91 3b66 6f6e 742d 7369 7a65 3a31 342e  ..;font-size:14.
-00002880: 3030 7074 3b66 6f6e 742d 7765 6967 6874  00pt;font-weight
-00002890: 3a62 6f6c 6422 3e3c 7473 7061 6e20 783d  :bold"><tspan x=
-000028a0: 2232 342e 3322 2079 3d22 3332 2e30 223e  "24.3" y="32.0">
+00002700: 3e3c 2f67 3e3c 6720 6964 3d22 7368 6170  ></g><g id="shap
+00002710: 6533 3522 2074 7261 6e73 666f 726d 3d22  e35" transform="
+00002720: 7472 616e 736c 6174 6528 3134 322e 3336  translate(142.36
+00002730: 3130 3030 2c31 3738 2e36 3837 3530 3029  1000,178.687500)
+00002740: 223e 3c70 6174 6820 643d 224d 342e 302c  "><path d="M4.0,
+00002750: 2e30 4c31 3539 2e30 2c2e 3043 3136 312e  .0L159.0,.0C161.
+00002760: 322c 2e30 2c31 3633 2e30 2c31 2e38 2c31  2,.0,163.0,1.8,1
+00002770: 3633 2e30 2c34 2e30 4c31 3633 2e30 2c34  63.0,4.0L163.0,4
+00002780: 362e 3043 3136 332e 302c 3438 2e32 2c31  6.0C163.0,48.2,1
+00002790: 3631 2e32 2c35 302e 302c 3135 392e 302c  61.2,50.0,159.0,
+000027a0: 3530 2e30 4c34 2e30 2c35 302e 3043 312e  50.0L4.0,50.0C1.
+000027b0: 382c 3530 2e30 2c2e 302c 3438 2e32 2c2e  8,50.0,.0,48.2,.
+000027c0: 302c 3436 2e30 4c2e 302c 342e 3043 2e30  0,46.0L.0,4.0C.0
+000027d0: 2c31 2e38 2c31 2e38 2c2e 302c 342e 302c  ,1.8,1.8,.0,4.0,
+000027e0: 2e30 7a22 2073 7472 6f6b 653d 2223 3435  .0z" stroke="#45
+000027f0: 3435 3435 2220 7374 726f 6b65 2d77 6964  4545" stroke-wid
+00002800: 7468 3d22 3422 2066 696c 6c2d 7275 6c65  th="4" fill-rule
+00002810: 3d22 6e6f 6e7a 6572 6f22 2066 696c 6c3d  ="nonzero" fill=
+00002820: 2223 6666 6666 6666 222f 3e3c 7465 7874  "#ffffff"/><text
+00002830: 2073 7479 6c65 3d22 6669 6c6c 3a23 3330   style="fill:#30
+00002840: 3330 3330 3b66 6f6e 742d 6661 6d69 6c79  3030;font-family
+00002850: 3ae5 beae e8bd afe9 9b85 e9bb 913b 666f  :............;fo
+00002860: 6e74 2d73 697a 653a 3134 2e30 3070 743b  nt-size:14.00pt;
+00002870: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
+00002880: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
+00002890: 7365 7276 6522 3e3c 7473 7061 6e20 793d  serve"><tspan y=
+000028a0: 2233 322e 3022 2078 3d22 3234 2e33 223e  "32.0" x="24.3">
 000028b0: 4465 706c 6f79 6d65 6e74 3c2f 7473 7061  Deployment</tspa
 000028c0: 6e3e 3c2f 7465 7874 3e3c 2f67 3e3c 6720  n></text></g><g 
-000028d0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-000028e0: 6c61 7465 2831 3435 2e33 3631 3030 302c  late(145.361000,
-000028f0: 3330 392e 3838 3735 3030 2922 2069 643d  309.887500)" id=
-00002900: 2273 6861 7065 3336 223e 3c70 6174 6820  "shape36"><path 
-00002910: 6669 6c6c 2d72 756c 653d 226e 6f6e 7a65  fill-rule="nonze
-00002920: 726f 2220 7374 726f 6b65 3d22 2334 3534  ro" stroke="#454
-00002930: 3534 3522 2073 7472 6f6b 652d 7769 6474  545" stroke-widt
-00002940: 683d 2234 2220 6669 6c6c 3d22 2366 6666  h="4" fill="#fff
-00002950: 6666 6622 2064 3d22 4d34 2e30 2c2e 304c  fff" d="M4.0,.0L
-00002960: 3135 362e 302c 2e30 4331 3538 2e32 2c2e  156.0,.0C158.2,.
-00002970: 302c 3136 302e 302c 312e 382c 3136 302e  0,160.0,1.8,160.
-00002980: 302c 342e 304c 3136 302e 302c 3436 2e30  0,4.0L160.0,46.0
-00002990: 4331 3630 2e30 2c34 382e 322c 3135 382e  C160.0,48.2,158.
-000029a0: 322c 3530 2e30 2c31 3536 2e30 2c35 302e  2,50.0,156.0,50.
-000029b0: 304c 342e 302c 3530 2e30 4331 2e38 2c35  0L4.0,50.0C1.8,5
-000029c0: 302e 302c 2e30 2c34 382e 322c 2e30 2c34  0.0,.0,48.2,.0,4
-000029d0: 362e 304c 2e30 2c34 2e30 432e 302c 312e  6.0L.0,4.0C.0,1.
-000029e0: 382c 312e 382c 2e30 2c34 2e30 2c2e 307a  8,1.8,.0,4.0,.0z
-000029f0: 222f 3e3c 7465 7874 2078 6d6c 3a73 7061  "/><text xml:spa
-00002a00: 6365 3d22 7072 6573 6572 7665 2220 7374  ce="preserve" st
-00002a10: 796c 653d 2266 696c 6c3a 2333 3033 3033  yle="fill:#30303
-00002a20: 303b 666f 6e74 2d66 616d 696c 793a e5be  0;font-family:..
-00002a30: aee8 bdaf e99b 85e9 bb91 3b66 6f6e 742d  ..........;font-
-00002a40: 7369 7a65 3a31 342e 3030 7074 3b66 6f6e  size:14.00pt;fon
-00002a50: 742d 7765 6967 6874 3a62 6f6c 6422 3e3c  t-weight:bold"><
-00002a60: 7473 7061 6e20 783d 2232 342e 3322 2079  tspan x="24.3" y
-00002a70: 3d22 3332 2e30 223e 5072 652d 7472 6169  ="32.0">Pre-trai
+000028d0: 6964 3d22 7368 6170 6533 3622 2074 7261  id="shape36" tra
+000028e0: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+000028f0: 6528 3134 352e 3336 3130 3030 2c33 3039  e(145.361000,309
+00002900: 2e38 3837 3530 3029 223e 3c70 6174 6820  .887500)"><path 
+00002910: 643d 224d 342e 302c 2e30 4c31 3536 2e30  d="M4.0,.0L156.0
+00002920: 2c2e 3043 3135 382e 322c 2e30 2c31 3630  ,.0C158.2,.0,160
+00002930: 2e30 2c31 2e38 2c31 3630 2e30 2c34 2e30  .0,1.8,160.0,4.0
+00002940: 4c31 3630 2e30 2c34 362e 3043 3136 302e  L160.0,46.0C160.
+00002950: 302c 3438 2e32 2c31 3538 2e32 2c35 302e  0,48.2,158.2,50.
+00002960: 302c 3135 362e 302c 3530 2e30 4c34 2e30  0,156.0,50.0L4.0
+00002970: 2c35 302e 3043 312e 382c 3530 2e30 2c2e  ,50.0C1.8,50.0,.
+00002980: 302c 3438 2e32 2c2e 302c 3436 2e30 4c2e  0,48.2,.0,46.0L.
+00002990: 302c 342e 3043 2e30 2c31 2e38 2c31 2e38  0,4.0C.0,1.8,1.8
+000029a0: 2c2e 302c 342e 302c 2e30 7a22 2073 7472  ,.0,4.0,.0z" str
+000029b0: 6f6b 653d 2223 3435 3435 3435 2220 7374  oke="#454545" st
+000029c0: 726f 6b65 2d77 6964 7468 3d22 3422 2066  roke-width="4" f
+000029d0: 696c 6c2d 7275 6c65 3d22 6e6f 6e7a 6572  ill-rule="nonzer
+000029e0: 6f22 2066 696c 6c3d 2223 6666 6666 6666  o" fill="#ffffff
+000029f0: 222f 3e3c 7465 7874 2073 7479 6c65 3d22  "/><text style="
+00002a00: 6669 6c6c 3a23 3330 3330 3330 3b66 6f6e  fill:#303030;fon
+00002a10: 742d 6661 6d69 6c79 3ae5 beae e8bd afe9  t-family:.......
+00002a20: 9b85 e9bb 913b 666f 6e74 2d73 697a 653a  .....;font-size:
+00002a30: 3134 2e30 3070 743b 666f 6e74 2d77 6569  14.00pt;font-wei
+00002a40: 6768 743a 626f 6c64 2220 786d 6c3a 7370  ght:bold" xml:sp
+00002a50: 6163 653d 2270 7265 7365 7276 6522 3e3c  ace="preserve"><
+00002a60: 7473 7061 6e20 793d 2233 322e 3022 2078  tspan y="32.0" x
+00002a70: 3d22 3234 2e33 223e 5072 652d 7472 6169  ="24.3">Pre-trai
 00002a80: 6e69 6e67 3c2f 7473 7061 6e3e 3c2f 7465  ning</tspan></te
-00002a90: 7874 3e3c 2f67 3e3c 6720 7472 616e 7366  xt></g><g transf
-00002aa0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2837  orm="translate(7
-00002ab0: 3432 2e38 3031 3030 302c 3637 2e31 3530  42.801000,67.150
-00002ac0: 3030 3029 2220 6964 3d22 7368 6170 6533  000)" id="shape3
-00002ad0: 3722 3e3c 7061 7468 2066 696c 6c2d 7275  7"><path fill-ru
-00002ae0: 6c65 3d22 6e6f 6e7a 6572 6f22 2066 696c  le="nonzero" fil
-00002af0: 6c3d 2223 6666 6666 6666 2220 643d 224d  l="#ffffff" d="M
-00002b00: 2e30 2c2e 304c 3134 342e 302c 2e30 4c31  .0,.0L144.0,.0L1
-00002b10: 3434 2e30 2c33 322e 334c 2e30 2c33 322e  44.0,32.3L.0,32.
-00002b20: 334c 2e30 2c2e 307a 222f 3e3c 7061 7468  3L.0,.0z"/><path
-00002b30: 2073 7472 6f6b 653d 2223 3435 3435 3435   stroke="#454545
-00002b40: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
-00002b50: 3422 2066 696c 6c3d 226e 6f6e 6522 2064  4" fill="none" d
-00002b60: 3d22 4d2e 302c 3332 2e33 4c31 3434 2e30  ="M.0,32.3L144.0
-00002b70: 2c33 322e 3322 2f3e 3c74 6578 7420 786d  ,32.3"/><text xm
-00002b80: 6c3a 7370 6163 653d 2270 7265 7365 7276  l:space="preserv
-00002b90: 6522 2073 7479 6c65 3d22 6669 6c6c 3a23  e" style="fill:#
-00002ba0: 3330 3330 3330 3b66 6f6e 742d 6661 6d69  303030;font-fami
-00002bb0: 6c79 3ae5 beae e8bd afe9 9b85 e9bb 913b  ly:............;
-00002bc0: 666f 6e74 2d73 697a 653a 3131 2e30 3070  font-size:11.00p
-00002bd0: 743b 666f 6e74 2d77 6569 6768 743a 626f  t;font-weight:bo
-00002be0: 6c64 223e 3c74 7370 616e 2078 3d22 3132  ld"><tspan x="12
-00002bf0: 2e39 2220 793d 2232 302e 3922 3e49 6e74  .9" y="20.9">Int
+00002a90: 7874 3e3c 2f67 3e3c 6720 6964 3d22 7368  xt></g><g id="sh
+00002aa0: 6170 6533 3722 2074 7261 6e73 666f 726d  ape37" transform
+00002ab0: 3d22 7472 616e 736c 6174 6528 3734 322e  ="translate(742.
+00002ac0: 3830 3130 3030 2c36 372e 3135 3030 3030  801000,67.150000
+00002ad0: 2922 3e3c 7061 7468 2064 3d22 4d2e 302c  )"><path d="M.0,
+00002ae0: 2e30 4c31 3434 2e30 2c2e 304c 3134 342e  .0L144.0,.0L144.
+00002af0: 302c 3332 2e33 4c2e 302c 3332 2e33 4c2e  0,32.3L.0,32.3L.
+00002b00: 302c 2e30 7a22 2066 696c 6c2d 7275 6c65  0,.0z" fill-rule
+00002b10: 3d22 6e6f 6e7a 6572 6f22 2066 696c 6c3d  ="nonzero" fill=
+00002b20: 2223 6666 6666 6666 222f 3e3c 7061 7468  "#ffffff"/><path
+00002b30: 2064 3d22 4d2e 302c 3332 2e33 4c31 3434   d="M.0,32.3L144
+00002b40: 2e30 2c33 322e 3322 2073 7472 6f6b 653d  .0,32.3" stroke=
+00002b50: 2223 3435 3435 3435 2220 7374 726f 6b65  "#454545" stroke
+00002b60: 2d77 6964 7468 3d22 3422 2066 696c 6c3d  -width="4" fill=
+00002b70: 226e 6f6e 6522 2f3e 3c74 6578 7420 7374  "none"/><text st
+00002b80: 796c 653d 2266 696c 6c3a 2333 3033 3033  yle="fill:#30303
+00002b90: 303b 666f 6e74 2d66 616d 696c 793a e5be  0;font-family:..
+00002ba0: aee8 bdaf e99b 85e9 bb91 3b66 6f6e 742d  ..........;font-
+00002bb0: 7369 7a65 3a31 312e 3030 7074 3b66 6f6e  size:11.00pt;fon
+00002bc0: 742d 7765 6967 6874 3a62 6f6c 6422 2078  t-weight:bold" x
+00002bd0: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
+00002be0: 7665 223e 3c74 7370 616e 2079 3d22 3230  ve"><tspan y="20
+00002bf0: 2e39 2220 783d 2231 322e 3922 3e49 6e74  .9" x="12.9">Int
 00002c00: 7269 6e73 6963 2052 6577 6172 643c 2f74  rinsic Reward</t
 00002c10: 7370 616e 3e3c 2f74 6578 743e 3c2f 673e  span></text></g>
-00002c20: 3c67 2074 7261 6e73 666f 726d 3d22 7472  <g transform="tr
-00002c30: 616e 736c 6174 6528 3734 322e 3830 3130  anslate(742.8010
-00002c40: 3030 2c31 3038 2e31 3030 3030 3029 2220  00,108.100000)" 
-00002c50: 6964 3d22 7368 6170 6533 3822 3e3c 7061  id="shape38"><pa
-00002c60: 7468 2066 696c 6c2d 7275 6c65 3d22 6e6f  th fill-rule="no
-00002c70: 6e7a 6572 6f22 2066 696c 6c3d 2223 6666  nzero" fill="#ff
-00002c80: 6666 6666 2220 643d 224d 2e30 2c2e 304c  ffff" d="M.0,.0L
-00002c90: 3133 332e 302c 2e30 4c31 3333 2e30 2c33  133.0,.0L133.0,3
-00002ca0: 322e 334c 2e30 2c33 322e 334c 2e30 2c2e  2.3L.0,32.3L.0,.
-00002cb0: 307a 222f 3e3c 7061 7468 2073 7472 6f6b  0z"/><path strok
-00002cc0: 653d 2223 3435 3435 3435 2220 7374 726f  e="#454545" stro
-00002cd0: 6b65 2d77 6964 7468 3d22 3422 2066 696c  ke-width="4" fil
-00002ce0: 6c3d 226e 6f6e 6522 2064 3d22 4d2e 302c  l="none" d="M.0,
-00002cf0: 3332 2e33 4c31 3333 2e30 2c33 322e 3322  32.3L133.0,32.3"
-00002d00: 2f3e 3c74 6578 7420 786d 6c3a 7370 6163  /><text xml:spac
-00002d10: 653d 2270 7265 7365 7276 6522 2073 7479  e="preserve" sty
-00002d20: 6c65 3d22 6669 6c6c 3a23 3330 3330 3330  le="fill:#303030
-00002d30: 3b66 6f6e 742d 6661 6d69 6c79 3ae5 beae  ;font-family:...
-00002d40: e8bd afe9 9b85 e9bb 913b 666f 6e74 2d73  .........;font-s
-00002d50: 697a 653a 3131 2e30 3070 743b 666f 6e74  ize:11.00pt;font
-00002d60: 2d77 6569 6768 743a 626f 6c64 223e 3c74  -weight:bold"><t
-00002d70: 7370 616e 2078 3d22 3132 2e39 2220 793d  span x="12.9" y=
-00002d80: 2232 302e 3922 3e41 7567 6d65 6e74 6174  "20.9">Augmentat
+00002c20: 3c67 2069 643d 2273 6861 7065 3338 2220  <g id="shape38" 
+00002c30: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00002c40: 6c61 7465 2837 3432 2e38 3031 3030 302c  late(742.801000,
+00002c50: 3130 382e 3130 3030 3030 2922 3e3c 7061  108.100000)"><pa
+00002c60: 7468 2064 3d22 4d2e 302c 2e30 4c31 3333  th d="M.0,.0L133
+00002c70: 2e30 2c2e 304c 3133 332e 302c 3332 2e33  .0,.0L133.0,32.3
+00002c80: 4c2e 302c 3332 2e33 4c2e 302c 2e30 7a22  L.0,32.3L.0,.0z"
+00002c90: 2066 696c 6c2d 7275 6c65 3d22 6e6f 6e7a   fill-rule="nonz
+00002ca0: 6572 6f22 2066 696c 6c3d 2223 6666 6666  ero" fill="#ffff
+00002cb0: 6666 222f 3e3c 7061 7468 2064 3d22 4d2e  ff"/><path d="M.
+00002cc0: 302c 3332 2e33 4c31 3333 2e30 2c33 322e  0,32.3L133.0,32.
+00002cd0: 3322 2073 7472 6f6b 653d 2223 3435 3435  3" stroke="#4545
+00002ce0: 3435 2220 7374 726f 6b65 2d77 6964 7468  45" stroke-width
+00002cf0: 3d22 3422 2066 696c 6c3d 226e 6f6e 6522  ="4" fill="none"
+00002d00: 2f3e 3c74 6578 7420 7374 796c 653d 2266  /><text style="f
+00002d10: 696c 6c3a 2333 3033 3033 303b 666f 6e74  ill:#303030;font
+00002d20: 2d66 616d 696c 793a e5be aee8 bdaf e99b  -family:........
+00002d30: 85e9 bb91 3b66 6f6e 742d 7369 7a65 3a31  ....;font-size:1
+00002d40: 312e 3030 7074 3b66 6f6e 742d 7765 6967  1.00pt;font-weig
+00002d50: 6874 3a62 6f6c 6422 2078 6d6c 3a73 7061  ht:bold" xml:spa
+00002d60: 6365 3d22 7072 6573 6572 7665 223e 3c74  ce="preserve"><t
+00002d70: 7370 616e 2079 3d22 3230 2e39 2220 783d  span y="20.9" x=
+00002d80: 2231 322e 3922 3e41 7567 6d65 6e74 6174  "12.9">Augmentat
 00002d90: 696f 6e3c 2f74 7370 616e 3e3c 2f74 6578  ion</tspan></tex
-00002da0: 743e 3c2f 673e 3c67 2074 7261 6e73 666f  t></g><g transfo
-00002db0: 726d 3d22 7472 616e 736c 6174 6528 3734  rm="translate(74
-00002dc0: 322e 3830 3130 3030 2c31 3439 2e30 3530  2.801000,149.050
-00002dd0: 3030 3029 2220 6964 3d22 7368 6170 6533  000)" id="shape3
-00002de0: 3922 3e3c 7061 7468 2066 696c 6c2d 7275  9"><path fill-ru
-00002df0: 6c65 3d22 6e6f 6e7a 6572 6f22 2066 696c  le="nonzero" fil
-00002e00: 6c3d 2223 6666 6666 6666 2220 643d 224d  l="#ffffff" d="M
-00002e10: 2e30 2c2e 304c 3131 322e 302c 2e30 4c31  .0,.0L112.0,.0L1
-00002e20: 3132 2e30 2c33 322e 334c 2e30 2c33 322e  12.0,32.3L.0,32.
-00002e30: 334c 2e30 2c2e 307a 222f 3e3c 7061 7468  3L.0,.0z"/><path
-00002e40: 2073 7472 6f6b 653d 2223 3435 3435 3435   stroke="#454545
-00002e50: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
-00002e60: 3422 2066 696c 6c3d 226e 6f6e 6522 2064  4" fill="none" d
-00002e70: 3d22 4d2e 302c 3332 2e33 4c31 3132 2e30  ="M.0,32.3L112.0
-00002e80: 2c33 322e 3322 2f3e 3c74 6578 7420 786d  ,32.3"/><text xm
-00002e90: 6c3a 7370 6163 653d 2270 7265 7365 7276  l:space="preserv
-00002ea0: 6522 2073 7479 6c65 3d22 6669 6c6c 3a23  e" style="fill:#
-00002eb0: 3330 3330 3330 3b66 6f6e 742d 6661 6d69  303030;font-fami
-00002ec0: 6c79 3ae5 beae e8bd afe9 9b85 e9bb 913b  ly:............;
-00002ed0: 666f 6e74 2d73 697a 653a 3131 2e30 3070  font-size:11.00p
-00002ee0: 743b 666f 6e74 2d77 6569 6768 743a 626f  t;font-weight:bo
-00002ef0: 6c64 223e 3c74 7370 616e 2078 3d22 3132  ld"><tspan x="12
-00002f00: 2e39 2220 793d 2232 302e 3922 3e44 6973  .9" y="20.9">Dis
+00002da0: 743e 3c2f 673e 3c67 2069 643d 2273 6861  t></g><g id="sha
+00002db0: 7065 3339 2220 7472 616e 7366 6f72 6d3d  pe39" transform=
+00002dc0: 2274 7261 6e73 6c61 7465 2837 3432 2e38  "translate(742.8
+00002dd0: 3031 3030 302c 3134 392e 3035 3030 3030  01000,149.050000
+00002de0: 2922 3e3c 7061 7468 2064 3d22 4d2e 302c  )"><path d="M.0,
+00002df0: 2e30 4c31 3132 2e30 2c2e 304c 3131 322e  .0L112.0,.0L112.
+00002e00: 302c 3332 2e33 4c2e 302c 3332 2e33 4c2e  0,32.3L.0,32.3L.
+00002e10: 302c 2e30 7a22 2066 696c 6c2d 7275 6c65  0,.0z" fill-rule
+00002e20: 3d22 6e6f 6e7a 6572 6f22 2066 696c 6c3d  ="nonzero" fill=
+00002e30: 2223 6666 6666 6666 222f 3e3c 7061 7468  "#ffffff"/><path
+00002e40: 2064 3d22 4d2e 302c 3332 2e33 4c31 3132   d="M.0,32.3L112
+00002e50: 2e30 2c33 322e 3322 2073 7472 6f6b 653d  .0,32.3" stroke=
+00002e60: 2223 3435 3435 3435 2220 7374 726f 6b65  "#454545" stroke
+00002e70: 2d77 6964 7468 3d22 3422 2066 696c 6c3d  -width="4" fill=
+00002e80: 226e 6f6e 6522 2f3e 3c74 6578 7420 7374  "none"/><text st
+00002e90: 796c 653d 2266 696c 6c3a 2333 3033 3033  yle="fill:#30303
+00002ea0: 303b 666f 6e74 2d66 616d 696c 793a e5be  0;font-family:..
+00002eb0: aee8 bdaf e99b 85e9 bb91 3b66 6f6e 742d  ..........;font-
+00002ec0: 7369 7a65 3a31 312e 3030 7074 3b66 6f6e  size:11.00pt;fon
+00002ed0: 742d 7765 6967 6874 3a62 6f6c 6422 2078  t-weight:bold" x
+00002ee0: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
+00002ef0: 7665 223e 3c74 7370 616e 2079 3d22 3230  ve"><tspan y="20
+00002f00: 2e39 2220 783d 2231 322e 3922 3e44 6973  .9" x="12.9">Dis
 00002f10: 7472 6962 7574 696f 6e3c 2f74 7370 616e  tribution</tspan
-00002f20: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2074  ></text></g><g t
-00002f30: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00002f40: 6174 6528 3736 362e 3830 3130 3030 2c33  ate(766.801000,3
-00002f50: 3631 2e34 3530 3030 3029 2220 6964 3d22  61.450000)" id="
-00002f60: 7368 6170 6534 3022 3e3c 7061 7468 2066  shape40"><path f
-00002f70: 696c 6c2d 7275 6c65 3d22 6e6f 6e7a 6572  ill-rule="nonzer
-00002f80: 6f22 2066 696c 6c3d 2223 6666 6666 6666  o" fill="#ffffff
-00002f90: 2220 643d 224d 2e30 2c2e 304c 3735 2e30  " d="M.0,.0L75.0
-00002fa0: 2c2e 304c 3735 2e30 2c33 322e 334c 2e30  ,.0L75.0,32.3L.0
-00002fb0: 2c33 322e 334c 2e30 2c2e 307a 222f 3e3c  ,32.3L.0,.0z"/><
-00002fc0: 7061 7468 2073 7472 6f6b 653d 2223 3435  path stroke="#45
-00002fd0: 3435 3435 2220 7374 726f 6b65 2d77 6964  4545" stroke-wid
-00002fe0: 7468 3d22 3422 2066 696c 6c3d 226e 6f6e  th="4" fill="non
-00002ff0: 6522 2064 3d22 4d2e 302c 3332 2e33 4c37  e" d="M.0,32.3L7
-00003000: 352e 302c 3332 2e33 222f 3e3c 7465 7874  5.0,32.3"/><text
-00003010: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
-00003020: 6572 7665 2220 7374 796c 653d 2266 696c  erve" style="fil
-00003030: 6c3a 2333 3033 3033 303b 666f 6e74 2d66  l:#303030;font-f
-00003040: 616d 696c 793a e5be aee8 bdaf e99b 85e9  amily:..........
-00003050: bb91 3b66 6f6e 742d 7369 7a65 3a31 312e  ..;font-size:11.
-00003060: 3030 7074 3b66 6f6e 742d 7765 6967 6874  00pt;font-weight
-00003070: 3a62 6f6c 6422 3e3c 7473 7061 6e20 783d  :bold"><tspan x=
-00003080: 2231 322e 3922 2079 3d22 3230 2e39 223e  "12.9" y="20.9">
+00002f20: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2069  ></text></g><g i
+00002f30: 643d 2273 6861 7065 3430 2220 7472 616e  d="shape40" tran
+00002f40: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00002f50: 2837 3636 2e38 3031 3030 302c 3336 312e  (766.801000,361.
+00002f60: 3435 3030 3030 2922 3e3c 7061 7468 2064  450000)"><path d
+00002f70: 3d22 4d2e 302c 2e30 4c37 352e 302c 2e30  ="M.0,.0L75.0,.0
+00002f80: 4c37 352e 302c 3332 2e33 4c2e 302c 3332  L75.0,32.3L.0,32
+00002f90: 2e33 4c2e 302c 2e30 7a22 2066 696c 6c2d  .3L.0,.0z" fill-
+00002fa0: 7275 6c65 3d22 6e6f 6e7a 6572 6f22 2066  rule="nonzero" f
+00002fb0: 696c 6c3d 2223 6666 6666 6666 222f 3e3c  ill="#ffffff"/><
+00002fc0: 7061 7468 2064 3d22 4d2e 302c 3332 2e33  path d="M.0,32.3
+00002fd0: 4c37 352e 302c 3332 2e33 2220 7374 726f  L75.0,32.3" stro
+00002fe0: 6b65 3d22 2334 3534 3534 3522 2073 7472  ke="#454545" str
+00002ff0: 6f6b 652d 7769 6474 683d 2234 2220 6669  oke-width="4" fi
+00003000: 6c6c 3d22 6e6f 6e65 222f 3e3c 7465 7874  ll="none"/><text
+00003010: 2073 7479 6c65 3d22 6669 6c6c 3a23 3330   style="fill:#30
+00003020: 3330 3330 3b66 6f6e 742d 6661 6d69 6c79  3030;font-family
+00003030: 3ae5 beae e8bd afe9 9b85 e9bb 913b 666f  :............;fo
+00003040: 6e74 2d73 697a 653a 3131 2e30 3070 743b  nt-size:11.00pt;
+00003050: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
+00003060: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
+00003070: 7365 7276 6522 3e3c 7473 7061 6e20 793d  serve"><tspan y=
+00003080: 2232 302e 3922 2078 3d22 3132 2e39 223e  "20.9" x="12.9">
 00003090: 456e 6769 6e65 3c2f 7473 7061 6e3e 3c2f  Engine</tspan></
-000030a0: 7465 7874 3e3c 2f67 3e3c 6720 7472 616e  text></g><g tran
-000030b0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-000030c0: 2837 3636 2e38 3031 3030 302c 3434 332e  (766.801000,443.
-000030d0: 3335 3030 3030 2922 2069 643d 2273 6861  350000)" id="sha
-000030e0: 7065 3431 223e 3c70 6174 6820 6669 6c6c  pe41"><path fill
-000030f0: 2d72 756c 653d 226e 6f6e 7a65 726f 2220  -rule="nonzero" 
-00003100: 6669 6c6c 3d22 2366 6666 6666 6622 2064  fill="#ffffff" d
-00003110: 3d22 4d2e 302c 2e30 4c36 352e 302c 2e30  ="M.0,.0L65.0,.0
-00003120: 4c36 352e 302c 3332 2e33 4c2e 302c 3332  L65.0,32.3L.0,32
-00003130: 2e33 4c2e 302c 2e30 7a22 2f3e 3c70 6174  .3L.0,.0z"/><pat
-00003140: 6820 7374 726f 6b65 3d22 2334 3534 3534  h stroke="#45454
-00003150: 3522 2073 7472 6f6b 652d 7769 6474 683d  5" stroke-width=
-00003160: 2234 2220 6669 6c6c 3d22 6e6f 6e65 2220  "4" fill="none" 
-00003170: 643d 224d 2e30 2c33 322e 334c 3635 2e30  d="M.0,32.3L65.0
-00003180: 2c33 322e 3322 2f3e 3c74 6578 7420 786d  ,32.3"/><text xm
-00003190: 6c3a 7370 6163 653d 2270 7265 7365 7276  l:space="preserv
-000031a0: 6522 2073 7479 6c65 3d22 6669 6c6c 3a23  e" style="fill:#
-000031b0: 3330 3330 3330 3b66 6f6e 742d 6661 6d69  303030;font-fami
-000031c0: 6c79 3ae5 beae e8bd afe9 9b85 e9bb 913b  ly:............;
-000031d0: 666f 6e74 2d73 697a 653a 3131 2e30 3070  font-size:11.00p
-000031e0: 743b 666f 6e74 2d77 6569 6768 743a 626f  t;font-weight:bo
-000031f0: 6c64 223e 3c74 7370 616e 2078 3d22 3132  ld"><tspan x="12
-00003200: 2e39 2220 793d 2232 302e 3922 3ec2 b7c2  .9" y="20.9">...
+000030a0: 7465 7874 3e3c 2f67 3e3c 6720 6964 3d22  text></g><g id="
+000030b0: 7368 6170 6534 3122 2074 7261 6e73 666f  shape41" transfo
+000030c0: 726d 3d22 7472 616e 736c 6174 6528 3736  rm="translate(76
+000030d0: 362e 3830 3130 3030 2c34 3433 2e33 3530  6.801000,443.350
+000030e0: 3030 3029 223e 3c70 6174 6820 643d 224d  000)"><path d="M
+000030f0: 2e30 2c2e 304c 3635 2e30 2c2e 304c 3635  .0,.0L65.0,.0L65
+00003100: 2e30 2c33 322e 334c 2e30 2c33 322e 334c  .0,32.3L.0,32.3L
+00003110: 2e30 2c2e 307a 2220 6669 6c6c 2d72 756c  .0,.0z" fill-rul
+00003120: 653d 226e 6f6e 7a65 726f 2220 6669 6c6c  e="nonzero" fill
+00003130: 3d22 2366 6666 6666 6622 2f3e 3c70 6174  ="#ffffff"/><pat
+00003140: 6820 643d 224d 2e30 2c33 322e 334c 3635  h d="M.0,32.3L65
+00003150: 2e30 2c33 322e 3322 2073 7472 6f6b 653d  .0,32.3" stroke=
+00003160: 2223 3435 3435 3435 2220 7374 726f 6b65  "#454545" stroke
+00003170: 2d77 6964 7468 3d22 3422 2066 696c 6c3d  -width="4" fill=
+00003180: 226e 6f6e 6522 2f3e 3c74 6578 7420 7374  "none"/><text st
+00003190: 796c 653d 2266 696c 6c3a 2333 3033 3033  yle="fill:#30303
+000031a0: 303b 666f 6e74 2d66 616d 696c 793a e5be  0;font-family:..
+000031b0: aee8 bdaf e99b 85e9 bb91 3b66 6f6e 742d  ..........;font-
+000031c0: 7369 7a65 3a31 312e 3030 7074 3b66 6f6e  size:11.00pt;fon
+000031d0: 742d 7765 6967 6874 3a62 6f6c 6422 2078  t-weight:bold" x
+000031e0: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
+000031f0: 7665 223e 3c74 7370 616e 2079 3d22 3230  ve"><tspan y="20
+00003200: 2e39 2220 783d 2231 322e 3922 3ec2 b7c2  .9" x="12.9">...
 00003210: b7c2 b7c2 b7c2 b7c2 b73c 2f74 7370 616e  .........</tspan
-00003220: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2074  ></text></g><g t
-00003230: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00003240: 6174 6528 3837 2e33 3631 3030 302c 3430  ate(87.361000,40
-00003250: 382e 3833 3735 3030 2922 2069 643d 2273  8.837500)" id="s
-00003260: 6861 7065 3432 223e 3c70 6174 6820 6669  hape42"><path fi
-00003270: 6c6c 2d72 756c 653d 226e 6f6e 7a65 726f  ll-rule="nonzero
-00003280: 2220 6669 6c6c 3d22 2366 6666 6666 6622  " fill="#ffffff"
-00003290: 2064 3d22 4d2e 302c 2e30 4c31 3134 2e30   d="M.0,.0L114.0
-000032a0: 2c2e 304c 3131 342e 302c 3332 2e33 4c2e  ,.0L114.0,32.3L.
-000032b0: 302c 3332 2e33 4c2e 302c 2e30 7a22 2f3e  0,32.3L.0,.0z"/>
-000032c0: 3c70 6174 6820 7374 726f 6b65 3d22 2334  <path stroke="#4
-000032d0: 3534 3534 3522 2073 7472 6f6b 652d 7769  54545" stroke-wi
-000032e0: 6474 683d 2234 2220 6669 6c6c 3d22 6e6f  dth="4" fill="no
-000032f0: 6e65 2220 643d 224d 2e30 2c33 322e 334c  ne" d="M.0,32.3L
-00003300: 3131 342e 302c 3332 2e33 222f 3e3c 7465  114.0,32.3"/><te
-00003310: 7874 2078 6d6c 3a73 7061 6365 3d22 7072  xt xml:space="pr
-00003320: 6573 6572 7665 2220 7374 796c 653d 2266  eserve" style="f
-00003330: 696c 6c3a 2333 3033 3033 303b 666f 6e74  ill:#303030;font
-00003340: 2d66 616d 696c 793a e5be aee8 bdaf e99b  -family:........
-00003350: 85e9 bb91 3b66 6f6e 742d 7369 7a65 3a31  ....;font-size:1
-00003360: 312e 3030 7074 3b66 6f6e 742d 7765 6967  1.00pt;font-weig
-00003370: 6874 3a62 6f6c 6422 3e3c 7473 7061 6e20  ht:bold"><tspan 
-00003380: 783d 2231 322e 3922 2079 3d22 3230 2e39  x="12.9" y="20.9
+00003220: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2069  ></text></g><g i
+00003230: 643d 2273 6861 7065 3432 2220 7472 616e  d="shape42" tran
+00003240: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00003250: 2838 372e 3336 3130 3030 2c34 3038 2e38  (87.361000,408.8
+00003260: 3337 3530 3029 223e 3c70 6174 6820 643d  37500)"><path d=
+00003270: 224d 2e30 2c2e 304c 3131 342e 302c 2e30  "M.0,.0L114.0,.0
+00003280: 4c31 3134 2e30 2c33 322e 334c 2e30 2c33  L114.0,32.3L.0,3
+00003290: 322e 334c 2e30 2c2e 307a 2220 6669 6c6c  2.3L.0,.0z" fill
+000032a0: 2d72 756c 653d 226e 6f6e 7a65 726f 2220  -rule="nonzero" 
+000032b0: 6669 6c6c 3d22 2366 6666 6666 6622 2f3e  fill="#ffffff"/>
+000032c0: 3c70 6174 6820 643d 224d 2e30 2c33 322e  <path d="M.0,32.
+000032d0: 334c 3131 342e 302c 3332 2e33 2220 7374  3L114.0,32.3" st
+000032e0: 726f 6b65 3d22 2334 3534 3534 3522 2073  roke="#454545" s
+000032f0: 7472 6f6b 652d 7769 6474 683d 2234 2220  troke-width="4" 
+00003300: 6669 6c6c 3d22 6e6f 6e65 222f 3e3c 7465  fill="none"/><te
+00003310: 7874 2073 7479 6c65 3d22 6669 6c6c 3a23  xt style="fill:#
+00003320: 3330 3330 3330 3b66 6f6e 742d 6661 6d69  303030;font-fami
+00003330: 6c79 3ae5 beae e8bd afe9 9b85 e9bb 913b  ly:............;
+00003340: 666f 6e74 2d73 697a 653a 3131 2e30 3070  font-size:11.00p
+00003350: 743b 666f 6e74 2d77 6569 6768 743a 626f  t;font-weight:bo
+00003360: 6c64 2220 786d 6c3a 7370 6163 653d 2270  ld" xml:space="p
+00003370: 7265 7365 7276 6522 3e3c 7473 7061 6e20  reserve"><tspan 
+00003380: 793d 2232 302e 3922 2078 3d22 3132 2e39  y="20.9" x="12.9
 00003390: 223e 4174 6172 6920 4761 6d65 733c 2f74  ">Atari Games</t
 000033a0: 7370 616e 3e3c 2f74 6578 743e 3c2f 673e  span></text></g>
-000033b0: 3c67 2074 7261 6e73 666f 726d 3d22 7472  <g transform="tr
-000033c0: 616e 736c 6174 6528 3736 362e 3830 3130  anslate(766.8010
-000033d0: 3030 2c34 3032 2e34 3030 3030 3029 2220  00,402.400000)" 
-000033e0: 6964 3d22 7368 6170 6534 3322 3e3c 7061  id="shape43"><pa
-000033f0: 7468 2066 696c 6c2d 7275 6c65 3d22 6e6f  th fill-rule="no
-00003400: 6e7a 6572 6f22 2066 696c 6c3d 2223 6666  nzero" fill="#ff
-00003410: 6666 6666 2220 643d 224d 2e30 2c2e 304c  ffff" d="M.0,.0L
-00003420: 3736 2e30 2c2e 304c 3736 2e30 2c33 322e  76.0,.0L76.0,32.
-00003430: 334c 2e30 2c33 322e 334c 2e30 2c2e 307a  3L.0,32.3L.0,.0z
-00003440: 222f 3e3c 7061 7468 2073 7472 6f6b 653d  "/><path stroke=
-00003450: 2223 3435 3435 3435 2220 7374 726f 6b65  "#454545" stroke
-00003460: 2d77 6964 7468 3d22 3422 2066 696c 6c3d  -width="4" fill=
-00003470: 226e 6f6e 6522 2064 3d22 4d2e 302c 3332  "none" d="M.0,32
-00003480: 2e33 4c37 362e 302c 3332 2e33 222f 3e3c  .3L76.0,32.3"/><
-00003490: 7465 7874 2078 6d6c 3a73 7061 6365 3d22  text xml:space="
-000034a0: 7072 6573 6572 7665 2220 7374 796c 653d  preserve" style=
-000034b0: 2266 696c 6c3a 2333 3033 3033 303b 666f  "fill:#303030;fo
-000034c0: 6e74 2d66 616d 696c 793a e5be aee8 bdaf  nt-family:......
-000034d0: e99b 85e9 bb91 3b66 6f6e 742d 7369 7a65  ......;font-size
-000034e0: 3a31 312e 3030 7074 3b66 6f6e 742d 7765  :11.00pt;font-we
-000034f0: 6967 6874 3a62 6f6c 6422 3e3c 7473 7061  ight:bold"><tspa
-00003500: 6e20 783d 2231 322e 3922 2079 3d22 3230  n x="12.9" y="20
+000033b0: 3c67 2069 643d 2273 6861 7065 3433 2220  <g id="shape43" 
+000033c0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+000033d0: 6c61 7465 2837 3636 2e38 3031 3030 302c  late(766.801000,
+000033e0: 3430 322e 3430 3030 3030 2922 3e3c 7061  402.400000)"><pa
+000033f0: 7468 2064 3d22 4d2e 302c 2e30 4c37 362e  th d="M.0,.0L76.
+00003400: 302c 2e30 4c37 362e 302c 3332 2e33 4c2e  0,.0L76.0,32.3L.
+00003410: 302c 3332 2e33 4c2e 302c 2e30 7a22 2066  0,32.3L.0,.0z" f
+00003420: 696c 6c2d 7275 6c65 3d22 6e6f 6e7a 6572  ill-rule="nonzer
+00003430: 6f22 2066 696c 6c3d 2223 6666 6666 6666  o" fill="#ffffff
+00003440: 222f 3e3c 7061 7468 2064 3d22 4d2e 302c  "/><path d="M.0,
+00003450: 3332 2e33 4c37 362e 302c 3332 2e33 2220  32.3L76.0,32.3" 
+00003460: 7374 726f 6b65 3d22 2334 3534 3534 3522  stroke="#454545"
+00003470: 2073 7472 6f6b 652d 7769 6474 683d 2234   stroke-width="4
+00003480: 2220 6669 6c6c 3d22 6e6f 6e65 222f 3e3c  " fill="none"/><
+00003490: 7465 7874 2073 7479 6c65 3d22 6669 6c6c  text style="fill
+000034a0: 3a23 3330 3330 3330 3b66 6f6e 742d 6661  :#303030;font-fa
+000034b0: 6d69 6c79 3ae5 beae e8bd afe9 9b85 e9bb  mily:...........
+000034c0: 913b 666f 6e74 2d73 697a 653a 3131 2e30  .;font-size:11.0
+000034d0: 3070 743b 666f 6e74 2d77 6569 6768 743a  0pt;font-weight:
+000034e0: 626f 6c64 2220 786d 6c3a 7370 6163 653d  bold" xml:space=
+000034f0: 2270 7265 7365 7276 6522 3e3c 7473 7061  "preserve"><tspa
+00003500: 6e20 793d 2232 302e 3922 2078 3d22 3132  n y="20.9" x="12
 00003510: 2e39 223e 4c6f 6767 6572 3c2f 7473 7061  .9">Logger</tspa
 00003520: 6e3e 3c2f 7465 7874 3e3c 2f67 3e3c 6720  n></text></g><g 
-00003530: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00003540: 6c61 7465 2833 392e 3336 3130 3030 2c31  late(39.361000,1
-00003550: 3530 2e39 3632 3530 3029 2220 6964 3d22  50.962500)" id="
-00003560: 7368 6170 6534 3422 3e3c 7061 7468 2066  shape44"><path f
-00003570: 696c 6c2d 7275 6c65 3d22 6e6f 6e7a 6572  ill-rule="nonzer
-00003580: 6f22 2066 696c 6c3d 2223 6666 6666 6666  o" fill="#ffffff
-00003590: 2220 643d 224d 2e30 2c2e 304c 3738 2e30  " d="M.0,.0L78.0
-000035a0: 2c2e 304c 3738 2e30 2c33 322e 334c 2e30  ,.0L78.0,32.3L.0
-000035b0: 2c33 322e 334c 2e30 2c2e 307a 222f 3e3c  ,32.3L.0,.0z"/><
-000035c0: 7061 7468 2073 7472 6f6b 653d 2223 3435  path stroke="#45
-000035d0: 3435 3435 2220 7374 726f 6b65 2d77 6964  4545" stroke-wid
-000035e0: 7468 3d22 3422 2066 696c 6c3d 226e 6f6e  th="4" fill="non
-000035f0: 6522 2064 3d22 4d2e 302c 3332 2e33 4c37  e" d="M.0,32.3L7
-00003600: 382e 302c 3332 2e33 222f 3e3c 7465 7874  8.0,32.3"/><text
-00003610: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
-00003620: 6572 7665 2220 7374 796c 653d 2266 696c  erve" style="fil
-00003630: 6c3a 2333 3033 3033 303b 666f 6e74 2d66  l:#303030;font-f
-00003640: 616d 696c 793a e5be aee8 bdaf e99b 85e9  amily:..........
-00003650: bb91 3b66 6f6e 742d 7369 7a65 3a31 312e  ..;font-size:11.
-00003660: 3030 7074 3b66 6f6e 742d 7765 6967 6874  00pt;font-weight
-00003670: 3a62 6f6c 6422 3e3c 7473 7061 6e20 783d  :bold"><tspan x=
-00003680: 2231 322e 3922 2079 3d22 3230 2e39 223e  "12.9" y="20.9">
+00003530: 6964 3d22 7368 6170 6534 3422 2074 7261  id="shape44" tra
+00003540: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+00003550: 6528 3339 2e33 3631 3030 302c 3135 302e  e(39.361000,150.
+00003560: 3936 3235 3030 2922 3e3c 7061 7468 2064  962500)"><path d
+00003570: 3d22 4d2e 302c 2e30 4c37 382e 302c 2e30  ="M.0,.0L78.0,.0
+00003580: 4c37 382e 302c 3332 2e33 4c2e 302c 3332  L78.0,32.3L.0,32
+00003590: 2e33 4c2e 302c 2e30 7a22 2066 696c 6c2d  .3L.0,.0z" fill-
+000035a0: 7275 6c65 3d22 6e6f 6e7a 6572 6f22 2066  rule="nonzero" f
+000035b0: 696c 6c3d 2223 6666 6666 6666 222f 3e3c  ill="#ffffff"/><
+000035c0: 7061 7468 2064 3d22 4d2e 302c 3332 2e33  path d="M.0,32.3
+000035d0: 4c37 382e 302c 3332 2e33 2220 7374 726f  L78.0,32.3" stro
+000035e0: 6b65 3d22 2334 3534 3534 3522 2073 7472  ke="#454545" str
+000035f0: 6f6b 652d 7769 6474 683d 2234 2220 6669  oke-width="4" fi
+00003600: 6c6c 3d22 6e6f 6e65 222f 3e3c 7465 7874  ll="none"/><text
+00003610: 2073 7479 6c65 3d22 6669 6c6c 3a23 3330   style="fill:#30
+00003620: 3330 3330 3b66 6f6e 742d 6661 6d69 6c79  3030;font-family
+00003630: 3ae5 beae e8bd afe9 9b85 e9bb 913b 666f  :............;fo
+00003640: 6e74 2d73 697a 653a 3131 2e30 3070 743b  nt-size:11.00pt;
+00003650: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
+00003660: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
+00003670: 7365 7276 6522 3e3c 7473 7061 6e20 793d  serve"><tspan y=
+00003680: 2232 302e 3922 2078 3d22 3132 2e39 223e  "20.9" x="12.9">
 00003690: 5079 7468 6f6e 3c2f 7473 7061 6e3e 3c2f  Python</tspan></
-000036a0: 7465 7874 3e3c 2f67 3e3c 6720 7472 616e  text></g><g tran
-000036b0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-000036c0: 2836 322e 3336 3130 3030 2c31 3931 2e39  (62.361000,191.9
-000036d0: 3132 3530 3029 2220 6964 3d22 7368 6170  12500)" id="shap
-000036e0: 6534 3522 3e3c 7061 7468 2066 696c 6c2d  e45"><path fill-
-000036f0: 7275 6c65 3d22 6e6f 6e7a 6572 6f22 2066  rule="nonzero" f
-00003700: 696c 6c3d 2223 6666 6666 6666 2220 643d  ill="#ffffff" d=
-00003710: 224d 2e30 2c2e 304c 3535 2e30 2c2e 304c  "M.0,.0L55.0,.0L
-00003720: 3535 2e30 2c33 322e 334c 2e30 2c33 322e  55.0,32.3L.0,32.
-00003730: 334c 2e30 2c2e 307a 222f 3e3c 7061 7468  3L.0,.0z"/><path
-00003740: 2073 7472 6f6b 653d 2223 3435 3435 3435   stroke="#454545
-00003750: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
-00003760: 3422 2066 696c 6c3d 226e 6f6e 6522 2064  4" fill="none" d
-00003770: 3d22 4d2e 302c 3332 2e33 4c35 352e 302c  ="M.0,32.3L55.0,
-00003780: 3332 2e33 222f 3e3c 7465 7874 2078 6d6c  32.3"/><text xml
-00003790: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-000037a0: 2220 7374 796c 653d 2266 696c 6c3a 2333  " style="fill:#3
-000037b0: 3033 3033 303b 666f 6e74 2d66 616d 696c  03030;font-famil
-000037c0: 793a e5be aee8 bdaf e99b 85e9 bb91 3b66  y:............;f
-000037d0: 6f6e 742d 7369 7a65 3a31 312e 3030 7074  ont-size:11.00pt
-000037e0: 3b66 6f6e 742d 7765 6967 6874 3a62 6f6c  ;font-weight:bol
-000037f0: 6422 3e3c 7473 7061 6e20 783d 2231 322e  d"><tspan x="12.
-00003800: 3922 2079 3d22 3230 2e39 223e 432b 2b3c  9" y="20.9">C++<
+000036a0: 7465 7874 3e3c 2f67 3e3c 6720 6964 3d22  text></g><g id="
+000036b0: 7368 6170 6534 3522 2074 7261 6e73 666f  shape45" transfo
+000036c0: 726d 3d22 7472 616e 736c 6174 6528 3632  rm="translate(62
+000036d0: 2e33 3631 3030 302c 3139 312e 3931 3235  .361000,191.9125
+000036e0: 3030 2922 3e3c 7061 7468 2064 3d22 4d2e  00)"><path d="M.
+000036f0: 302c 2e30 4c35 352e 302c 2e30 4c35 352e  0,.0L55.0,.0L55.
+00003700: 302c 3332 2e33 4c2e 302c 3332 2e33 4c2e  0,32.3L.0,32.3L.
+00003710: 302c 2e30 7a22 2066 696c 6c2d 7275 6c65  0,.0z" fill-rule
+00003720: 3d22 6e6f 6e7a 6572 6f22 2066 696c 6c3d  ="nonzero" fill=
+00003730: 2223 6666 6666 6666 222f 3e3c 7061 7468  "#ffffff"/><path
+00003740: 2064 3d22 4d2e 302c 3332 2e33 4c35 352e   d="M.0,32.3L55.
+00003750: 302c 3332 2e33 2220 7374 726f 6b65 3d22  0,32.3" stroke="
+00003760: 2334 3534 3534 3522 2073 7472 6f6b 652d  #454545" stroke-
+00003770: 7769 6474 683d 2234 2220 6669 6c6c 3d22  width="4" fill="
+00003780: 6e6f 6e65 222f 3e3c 7465 7874 2073 7479  none"/><text sty
+00003790: 6c65 3d22 6669 6c6c 3a23 3330 3330 3330  le="fill:#303030
+000037a0: 3b66 6f6e 742d 6661 6d69 6c79 3ae5 beae  ;font-family:...
+000037b0: e8bd afe9 9b85 e9bb 913b 666f 6e74 2d73  .........;font-s
+000037c0: 697a 653a 3131 2e30 3070 743b 666f 6e74  ize:11.00pt;font
+000037d0: 2d77 6569 6768 743a 626f 6c64 2220 786d  -weight:bold" xm
+000037e0: 6c3a 7370 6163 653d 2270 7265 7365 7276  l:space="preserv
+000037f0: 6522 3e3c 7473 7061 6e20 793d 2232 302e  e"><tspan y="20.
+00003800: 3922 2078 3d22 3132 2e39 223e 432b 2b3c  9" x="12.9">C++<
 00003810: 2f74 7370 616e 3e3c 2f74 6578 743e 3c2f  /tspan></text></
-00003820: 673e 3c67 2074 7261 6e73 666f 726d 3d22  g><g transform="
-00003830: 7472 616e 736c 6174 6528 3637 2e33 3631  translate(67.361
-00003840: 3030 302c 3236 312e 3638 3735 3030 2922  000,261.687500)"
-00003850: 2069 643d 2273 6861 7065 3436 223e 3c70   id="shape46"><p
-00003860: 6174 6820 6669 6c6c 2d72 756c 653d 226e  ath fill-rule="n
-00003870: 6f6e 7a65 726f 2220 6669 6c6c 3d22 2366  onzero" fill="#f
-00003880: 6666 6666 6622 2064 3d22 4d2e 302c 2e30  fffff" d="M.0,.0
-00003890: 4c35 332e 302c 2e30 4c35 332e 302c 3332  L53.0,.0L53.0,32
-000038a0: 2e33 4c2e 302c 3332 2e33 4c2e 302c 2e30  .3L.0,32.3L.0,.0
-000038b0: 7a22 2f3e 3c70 6174 6820 7374 726f 6b65  z"/><path stroke
-000038c0: 3d22 2334 3534 3534 3522 2073 7472 6f6b  ="#454545" strok
-000038d0: 652d 7769 6474 683d 2234 2220 6669 6c6c  e-width="4" fill
-000038e0: 3d22 6e6f 6e65 2220 643d 224d 2e30 2c33  ="none" d="M.0,3
-000038f0: 322e 334c 3533 2e30 2c33 322e 3322 2f3e  2.3L53.0,32.3"/>
-00003900: 3c74 6578 7420 786d 6c3a 7370 6163 653d  <text xml:space=
-00003910: 2270 7265 7365 7276 6522 2073 7479 6c65  "preserve" style
-00003920: 3d22 6669 6c6c 3a23 3330 3330 3330 3b66  ="fill:#303030;f
-00003930: 6f6e 742d 6661 6d69 6c79 3ae5 beae e8bd  ont-family:.....
-00003940: afe9 9b85 e9bb 913b 666f 6e74 2d73 697a  .......;font-siz
-00003950: 653a 3131 2e30 3070 743b 666f 6e74 2d77  e:11.00pt;font-w
-00003960: 6569 6768 743a 626f 6c64 223e 3c74 7370  eight:bold"><tsp
-00003970: 616e 2078 3d22 3132 2e39 2220 793d 2232  an x="12.9" y="2
-00003980: 302e 3922 3e41 5053 3c2f 7473 7061 6e3e  0.9">APS</tspan>
-00003990: 3c2f 7465 7874 3e3c 2f67 3e3c 6720 7472  </text></g><g tr
-000039a0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-000039b0: 7465 2836 392e 3336 3130 3030 2c33 3032  te(69.361000,302
-000039c0: 2e36 3337 3530 3029 2220 6964 3d22 7368  .637500)" id="sh
-000039d0: 6170 6534 3722 3e3c 7061 7468 2066 696c  ape47"><path fil
-000039e0: 6c2d 7275 6c65 3d22 6e6f 6e7a 6572 6f22  l-rule="nonzero"
-000039f0: 2066 696c 6c3d 2223 6666 6666 6666 2220   fill="#ffffff" 
-00003a00: 643d 224d 2e30 2c2e 304c 3531 2e30 2c2e  d="M.0,.0L51.0,.
-00003a10: 304c 3531 2e30 2c33 322e 334c 2e30 2c33  0L51.0,32.3L.0,3
-00003a20: 322e 334c 2e30 2c2e 307a 222f 3e3c 7061  2.3L.0,.0z"/><pa
-00003a30: 7468 2073 7472 6f6b 653d 2223 3435 3435  th stroke="#4545
-00003a40: 3435 2220 7374 726f 6b65 2d77 6964 7468  45" stroke-width
-00003a50: 3d22 3422 2066 696c 6c3d 226e 6f6e 6522  ="4" fill="none"
-00003a60: 2064 3d22 4d2e 302c 3332 2e33 4c35 312e   d="M.0,32.3L51.
-00003a70: 302c 3332 2e33 222f 3e3c 7465 7874 2078  0,32.3"/><text x
-00003a80: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
-00003a90: 7665 2220 7374 796c 653d 2266 696c 6c3a  ve" style="fill:
-00003aa0: 2333 3033 3033 303b 666f 6e74 2d66 616d  #303030;font-fam
-00003ab0: 696c 793a e5be aee8 bdaf e99b 85e9 bb91  ily:............
-00003ac0: 3b66 6f6e 742d 7369 7a65 3a31 312e 3030  ;font-size:11.00
-00003ad0: 7074 3b66 6f6e 742d 7765 6967 6874 3a62  pt;font-weight:b
-00003ae0: 6f6c 6422 3e3c 7473 7061 6e20 783d 2231  old"><tspan x="1
-00003af0: 322e 3922 2079 3d22 3230 2e39 223e 5245  2.9" y="20.9">RE
+00003820: 673e 3c67 2069 643d 2273 6861 7065 3436  g><g id="shape46
+00003830: 2220 7472 616e 7366 6f72 6d3d 2274 7261  " transform="tra
+00003840: 6e73 6c61 7465 2836 372e 3336 3130 3030  nslate(67.361000
+00003850: 2c32 3631 2e36 3837 3530 3029 223e 3c70  ,261.687500)"><p
+00003860: 6174 6820 643d 224d 2e30 2c2e 304c 3533  ath d="M.0,.0L53
+00003870: 2e30 2c2e 304c 3533 2e30 2c33 322e 334c  .0,.0L53.0,32.3L
+00003880: 2e30 2c33 322e 334c 2e30 2c2e 307a 2220  .0,32.3L.0,.0z" 
+00003890: 6669 6c6c 2d72 756c 653d 226e 6f6e 7a65  fill-rule="nonze
+000038a0: 726f 2220 6669 6c6c 3d22 2366 6666 6666  ro" fill="#fffff
+000038b0: 6622 2f3e 3c70 6174 6820 643d 224d 2e30  f"/><path d="M.0
+000038c0: 2c33 322e 334c 3533 2e30 2c33 322e 3322  ,32.3L53.0,32.3"
+000038d0: 2073 7472 6f6b 653d 2223 3435 3435 3435   stroke="#454545
+000038e0: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
+000038f0: 3422 2066 696c 6c3d 226e 6f6e 6522 2f3e  4" fill="none"/>
+00003900: 3c74 6578 7420 7374 796c 653d 2266 696c  <text style="fil
+00003910: 6c3a 2333 3033 3033 303b 666f 6e74 2d66  l:#303030;font-f
+00003920: 616d 696c 793a e5be aee8 bdaf e99b 85e9  amily:..........
+00003930: bb91 3b66 6f6e 742d 7369 7a65 3a31 312e  ..;font-size:11.
+00003940: 3030 7074 3b66 6f6e 742d 7765 6967 6874  00pt;font-weight
+00003950: 3a62 6f6c 6422 2078 6d6c 3a73 7061 6365  :bold" xml:space
+00003960: 3d22 7072 6573 6572 7665 223e 3c74 7370  ="preserve"><tsp
+00003970: 616e 2079 3d22 3230 2e39 2220 783d 2231  an y="20.9" x="1
+00003980: 322e 3922 3e49 434d 3c2f 7473 7061 6e3e  2.9">ICM</tspan>
+00003990: 3c2f 7465 7874 3e3c 2f67 3e3c 6720 6964  </text></g><g id
+000039a0: 3d22 7368 6170 6534 3722 2074 7261 6e73  ="shape47" trans
+000039b0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+000039c0: 3639 2e33 3631 3030 302c 3330 322e 3633  69.361000,302.63
+000039d0: 3735 3030 2922 3e3c 7061 7468 2064 3d22  7500)"><path d="
+000039e0: 4d2e 302c 2e30 4c35 312e 302c 2e30 4c35  M.0,.0L51.0,.0L5
+000039f0: 312e 302c 3332 2e33 4c2e 302c 3332 2e33  1.0,32.3L.0,32.3
+00003a00: 4c2e 302c 2e30 7a22 2066 696c 6c2d 7275  L.0,.0z" fill-ru
+00003a10: 6c65 3d22 6e6f 6e7a 6572 6f22 2066 696c  le="nonzero" fil
+00003a20: 6c3d 2223 6666 6666 6666 222f 3e3c 7061  l="#ffffff"/><pa
+00003a30: 7468 2064 3d22 4d2e 302c 3332 2e33 4c35  th d="M.0,32.3L5
+00003a40: 312e 302c 3332 2e33 2220 7374 726f 6b65  1.0,32.3" stroke
+00003a50: 3d22 2334 3534 3534 3522 2073 7472 6f6b  ="#454545" strok
+00003a60: 652d 7769 6474 683d 2234 2220 6669 6c6c  e-width="4" fill
+00003a70: 3d22 6e6f 6e65 222f 3e3c 7465 7874 2073  ="none"/><text s
+00003a80: 7479 6c65 3d22 6669 6c6c 3a23 3330 3330  tyle="fill:#3030
+00003a90: 3330 3b66 6f6e 742d 6661 6d69 6c79 3ae5  30;font-family:.
+00003aa0: beae e8bd afe9 9b85 e9bb 913b 666f 6e74  ...........;font
+00003ab0: 2d73 697a 653a 3131 2e30 3070 743b 666f  -size:11.00pt;fo
+00003ac0: 6e74 2d77 6569 6768 743a 626f 6c64 2220  nt-weight:bold" 
+00003ad0: 786d 6c3a 7370 6163 653d 2270 7265 7365  xml:space="prese
+00003ae0: 7276 6522 3e3c 7473 7061 6e20 793d 2232  rve"><tspan y="2
+00003af0: 302e 3922 2078 3d22 3132 2e39 223e 5245  0.9" x="12.9">RE
 00003b00: 333c 2f74 7370 616e 3e3c 2f74 6578 743e  3</tspan></text>
-00003b10: 3c2f 673e 3c67 2074 7261 6e73 666f 726d  </g><g transform
-00003b20: 3d22 7472 616e 736c 6174 6528 3535 2e33  ="translate(55.3
-00003b30: 3631 3030 302c 3334 332e 3538 3735 3030  61000,343.587500
-00003b40: 2922 2069 643d 2273 6861 7065 3438 223e  )" id="shape48">
-00003b50: 3c70 6174 6820 6669 6c6c 2d72 756c 653d  <path fill-rule=
-00003b60: 226e 6f6e 7a65 726f 2220 6669 6c6c 3d22  "nonzero" fill="
-00003b70: 2366 6666 6666 6622 2064 3d22 4d2e 302c  #ffffff" d="M.0,
-00003b80: 2e30 4c36 352e 302c 2e30 4c36 352e 302c  .0L65.0,.0L65.0,
-00003b90: 3332 2e33 4c2e 302c 3332 2e33 4c2e 302c  32.3L.0,32.3L.0,
-00003ba0: 2e30 7a22 2f3e 3c70 6174 6820 7374 726f  .0z"/><path stro
-00003bb0: 6b65 3d22 2334 3534 3534 3522 2073 7472  ke="#454545" str
-00003bc0: 6f6b 652d 7769 6474 683d 2234 2220 6669  oke-width="4" fi
-00003bd0: 6c6c 3d22 6e6f 6e65 2220 643d 224d 2e30  ll="none" d="M.0
-00003be0: 2c33 322e 334c 3635 2e30 2c33 322e 3322  ,32.3L65.0,32.3"
-00003bf0: 2f3e 3c74 6578 7420 786d 6c3a 7370 6163  /><text xml:spac
-00003c00: 653d 2270 7265 7365 7276 6522 2073 7479  e="preserve" sty
-00003c10: 6c65 3d22 6669 6c6c 3a23 3330 3330 3330  le="fill:#303030
-00003c20: 3b66 6f6e 742d 6661 6d69 6c79 3ae5 beae  ;font-family:...
-00003c30: e8bd afe9 9b85 e9bb 913b 666f 6e74 2d73  .........;font-s
-00003c40: 697a 653a 3131 2e30 3070 743b 666f 6e74  ize:11.00pt;font
-00003c50: 2d77 6569 6768 743a 626f 6c64 223e 3c74  -weight:bold"><t
-00003c60: 7370 616e 2078 3d22 3132 2e39 2220 793d  span x="12.9" y=
-00003c70: 2232 302e 3922 3ec2 b7c2 b7c2 b7c2 b7c2  "20.9">.........
+00003b10: 3c2f 673e 3c67 2069 643d 2273 6861 7065  </g><g id="shape
+00003b20: 3438 2220 7472 616e 7366 6f72 6d3d 2274  48" transform="t
+00003b30: 7261 6e73 6c61 7465 2835 352e 3336 3130  ranslate(55.3610
+00003b40: 3030 2c33 3433 2e35 3837 3530 3029 223e  00,343.587500)">
+00003b50: 3c70 6174 6820 643d 224d 2e30 2c2e 304c  <path d="M.0,.0L
+00003b60: 3635 2e30 2c2e 304c 3635 2e30 2c33 322e  65.0,.0L65.0,32.
+00003b70: 334c 2e30 2c33 322e 334c 2e30 2c2e 307a  3L.0,32.3L.0,.0z
+00003b80: 2220 6669 6c6c 2d72 756c 653d 226e 6f6e  " fill-rule="non
+00003b90: 7a65 726f 2220 6669 6c6c 3d22 2366 6666  zero" fill="#fff
+00003ba0: 6666 6622 2f3e 3c70 6174 6820 643d 224d  fff"/><path d="M
+00003bb0: 2e30 2c33 322e 334c 3635 2e30 2c33 322e  .0,32.3L65.0,32.
+00003bc0: 3322 2073 7472 6f6b 653d 2223 3435 3435  3" stroke="#4545
+00003bd0: 3435 2220 7374 726f 6b65 2d77 6964 7468  45" stroke-width
+00003be0: 3d22 3422 2066 696c 6c3d 226e 6f6e 6522  ="4" fill="none"
+00003bf0: 2f3e 3c74 6578 7420 7374 796c 653d 2266  /><text style="f
+00003c00: 696c 6c3a 2333 3033 3033 303b 666f 6e74  ill:#303030;font
+00003c10: 2d66 616d 696c 793a e5be aee8 bdaf e99b  -family:........
+00003c20: 85e9 bb91 3b66 6f6e 742d 7369 7a65 3a31  ....;font-size:1
+00003c30: 312e 3030 7074 3b66 6f6e 742d 7765 6967  1.00pt;font-weig
+00003c40: 6874 3a62 6f6c 6422 2078 6d6c 3a73 7061  ht:bold" xml:spa
+00003c50: 6365 3d22 7072 6573 6572 7665 223e 3c74  ce="preserve"><t
+00003c60: 7370 616e 2079 3d22 3230 2e39 2220 783d  span y="20.9" x=
+00003c70: 2231 322e 3922 3ec2 b7c2 b7c2 b7c2 b7c2  "12.9">.........
 00003c80: b7c2 b73c 2f74 7370 616e 3e3c 2f74 6578  ...</tspan></tex
-00003c90: 743e 3c2f 673e 3c67 2074 7261 6e73 666f  t></g><g transfo
-00003ca0: 726d 3d22 7472 616e 736c 6174 6528 3630  rm="translate(60
-00003cb0: 2e33 3631 3030 302c 3434 392e 3738 3735  .361000,449.7875
-00003cc0: 3030 2922 2069 643d 2273 6861 7065 3439  00)" id="shape49
-00003cd0: 223e 3c70 6174 6820 6669 6c6c 2d72 756c  "><path fill-rul
-00003ce0: 653d 226e 6f6e 7a65 726f 2220 6669 6c6c  e="nonzero" fill
-00003cf0: 3d22 2366 6666 6666 6622 2064 3d22 4d2e  ="#ffffff" d="M.
-00003d00: 302c 2e30 4c31 3431 2e30 2c2e 304c 3134  0,.0L141.0,.0L14
-00003d10: 312e 302c 3332 2e33 4c2e 302c 3332 2e33  1.0,32.3L.0,32.3
-00003d20: 4c2e 302c 2e30 7a22 2f3e 3c70 6174 6820  L.0,.0z"/><path 
-00003d30: 7374 726f 6b65 3d22 2334 3534 3534 3522  stroke="#454545"
-00003d40: 2073 7472 6f6b 652d 7769 6474 683d 2234   stroke-width="4
-00003d50: 2220 6669 6c6c 3d22 6e6f 6e65 2220 643d  " fill="none" d=
-00003d60: 224d 2e30 2c33 322e 334c 3134 312e 302c  "M.0,32.3L141.0,
-00003d70: 3332 2e33 222f 3e3c 7465 7874 2078 6d6c  32.3"/><text xml
-00003d80: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-00003d90: 2220 7374 796c 653d 2266 696c 6c3a 2333  " style="fill:#3
-00003da0: 3033 3033 303b 666f 6e74 2d66 616d 696c  03030;font-famil
-00003db0: 793a e5be aee8 bdaf e99b 85e9 bb91 3b66  y:............;f
-00003dc0: 6f6e 742d 7369 7a65 3a31 312e 3030 7074  ont-size:11.00pt
-00003dd0: 3b66 6f6e 742d 7765 6967 6874 3a62 6f6c  ;font-weight:bol
-00003de0: 6422 3e3c 7473 7061 6e20 783d 2231 322e  d"><tspan x="12.
-00003df0: 3922 2079 3d22 3230 2e39 223e 5072 6f63  9" y="20.9">Proc
+00003c90: 743e 3c2f 673e 3c67 2069 643d 2273 6861  t></g><g id="sha
+00003ca0: 7065 3439 2220 7472 616e 7366 6f72 6d3d  pe49" transform=
+00003cb0: 2274 7261 6e73 6c61 7465 2836 302e 3336  "translate(60.36
+00003cc0: 3130 3030 2c34 3439 2e37 3837 3530 3029  1000,449.787500)
+00003cd0: 223e 3c70 6174 6820 643d 224d 2e30 2c2e  "><path d="M.0,.
+00003ce0: 304c 3134 312e 302c 2e30 4c31 3431 2e30  0L141.0,.0L141.0
+00003cf0: 2c33 322e 334c 2e30 2c33 322e 334c 2e30  ,32.3L.0,32.3L.0
+00003d00: 2c2e 307a 2220 6669 6c6c 2d72 756c 653d  ,.0z" fill-rule=
+00003d10: 226e 6f6e 7a65 726f 2220 6669 6c6c 3d22  "nonzero" fill="
+00003d20: 2366 6666 6666 6622 2f3e 3c70 6174 6820  #ffffff"/><path 
+00003d30: 643d 224d 2e30 2c33 322e 334c 3134 312e  d="M.0,32.3L141.
+00003d40: 302c 3332 2e33 2220 7374 726f 6b65 3d22  0,32.3" stroke="
+00003d50: 2334 3534 3534 3522 2073 7472 6f6b 652d  #454545" stroke-
+00003d60: 7769 6474 683d 2234 2220 6669 6c6c 3d22  width="4" fill="
+00003d70: 6e6f 6e65 222f 3e3c 7465 7874 2073 7479  none"/><text sty
+00003d80: 6c65 3d22 6669 6c6c 3a23 3330 3330 3330  le="fill:#303030
+00003d90: 3b66 6f6e 742d 6661 6d69 6c79 3ae5 beae  ;font-family:...
+00003da0: e8bd afe9 9b85 e9bb 913b 666f 6e74 2d73  .........;font-s
+00003db0: 697a 653a 3131 2e30 3070 743b 666f 6e74  ize:11.00pt;font
+00003dc0: 2d77 6569 6768 743a 626f 6c64 2220 786d  -weight:bold" xm
+00003dd0: 6c3a 7370 6163 653d 2270 7265 7365 7276  l:space="preserv
+00003de0: 6522 3e3c 7473 7061 6e20 793d 2232 302e  e"><tspan y="20.
+00003df0: 3922 2078 3d22 3132 2e39 223e 5072 6f63  9" x="12.9">Proc
 00003e00: 6765 6e20 4761 6d65 733c 2f74 7370 616e  gen Games</tspan
-00003e10: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2074  ></text></g><g t
-00003e20: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00003e30: 6174 6528 3133 362e 3336 3130 3030 2c34  ate(136.361000,4
-00003e40: 3930 2e37 3337 3530 3029 2220 6964 3d22  90.737500)" id="
-00003e50: 7368 6170 6535 3022 3e3c 7061 7468 2066  shape50"><path f
-00003e60: 696c 6c2d 7275 6c65 3d22 6e6f 6e7a 6572  ill-rule="nonzer
-00003e70: 6f22 2066 696c 6c3d 2223 6666 6666 6666  o" fill="#ffffff
-00003e80: 2220 643d 224d 2e30 2c2e 304c 3635 2e30  " d="M.0,.0L65.0
-00003e90: 2c2e 304c 3635 2e30 2c33 322e 334c 2e30  ,.0L65.0,32.3L.0
-00003ea0: 2c33 322e 334c 2e30 2c2e 307a 222f 3e3c  ,32.3L.0,.0z"/><
-00003eb0: 7061 7468 2073 7472 6f6b 653d 2223 3435  path stroke="#45
-00003ec0: 3435 3435 2220 7374 726f 6b65 2d77 6964  4545" stroke-wid
-00003ed0: 7468 3d22 3422 2066 696c 6c3d 226e 6f6e  th="4" fill="non
-00003ee0: 6522 2064 3d22 4d2e 302c 3332 2e33 4c36  e" d="M.0,32.3L6
-00003ef0: 352e 302c 3332 2e33 222f 3e3c 7465 7874  5.0,32.3"/><text
-00003f00: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
-00003f10: 6572 7665 2220 7374 796c 653d 2266 696c  erve" style="fil
-00003f20: 6c3a 2333 3033 3033 303b 666f 6e74 2d66  l:#303030;font-f
-00003f30: 616d 696c 793a e5be aee8 bdaf e99b 85e9  amily:..........
-00003f40: bb91 3b66 6f6e 742d 7369 7a65 3a31 312e  ..;font-size:11.
-00003f50: 3030 7074 3b66 6f6e 742d 7765 6967 6874  00pt;font-weight
-00003f60: 3a62 6f6c 6422 3e3c 7473 7061 6e20 783d  :bold"><tspan x=
-00003f70: 2231 322e 3922 2079 3d22 3230 2e39 223e  "12.9" y="20.9">
+00003e10: 3e3c 2f74 6578 743e 3c2f 673e 3c67 2069  ></text></g><g i
+00003e20: 643d 2273 6861 7065 3530 2220 7472 616e  d="shape50" tran
+00003e30: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00003e40: 2831 3336 2e33 3631 3030 302c 3439 302e  (136.361000,490.
+00003e50: 3733 3735 3030 2922 3e3c 7061 7468 2064  737500)"><path d
+00003e60: 3d22 4d2e 302c 2e30 4c36 352e 302c 2e30  ="M.0,.0L65.0,.0
+00003e70: 4c36 352e 302c 3332 2e33 4c2e 302c 3332  L65.0,32.3L.0,32
+00003e80: 2e33 4c2e 302c 2e30 7a22 2066 696c 6c2d  .3L.0,.0z" fill-
+00003e90: 7275 6c65 3d22 6e6f 6e7a 6572 6f22 2066  rule="nonzero" f
+00003ea0: 696c 6c3d 2223 6666 6666 6666 222f 3e3c  ill="#ffffff"/><
+00003eb0: 7061 7468 2064 3d22 4d2e 302c 3332 2e33  path d="M.0,32.3
+00003ec0: 4c36 352e 302c 3332 2e33 2220 7374 726f  L65.0,32.3" stro
+00003ed0: 6b65 3d22 2334 3534 3534 3522 2073 7472  ke="#454545" str
+00003ee0: 6f6b 652d 7769 6474 683d 2234 2220 6669  oke-width="4" fi
+00003ef0: 6c6c 3d22 6e6f 6e65 222f 3e3c 7465 7874  ll="none"/><text
+00003f00: 2073 7479 6c65 3d22 6669 6c6c 3a23 3330   style="fill:#30
+00003f10: 3330 3330 3b66 6f6e 742d 6661 6d69 6c79  3030;font-family
+00003f20: 3ae5 beae e8bd afe9 9b85 e9bb 913b 666f  :............;fo
+00003f30: 6e74 2d73 697a 653a 3131 2e30 3070 743b  nt-size:11.00pt;
+00003f40: 666f 6e74 2d77 6569 6768 743a 626f 6c64  font-weight:bold
+00003f50: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
+00003f60: 7365 7276 6522 3e3c 7473 7061 6e20 793d  serve"><tspan y=
+00003f70: 2232 302e 3922 2078 3d22 3132 2e39 223e  "20.9" x="12.9">
 00003f80: c2b7 c2b7 c2b7 c2b7 c2b7 c2b7 3c2f 7473  ............</ts
 00003f90: 7061 6e3e 3c2f 7465 7874 3e3c 2f67 3e3c  pan></text></g><
-00003fa0: 6720 7472 616e 7366 6f72 6d3d 2274 7261  g transform="tra
-00003fb0: 6e73 6c61 7465 2831 3630 2e33 3631 3030  nslate(160.36100
-00003fc0: 302c 3637 2e39 3632 3530 3029 2220 6964  0,67.962500)" id
-00003fd0: 3d22 7368 6170 6535 3122 3e3c 7061 7468  ="shape51"><path
-00003fe0: 2066 696c 6c2d 7275 6c65 3d22 6e6f 6e7a   fill-rule="nonz
-00003ff0: 6572 6f22 2073 7472 6f6b 653d 2223 3435  ero" stroke="#45
-00004000: 3435 3435 2220 7374 726f 6b65 2d77 6964  4545" stroke-wid
-00004010: 7468 3d22 3422 2066 696c 6c3d 2223 6666  th="4" fill="#ff
-00004020: 6666 6666 2220 643d 224d 342e 302c 2e30  ffff" d="M4.0,.0
-00004030: 4c31 3431 2e30 2c2e 3043 3134 332e 322c  L141.0,.0C143.2,
-00004040: 2e30 2c31 3435 2e30 2c31 2e38 2c31 3435  .0,145.0,1.8,145
-00004050: 2e30 2c34 2e30 4c31 3435 2e30 2c34 362e  .0,4.0L145.0,46.
-00004060: 3043 3134 352e 302c 3438 2e32 2c31 3433  0C145.0,48.2,143
-00004070: 2e32 2c35 302e 302c 3134 312e 302c 3530  .2,50.0,141.0,50
-00004080: 2e30 4c34 2e30 2c35 302e 3043 312e 382c  .0L4.0,50.0C1.8,
-00004090: 3530 2e30 2c2e 302c 3438 2e32 2c2e 302c  50.0,.0,48.2,.0,
-000040a0: 3436 2e30 4c2e 302c 342e 3043 2e30 2c31  46.0L.0,4.0C.0,1
-000040b0: 2e38 2c31 2e38 2c2e 302c 342e 302c 2e30  .8,1.8,.0,4.0,.0
-000040c0: 7a22 2f3e 3c74 6578 7420 786d 6c3a 7370  z"/><text xml:sp
-000040d0: 6163 653d 2270 7265 7365 7276 6522 2073  ace="preserve" s
-000040e0: 7479 6c65 3d22 6669 6c6c 3a23 3330 3330  tyle="fill:#3030
-000040f0: 3330 3b66 6f6e 742d 6661 6d69 6c79 3ae5  30;font-family:.
-00004100: beae e8bd afe9 9b85 e9bb 913b 666f 6e74  ...........;font
-00004110: 2d73 697a 653a 3134 2e30 3070 743b 666f  -size:14.00pt;fo
-00004120: 6e74 2d77 6569 6768 743a 626f 6c64 223e  nt-weight:bold">
-00004130: 3c74 7370 616e 2078 3d22 3234 2e33 2220  <tspan x="24.3" 
-00004140: 793d 2233 322e 3022 3e45 7661 6c75 6174  y="32.0">Evaluat
+00003fa0: 6720 6964 3d22 7368 6170 6535 3122 2074  g id="shape51" t
+00003fb0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00003fc0: 6174 6528 3136 302e 3336 3130 3030 2c36  ate(160.361000,6
+00003fd0: 372e 3936 3235 3030 2922 3e3c 7061 7468  7.962500)"><path
+00003fe0: 2064 3d22 4d34 2e30 2c2e 304c 3134 312e   d="M4.0,.0L141.
+00003ff0: 302c 2e30 4331 3433 2e32 2c2e 302c 3134  0,.0C143.2,.0,14
+00004000: 352e 302c 312e 382c 3134 352e 302c 342e  5.0,1.8,145.0,4.
+00004010: 304c 3134 352e 302c 3436 2e30 4331 3435  0L145.0,46.0C145
+00004020: 2e30 2c34 382e 322c 3134 332e 322c 3530  .0,48.2,143.2,50
+00004030: 2e30 2c31 3431 2e30 2c35 302e 304c 342e  .0,141.0,50.0L4.
+00004040: 302c 3530 2e30 4331 2e38 2c35 302e 302c  0,50.0C1.8,50.0,
+00004050: 2e30 2c34 382e 322c 2e30 2c34 362e 304c  .0,48.2,.0,46.0L
+00004060: 2e30 2c34 2e30 432e 302c 312e 382c 312e  .0,4.0C.0,1.8,1.
+00004070: 382c 2e30 2c34 2e30 2c2e 307a 2220 7374  8,.0,4.0,.0z" st
+00004080: 726f 6b65 3d22 2334 3534 3534 3522 2073  roke="#454545" s
+00004090: 7472 6f6b 652d 7769 6474 683d 2234 2220  troke-width="4" 
+000040a0: 6669 6c6c 2d72 756c 653d 226e 6f6e 7a65  fill-rule="nonze
+000040b0: 726f 2220 6669 6c6c 3d22 2366 6666 6666  ro" fill="#fffff
+000040c0: 6622 2f3e 3c74 6578 7420 7374 796c 653d  f"/><text style=
+000040d0: 2266 696c 6c3a 2333 3033 3033 303b 666f  "fill:#303030;fo
+000040e0: 6e74 2d66 616d 696c 793a e5be aee8 bdaf  nt-family:......
+000040f0: e99b 85e9 bb91 3b66 6f6e 742d 7369 7a65  ......;font-size
+00004100: 3a31 342e 3030 7074 3b66 6f6e 742d 7765  :14.00pt;font-we
+00004110: 6967 6874 3a62 6f6c 6422 2078 6d6c 3a73  ight:bold" xml:s
+00004120: 7061 6365 3d22 7072 6573 6572 7665 223e  pace="preserve">
+00004130: 3c74 7370 616e 2079 3d22 3332 2e30 2220  <tspan y="32.0" 
+00004140: 783d 2232 342e 3322 3e45 7661 6c75 6174  x="24.3">Evaluat
 00004150: 696f 6e3c 2f74 7370 616e 3e3c 2f74 6578  ion</tspan></tex
-00004160: 743e 3c2f 673e 3c67 2074 7261 6e73 666f  t></g><g transfo
-00004170: 726d 3d22 7472 616e 736c 6174 6528 3439  rm="translate(49
-00004180: 2e33 3631 3030 302c 3430 2e32 3337 3530  .361000,40.23750
-00004190: 3029 2220 6964 3d22 7368 6170 6535 3222  0)" id="shape52"
-000041a0: 3e3c 7061 7468 2066 696c 6c2d 7275 6c65  ><path fill-rule
-000041b0: 3d22 6e6f 6e7a 6572 6f22 2066 696c 6c3d  ="nonzero" fill=
-000041c0: 2223 6666 6666 6666 2220 643d 224d 2e30  "#ffffff" d="M.0
-000041d0: 2c2e 304c 3836 2e30 2c2e 304c 3836 2e30  ,.0L86.0,.0L86.0
-000041e0: 2c33 322e 334c 2e30 2c33 322e 334c 2e30  ,32.3L.0,32.3L.0
-000041f0: 2c2e 307a 222f 3e3c 7061 7468 2073 7472  ,.0z"/><path str
-00004200: 6f6b 653d 2223 3435 3435 3435 2220 7374  oke="#454545" st
-00004210: 726f 6b65 2d77 6964 7468 3d22 3422 2066  roke-width="4" f
-00004220: 696c 6c3d 226e 6f6e 6522 2064 3d22 4d2e  ill="none" d="M.
-00004230: 302c 3332 2e33 4c38 362e 302c 3332 2e33  0,32.3L86.0,32.3
-00004240: 222f 3e3c 7465 7874 2078 6d6c 3a73 7061  "/><text xml:spa
-00004250: 6365 3d22 7072 6573 6572 7665 2220 7374  ce="preserve" st
-00004260: 796c 653d 2266 696c 6c3a 2333 3033 3033  yle="fill:#30303
-00004270: 303b 666f 6e74 2d66 616d 696c 793a e5be  0;font-family:..
-00004280: aee8 bdaf e99b 85e9 bb91 3b66 6f6e 742d  ..........;font-
-00004290: 7369 7a65 3a31 312e 3030 7074 3b66 6f6e  size:11.00pt;fon
-000042a0: 742d 7765 6967 6874 3a62 6f6c 6422 3e3c  t-weight:bold"><
-000042b0: 7473 7061 6e20 783d 2231 322e 3922 2079  tspan x="12.9" y
-000042c0: 3d22 3230 2e39 223e 4951 4d2c 204f 473c  ="20.9">IQM, OG<
+00004160: 743e 3c2f 673e 3c67 2069 643d 2273 6861  t></g><g id="sha
+00004170: 7065 3532 2220 7472 616e 7366 6f72 6d3d  pe52" transform=
+00004180: 2274 7261 6e73 6c61 7465 2834 392e 3336  "translate(49.36
+00004190: 3130 3030 2c34 302e 3233 3735 3030 2922  1000,40.237500)"
+000041a0: 3e3c 7061 7468 2064 3d22 4d2e 302c 2e30  ><path d="M.0,.0
+000041b0: 4c38 362e 302c 2e30 4c38 362e 302c 3332  L86.0,.0L86.0,32
+000041c0: 2e33 4c2e 302c 3332 2e33 4c2e 302c 2e30  .3L.0,32.3L.0,.0
+000041d0: 7a22 2066 696c 6c2d 7275 6c65 3d22 6e6f  z" fill-rule="no
+000041e0: 6e7a 6572 6f22 2066 696c 6c3d 2223 6666  nzero" fill="#ff
+000041f0: 6666 6666 222f 3e3c 7061 7468 2064 3d22  ffff"/><path d="
+00004200: 4d2e 302c 3332 2e33 4c38 362e 302c 3332  M.0,32.3L86.0,32
+00004210: 2e33 2220 7374 726f 6b65 3d22 2334 3534  .3" stroke="#454
+00004220: 3534 3522 2073 7472 6f6b 652d 7769 6474  545" stroke-widt
+00004230: 683d 2234 2220 6669 6c6c 3d22 6e6f 6e65  h="4" fill="none
+00004240: 222f 3e3c 7465 7874 2073 7479 6c65 3d22  "/><text style="
+00004250: 6669 6c6c 3a23 3330 3330 3330 3b66 6f6e  fill:#303030;fon
+00004260: 742d 6661 6d69 6c79 3ae5 beae e8bd afe9  t-family:.......
+00004270: 9b85 e9bb 913b 666f 6e74 2d73 697a 653a  .....;font-size:
+00004280: 3131 2e30 3070 743b 666f 6e74 2d77 6569  11.00pt;font-wei
+00004290: 6768 743a 626f 6c64 2220 786d 6c3a 7370  ght:bold" xml:sp
+000042a0: 6163 653d 2270 7265 7365 7276 6522 3e3c  ace="preserve"><
+000042b0: 7473 7061 6e20 793d 2232 302e 3922 2078  tspan y="20.9" x
+000042c0: 3d22 3132 2e39 223e 4951 4d2c 204f 473c  ="12.9">IQM, OG<
 000042d0: 2f74 7370 616e 3e3c 2f74 6578 743e 3c2f  /tspan></text></
-000042e0: 673e 3c67 2074 7261 6e73 666f 726d 3d22  g><g transform="
-000042f0: 7472 616e 736c 6174 6528 3730 2e33 3631  translate(70.361
-00004300: 3030 302c 3831 2e31 3837 3530 3029 2220  000,81.187500)" 
-00004310: 6964 3d22 7368 6170 6535 3322 3e3c 7061  id="shape53"><pa
-00004320: 7468 2066 696c 6c2d 7275 6c65 3d22 6e6f  th fill-rule="no
-00004330: 6e7a 6572 6f22 2066 696c 6c3d 2223 6666  nzero" fill="#ff
-00004340: 6666 6666 2220 643d 224d 2e30 2c2e 304c  ffff" d="M.0,.0L
-00004350: 3635 2e30 2c2e 304c 3635 2e30 2c33 322e  65.0,.0L65.0,32.
-00004360: 334c 2e30 2c33 322e 334c 2e30 2c2e 307a  3L.0,32.3L.0,.0z
-00004370: 222f 3e3c 7061 7468 2073 7472 6f6b 653d  "/><path stroke=
-00004380: 2223 3435 3435 3435 2220 7374 726f 6b65  "#454545" stroke
-00004390: 2d77 6964 7468 3d22 3422 2066 696c 6c3d  -width="4" fill=
-000043a0: 226e 6f6e 6522 2064 3d22 4d2e 302c 3332  "none" d="M.0,32
-000043b0: 2e33 4c36 352e 302c 3332 2e33 222f 3e3c  .3L65.0,32.3"/><
-000043c0: 7465 7874 2078 6d6c 3a73 7061 6365 3d22  text xml:space="
-000043d0: 7072 6573 6572 7665 2220 7374 796c 653d  preserve" style=
-000043e0: 2266 696c 6c3a 2333 3033 3033 303b 666f  "fill:#303030;fo
-000043f0: 6e74 2d66 616d 696c 793a e5be aee8 bdaf  nt-family:......
-00004400: e99b 85e9 bb91 3b66 6f6e 742d 7369 7a65  ......;font-size
-00004410: 3a31 312e 3030 7074 3b66 6f6e 742d 7765  :11.00pt;font-we
-00004420: 6967 6874 3a62 6f6c 6422 3e3c 7473 7061  ight:bold"><tspa
-00004430: 6e20 783d 2231 312e 3922 2079 3d22 3230  n x="11.9" y="20
+000042e0: 673e 3c67 2069 643d 2273 6861 7065 3533  g><g id="shape53
+000042f0: 2220 7472 616e 7366 6f72 6d3d 2274 7261  " transform="tra
+00004300: 6e73 6c61 7465 2837 302e 3336 3130 3030  nslate(70.361000
+00004310: 2c38 312e 3138 3735 3030 2922 3e3c 7061  ,81.187500)"><pa
+00004320: 7468 2064 3d22 4d2e 302c 2e30 4c36 352e  th d="M.0,.0L65.
+00004330: 302c 2e30 4c36 352e 302c 3332 2e33 4c2e  0,.0L65.0,32.3L.
+00004340: 302c 3332 2e33 4c2e 302c 2e30 7a22 2066  0,32.3L.0,.0z" f
+00004350: 696c 6c2d 7275 6c65 3d22 6e6f 6e7a 6572  ill-rule="nonzer
+00004360: 6f22 2066 696c 6c3d 2223 6666 6666 6666  o" fill="#ffffff
+00004370: 222f 3e3c 7061 7468 2064 3d22 4d2e 302c  "/><path d="M.0,
+00004380: 3332 2e33 4c36 352e 302c 3332 2e33 2220  32.3L65.0,32.3" 
+00004390: 7374 726f 6b65 3d22 2334 3534 3534 3522  stroke="#454545"
+000043a0: 2073 7472 6f6b 652d 7769 6474 683d 2234   stroke-width="4
+000043b0: 2220 6669 6c6c 3d22 6e6f 6e65 222f 3e3c  " fill="none"/><
+000043c0: 7465 7874 2073 7479 6c65 3d22 6669 6c6c  text style="fill
+000043d0: 3a23 3330 3330 3330 3b66 6f6e 742d 6661  :#303030;font-fa
+000043e0: 6d69 6c79 3ae5 beae e8bd afe9 9b85 e9bb  mily:...........
+000043f0: 913b 666f 6e74 2d73 697a 653a 3131 2e30  .;font-size:11.0
+00004400: 3070 743b 666f 6e74 2d77 6569 6768 743a  0pt;font-weight:
+00004410: 626f 6c64 2220 786d 6c3a 7370 6163 653d  bold" xml:space=
+00004420: 2270 7265 7365 7276 6522 3e3c 7473 7061  "preserve"><tspa
+00004430: 6e20 793d 2232 302e 3922 2078 3d22 3131  n y="20.9" x="11
 00004440: 2e39 223e c2b7 c2b7 c2b7 c2b7 c2b7 c2b7  .9">............
 00004450: 3c2f 7473 7061 6e3e 3c2f 7465 7874 3e3c  </tspan></text><
 00004460: 2f67 3e3c 2f67 3e3c 2f73 7667 3e         /g></g></svg>
```

### Comparing `hsuanwu-0.0.1b4/docs/tutorials/quick_start.md` & `hsuanwu-0.0.1b5/docs/tutorials/quick_start.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## Build Application
 
-Hsuanwu uses [Hydra](hydra.cc) to manage RL applications elegantly. For example, 
+Hsuanwu uses [Hydra](https://hydra.cc/) to manage RL applications elegantly. For example, 
 we want to use [DrQ-v2](https://openreview.net/forum?id=_SJ-_yyes8) to solve a task of DeepMind Control Suite, and we only need the following two steps:
 
 1. Write a `config.yaml` file in your working directory like:
 ``` yaml title="config.yaml"
 experiment: drqv2_dmc     # Experiment ID.
 device: cuda:0            # Device (cpu, cuda, ...).
 seed: 1                   # Random seed for reproduction.
@@ -55,14 +55,27 @@
 num_train_steps: 5000     # Number of training steps.
 
 agent:
   name: DrQv2             # The agent name.
 
 hydra:
 run:
-  dir: ./logs/${experiment}/${now:%Y.%m.%d}/${now:%H%M%S}_${hydra.job.override_dirname} # Used to specify the output directory.
+  dir: ./logs/${experiment}/${now:%Y.%m.%d}/${now:%H%M%S}_${hydra.job.override_dirname} # Specify the output directory.
 job:
   chdir: true # Change the working working.
 ```
 
 ## Load the Trained Model
-Once the training is finished, you can find the trained model in the subfolder `model` of the specified working directory.
+Once the training is finished, you can find `encoder.pth` and `actor.pth` in the subfolder `model` of the specified working directory.
+
+``` py title="play.py"
+import torch as th
+
+# load the model and specify the map location
+encoder = th.load("encoder.pth", map_location=th.device('cpu'))
+actor = th.load("actor.pth", map_location=th.device('cpu'))
+obs = th.zeros(size=(1, 9, 84, 84))
+action = actor(encoder(obs))
+print(action)
+
+# Output: tensor([[-1.0000]], grad_fn=<TanhBackward0>)
+```
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/verification.py` & `hsuanwu-0.0.1b5/hsuanwu/verification.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 import gymnasium as gym
+from gym.vector import SyncVectorEnv
 from omegaconf import OmegaConf
+from termcolor import colored
+
 from hsuanwu.common.engine import HsuanwuEngine
 from hsuanwu.env.utils import HsuanwuEnvWrapper
-from termcolor import colored
+
 
 def make_env():
     def _thunk():
         return gym.make("Acrobot-v1")
 
     return _thunk
 
-gym_env = gym.vector.SyncVectorEnv([make_env() for _ in range(1)])
+
+gym_env = SyncVectorEnv([make_env() for _ in range(1)])
 gym_env = gym.wrappers.RecordEpisodeStatistics(gym_env)
-train_env = HsuanwuEnvWrapper(gym_env, device='cpu')
+train_env = HsuanwuEnvWrapper(gym_env, device="cpu")
 
 cfgs = {
-    'experiment': 'Verification',
-    'device': 'cpu',
-    'seed': 1,
-    'num_train_steps': 5000,
-    'agent': {
-        'name': 'PPO'
-    },
-    'encoder': {
-        'name': 'IdentityEncoder'
-    },
+    "experiment": "Verification",
+    "device": "cpu",
+    "seed": 1,
+    "num_train_steps": 5000,
+    "agent": {"name": "PPO"},
+    "encoder": {"name": "IdentityEncoder"},
 }
 cfgs = OmegaConf.create(cfgs)
 
-if __name__ == '__main__':
-    engine = HsuanwuEngine(
-        cfgs=cfgs,
-        train_env=train_env
-    )
+if __name__ == "__main__":
+    engine = HsuanwuEngine(cfgs=cfgs, train_env=train_env)
     try:
         engine.invoke()
-        print(colored('Verification Passed!'.upper(), "green", attrs=["bold"]))
+        print(colored("Verification Passed!".upper(), "green", attrs=["bold"]))
     except RuntimeError:
-        print(colored('Verification failed!'.upper(), "red", attrs=["bold"]))
+        print(colored("Verification failed!".upper(), "red", attrs=["bold"]))
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/common/logger.py` & `hsuanwu-0.0.1b5/hsuanwu/common/logger.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/common/engine/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/common/engine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from hsuanwu.xploit.agent import ALL_DEFAULT_CFGS, ALL_MATCH_KEYS
 
 from .base_policy_trainer import BasePolicyTrainer as BasePolicyTrainer
 from .distributed_trainer import DistributedTrainer as DistributedTrainer
 from .off_policy_trainer import OffPolicyTrainer as OffPolicyTrainer
 from .on_policy_trainer import OnPolicyTrainer as OnPolicyTrainer
 
+
 class HsuanwuEngine:
     """Hsuanwu RL engine.
 
     Args:
         cfgs (DictConfig): Dict config for configuring RL algorithms.
         train_env (Env): A Gym-like environment for training.
         test_env (Env): A Gym-like environment for testing.
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/common/engine/base_policy_trainer.py` & `hsuanwu-0.0.1b5/hsuanwu/common/engine/base_policy_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     # Mandatory parameters
     ## TODO: Train setup
     "device": "cpu",
     "seed": 1,
     "num_train_steps": 100000,
     "num_init_steps": 2000,  # only for off-policy algorithms
     "pretraining": False,
+    "init_model_path": None,
     ## TODO: Test setup
     "test_every_steps": 5000,  # only for off-policy algorithms
     "test_every_episodes": 10,  # only for on-policy algorithms
     "num_test_episodes": 10,
     ## TODO: xploit part
     "encoder": {
         "name": None,
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/common/engine/distributed_trainer.py` & `hsuanwu-0.0.1b5/hsuanwu/common/engine/distributed_trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,20 +30,27 @@
         Processed env.
     """
 
     def __init__(self, env: gym.Env) -> None:
         self.env = env
         self.episode_return = None
         self.episode_step = None
+        if env.action_space.__class__.__name__ == "Discrete":
+            self.action_type = "Discrete"
+            self.action_dim = 1
+        elif env.action_space.__class__.__name__ == "Box":
+            self.action_type = "Box"
+            self.action_dim = env.action_space.shape[0]
+        else:
+            raise NotImplementedError("Unsupported action type!")
 
     def reset(self, seed) -> Dict[str, th.Tensor]:
         """Reset the environment."""
         init_reward = th.zeros(1, 1)
-        # This supports only single-tensor actions ATM.
-        init_last_action = th.zeros(1, 1, dtype=th.int64)
+        init_last_action = th.zeros(1, self.action_dim, dtype=th.int64)
         self.episode_return = th.zeros(1, 1)
         self.episode_step = th.zeros(1, 1, dtype=th.int32)
         init_terminated = th.ones(1, 1, dtype=th.uint8)
         init_truncated = th.ones(1, 1, dtype=th.uint8)
 
         obs, info = self.env.reset(seed=seed)
         obs = self._format_obs(obs)
@@ -63,15 +70,22 @@
 
         Args:
             action (Tensor): Action tensor.
 
         Returns:
             Step information dict.
         """
-        obs, reward, terminated, truncated, info = self.env.step(action.item())
+        if self.action_type == "Discrete":
+            _action = action.item()
+        elif self.action_type == "Box":
+            _action = action.squeeze(0).cpu().numpy()
+        else:
+            raise NotImplementedError("Unsupported action type!")
+
+        obs, reward, terminated, truncated, info = self.env.step(_action)
         self.episode_step += 1
         self.episode_return += reward
         episode_step = self.episode_step
         episode_return = self.episode_return
         if terminated or truncated:
             obs, info = self.env.reset()
             self.episode_return = th.zeros(1, 1)
@@ -122,50 +136,39 @@
     """
 
     def __init__(self, cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None) -> None:
         super().__init__(cfgs, train_env, test_env)
         self._logger.info("Deploying DistributedTrainer...")
         # xploit part
         self._agent = hydra.utils.instantiate(self._cfgs.agent)
-        self._agent.actor.encoder = hydra.utils.instantiate(self._cfgs.encoder)
-        self._agent.learner.encoder = hydra.utils.instantiate(self._cfgs.encoder)
-
-        self._agent.actor.share_memory()
-        self._agent.learner.to(self._device)
-        self._agent.opt = th.optim.RMSprop(
-            self._agent.learner.parameters(),
-            lr=self._agent.lr,
-            eps=self._agent.eps,
-        )
-
-        def lr_lambda(epoch):
-            return (
-                1.0
-                - min(
-                    epoch * self._cfgs.num_steps * self._cfgs.num_learners,
-                    self._cfgs.num_train_steps,
-                )
-                / self._cfgs.num_train_steps
-            )
-
-        self._agent.lr_scheduler = th.optim.lr_scheduler.LambdaLR(self._agent.opt, lr_lambda)
+        encoder = hydra.utils.instantiate(self._cfgs.encoder)
 
         ## TODO: build storage
         self._shared_storages = hydra.utils.instantiate(self._cfgs.storage)
         self._train_env = self._train_env.envs
 
         # xplore part
         ## TODO: build distribution
         if "Noise" in self._cfgs.distribution._target_:
             dist = hydra.utils.instantiate(self._cfgs.distribution)
         else:
             dist = hydra.utils.get_class(self._cfgs.distribution._target_)
 
-        self._agent.actor.dist = dist
-        self._agent.learner.dist = dist
+        def lr_lambda(epoch):
+            return (
+                1.0
+                - min(
+                    epoch * self._cfgs.num_steps * self._cfgs.num_learners,
+                    self._cfgs.num_train_steps,
+                )
+                / self._cfgs.num_train_steps
+            )
+
+        # TODO: Integrate agent and modules
+        self._agent.integrate(encoder=encoder, dist=dist, lr_lambda=lr_lambda)
 
     @staticmethod
     def act(  # noqa: C901
         cfgs: omegaconf.DictConfig,
         logger: Logger,
         gym_env: gym.Env,
         actor_idx: int,
@@ -305,14 +308,15 @@
         for i in range(self._cfgs.num_learners):
             thread = threading.Thread(target=sample_and_update, name="sample-and-update-%d" % i, args=(i,))
             thread.start()
             self._logger.info(f"Learner {i} started!")
             threads.append(thread)
 
         try:
+            log_times = 0
             while global_step < self._cfgs.num_train_steps:
                 start_step = global_step
                 time.sleep(5)
 
                 if metrics.get("episode_returns"):
                     episode_rewards.extend(metrics["episode_returns"])
                     episode_steps.extend(metrics["episode_steps"])
@@ -324,14 +328,25 @@
                         "episode": global_episode,
                         "episode_length": np.mean(episode_steps),
                         "episode_reward": np.mean(episode_rewards),
                         "fps": (global_step - start_step) / episode_time,
                         "total_time": total_time,
                     }
                     self._logger.train(msg=train_metrics)
+                    log_times += 1
+
+                # if log_times % 50 == 0:
+                #     episode_time, total_time = self._timer.reset()
+                #     test_metrics = self.test()
+                #     test_metrics.update({
+                #         "step": global_step,
+                #         "episode": global_episode,
+                #         "total_time": total_time,
+                #         })
+                #     self._logger.test(msg=test_metrics)
 
         except KeyboardInterrupt:
             # TODO: join actors then quit.
             return
         else:
             for thread in threads:
                 thread.join()
@@ -342,15 +357,32 @@
             for _ in range(self._cfgs.num_actors):
                 free_queue.put(None)
             for actor in actor_pool:
                 actor.join(timeout=1)
 
     def test(self) -> Dict[str, float]:
         """Testing function."""
-        return {"step": 0}
+        env = Environment(self._test_env.envs[0])
+        seed = self._cfgs.num_actors * int.from_bytes(os.urandom(4), byteorder="little")
+        env_output = env.reset(seed)
+
+        episode_rewards = list()
+        episode_steps = list()
+        while len(episode_rewards) < self._cfgs.num_test_episodes:
+            with th.no_grad():
+                actor_output, _ = self._agent.actor.get_action(env_output, training=False)
+            env_output = env.step(actor_output["action"])
+            if env_output["terminated"].item() or env_output["truncated"].item():
+                episode_rewards.append(env_output["episode_return"].item())
+                episode_steps.append(env_output["episode_step"].item())
+
+        return {
+            "episode_length": np.mean(episode_steps),
+            "episode_reward": np.mean(episode_rewards),
+        }
 
     def save(self) -> None:
         """Save the trained model."""
         save_dir = Path.cwd() / "model"
         save_dir.mkdir(exist_ok=True)
-        th.save(self._agent.actor, save_dir / "actor.pth")
-        th.save(self._agent.learner, save_dir / "learner.pth")
+        self._agent.save(path=save_dir)
+        self._logger.info(f"Model saved at: {save_dir}")
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/common/engine/off_policy_trainer.py` & `hsuanwu-0.0.1b5/hsuanwu/common/engine/on_policy_trainer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,200 +1,170 @@
+from collections import deque
 from pathlib import Path
-from typing import Dict, Iterable
+from typing import Dict
 
 import gymnasium as gym
 import hydra
 import numpy as np
 import omegaconf
 import torch as th
 
 from hsuanwu.common.engine.base_policy_trainer import BasePolicyTrainer
 from hsuanwu.common.engine.utils import eval_mode
-from hsuanwu.xploit.storage.utils import worker_init_fn
 
 
-class OffPolicyTrainer(BasePolicyTrainer):
-    """Trainer for off-policy algorithms.
+class OnPolicyTrainer(BasePolicyTrainer):
+    """Trainer for on-policy algorithms.
 
     Args:
         cfgs (DictConfig): Dict config for configuring RL algorithms.
         train_env (Env): A Gym-like environment for training.
         test_env (Env): A Gym-like environment for testing.
 
     Returns:
-        Off-policy trainer instance.
+        On-policy trainer instance.
     """
 
     def __init__(self, cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None) -> None:
         super().__init__(cfgs, train_env, test_env)
-        self._logger.info("Deploying OffPolicyTrainer...")
+        self._logger.info("Deploying OnPolicyTrainer...")
         # TODO: turn on the pretraining mode, no extrinsic rewards will be provided.
         if self._cfgs.pretraining:
             self._logger.info("Pre-training Mode On...")
         # xploit part
         self._agent = hydra.utils.instantiate(self._cfgs.agent)
-        ## TODO: build encoder
-        self._agent.encoder = hydra.utils.instantiate(self._cfgs.encoder).to(self._device)
-        self._agent.encoder.train()
-        self._agent.encoder_opt = th.optim.Adam(
-            self._agent.encoder.parameters(),
-            lr=self._agent.lr,
-            eps=self._agent.eps,
-        )
-        ## TODO: build storage
-        self._replay_storage = hydra.utils.instantiate(self._cfgs.storage)
+        # TODO: build encoder
+        encoder = hydra.utils.instantiate(self._cfgs.encoder).to(self._device)
+        # TODO: build storage
+        self._rollout_storage = hydra.utils.instantiate(self._cfgs.storage)
 
         # xplore part
-        ## TODO: get distribution
-        if "Noise" in self._cfgs.distribution._target_:
-            dist = hydra.utils.instantiate(self._cfgs.distribution)
-        else:
-            dist = hydra.utils.get_class(self._cfgs.distribution._target_)
-        self._agent.dist = dist
-        self._agent.actor.dist = dist
+        # TODO: get distribution
+        dist = hydra.utils.get_class(self._cfgs.distribution._target_)
         ## TODO: get augmentation
-        if self._cfgs.use_aug:
-            self._agent.aug = hydra.utils.instantiate(self._cfgs.augmentation).to(self._device)
+        aug = hydra.utils.instantiate(self._cfgs.augmentation).to(self._device) if self._cfgs.use_aug else None
         ## TODO: get intrinsic reward
-        if self._cfgs.use_irs:
-            self._agent.irs = hydra.utils.instantiate(self._cfgs.reward)
+        irs = hydra.utils.instantiate(self._cfgs.reward) if self._cfgs.use_irs else None
 
-        # TODO: make data loader
-        if "NStepReplayStorage" in self._cfgs.storage._target_:
-            self._replay_loader = th.utils.data.DataLoader(
-                self._replay_storage,
-                batch_size=self._replay_storage.get_batch_size,
-                num_workers=self._replay_storage.get_num_workers,
-                pin_memory=self._replay_storage.get_pin_memory,
-                worker_init_fn=worker_init_fn,
-            )
-            self._replay_iter = None
-            self._use_nstep_replay_storage = True
-        else:
-            self._use_nstep_replay_storage = False
+        # TODO: Integrate agent and modules
+        self._agent.integrate(encoder=encoder, dist=dist, aug=aug, irs=irs)
+        # TODO: load initial parameters
+        if self._cfgs.init_model_path is not None:
+            self._logger.info(f"Loading Initial Parameters from {self._cfgs.init_model_path}")
+            self._agent.load(self._cfgs.init_model_path)
 
-        self._num_init_steps = self._cfgs.num_init_steps
+        self._num_steps = self._cfgs.num_steps
+        self._num_envs = self._cfgs.num_envs
 
         # debug
         self._logger.debug("Check Accomplished. Start Training...")
 
-    @property
-    def replay_iter(self) -> Iterable:
-        """Create iterable dataloader."""
-        if self._replay_iter is None:
-            self._replay_iter = iter(self._replay_loader)
-        return self._replay_iter
-
     def train(self) -> None:
         """Training function."""
-        episode_step, episode_reward = 0, 0
+        episode_rewards = deque(maxlen=10)
+        episode_steps = deque(maxlen=10)
         obs, info = self._train_env.reset(seed=self._seed)
-        metrics = None
+        # Number of updates
+        num_updates = self._num_train_steps // self._num_envs // self._num_steps
 
-        while self._global_step <= self._num_train_steps:
+        for update in range(num_updates):
             # try to test
-            if (self._global_step % self._test_every_steps) == 0 and (self._test_env is not None):
+            if (update % self._test_every_episodes) == 0 and (self._test_env is not None):
                 test_metrics = self.test()
                 self._logger.test(msg=test_metrics)
 
-            # sample actions
-            with th.no_grad(), eval_mode(self._agent):
-                action = self._agent.act(obs, training=True, step=self._global_step)
-                # TODO: Initial exploration
-                if self._global_step < self._num_init_steps:
-                    action.uniform_(-1.0, 1.0)
-            next_obs, reward, terminated, truncated, info = self._train_env.step(action)
-            episode_reward += reward[0].cpu().numpy()
-            episode_step += 1
-            self._global_step += 1
-
-            # save transition
-            self._replay_storage.add(
-                obs[0].cpu().numpy(),
-                action[0].cpu().numpy(),
-                np.zeros_like(reward[0].cpu().numpy())
-                if self._cfgs.pretraining
-                else reward[0].cpu().numpy(),  # pre-training mode
-                terminated[0].cpu().numpy(),
-                info,
-                next_obs[0].cpu().numpy(),
-            )
-
-            # update agent
-            if self._global_step >= self._num_init_steps:
-                if self._use_nstep_replay_storage:
-                    # TODO: for NStepReplayStorage
-                    metrics = self._agent.update(self.replay_iter, step=self._global_step)
-                else:
-                    metrics = self._agent.update(self._replay_storage, step=self._global_step)
-                    # TODO: for PrioritizedReplayStorage
-                    if "indices" in metrics and "priorities" in metrics:
-                        self._replay_storage.update_priorities(metrics["indices"], metrics["priorities"])
-
-            # done
-            if terminated or truncated:
-                episode_time, total_time = self._timer.reset()
-                if metrics is not None:
-                    train_metrics = {
-                        "step": self._global_step,
-                        "episode": self._global_episode,
-                        "episode_length": episode_step,
-                        "episode_reward": episode_reward,
-                        "fps": episode_step / episode_time,
-                        "total_time": total_time,
+            for _step in range(self._num_steps):
+                # sample actions
+                with th.no_grad(), eval_mode(self._agent):
+                    agent_outputs = self._agent.act(obs, training=True, step=self._global_step)
+                (
+                    next_obs,
+                    rewards,
+                    terminateds,
+                    truncateds,
+                    infos,
+                ) = self._train_env.step(agent_outputs["actions"])
+
+                agent_outputs.update(
+                    {
+                        "obs": obs,
+                        "rewards": th.zeros_like(rewards, device=self._device)
+                        if self._cfgs.pretraining
+                        else rewards,  # pre-training mode
+                        "terminateds": terminateds,
+                        "truncateds": truncateds,
+                        "next_obs": next_obs,
                     }
-                    self._logger.train(msg=train_metrics)
+                )
 
-                obs, info = self._train_env.reset(seed=self._seed)
-                self._global_episode += 1
-                episode_step, episode_reward = 0, 0
-                continue
-
-            obs = next_obs
+                if "episode" in infos:
+                    indices = np.nonzero(infos["episode"]["r"])
+                    episode_rewards.extend(infos["episode"]["r"][indices].tolist())
+                    episode_steps.extend(infos["episode"]["l"][indices].tolist())
+
+                # add transitions
+                self._rollout_storage.add(**agent_outputs)
+
+                obs = next_obs
+
+            # get the value estimation of the last step
+            with th.no_grad():
+                last_values = self._agent.get_value(next_obs).detach()
+
+            # perform return and advantage estimation
+            self._rollout_storage.compute_returns_and_advantages(last_values)
+
+            # policy update
+            self._agent.update(self._rollout_storage, episode=self._global_episode)
+
+            # update and reset buffer
+            self._rollout_storage.update()
+
+            self._global_episode += 1
+            self._global_step += self._num_envs * self._num_steps
+            episode_time, total_time = self._timer.reset()
+
+            if len(episode_rewards) > 1:
+                train_metrics = {
+                    "step": self._global_step,
+                    "episode": self._global_episode,
+                    "episode_length": np.mean(episode_steps),
+                    "episode_reward": np.mean(episode_rewards),
+                    "fps": self._num_steps * self._num_envs / episode_time,
+                    "total_time": total_time,
+                }
+                self._logger.train(msg=train_metrics)
 
         # save model
         self._logger.info("Training Accomplished!")
         self.save()
 
     def test(self) -> Dict[str, float]:
         """Testing function."""
-        step, episode, total_reward = 0, 0, 0
         obs, info = self._test_env.reset(seed=self._seed)
+        episode_rewards = list()
+        episode_steps = list()
 
-        while episode <= self._num_test_episodes:
+        while len(episode_rewards) < self._num_test_episodes:
             with th.no_grad(), eval_mode(self._agent):
-                action = self._agent.act(obs, training=False, step=self._global_step)
-
-            next_obs, reward, terminated, truncated, info = self._test_env.step(action)
-            total_reward += reward[0].cpu().numpy()
-            step += 1
-
-            if terminated or truncated:
-                obs, info = self._test_env.reset(seed=self._seed)
-                episode += 1
-                continue
+                actions = self._agent.act(obs, training=False, step=self._global_step)
+            obs, rewards, terminateds, truncateds, infos = self._test_env.step(actions)
 
-            obs = next_obs
+            if "episode" in infos:
+                indices = np.nonzero(infos["episode"]["r"])
+                episode_rewards.extend(infos["episode"]["r"][indices].tolist())
+                episode_steps.extend(infos["episode"]["l"][indices].tolist())
 
         return {
             "step": self._global_step,
             "episode": self._global_episode,
-            "episode_length": step / episode,
-            "episode_reward": total_reward / episode,
+            "episode_length": np.mean(episode_steps),
+            "episode_reward": np.mean(episode_rewards),
             "total_time": self._timer.total_time(),
         }
 
     def save(self) -> None:
         """Save the trained model."""
-        save_dir = Path.cwd() / "model"
+        save_dir = Path.cwd() / "pretrained" if self._cfgs.pretraining else Path.cwd() / "model"
         save_dir.mkdir(exist_ok=True)
-
-        if self._cfgs.pretraining:
-            th.save(self._agent.encoder, save_dir / "pretrained_encoder.pth")
-            th.save(self._agent.actor, save_dir / "pretrained_actor.pth")
-            th.save(self._agent.critic, save_dir / "pretrained_critic.pth")
-        else:
-            th.save(self._agent.encoder, save_dir / "encoder.pth")
-            th.save(self._agent.actor, save_dir / "actor.pth")
-            th.save(self._agent.critic, save_dir / "critic.pth")
-
+        self._agent.save(path=save_dir)
         self._logger.info(f"Model saved at: {save_dir}")
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/common/engine/on_policy_trainer.py` & `hsuanwu-0.0.1b5/hsuanwu/common/engine/off_policy_trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,177 +1,161 @@
-from collections import deque
 from pathlib import Path
 from typing import Dict
 
 import gymnasium as gym
 import hydra
 import numpy as np
 import omegaconf
 import torch as th
 
 from hsuanwu.common.engine.base_policy_trainer import BasePolicyTrainer
 from hsuanwu.common.engine.utils import eval_mode
 
 
-class OnPolicyTrainer(BasePolicyTrainer):
-    """Trainer for on-policy algorithms.
+class OffPolicyTrainer(BasePolicyTrainer):
+    """Trainer for off-policy algorithms.
 
     Args:
         cfgs (DictConfig): Dict config for configuring RL algorithms.
         train_env (Env): A Gym-like environment for training.
         test_env (Env): A Gym-like environment for testing.
 
     Returns:
-        On-policy trainer instance.
+        Off-policy trainer instance.
     """
 
     def __init__(self, cfgs: omegaconf.DictConfig, train_env: gym.Env, test_env: gym.Env = None) -> None:
         super().__init__(cfgs, train_env, test_env)
-        self._logger.info("Deploying OnPolicyTrainer...")
+        self._logger.info("Deploying OffPolicyTrainer...")
         # TODO: turn on the pretraining mode, no extrinsic rewards will be provided.
         if self._cfgs.pretraining:
             self._logger.info("Pre-training Mode On...")
         # xploit part
         self._agent = hydra.utils.instantiate(self._cfgs.agent)
-        # TODO: build encoder
-        self._agent.encoder = hydra.utils.instantiate(self._cfgs.encoder).to(self._device)
-        self._agent.encoder.train()
-        self._agent.encoder_opt = th.optim.Adam(
-            self._agent.encoder.parameters(),
-            lr=self._agent.lr,
-            eps=self._agent.eps,
-        )
-        # TODO: build storage
-        self._rollout_storage = hydra.utils.instantiate(self._cfgs.storage)
+        ## TODO: build encoder
+        encoder = hydra.utils.instantiate(self._cfgs.encoder).to(self._device)
+        ## TODO: build storage
+        self._replay_storage = hydra.utils.instantiate(self._cfgs.storage)
 
         # xplore part
-        # TODO: get distribution
-        dist = hydra.utils.get_class(self._cfgs.distribution._target_)
-        self._agent.dist = dist
-        self._agent.ac.dist = dist
-        # TODO: get augmentation
-        if self._cfgs.use_aug:
-            self._agent.aug = hydra.utils.instantiate(self._cfgs.augmentation).to(self._device)
-        # TODO: get intrinsic reward
-        if self._cfgs.use_irs:
-            self._agent.irs = hydra.utils.instantiate(self._cfgs.reward)
+        ## TODO: get distribution
+        if "Noise" in self._cfgs.distribution._target_:
+            dist = hydra.utils.instantiate(self._cfgs.distribution)
+        else:
+            dist = hydra.utils.get_class(self._cfgs.distribution._target_)
+        ## TODO: get augmentation
+        aug = hydra.utils.instantiate(self._cfgs.augmentation).to(self._device) if self._cfgs.use_aug else None
+        ## TODO: get intrinsic reward
+        irs = hydra.utils.instantiate(self._cfgs.reward) if self._cfgs.use_irs else None
+
+        # TODO: Integrate agent and modules
+        self._agent.integrate(encoder=encoder, dist=dist, aug=aug, irs=irs)
+        # TODO: load initial parameters
+        if self._cfgs.init_model_path is not None:
+            self._logger.info(f"Loading Initial Parameters from {self._cfgs.init_model_path}")
+            self._agent.load(self._cfgs.init_model_path)
 
-        self._num_steps = self._cfgs.num_steps
-        self._num_envs = self._cfgs.num_envs
+        self._num_init_steps = self._cfgs.num_init_steps
 
         # debug
         self._logger.debug("Check Accomplished. Start Training...")
 
     def train(self) -> None:
         """Training function."""
-        episode_rewards = deque(maxlen=10)
-        episode_steps = deque(maxlen=10)
+        episode_step, episode_reward = 0, 0
         obs, info = self._train_env.reset(seed=self._seed)
-        # Number of updates
-        num_updates = self._num_train_steps // self._num_envs // self._num_steps
+        metrics = None
 
-        for update in range(num_updates):
+        while self._global_step <= self._num_train_steps:
             # try to test
-            if (update % self._test_every_episodes) == 0 and (self._test_env is not None):
+            if (self._global_step % self._test_every_steps) == 0 and (self._test_env is not None):
                 test_metrics = self.test()
                 self._logger.test(msg=test_metrics)
 
-            for _step in range(self._num_steps):
-                # sample actions
-                with th.no_grad(), eval_mode(self._agent):
-                    actions, values, log_probs, entropy = self._agent.act(obs, training=True, step=self._global_step)
-                (
-                    next_obs,
-                    rewards,
-                    terminateds,
-                    truncateds,
-                    infos,
-                ) = self._train_env.step(actions)
-
-                if "episode" in infos:
-                    indices = np.nonzero(infos["episode"]["r"])
-                    episode_rewards.extend(infos["episode"]["r"][indices].tolist())
-                    episode_steps.extend(infos["episode"]["l"][indices].tolist())
-
-                # add transitions
-                self._rollout_storage.add(
-                    obs=obs,
-                    actions=actions,
-                    rewards=np.zeros_like(rewards) if self._cfgs.pretraining else rewards,  # pre-training mode
-                    terminateds=terminateds,
-                    truncateds=truncateds,
-                    log_probs=log_probs,
-                    next_obs=next_obs,
-                    values=values,
-                )
-
-                obs = next_obs
-
-            # get the value estimation of the last step
-            with th.no_grad():
-                last_values = self._agent.get_value(next_obs).detach()
-
-            # perform return and advantage estimation
-            self._rollout_storage.compute_returns_and_advantages(last_values)
-
-            # policy update
-            self._agent.update(self._rollout_storage, episode=self._global_episode)
-
-            # reset buffer
-            self._rollout_storage.reset()
-
-            self._global_episode += 1
-            self._global_step += self._num_envs * self._num_steps
-            episode_time, total_time = self._timer.reset()
-
-            if len(episode_rewards) > 1:
-                train_metrics = {
-                    "step": self._global_step,
-                    "episode": self._global_episode,
-                    "episode_length": np.mean(episode_steps),
-                    "episode_reward": np.mean(episode_rewards),
-                    "fps": self._num_steps * self._num_envs / episode_time,
-                    "total_time": total_time,
-                }
-                self._logger.train(msg=train_metrics)
+            # sample actions
+            with th.no_grad(), eval_mode(self._agent):
+                action = self._agent.act(obs, training=True, step=self._global_step)
+                # TODO: Initial exploration
+                if self._global_step < self._num_init_steps:
+                    action.uniform_(-1.0, 1.0)
+            next_obs, reward, terminated, truncated, info = self._train_env.step(action)
+            episode_reward += reward[0].cpu().numpy()
+            episode_step += 1
+            self._global_step += 1
+
+            # save transition
+            self._replay_storage.add(
+                obs[0].cpu().numpy(),
+                action[0].cpu().numpy(),
+                np.zeros_like(reward[0].cpu().numpy())
+                if self._cfgs.pretraining
+                else reward[0].cpu().numpy(),  # pre-training mode
+                terminated[0].cpu().numpy(),
+                info,
+                next_obs[0].cpu().numpy(),
+            )
+
+            # update agent
+            if self._global_step >= self._num_init_steps:
+                metrics = self._agent.update(self._replay_storage, step=self._global_step)
+                # try to update storage
+                self._replay_storage.update(metrics)
+
+            # done
+            if terminated or truncated:
+                episode_time, total_time = self._timer.reset()
+                if metrics is not None:
+                    train_metrics = {
+                        "step": self._global_step,
+                        "episode": self._global_episode,
+                        "episode_length": episode_step,
+                        "episode_reward": episode_reward,
+                        "fps": episode_step / episode_time,
+                        "total_time": total_time,
+                    }
+                    self._logger.train(msg=train_metrics)
+
+                obs, info = self._train_env.reset(seed=self._seed)
+                self._global_episode += 1
+                episode_step, episode_reward = 0, 0
+                continue
+
+            obs = next_obs
 
         # save model
         self._logger.info("Training Accomplished!")
         self.save()
 
     def test(self) -> Dict[str, float]:
         """Testing function."""
+        step, episode, total_reward = 0, 0, 0
         obs, info = self._test_env.reset(seed=self._seed)
-        episode_rewards = list()
-        episode_steps = list()
 
-        while len(episode_rewards) < self._num_test_episodes:
+        while episode <= self._num_test_episodes:
             with th.no_grad(), eval_mode(self._agent):
-                actions = self._agent.act(obs, training=False, step=self._global_step)
-            obs, rewards, terminateds, truncateds, infos = self._test_env.step(actions)
+                action = self._agent.act(obs, training=False, step=self._global_step)
+
+            next_obs, reward, terminated, truncated, info = self._test_env.step(action)
+            total_reward += reward[0].cpu().numpy()
+            step += 1
+
+            if terminated or truncated:
+                obs, info = self._test_env.reset(seed=self._seed)
+                episode += 1
+                continue
 
-            if "episode" in infos:
-                indices = np.nonzero(infos["episode"]["r"])
-                episode_rewards.extend(infos["episode"]["r"][indices].tolist())
-                episode_steps.extend(infos["episode"]["l"][indices].tolist())
+            obs = next_obs
 
         return {
             "step": self._global_step,
             "episode": self._global_episode,
-            "episode_length": np.mean(episode_steps),
-            "episode_reward": np.mean(episode_rewards),
+            "episode_length": step / episode,
+            "episode_reward": total_reward / episode,
             "total_time": self._timer.total_time(),
         }
 
     def save(self) -> None:
         """Save the trained model."""
-        save_dir = Path.cwd() / "model"
+        save_dir = Path.cwd() / "pretrained" if self._cfgs.pretraining else Path.cwd() / "model"
         save_dir.mkdir(exist_ok=True)
-
-        if self._cfgs.pretraining:
-            th.save(self._agent.encoder, save_dir / "pretrained_encoder.pth")
-            th.save(self._agent.ac, save_dir / "pretrained_actor_critic.pth")
-        else:
-            th.save(self._agent.encoder, save_dir / "encoder.pth")
-            th.save(self._agent.ac, save_dir / "actor_critic.pth")
-
+        self._agent.save(path=save_dir)
         self._logger.info(f"Model saved at: {save_dir}")
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/env/utils.py` & `hsuanwu-0.0.1b5/hsuanwu/env/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,18 @@
             self.action_space = OmegaConf.create(
                 {
                     "shape": env.single_action_space.shape,
                     "type": "Box",
                     "range": [low, high],
                 }
             )
+        elif env.single_action_space.__class__.__name__ == "MultiBinary":
+            self.action_space = OmegaConf.create(
+                {"shape": env.single_action_space.shape, "type": "MultiBinary", "range": [0, 1]}
+            )
         else:
             raise NotImplementedError("Unsupported action type!")
         self.num_envs = len(env.envs)
 
     def reset(
         self,
         seed: Optional[Union[int, List[int]]] = None,
@@ -65,20 +69,15 @@
 
         Args:
             actions (Tensor): element of :attr:`action_space` Batch of actions.
 
         Returns:
             Batch of (observations, rewards, terminations, truncations, infos)
         """
-        if self.action_space["type"] == "Discrete":
-            actions = actions.squeeze(1).cpu().numpy()
-        else:
-            actions = actions.cpu().numpy()
-
-        obs, reward, terminated, truncated, info = self.env.step(actions)
+        obs, reward, terminated, truncated, info = self.env.step(actions.cpu().numpy())
         obs = th.as_tensor(obs, device=self._device)
         reward = th.as_tensor(reward, dtype=th.float32, device=self._device)
         terminated = th.as_tensor(
             [1.0 if _ else 0.0 for _ in terminated],
             dtype=th.float32,
             device=self._device,
         )
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/env/atari/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/env/atari/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from hsuanwu.env.utils import HsuanwuEnvWrapper
 
 
 def make_atari_env(
     env_id: str = "Alien-v5",
     num_envs: int = 8,
     device: str = "cpu",
-    seed: int = 0,
+    seed: int = 1,
     frame_stack: int = 4,
 ) -> gym.Env:
     """Build Atari environments.
 
     Args:
         env_id (str): Name of environment.
         num_envs (int): Number of parallel environments.
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/env/atari/wrappers.py` & `hsuanwu-0.0.1b5/hsuanwu/env/atari/wrappers.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/env/bullet/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/env/bullet/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/env/dmc/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/env/dmc/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/env/dmc/natural_imgsource.py` & `hsuanwu-0.0.1b5/hsuanwu/env/dmc/natural_imgsource.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/env/dmc/wrappers.py` & `hsuanwu-0.0.1b5/hsuanwu/env/dmc/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 def _flatten_obs(obs):
     obs_pieces = []
     for v in obs.values():
         flat = np.array([v]) if np.isscalar(v) else v.ravel()
         obs_pieces.append(flat)
-    return np.concatenate(obs_pieces, axis=0)
+    return np.concatenate(obs_pieces, axis=0, dtype=np.float32)
 
 
 class DMCWrapper(core.Env):
     def __init__(
         self,
         domain_name,
         task_name,
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/env/minigrid/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/env/minigrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/env/procgen/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/env/procgen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         return obs, {}
 
 
 def make_procgen_env(
     env_id: str = "bigfish",
     num_envs: int = 64,
     gamma: float = 0.99,
-    num_levels: int = 0,
+    num_levels: int = 200,
     start_level: int = 0,
     distribution_mode: str = "easy",
     device: str = "cpu",
 ) -> gym.Env:
     """Build Prcogen environments.
 
     Args:
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/experimental/npu_ppo.py` & `hsuanwu-0.0.1b5/hsuanwu/experimental/npu_ppo.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/agent/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from .base import BaseAgent as BaseAgent
+from .daac import DAAC as DAAC
+from .daac import DEFAULT_CFGS as DAAC_DEFAULT_CFGS
+from .daac import MATCH_KEYS as DAAC_MATCH_KEYS
 from .drqv2 import DEFAULT_CFGS as DRQV2_DEFAULT_CFGS
 from .drqv2 import MATCH_KEYS as DRQV2_MATCH_KEYS
 from .drqv2 import DrQv2 as DrQv2
 from .impala import DEFAULT_CFGS as IMPALA_DEFAULT_CFGS
 from .impala import IMPALA as IMPALA
 from .impala import MATCH_KEYS as IMPALA_MATCH_KEYS
 from .ppg import DEFAULT_CFGS as PPG_DEFAULT_CFGS
@@ -12,20 +15,22 @@
 from .ppo import MATCH_KEYS as PPO_MATCH_KEYS
 from .ppo import PPO as PPO
 from .sac import DEFAULT_CFGS as SAC_DEFAULT_CFGS
 from .sac import MATCH_KEYS as SAC_MATCH_KEYS
 from .sac import SAC as SAC
 
 ALL_DEFAULT_CFGS = {
+    "DAAC": DAAC_DEFAULT_CFGS,
     "DrQv2": DRQV2_DEFAULT_CFGS,
     "PPG": PPG_DEFAULT_CFGS,
     "SAC": SAC_DEFAULT_CFGS,
     "PPO": PPO_DEFAULT_CFGS,
     "IMPALA": IMPALA_DEFAULT_CFGS,
 }
 ALL_MATCH_KEYS = {
+    "DAAC": DAAC_MATCH_KEYS,
     "DrQv2": DRQV2_MATCH_KEYS,
     "PPG": PPG_MATCH_KEYS,
     "SAC": SAC_MATCH_KEYS,
     "PPO": PPO_MATCH_KEYS,
     "IMPALA": IMPALA_MATCH_KEYS,
 }
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/base.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/agent/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
-from typing import Dict, Tuple, Union
+from pathlib import Path
+from typing import Any, Dict, Union
 
 import gymnasium as gym
 import torch as th
 from omegaconf import DictConfig
 
 
 class BaseAgent(ABC):
@@ -33,24 +34,28 @@
         feature_dim: int,
         lr: float,
         eps: float,
     ) -> None:
         if isinstance(observation_space, gym.Space) and isinstance(action_space, gym.Space):
             self.obs_shape = observation_space.shape
             if action_space.__class__.__name__ == "Discrete":
-                self.action_shape = (int(action_space.n),)  # type: ignore[attr-defined]
+                self.action_shape = (int(action_space.n),)
                 self.action_type = "Discrete"
-                self.action_range = [0, int(action_space.n) - 1]  # type: ignore[attr-defined]
+                self.action_range = [0, int(action_space.n) - 1]
             elif action_space.__class__.__name__ == "Box":
-                self.action_shape = action_space.shape  # type: ignore[attr-defined, list-item, assignment]
+                self.action_shape = action_space.shape
                 self.action_type = "Box"
                 self.action_range = [
-                    float(action_space.low[0]),  # type: ignore[attr-defined, list-item]
-                    float(action_space.high[0]),  # type: ignore[attr-defined, list-item]
+                    float(action_space.low[0]),
+                    float(action_space.high[0]),
                 ]
+            elif action_space.__class__.__name__ == "MultiBinary":
+                self.action_shape = action_space.shape
+                self.action_type = "MultiBinary"
+                self.action_range = [0, 1]
             else:
                 raise NotImplementedError("Unsupported action type!")
         elif isinstance(observation_space, DictConfig) and isinstance(action_space, DictConfig):
             # by DictConfig
             self.obs_shape = observation_space.shape
             self.action_shape = action_space.shape
             self.action_type = action_space.type
@@ -61,15 +66,14 @@
         self.device = th.device(device)
         self.feature_dim = feature_dim
         self.lr = lr
         self.eps = eps
 
         # placeholder for distribution, augmentation, and intrinsic reward function.
         self.encoder = None
-        self.encoder_opt = None
         self.dist = None
         self.aug = None
         self.irs = None
 
     @abstractmethod
     def train(self, training: bool = True) -> None:
         """Set the train mode.
@@ -79,22 +83,48 @@
 
         Returns:
             None.
         """
         self.training = training
 
     @abstractmethod
-    def act(self, obs: th.Tensor, training: bool = True, step: int = 0) -> Tuple[th.Tensor]:
+    def integrate(self, **kwargs) -> None:
+        """Integrate agent and other modules (encoder, reward, ...) together"""
+
+    @abstractmethod
+    def act(self, obs: th.Tensor, training: bool = True, step: int = 0) -> Any:
         """Sample actions based on observations.
 
         Args:
             obs (Tensor): Observations.
             training (bool): training mode, True or False.
             step (int): Global training step.
 
         Returns:
             Sampled actions.
         """
 
     @abstractmethod
-    def update(self, *kwargs) -> Dict[str, float]:
+    def update(self, **kwargs) -> Dict[str, float]:
         """Update agent and return training metrics such as loss functions."""
+
+    @abstractmethod
+    def save(self, path: Path) -> None:
+        """Save models.
+
+        Args:
+            path (path): Storage path.
+
+        Returns:
+            None.
+        """
+
+    @abstractmethod
+    def load(self, path: str) -> None:
+        """Load initial parameters.
+
+        Args:
+            path (path): Import path.
+
+        Returns:
+            None.
+        """
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/drqv2.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/agent/drqv2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import Dict, Generator, Tuple, Union
+import os
+from pathlib import Path
+from typing import Dict, Tuple, Union
 
 import gymnasium as gym
 import torch as th
 from omegaconf import DictConfig
 from torch.nn import functional as F
 
 from hsuanwu.xploit.agent import utils
 from hsuanwu.xploit.agent.base import BaseAgent
-from hsuanwu.xploit.agent.network import DeterministicActor, DoubleCritic
+from hsuanwu.xploit.agent.network import OffPolicyDeterministicActor, OffPolicyDoubleCritic
 
 MATCH_KEYS = {
     "trainer": "OffPolicyTrainer",
     "storage": ["NStepReplayStorage"],
     "distribution": [
         "OrnsteinUhlenbeckNoise",
         "TruncatedNormalNoise",
@@ -100,21 +102,23 @@
     ) -> None:
         super().__init__(observation_space, action_space, device, feature_dim, lr, eps)
 
         self.critic_target_tau = critic_target_tau
         self.update_every_steps = update_every_steps
 
         # create models
-        self.actor = DeterministicActor(action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim).to(
+        self.actor = OffPolicyDeterministicActor(action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim).to(
             self.device
         )
-        self.critic = DoubleCritic(action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim).to(self.device)
-        self.critic_target = DoubleCritic(action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim).to(
+        self.critic = OffPolicyDoubleCritic(action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim).to(
             self.device
         )
+        self.critic_target = OffPolicyDoubleCritic(
+            action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim
+        ).to(self.device)
         self.critic_target.load_state_dict(self.critic.state_dict())
 
         # create optimizers
         self.actor_opt = th.optim.Adam(self.actor.parameters(), lr=self.lr)
         self.critic_opt = th.optim.Adam(self.critic.parameters(), lr=self.lr)
         self.train()
         self.critic_target.train()
@@ -130,51 +134,63 @@
         """
         self.training = training
         self.actor.train(training)
         self.critic.train(training)
         if self.encoder is not None:
             self.encoder.train(training)
 
+    def integrate(self, **kwargs) -> None:
+        """Integrate agent and other modules (encoder, reward, ...) together"""
+        self.encoder = kwargs["encoder"]
+        self.encoder_opt = th.optim.Adam(self.encoder.parameters(), lr=self.lr, eps=self.eps)
+        self.encoder.train()
+        self.dist = kwargs["dist"]
+        self.actor.dist = kwargs["dist"]
+        if kwargs["aug"] is not None:
+            self.aug = kwargs["aug"]
+        if kwargs["irs"] is not None:
+            self.irs = kwargs["irs"]
+
     def act(self, obs: th.Tensor, training: bool = True, step: int = 0) -> Tuple[th.Tensor]:
         """Sample actions based on observations.
 
         Args:
             obs (Tensor): Observations.
             training (bool): training mode, True or False.
             step (int): Global training step.
 
         Returns:
             Sampled actions.
         """
         encoded_obs = self.encoder(obs)
-        dist = self.actor.get_action(obs=encoded_obs, step=step)
+        dist = self.actor.get_dist(obs=encoded_obs, step=step)
 
         if not training:
             action = dist.mean
         else:
             action = dist.sample()
 
         return action.clamp(*self.action_range)
 
-    def update(self, replay_iter: Generator, step: int = 0) -> Dict[str, float]:
+    def update(self, replay_storage, step: int = 0) -> Dict[str, float]:
         """Update the agent.
 
         Args:
-            replay_iter (Generator): Hsuanwu replay storage iterable dataloader.
+            replay_storage (Storage): Hsuanwu replay storage.
             step (int): Global training step.
 
         Returns:
             Training metrics such as actor loss, critic_loss, etc.
         """
 
         metrics = {}
         if step % self.update_every_steps != 0:
             return metrics
 
-        obs, action, reward, discount, next_obs = next(replay_iter)
+        obs, action, reward, discount, next_obs = replay_storage.sample(step)
         obs = obs.float().to(self.device)
         action = action.float().to(self.device)
         reward = reward.float().to(self.device)
         discount = discount.float().to(self.device)
         next_obs = next_obs.float().to(self.device)
 
         if self.irs is not None:
@@ -230,15 +246,15 @@
 
         Returns:
             Critic loss metrics.
         """
 
         with th.no_grad():
             # sample actions
-            dist = self.actor.get_action(next_obs, step=step)
+            dist = self.actor.get_dist(next_obs, step=step)
 
             next_action = dist.sample(clip=True)
             target_Q1, target_Q2 = self.critic_target(next_obs, next_action)
             target_V = th.min(target_Q1, target_Q2)
             target_Q = reward + (discount * target_V)
 
         Q1, Q2 = self.critic(obs, action)
@@ -265,21 +281,55 @@
             obs (Tensor): Observations.
             step (int): Global training step.
 
         Returns:
             Actor loss metrics.
         """
         # sample actions
-        dist = self.actor.get_action(obs, step=step)
+        dist = self.actor.get_dist(obs, step=step)
         action = dist.sample(clip=True)
 
         Q1, Q2 = self.critic(obs, action)
         Q = th.min(Q1, Q2)
 
         actor_loss = -Q.mean()
 
         # optimize actor
         self.actor_opt.zero_grad(set_to_none=True)
         actor_loss.backward()
         self.actor_opt.step()
 
         return {"actor_loss": actor_loss.item()}
+
+    def save(self, path: Path) -> None:
+        """Save models.
+
+        Args:
+            path (Path): Storage path.
+
+        Returns:
+            None.
+        """
+        if "pretrained" in str(path):  # pretraining
+            th.save(self.encoder.state_dict(), path / "encoder.pth")
+            th.save(self.actor.state_dict(), path / "actor.pth")
+            th.save(self.critic.state_dict(), path / "critic.pth")
+        else:
+            th.save(self.encoder, path / "encoder.pth")
+            th.save(self.actor, path / "actor.pth")
+            th.save(self.critic, path / "critic.pth")
+
+    def load(self, path: str) -> None:
+        """Load initial parameters.
+
+        Args:
+            path (str): Import path.
+
+        Returns:
+            None.
+        """
+        encoder_params = th.load(os.path.join(path, "encoder.pth"), map_location=self.device)
+        actor_params = th.load(os.path.join(path, "actor.pth"), map_location=self.device)
+        critic_params = th.load(os.path.join(path, "critic.pth"), map_location=self.device)
+        self.encoder.load_state_dict(encoder_params)
+        self.actor.load_state_dict(actor_params)
+        self.critic.load_state_dict(critic_params)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/impala.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/agent/impala.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import collections
+import os
 import threading
+from copy import deepcopy
+from pathlib import Path
 from typing import Dict, Tuple, Union
 
 import gymnasium as gym
 import omegaconf
 import torch as th
 from omegaconf import DictConfig
 from torch import nn
 from torch.nn import functional as F
 
 from hsuanwu.xploit.agent.base import BaseAgent
-from hsuanwu.xploit.agent.network import DiscreteLSTMActor
+from hsuanwu.xploit.agent.network import DistributedActorCritic
 
 MATCH_KEYS = {
     "trainer": "DistributedTrainer",
     "storage": ["DistributedStorage"],
-    "distribution": ["Categorical"],
+    "distribution": ["Categorical", "DiagonalGaussian"],
     "augmentation": [],
     "reward": [],
 }
 
 DEFAULT_CFGS = {
     ## TODO: Train setup
     "device": "cpu",
@@ -55,120 +57,73 @@
     ## TODO: xplore part
     "distribution": {"name": "Categorical"},
     "augmentation": {"name": None},
     "reward": {"name": None},
 }
 
 
-VTraceFromLogitsReturns = collections.namedtuple(
-    "VTraceFromLogitsReturns",
-    [
-        "vs",
-        "pg_advantages",
-        "log_rhos",
-        "behavior_action_log_probs",
-        "target_action_log_probs",
-    ],
-)
-
-VTraceReturns = collections.namedtuple("VTraceReturns", "vs pg_advantages")
-
-
-class VTrace:
-    """Compute V-trace off-policy actor critic targets."""
-
-    def __init__(self) -> None:
-        pass
-
-    def action_log_probs(self, policy_logits, actions):
-        return -F.nll_loss(
-            F.log_softmax(th.flatten(policy_logits, 0, -2), dim=-1),
-            th.flatten(actions),
-            reduction="none",
-        ).view_as(actions)
-
-    def from_logits(
+class VTraceLoss:
+    def __init__(
         self,
-        behavior_policy_logits,
-        target_policy_logits,
-        actions,
-        discounts,
-        rewards,
-        values,
-        bootstrap_value,
         clip_rho_threshold=1.0,
         clip_pg_rho_threshold=1.0,
-    ):
-        """V-trace for softmax policies."""
-
-        target_action_log_probs = self.action_log_probs(target_policy_logits, actions)
-        behavior_action_log_probs = self.action_log_probs(behavior_policy_logits, actions)
-        log_rhos = target_action_log_probs - behavior_action_log_probs
-        vtrace_returns = self.from_importance_weights(
-            log_rhos=log_rhos,
-            discounts=discounts,
-            rewards=rewards,
-            values=values,
-            bootstrap_value=bootstrap_value,
-            clip_rho_threshold=clip_rho_threshold,
-            clip_pg_rho_threshold=clip_pg_rho_threshold,
-        )
-        return VTraceFromLogitsReturns(
-            log_rhos=log_rhos,
-            behavior_action_log_probs=behavior_action_log_probs,
-            target_action_log_probs=target_action_log_probs,
-            **vtrace_returns._asdict(),
-        )
+    ) -> None:
+        self.dist = None
+        self.clip_rho_threshold = clip_rho_threshold
+        self.clip_pg_rho_threshold = clip_pg_rho_threshold
+
+    def compute_ISW(self, target_dist, behavior_dist, action):
+        log_rhos = target_dist.log_prob(action) - behavior_dist.log_prob(action)
+        return th.exp(log_rhos)
+
+    def __call__(self, batch):
+        _target_dist = batch["target_dist"]
+        _behavior_dist = batch["behavior_dist"]
+        _action = batch["action"]
+        _baseline = batch["values"]
+        _bootstrap_value = batch["bootstrap_value"]
+        _values = batch["values"]
+        _discounts = batch["discounts"]
+        _rewards = batch["reward"]
 
-    @th.no_grad()
-    def from_importance_weights(
-        self,
-        log_rhos,
-        discounts,
-        rewards,
-        values,
-        bootstrap_value,
-        clip_rho_threshold=1.0,
-        clip_pg_rho_threshold=1.0,
-    ):
-        """V-trace from log importance weights."""
         with th.no_grad():
-            rhos = th.exp(log_rhos)
-            if clip_rho_threshold is not None:
-                clipped_rhos = th.clamp(rhos, max=clip_rho_threshold)
+            rhos = self.compute_ISW(target_dist=_target_dist, behavior_dist=_behavior_dist, action=_action)
+            if self.clip_rho_threshold is not None:
+                clipped_rhos = th.clamp(rhos, max=self.clip_rho_threshold)
             else:
                 clipped_rhos = rhos
-
             cs = th.clamp(rhos, max=1.0)
             # Append bootstrapped value to get [v1, ..., v_t+1]
-            values_t_plus_1 = th.cat([values[1:], th.unsqueeze(bootstrap_value, 0)], dim=0)
-            deltas = clipped_rhos * (rewards + discounts * values_t_plus_1 - values)
+            values_t_plus_1 = th.cat([_values[1:], th.unsqueeze(_bootstrap_value, 0)], dim=0)
+            deltas = clipped_rhos * (_rewards + _discounts * values_t_plus_1 - _values)
 
-            acc = th.zeros_like(bootstrap_value)
+            acc = th.zeros_like(_bootstrap_value)
             result = []
-            for t in range(discounts.shape[0] - 1, -1, -1):
-                acc = deltas[t] + discounts[t] * cs[t] * acc
+            for t in range(_discounts.shape[0] - 1, -1, -1):
+                acc = deltas[t] + _discounts[t] * cs[t] * acc
                 result.append(acc)
             result.reverse()
             vs_minus_v_xs = th.stack(result)
 
             # Add V(x_s) to get v_s.
-            vs = th.add(vs_minus_v_xs, values)
-
+            vs = th.add(vs_minus_v_xs, _values)
             # Advantage for policy gradient.
-            broadcasted_bootstrap_values = th.ones_like(vs[0]) * bootstrap_value
+            broadcasted_bootstrap_values = th.ones_like(vs[0]) * _bootstrap_value
             vs_t_plus_1 = th.cat([vs[1:], broadcasted_bootstrap_values.unsqueeze(0)], dim=0)
-            if clip_pg_rho_threshold is not None:
-                clipped_pg_rhos = th.clamp(rhos, max=clip_pg_rho_threshold)
+            if self.clip_pg_rho_threshold is not None:
+                clipped_pg_rhos = th.clamp(rhos, max=self.clip_pg_rho_threshold)
             else:
                 clipped_pg_rhos = rhos
-            pg_advantages = clipped_pg_rhos * (rewards + discounts * vs_t_plus_1 - values)
+            pg_advantages = clipped_pg_rhos * (_rewards + _discounts * vs_t_plus_1 - _values)
+
+        pg_loss = -(_target_dist.log_prob(_action) * pg_advantages).sum()
+        baseline_loss = F.mse_loss(vs, _baseline, reduction="sum") * 0.5
+        entropy_loss = (_target_dist.entropy()).sum()
 
-            # Make sure no gradients backpropagated through the returned values.
-            return VTraceReturns(vs=vs, pg_advantages=pg_advantages)
+        return pg_loss, baseline_loss, entropy_loss
 
 
 class IMPALA(BaseAgent):
     """Importance Weighted Actor-Learner Architecture (IMPALA).
 
     Args:
         observation_space (Space or DictConfig): The observation space of environment. When invoked by Hydra,
@@ -208,31 +163,59 @@
         super().__init__(observation_space, action_space, device, feature_dim, lr, eps)
 
         self.ent_coef = ent_coef
         self.baseline_coef = baseline_coef
         self.max_grad_norm = max_grad_norm
         self.discount = discount
 
-        self.actor = DiscreteLSTMActor(action_space=action_space, feature_dim=feature_dim, use_lstm=use_lstm)
-
-        self.learner = DiscreteLSTMActor(action_space=action_space, feature_dim=feature_dim, use_lstm=use_lstm)
+        self.actor = DistributedActorCritic(
+            action_shape=self.action_shape,
+            action_type=self.action_type,
+            action_range=self.action_range,
+            feature_dim=feature_dim,
+            use_lstm=use_lstm,
+        )
+        self.learner = DistributedActorCritic(
+            action_shape=self.action_shape,
+            action_type=self.action_type,
+            action_range=self.action_range,
+            feature_dim=feature_dim,
+            use_lstm=use_lstm,
+        )
 
     def train(self, training: bool = True) -> None:
         """Set the train mode.
 
         Args:
             training (bool): True (training) or False (testing).
 
         Returns:
             None.
         """
         self.training = training
         self.actor.train(training)
         self.learner.train(training)
 
+    def integrate(self, **kwargs) -> None:
+        """Integrate agent and other modules (encoder, reward, ...) together"""
+        self.actor.encoder = kwargs["encoder"]
+        self.learner.encoder = deepcopy(kwargs["encoder"])
+        self.actor.dist = kwargs["dist"]
+        self.learner.dist = kwargs["dist"]
+        self.dist = kwargs["dist"]
+        self.actor.share_memory()
+        self.learner.to(self.device)
+        self.opt = th.optim.RMSprop(
+            self.learner.parameters(),
+            lr=self.lr,
+            eps=self.eps,
+        )
+
+        self.lr_scheduler = th.optim.lr_scheduler.LambdaLR(self.opt, kwargs["lr_lambda"])
+
     def act(self, *kwargs):
         """Sample actions based on observations."""
         return None
 
     @staticmethod
     def update(
         cfgs: omegaconf.DictConfig,
@@ -256,70 +239,38 @@
             optimizer (th.optim.Optimizer): Optimizer.
             lr_scheduler (th.optim.lr_scheduler): Learning rate scheduler.
             lock (Lock): Thread lock.
 
         Returns:
             Training metrics.
         """
-
-        ###########################################################################
-        def compute_policy_gradient_loss(logits, actions, advantages):
-            cross_entropy = F.nll_loss(
-                F.log_softmax(th.flatten(logits, 0, 1), dim=-1),
-                target=th.flatten(actions, 0, 1),
-                reduction="none",
-            )
-            cross_entropy = cross_entropy.view_as(advantages)
-            return th.sum(cross_entropy * advantages.detach())
-
-        def compute_baseline_loss(advantages):
-            return 0.5 * th.sum(advantages**2)
-
-        def compute_entropy_loss(logits):
-            """Return the entropy loss, i.e., the negative entropy of the policy."""
-            policy = F.softmax(logits, dim=-1)
-            log_policy = F.log_softmax(logits, dim=-1)
-            return th.sum(policy * log_policy)
-
-        ###########################################################################
-        """Performs a learning (optimization) step."""
         with lock:
             learner_outputs, _ = learner_model.get_action(batch, init_actor_states)
 
             # Take final value function slice for bootstrapping.
             bootstrap_value = learner_outputs["baseline"][-1]
 
             # Move from obs[t] -> action[t] to action[t] -> obs[t].
             batch = {key: tensor[1:] for key, tensor in batch.items()}
             learner_outputs = {key: tensor[:-1] for key, tensor in learner_outputs.items()}
 
-            rewards = batch["reward"]
-            clipped_rewards = th.clamp(rewards, -1, 1)
-
             discounts = (~batch["terminated"]).float() * cfgs.agent.discount
 
-            vtrace_returns = VTrace().from_logits(
-                behavior_policy_logits=batch["policy_logits"],
-                target_policy_logits=learner_outputs["policy_logits"],
-                actions=batch["action"],
-                discounts=discounts,
-                rewards=clipped_rewards,
-                values=learner_outputs["baseline"],
-                bootstrap_value=bootstrap_value,
-            )
-
-            pg_loss = compute_policy_gradient_loss(
-                learner_outputs["policy_logits"],
-                batch["action"],
-                vtrace_returns.pg_advantages,
+            batch.update(
+                {
+                    "discounts": discounts,
+                    "bootstrap_value": bootstrap_value,
+                    "target_dist": learner_model.get_dist(learner_outputs["policy_outputs"]),
+                    "behavior_dist": learner_model.get_dist(batch["policy_outputs"]),
+                    "values": learner_outputs["baseline"],
+                }
             )
-            baseline_loss = cfgs.agent.baseline_coef * compute_baseline_loss(vtrace_returns.vs - learner_outputs["baseline"])
-            entropy_loss = cfgs.agent.ent_coef * compute_entropy_loss(learner_outputs["policy_logits"])
 
-            total_loss = pg_loss + baseline_loss + entropy_loss
+            pg_loss, baseline_loss, entropy_loss = VTraceLoss()(batch)
+            total_loss = pg_loss + cfgs.agent.baseline_coef * baseline_loss - cfgs.agent.ent_coef * entropy_loss
 
             episode_returns = batch["episode_return"][batch["terminated"]]
             episode_steps = batch["episode_step"][batch["terminated"]]
 
             optimizer.zero_grad()
             total_loss.backward()
             nn.utils.clip_grad_norm_(learner_model.parameters(), cfgs.agent.max_grad_norm)
@@ -331,7 +282,33 @@
                 "episode_returns": tuple(episode_returns.cpu().numpy()),
                 "episode_steps": tuple(episode_steps.cpu().numpy()),
                 "total_loss": total_loss.item(),
                 "pg_loss": pg_loss.item(),
                 "baseline_loss": baseline_loss.item(),
                 "entropy_loss": entropy_loss.item(),
             }
+
+    def save(self, path: Path) -> None:
+        """Save models.
+
+        Args:
+            path (Path): Storage path.
+
+        Returns:
+            None.
+        """
+        th.save(self.actor, path / "actor.pth")
+        th.save(self.learner, path / "learner.pth")
+
+    def load(self, path: str) -> None:
+        """Load initial parameters.
+
+        Args:
+            path (str): Import path.
+
+        Returns:
+            None.
+        """
+        actor_params = th.load(os.path.join(path, "actor.pth"), map_location=self.device)
+        learner_params = th.load(os.path.join(path, "learner.pth"), map_location=self.device)
+        self.actor.load_state_dict(actor_params)
+        self.learner.load_state_dict(learner_params)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/network.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/ride.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,410 +1,312 @@
-from typing import Dict, Tuple
+from collections import deque
+from typing import Dict, Tuple, Union
 
 import gymnasium as gym
+import numpy as np
 import torch as th
+from omegaconf import DictConfig
 from torch import nn
-from torch.distributions import Distribution
 from torch.nn import functional as F
+from torch.utils.data import DataLoader, TensorDataset
 
-from hsuanwu.xploit.agent import utils
+from hsuanwu.xplore.reward.base import BaseIntrinsicRewardModule
 
 
-class StochasticActor(nn.Module):
-    """Stochastic actor network for SAC. Here the 'self.dist' refers to an sampling distribution instance.
+class Encoder(nn.Module):
+    """Encoder for encoding observations.
 
     Args:
-        action_space (Space): Action space of the environment.
-        feature_dim (int): Number of features accepted.
-        hidden_dim (int): Number of units per hidden layer.
+        obs_shape (Tuple): The data shape of observations.
+        action_shape (Tuple): The data shape of actions.
+        latent_dim (int): The dimension of encoding vectors.
 
     Returns:
-        Actor network instance.
+        Encoder instance.
     """
 
-    def __init__(
-        self,
-        action_space: gym.Space,
-        feature_dim: int = 64,
-        hidden_dim: int = 1024,
-        log_std_range: Tuple = (-10, 2),
-    ) -> None:
+    def __init__(self, obs_shape: Tuple, action_shape: Tuple, latent_dim: int) -> None:
         super().__init__()
 
-        self.policy = nn.Sequential(
-            nn.Linear(feature_dim, hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(hidden_dim, hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(hidden_dim, 2 * action_space.shape[0]),
-        )
-        # placeholder for distribution
-        self.dist = None
-        self.log_std_min, self.log_std_max = log_std_range
+        # visual
+        if len(obs_shape) == 3:
+            self.trunk = nn.Sequential(
+                nn.Conv2d(obs_shape[0], 32, 8, 4),
+                nn.ReLU(),
+                nn.Conv2d(32, 64, 4, 2),
+                nn.ReLU(),
+                nn.Conv2d(64, 64, 3, 1),
+                nn.ReLU(),
+                nn.Flatten(),
+            )
+            with th.no_grad():
+                sample = th.ones(size=tuple(obs_shape))
+                n_flatten = self.trunk(sample.unsqueeze(0)).shape[1]
 
-        self.apply(utils.network_init)
+            self.linear = nn.Linear(n_flatten, latent_dim)
+        else:
+            self.trunk = nn.Sequential(nn.Linear(obs_shape[0], 256), nn.ReLU())
+            self.linear = nn.Linear(256, latent_dim)
 
-    def get_action(self, obs: th.Tensor, step: int) -> Distribution:
-        """Get actions.
+    def forward(self, obs: th.Tensor) -> th.Tensor:
+        """Encode the input tensors.
 
         Args:
             obs (Tensor): Observations.
-            step (int): Global training step.
 
         Returns:
-            Hsuanwu distribution.
+            Encoding tensors.
         """
-        mu, log_std = self.policy(obs).chunk(2, dim=-1)
-
-        log_std = th.tanh(log_std)
-        log_std = self.log_std_min + 0.5 * (self.log_std_max - self.log_std_min) * (log_std + 1)
-
-        std = log_std.exp()
-
-        return self.dist(mu, std)
+        return self.linear(self.trunk(obs))
 
 
-class DeterministicActor(nn.Module):
-    """Deterministic actor network for DrQv2. Here the 'self.dist' refers to an action noise instance.
+class InverseDynamicsModel(nn.Module):
+    """Inverse model for reconstructing transition process.
 
     Args:
-        action_space (Space): Action space of the environment.
-        feature_dim (int): Number of features accepted.
-        hidden_dim (int): Number of units per hidden layer.
+        latent_dim (int): The dimension of encoding vectors of the observations.
+        action_dim (int): The dimension of predicted actions.
 
     Returns:
-        Actor network instance.
+        Model instance.
     """
 
-    def __init__(self, action_space: gym.Space, feature_dim: int = 64, hidden_dim: int = 1024) -> None:
+    def __init__(self, latent_dim, action_dim) -> None:
         super().__init__()
-        self.trunk = nn.Sequential(nn.LayerNorm(feature_dim), nn.Tanh())
 
-        self.policy = nn.Sequential(
-            nn.Linear(feature_dim, hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(hidden_dim, hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(hidden_dim, action_space.shape[0]),
-        )
-        # placeholder for distribution
-        self.dist = None
-
-        self.apply(utils.network_init)
+        self.trunk = nn.Sequential(nn.Linear(2 * latent_dim, 256), nn.ReLU(), nn.Linear(256, action_dim))
 
-    def get_action(self, obs: th.Tensor, step: int) -> Distribution:
-        """Get actions.
+    def forward(self, obs: th.Tensor, next_obs: th.Tensor) -> th.Tensor:
+        """Forward function for outputing predicted actions.
 
         Args:
-            obs (Tensor): Observations.
-            step (int): Global training step.
+            obs (Tensor): Current observations.
+            next_obs (Tensor): Next observations.
 
         Returns:
-            Hsuanwu distribution.
+            Predicted actions.
         """
-        h = self.trunk(obs)
-        mu = self.policy(h)
-        mu = th.tanh(mu)
-
-        # for Scheduled Exploration Noise
-        self.dist.reset(mu, step)
-
-        return self.dist
+        return self.trunk(th.cat([obs, next_obs], dim=1))
 
 
-class DoubleCritic(nn.Module):
-    """Double critic network for DrQv2 and SAC.
+class ForwardDynamicsModel(nn.Module):
+    """Forward model for reconstructing transition process.
 
     Args:
-        action_space (Space): Action space of the environment.
-        feature_dim (int): Number of features accepted.
-        hidden_dim (int): Number of units per hidden layer.
+        latent_dim (int): The dimension of encoding vectors of the observations.
+        action_dim (int): The dimension of predicted actions.
 
     Returns:
-        Critic network instance.
+        Model instance.
     """
 
-    def __init__(self, action_space: gym.Space, feature_dim: int = 64, hidden_dim: int = 1024) -> None:
+    def __init__(self, latent_dim, action_dim) -> None:
         super().__init__()
 
-        action_shape = action_space.shape
-        self.Q1 = nn.Sequential(
-            nn.Linear(feature_dim + action_shape[0], hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(hidden_dim, hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(hidden_dim, 1),
-        )
-
-        self.Q2 = nn.Sequential(
-            nn.Linear(feature_dim + action_shape[0], hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(hidden_dim, hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(hidden_dim, 1),
+        self.trunk = nn.Sequential(
+            nn.Linear(latent_dim + action_dim, 256),
+            nn.ReLU(),
+            nn.Linear(256, latent_dim),
         )
 
-        self.apply(utils.network_init)
-
-    def forward(self, obs: th.Tensor, action: th.Tensor) -> Tuple[th.Tensor, ...]:
-        """Value estimation.
+    def forward(self, obs: th.Tensor, pred_actions: th.Tensor) -> th.Tensor:
+        """Forward function for outputing predicted next-obs.
 
         Args:
-            obs (Tensor): Observations.
-            action (Tensor): Actions.
+            obs (Tensor): Current observations.
+            pred_actions (Tensor): Predicted observations.
 
         Returns:
-            Estimated values.
+            Predicted next-obs.
         """
-        h_action = th.cat([obs, action], dim=-1)
-
-        q1 = self.Q1(h_action)
-        q2 = self.Q2(h_action)
+        return self.trunk(th.cat([obs, pred_actions], dim=1))
 
-        return q1, q2
 
-
-class ActorCritic(nn.Module):
-    """Actor-Critic network for on-policy algorithms.
+class RIDE(BaseIntrinsicRewardModule):
+    """RIDE: Rewarding Impact-Driven Exploration for Procedurally-Generated Environments.
+        See paper: https://arxiv.org/pdf/2002.12292
 
     Args:
-        action_shape (Tuple): The data shape of actions.
-        action_type (str): The action type like 'Discrete' or 'Box', etc.
-        feature_dim (int): Number of features accepted.
-        hidden_dim (int): Number of units per hidden layer.
-        aux_critic (bool): Use auxiliary critic or not.
+        observation_space (Space or DictConfig): The observation space of environment. When invoked by Hydra,
+            'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+        action_space (Space or DictConfig): The action space of environment. When invoked by Hydra,
+            'action_space' is a 'DictConfig' like
+            {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+            {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+        device (str): Device (cpu, cuda, ...) on which the code should be run.
+        beta (float): The initial weighting coefficient of the intrinsic rewards.
+        kappa (float): The decay rate.
+        latent_dim (int): The dimension of encoding vectors.
+        lr (float): The learning rate.
+        batch_size (int): The batch size for update.
+        capacity (int): The of capacity the episodic memory.
+        k (int): Number of neighbors.
+        kernel_cluster_distance (float): The kernel cluster distance.
+        kernel_epsilon (float): The kernel constant.
+        c (float): The pseudo-counts constant.
+        sm (float): The kernel maximum similarity.
 
     Returns:
-        Actor-Critic instance.
+        Instance of RIDE.
     """
 
-    class DiscreteActor(nn.Module):
-        """Actor for 'Discrete' tasks."""
-
-        def __init__(self, action_shape, hidden_dim) -> None:
-            super().__init__()
-            self.actor = nn.Linear(hidden_dim, action_shape[0])
-
-        def forward(self, obs: th.Tensor, dist: Distribution) -> Distribution:
-            mu = self.actor(obs)
-            return dist(mu)
-
-    class BoxActor(nn.Module):
-        """Actor for 'Box' tasks."""
-
-        def __init__(self, action_shape, hidden_dim) -> None:
-            super().__init__()
-            self.actor_mu = nn.Linear(hidden_dim, action_shape[0])
-            self.actor_logstd = nn.Parameter(th.zeros(1, action_shape[0]))
-
-        def forward(self, obs: th.Tensor, dist: Distribution) -> Distribution:
-            mu = self.actor_mu(obs)
-            logstd = self.actor_logstd.expand_as(mu)
-            return dist(mu, logstd.exp())
-
     def __init__(
         self,
-        action_shape: Tuple,
-        action_type: str,
-        feature_dim: int,
-        hidden_dim: int,
-        aux_critic: bool = False,
+        observation_space: Union[gym.Space, DictConfig],
+        action_space: Union[gym.Space, DictConfig],
+        device: str = "cpu",
+        beta: float = 0.05,
+        kappa: float = 0.000025,
+        latent_dim: int = 128,
+        lr: float = 0.001,
+        batch_size: int = 64,
+        capacity: int = 1000,
+        k: int = 10,
+        kernel_cluster_distance: float = 0.008,
+        kernel_epsilon: float = 0.0001,
+        c: float = 0.001,
+        sm: float = 8.0,
     ) -> None:
-        super().__init__()
-
-        self.trunk = nn.Sequential(
-            nn.LayerNorm(feature_dim),
-            nn.Tanh(),
-            nn.Linear(feature_dim, hidden_dim),
-            nn.ReLU(),
-        )
-        if action_type == "Discrete":
-            self.base = self.DiscreteActor(action_shape=action_shape, hidden_dim=hidden_dim)
-        elif action_type == "Box":
-            self.base = self.BoxActor(action_shape=action_shape, hidden_dim=hidden_dim)
+        super().__init__(observation_space, action_space, device, beta, kappa)
+        self.encoder = Encoder(
+            obs_shape=observation_space.shape,
+            action_shape=action_space.shape,
+            latent_dim=latent_dim,
+        ).to(self._device)
+
+        self.im = InverseDynamicsModel(latent_dim=latent_dim, action_dim=self._action_shape[0]).to(self._device)
+        if self._action_shape == "Discrete":
+            self.im_loss = nn.CrossEntropyLoss()
         else:
-            raise NotImplementedError("Unsupported action type!")
-
-        self.critic = nn.Linear(hidden_dim, 1)
-        if aux_critic:
-            self.aux_critic = nn.Linear(hidden_dim, 1)
+            self.im_loss = nn.MSELoss()
 
-        # placeholder for distribution
-        self.dist = None
+        self.fm = ForwardDynamicsModel(latent_dim=latent_dim, action_dim=self._action_shape[0]).to(self._device)
 
-        self.apply(utils.network_init)
+        self.encoder_opt = th.optim.Adam(self.encoder.parameters(), lr=lr)
+        self.im_opt = th.optim.Adam(self.im.parameters(), lr=lr)
+        self.fm_opt = th.optim.Adam(self.fm.parameters(), lr=lr)
+        self.batch_size = batch_size
+
+        # episodic memory
+        self.episodic_memory = deque(maxlen=capacity)
+        self.k = k
+        self.kernel_cluster_distance = kernel_cluster_distance
+        self.kernel_epsilon = kernel_epsilon
+        self.c = c
+        self.sm = sm
 
-    def get_value(self, obs: th.Tensor) -> th.Tensor:
-        """Get estimated values for observations.
+    def pseudo_counts(self, e: th.Tensor) -> th.Tensor:
+        """Pseudo counts.
 
         Args:
-            obs (Tensor): Observations.
+            e (Tensor): Encoded observations.
 
         Returns:
-            Estimated values.
+            Conut values.
         """
-        return self.critic(self.trunk(obs))
+        num_steps = e.size()[0]
+        counts = th.zeros(size=(num_steps,))
+        memory = th.stack(list(self.episodic_memory)).squeeze(1)
+        for step in range(num_steps):
+            dist = th.norm(e[step] - memory, p=2, dim=1).sort().values[: self.k]
+            # moving average
+            dist = dist / (dist.mean() + 1e-11)
+            dist = th.maximum(dist - self.kernel_cluster_distance, th.zeros_like(dist))
+            kernel = self.kernel_epsilon / (dist + self.kernel_epsilon)
+            s = th.sqrt(kernel.sum()) + self.c
+
+            if s is th.nan or s > self.sm:
+                counts[step] = 0.0
+            else:
+                counts[step] = 1.0 / s
 
-    def get_action(self, obs: th.Tensor) -> th.Tensor:
-        """Get deterministic actions for observations.
+        return counts
 
-        Args:
-            obs (Tensor): Observations.
-
-        Returns:
-            Estimated values.
-        """
-        h = self.trunk(obs)
-        dist = self.base(h, self.dist)
-
-        return dist.mean
-
-    def get_action_and_value(self, obs: th.Tensor, actions: th.Tensor = None) -> Tuple[th.Tensor, ...]:
-        """Get actions and estimated values for observations.
-
-        Args:
-            obs (Tensor): Sampled observations.
-            actions (Tensor): Sampled actions.
-
-        Returns:
-            Actions, Estimated values, log of the probability evaluated at `actions`, entropy of distribution.
-        """
-        h = self.trunk(obs)
-        dist = self.base(h, self.dist)
-        if actions is None:
-            actions = dist.sample()
-
-        log_probs = dist.log_prob(actions)
-        entropy = dist.entropy().mean()
-
-        return actions, self.critic(h), log_probs, entropy
-
-    def get_probs_and_aux_value(self, obs: th.Tensor) -> Tuple[th.Tensor, ...]:
-        """Get probs and auxiliary estimated values for auxiliary phase update.
-
-        Args:
-            obs: Sampled observations.
-
-        Returns:
-            Distribution, estimated values, auxiliary estimated values.
-        """
-        h = self.trunk(obs)
-        dist = self.base(h, self.dist)
-
-        return dist, self.critic(h.detach()), self.aux_critic(h)
-
-    def get_logits(self, obs: th.Tensor) -> Distribution:
-        """Get the log-odds of sampling.
+    def compute_irs(self, samples: Dict, step: int = 0) -> th.Tensor:
+        """Compute the intrinsic rewards for current samples.
 
         Args:
-            obs: Sampled observations.
+            samples (Dict): The collected samples. A python dict like
+                {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+                actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+                rewards (n_steps, n_envs) <class 'th.Tensor'>,
+                next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
+            step (int): The global training step.
 
         Returns:
-            Distribution
+            The intrinsic rewards.
         """
-        h = self.trunk(obs)
-        dist = self.base(h, self.dist)
-        return dist
+        # compute the weighting coefficient of timestep t
+        beta_t = self._beta * np.power(1.0 - self._kappa, step)
+        num_steps = samples["obs"].size()[0]
+        num_envs = samples["obs"].size()[1]
+        obs_tensor = samples["obs"].to(self._device)
+        actions_tensor = samples["actions"]
+        if self._action_type == "Discrete":
+            actions_tensor = F.one_hot(actions_tensor.long(), self._action_shape[0]).float()
+            actions_tensor = actions_tensor.to(self._device)
+        next_obs_tensor = samples["next_obs"].to(self._device)
+
+        intrinsic_rewards = th.zeros(size=(num_steps, num_envs))
+
+        with th.no_grad():
+            for i in range(num_envs):
+                encoded_obs = self.encoder(obs_tensor[:, i])
+                encoded_next_obs = self.encoder(next_obs_tensor[:, i])
+
+                # TODO: add encodings into memory
+                self.episodic_memory.extend(encoded_next_obs.split(1))
+                n_eps = self.pseudo_counts(e=encoded_next_obs)
+
+                dist = F.mse_loss(encoded_next_obs, encoded_obs, reduction="none").sum(dim=1)
+                intrinsic_rewards[:, i] = dist.cpu() * n_eps
 
+        self.update(samples)
 
-class DiscreteLSTMActor(nn.Module):
-    def __init__(
-        self,
-        action_space,
-        feature_dim,
-        hidden_dim: int = 512,
-        use_lstm: bool = False,
-    ) -> None:
-        super().__init__()
-        """
-        Actor network for IMPALA  that supports LSTM module.
+        return intrinsic_rewards * beta_t
 
-        Args:
-            action_space (Space): Action space of the environment.
-            feature_dim (int): Number of features accepted.
-            hidden_dim (int): Number of units per hidden layer.
-            use_lstm (bool): Use LSTM or not.
-
-        Returns:
-            Actor network instance.
-        """
-        self.num_actions = action_space.shape[0]
-        self.use_lstm = use_lstm
-
-        # feature_dim + one-hot of last action + last reward
-        lstm_output_size = feature_dim + self.num_actions + 1
-        if use_lstm:
-            self.lstm = nn.LSTM(lstm_output_size, lstm_output_size, 2)
-
-        # policy logits
-        self.policy = nn.Linear(lstm_output_size, self.num_actions)
-        # baseline value function
-        self.baseline = nn.Linear(lstm_output_size, 1)
-
-        # internal encoder
-        self.encoder = None
-        self.dist = None
-
-    def init_state(self, batch_size: int) -> Tuple[th.Tensor, ...]:
-        """Generate the initial states for LSTM.
+    def update(self, samples: Dict) -> None:
+        """Update the intrinsic reward module if necessary.
 
         Args:
-            batch_size (int): The batch size for training.
+            samples: The collected samples. A python dict like
+                {obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>,
+                actions (n_steps, n_envs, *action_shape) <class 'th.Tensor'>,
+                rewards (n_steps, n_envs) <class 'th.Tensor'>,
+                next_obs (n_steps, n_envs, *obs_shape) <class 'th.Tensor'>}.
 
         Returns:
-            Initial states.
+            None
         """
-        if not self.use_lstm:
-            return tuple()
-        return tuple(th.zeros(self.lstm.num_layers, batch_size, self.lstm.hidden_size) for _ in range(2))
-
-    def get_action(
-        self,
-        inputs: Dict,
-        lstm_state: Tuple = (),
-        training: bool = True,
-    ) -> th.Tensor:
-        x = inputs["obs"]  # [T, B, *obs_shape], T: rollout length, B: batch size
-        T, B, *_ = x.shape
-        # TODO: merge time and batch
-        x = th.flatten(x, 0, 1)
-        # TODO: extract features from observations
-        features = F.relu(self.encoder(x))
-        # TODO: get one-hot last actions
-        one_hot_last_actions = F.one_hot(inputs["last_action"].view(T * B), self.num_actions).float()
-
-        clipped_reward = th.clamp(inputs["reward"], -1, 1).view(T * B, 1)
-        lstm_input = th.cat([features, clipped_reward, one_hot_last_actions], dim=-1)
-
-        if self.use_lstm:
-            lstm_input = lstm_input.view(T, B, -1)
-            lstm_output_list = []
-            notdone = (~inputs["terminated"]).float()
-            for input, nd in zip(lstm_input.unbind(), notdone.unbind()):
-                # Reset lstm state to zero whenever an episode ended.
-                # Make `done` broadcastable with (num_layers, B, hidden_size)
-                # states:
-                nd = nd.view(1, -1, 1)
-                lstm_state = tuple(nd * s for s in lstm_state)
-                output, lstm_state = self.lstm(input.unsqueeze(0), lstm_state)
-                lstm_output_list.append(output)
-            lstm_output = th.flatten(th.cat(lstm_output_list), 0, 1)
+        num_steps = samples["obs"].size()[0]
+        num_envs = samples["obs"].size()[1]
+        obs_tensor = samples["obs"].view((num_envs * num_steps, *self._obs_shape)).to(self._device)
+        next_obs_tensor = samples["next_obs"].view((num_envs * num_steps, *self._obs_shape)).to(self._device)
+
+        if self._action_type == "Discrete":
+            actions_tensor = samples["actions"].view(num_envs * num_steps).to(self._device)
+            actions_tensor = F.one_hot(actions_tensor.long(), self._action_shape[0]).float()
         else:
-            lstm_output = lstm_input
-            lstm_state = tuple()
+            actions_tensor = samples["actions"].view((num_envs * num_steps, self._action_shape[0])).to(self._device)
 
-        policy_logits = self.policy(lstm_output)
-        baseline = self.baseline(lstm_output)
+        dataset = TensorDataset(obs_tensor, actions_tensor, next_obs_tensor)
+        loader = DataLoader(dataset=dataset, batch_size=self.batch_size)
 
-        if training:
-            action = self.dist(policy_logits).sample()
-        else:
-            action = self.dist(policy_logits).mode
+        for _idx, batch in enumerate(loader):
+            obs, actions, next_obs = batch
 
-        policy_logits = policy_logits.view(T, B, self.num_actions)
-        baseline = baseline.view(T, B)
-        action = action.view(T, B)
-
-        return (
-            dict(policy_logits=policy_logits, baseline=baseline, action=action),
-            lstm_state,
-        )
+            self.encoder_opt.zero_grad()
+            self.im_opt.zero_grad()
+            self.fm_opt.zero_grad()
+
+            encoded_obs = self.encoder(obs)
+            encoded_next_obs = self.encoder(next_obs)
+
+            pred_actions = self.im(encoded_obs, encoded_next_obs)
+            im_loss = self.im_loss(pred_actions, actions)
+            pred_next_obs = self.fm(encoded_obs, actions)
+            fm_loss = F.mse_loss(pred_next_obs, encoded_next_obs)
+            (im_loss + fm_loss).backward()
+
+            self.encoder_opt.step()
+            self.im_opt.step()
+            self.fm_opt.step()
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/ppg.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/agent/ppg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import Dict, Tuple, Union
+import os
+from pathlib import Path
+from typing import Any, Dict, Tuple, Union
 
 import gymnasium as gym
 import numpy as np
 import torch as th
 from omegaconf import DictConfig
 from torch import nn
 
 from hsuanwu.xploit.agent.base import BaseAgent
-from hsuanwu.xploit.agent.network import ActorCritic
+from hsuanwu.xploit.agent.network import OnPolicySharedActorCritic
 from hsuanwu.xploit.storage import VanillaRolloutStorage as Storage
 
 MATCH_KEYS = {
     "trainer": "OnPolicyTrainer",
     "storage": ["VanillaRolloutStorage"],
     "distribution": ["Categorical", "DiagonalGaussian"],
     "augmentation": [],
@@ -128,76 +130,85 @@
         self.aux_epochs = aux_epochs
         self.kl_coef = kl_coef
         self.num_aux_grad_accum = num_aux_grad_accum
 
         # auxiliary storage
         self.aux_obs = None
         self.aux_returns = None
-        self.aux_logits = None
+        # self.aux_logits = None
+        self.aux_policy_outputs = None
 
         # create models
         self.encoder = None
         # create models
-        self.ac = ActorCritic(
+        self.ac = OnPolicySharedActorCritic(
             action_shape=self.action_shape,
             action_type=self.action_type,
             feature_dim=feature_dim,
             hidden_dim=hidden_dim,
             aux_critic=True,
-        ).to(self.device)
-
-        self.ac_opt = th.optim.Adam(self.ac.parameters(), lr=lr, eps=eps)
-        self.train()
+        )
 
     def train(self, training: bool = True) -> None:
         """Set the train mode.
 
         Args:
             training (bool): True (training) or False (testing).
 
         Returns:
             None.
         """
         self.training = training
         self.ac.train(training)
-        if self.encoder is not None:
-            self.encoder.train(training)
+
+    def integrate(self, **kwargs) -> None:
+        """Integrate agent and other modules (encoder, reward, ...) together"""
+        self.dist = kwargs["dist"]
+        self.ac.encoder = kwargs["encoder"]
+        self.ac.dist = kwargs["dist"]
+        # to device
+        self.ac.to(self.device)
+        # create optimizers
+        self.ac_opt = th.optim.Adam(self.ac.parameters(), lr=self.lr, eps=self.eps)
+        self.train()
+        if kwargs["aug"] is not None:
+            self.aug = kwargs["aug"]
+        if kwargs["irs"] is not None:
+            self.irs = kwargs["irs"]
 
     def get_value(self, obs: th.Tensor) -> th.Tensor:
         """Get estimated values for observations.
 
         Args:
             obs (Tensor): Observations.
 
         Returns:
             Estimated values.
         """
-        encoded_obs = self.encoder(obs)
-        return self.ac.get_value(obs=encoded_obs)
+        return self.ac.get_value(obs)
 
-    def act(self, obs: th.Tensor, training: bool = True, step: int = 0) -> Tuple[th.Tensor, ...]:
+    def act(self, obs: th.Tensor, training: bool = True, step: int = 0) -> Union[Tuple[th.Tensor, ...], Dict[str, Any]]:
         """Sample actions based on observations.
 
         Args:
             obs: Observations.
             training: training mode, True or False.
             step: Global training step.
 
         Returns:
             Sampled actions.
         """
-        encoded_obs = self.encoder(obs)
         if training:
-            actions, values, log_probs, entropy = self.ac.get_action_and_value(obs=encoded_obs)
-            return actions.clamp(*self.action_range), values, log_probs, entropy
+            actions, values, log_probs, entropy = self.ac.get_action_and_value(obs)
+            return {"actions": actions.clamp(*self.action_range), "values": values, "log_probs": log_probs}
         else:
-            actions = self.ac.get_action(obs=encoded_obs)
+            actions = self.ac.get_det_action(obs)
             return actions.clamp(*self.action_range)
 
-    def update(self, rollout_storage: Storage, episode: int = 0) -> Dict[str, float]:
+    def update(self, rollout_storage: Storage, episode: int = 0) -> Dict[str, float]:  # noqa: c901
         """Update the agent.
 
         Args:
             rollout_storage (Storage): Hsuanwu rollout storage.
             episode (int): Global training episode.
 
         Returns:
@@ -217,23 +228,36 @@
                 dtype=th.float32,
             )
             self.aux_returns = th.empty(
                 size=(num_steps, num_envs * self.policy_epochs),
                 device="cpu",
                 dtype=th.float32,
             )
-            self.aux_logits = th.empty(
-                size=(
-                    num_steps,
-                    num_envs * self.policy_epochs,
-                    self.action_shape[0],
-                ),
-                device="cpu",
-                dtype=th.float32,
-            )
+            if self.action_type == "Discrete":
+                self.aux_policy_outputs = th.empty(
+                    size=(
+                        num_steps,
+                        num_envs * self.policy_epochs,
+                        self.action_shape[0],
+                    ),
+                    device="cpu",
+                    dtype=th.float32,
+                )
+            elif self.action_type == "Box":
+                self.aux_policy_outputs = th.empty(
+                    size=(
+                        num_steps,
+                        num_envs * self.policy_epochs,
+                        self.action_shape[0] * 2,
+                    ),
+                    device="cpu",
+                    dtype=th.float32,
+                )
+            else:
+                raise NotImplementedError
             self.num_aux_rollouts = num_envs * self.policy_epochs
             self.num_envs = num_envs
             self.num_steps = num_steps
 
         idx = int(episode % self.policy_epochs)
         self.aux_obs[:, idx * self.num_envs : (idx + 1) * self.num_envs].copy_(rollout_storage.obs[:-1].clone())
         self.aux_returns[:, idx * self.num_envs : (idx + 1) * self.num_envs].copy_(rollout_storage.returns.clone())
@@ -266,15 +290,15 @@
                 batch_terminateds,
                 batch_truncateds,
                 batch_old_log_probs,
                 adv_targ,
             ) = batch
 
             # evaluate sampled actions
-            _, values, log_probs, entropy = self.ac.get_action_and_value(obs=self.encoder(batch_obs), actions=batch_actions)
+            _, values, log_probs, entropy = self.ac.get_action_and_value(obs=batch_obs, actions=batch_actions)
 
             # actor loss part
             ratio = th.exp(log_probs - batch_old_log_probs)
             surr1 = ratio * adv_targ
             surr2 = th.clamp(ratio, 1.0 - self.clip_range, 1.0 + self.clip_range) * adv_targ
             actor_loss = -th.min(surr1, surr2).mean()
 
@@ -283,33 +307,28 @@
             values_losses = (batch_values - batch_returns).pow(2)
             values_losses_clipped = (values_clipped - batch_returns).pow(2)
             critic_loss = 0.5 * th.max(values_losses, values_losses_clipped).mean()
 
             if self.aug is not None:
                 # augmentation loss part
                 batch_obs_aug = self.aug(batch_obs)
-                new_batch_actions, _, _, _ = self.ac.get_action_and_value(obs=self.encoder(batch_obs))
+                new_batch_actions, _, _, _ = self.ac.get_action_and_value(obs=batch_obs)
 
-                _, values_aug, log_probs_aug, _ = self.ac.get_action_and_value(
-                    obs=self.encoder(batch_obs_aug), actions=new_batch_actions
-                )
+                _, values_aug, log_probs_aug, _ = self.ac.get_action_and_value(obs=batch_obs_aug, actions=new_batch_actions)
                 action_loss_aug = -log_probs_aug.mean()
                 value_loss_aug = 0.5 * (th.detach(values) - values_aug).pow(2).mean()
                 aug_loss = self.aug_coef * (action_loss_aug + value_loss_aug)
             else:
                 aug_loss = th.scalar_tensor(s=0.0, requires_grad=False, device=critic_loss.device)
 
             # update
-            self.encoder_opt.zero_grad(set_to_none=True)
             self.ac_opt.zero_grad(set_to_none=True)
             (critic_loss * self.vf_coef + actor_loss - entropy * self.ent_coef + aug_loss).backward()
-            nn.utils.clip_grad_norm_(self.encoder.parameters(), self.max_grad_norm)
             nn.utils.clip_grad_norm_(self.ac.parameters(), self.max_grad_norm)
             self.ac_opt.step()
-            self.encoder_opt.step()
 
             total_actor_loss += actor_loss.item()
             total_critic_loss += critic_loss.item()
             total_entropy_loss += entropy.item()
             num_updates += 1
 
         total_actor_loss /= num_updates
@@ -328,53 +347,85 @@
         for idx in range(self.policy_epochs):
             with th.no_grad():
                 aux_obs = (
                     self.aux_obs[:, idx * self.num_envs : (idx + 1) * self.num_envs]
                     .to(self.device)
                     .reshape(-1, *self.aux_obs.size()[2:])
                 )
-                # get logits
-                logits = self.ac.get_logits(self.encoder(aux_obs)).logits.cpu().clone()
-                self.aux_logits[:, idx * self.num_envs : (idx + 1) * self.num_envs] = logits.reshape(
-                    self.num_steps, self.num_envs, self.aux_logits.size()[2]
+                # get policy outputs
+                policy_outputs = self.ac.get_policy_outputs(aux_obs).cpu().clone()
+                self.aux_policy_outputs[:, idx * self.num_envs : (idx + 1) * self.num_envs] = policy_outputs.reshape(
+                    self.num_steps, self.num_envs, self.aux_policy_outputs.size()[2]
                 )
 
         total_aux_value_loss = 0.0
         total_kl_loss = 0.0
 
         for e in range(self.aux_epochs):
             print("Auxiliary Phase", e)
             aux_inds = np.arange(self.num_aux_rollouts)
             np.random.shuffle(aux_inds)
 
             for idx in range(0, self.num_aux_rollouts, self.num_aux_mini_batch):
                 batch_inds = aux_inds[idx : idx + self.num_aux_mini_batch]
                 batch_aux_obs = self.aux_obs[:, batch_inds].reshape(-1, *self.aux_obs.size()[2:]).to(self.device)
                 batch_aux_returns = self.aux_returns[:, batch_inds].reshape(-1, *self.aux_returns.size()[2:]).to(self.device)
-                batch_aux_logits = self.aux_logits[:, batch_inds].reshape(-1, *self.aux_logits.size()[2:]).to(self.device)
+                # batch_aux_logits = self.aux_logits[:, batch_inds].reshape(-1, *self.aux_logits.size()[2:]).to(self.device)
+                batch_aux_policy_outputs = (
+                    self.aux_policy_outputs[:, batch_inds].reshape(-1, *self.aux_policy_outputs.size()[2:]).to(self.device)
+                )
 
-                new_dist, new_values, new_aux_values = self.ac.get_probs_and_aux_value(self.encoder(batch_aux_obs))
+                new_dist, new_values, new_aux_values = self.ac.get_probs_and_aux_value(batch_aux_obs)
 
                 new_values = new_values.view(-1)
                 new_aux_values = new_aux_values.view(-1)
-                old_dist = self.dist(logits=batch_aux_logits)
+                if self.action_type == "Discrete":
+                    old_dist = self.dist(batch_aux_policy_outputs)
+                elif self.action_type == "Box":
+                    old_dist = self.dist(*batch_aux_policy_outputs.chunk(2, dim=1))
+                else:
+                    raise NotImplementedError
                 # divergence loss
                 kl_loss = th.distributions.kl_divergence(old_dist, new_dist).mean()
                 # value loss
                 value_loss = 0.5 * (new_values - batch_aux_returns).mean()
                 aux_value_loss = 0.5 * (new_aux_values - batch_aux_returns).mean()
                 # total loss
                 (value_loss + aux_value_loss + self.kl_coef * kl_loss).backward()
 
                 if (idx + 1) % self.num_aux_grad_accum == 0:
-                    self.encoder_opt.zero_grad(set_to_none=True)
                     self.ac_opt.zero_grad(set_to_none=True)
-                    nn.utils.clip_grad_norm_(self.encoder.parameters(), self.max_grad_norm)
                     nn.utils.clip_grad_norm_(self.ac.parameters(), self.max_grad_norm)
-                    self.encoder_opt.step()
                     self.ac_opt.step()
 
                 total_aux_value_loss += value_loss.item()
                 total_aux_value_loss += aux_value_loss.item()
                 total_kl_loss += kl_loss.item()
 
         return {"aux_value_loss": total_aux_value_loss / self.aux_epochs, "kl_loss": total_kl_loss / self.aux_epochs}
+
+    def save(self, path: Path) -> None:
+        """Save models.
+
+        Args:
+            path (Path): Storage path.
+
+        Returns:
+            None.
+        """
+        if "pretrained" in str(path):  # pretraining
+            th.save(self.ac.state_dict(), path / "actor_critic.pth")
+        else:
+            del self.ac.critic
+            th.save(self.ac, path / "actor.pth")
+
+    def load(self, path: str) -> None:
+        """Load initial parameters.
+
+        Args:
+            path (str): Import path.
+
+        Returns:
+            None.
+        """
+        actor_critic_params = th.load(os.path.join(path, "actor_critic.pth"), map_location=self.device)
+        self.ac.load_state_dict(actor_critic_params)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/ppo.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/agent/ppo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from typing import Dict, Tuple, Union
+import os
+from pathlib import Path
+from typing import Any, Dict, Tuple, Union
 
 import gymnasium as gym
 import torch as th
 from omegaconf import DictConfig
 from torch import nn
 
 from hsuanwu.xploit.agent.base import BaseAgent
-from hsuanwu.xploit.agent.network import ActorCritic
+from hsuanwu.xploit.agent.network import OnPolicySharedActorCritic
 from hsuanwu.xploit.storage import VanillaRolloutStorage as Storage
 
 MATCH_KEYS = {
     "trainer": "OnPolicyTrainer",
     "storage": ["VanillaRolloutStorage"],
-    "distribution": ["Categorical", "DiagonalGaussian"],
+    "distribution": ["Categorical", "DiagonalGaussian", "Bernoulli"],
     "augmentation": [],
     "reward": [],
 }
 
 DEFAULT_CFGS = {
     ## TODO: Train setup
     "device": "cpu",
@@ -111,68 +113,75 @@
         self.num_mini_batch = num_mini_batch
         self.vf_coef = vf_coef
         self.ent_coef = ent_coef
         self.aug_coef = aug_coef
         self.max_grad_norm = max_grad_norm
 
         # create models
-        self.ac = ActorCritic(
+        self.ac = OnPolicySharedActorCritic(
             action_shape=self.action_shape,
             action_type=self.action_type,
             feature_dim=feature_dim,
             hidden_dim=hidden_dim,
-        ).to(self.device)
-
-        # create optimizers
-        self.ac_opt = th.optim.Adam(self.ac.parameters(), lr=lr, eps=eps)
-        self.train()
+        )
 
     def train(self, training: bool = True) -> None:
         """Set the train mode.
 
         Args:
             training (bool): True (training) or False (testing).
 
         Returns:
             None.
         """
         self.training = training
         self.ac.train(training)
-        if self.encoder is not None:
-            self.encoder.train(training)
+
+    def integrate(self, **kwargs) -> None:
+        """Integrate agent and other modules (encoder, reward, ...) together"""
+        self.dist = kwargs["dist"]
+        self.ac.encoder = kwargs["encoder"]
+        self.ac.dist = kwargs["dist"]
+        # to device
+        self.ac.to(self.device)
+        # create optimizers
+        self.ac_opt = th.optim.Adam(self.ac.parameters(), lr=self.lr, eps=self.eps)
+        self.train()
+        if kwargs["aug"] is not None:
+            self.aug = kwargs["aug"]
+        if kwargs["irs"] is not None:
+            self.irs = kwargs["irs"]
 
     def get_value(self, obs: th.Tensor) -> th.Tensor:
         """Get estimated values for observations.
 
         Args:
             obs (Tensor): Observations.
 
         Returns:
             Estimated values.
         """
-        encoded_obs = self.encoder(obs)
-        return self.ac.get_value(obs=encoded_obs)
+        return self.ac.get_value(obs)
 
-    def act(self, obs: th.Tensor, training: bool = True, step: int = 0) -> Tuple[th.Tensor, ...]:
+    def act(self, obs: th.Tensor, training: bool = True, step: int = 0) -> Union[Tuple[th.Tensor, ...], Dict[str, Any]]:
         """Sample actions based on observations.
 
         Args:
             obs: Observations.
             training: training mode, True or False.
             step: Global training step.
 
         Returns:
             Sampled actions.
         """
-        encoded_obs = self.encoder(obs)
         if training:
-            actions, values, log_probs, entropy = self.ac.get_action_and_value(obs=encoded_obs)
-            return actions.clamp(*self.action_range), values, log_probs, entropy
+            actions, values, log_probs, entropy = self.ac.get_action_and_value(obs)
+            return {"actions": actions.clamp(*self.action_range), "values": values, "log_probs": log_probs}
         else:
-            actions = self.ac.get_action(obs=encoded_obs)
+            actions = self.ac.get_det_action(obs)
             return actions.clamp(*self.action_range)
 
     def update(self, rollout_storage: Storage, episode: int = 0) -> Dict[str, float]:
         """Update the learner.
 
         Args:
             rollout_storage (Storage): Hsuanwu rollout storage.
@@ -194,15 +203,15 @@
                     "actions": rollout_storage.actions,
                     "next_obs": rollout_storage.obs[1:],
                 },
                 step=episode * num_envs * num_steps,
             )
             rollout_storage.rewards += intrinsic_reward.to(self.device)
 
-        for _e in range(self.n_epochs):
+        for _ in range(self.n_epochs):
             generator = rollout_storage.sample(self.num_mini_batch)
 
             for batch in generator:
                 (
                     batch_obs,
                     batch_actions,
                     batch_values,
@@ -210,17 +219,15 @@
                     batch_terminateds,
                     batch_truncateds,
                     batch_old_log_probs,
                     adv_targ,
                 ) = batch
 
                 # evaluate sampled actions
-                _, values, log_probs, entropy = self.ac.get_action_and_value(
-                    obs=self.encoder(batch_obs), actions=batch_actions
-                )
+                _, values, log_probs, entropy = self.ac.get_action_and_value(obs=batch_obs, actions=batch_actions)
 
                 # actor loss part
                 ratio = th.exp(log_probs - batch_old_log_probs)
                 surr1 = ratio * adv_targ
                 surr2 = th.clamp(ratio, 1.0 - self.clip_range, 1.0 + self.clip_range) * adv_targ
                 actor_loss = -th.min(surr1, surr2).mean()
 
@@ -229,33 +236,30 @@
                 values_losses = (batch_values - batch_returns).pow(2)
                 values_losses_clipped = (values_clipped - batch_returns).pow(2)
                 critic_loss = 0.5 * th.max(values_losses, values_losses_clipped).mean()
 
                 if self.aug is not None:
                     # augmentation loss part
                     batch_obs_aug = self.aug(batch_obs)
-                    new_batch_actions, _, _, _ = self.ac.get_action_and_value(obs=self.encoder(batch_obs))
+                    new_batch_actions, _, _, _ = self.ac.get_action_and_value(obs=batch_obs)
 
                     _, values_aug, log_probs_aug, _ = self.ac.get_action_and_value(
-                        obs=self.encoder(batch_obs_aug), actions=new_batch_actions
+                        obs=batch_obs_aug, actions=new_batch_actions
                     )
                     action_loss_aug = -log_probs_aug.mean()
                     value_loss_aug = 0.5 * (th.detach(values) - values_aug).pow(2).mean()
                     aug_loss = self.aug_coef * (action_loss_aug + value_loss_aug)
                 else:
                     aug_loss = th.scalar_tensor(s=0.0, requires_grad=False, device=critic_loss.device)
 
                 # update
-                self.encoder_opt.zero_grad(set_to_none=True)
                 self.ac_opt.zero_grad(set_to_none=True)
                 (critic_loss * self.vf_coef + actor_loss - entropy * self.ent_coef + aug_loss).backward()
-                nn.utils.clip_grad_norm_(self.encoder.parameters(), self.max_grad_norm)
                 nn.utils.clip_grad_norm_(self.ac.parameters(), self.max_grad_norm)
                 self.ac_opt.step()
-                self.encoder_opt.step()
 
                 total_actor_loss += actor_loss.item()
                 total_critic_loss += critic_loss.item()
                 total_entropy_loss += entropy.item()
                 total_aug_loss += aug_loss.item()
 
         num_updates = self.n_epochs * self.num_mini_batch
@@ -267,7 +271,34 @@
 
         return {
             "actor_loss": total_actor_loss,
             "critic_loss": total_critic_loss,
             "entropy": total_entropy_loss,
             "aug_loss": total_aug_loss,
         }
+
+    def save(self, path: Path) -> None:
+        """Save models.
+
+        Args:
+            path (Path): Storage path.
+
+        Returns:
+            None.
+        """
+        if "pretrained" in str(path):  # pretraining
+            th.save(self.ac.state_dict(), path / "actor_critic.pth")
+        else:
+            del self.ac.critic
+            th.save(self.ac, path / "actor.pth")
+
+    def load(self, path: str) -> None:
+        """Load initial parameters.
+
+        Args:
+            path (str): Import path.
+
+        Returns:
+            None.
+        """
+        actor_critic_params = th.load(os.path.join(path, "actor_critic.pth"), map_location=self.device)
+        self.ac.load_state_dict(actor_critic_params)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/sac.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/agent/sac.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import os
+from pathlib import Path
 from typing import Dict, Tuple, Union
 
 import gymnasium as gym
 import numpy as np
 import torch as th
 from omegaconf import DictConfig
 from torch.nn import functional as F
 
 from hsuanwu.xploit.agent import utils
 from hsuanwu.xploit.agent.base import BaseAgent
-from hsuanwu.xploit.agent.network import DoubleCritic, StochasticActor
+from hsuanwu.xploit.agent.network import OffPolicyDoubleCritic, OffPolicyStochasticActor
 
 MATCH_KEYS = {
     "trainer": "OffPolicyTrainer",
     "storage": ["VanillaReplayStorage", "PrioritizedReplayStorage"],
     "distribution": ["SquashedNormal"],
     "augmentation": [],
     "reward": [],
@@ -113,24 +115,26 @@
 
         self.critic_target_tau = critic_target_tau
         self.update_every_steps = update_every_steps
         self.fixed_temperature = fixed_temperature
         self.discount = discount
 
         # create models
-        self.actor = StochasticActor(
+        self.actor = OffPolicyStochasticActor(
             action_space=action_space,
             feature_dim=feature_dim,
             hidden_dim=hidden_dim,
             log_std_range=log_std_range,
         ).to(self.device)
-        self.critic = DoubleCritic(action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim).to(self.device)
-        self.critic_target = DoubleCritic(action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim).to(
+        self.critic = OffPolicyDoubleCritic(action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim).to(
             self.device
         )
+        self.critic_target = OffPolicyDoubleCritic(
+            action_space=action_space, feature_dim=feature_dim, hidden_dim=hidden_dim
+        ).to(self.device)
         self.critic_target.load_state_dict(self.critic.state_dict())
 
         # target entropy
         self.target_entropy = -np.prod(action_space.shape)
         self.log_alpha = th.tensor(np.log(temperature), device=self.device, requires_grad=True)
 
         # create optimizers
@@ -152,14 +156,26 @@
         """
         self.training = training
         self.actor.train(training)
         self.critic.train(training)
         if self.encoder is not None:
             self.encoder.train(training)
 
+    def integrate(self, **kwargs) -> None:
+        """Integrate agent and other modules (encoder, reward, ...) together"""
+        self.encoder = kwargs["encoder"]
+        self.encoder_opt = th.optim.Adam(self.encoder.parameters(), lr=self.lr, eps=self.eps)
+        self.encoder.train()
+        self.dist = kwargs["dist"]
+        self.actor.dist = kwargs["dist"]
+        if kwargs["aug"] is not None:
+            self.aug = kwargs["aug"]
+        if kwargs["irs"] is not None:
+            self.irs = kwargs["irs"]
+
     @property
     def alpha(self) -> th.Tensor:
         """Get the temperature coefficient."""
         return self.log_alpha.exp()
 
     def act(self, obs: th.Tensor, training: bool = True, step: int = 0) -> Tuple[th.Tensor]:
         """Sample actions based on observations.
@@ -169,15 +185,15 @@
             training (bool): training mode, True or False.
             step (int): Global training step.
 
         Returns:
             Sampled actions.
         """
         encoded_obs = self.encoder(obs)
-        dist = self.actor.get_action(obs=encoded_obs, step=step)
+        dist = self.actor.get_dist(obs=encoded_obs, step=step)
 
         if not training:
             action = dist.mean
         else:
             action = dist.sample()
 
         return action.clamp(*self.action_range)
@@ -287,24 +303,24 @@
             aug_next_obs (Tensor): Augmented next observations.
             step (int): Global training step.
 
         Returns:
             Critic loss metrics.
         """
         with th.no_grad():
-            dist = self.actor.get_action(next_obs, step=step)
+            dist = self.actor.get_dist(next_obs, step=step)
             next_action = dist.rsample()
             log_prob = dist.log_prob(next_action).sum(-1, keepdim=True)
             target_Q1, target_Q2 = self.critic_target(next_obs, next_action)
             target_V = th.min(target_Q1, target_Q2) - self.alpha.detach() * log_prob
             target_Q = reward + (1.0 - terminated) * self.discount * target_V
 
             # enable observation augmentation
             if self.aug is not None:
-                dist_aug = self.actor.get_action(aug_next_obs, step=step)
+                dist_aug = self.actor.get_dist(aug_next_obs, step=step)
                 next_action_aug = dist_aug.rsample()
                 log_prob_aug = dist_aug.log_prob(next_action_aug).sum(-1, keepdim=True)
                 target_Q1, target_Q2 = self.critic_target(aug_next_obs, next_action_aug)
                 target_V = th.min(target_Q1, target_Q2) - self.alpha.detach() * log_prob_aug
                 target_Q_aug = reward + (1.0 - terminated) * self.discount * target_V
                 # mixed target Q-function
                 target_Q = (target_Q + target_Q_aug) / 2
@@ -344,15 +360,15 @@
             weights (Tensor): Batch sample weights.
             step (int): Global training step.
 
         Returns:
             Actor loss metrics.
         """
         # sample actions
-        dist = self.actor.get_action(obs, step=step)
+        dist = self.actor.get_dist(obs, step=step)
         action = dist.rsample()
         log_prob = dist.log_prob(action).sum(-1, keepdim=True)
         Q1, Q2 = self.critic(obs, action)
         Q = th.min(Q1, Q2)
 
         actor_loss = ((self.alpha.detach() * log_prob - Q) * weights).mean()
 
@@ -367,7 +383,41 @@
             alpha_loss = (self.alpha * (-log_prob - self.target_entropy).detach() * weights).mean()
             alpha_loss.backward()
             self.log_alpha_opt.step()
         else:
             alpha_loss = th.scalar_tensor(s=0.0)
 
         return {"actor_loss": actor_loss.item(), "alpha_loss": alpha_loss.item()}
+
+    def save(self, path: Path) -> None:
+        """Save models.
+
+        Args:
+            path (Path): Storage path.
+
+        Returns:
+            None.
+        """
+        if "pretrained" in str(path):  # pretraining
+            th.save(self.encoder.state_dict(), path / "encoder.pth")
+            th.save(self.actor.state_dict(), path / "actor.pth")
+            th.save(self.critic.state_dict(), path / "critic.pth")
+        else:
+            th.save(self.encoder, path / "encoder.pth")
+            th.save(self.actor, path / "actor.pth")
+            th.save(self.critic, path / "critic.pth")
+
+    def load(self, path: str) -> None:
+        """Load initial parameters.
+
+        Args:
+            path (str): Import path.
+
+        Returns:
+            None.
+        """
+        encoder_params = th.load(os.path.join(path, "encoder.pth"), map_location=self.device)
+        actor_params = th.load(os.path.join(path, "actor.pth"), map_location=self.device)
+        critic_params = th.load(os.path.join(path, "critic.pth"), map_location=self.device)
+        self.encoder.load_state_dict(encoder_params)
+        self.actor.load_state_dict(actor_params)
+        self.critic.load_state_dict(critic_params)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/utils.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/agent/utils.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/base.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/base.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/espeholt_residual_encoder.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/espeholt_residual_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,17 @@
             shape = shape[1:]
 
         for out_channels in net_arch:
             layer = ResidualLayer(shape, out_channels)
             shape = layer.get_output_shape()
             modules.append(layer)
         modules.append(nn.Flatten())
-
+        modules.append(nn.Linear(in_features=shape[0] * shape[1] * shape[2], out_features=feature_dim))
+        modules.append(nn.ReLU())
         self.trunk = nn.Sequential(*modules)
-        self.linear = nn.Linear(in_features=shape[0] * shape[1] * shape[2], out_features=feature_dim)
 
         self.apply(network_init)
 
     def forward(self, obs: th.Tensor) -> th.Tensor:
         obs = obs / 255.0
         h = self.trunk(obs)
-        return self.linear(h)
+        return h
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/identity_encoder.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/identity_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,11 +21,12 @@
     """
 
     def __init__(self, observation_space: Union[gym.Space, DictConfig], feature_dim: int = 64) -> None:
         super().__init__(observation_space, feature_dim)
 
         obs_shape = observation_space.shape
         assert len(obs_shape) == 1
-        self.trunk = nn.Sequential(nn.Linear(1, 1))
+        self.trunk = nn.Sequential(nn.Identity(obs_shape[0]))
+        self.unused = nn.Linear(1, 1)  # for avoiding the ValueError: optimizer got an empty parameter list
 
     def forward(self, obs: th.Tensor) -> th.Tensor:
-        return obs
+        return self.trunk(obs)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/mnih_cnn_encoder.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/mnih_cnn_encoder.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,16 +39,15 @@
             nn.Flatten(),
         )
 
         with th.no_grad():
             sample = th.ones(size=tuple(obs_shape)).float()
             n_flatten = self.trunk(sample.unsqueeze(0)).shape[1]
 
-        self.linear = nn.Linear(n_flatten, feature_dim)
-
+        self.trunk.extend([nn.Linear(n_flatten, feature_dim), nn.ReLU()])
         # self.apply(network_init)
 
     def forward(self, obs: th.Tensor) -> th.Tensor:
         obs = obs / 255.0
         h = self.trunk(obs)
 
-        return self.linear(h.view(h.size()[0], -1))
+        return h.view(h.size()[0], -1)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/tassa_cnn_encoder.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/tassa_cnn_encoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,17 +40,16 @@
             nn.Flatten(),
         )
 
         with th.no_grad():
             sample = th.ones(size=tuple(obs_shape)).float()
             n_flatten = self.trunk(sample.unsqueeze(0)).shape[1]
 
-        self.linear = nn.Linear(n_flatten, feature_dim)
-        self.layer_norm = nn.LayerNorm(feature_dim)
+        self.trunk.append(nn.Linear(n_flatten, feature_dim))
 
         self.apply(network_init)
 
     def forward(self, obs: th.Tensor) -> th.Tensor:
         obs = obs / 255.0 - 0.5
         h = self.trunk(obs)
 
-        return self.layer_norm(self.linear(h.view(h.size()[0], -1)))
+        return h.view(h.size()[0], -1)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/vanilla_mlp_encoder.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/encoder/vanilla_mlp_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,13 +32,14 @@
         input_dim = observation_space.shape[0]
         self.trunk = nn.Sequential(
             nn.Linear(input_dim, hidden_dim),
             nn.ReLU(),
             nn.Linear(hidden_dim, hidden_dim),
             nn.ReLU(),
             nn.Linear(hidden_dim, feature_dim),
+            nn.ReLU(),
         )
 
         self.apply(network_init)
 
     def forward(self, obs: th.Tensor) -> th.Tensor:
         return self.trunk(obs)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/base.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/storage/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,7 +52,11 @@
     @abstractmethod
     def add(self, *args) -> None:
         """Add sampled transitions into storage."""
 
     @abstractmethod
     def sample(self, *args) -> Any:
         """Sample from the storage."""
+
+    @abstractmethod
+    def update(self, *args) -> None:
+        """Update the storage"""
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/distributed_storage.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/storage/distributed_storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -39,32 +39,48 @@
         super().__init__(observation_space, action_space, device)
         self._num_steps = num_steps
         self._num_storages = num_storages
         self._batch_size = batch_size
 
         if self._action_type == "Discrete":
             self._action_dim = 1
+            policy_outputs_dim = self._action_shape[0]
+
+            specs = dict(
+                obs=dict(size=(num_steps + 1, *self._obs_shape), dtype=th.uint8),
+                reward=dict(size=(num_steps + 1,), dtype=th.float32),
+                terminated=dict(size=(num_steps + 1,), dtype=th.bool),
+                truncated=dict(size=(num_steps + 1,), dtype=th.bool),
+                episode_return=dict(size=(num_steps + 1,), dtype=th.float32),
+                episode_step=dict(size=(num_steps + 1,), dtype=th.int32),
+                last_action=dict(size=(num_steps + 1,), dtype=th.int64),
+                policy_outputs=dict(size=(num_steps + 1, policy_outputs_dim), dtype=th.float32),
+                baseline=dict(size=(num_steps + 1,), dtype=th.float32),
+                action=dict(size=(num_steps + 1,), dtype=th.int64),
+            )
+
         elif self._action_type == "Box":
             self._action_dim = self._action_shape[0]
+            policy_outputs_dim = self._action_shape[0] * 2
+
+            specs = dict(
+                obs=dict(size=(num_steps + 1, *self._obs_shape), dtype=th.uint8),
+                reward=dict(size=(num_steps + 1,), dtype=th.float32),
+                terminated=dict(size=(num_steps + 1,), dtype=th.bool),
+                truncated=dict(size=(num_steps + 1,), dtype=th.bool),
+                episode_return=dict(size=(num_steps + 1,), dtype=th.float32),
+                episode_step=dict(size=(num_steps + 1,), dtype=th.int32),
+                last_action=dict(size=(num_steps + 1, self._action_dim), dtype=th.float32),
+                policy_outputs=dict(size=(num_steps + 1, policy_outputs_dim), dtype=th.float32),
+                baseline=dict(size=(num_steps + 1,), dtype=th.float32),
+                action=dict(size=(num_steps + 1, self._action_dim), dtype=th.float32),
+            )
         else:
             raise NotImplementedError
 
-        specs = dict(
-            obs=dict(size=(num_steps + 1, *self._obs_shape), dtype=th.uint8),
-            reward=dict(size=(num_steps + 1,), dtype=th.float32),
-            terminated=dict(size=(num_steps + 1,), dtype=th.bool),
-            truncated=dict(size=(num_steps + 1,), dtype=th.bool),
-            episode_return=dict(size=(num_steps + 1,), dtype=th.float32),
-            episode_step=dict(size=(num_steps + 1,), dtype=th.int32),
-            last_action=dict(size=(num_steps + 1,), dtype=th.int64),
-            policy_logits=dict(size=(num_steps + 1, self._action_shape[0]), dtype=th.float32),
-            baseline=dict(size=(num_steps + 1,), dtype=th.float32),
-            action=dict(size=(num_steps + 1,), dtype=th.int64),
-        )
-
         self.storages = {key: [] for key in specs}
         for _ in range(num_storages):
             for key in self.storages:
                 self.storages[key].append(th.empty(**specs[key]).share_memory_())
 
     def add(self, *args) -> None:
         """Add sampled transitions into storage."""
@@ -100,7 +116,10 @@
         init_actor_states = (th.cat(ts, dim=1) for ts in zip(*[init_actor_state_storages[i] for i in indices]))
 
         for i in indices:
             free_queue.put(i)
 
         batch = {key: tensor.to(device=th.device(device), non_blocking=True) for key, tensor in batch.items()}
         return batch, init_actor_states
+
+    def update(self, *args) -> None:
+        """Update the storage"""
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/nstep_replay_storage.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/storage/nstep_replay_storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
 import random
 import traceback
 from collections import defaultdict
 from pathlib import Path
-from typing import Any, Dict, Tuple, Union
+from typing import Any, Dict, Iterator, Tuple, Union
 
 import gymnasium as gym
 import numpy as np
 import torch as th
 from omegaconf import DictConfig
 from torch.utils.data import IterableDataset
 
-from hsuanwu.xploit.storage.utils import dump_episode, episode_len, load_episode
+from hsuanwu.xploit.storage.base import BaseStorage
+from hsuanwu.xploit.storage.utils import dump_episode, episode_len, load_episode, worker_init_fn
 
 
 class ReplayStorage:
     """Storage collected experiences to local files.
 
     Args:
         replay_dir (Path): save directory.
@@ -61,118 +62,61 @@
                 episode[key] = np.array(self._current_episode[key])
 
             # save episode to file
             self._store_episode(episode)
             self._current_episode = defaultdict(list)
 
 
-class NStepReplayStorage(IterableDataset):
-    """Replay storage for off-policy algorithms (N-step returns supported).
+class NStepReplayDataset(IterableDataset):
+    """Iterable replay dataset (N-step returns supported).
+        Based on: https://github.com/facebookresearch/drqv2
 
     Args:
-        observation_space (Space or DictConfig): The observation space of environment. When invoked by Hydra,
-            'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
-        action_space (Space or DictConfig): The action space of environment. When invoked by Hydra,
-            'action_space' is a 'DictConfig' like
-            {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
-            {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
-        device (str): Device (cpu, cuda, ...) on which the code should be run.
+        replay_dir (Path): Replay directory.
         storage_size (int): Max number of element in the storage.
-        batch_size (int): Number of samples per batch to load.
         num_workers (int): Subprocesses to use for data loading.
-        pin_memory (bool): Copy Tensors into device/CUDA pinned memory before returning them.
         n_step (int) The number of transitions to consider when computing n-step returns
         discount (float): The discount factor for future rewards.
         fetch_every (int): Loading interval.
         save_snapshot (bool): Save loaded file or not.
 
     Returns:
-        N-step replay storage.
+        Iterable replay dataset.
     """
 
     def __init__(
         self,
-        observation_space: Union[gym.Space, DictConfig],
-        action_space: Union[gym.Space, DictConfig],
-        device: str = "cpu",
+        replay_dir: Path,
         storage_size: int = 500000,
-        batch_size: int = 256,
         num_workers: int = 4,
-        pin_memory: bool = True,
         n_step: int = 3,
         discount: float = 0.99,
         fetch_every: int = 1000,
         save_snapshot: bool = False,
     ) -> None:
         # set storage
-        self._replay_dir = Path.cwd() / "storage"
-        self._replay_storage = ReplayStorage(self._replay_dir)
+        self._replay_dir = replay_dir
         self._storage_size = storage_size
-        self._batch_size = batch_size
         self._num_workers = max(1, num_workers)
-        self._pin_memory = pin_memory
         self._n_step = n_step
         self._discount = discount
         self._save_snapshot = save_snapshot
 
         # setup for single worker
         self._worker_eps_pool = dict()
         self._worker_eps_fn_pool = list()
         self._worker_size = 0
         self._worker_max_size = storage_size // max(1, num_workers)
         self._fetch_every = fetch_every
         self._fetched_samples = fetch_every
 
-    @property
-    def get_batch_size(self):
-        return self._batch_size
-
-    @property
-    def get_num_workers(self):
-        return self._num_workers
-
-    @property
-    def get_pin_memory(self):
-        return self._pin_memory
-
     def _sample_episode(self) -> Dict:
         eps_fn = random.choice(self._worker_eps_fn_pool)
         return self._worker_eps_pool[eps_fn]
 
-    def add(
-        self,
-        obs: Any,
-        action: Any,
-        reward: Any,
-        terminated: Any,
-        info: Any,
-        next_obs: Any,
-    ) -> None:
-        """Add sampled transitions into storage.
-
-        Args:
-            obs (Any): Observations.
-            action (Any): Actions.
-            reward (Any): Rewards.
-            terminated (Any): Terminateds.
-            info (Any): Infos.
-            next_obs (Any): Next observations.
-
-        Returns:
-            None.
-        """
-        if "discount" in info.keys():
-            discount = info["discount"][0]
-        elif "discount" in info["final_info"][0].keys():
-            discount = info["final_info"][0]["discount"]
-        else:
-            raise ValueError("When using NStepReplayStorage, please put the discount factor in 'info'!")
-
-        self._replay_storage.add(obs, action, reward, terminated, discount)
-
     def _store_episode(self, eps_fn: Path) -> bool:
         try:
             episode = load_episode(eps_fn)
         except:  # noqa E722
             return False
         eps_len = episode_len(episode)
         while eps_len + self._worker_size > self._worker_max_size:
@@ -207,15 +151,15 @@
                 break
             if fetched_size + eps_len > self._worker_max_size:
                 break
             fetched_size += eps_len
             if not self._store_episode(eps_fn):
                 break
 
-    def sample(self) -> Tuple:
+    def _sample(self) -> Tuple:
         """Generate samples.
 
         Args:
             None.
 
         Returns:
             Batched samples.
@@ -237,8 +181,122 @@
             step_reward = episode["reward"][idx + i]
             reward += discount * step_reward
             discount *= episode["discount"][idx + i] * self._discount
         return (obs, action, reward, discount, next_obs)
 
     def __iter__(self):
         while True:
-            yield self.sample()
+            yield self._sample()
+
+
+class NStepReplayStorage(BaseStorage):
+    """Replay storage for off-policy algorithms (N-step returns supported).
+
+    Args:
+        observation_space (Space or DictConfig): The observation space of environment. When invoked by Hydra,
+            'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
+        action_space (Space or DictConfig): The action space of environment. When invoked by Hydra,
+            'action_space' is a 'DictConfig' like
+            {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
+            {"shape": action_space.shape, "type": "Box", "range": [action_space.low[0], action_space.high[0]]}.
+        device (str): Device (cpu, cuda, ...) on which the code should be run.
+        storage_size (int): Max number of element in the storage.
+        batch_size (int): Number of samples per batch to load.
+        num_workers (int): Subprocesses to use for data loading.
+        pin_memory (bool): Copy Tensors into device/CUDA pinned memory before returning them.
+        n_step (int) The number of transitions to consider when computing n-step returns
+        discount (float): The discount factor for future rewards.
+        fetch_every (int): Loading interval.
+        save_snapshot (bool): Save loaded file or not.
+
+    Returns:
+        N-step replay storage.
+    """
+
+    def __init__(
+        self,
+        observation_space: Union[gym.Space, DictConfig],
+        action_space: Union[gym.Space, DictConfig],
+        device: str = "cpu",
+        storage_size: int = 500000,
+        batch_size: int = 256,
+        num_workers: int = 4,
+        pin_memory: bool = True,
+        n_step: int = 3,
+        discount: float = 0.99,
+        fetch_every: int = 1000,
+        save_snapshot: bool = False,
+    ) -> None:
+        self._replay_dir = Path.cwd() / "storage"
+        self._replay_storage = ReplayStorage(self._replay_dir)
+        self._replay_dataset = NStepReplayDataset(
+            replay_dir=self._replay_dir,
+            storage_size=storage_size,
+            num_workers=num_workers,
+            n_step=n_step,
+            discount=discount,
+            fetch_every=fetch_every,
+            save_snapshot=save_snapshot,
+        )
+
+        # make data loader
+        self._replay_loader = th.utils.data.DataLoader(
+            self._replay_dataset,
+            batch_size=batch_size,
+            num_workers=num_workers,
+            pin_memory=pin_memory,
+            worker_init_fn=worker_init_fn,
+        )
+
+        self._replay_iter = None
+
+    def add(
+        self,
+        obs: Any,
+        action: Any,
+        reward: Any,
+        terminated: Any,
+        info: Any,
+        next_obs: Any,
+    ) -> None:
+        """Add sampled transitions into storage.
+
+        Args:
+            obs (Any): Observations.
+            action (Any): Actions.
+            reward (Any): Rewards.
+            terminated (Any): Terminateds.
+            info (Any): Infos.
+            next_obs (Any): Next observations.
+
+        Returns:
+            None.
+        """
+        if "discount" in info.keys():
+            discount = info["discount"][0]
+        elif "discount" in info["final_info"][0].keys():
+            discount = info["final_info"][0]["discount"]
+        else:
+            raise ValueError("When using NStepReplayStorage, please put the discount factor in 'info'!")
+
+        self._replay_storage.add(obs, action, reward, terminated, discount)
+
+    @property
+    def replay_iter(self) -> Iterator:
+        """Create iterable dataloader."""
+        if self._replay_iter is None:
+            self._replay_iter = iter(self._replay_loader)
+        return self._replay_iter
+
+    def sample(self, step: int) -> Tuple:
+        """Generate samples.
+
+        Args:
+            step (int): Global training step.
+
+        Returns:
+            Batched samples.
+        """
+        return next(self.replay_iter)
+
+    def update(self, *args) -> None:
+        """Update the storage"""
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/prioritized_replay_storage.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/storage/prioritized_replay_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import deque
-from typing import Any, Tuple, Union
+from typing import Any, Dict, Tuple, Union
 
 import gymnasium as gym
 import numpy as np
 import torch as th
 from omegaconf import DictConfig
 
 from hsuanwu.xploit.storage.base import BaseStorage
@@ -126,19 +126,21 @@
         rewards = th.as_tensor(rewards, device=self._device).float()
         next_obs = th.as_tensor(next_obs, device=self._device).float()
         terminateds = th.as_tensor(terminateds, device=self._device).float()
         weights = th.as_tensor(weights, device=self._device).float()
 
         return indices, obs, actions, rewards, terminateds, next_obs, weights
 
-    def update_priorities(self, indices: np.ndarray, priorities: np.ndarray) -> None:
+    def update(self, metrics: Dict) -> None:
         """Update the priorities.
 
         Args:
-            indices (NdArray): The indices of current batch data.
-            priorities (NdArray): The priorities of current batch data.
+            metrics (Dict): Training metrics from agent to udpate the priorities:
+                indices (NdArray): The indices of current batch data.
+                priorities (NdArray): The priorities of current batch data.
 
         Returns:
             None.
         """
-        for i, priority in zip(indices, priorities):
-            self._priorities[i] = abs(priority)
+        if "indices" in metrics and "priorities" in metrics:
+            for i, priority in zip(metrics["indices"], metrics["priorities"]):
+                self._priorities[i] = abs(priority)
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/utils.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/storage/utils.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/vanilla_replay_storage.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/storage/vanilla_replay_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,7 +107,10 @@
         actions = th.as_tensor(self.actions[indices], device=self._device).float()
         rewards = th.as_tensor(self.rewards[indices], device=self._device).float()
         next_obs = th.as_tensor(self.obs[(indices + 1) % self._storage_size], device=self._device).float()
         terminateds = th.as_tensor(self.terminateds[indices], device=self._device).float()
         weights = th.ones_like(terminateds, device=self._device)
 
         return indices, obs, actions, rewards, terminateds, next_obs, weights
+
+    def update(self, *args) -> None:
+        """Update the storage"""
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/vanilla_rollout_storage.py` & `hsuanwu-0.0.1b5/hsuanwu/xploit/storage/decoupled_rollout_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import torch as th
 from omegaconf import DictConfig
 from torch.utils.data.sampler import BatchSampler, SubsetRandomSampler
 
 from hsuanwu.xploit.storage.base import BaseStorage
 
 
-class VanillaRolloutStorage(BaseStorage):
-    """Vanilla rollout storage for on-policy algorithms.
+class DecoupledRolloutStorage(BaseStorage):
+    """Decoupled rollout storage for on-policy algorithms like DAAC.
 
     Args:
         observation_space (Space or DictConfig): The observation space of environment. When invoked by Hydra,
             'observation_space' is a 'DictConfig' like {"shape": observation_space.shape, }.
         action_space (Space or DictConfig): The action space of environment. When invoked by Hydra,
             'action_space' is a 'DictConfig' like
             {"shape": (n, ), "type": "Discrete", "range": [0, n - 1]} or
@@ -49,79 +49,90 @@
             size=(num_steps + 1, num_envs, *self._obs_shape),
             dtype=th.float32,
             device=self._device,
         )
         if self._action_type == "Discrete":
             self._action_dim = 1
             self.actions = th.empty(
-                size=(num_steps, num_envs, self._action_dim),
+                size=(num_steps, num_envs),
                 dtype=th.float32,
                 device=self._device,
             )
         elif self._action_type == "Box":
             self._action_dim = self._action_shape[0]
             self.actions = th.empty(
                 size=(num_steps, num_envs, self._action_dim),
                 dtype=th.float32,
                 device=self._device,
             )
+        elif self._action_type == "MultiBinary":
+            self._action_dim = self._action_shape[0]
+            self.actions = th.empty(
+                size=(num_steps, num_envs, self._action_dim),
+                dtype=th.float32,
+                device=self._device,
+            )
         else:
             raise NotImplementedError
         self.rewards = th.empty(size=(num_steps, num_envs), dtype=th.float32, device=self._device)
         self.terminateds = th.empty(size=(num_steps + 1, num_envs), dtype=th.float32, device=self._device)
         self.truncateds = th.empty(size=(num_steps + 1, num_envs), dtype=th.float32, device=self._device)
         # first next_terminated
         self.terminateds[0].copy_(th.zeros(num_envs).to(self._device))
         self.truncateds[0].copy_(th.zeros(num_envs).to(self._device))
         # extra part
         self.log_probs = th.empty(size=(num_steps, num_envs), dtype=th.float32, device=self._device)
         self.values = th.empty(size=(num_steps, num_envs), dtype=th.float32, device=self._device)
         self.returns = th.empty(size=(num_steps, num_envs), dtype=th.float32, device=self._device)
         self.advantages = th.empty(size=(num_steps, num_envs), dtype=th.float32, device=self._device)
+        self.adv_preds = th.empty(size=(num_steps, num_envs), dtype=th.float32, device=self._device)
 
         self._global_step = 0
 
     def add(
         self,
         obs: th.Tensor,
         actions: th.Tensor,
         rewards: th.Tensor,
         terminateds: th.Tensor,
         truncateds: th.Tensor,
         next_obs: th.Tensor,
         log_probs: th.Tensor,
         values: th.Tensor,
+        adv_preds: th.Tensor,
     ) -> None:
         """Add sampled transitions into storage.
 
         Args:
             obs (Tensor): Observations.
             actions (Tensor): Actions.
             rewards (Tensor): Rewards.
             terminateds (Tensor): Terminateds.
             truncateds (Tensor): Truncateds.
             next_obs (Tensor): Next observations.
             log_probs (Tensor): Log of the probability evaluated at `actions`.
             values (Tensor): Estimated values.
+            adv_preds (Tensor): Predicted advantages.
 
         Returns:
             None.
         """
         self.obs[self._global_step].copy_(obs)
         self.actions[self._global_step].copy_(actions)
         self.rewards[self._global_step].copy_(rewards)
         self.terminateds[self._global_step + 1].copy_(terminateds)
         self.truncateds[self._global_step + 1].copy_(truncateds)
         self.obs[self._global_step + 1].copy_(next_obs)
-        self.log_probs[self._global_step].copy_(log_probs[:, 0])
+        self.log_probs[self._global_step].copy_(log_probs)
         self.values[self._global_step].copy_(values[:, 0])
+        self.adv_preds[self._global_step].copy_(adv_preds[:, 0])
 
         self._global_step = (self._global_step + 1) % self._num_steps
 
-    def reset(self) -> None:
+    def update(self) -> None:
         """Reset the terminal state of each env."""
         self.terminateds[0].copy_(self.terminateds[-1])
         self.truncateds[0].copy_(self.truncateds[-1])
 
     def compute_returns_and_advantages(self, last_values: th.Tensor) -> None:
         """Perform generalized advantage estimation (GAE).
 
@@ -169,23 +180,25 @@
 
         sampler = BatchSampler(SubsetRandomSampler(range(batch_size)), mini_batch_size, drop_last=True)
 
         for indices in sampler:
             batch_obs = self.obs[:-1].view(-1, *self._obs_shape)[indices]
             batch_actions = self.actions.view(-1, self._action_dim)[indices]
             batch_values = self.values.view(-1, 1)[indices]
+            batch_adv_preds = self.adv_preds.view(-1, 1)[indices]
             batch_returns = self.returns.view(-1, 1)[indices]
             batch_terminateds = self.terminateds[:-1].view(-1, 1)[indices]
             batch_truncateds = self.truncateds[:-1].view(-1, 1)[indices]
             batch_old_log_probs = self.log_probs.view(-1, 1)[indices]
             adv_targ = self.advantages.view(-1, 1)[indices]
 
             yield (
                 batch_obs,
                 batch_actions,
                 batch_values,
+                batch_adv_preds,
                 batch_returns,
                 batch_terminateds,
                 batch_truncateds,
                 batch_old_log_probs,
                 adv_targ,
             )
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/auto_augment.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/auto_augment.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/elastic_transform.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/elastic_transform.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/gaussian_noise.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/grayscale.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/grayscale.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_adjustsharpness.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_adjustsharpness.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_amplitude_scaling.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_amplitude_scaling.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_augment.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_augment.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_autocontrast.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_autocontrast.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_colorjitter.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_colorjitter.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_convolution.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_convolution.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_crop.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_crop.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,11 +27,11 @@
         x = F.pad(x, padding, "replicate")
 
         crop_max = x.size()[2] - self._out + 1
         new_w = th.randint(0, crop_max, (n,))
         new_h = th.randint(0, crop_max, (n,))
         cropped = th.empty(size=(n, c, self._out, self._out))
 
-        for idx, (img, new_h, new_w) in enumerate(zip(x, new_h, new_w)):
-            cropped[idx] = img[:, new_h : new_h + self._out, new_w : new_w + self._out]
+        for idx, (img, t_h, t_w) in enumerate(zip(x, new_h, new_w)):
+            cropped[idx] = img[:, t_h : t_h + self._out, t_w : t_w + self._out]
 
         return cropped
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_cutout.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_cutout.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_cutoutcolor.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_cutoutcolor.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_equalize.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_equalize.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_flip.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_flip.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_invert.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_invert.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_perspective.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_perspective.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_rotate.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_rotate.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_shift.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_shift.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_translate.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/augmentation/random_translate.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from .base import BaseDistribution as BaseDistribution
+from .bernoulli import Bernoulli as Bernoulli
 from .categorical import Categorical as Categorical
 from .diagonal_gaussian import DiagonalGaussian as DiagonalGaussian
 from .kl import kl_categorical_categorical as kl_categorical_categorical
+from .kl import kl_diagonal_gaussian_diagonal_gaussian as kl_diagonal_gaussian_diagonal_gaussian
 from .normal_noise import NormalNoise as NormalNoise
 from .ornstein_uhlenbeck_noise import OrnsteinUhlenbeckNoise as OrnsteinUhlenbeckNoise
 from .squashed_normal import SquashedNormal as SquashedNormal
 from .truncated_normal_noise import TruncatedNormalNoise as TruncatedNormalNoise
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/base.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,7 +56,15 @@
     @abstractmethod
     def mean(self) -> th.Tensor:
         """Returns the mean of the distribution."""
 
     @abstractmethod
     def mode(self) -> th.Tensor:
         """Returns the mode of the distribution."""
+
+    @abstractmethod
+    def stddev(self) -> th.Tensor:
+        """Returns the standard deviation of the distribution."""
+
+    @abstractmethod
+    def variance(self) -> th.Tensor:
+        """Returns the variance of the distribution."""
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/categorical.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/categorical.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,85 @@
 import torch as th
 import torch.distributions as pyd
 
 from hsuanwu.xplore.distribution import BaseDistribution
 
 
 class Categorical(BaseDistribution):
-    """Categorical distribution for sampling actions in discrete control tasks.
+    """Categorical distribution for sampling actions for 'Discrete' tasks.
     Args:
         logits (Tensor): The event log probabilities (unnormalized).
 
     Returns:
         Categorical distribution instance.
     """
 
     def __init__(
         self,
         logits: th.Tensor,
     ) -> None:
         super().__init__()
-        self._logits = logits
         self.dist = pyd.Categorical(logits=logits)
 
     @property
     def probs(self) -> th.Tensor:
         """Return probabilities."""
         return self.dist.probs
 
     @property
     def logits(self) -> th.Tensor:
         """Returns the unnormalized log probabilities."""
         return self.dist.logits
 
     def sample(self, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
         """Generates a sample_shape shaped sample or sample_shape shaped batch of
-        samples if the distribution parameters are batched.
+            samples if the distribution parameters are batched.
 
         Args:
             sample_shape (TorchSize): The size of the sample to be drawn.
 
         Returns:
             A sample_shape shaped sample.
         """
-        return self.dist.sample().unsqueeze(-1)
+        return self.dist.sample()
 
     def log_prob(self, actions: th.Tensor) -> th.Tensor:
-        """Returns the log of the probability density/mass function evaluated at `value`.
+        """Returns the log of the probability density/mass function evaluated at actions.
 
         Args:
             actions (Tensor): The actions to be evaluated.
 
         Returns:
             The log_prob value.
         """
-        return self.dist.log_prob(actions.squeeze(-1)).view(actions.size(0), -1).sum(-1).unsqueeze(-1)
+        return self.dist.log_prob(actions)
 
     def entropy(self) -> th.Tensor:
         """Returns the Shannon entropy of distribution."""
         return self.dist.entropy()
 
     @property
     def mode(self) -> th.Tensor:
         """Returns the mode of the distribution."""
-        return self.dist.probs.argmax(dim=-1, keepdim=True)
+        return self.dist.mode
 
     @property
     def mean(self) -> th.Tensor:
         """Returns the mean of the distribution."""
-        return self.dist.probs.argmax(dim=-1, keepdim=True)
+        return self.dist.mode
+
+    @property
+    def stddev(self) -> th.Tensor:
+        """Returns the standard deviation of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement stddev!")
+
+    @property
+    def variance(self) -> th.Tensor:
+        """Returns the variance of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement variance!")
 
     def reset(self) -> None:
         """Reset the distribution."""
-        raise NotImplementedError
+        raise NotImplementedError(f"{self.__class__} does not implement reset!")
 
     def rsample(self, sample_shape: th.Size = ...) -> th.Tensor:  # B008
-        raise NotImplementedError
+        raise NotImplementedError(f"{self.__class__} does not implement rsample!")
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/diagonal_gaussian.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/diagonal_gaussian.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from hsuanwu.xplore.distribution.base import BaseDistribution
 
 
 class DiagonalGaussian(BaseDistribution):
     """Diagonal Gaussian distribution for 'Box' tasks.
 
     Args:
-        mu (Tensor): The mean of the distribution (often referred to as mu).
-        sigma (Tensor): The standard deviation of the distribution (often referred to as sigma).
+        loc (Tensor): The mean of the distribution (often referred to as mu).
+        scale (Tensor): The standard deviation of the distribution (often referred to as sigma).
 
     Returns:
         Squashed normal distribution instance.
     """
 
-    def __init__(self, mu: th.Tensor, sigma: th.Tensor) -> None:
+    def __init__(self, loc: th.Tensor, scale: th.Tensor) -> None:
         super().__init__()
 
-        self._mu = mu
-        self._sigma = sigma
-        self.dist = pyd.Normal(loc=mu, scale=sigma)
+        self.loc = loc
+        self.scale = scale
+        self.dist = pyd.Normal(loc=loc, scale=scale)
 
     def sample(self, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
         """Generates a sample_shape shaped sample or sample_shape shaped batch of
             samples if the distribution parameters are batched.
 
         Args:
             sample_shape (Size): The size of the sample to be drawn.
@@ -44,32 +44,43 @@
         Returns:
             A sample_shape shaped sample.
         """
         return self.dist.rsample(sample_shape)
 
     @property
     def mean(self) -> th.Tensor:
-        """Return the transformed mean."""
-        return self._mu
+        """Returns the mean of the distribution."""
+        return self.loc
+
+    @property
+    def mode(self) -> th.Tensor:
+        """Returns the mode of the distribution."""
+        return self.loc
+
+    @property
+    def stddev(self) -> th.Tensor:
+        """Returns the standard deviation of the distribution."""
+        raise self.scale
+
+    @property
+    def variance(self) -> th.Tensor:
+        """Returns the variance of the distribution."""
+        return self.stddev.pow(2)
 
     def log_prob(self, actions: th.Tensor) -> th.Tensor:
-        """Scores the sample by inverting the transform(s) and computing the score using the
-            score of the base distribution and the log abs det jacobian.
+        """Returns the log of the probability density/mass function evaluated at actions.
+
         Args:
             actions (Tensor): The actions to be evaluated.
 
         Returns:
             The log_prob value.
         """
-        return self.dist.log_prob(actions)
+        return self.dist.log_prob(actions).sum(-1)
 
     def reset(self) -> None:
         """Reset the distribution."""
-        raise NotImplementedError
+        raise NotImplementedError(f"{self.__class__} does not implement reset!")
 
     def entropy(self) -> th.Tensor:
         """Returns the Shannon entropy of distribution."""
         return self.dist.entropy()
-
-    def mode(self) -> th.Tensor:
-        """Returns the mode of the distribution."""
-        raise NotImplementedError
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/normal_noise.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/bernoulli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,85 @@
 import torch as th
 import torch.distributions as pyd
 
-from hsuanwu.xplore.distribution import utils
-from hsuanwu.xplore.distribution.base import BaseDistribution
+from hsuanwu.xplore.distribution import BaseDistribution
 
 
-class NormalNoise(BaseDistribution):
-    """Gaussian action noise.
-
+class Bernoulli(BaseDistribution):
+    """Bernoulli distribution for sampling actions for 'MultiBinary' tasks.
     Args:
-        mu (float): mean of the noise (often referred to as mu).
-        sigma (float): standard deviation of the noise (often referred to as sigma).
-        stddev_schedule (str): Use the exploration std schedule.
+        logits (Tensor): The event log probabilities (unnormalized).
 
     Returns:
-        Gaussian action noise instance.
+        Categorical distribution instance.
     """
 
     def __init__(
         self,
-        mu: float = 0.0,
-        sigma: float = 1.0,
-        stddev_schedule: str = "linear(1.0, 0.1, 100000)",
-        stddev_clip: float = 0.3,
+        logits: th.Tensor,
     ) -> None:
         super().__init__()
+        self.dist = pyd.Bernoulli(logits=logits)
 
-        self.dist = pyd.Normal(loc=mu, scale=sigma)
-        self._noiseless_action = None
-        self._stddev_schedule = stddev_schedule
-
-    def sample(self, clip: bool = False, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
-        """Generates a sample_shape shaped sample or sample_shape shaped batch of
-            samples if the distribution parameters are batched.
-
-        Args:
-            clip (bool): Whether to perform noise truncation.
-            sample_shape (Size): The size of the sample to be drawn.
-
-        Returns:
-            A sample_shape shaped sample.
-        """
-        noise = th.as_tensor(
-            self.dist.sample(sample_shape=self._noiseless_action.size()),
-            device=self._noiseless_action.device,
-            dtype=self._noiseless_action.dtype,
-        )
+    @property
+    def probs(self) -> th.Tensor:
+        """Return probabilities."""
+        return self.dist.probs
 
-        return noise + self._noiseless_action
+    @property
+    def logits(self) -> th.Tensor:
+        """Returns the unnormalized log probabilities."""
+        return self.dist.logits
 
-    def rsample(self, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
+    def sample(self, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
         """Generates a sample_shape shaped sample or sample_shape shaped batch of
             samples if the distribution parameters are batched.
 
         Args:
-            sample_shape (Size): The size of the sample to be drawn.
+            sample_shape (TorchSize): The size of the sample to be drawn.
 
         Returns:
             A sample_shape shaped sample.
         """
-        raise NotImplementedError
+        return self.dist.sample()
 
-    def log_prob(self, value: th.Tensor) -> th.Tensor:
-        """Returns the log of the probability density/mass function evaluated at `value`.
+    def log_prob(self, actions: th.Tensor) -> th.Tensor:
+        """Returns the log of the probability density/mass function evaluated at actions.
 
         Args:
-            value (Tensor): The value to be evaluated.
+            actions (Tensor): The actions to be evaluated.
 
         Returns:
             The log_prob value.
         """
-        raise NotImplementedError
+        return self.dist.log_prob(actions).sum(-1)
 
     def entropy(self) -> th.Tensor:
         """Returns the Shannon entropy of distribution."""
-        raise NotImplementedError
-
-    def reset(self, noiseless_action: th.Tensor, step: int = 0) -> None:
-        """Reset the noise instance.
+        return self.dist.entropy().sum(-1)
 
-        Args:
-            noiseless_action (Tensor): Unprocessed actions.
-            step (int): Global training step that can be None when there is no noise schedule.
-
-        Returns:
-            None.
-        """
-        self._noiseless_action = noiseless_action
-        if self._stddev_schedule is not None:
-            # TODO: reset the std of normal distribution.
-            self.dist.scale = th.ones_like(self.dist.scale) * utils.schedule(self._stddev_schedule, step)
+    @property
+    def mode(self) -> th.Tensor:
+        """Returns the mode of the distribution."""
+        return th.gt(self.dist.probs, 0.5).float()
 
     @property
     def mean(self) -> th.Tensor:
         """Returns the mean of the distribution."""
-        return self._noiseless_action
+        return th.gt(self.dist.probs, 0.5).float()
 
     @property
-    def mode(self) -> th.Tensor:
-        """Returns the mode of the distribution."""
-        return self._noiseless_action
+    def stddev(self) -> th.Tensor:
+        """Returns the standard deviation of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement stddev!")
+
+    @property
+    def variance(self) -> th.Tensor:
+        """Returns the variance of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement variance!")
+
+    def reset(self) -> None:
+        """Reset the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement reset!")
+
+    def rsample(self, sample_shape: th.Size = ...) -> th.Tensor:  # B008
+        raise NotImplementedError(f"{self.__class__} does not implement rsample!")
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,118 +7,128 @@
 
 
 class OrnsteinUhlenbeckNoise(BaseDistribution):
     """Ornstein Uhlenbeck action noise.
         Based on http://math.stackexchange.com/questions/1287634/implementing-ornstein-uhlenbeck-in-matlab
 
     Args:
-        mu (float): mean of the noise (often referred to as mu).
-        sigma (float): standard deviation of the noise (often referred to as sigma).
+        loc (float): mean of the noise (often referred to as mu).
+        scale (float): standard deviation of the noise (often referred to as sigma).
         theta (float): Rate of mean reversion.
         dt (float): Timestep for the noise.
 
     Returns:
         Ornstein-Uhlenbeck noise instance.
     """
 
     def __init__(
         self,
-        mu: float = 0.0,
-        sigma: float = 1.0,
+        loc: float = 0.0,
+        scale: float = 1.0,
         theta: float = 0.15,
         dt: float = 1e-2,
         stddev_schedule: str = "linear(1.0, 0.1, 100000)",
     ) -> None:
         super().__init__()
 
-        self._mu = mu
-        self._sigma = sigma
+        self.loc = loc
+        self.scale = scale
         self._theta = theta
-        self._dt = dt
-        self._noiseless_action = None
-        self._stddev_schedule = stddev_schedule
+        self.dt = dt
+        self.noiseless_action = None
+        self.stddev_schedule = stddev_schedule
 
         self.noise_prev = None
 
     def reset(self, noiseless_action: th.Tensor, step: int = 0) -> None:
         """Reset the noise instance.
 
         Args:
             noiseless_action (Tensor): Unprocessed actions.
             step (int): Global training step that can be None when there is no noise schedule.
 
         Returns:
             None.
         """
-        self._noiseless_action = noiseless_action
+        self.noiseless_action = noiseless_action
         if self.noise_prev is None:
-            self.noise_prev = th.zeros_like(self._noiseless_action)
-        if self._stddev_schedule is not None:
+            self.noise_prev = th.zeros_like(self.noiseless_action)
+        if self.stddev_schedule is not None:
             # TODO: reset the std of
-            self._sigma = utils.schedule(self._stddev_schedule, step)
+            self.scale = utils.schedule(self.stddev_schedule, step)
 
     def sample(self, clip: bool = False, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
         """Generates a sample_shape shaped sample
 
         Args:
             clip (bool): Range for noise truncation operation.
             sample_shape (Size): The size of the sample to be drawn.
 
         Returns:
             A sample_shape shaped sample.
         """
         noise = (
             self.noise_prev
-            + self._theta * (self._mu - self.noise_prev) * self._dt
-            + self._sigma
-            * np.sqrt(self._dt)
+            + self._theta * (self.loc - self.noise_prev) * self.dt
+            + self.scale
+            * np.sqrt(self.dt)
             * _standard_normal(
-                self._noiseless_action.size(),
-                dtype=self._noiseless_action.dtype,
-                device=self._noiseless_action.device,
+                self.noiseless_action.size(),
+                dtype=self.noiseless_action.dtype,
+                device=self.noiseless_action.device,
             )
         )
         noise = th.as_tensor(
             noise,
-            dtype=self._noiseless_action.dtype,
-            device=self._noiseless_action.device,
+            dtype=self.noiseless_action.dtype,
+            device=self.noiseless_action.device,
         )
         self.noise_prev = noise
 
-        return noise + self._noiseless_action
+        return noise + self.noiseless_action
 
     @property
     def mean(self) -> th.Tensor:
         """Returns the mean of the distribution."""
-        return self._noiseless_action
+        return self.noiseless_action
 
     @property
     def mode(self) -> th.Tensor:
         """Returns the mode of the distribution."""
-        return self._noiseless_action
+        return self.noiseless_action
 
     def rsample(self, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
         """Generates a sample_shape shaped sample or sample_shape shaped batch of
             samples if the distribution parameters are batched.
 
         Args:
             sample_shape (Size): The size of the sample to be drawn.
 
         Returns:
             A sample_shape shaped sample.
         """
-        raise NotImplementedError
+        raise NotImplementedError(f"{self.__class__} does not implement rsample!")
 
     def log_prob(self, value: th.Tensor) -> th.Tensor:
         """Returns the log of the probability density/mass function evaluated at `value`.
 
         Args:
             value (Tensor): The value to be evaluated.
 
         Returns:
             The log_prob value.
         """
-        raise NotImplementedError
+        raise NotImplementedError(f"{self.__class__} does not implement log_prob!")
 
     def entropy(self) -> th.Tensor:
         """Returns the Shannon entropy of distribution."""
-        raise NotImplementedError
+        raise NotImplementedError(f"{self.__class__} does not implement entropy!")
+
+    @property
+    def stddev(self) -> th.Tensor:
+        """Returns the standard deviation of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement stddev!")
+
+    @property
+    def variance(self) -> th.Tensor:
+        """Returns the variance of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement variance!")
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/squashed_normal.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/squashed_normal.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,28 +36,28 @@
         return 2.0 * (math.log(2.0) - x - F.softplus(-2.0 * x))
 
 
 class SquashedNormal(BaseDistribution):
     """Squashed normal distribution for Soft Actor-Critic learner.
 
     Args:
-        mu (Tensor): The mean of the distribution (often referred to as mu).
-        sigma (Tensor): The standard deviation of the distribution (often referred to as sigma).
+        loc (Tensor): The mean of the distribution (often referred to as mu).
+        scale (Tensor): The standard deviation of the distribution (often referred to as sigma).
 
     Returns:
         Squashed normal distribution instance.
     """
 
-    def __init__(self, mu: th.Tensor, sigma: th.Tensor) -> None:
+    def __init__(self, loc: th.Tensor, scale: th.Tensor) -> None:
         super().__init__()
 
-        self._mu = mu
-        self._sigma = sigma
+        self.loc = loc
+        self.scale = scale
         self.dist = pyd.TransformedDistribution(
-            base_distribution=pyd.Normal(loc=mu, scale=sigma),
+            base_distribution=pyd.Normal(loc=loc, scale=scale),
             transforms=[TanhTransform()],
         )
 
     def sample(self, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
         """Generates a sample_shape shaped sample or sample_shape shaped
             batch of samples if the distribution parameters are batched.
 
@@ -80,34 +80,45 @@
             A sample_shape shaped sample.
         """
         return self.dist.rsample(sample_shape)
 
     @property
     def mean(self) -> th.Tensor:
         """Return the transformed mean."""
-        mu = self._mu
+        loc = self.loc
         for tr in self.dist.transforms:
-            mu = tr(mu)
-        return mu
+            loc = tr(loc)
+        return loc
+
+    @property
+    def mode(self) -> th.Tensor:
+        """Returns the mode of the distribution."""
+        return self.mean
 
     def log_prob(self, actions: th.Tensor) -> th.Tensor:
         """Scores the sample by inverting the transform(s) and computing the score using
             the score of the base distribution and the log abs det jacobian.
         Args:
             actions (Tensor): The actions to be evaluated.
 
         Returns:
             The log_prob value.
         """
         return self.dist.log_prob(actions)
 
-    def reset(self) -> None:
-        """Reset the distribution."""
-        raise NotImplementedError
-
     def entropy(self) -> th.Tensor:
         """Returns the Shannon entropy of distribution."""
-        raise NotImplementedError
+        raise NotImplementedError(f"{self.__class__} does not implement entropy!")
 
-    def mode(self) -> th.Tensor:
-        """Returns the mode of the distribution."""
-        raise NotImplementedError
+    @property
+    def stddev(self) -> th.Tensor:
+        """Returns the standard deviation of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement stddev!")
+
+    @property
+    def variance(self) -> th.Tensor:
+        """Returns the variance of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement variance!")
+
+    def reset(self) -> None:
+        """Reset the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement reset!")
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/truncated_normal_noise.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/truncated_normal_noise.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,104 +6,114 @@
 
 
 class TruncatedNormalNoise(BaseDistribution):
     """Truncated normal action noise. See Section 3.1 of
         "Mastering Visual Continuous Control: Improved Data-Augmented Reinforcement Learning".
 
     Args:
-        mu (float): mean of the noise (often referred to as mu).
-        sigma (float): standard deviation of the noise (often referred to as sigma).
+        loc (float): mean of the noise (often referred to as mu).
+        scale (float): standard deviation of the noise (often referred to as sigma).
         stddev_schedule (str): Use the exploration std schedule.
         stddev_clip (float): The exploration std clip range.
 
     Returns:
         Truncated normal noise instance.
     """
 
     def __init__(
         self,
-        mu: float = 0.0,
-        sigma: float = 1.0,
+        loc: float = 0.0,
+        scale: float = 1.0,
         stddev_schedule: str = "linear(1.0, 0.1, 100000)",
         stddev_clip: float = 0.3,
     ) -> None:
         super().__init__()
 
-        self._mu = mu
-        self._sigma = sigma
-        self.dist = pyd.Normal(loc=mu, scale=sigma)
-        self._noiseless_action = None
-        self._stddev_schedule = stddev_schedule
-        self._stddev_clip = stddev_clip
+        self.loc = loc
+        self.scale = scale
+        self.dist = pyd.Normal(loc=loc, scale=scale)
+        self.noiseless_action = None
+        self.stddev_schedule = stddev_schedule
+        self.stddev_clip = stddev_clip
 
     def sample(self, clip: bool = False, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
         """Generates a sample_shape shaped sample or sample_shape shaped batch of
             samples if the distribution parameters are batched.
 
         Args:
             clip (bool): Whether to perform noise truncation.
             sample_shape (Size): The size of the sample to be drawn.
 
         Returns:
             A sample_shape shaped sample.
         """
         noise = th.as_tensor(
-            self.dist.sample(sample_shape=self._noiseless_action.size()),
-            device=self._noiseless_action.device,
-            dtype=self._noiseless_action.dtype,
+            self.dist.sample(sample_shape=self.noiseless_action.size()),
+            device=self.noiseless_action.device,
+            dtype=self.noiseless_action.dtype,
         )
         if clip:
             # clip the sampled noises
-            noise = th.clamp(noise, -self._stddev_clip, self._stddev_clip)
-        return noise + self._noiseless_action
+            noise = th.clamp(noise, -self.stddev_clip, self.stddev_clip)
+        return noise + self.noiseless_action
 
     def rsample(self, sample_shape: th.Size = th.Size()) -> th.Tensor:  # noqa B008
         """Generates a sample_shape shaped sample or sample_shape shaped batch of
             samples if the distribution parameters are batched.
 
         Args:
             sample_shape (Size): The size of the sample to be drawn.
 
         Returns:
             A sample_shape shaped sample.
         """
-        raise NotImplementedError
+        raise NotImplementedError(f"{self.__class__} does not implement rsample!")
 
     def log_prob(self, value: th.Tensor) -> th.Tensor:
         """Returns the log of the probability density/mass function evaluated at `value`.
 
         Args:
             value (Tensor): The value to be evaluated.
 
         Returns:
             The log_prob value.
         """
-        raise NotImplementedError
-
-    def entropy(self) -> th.Tensor:
-        """Returns the Shannon entropy of distribution."""
-        raise NotImplementedError
+        raise NotImplementedError(f"{self.__class__} does not implement log_prob!")
 
     def reset(self, noiseless_action: th.Tensor, step: int = 0) -> None:
         """Reset the noise instance.
 
         Args:
             noiseless_action (Tensor): Unprocessed actions.
             step (int): Global training step that can be None when there is no noise schedule.
 
         Returns:
             None.
         """
-        self._noiseless_action = noiseless_action
-        if self._stddev_schedule is not None:
+        self.noiseless_action = noiseless_action
+        if self.stddev_schedule is not None:
             # TODO: reset the std of normal distribution.
-            self.dist.scale = th.ones_like(self.dist.scale) * utils.schedule(self._stddev_schedule, step)
+            self.dist.scale = th.ones_like(self.dist.scale) * utils.schedule(self.stddev_schedule, step)
 
     @property
     def mean(self) -> th.Tensor:
         """Returns the mean of the distribution."""
-        return self._noiseless_action
+        return self.noiseless_action
 
     @property
     def mode(self) -> th.Tensor:
         """Returns the mode of the distribution."""
-        return self._noiseless_action
+        return self.noiseless_action
+
+    def entropy(self) -> th.Tensor:
+        """Returns the Shannon entropy of distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement entropy!")
+
+    @property
+    def stddev(self) -> th.Tensor:
+        """Returns the standard deviation of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement stddev!")
+
+    @property
+    def variance(self) -> th.Tensor:
+        """Returns the variance of the distribution."""
+        raise NotImplementedError(f"{self.__class__} does not implement variance!")
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/utils.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/distribution/utils.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/__init__.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/base.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,20 +31,22 @@
         device: str = "cpu",
         beta: float = 0.05,
         kappa: float = 0.000025,
     ) -> None:
         if isinstance(observation_space, gym.Space) and isinstance(action_space, gym.Space):
             self._obs_shape = observation_space.shape
             if action_space.__class__.__name__ == "Discrete":
-                self._action_shape = (int(action_space.n),)  # type: ignore[attr-defined]
+                self._action_shape = (int(action_space.n),)
                 self._action_type = "Discrete"
-
             elif action_space.__class__.__name__ == "Box":
-                self._action_shape = action_space.shape  # type: ignore[attr-defined, assignment]
+                self._action_shape = action_space.shape
                 self._action_type = "Box"
+            elif action_space.__class__.__name__ == "MultiBinary":
+                self._action_shape = action_space.shape
+                self._action_type = "MultiBinary"
             else:
                 raise NotImplementedError("Unsupported action type!")
         elif isinstance(observation_space, DictConfig) and isinstance(action_space, DictConfig):
             # by DictConfig
             self._obs_shape = observation_space.shape
             self._action_shape = action_space.shape
             self._action_type = action_space.type
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/girm.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/girm.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         # compute the weighting coefficient of timestep t
         beta_t = self._beta * np.power(1.0 - self._kappa, step)
         num_steps = samples["obs"].size()[0]
         num_envs = samples["obs"].size()[1]
         obs_tensor = samples["obs"].to(self._device)
         actions_tensor = samples["actions"].to(self._device)
         if self._action_type == "Discrete":
-            actions_tensor = F.one_hot(actions_tensor[:, :, 0].long(), self._action_shape[0]).float()
+            actions_tensor = F.one_hot(actions_tensor.long(), self._action_shape[0]).float()
             actions_tensor = actions_tensor.to(self._device)
         next_obs_tensor = samples["next_obs"].to(self._device)
         intrinsic_rewards = th.zeros(size=(num_steps, num_envs)).to(self._device)
 
         with th.no_grad():
             for i in range(num_envs):
                 latent = self.vae.encoder(obs_tensor[:, i], next_obs_tensor[:, i])
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/icm.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/icm.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         beta (float): The initial weighting coefficient of the intrinsic rewards.
         kappa (float): The decay rate.
         latent_dim (int): The dimension of encoding vectors.
         lr (float): The learning rate.
         batch_size (int): The batch size for update.
 
     Returns:
-        Instance of RND.
+        Instance of ICM.
     """
 
     def __init__(
         self,
         observation_space: Union[gym.Space, DictConfig],
         action_space: Union[gym.Space, DictConfig],
         device: str = "cpu",
@@ -190,15 +190,15 @@
         # compute the weighting coefficient of timestep t
         beta_t = self._beta * np.power(1.0 - self._kappa, step)
         num_steps = samples["obs"].size()[0]
         num_envs = samples["obs"].size()[1]
         obs_tensor = samples["obs"].to(self._device)
         actions_tensor = samples["actions"].to(self._device)
         if self._action_type == "Discrete":
-            actions_tensor = F.one_hot(actions_tensor[:, :, 0].long(), self._action_shape[0]).float()
+            actions_tensor = F.one_hot(actions_tensor.long(), self._action_shape[0]).float()
         next_obs_tensor = samples["next_obs"].to(self._device)
 
         intrinsic_rewards = th.zeros(size=(num_steps, num_envs))
 
         with th.no_grad():
             for i in range(num_envs):
                 encoded_obs = self.encoder(obs_tensor[:, i])
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/ngu.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/ngu.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         kernel_cluster_distance (float): The kernel cluster distance.
         kernel_epsilon (float): The kernel constant.
         c (float): The pseudo-counts constant.
         sm (float): The kernel maximum similarity.
         mrs (float): The maximum reward scaling.
 
     Returns:
-        Instance of the base intrinsic reward module.
+        Instance of NGU.
     """
 
     def __init__(
         self,
         observation_space: Union[gym.Space, DictConfig],
         action_space: Union[gym.Space, DictConfig],
         device: str = "cpu",
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/pseudo_counts.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/pseudo_counts.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         k (int): Number of neighbors.
         kernel_cluster_distance (float): The kernel cluster distance.
         kernel_epsilon (float): The kernel constant.
         c (float): The pseudo-counts constant.
         sm (float): The kernel maximum similarity.
 
     Returns:
-        Instance of the base intrinsic reward module.
+        Instance of PseudoCounts.
     """
 
     def __init__(
         self,
         observation_space: Union[gym.Space, DictConfig],
         action_space: Union[gym.Space, DictConfig],
         device: str = "cpu",
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/re3.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/re3.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         beta (float): The initial weighting coefficient of the intrinsic rewards.
         kappa (float): The decay rate.
         latent_dim (int): The dimension of encoding vectors.
         k (int): Use the k-th neighbors.
         average_entropy (bool): Use the average of entropy estimation.
 
     Returns:
-        Instance of RND.
+        Instance of RE3.
     """
 
     def __init__(
         self,
         observation_space: Union[gym.Space, DictConfig],
         action_space: Union[gym.Space, DictConfig],
         device: str = "cpu",
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/revd.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/revd.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/rise.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/rise.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         kappa (float): The decay rate.
         latent_dim (int): The dimension of encoding vectors.
         alpha (alpha): The The order of Rényi entropy.
         k (int): Use the k-th neighbors.
         average_entropy (bool): Use the average of entropy estimation.
 
     Returns:
-        Instance of RND.
+        Instance of RISE.
     """
 
     def __init__(
         self,
         observation_space: Union[gym.Space, DictConfig],
         action_space: Union[gym.Space, DictConfig],
         device: str = "cpu",
```

### Comparing `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/rnd.py` & `hsuanwu-0.0.1b5/hsuanwu/xplore/reward/rnd.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/tests/test_aug.py` & `hsuanwu-0.0.1b5/tests/test_aug.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/tests/test_dist.py` & `hsuanwu-0.0.1b5/tests/test_dist.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     SquashedNormal,
     TruncatedNormalNoise,
 )
 
 if __name__ == "__main__":
     device = torch.device("cuda:0")
 
-    dist = SquashedNormal(mu=torch.rand(1, 17), sigma=torch.rand(1, 17))
+    dist = SquashedNormal(loc=torch.rand(1, 17), scale=torch.rand(1, 17))
 
     print(dist.sample())
     print(dist.rsample())
     print(dist.log_prob(actions=torch.rand(1, 17)))
 
     dist = Categorical(logits=torch.randn(1, 7))
     print(dist.sample())
```

### Comparing `hsuanwu-0.0.1b4/tests/test_env.py` & `hsuanwu-0.0.1b5/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/tests/test_eval.py` & `hsuanwu-0.0.1b5/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/tests/test_logger.py` & `hsuanwu-0.0.1b5/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/tests/test_mp.py` & `hsuanwu-0.0.1b5/tests/test_mp.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/tests/test_reward.py` & `hsuanwu-0.0.1b5/tests/test_reward.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/tests/test_torch.py` & `hsuanwu-0.0.1b5/tests/test_torch.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/LICENSE` & `hsuanwu-0.0.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b4/README.md` & `hsuanwu-0.0.1b5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,778 +1,891 @@
-00000000: 3c64 6976 2061 6c69 676e 3d63 656e 7465  <div align=cente
-00000010: 723e 0d0a 3c69 6d67 2073 7263 3d27 2e2f  r>..<img src='./
-00000020: 646f 6373 2f61 7373 6574 732f 696d 6167  docs/assets/imag
-00000030: 6573 2f6c 6f67 6f2e 706e 6727 2073 7479  es/logo.png' sty
-00000040: 6c65 3d22 7769 6474 683a 2037 3025 223e  le="width: 70%">
-00000050: 0d0a 3c2f 6469 763e 0d0a 0d0a 7c3c 696d  ..</div>....|<im
-00000060: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000070: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000080: 6467 652f 4c69 6365 6e73 652d 4d49 542d  dge/License-MIT-
-00000090: 2532 3330 3637 3762 3822 3e20 3c69 6d67  %230677b8"> <img
-000000a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-000000b0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000000c0: 6765 2f47 5055 2d4e 5649 4449 412d 2532  ge/GPU-NVIDIA-%2
-000000d0: 3337 3762 3930 3022 3e20 3c69 6d67 2073  377b900"> <img s
-000000e0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-000000f0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000100: 2f4e 5055 2d41 7363 656e 642d 2532 3363  /NPU-Ascend-%23c
-00000110: 3331 6432 3022 3e20 3c69 6d67 2073 7263  31d20"> <img src
-00000120: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000130: 6965 6c64 732e 696f 2f62 6164 6765 2f50  ields.io/badge/P
-00000140: 7974 686f 6e2d 2533 4525 3344 332e 382d  ython-%3E%3D3.8-
-00000150: 2532 3333 3537 3039 4622 3e20 3c69 6d67  %2335709F"> <img
-00000160: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000170: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000180: 6765 2f44 6f63 732d 5061 7373 696e 672d  ge/Docs-Passing-
-00000190: 2532 3330 3039 3438 3522 3e20 3c69 6d67  %23009485"> <img
-000001a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-000001b0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000001c0: 6765 2f43 6f64 6573 7479 6c65 2d42 6c61  ge/Codestyle-Bla
-000001d0: 636b 2d62 6c61 636b 223e 203c 696d 6720  ck-black"> <img 
-000001e0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000001f0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000200: 652f 5079 5049 2532 3050 6163 6b61 6765  e/PyPI%20Package
-00000210: 2d30 2e30 2e31 2d25 3233 3030 3644 4144  -0.0.1-%23006DAD
-00000220: 223e 203c 696d 6720 7372 633d 2268 7474  "> <img src="htt
-00000230: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000240: 2e69 6f2f 6261 6467 652f f09f a497 4265  .io/badge/....Be
-00000250: 6e63 686d 6172 6b2d 4875 6767 696e 6746  nchmark-HuggingF
-00000260: 6163 652d 2532 3346 4644 3231 4522 3e20  ace-%23FFD21E"> 
-00000270: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000280: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000290: 2f62 6164 6765 2f50 7974 6f72 6368 2d25  /badge/Pytorch-%
-000002a0: 3345 2533 4432 2e30 2e30 2d25 3233 4546  3E%3D2.0.0-%23EF
-000002b0: 3537 3339 223e 203c 696d 6720 7372 633d  5739"> <img src=
-000002c0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000002d0: 656c 6473 2e69 6f2f 6261 6467 652f 4879  elds.io/badge/Hy
-000002e0: 6472 612d 312e 332e 322d 2532 3345 3838  dra-1.3.2-%23E88
-000002f0: 3434 3422 3e20 3c69 6d67 2073 7263 3d22  444"> <img src="
-00000300: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000310: 6c64 732e 696f 2f62 6164 6765 2f47 796d  lds.io/badge/Gym
-00000320: 6e61 7369 756d 2d25 3345 2533 4430 2e32  nasium-%3E%3D0.2
-00000330: 382e 312d 6272 6967 6874 6772 6565 6e22  8.1-brightgreen"
-00000340: 3e20 3c69 6d67 2073 7263 3d22 6874 7470  > <img src="http
-00000350: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000360: 696f 2f62 6164 6765 2f44 4d43 2053 7569  io/badge/DMC Sui
-00000370: 7465 2d31 2e30 2e31 312d 626c 7565 223e  te-1.0.11-blue">
-00000380: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000390: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000003a0: 6f2f 6261 6467 652f 5072 6f63 6765 6e2d  o/badge/Procgen-
-000003b0: 302e 3130 2e37 2d62 6c75 6576 696f 6c65  0.10.7-blueviole
-000003c0: 7422 3e20 3c69 6d67 2073 7263 3d22 6874  t"> <img src="ht
-000003d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000003e0: 732e 696f 2f62 6164 6765 2f32 2e32 2e31  s.io/badge/2.2.1
-000003f0: 2d4d 696e 6947 7269 642d 2532 3363 3863  -MiniGrid-%23c8c
-00000400: 3863 3822 3e20 3c69 6d67 2073 7263 3d22  8c8"> <img src="
-00000410: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000420: 6c64 732e 696f 2f62 6164 6765 2f50 7942  lds.io/badge/PyB
-00000430: 756c 6c65 742d 332e 322e 352d 2532 3336  ullet-3.2.5-%236
-00000440: 4139 3444 3422 3e7c 0d0a 7c3a 2d3a 7c0d  A94D4">|..|:-:|.
-00000450: 0a0d 0a2a 2a48 7375 616e 7775 3a20 4c6f  ...**Hsuanwu: Lo
-00000460: 6e67 2d54 6572 6d20 4576 6f6c 7574 696f  ng-Term Evolutio
-00000470: 6e20 5072 6f6a 6563 7420 6f66 2052 6569  n Project of Rei
-00000480: 6e66 6f72 6365 6d65 6e74 204c 6561 726e  nforcement Learn
-00000490: 696e 672a 2a20 6973 2069 6e73 7069 7265  ing** is inspire
-000004a0: 6420 6279 2074 6865 206c 6f6e 672d 7465  d by the long-te
-000004b0: 726d 2065 766f 6c75 7469 6f6e 2028 4c54  rm evolution (LT
-000004c0: 4529 2073 7461 6e64 6172 6420 7072 6f6a  E) standard proj
-000004d0: 6563 7420 696e 2074 656c 6563 6f6d 6d75  ect in telecommu
-000004e0: 6e69 6361 7469 6f6e 732c 2077 6869 6368  nications, which
-000004f0: 2061 696d 7320 746f 2074 7261 636b 2074   aims to track t
-00000500: 6865 206c 6174 6573 7420 7265 7365 6172  he latest resear
-00000510: 6368 2070 726f 6772 6573 7320 696e 2072  ch progress in r
-00000520: 6569 6e66 6f72 6365 6d65 6e74 206c 6561  einforcement lea
-00000530: 726e 696e 6720 2852 4c29 2061 6e64 2070  rning (RL) and p
-00000540: 726f 7669 6465 2073 7461 626c 6520 616e  rovide stable an
-00000550: 6420 6566 6669 6369 656e 7420 6261 7365  d efficient base
-00000560: 6c69 6e65 732e 2049 6e20 4873 7561 6e77  lines. In Hsuanw
-00000570: 752c 2079 6f75 2063 616e 2066 696e 6420  u, you can find 
-00000580: 6576 6572 7974 6869 6e67 2079 6f75 206e  everything you n
-00000590: 6565 6420 696e 2052 4c2c 2073 7563 6820  eed in RL, such 
-000005a0: 6173 2074 7261 696e 696e 672c 2065 7661  as training, eva
-000005b0: 6c75 6174 696f 6e2c 2064 6570 6c6f 796d  luation, deploym
-000005c0: 656e 742c 2065 7463 2e20 5468 6520 6869  ent, etc. The hi
-000005d0: 6768 6c69 6768 7420 6665 6174 7572 6573  ghlight features
-000005e0: 206f 6620 4873 7561 6e77 753a 0d0a 0d0a   of Hsuanwu:....
-000005f0: 2d20 e28f b1ef b88f 204c 6174 6573 7420  - ...... Latest 
-00000600: 616c 676f 7269 7468 6d73 2061 6e64 2074  algorithms and t
-00000610: 7269 636b 733b 0d0a 2d20 f09f a7b1 2048  ricks;..- .... H
-00000620: 6967 686c 7920 6d6f 6475 6c61 7269 7a65  ighly modularize
-00000630: 6420 6465 7369 676e 2066 6f72 2063 6f6d  d design for com
-00000640: 706c 6574 6520 6465 636f 7570 6c69 6e67  plete decoupling
-00000650: 206f 6620 524c 2061 6c67 6f72 6974 686d   of RL algorithm
-00000660: 733b 0d0a 2d20 f09f 9a80 204f 7074 696d  s;..- .... Optim
-00000670: 697a 6564 2077 6f72 6b66 6c6f 7720 666f  ized workflow fo
-00000680: 7220 6675 6c6c 2068 6172 6477 6172 6520  r full hardware 
-00000690: 6163 6365 6c65 7261 7469 6f6e 3b0d 0a2d  acceleration;..-
-000006a0: 20e2 9a99 efb8 8f20 5375 7070 6f72 7420   ...... Support 
-000006b0: 666f 7220 6375 7374 6f6d 2065 6e76 6972  for custom envir
-000006c0: 6f6e 6d65 6e74 733b 0d0a 2d20 f09f 96a5  onments;..- ....
-000006d0: efb8 8f20 5375 7070 6f72 7420 666f 7220  ... Support for 
-000006e0: 6d75 6c74 6970 6c65 2063 6f6d 7075 7469  multiple computi
-000006f0: 6e67 2064 6576 6963 6573 206c 696b 6520  ng devices like 
-00000700: 4750 5520 616e 6420 4e50 553b 0d0a 2d20  GPU and NPU;..- 
-00000710: f09f 9ba0 efb8 8f20 5375 7070 6f72 7420  ....... Support 
-00000720: 666f 7220 524c 206d 6f64 656c 2065 6e67  for RL model eng
-00000730: 696e 6565 7269 6e67 2064 6570 6c6f 796d  ineering deploym
-00000740: 656e 7420 2854 656e 736f 7252 542c 2043  ent (TensorRT, C
-00000750: 414e 4e2c 202e 2e2e 293b 0d0a 2d20 f09f  ANN, ...);..- ..
-00000760: 92be 204c 6172 6765 206e 756d 6265 7220  .. Large number 
-00000770: 6f66 2072 6575 7361 626c 6520 6265 6368  of reusable bech
-00000780: 6d61 726b 7320 285b 5365 6520 4873 7561  marks ([See Hsua
-00000790: 6e77 7548 7562 5d28 6875 622e 6873 7561  nwuHub](hub.hsua
-000007a0: 6e77 752e 6465 7629 293b 0d0a 2d20 f09f  nwu.dev));..- ..
-000007b0: 938b 2045 6c65 6761 6e74 2065 7870 6572  .. Elegant exper
-000007c0: 696d 656e 7461 6c20 6d61 6e61 6765 6d65  imental manageme
-000007d0: 6e74 2070 6f77 6572 6564 2062 7920 5b48  nt powered by [H
-000007e0: 7964 7261 5d28 6874 7470 733a 2f2f 6879  ydra](https://hy
-000007f0: 6472 612e 6363 2f29 2e0d 0a0d 0a4a 6f69  dra.cc/).....Joi
-00000800: 6e20 7468 6520 6465 7665 6c6f 7065 7220  n the developer 
-00000810: 636f 6d6d 756e 6974 7920 666f 7220 6973  community for is
-00000820: 7375 6573 2061 6e64 2064 6973 6375 7373  sues and discuss
-00000830: 696f 6e73 3a0d 0a7c 536c 6163 6b7c 5151  ions:..|Slack|QQ
-00000840: 7c47 6974 4875 627c 0d0a 7c3a 2d3a 7c3a  |GitHub|..|:-:|:
-00000850: 2d3a 7c3a 2d3a 7c0d 0a7c 3c61 2068 7265  -:|:-:|..|<a hre
-00000860: 663d 2268 7474 7073 3a2f 2f61 7070 2e73  f="https://app.s
-00000870: 6c61 636b 2e63 6f6d 2f63 6c69 656e 742f  lack.com/client/
-00000880: 5430 3534 4a34 4e4a 5850 302f 4330 3534  T054J4NJXP0/C054
-00000890: 5437 3851 5a39 4122 3e3c 696d 6720 7372  T78QZ9A"><img sr
-000008a0: 633d 272e 2f64 6f63 732f 6173 7365 7473  c='./docs/assets
-000008b0: 2f69 6d61 6765 732f 736c 6163 6b2e 706e  /images/slack.pn
-000008c0: 6727 2073 7479 6c65 3d22 7769 6474 683a  g' style="width:
-000008d0: 2035 3025 2220 3e3c 2f61 3e7c 3c69 6d67   50%" ></a>|<img
-000008e0: 2073 7263 3d27 2e2f 646f 6373 2f61 7373   src='./docs/ass
-000008f0: 6574 732f 696d 6167 6573 2f71 712e 6a70  ets/images/qq.jp
-00000900: 6727 2073 7479 6c65 3d22 7769 6474 683a  g' style="width:
-00000910: 2036 3525 223e 7c3c 6120 6872 6566 3d22   65%">|<a href="
-00000920: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000930: 6f6d 2f52 4c45 2d46 6f75 6e64 6174 696f  om/RLE-Foundatio
-00000940: 6e2f 4873 7561 6e77 752f 6973 7375 6573  n/Hsuanwu/issues
-00000950: 223e 3c69 6d67 2073 7263 3d27 2e2f 646f  "><img src='./do
-00000960: 6373 2f61 7373 6574 732f 696d 6167 6573  cs/assets/images
-00000970: 2f67 6974 6875 625f 6973 7375 6573 2e70  /github_issues.p
-00000980: 6e67 2720 7374 796c 653d 2277 6964 7468  ng' style="width
-00000990: 3a20 3530 2522 3e3c 2f61 3e7c 0d0a 0d0a  : 50%"></a>|....
-000009a0: 0d0a 0d0a 3c21 2d2d 2050 6c65 6173 6520  ....<!-- Please 
-000009b0: 6369 7465 2074 6865 2066 6f6c 6c6f 7769  cite the followi
-000009c0: 6e67 2070 6170 6572 2069 6620 796f 7520  ng paper if you 
-000009d0: 7573 6520 4873 7561 6e77 7520 696e 2079  use Hsuanwu in y
-000009e0: 6f75 7220 776f 726b 2c20 7468 616e 6b20  our work, thank 
-000009f0: 796f 7521 0d0a 6060 6062 6962 7465 780d  you!..```bibtex.
-00000a00: 0a40 6172 7469 636c 657b 7975 616e 3230  .@article{yuan20
-00000a10: 3233 6873 7561 6e77 752c 0d0a 2020 7469  23hsuanwu,..  ti
-00000a20: 746c 653d 7b48 7375 616e 7775 3a20 4c6f  tle={Hsuanwu: Lo
-00000a30: 6e67 2d54 6572 6d20 4576 6f6c 7574 696f  ng-Term Evolutio
-00000a40: 6e20 5072 6f6a 6563 7420 6f66 2052 6569  n Project of Rei
-00000a50: 6e66 6f72 6365 6d65 6e74 204c 6561 726e  nforcement Learn
-00000a60: 696e 677d 2c0d 0a20 2061 7574 686f 723d  ing},..  author=
-00000a70: 7b59 7561 6e2c 204d 696e 6771 6920 616e  {Yuan, Mingqi an
-00000a80: 6420 4c75 6f2c 2053 6869 6861 6f20 616e  d Luo, Shihao an
-00000a90: 6420 5a68 616e 672c 205a 6571 756e 2061  d Zhang, Zequn a
-00000aa0: 6e64 2059 616e 672c 2058 7520 616e 6420  nd Yang, Xu and 
-00000ab0: 4a69 6e2c 2058 696e 2061 6e64 204c 692c  Jin, Xin and Li,
-00000ac0: 2042 6f20 616e 6420 5a65 6e67 2c20 5765   Bo and Zeng, We
-00000ad0: 6e6a 756e 7d2c 0d0a 2020 6a6f 7572 6e61  njun},..  journa
-00000ae0: 6c3d 7b61 7258 6976 2070 7265 7072 696e  l={arXiv preprin
-00000af0: 7420 6172 5869 763a 3233 3131 2e31 3532  t arXiv:2311.152
-00000b00: 3737 7d2c 0d0a 2020 7965 6172 3d7b 3230  77},..  year={20
-00000b10: 3233 7d0d 0a7d 0d0a 6060 6020 2d2d 3e0d  23}..}..``` -->.
-00000b20: 0a0d 0a2d 205b 5175 6963 6b20 5374 6172  ...- [Quick Star
-00000b30: 745d 2823 7175 6963 6b2d 7374 6172 7429  t](#quick-start)
-00000b40: 0d0a 2020 2d20 5b49 6e73 7461 6c6c 6174  ..  - [Installat
-00000b50: 696f 6e5d 2823 696e 7374 616c 6c61 7469  ion](#installati
-00000b60: 6f6e 290d 0a20 202d 205b 4275 696c 6420  on)..  - [Build 
-00000b70: 796f 7572 2066 6972 7374 2048 7375 616e  your first Hsuan
-00000b80: 7775 2061 7070 6c69 6361 7469 6f6e 5d28  wu application](
-00000b90: 2362 7569 6c64 2d79 6f75 722d 6669 7273  #build-your-firs
-00000ba0: 742d 6873 7561 6e77 752d 6170 706c 6963  t-hsuanwu-applic
-00000bb0: 6174 696f 6e29 0d0a 2d20 5b49 6d70 6c65  ation)..- [Imple
-00000bc0: 6d65 6e74 6564 204d 6f64 756c 6573 5d28  mented Modules](
-00000bd0: 2369 6d70 6c65 6d65 6e74 6564 2d6d 6f64  #implemented-mod
-00000be0: 756c 6573 290d 0a20 202d 205b 526f 6164  ules)..  - [Road
-00000bf0: 6d61 705d 2823 726f 6164 6d61 7029 0d0a  map](#roadmap)..
-00000c00: 2020 2d20 5b50 726f 6a65 6374 2053 7472    - [Project Str
-00000c10: 7563 7475 7265 5d28 2370 726f 6a65 6374  ucture](#project
-00000c20: 2d73 7472 7563 7475 7265 290d 0a20 202d  -structure)..  -
-00000c30: 205b 524c 2041 6765 6e74 735d 2823 726c   [RL Agents](#rl
-00000c40: 2d61 6765 6e74 7329 0d0a 2020 2d20 5b49  -agents)..  - [I
-00000c50: 6e74 7269 6e73 6963 2052 6577 6172 6420  ntrinsic Reward 
-00000c60: 4d6f 6475 6c65 735d 2823 696e 7472 696e  Modules](#intrin
-00000c70: 7369 632d 7265 7761 7264 2d6d 6f64 756c  sic-reward-modul
-00000c80: 6573 290d 0a2d 205b 4d6f 6465 6c20 5a6f  es)..- [Model Zo
-00000c90: 6f5d 2823 6d6f 6465 6c2d 7a6f 6f29 0d0a  o](#model-zoo)..
-00000ca0: 2d20 5b41 5049 2044 6f63 756d 656e 7461  - [API Documenta
-00000cb0: 7469 6f6e 5d28 2361 7069 2d64 6f63 756d  tion](#api-docum
-00000cc0: 656e 7461 7469 6f6e 290d 0a2d 205b 486f  entation)..- [Ho
-00000cd0: 7720 546f 2043 6f6e 7472 6962 7574 655d  w To Contribute]
-00000ce0: 2823 686f 772d 746f 2d63 6f6e 7472 6962  (#how-to-contrib
-00000cf0: 7574 6529 0d0a 2d20 5b41 636b 6e6f 776c  ute)..- [Acknowl
-00000d00: 6564 676d 656e 745d 2823 6163 6b6e 6f77  edgment](#acknow
-00000d10: 6c65 6467 6d65 6e74 290d 0a0d 0a23 2051  ledgment)....# Q
-00000d20: 7569 636b 2053 7461 7274 0d0a 2323 2049  uick Start..## I
-00000d30: 6e73 7461 6c6c 6174 696f 6e0d 0a2d 2050  nstallation..- P
-00000d40: 7265 7265 7175 6973 6974 6573 0d0a 0d0a  rerequisites....
-00000d50: 4375 7272 656e 746c 792c 2048 7375 616e  Currently, Hsuan
-00000d60: 7775 2072 6571 7569 7265 7320 6050 7974  wu requires `Pyt
-00000d70: 686f 6e3e 3d33 2e38 602c 2075 7365 7220  hon>=3.8`, user 
-00000d80: 6361 6e20 6372 6561 7465 2061 6e20 7669  can create an vi
-00000d90: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
-00000da0: 7420 6279 0d0a 6060 6020 7368 0d0a 636f  t by..``` sh..co
-00000db0: 6e64 6120 6372 6561 7465 202d 6e20 6873  nda create -n hs
-00000dc0: 7561 6e77 7520 7079 7468 6f6e 3d33 2e38  uanwu python=3.8
-00000dd0: 0d0a 6060 600d 0a0d 0a2d 2077 6974 6820  ..```....- with 
-00000de0: 7069 7020 6072 6563 6f6d 6d65 6e64 6564  pip `recommended
-00000df0: 600d 0a0d 0a4f 7065 6e20 7570 2061 2074  `....Open up a t
-00000e00: 6572 6d69 6e61 6c20 616e 6420 696e 7374  erminal and inst
-00000e10: 616c 6c20 2a2a 4873 7561 6e77 752a 2a20  all **Hsuanwu** 
-00000e20: 7769 7468 2060 7069 7060 3a0d 0a60 6060  with `pip`:..```
-00000e30: 2073 6865 6c6c 0d0a 7069 7020 696e 7374   shell..pip inst
-00000e40: 616c 6c20 6873 7561 6e77 7520 2320 6261  all hsuanwu # ba
-00000e50: 7369 6320 696e 7374 616c 6c61 7469 6f6e  sic installation
-00000e60: 0d0a 7069 7020 696e 7374 616c 6c20 6873  ..pip install hs
-00000e70: 7561 6e77 755b 656e 7673 5d20 2320 666f  uanwu[envs] # fo
-00000e80: 7220 7072 652d 6465 6669 6e65 6420 656e  r pre-defined en
-00000e90: 7669 726f 6e6d 656e 7473 0d0a 7069 7020  vironments..pip 
-00000ea0: 696e 7374 616c 6c20 6873 7561 6e77 755b  install hsuanwu[
-00000eb0: 7465 7374 735d 2023 2066 6f72 2070 726f  tests] # for pro
-00000ec0: 6a65 6374 2074 6573 7473 0d0a 7069 7020  ject tests..pip 
-00000ed0: 696e 7374 616c 6c20 6873 7561 6e77 755b  install hsuanwu[
-00000ee0: 616c 6c5d 2023 2069 6e73 7461 6c6c 2061  all] # install a
-00000ef0: 6c6c 2074 6865 2064 6570 656e 6465 6e63  ll the dependenc
-00000f00: 6965 730d 0a60 6060 0d0a 0d0a 2d20 7769  ies..```....- wi
-00000f10: 7468 2067 6974 0d0a 0d0a 4f70 656e 2075  th git....Open u
-00000f20: 7020 6120 7465 726d 696e 616c 2061 6e64  p a terminal and
-00000f30: 2063 6c6f 6e65 2074 6865 2072 6570 6f73   clone the repos
-00000f40: 6974 6f72 7920 6672 6f6d 205b 4769 7448  itory from [GitH
-00000f50: 7562 5d28 6874 7470 733a 2f2f 6769 7468  ub](https://gith
-00000f60: 7562 2e63 6f6d 2f52 4c45 2d46 6f75 6e64  ub.com/RLE-Found
-00000f70: 6174 696f 6e2f 4873 7561 6e77 7529 2077  ation/Hsuanwu) w
-00000f80: 6974 6820 6067 6974 603a 0d0a 6060 6020  ith `git`:..``` 
-00000f90: 7368 0d0a 6769 7420 636c 6f6e 6520 6874  sh..git clone ht
-00000fa0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000fb0: 2f52 4c45 2d46 6f75 6e64 6174 696f 6e2f  /RLE-Foundation/
-00000fc0: 4873 7561 6e77 752e 6769 740d 0a60 6060  Hsuanwu.git..```
-00000fd0: 0d0a 4166 7465 7220 7468 6174 2c20 7275  ..After that, ru
-00000fe0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-00000ff0: 636f 6d6d 616e 6420 746f 2069 6e73 7461  command to insta
-00001000: 6c6c 2070 6163 6b61 6765 2061 6e64 2064  ll package and d
-00001010: 6570 656e 6465 6e63 6965 733a 0d0a 6060  ependencies:..``
-00001020: 6020 7368 0d0a 7069 7020 696e 7374 616c  ` sh..pip instal
-00001030: 6c20 2d65 202e 2023 2062 6173 6963 2069  l -e . # basic i
-00001040: 6e73 7461 6c6c 6174 696f 6e0d 0a70 6970  nstallation..pip
-00001050: 2069 6e73 7461 6c6c 202d 6520 2e5b 656e   install -e .[en
-00001060: 7673 5d20 2320 666f 7220 7072 652d 6465  vs] # for pre-de
-00001070: 6669 6e65 6420 656e 7669 726f 6e6d 656e  fined environmen
-00001080: 7473 0d0a 7069 7020 696e 7374 616c 6c20  ts..pip install 
-00001090: 2d65 202e 5b74 6573 7473 5d20 2320 666f  -e .[tests] # fo
-000010a0: 7220 7072 6f6a 6563 7420 7465 7374 730d  r project tests.
-000010b0: 0a70 6970 2069 6e73 7461 6c6c 202d 6520  .pip install -e 
-000010c0: 2e5b 616c 6c5d 2023 2069 6e73 7461 6c6c  .[all] # install
-000010d0: 2061 6c6c 2074 6865 2064 6570 656e 6465   all the depende
-000010e0: 6e63 6965 730d 0a60 6060 0d0a 0d0a 466f  ncies..```....Fo
-000010f0: 7220 6d6f 7265 2064 6574 6169 6c65 6420  r more detailed 
-00001100: 696e 7374 616c 6c61 7469 6f6e 2069 6e73  installation ins
-00001110: 7472 7563 7469 6f6e 2c20 7365 6520 5b68  truction, see [h
-00001120: 7474 7073 3a2f 2f64 6f63 732e 6873 7561  ttps://docs.hsua
-00001130: 6e77 752e 6465 762f 6765 7474 696e 675f  nwu.dev/getting_
-00001140: 7374 6172 7465 645d 2868 7474 7073 3a2f  started](https:/
-00001150: 2f64 6f63 732e 6873 7561 6e77 752e 6465  /docs.hsuanwu.de
-00001160: 762f 6765 7474 696e 675f 7374 6172 7465  v/getting_starte
-00001170: 6429 2e0d 0a0d 0a23 2320 4275 696c 6420  d).....## Build 
-00001180: 796f 7572 2066 6972 7374 2048 7375 616e  your first Hsuan
-00001190: 7775 2061 7070 6c69 6361 7469 6f6e 0d0a  wu application..
-000011a0: 466f 7220 6578 616d 706c 652c 2077 6520  For example, we 
-000011b0: 7761 6e74 2074 6f20 7573 6520 5b44 7251  want to use [DrQ
-000011c0: 2d76 325d 2868 7474 7073 3a2f 2f6f 7065  -v2](https://ope
-000011d0: 6e72 6576 6965 772e 6e65 742f 666f 7275  nreview.net/foru
-000011e0: 6d3f 6964 3d5f 534a 2d5f 7979 6573 3829  m?id=_SJ-_yyes8)
-000011f0: 2074 6f20 736f 6c76 6520 6120 7461 736b   to solve a task
-00001200: 206f 6620 5b44 6565 704d 696e 6420 436f   of [DeepMind Co
-00001210: 6e74 726f 6c20 5375 6974 655d 2868 7474  ntrol Suite](htt
-00001220: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001230: 6465 6570 6d69 6e64 2f64 6d5f 636f 6e74  deepmind/dm_cont
-00001240: 726f 6c29 2c20 616e 6420 7765 206f 6e6c  rol), and we onl
-00001250: 7920 6e65 6564 2074 6865 2066 6f6c 6c6f  y need the follo
-00001260: 7769 6e67 2074 776f 2073 7465 7073 3a0d  wing two steps:.
-00001270: 0a0d 0a31 2e20 5772 6974 6520 6120 6063  ...1. Write a `c
-00001280: 6f6e 6669 672e 7961 6d6c 6020 6669 6c65  onfig.yaml` file
-00001290: 2069 6e20 796f 7572 2077 6f72 6b69 6e67   in your working
-000012a0: 2064 6972 6563 746f 7279 206c 696b 653a   directory like:
-000012b0: 0d0a 6060 6020 7961 6d6c 0d0a 6578 7065  ..``` yaml..expe
-000012c0: 7269 6d65 6e74 3a20 6472 7176 325f 646d  riment: drqv2_dm
-000012d0: 6320 2020 2020 2320 4578 7065 7269 6d65  c     # Experime
-000012e0: 6e74 2049 442e 0d0a 6465 7669 6365 3a20  nt ID...device: 
-000012f0: 6375 6461 3a30 2020 2020 2020 2020 2020  cuda:0          
-00001300: 2020 2320 4465 7669 6365 2028 6370 752c    # Device (cpu,
-00001310: 2063 7564 612c 202e 2e2e 2920 6f6e 2077   cuda, ...) on w
-00001320: 6869 6368 2074 6865 2063 6f64 6520 7368  hich the code sh
-00001330: 6f75 6c64 2062 6520 7275 6e2e 0d0a 7365  ould be run...se
-00001340: 6564 3a20 3120 2020 2020 2020 2020 2020  ed: 1           
-00001350: 2020 2020 2020 2020 2320 5261 6e64 6f6d          # Random
-00001360: 2073 6565 6420 666f 7220 7265 7072 6f64   seed for reprod
-00001370: 7563 7469 6f6e 2e0d 0a6e 756d 5f74 7261  uction...num_tra
-00001380: 696e 5f73 7465 7073 3a20 3235 3030 3030  in_steps: 250000
-00001390: 2020 2023 204e 756d 6265 7220 6f66 2074     # Number of t
-000013a0: 7261 696e 696e 6720 7374 6570 732e 0d0a  raining steps...
-000013b0: 0d0a 6167 656e 743a 0d0a 2020 6e61 6d65  ..agent:..  name
-000013c0: 3a20 4472 5176 3220 2020 2020 2020 2020  : DrQv2         
-000013d0: 2020 2020 2320 5468 6520 6167 656e 7420      # The agent 
-000013e0: 6e61 6d65 2e0d 0a60 6060 0d0a 0d0a 322e  name...```....2.
-000013f0: 2057 7269 7465 2061 2060 7472 6169 6e2e   Write a `train.
-00001400: 7079 6020 6669 6c65 206c 696b 653a 0d0a  py` file like:..
-00001410: 6060 6020 7079 7468 6f6e 0d0a 696d 706f  ``` python..impo
-00001420: 7274 2068 7964 7261 2023 2055 7365 2048  rt hydra # Use H
-00001430: 7964 7261 2074 6f20 6d61 6e61 6765 2065  ydra to manage e
-00001440: 7870 6572 696d 656e 7473 0d0a 0d0a 6672  xperiments....fr
-00001450: 6f6d 2068 7375 616e 7775 2e65 6e76 2069  om hsuanwu.env i
-00001460: 6d70 6f72 7420 6d61 6b65 5f64 6d63 5f65  mport make_dmc_e
-00001470: 6e76 2023 2049 6d70 6f72 7420 4465 6570  nv # Import Deep
-00001480: 4d69 6e64 2043 6f6e 7472 6f6c 2053 7569  Mind Control Sui
-00001490: 7465 0d0a 6672 6f6d 2068 7375 616e 7775  te..from hsuanwu
-000014a0: 2e63 6f6d 6d6f 6e2e 656e 6769 6e65 2069  .common.engine i
-000014b0: 6d70 6f72 7420 4873 7561 6e77 7545 6e67  mport HsuanwuEng
-000014c0: 696e 6520 2320 496d 706f 7274 2048 7375  ine # Import Hsu
-000014d0: 616e 7775 2065 6e67 696e 650d 0a0d 0a74  anwu engine....t
-000014e0: 7261 696e 5f65 6e76 203d 206d 616b 655f  rain_env = make_
-000014f0: 646d 635f 656e 7628 656e 765f 6964 3d27  dmc_env(env_id='
-00001500: 6361 7274 706f 6c65 5f62 616c 616e 6365  cartpole_balance
-00001510: 2729 2023 2043 7265 6174 6520 7472 6169  ') # Create trai
-00001520: 6e20 656e 760d 0a74 6573 745f 656e 7620  n env..test_env 
-00001530: 3d20 6d61 6b65 5f64 6d63 5f65 6e76 2865  = make_dmc_env(e
-00001540: 6e76 5f69 643d 2763 6172 7470 6f6c 655f  nv_id='cartpole_
-00001550: 6261 6c61 6e63 6527 2920 2320 4372 6561  balance') # Crea
-00001560: 7465 2074 6573 7420 656e 760d 0a0d 0a40  te test env....@
-00001570: 6879 6472 612e 6d61 696e 2876 6572 7369  hydra.main(versi
-00001580: 6f6e 5f62 6173 653d 4e6f 6e65 2c20 636f  on_base=None, co
-00001590: 6e66 6967 5f70 6174 683d 272e 2f27 2c20  nfig_path='./', 
-000015a0: 636f 6e66 6967 5f6e 616d 653d 2763 6f6e  config_name='con
-000015b0: 6669 6727 290d 0a64 6566 206d 6169 6e28  fig')..def main(
-000015c0: 6366 6773 293a 0d0a 2020 2020 656e 6769  cfgs):..    engi
-000015d0: 6e65 203d 2048 7375 616e 7775 456e 6769  ne = HsuanwuEngi
-000015e0: 6e65 2863 6667 733d 6366 6773 2c20 7472  ne(cfgs=cfgs, tr
-000015f0: 6169 6e5f 656e 763d 7472 6169 6e5f 656e  ain_env=train_en
-00001600: 762c 2074 6573 745f 656e 763d 7465 7374  v, test_env=test
-00001610: 5f65 6e76 2920 2320 496e 6974 6961 6c69  _env) # Initiali
-00001620: 7a65 2065 6e67 696e 650d 0a20 2020 2065  ze engine..    e
-00001630: 6e67 696e 652e 696e 766f 6b65 2829 2023  ngine.invoke() #
-00001640: 2053 7461 7274 2074 7261 696e 696e 670d   Start training.
-00001650: 0a0d 0a69 6620 5f5f 6e61 6d65 5f5f 203d  ...if __name__ =
-00001660: 3d20 275f 5f6d 6169 6e5f 5f27 3a0d 0a20  = '__main__':.. 
-00001670: 2020 206d 6169 6e28 290d 0a60 6060 0d0a     main()..```..
-00001680: 5275 6e20 6074 7261 696e 2e70 7960 2061  Run `train.py` a
-00001690: 6e64 2079 6f75 2077 696c 6c20 7365 6520  nd you will see 
-000016a0: 7468 6520 666f 6c6c 6f77 696e 6720 6f75  the following ou
-000016b0: 7470 7574 3a0d 0a0d 0a3c 6469 7620 616c  tput:....<div al
-000016c0: 6967 6e3d 6365 6e74 6572 3e0d 0a3c 696d  ign=center>..<im
-000016d0: 6720 7372 633d 272e 2f64 6f63 732f 6173  g src='./docs/as
-000016e0: 7365 7473 2f69 6d61 6765 732f 726c 5f74  sets/images/rl_t
-000016f0: 7261 696e 696e 672e 706e 6727 3e0d 0a3c  raining.png'>..<
-00001700: 2f64 6976 3e0d 0a0d 0a46 6f72 206d 6f72  /div>....For mor
-00001710: 6520 6465 7461 696c 6564 2074 7574 6f72  e detailed tutor
-00001720: 6961 6c73 2c20 7365 6520 5b68 7474 7073  ials, see [https
-00001730: 3a2f 2f64 6f63 732e 6873 7561 6e77 752e  ://docs.hsuanwu.
-00001740: 6465 762f 7475 746f 7269 616c 735d 2868  dev/tutorials](h
-00001750: 7474 7073 3a2f 2f64 6f63 732e 6873 7561  ttps://docs.hsua
-00001760: 6e77 752e 6465 762f 7475 746f 7269 616c  nwu.dev/tutorial
-00001770: 7329 2e0d 0a0d 0a23 2049 6d70 6c65 6d65  s).....# Impleme
-00001780: 6e74 6564 204d 6f64 756c 6573 0d0a 2323  nted Modules..##
-00001790: 2052 6f61 646d 6170 0d0a 4873 7561 6e77   Roadmap..Hsuanw
-000017a0: 7520 6576 6f6c 7665 7320 6261 7365 6420  u evolves based 
-000017b0: 6f6e 2072 6569 6e66 6f72 6365 6d65 6e74  on reinforcement
-000017c0: 206c 6561 726e 696e 6720 616c 676f 7269   learning algori
-000017d0: 7468 6d73 2061 6e64 2069 6e74 6567 7261  thms and integra
-000017e0: 7465 7320 6c61 7465 7374 2074 7269 636b  tes latest trick
-000017f0: 732e 2054 6865 2066 6f6c 6c6f 7769 6e67  s. The following
-00001800: 2066 6967 7572 6520 6465 6d6f 6e73 7472   figure demonstr
-00001810: 6174 6573 2074 6865 206d 6169 6e20 6576  ates the main ev
-00001820: 6f6c 7574 696f 6e20 726f 6164 6d61 7020  olution roadmap 
-00001830: 6f66 2048 7375 616e 7775 3a0d 0a0d 0a3c  of Hsuanwu:....<
-00001840: 6469 7620 616c 6967 6e3d 6365 6e74 6572  div align=center
-00001850: 3e0d 0a3c 696d 6720 7372 633d 272e 2f64  >..<img src='./d
-00001860: 6f63 732f 6173 7365 7473 2f69 6d61 6765  ocs/assets/image
-00001870: 732f 726f 6164 6d61 702e 7376 6727 2020  s/roadmap.svg'  
-00001880: 7374 796c 653d 2277 6964 7468 3a20 3930  style="width: 90
-00001890: 2522 3e0d 0a3c 2f64 6976 3e0d 0a0d 0a23  %">..</div>....#
-000018a0: 2320 5072 6f6a 6563 7420 5374 7275 6374  # Project Struct
-000018b0: 7572 650d 0a0d 0a53 6565 2074 6865 2070  ure....See the p
-000018c0: 726f 6a65 6374 2073 7472 7563 7475 7265  roject structure
-000018d0: 2062 656c 6f77 3a0d 0a3c 6469 7620 616c   below:..<div al
-000018e0: 6967 6e3d 6365 6e74 6572 3e0d 0a3c 696d  ign=center>..<im
-000018f0: 6720 7372 633d 272e 2f64 6f63 732f 6173  g src='./docs/as
-00001900: 7365 7473 2f69 6d61 6765 732f 7374 7275  sets/images/stru
-00001910: 6374 7572 652e 7376 6727 2073 7479 6c65  cture.svg' style
-00001920: 3d22 7769 6474 683a 2039 3025 223e 0d0a  ="width: 90%">..
-00001930: 3c2f 6469 763e 0d0a 0d0a 2d20 2a2a 5b43  </div>....- **[C
-00001940: 6f6d 6d6f 6e5d 2868 7474 7073 3a2f 2f64  ommon](https://d
-00001950: 6f63 732e 6873 7561 6e77 752e 6465 762f  ocs.hsuanwu.dev/
-00001960: 636f 6d6d 6f6e 5f69 6e64 6578 2f29 2a2a  common_index/)**
-00001970: 3a20 4175 7869 6c69 6172 7920 6d6f 6475  : Auxiliary modu
-00001980: 6c65 7320 6c69 6b65 2074 7261 696e 6572  les like trainer
-00001990: 2061 6e64 206c 6f67 6765 722e 0d0a 2020   and logger...  
-000019a0: 2020 2b20 2a2a 456e 6769 6e65 2a2a 3a20    + **Engine**: 
-000019b0: 2a45 6e67 696e 6520 666f 7220 6275 696c  *Engine for buil
-000019c0: 6469 6e67 2048 7375 616e 7775 2061 7070  ding Hsuanwu app
-000019d0: 6c69 6361 7469 6f6e 2e2a 0d0a 2020 2020  lication.*..    
-000019e0: 2b20 2a2a 4c6f 6767 6572 2a2a 3a20 2a4c  + **Logger**: *L
-000019f0: 6f67 6765 7220 666f 7220 6d61 6e61 6769  ogger for managi
-00001a00: 6e67 206f 7574 7075 7420 696e 666f 726d  ng output inform
-00001a10: 6174 696f 6e2e 2a0d 0a0d 0a2d 202a 2a5b  ation.*....- **[
-00001a20: 5870 6c6f 6974 5d28 6874 7470 733a 2f2f  Xploit](https://
-00001a30: 646f 6373 2e68 7375 616e 7775 2e64 6576  docs.hsuanwu.dev
-00001a40: 2f78 706c 6f69 745f 696e 6465 782f 292a  /xploit_index/)*
-00001a50: 2a3a 204d 6f64 756c 6573 2074 6861 7420  *: Modules that 
-00001a60: 666f 6375 7320 6f6e 203c 666f 6e74 2063  focus on <font c
-00001a70: 6f6c 6f72 3d22 2342 3830 3030 3022 3e3c  olor="#B80000"><
-00001a80: 623e 6578 706c 6f69 7461 7469 6f6e 3c2f  b>exploitation</
-00001a90: 623e 3c2f 666f 6e74 3e20 696e 2052 4c2e  b></font> in RL.
-00001aa0: 0d0a 2020 2020 2b20 2a2a 456e 636f 6465  ..    + **Encode
-00001ab0: 722a 2a3a 202a 4e65 7572 616c 206e 6577  r**: *Neural new
-00001ac0: 6f72 6b2d 6261 7365 6420 656e 636f 6465  ork-based encode
-00001ad0: 7220 666f 7220 7072 6f63 6573 7369 6e67  r for processing
-00001ae0: 206f 6273 6572 7661 7469 6f6e 732e 2a0d   observations.*.
-00001af0: 0a20 2020 202b 202a 2a41 6765 6e74 2a2a  .    + **Agent**
-00001b00: 3a20 2a41 6765 6e74 2066 6f72 2069 6e74  : *Agent for int
-00001b10: 6572 6163 7469 6e67 2061 6e64 206c 6561  eracting and lea
-00001b20: 726e 696e 672e 2a0d 0a20 2020 202b 202a  rning.*..    + *
-00001b30: 2a53 746f 7261 6765 2a2a 3a20 2a53 746f  *Storage**: *Sto
-00001b40: 7261 6765 2066 6f72 2073 746f 7269 6e67  rage for storing
-00001b50: 2063 6f6c 6c65 6374 6564 2065 7870 6572   collected exper
-00001b60: 6965 6e63 6573 2e2a 0d0a 0d0a 2d20 2a2a  iences.*....- **
-00001b70: 5b58 706c 6f72 655d 2868 7474 7073 3a2f  [Xplore](https:/
-00001b80: 2f64 6f63 732e 6873 7561 6e77 752e 6465  /docs.hsuanwu.de
-00001b90: 762f 7870 6c6f 7265 5f69 6e64 6578 2f29  v/xplore_index/)
-00001ba0: 2a2a 3a20 4d6f 6475 6c65 7320 7468 6174  **: Modules that
-00001bb0: 2066 6f63 7573 206f 6e20 3c66 6f6e 7420   focus on <font 
-00001bc0: 636f 6c6f 723d 2223 4238 3030 3030 223e  color="#B80000">
-00001bd0: 3c62 3e65 7870 6c6f 7261 7469 6f6e 3c2f  <b>exploration</
-00001be0: 623e 3c2f 666f 6e74 3e20 696e 2052 4c2e  b></font> in RL.
-00001bf0: 0d0a 2020 2020 2b20 2a2a 4175 676d 656e  ..    + **Augmen
-00001c00: 7461 7469 6f6e 2a2a 3a20 2a50 7954 6f72  tation**: *PyTor
-00001c10: 6368 2e6e 6e2d 6c69 6b65 206d 6f64 756c  ch.nn-like modul
-00001c20: 6573 2066 6f72 206f 6273 6572 7661 7469  es for observati
-00001c30: 6f6e 2061 7567 6d65 6e74 6174 696f 6e2e  on augmentation.
-00001c40: 2a0d 0a20 2020 202b 202a 2a44 6973 7472  *..    + **Distr
-00001c50: 6962 7574 696f 6e2a 2a3a 202a 4469 7374  ibution**: *Dist
-00001c60: 7269 6275 7469 6f6e 7320 666f 7220 7361  ributions for sa
-00001c70: 6d70 6c69 6e67 2061 6374 696f 6e73 2e2a  mpling actions.*
-00001c80: 0d0a 2020 2020 2b20 2a2a 5265 7761 7264  ..    + **Reward
-00001c90: 2a2a 3a20 2a49 6e74 7269 6e73 6963 2072  **: *Intrinsic r
-00001ca0: 6577 6172 6420 6d6f 6475 6c65 7320 666f  eward modules fo
-00001cb0: 7220 656e 6861 6e63 696e 6720 6578 706c  r enhancing expl
-00001cc0: 6f72 6174 696f 6e2e 2a0d 0a0d 0a2d 202a  oration.*....- *
-00001cd0: 2a5b 4576 616c 7561 7469 6f6e 5d28 6874  *[Evaluation](ht
-00001ce0: 7470 733a 2f2f 646f 6373 2e68 7375 616e  tps://docs.hsuan
-00001cf0: 7775 2e64 6576 2f65 7661 6c75 6174 696f  wu.dev/evaluatio
-00001d00: 6e5f 696e 6465 782f 292a 2a3a 2052 6561  n_index/)**: Rea
-00001d10: 736f 6e61 626c 6520 616e 6420 7265 6c69  sonable and reli
-00001d20: 6162 6c65 206d 6574 7269 6373 2066 6f72  able metrics for
-00001d30: 2061 6c67 6f72 6974 686d 2065 7661 6c75   algorithm evalu
-00001d40: 6174 696f 6e2e 0d0a 0d0a 2d20 2a2a 5b45  ation.....- **[E
-00001d50: 6e76 5d28 6874 7470 733a 2f2f 646f 6373  nv](https://docs
-00001d60: 2e68 7375 616e 7775 2e64 6576 2f65 6e76  .hsuanwu.dev/env
-00001d70: 5f69 6e64 6578 2f29 2a2a 3a20 5061 636b  _index/)**: Pack
-00001d80: 6167 6564 2065 6e76 6972 6f6e 6d65 6e74  aged environment
-00001d90: 7320 2865 2e67 2e2c 2041 7461 7269 2067  s (e.g., Atari g
-00001da0: 616d 6573 2920 666f 7220 6661 7374 2069  ames) for fast i
-00001db0: 6e76 6f63 6174 696f 6e2e 0d0a 0d0a 2d20  nvocation.....- 
-00001dc0: 2a2a 5b50 7265 2d74 7261 696e 696e 675d  **[Pre-training]
-00001dd0: 2868 7474 7073 3a2f 2f64 6f63 732e 6873  (https://docs.hs
-00001de0: 7561 6e77 752e 6465 762f 7072 6574 7261  uanwu.dev/pretra
-00001df0: 696e 696e 675f 696e 6465 782f 292a 2a3a  ining_index/)**:
-00001e00: 204d 6574 686f 6473 206f 6620 3c66 6f6e   Methods of <fon
-00001e10: 7420 636f 6c6f 723d 2223 4238 3030 3030  t color="#B80000
-00001e20: 223e 3c62 3e70 7265 2d74 7261 696e 696e  "><b>pre-trainin
-00001e30: 673c 2f62 3e3c 2f66 6f6e 743e 2069 6e20  g</b></font> in 
-00001e40: 524c 2e0d 0a0d 0a2d 202a 2a5b 4465 706c  RL.....- **[Depl
-00001e50: 6f79 6d65 6e74 5d28 6874 7470 733a 2f2f  oyment](https://
-00001e60: 646f 6373 2e68 7375 616e 7775 2e64 6576  docs.hsuanwu.dev
-00001e70: 2f64 6570 6c6f 796d 656e 745f 696e 6465  /deployment_inde
-00001e80: 782f 292a 2a3a 204d 6574 686f 6473 206f  x/)**: Methods o
-00001e90: 6620 3c66 6f6e 7420 636f 6c6f 723d 2223  f <font color="#
-00001ea0: 4238 3030 3030 223e 3c62 3e6d 6f64 656c  B80000"><b>model
-00001eb0: 2064 6570 6c6f 796d 656e 743c 2f62 3e3c   deployment</b><
-00001ec0: 2f66 6f6e 743e 2069 6e20 524c 2e0d 0a0d  /font> in RL....
-00001ed0: 0a46 6f72 206d 6f72 6520 6465 7469 6c65  .For more detile
-00001ee0: 6420 6465 7363 7269 7074 696f 6e73 206f  d descriptions o
-00001ef0: 6620 7468 6573 6520 6d6f 6475 6c65 732c  f these modules,
-00001f00: 2073 6565 205b 6874 7470 733a 2f2f 646f   see [https://do
-00001f10: 6373 2e68 7375 616e 7775 2e64 6576 2f61  cs.hsuanwu.dev/a
-00001f20: 7069 5d28 6874 7470 733a 2f2f 646f 6373  pi](https://docs
-00001f30: 2e68 7375 616e 7775 2e64 6576 2f6f 7665  .hsuanwu.dev/ove
-00001f40: 7276 6965 772f 6170 6929 0d0a 0d0a 2323  rview/api)....##
-00001f50: 2052 4c20 4167 656e 7473 0d0a 7c4d 6f64   RL Agents..|Mod
-00001f60: 756c 657c 5265 6375 7272 656e 747c 426f  ule|Recurrent|Bo
-00001f70: 787c 4469 7363 7265 7465 7c4d 756c 7469  x|Discrete|Multi
-00001f80: 4269 6e61 7279 7c4d 756c 7469 2050 726f  Binary|Multi Pro
-00001f90: 6365 7373 696e 677c 4e50 557c 5061 7065  cessing|NPU|Pape
-00001fa0: 727c 4369 7461 7469 6f6e 737c 0d0a 7c3a  r|Citations|..|:
-00001fb0: 2d7c 3a2d 7c3a 2d7c 3a2d 7c3a 2d7c 3a2d  -|:-|:-|:-|:-|:-
-00001fc0: 7c3a 2d7c 3a2d 7c3a 2d7c 0d0a 7c53 4143  |:-|:-|:-|..|SAC
-00001fd0: 7ce2 9d8c 7c20 e29c 94ef b88f 207c e29d  |...| ...... |..
-00001fe0: 8c7c e29d 8c7c e29d 8c7c f09f 908c 207c  .|...|...|.... |
-00001ff0: 205b 4c69 6e6b 5d28 6874 7470 3a2f 2f70   [Link](http://p
-00002000: 726f 6365 6564 696e 6773 2e6d 6c72 2e70  roceedings.mlr.p
-00002010: 7265 7373 2f76 3830 2f68 6161 726e 6f6a  ress/v80/haarnoj
-00002020: 6131 3862 2f68 6161 726e 6f6a 6131 3862  a18b/haarnoja18b
-00002030: 2e70 6466 2920 7c35 3037 37e2 ad90 7c0d  .pdf) |5077...|.
-00002040: 0a7c 4472 517c e29d 8c7c 20e2 9c94 efb8  .|DrQ|...| .....
-00002050: 8f20 7ce2 9d8c 7ce2 9d8c 7ce2 9d8c 7cf0  . |...|...|...|.
-00002060: 9f90 8c20 7c20 5b4c 696e 6b5d 2868 7474  ... | [Link](htt
-00002070: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f70  ps://arxiv.org/p
-00002080: 6466 2f32 3030 342e 3133 3634 3929 207c  df/2004.13649) |
-00002090: 3433 33e2 ad90 7c0d 0a7c 4444 5047 7ce2  433...|..|DDPG|.
-000020a0: 9d8c 7c20 e29c 94ef b88f 207c e29d 8c7c  ..| ...... |...|
-000020b0: e29d 8c7c e29d 8c7c f09f 908c 207c 205b  ...|...|.... | [
-000020c0: 4c69 6e6b 5d28 6874 7470 733a 2f2f 6172  Link](https://ar
-000020d0: 7869 762e 6f72 672f 7064 662f 3135 3039  xiv.org/pdf/1509
-000020e0: 2e30 3239 3731 2e70 6466 3f73 6f75 7263  .02971.pdf?sourc
-000020f0: 653d 706f 7374 5f70 6167 652d 2d2d 2d2d  e=post_page-----
-00002100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002110: 2d2d 2d2d 2d2d 2920 7c31 3138 3139 e2ad  ------) |11819..
-00002120: 907c 0d0a 7c44 7251 2d76 327c e29d 8c7c  .|..|DrQ-v2|...|
-00002130: 20e2 9c94 efb8 8f20 7ce2 9d8c 7ce2 9d8c   ...... |...|...
-00002140: 7ce2 9d8c 7cf0 9f90 8c20 7c20 5b4c 696e  |...|.... | [Lin
-00002150: 6b5d 2868 7474 7073 3a2f 2f61 7278 6976  k](https://arxiv
-00002160: 2e6f 7267 2f70 6466 2f32 3130 372e 3039  .org/pdf/2107.09
-00002170: 3634 352e 7064 663f 7574 6d5f 736f 7572  645.pdf?utm_sour
-00002180: 6365 3d6d 6f72 696f 682e 636f 6d29 207c  ce=morioh.com) |
-00002190: 3130 30e2 ad90 7c0d 0a7c 5050 4f7c e29d  100...|..|PPO|..
-000021a0: 8c7c 20e2 9c94 efb8 8f20 7ce2 9c94 efb8  .| ...... |.....
-000021b0: 8f7c f09f 908c 7ce2 9c94 efb8 8f7c f09f  .|....|......|..
-000021c0: 908c 207c 205b 4c69 6e6b 5d28 6874 7470  .. | [Link](http
-000021d0: 733a 2f2f 6172 7869 762e 6f72 672f 7064  s://arxiv.org/pd
-000021e0: 662f 3137 3037 2e30 3633 3437 2920 7c31  f/1707.06347) |1
-000021f0: 3131 3535 e2ad 907c 0d0a 7c44 7241 437c  1155...|..|DrAC|
-00002200: e29d 8c7c 20e2 9c94 efb8 8f20 7ce2 9c94  ...| ...... |...
-00002210: efb8 8f7c f09f 908c 7ce2 9c94 efb8 8f7c  ...|....|......|
-00002220: f09f 908c 207c 205b 4c69 6e6b 5d28 6874  .... | [Link](ht
-00002230: 7470 733a 2f2f 7072 6f63 6565 6469 6e67  tps://proceeding
-00002240: 732e 6e65 7572 6970 732e 6363 2f70 6170  s.neurips.cc/pap
-00002250: 6572 2f32 3032 312f 6669 6c65 2f32 6233  er/2021/file/2b3
-00002260: 3863 3264 6636 6134 3962 3937 6637 3036  8c2df6a49b97f706
-00002270: 6563 3931 3438 6365 3438 6438 362d 5061  ec9148ce48d86-Pa
-00002280: 7065 722e 7064 6629 207c 3239 e2ad 907c  per.pdf) |29...|
-00002290: 0d0a 7c50 5047 7ce2 9d8c 7c20 e29c 94ef  ..|PPG|...| ....
-000022a0: b88f 207c e29c 94ef b88f 7cf0 9f90 8c7c  .. |......|....|
-000022b0: e29c 94ef b88f 7cf0 9f90 8c7c 205b 4c69  ......|....| [Li
-000022c0: 6e6b 5d28 6874 7470 3a2f 2f70 726f 6365  nk](http://proce
-000022d0: 6564 696e 6773 2e6d 6c72 2e70 7265 7373  edings.mlr.press
-000022e0: 2f76 3133 392f 636f 6262 6532 3161 2f63  /v139/cobbe21a/c
-000022f0: 6f62 6265 3231 612e 7064 6629 207c 3832  obbe21a.pdf) |82
-00002300: e2ad 907c 0d0a 7c49 4d50 414c 417c e29c  ...|..|IMPALA|..
-00002310: 94ef b88f 7c20 e29c 94ef b88f 207c e29c  ....| ...... |..
-00002320: 94ef b88f 7cf0 9f90 8c7c e29c 94ef b88f  ....|....|......
-00002330: 7cf0 9f90 8c7c 205b 4c69 6e6b 5d28 6874  |....| [Link](ht
-00002340: 7470 3a2f 2f70 726f 6365 6564 696e 6773  tp://proceedings
-00002350: 2e6d 6c72 2e70 7265 7373 2f76 3830 2f65  .mlr.press/v80/e
-00002360: 7370 6568 6f6c 7431 3861 2f65 7370 6568  speholt18a/espeh
-00002370: 6f6c 7431 3861 2e70 6466 2920 7c31 3231  olt18a.pdf) |121
-00002380: 39e2 ad90 7c0d 0a0d 0a3e 202d 20f0 9f90  9...|....> - ...
-00002390: 8c3a 2044 6576 656c 6f70 696e 672e 0d0a  .: Developing...
-000023a0: 3e20 2d20 604e 5055 603a 2053 7570 706f  > - `NPU`: Suppo
-000023b0: 7274 204e 6575 7261 6c2d 6e65 7477 6f72  rt Neural-networ
-000023c0: 6b20 7072 6f63 6573 7369 6e67 2075 6e69  k processing uni
-000023d0: 742e 0d0a 3e20 2d20 6052 6563 7572 7265  t...> - `Recurre
-000023e0: 6e74 603a 2053 7570 706f 7274 2072 6563  nt`: Support rec
-000023f0: 7572 7265 6e74 206e 6575 7261 6c20 6e65  urrent neural ne
-00002400: 7477 6f72 6b2e 0d0a 3e20 2d20 6042 6f78  twork...> - `Box
-00002410: 603a 2041 204e 2d64 696d 656e 7369 6f6e  `: A N-dimension
-00002420: 616c 2062 6f78 2074 6861 7420 636f 6e74  al box that cont
-00002430: 6169 6e65 7320 6576 6572 7920 706f 696e  aines every poin
-00002440: 7420 696e 2074 6865 2061 6374 696f 6e20  t in the action 
-00002450: 7370 6163 652e 0d0a 3e20 2d20 6044 6973  space...> - `Dis
-00002460: 6372 6574 6560 3a20 4120 6c69 7374 206f  crete`: A list o
-00002470: 6620 706f 7373 6962 6c65 2061 6374 696f  f possible actio
-00002480: 6e73 2c20 7768 6572 6520 6561 6368 2074  ns, where each t
-00002490: 696d 6573 7465 7020 6f6e 6c79 206f 6e65  imestep only one
-000024a0: 206f 6620 7468 6520 6163 7469 6f6e 7320   of the actions 
-000024b0: 6361 6e20 6265 2075 7365 642e 0d0a 3e20  can be used...> 
-000024c0: 2d20 604d 756c 7469 4269 6e61 7279 603a  - `MultiBinary`:
-000024d0: 2041 206c 6973 7420 6f66 2070 6f73 7369   A list of possi
-000024e0: 626c 6520 6163 7469 6f6e 732c 2077 6865  ble actions, whe
-000024f0: 7265 2065 6163 6820 7469 6d65 7374 6570  re each timestep
-00002500: 2061 6e79 206f 6620 7468 6520 6163 7469   any of the acti
-00002510: 6f6e 7320 6361 6e20 6265 2075 7365 6420  ons can be used 
-00002520: 696e 2061 6e79 2063 6f6d 6269 6e61 7469  in any combinati
-00002530: 6f6e 2e0d 0a0d 0a23 2320 496e 7472 696e  on.....## Intrin
-00002540: 7369 6320 5265 7761 7264 204d 6f64 756c  sic Reward Modul
-00002550: 6573 0d0a 7c20 4d6f 6475 6c65 207c 2052  es..| Module | R
-00002560: 656d 6172 6b20 7c20 5265 7072 2e20 207c  emark | Repr.  |
-00002570: 2056 6973 7561 6c20 7c20 5265 6665 7265   Visual | Refere
-00002580: 6e63 6520 7c20 0d0a 7c3a 2d7c 3a2d 7c3a  nce | ..|:-|:-|:
-00002590: 2d7c 3a2d 7c3a 2d7c 0d0a 7c20 5073 6575  -|:-|:-|..| Pseu
-000025a0: 646f 436f 756e 7473 207c 2043 6f75 6e74  doCounts | Count
-000025b0: 2d42 6173 6564 2065 7870 6c6f 7261 7469  -Based explorati
-000025c0: 6f6e 207c e29c 94ef b88f 7ce2 9c94 efb8  on |......|.....
-000025d0: 8f7c 5b4e 6576 6572 2047 6976 6520 5570  .|[Never Give Up
-000025e0: 3a20 4c65 6172 6e69 6e67 2044 6972 6563  : Learning Direc
-000025f0: 7465 6420 4578 706c 6f72 6174 696f 6e20  ted Exploration 
-00002600: 5374 7261 7465 6769 6573 5d28 6874 7470  Strategies](http
-00002610: 733a 2f2f 6172 7869 762e 6f72 672f 7064  s://arxiv.org/pd
-00002620: 662f 3230 3032 2e30 3630 3338 2920 7c0d  f/2002.06038) |.
-00002630: 0a7c 2049 434d 2020 7c20 4375 7269 6f73  .| ICM  | Curios
-00002640: 6974 792d 6472 6976 656e 2065 7870 6c6f  ity-driven explo
-00002650: 7261 7469 6f6e 2020 7c20 e29c 94ef b88f  ration  | ......
-00002660: 7ce2 9c94 efb8 8f7c 205b 4375 7269 6f73  |......| [Curios
-00002670: 6974 792d 4472 6976 656e 2045 7870 6c6f  ity-Driven Explo
-00002680: 7261 7469 6f6e 2062 7920 5365 6c66 2d53  ration by Self-S
-00002690: 7570 6572 7669 7365 6420 5072 6564 6963  upervised Predic
-000026a0: 7469 6f6e 5d28 6874 7470 3a2f 2f70 726f  tion](http://pro
-000026b0: 6365 6564 696e 6773 2e6d 6c72 2e70 7265  ceedings.mlr.pre
-000026c0: 7373 2f76 3730 2f70 6174 6861 6b31 3761  ss/v70/pathak17a
-000026d0: 2f70 6174 6861 6b31 3761 2e70 6466 2920  /pathak17a.pdf) 
-000026e0: 7c20 0d0a 7c20 524e 4420 207c 2043 6f75  | ..| RND  | Cou
-000026f0: 6e74 2d62 6173 6564 2065 7870 6c6f 7261  nt-based explora
-00002700: 7469 6f6e 2020 7c20 e29d 8c7c e29c 94ef  tion  | ...|....
-00002710: b88f 7c20 5b45 7870 6c6f 7261 7469 6f6e  ..| [Exploration
-00002720: 2062 7920 5261 6e64 6f6d 204e 6574 776f   by Random Netwo
-00002730: 726b 2044 6973 7469 6c6c 6174 696f 6e5d  rk Distillation]
-00002740: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00002750: 7267 2f70 6466 2f31 3831 302e 3132 3839  rg/pdf/1810.1289
-00002760: 342e 7064 6629 207c 200d 0a7c 2047 4952  4.pdf) | ..| GIR
-00002770: 4d20 7c20 4375 7269 6f73 6974 792d 6472  M | Curiosity-dr
-00002780: 6976 656e 2065 7870 6c6f 7261 7469 6f6e  iven exploration
-00002790: 2020 7c20 e29c 94ef b88f 207c e29c 94ef    | ...... |....
-000027a0: b88f 7c20 5b49 6e74 7269 6e73 6963 2052  ..| [Intrinsic R
-000027b0: 6577 6172 6420 4472 6976 656e 2049 6d69  eward Driven Imi
-000027c0: 7461 7469 6f6e 204c 6561 726e 696e 6720  tation Learning 
-000027d0: 7669 6120 4765 6e65 7261 7469 7665 204d  via Generative M
-000027e0: 6f64 656c 5d28 6874 7470 3a2f 2f70 726f  odel](http://pro
-000027f0: 6365 6564 696e 6773 2e6d 6c72 2e70 7265  ceedings.mlr.pre
-00002800: 7373 2f76 3131 392f 7975 3230 642f 7975  ss/v119/yu20d/yu
-00002810: 3230 642e 7064 6629 7c0d 0a7c 204e 4755  20d.pdf)|..| NGU
-00002820: 207c 204d 656d 6f72 792d 6261 7365 6420   | Memory-based 
-00002830: 6578 706c 6f72 6174 696f 6e20 207c 20e2  exploration  | .
-00002840: 9c94 efb8 8f20 207c e29c 94ef b88f 7c20  .....  |......| 
-00002850: 5b4e 6576 6572 2047 6976 6520 5570 3a20  [Never Give Up: 
-00002860: 4c65 6172 6e69 6e67 2044 6972 6563 7465  Learning Directe
-00002870: 6420 4578 706c 6f72 6174 696f 6e20 5374  d Exploration St
-00002880: 7261 7465 6769 6573 5d28 6874 7470 733a  rategies](https:
-00002890: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
-000028a0: 3230 3032 2e30 3630 3338 2920 7c20 0d0a  2002.06038) | ..
-000028b0: 7c20 5249 4445 7c20 5072 6f63 6564 7572  | RIDE| Procedur
-000028c0: 616c 6c79 2d67 656e 6572 6174 6564 2065  ally-generated e
-000028d0: 6e76 6972 6f6e 6d65 6e74 207c 20e2 9c94  nvironment | ...
-000028e0: efb8 8f20 7ce2 9c94 efb8 8f7c 205b 5249  ... |......| [RI
-000028f0: 4445 3a20 5265 7761 7264 696e 6720 496d  DE: Rewarding Im
-00002900: 7061 6374 2d44 7269 7665 6e20 4578 706c  pact-Driven Expl
-00002910: 6f72 6174 696f 6e20 666f 7220 5072 6f63  oration for Proc
-00002920: 6564 7572 616c 6c79 2d47 656e 6572 6174  edurally-Generat
-00002930: 6564 2045 6e76 6972 6f6e 6d65 6e74 735d  ed Environments]
-00002940: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00002950: 7267 2f70 6466 2f32 3030 322e 3132 3239  rg/pdf/2002.1229
-00002960: 3229 7c0d 0a7c 2052 4533 2020 7c20 456e  2)|..| RE3  | En
-00002970: 7472 6f70 7920 4d61 7869 6d69 7a61 7469  tropy Maximizati
-00002980: 6f6e 207c 20e2 9d8c 207c e29c 94ef b88f  on | ... |......
-00002990: 7c20 5b53 7461 7465 2045 6e74 726f 7079  | [State Entropy
-000029a0: 204d 6178 696d 697a 6174 696f 6e20 7769   Maximization wi
-000029b0: 7468 2052 616e 646f 6d20 456e 636f 6465  th Random Encode
-000029c0: 7273 2066 6f72 2045 6666 6963 6965 6e74  rs for Efficient
-000029d0: 2045 7870 6c6f 7261 7469 6f6e 5d28 6874   Exploration](ht
-000029e0: 7470 3a2f 2f70 726f 6365 6564 696e 6773  tp://proceedings
-000029f0: 2e6d 6c72 2e70 7265 7373 2f76 3133 392f  .mlr.press/v139/
-00002a00: 7365 6f32 3161 2f73 656f 3231 612e 7064  seo21a/seo21a.pd
-00002a10: 6629 207c 0d0a 7c20 5249 5345 2020 7c20  f) |..| RISE  | 
-00002a20: 456e 7472 6f70 7920 4d61 7869 6d69 7a61  Entropy Maximiza
-00002a30: 7469 6f6e 2020 7c20 e29d 8c20 207c e29c  tion  | ...  |..
-00002a40: 94ef b88f 7c20 5b52 c3a9 6e79 6920 5374  ....| [R..nyi St
-00002a50: 6174 6520 456e 7472 6f70 7920 4d61 7869  ate Entropy Maxi
-00002a60: 6d69 7a61 7469 6f6e 2066 6f72 2045 7870  mization for Exp
-00002a70: 6c6f 7261 7469 6f6e 2041 6363 656c 6572  loration Acceler
-00002a80: 6174 696f 6e20 696e 2052 6569 6e66 6f72  ation in Reinfor
-00002a90: 6365 6d65 6e74 204c 6561 726e 696e 675d  cement Learning]
-00002aa0: 2868 7474 7073 3a2f 2f69 6565 6578 706c  (https://ieeexpl
-00002ab0: 6f72 652e 6965 6565 2e6f 7267 2f61 6273  ore.ieee.org/abs
-00002ac0: 7472 6163 742f 646f 6375 6d65 6e74 2f39  tract/document/9
-00002ad0: 3830 3239 3137 2f29 207c 200d 0a7c 2052  802917/) | ..| R
-00002ae0: 4556 4420 207c 2044 6976 6572 6765 6e63  EVD  | Divergenc
-00002af0: 6520 4d61 7869 6d69 7a61 7469 6f6e 207c  e Maximization |
-00002b00: 20e2 9d8c 2020 7ce2 9c94 efb8 8f7c 205b   ...  |......| [
-00002b10: 5265 7761 7264 696e 6720 4570 6973 6f64  Rewarding Episod
-00002b20: 6963 2056 6973 6974 6174 696f 6e20 4469  ic Visitation Di
-00002b30: 7363 7265 7061 6e63 7920 666f 7220 4578  screpancy for Ex
-00002b40: 706c 6f72 6174 696f 6e20 696e 2052 6569  ploration in Rei
-00002b50: 6e66 6f72 6365 6d65 6e74 204c 6561 726e  nforcement Learn
-00002b60: 696e 675d 2868 7474 7073 3a2f 2f6f 7065  ing](https://ope
-00002b70: 6e72 6576 6965 772e 6e65 742f 7064 663f  nreview.net/pdf?
-00002b80: 6964 3d56 3270 7731 5659 4d72 446f 297c  id=V2pw1VYMrDo)|
-00002b90: 0d0a 7c50 726f 746f 524c 3c73 7570 3ef0  ..|ProtoRL<sup>.
-00002ba0: 9f90 8c3c 2f73 7570 3e7c 2045 6e74 726f  ...</sup>| Entro
-00002bb0: 7079 204d 6178 696d 697a 6174 696f 6e20  py Maximization 
-00002bc0: 7c20 e29c 94ef b88f 207c 20e2 9c94 efb8  | ...... | .....
-00002bd0: 8f20 7c20 5b52 6569 6e66 6f72 6365 6d65  . | [Reinforceme
-00002be0: 6e74 204c 6561 726e 696e 6720 7769 7468  nt Learning with
-00002bf0: 2050 726f 746f 7479 7069 6361 6c20 5265   Prototypical Re
-00002c00: 7072 6573 656e 7461 7469 6f6e 735d 2868  presentations](h
-00002c10: 7474 703a 2f2f 7072 6f63 6565 6469 6e67  ttp://proceeding
-00002c20: 732e 6d6c 722e 7072 6573 732f 7631 3339  s.mlr.press/v139
-00002c30: 2f79 6172 6174 7332 3161 2f79 6172 6174  /yarats21a/yarat
-00002c40: 7332 3161 2e70 6466 2920 7c0d 0a7c 4150  s21a.pdf) |..|AP
-00002c50: 533c 7375 703e f09f 908c 3c2f 7375 703e  S<sup>....</sup>
-00002c60: 7c20 536b 696c 6c20 4469 7363 6f76 6572  | Skill Discover
-00002c70: 7920 7c20 e29c 94ef b88f 207c 20e2 9c94  y | ...... | ...
-00002c80: efb8 8f20 7c20 5b41 5053 3a20 4163 7469  ... | [APS: Acti
-00002c90: 7665 2050 7265 7472 6169 6e69 6e67 2077  ve Pretraining w
-00002ca0: 6974 6820 5375 6363 6573 736f 7220 4665  ith Successor Fe
-00002cb0: 6174 7572 6573 5d28 6874 7470 3a2f 2f70  atures](http://p
-00002cc0: 726f 6365 6564 696e 6773 2e6d 6c72 2e70  roceedings.mlr.p
-00002cd0: 7265 7373 2f76 3133 392f 6c69 7532 3162  ress/v139/liu21b
-00002ce0: 2f6c 6975 3231 622e 7064 6629 207c 0d0a  /liu21b.pdf) |..
-00002cf0: 0d0a 3e20 2d20 f09f 908c 3a20 4465 7665  ..> - ....: Deve
-00002d00: 6c6f 7069 6e67 2e0d 0a3e 202d 2060 5265  loping...> - `Re
-00002d10: 7072 2e60 3a20 5468 6520 6d65 7468 6f64  pr.`: The method
-00002d20: 2069 6e76 6f6c 7665 7320 7265 7072 6573   involves repres
-00002d30: 656e 7461 7469 6f6e 206c 6561 726e 696e  entation learnin
-00002d40: 672e 0d0a 3e20 2d20 6056 6973 7561 6c60  g...> - `Visual`
-00002d50: 3a20 5468 6520 6d65 7468 6f64 2077 6f72  : The method wor
-00002d60: 6b73 2077 656c 6c20 696e 2076 6973 7561  ks well in visua
-00002d70: 6c20 524c 2e0d 0a0d 0a23 204d 6f64 656c  l RL.....# Model
-00002d80: 205a 6f6f 0d0a 4873 7561 6e77 7520 7072   Zoo..Hsuanwu pr
-00002d90: 6f76 6964 6573 2061 206c 6172 6765 206e  ovides a large n
-00002da0: 756d 6265 7220 6f66 2072 6575 7361 626c  umber of reusabl
-00002db0: 6520 6265 6368 6d61 726b 732c 2073 6565  e bechmarks, see
-00002dc0: 205b 6874 7470 733a 2f2f 6875 622e 6873   [https://hub.hs
-00002dd0: 7561 6e77 752e 6465 762f 5d28 6874 7470  uanwu.dev/](http
-00002de0: 733a 2f2f 6875 622e 6873 7561 6e77 752e  s://hub.hsuanwu.
-00002df0: 6465 762f 290d 0a0d 0a23 2041 5049 2044  dev/)....# API D
-00002e00: 6f63 756d 656e 7461 7469 6f6e 0d0a 5669  ocumentation..Vi
-00002e10: 6577 206f 7572 2077 656c 6c2d 6465 7369  ew our well-desi
-00002e20: 676e 6564 2064 6f63 756d 656e 7461 7469  gned documentati
-00002e30: 6f6e 3a20 5b68 7474 7073 3a2f 2f64 6f63  on: [https://doc
-00002e40: 732e 6873 7561 6e77 752e 6465 762f 5d28  s.hsuanwu.dev/](
-00002e50: 6874 7470 733a 2f2f 646f 6373 2e68 7375  https://docs.hsu
-00002e60: 616e 7775 2e64 6576 2f29 0d0a 0d0a 2320  anwu.dev/)....# 
-00002e70: 486f 7720 546f 2043 6f6e 7472 6962 7574  How To Contribut
-00002e80: 650d 0a57 656c 636f 6d65 2074 6f20 636f  e..Welcome to co
-00002e90: 6e74 7269 6275 7465 2074 6f20 7468 6973  ntribute to this
-00002ea0: 2070 726f 6a65 6374 2120 4265 666f 7265   project! Before
-00002eb0: 2079 6f75 2062 6567 696e 2077 7269 7469   you begin writi
-00002ec0: 6e67 2063 6f64 652c 2070 6c65 6173 6520  ng code, please 
-00002ed0: 7265 6164 205b 434f 4e54 5249 4255 5449  read [CONTRIBUTI
-00002ee0: 4e47 2e6d 645d 2868 7474 7073 3a2f 2f67  NG.md](https://g
-00002ef0: 6974 6875 622e 636f 6d2f 524c 452d 466f  ithub.com/RLE-Fo
-00002f00: 756e 6461 7469 6f6e 2f48 7375 616e 7775  undation/Hsuanwu
-00002f10: 2f62 6c6f 622f 6d61 696e 2f43 4f4e 5452  /blob/main/CONTR
-00002f20: 4942 5554 494e 472e 6d64 2920 666f 7220  IBUTING.md) for 
-00002f30: 6775 6964 6520 6669 7273 742e 0d0a 0d0a  guide first.....
-00002f40: 2320 4163 6b6e 6f77 6c65 6467 6d65 6e74  # Acknowledgment
-00002f50: 0d0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
-00002f60: 7320 7375 7070 6f72 7465 6420 6279 205b  s supported by [
-00002f70: 4655 4e44 494e 472e 796d 6c5d 2868 7474  FUNDING.yml](htt
-00002f80: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002f90: 524c 452d 466f 756e 6461 7469 6f6e 2f48  RLE-Foundation/H
-00002fa0: 7375 616e 7775 2f62 6c6f 622f 6d61 696e  suanwu/blob/main
-00002fb0: 2f2e 6769 7468 7562 2f46 554e 4449 4e47  /.github/FUNDING
-00002fc0: 2e79 6d6c 292e 2053 6f6d 6520 636f 6465  .yml). Some code
-00002fd0: 206f 6620 7468 6973 2070 726f 6a65 6374   of this project
-00002fe0: 2069 7320 626f 7272 6f77 6564 206f 7220   is borrowed or 
-00002ff0: 696e 7370 6972 6564 2062 7920 7365 7665  inspired by seve
-00003000: 7261 6c20 6578 6365 6c6c 656e 7420 7072  ral excellent pr
-00003010: 6f6a 6563 7473 2c20 616e 6420 7765 2068  ojects, and we h
-00003020: 6967 686c 7920 6170 7072 6563 6961 7465  ighly appreciate
-00003030: 2074 6865 6d2e 2053 6565 205b 4143 4b4e   them. See [ACKN
-00003040: 4f57 4c45 4447 4d45 4e54 2e6d 645d 2868  OWLEDGMENT.md](h
-00003050: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003060: 6d2f 524c 452d 466f 756e 6461 7469 6f6e  m/RLE-Foundation
-00003070: 2f48 7375 616e 7775 2f62 6c6f 622f 6d61  /Hsuanwu/blob/ma
-00003080: 696e 2f41 434b 4e4f 574c 4544 474d 454e  in/ACKNOWLEDGMEN
-00003090: 542e 6d64 292e 0d0a                      T.md)...
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6873 7561  : 2.1.Name: hsua
+00000020: 6e77 750a 5665 7273 696f 6e3a 2030 2e30  nwu.Version: 0.0
+00000030: 2e31 6235 0a53 756d 6d61 7279 3a20 4c6f  .1b5.Summary: Lo
+00000040: 6e67 2d54 6572 6d20 4576 6f6c 7574 696f  ng-Term Evolutio
+00000050: 6e20 5072 6f6a 6563 7420 6f66 2052 6569  n Project of Rei
+00000060: 6e66 6f72 6365 6d65 6e74 204c 6561 726e  nforcement Learn
+00000070: 696e 670a 5072 6f6a 6563 742d 5552 4c3a  ing.Project-URL:
+00000080: 2043 6f64 652c 2068 7474 7073 3a2f 2f67   Code, https://g
+00000090: 6974 6875 622e 636f 6d2f 524c 452d 466f  ithub.com/RLE-Fo
+000000a0: 756e 6461 7469 6f6e 2f48 7375 616e 7775  undation/Hsuanwu
+000000b0: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
+000000c0: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
+000000d0: 7073 3a2f 2f64 6f63 732e 6873 7561 6e77  ps://docs.hsuanw
+000000e0: 752e 6465 762f 0a50 726f 6a65 6374 2d55  u.dev/.Project-U
+000000f0: 524c 3a20 4265 6e63 686d 6172 6b2c 2068  RL: Benchmark, h
+00000100: 7474 7073 3a2f 2f68 7562 2e68 7375 616e  ttps://hub.hsuan
+00000110: 7775 2e64 6576 2f0a 5072 6f6a 6563 742d  wu.dev/.Project-
+00000120: 5552 4c3a 2042 7567 2054 7261 636b 6572  URL: Bug Tracker
+00000130: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+00000140: 2e63 6f6d 2f52 4c45 2d46 6f75 6e64 6174  .com/RLE-Foundat
+00000150: 696f 6e2f 4873 7561 6e77 752f 6973 7375  ion/Hsuanwu/issu
+00000160: 6573 0a41 7574 686f 722d 656d 6169 6c3a  es.Author-email:
+00000170: 2052 6569 6e66 6f72 6365 6d65 6e74 204c   Reinforcement L
+00000180: 6561 726e 696e 6720 4576 6f6c 7574 696f  earning Evolutio
+00000190: 6e20 466f 756e 6461 7469 6f6e 203c 6672  n Foundation <fr
+000001a0: 6965 6472 6963 6879 7561 6e31 3939 3930  iedrichyuan19990
+000001b0: 3832 3740 676d 6169 6c2e 636f 6d3e 0a4c  827@gmail.com>.L
+000001c0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
+000001d0: 454e 5345 0a4b 6579 776f 7264 733a 2041  ENSE.Keywords: A
+000001e0: 6c67 6f72 6974 686d 2c42 6173 656c 696e  lgorithm,Baselin
+000001f0: 652c 4576 6f6c 7574 696f 6e2c 5265 696e  e,Evolution,Rein
+00000200: 666f 7263 656d 656e 7420 4c65 6172 6e69  forcement Learni
+00000210: 6e67 0a43 6c61 7373 6966 6965 723a 204c  ng.Classifier: L
+00000220: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000230: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000240: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
+00000250: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
+00000260: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000270: 6465 6e74 0a43 6c61 7373 6966 6965 723a  dent.Classifier:
+00000280: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000290: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002a0: 3a3a 2033 0a52 6571 7569 7265 732d 5079  :: 3.Requires-Py
+000002b0: 7468 6f6e 3a20 3e3d 332e 380a 5265 7175  thon: >=3.8.Requ
+000002c0: 6972 6573 2d44 6973 743a 2061 7263 683d  ires-Dist: arch=
+000002d0: 3d35 2e33 2e30 0a52 6571 7569 7265 732d  =5.3.0.Requires-
+000002e0: 4469 7374 3a20 6779 6d6e 6173 6975 6d5b  Dist: gymnasium[
+000002f0: 6163 6365 7074 2d72 6f6d 2d6c 6963 656e  accept-rom-licen
+00000300: 7365 5d3d 3d30 2e32 382e 310a 5265 7175  se]==0.28.1.Requ
+00000310: 6972 6573 2d44 6973 743a 2068 7964 7261  ires-Dist: hydra
+00000320: 2d63 6f72 653d 3d31 2e33 2e32 0a52 6571  -core==1.3.2.Req
+00000330: 7569 7265 732d 4469 7374 3a20 6879 6472  uires-Dist: hydr
+00000340: 612d 7375 626d 6974 6974 2d6c 6175 6e63  a-submitit-launc
+00000350: 6865 723d 3d31 2e32 2e30 0a52 6571 7569  her==1.2.0.Requi
+00000360: 7265 732d 4469 7374 3a20 6f70 656e 6376  res-Dist: opencv
+00000370: 2d70 7974 686f 6e0a 5265 7175 6972 6573  -python.Requires
+00000380: 2d44 6973 743a 2073 6369 7079 3e3d 312e  -Dist: scipy>=1.
+00000390: 372e 300a 5265 7175 6972 6573 2d44 6973  7.0.Requires-Dis
+000003a0: 743a 2074 656e 736f 7262 6f61 7264 780a  t: tensorboardx.
+000003b0: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+000003c0: 6572 6d63 6f6c 6f72 0a52 6571 7569 7265  ermcolor.Require
+000003d0: 732d 4469 7374 3a20 746f 7263 683d 3d32  s-Dist: torch==2
+000003e0: 2e30 2e30 0a52 6571 7569 7265 732d 4469  .0.0.Requires-Di
+000003f0: 7374 3a20 746f 7263 6876 6973 696f 6e3d  st: torchvision=
+00000400: 3d30 2e31 352e 310a 5072 6f76 6964 6573  =0.15.1.Provides
+00000410: 2d45 7874 7261 3a20 646f 6373 0a52 6571  -Extra: docs.Req
+00000420: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
+00000430: 6373 2d6d 6174 6572 6961 6c3b 2065 7874  cs-material; ext
+00000440: 7261 203d 3d20 2764 6f63 7327 0a52 6571  ra == 'docs'.Req
+00000450: 7569 7265 732d 4469 7374 3a20 6d6b 6765  uires-Dist: mkge
+00000460: 6e64 6f63 733b 2065 7874 7261 203d 3d20  ndocs; extra == 
+00000470: 2764 6f63 7327 0a50 726f 7669 6465 732d  'docs'.Provides-
+00000480: 4578 7472 613a 2065 6e76 730a 5265 7175  Extra: envs.Requ
+00000490: 6972 6573 2d44 6973 743a 2061 6c65 2d70  ires-Dist: ale-p
+000004a0: 793d 3d30 2e38 2e31 3b20 6578 7472 6120  y==0.8.1; extra 
+000004b0: 3d3d 2027 656e 7673 270a 5265 7175 6972  == 'envs'.Requir
+000004c0: 6573 2d44 6973 743a 2064 6d2d 636f 6e74  es-Dist: dm-cont
+000004d0: 726f 6c3d 3d31 2e30 2e31 313b 2065 7874  rol==1.0.11; ext
+000004e0: 7261 203d 3d20 2765 6e76 7327 0a52 6571  ra == 'envs'.Req
+000004f0: 7569 7265 732d 4469 7374 3a20 6779 6d3d  uires-Dist: gym=
+00000500: 3d30 2e32 312e 303b 2065 7874 7261 203d  =0.21.0; extra =
+00000510: 3d20 2765 6e76 7327 0a52 6571 7569 7265  = 'envs'.Require
+00000520: 732d 4469 7374 3a20 6779 6d6e 6173 6975  s-Dist: gymnasiu
+00000530: 6d5b 6163 6365 7074 2d72 6f6d 2d6c 6963  m[accept-rom-lic
+00000540: 656e 7365 5d3b 2065 7874 7261 203d 3d20  ense]; extra == 
+00000550: 2765 6e76 7327 0a52 6571 7569 7265 732d  'envs'.Requires-
+00000560: 4469 7374 3a20 696d 6167 6569 6f3b 2065  Dist: imageio; e
+00000570: 7874 7261 203d 3d20 2765 6e76 7327 0a52  xtra == 'envs'.R
+00000580: 6571 7569 7265 732d 4469 7374 3a20 6d69  equires-Dist: mi
+00000590: 6e69 6772 6964 3b20 6578 7472 6120 3d3d  nigrid; extra ==
+000005a0: 2027 656e 7673 270a 5265 7175 6972 6573   'envs'.Requires
+000005b0: 2d44 6973 743a 2070 726f 6367 656e 3d3d  -Dist: procgen==
+000005c0: 302e 3130 2e37 3b20 6578 7472 6120 3d3d  0.10.7; extra ==
+000005d0: 2027 656e 7673 270a 5265 7175 6972 6573   'envs'.Requires
+000005e0: 2d44 6973 743a 2073 6369 6b69 742d 696d  -Dist: scikit-im
+000005f0: 6167 653b 2065 7874 7261 203d 3d20 2765  age; extra == 'e
+00000600: 6e76 7327 0a52 6571 7569 7265 732d 4469  nvs'.Requires-Di
+00000610: 7374 3a20 7363 696b 6974 2d76 6964 656f  st: scikit-video
+00000620: 3b20 6578 7472 6120 3d3d 2027 656e 7673  ; extra == 'envs
+00000630: 270a 5072 6f76 6964 6573 2d45 7874 7261  '.Provides-Extra
+00000640: 3a20 7465 7374 730a 5265 7175 6972 6573  : tests.Requires
+00000650: 2d44 6973 743a 2062 6c61 636b 3b20 6578  -Dist: black; ex
+00000660: 7472 6120 3d3d 2027 7465 7374 7327 0a52  tra == 'tests'.R
+00000670: 6571 7569 7265 732d 4469 7374 3a20 6275  equires-Dist: bu
+00000680: 696c 642d 302d 3130 2d30 3b20 6578 7472  ild-0-10-0; extr
+00000690: 6120 3d3d 2027 7465 7374 7327 0a52 6571  a == 'tests'.Req
+000006a0: 7569 7265 732d 4469 7374 3a20 6973 6f72  uires-Dist: isor
+000006b0: 743e 3d35 2e30 3b20 6578 7472 6120 3d3d  t>=5.0; extra ==
+000006c0: 2027 7465 7374 7327 0a52 6571 7569 7265   'tests'.Require
+000006d0: 732d 4469 7374 3a20 7079 7465 7374 3b20  s-Dist: pytest; 
+000006e0: 6578 7472 6120 3d3d 2027 7465 7374 7327  extra == 'tests'
+000006f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000700: 7079 7465 7374 2d63 6f76 3b20 6578 7472  pytest-cov; extr
+00000710: 6120 3d3d 2027 7465 7374 7327 0a52 6571  a == 'tests'.Req
+00000720: 7569 7265 732d 4469 7374 3a20 7079 7465  uires-Dist: pyte
+00000730: 7374 2d65 6e76 3b20 6578 7472 6120 3d3d  st-env; extra ==
+00000740: 2027 7465 7374 7327 0a52 6571 7569 7265   'tests'.Require
+00000750: 732d 4469 7374 3a20 7079 7465 7374 2d78  s-Dist: pytest-x
+00000760: 6469 7374 3b20 6578 7472 6120 3d3d 2027  dist; extra == '
+00000770: 7465 7374 7327 0a52 6571 7569 7265 732d  tests'.Requires-
+00000780: 4469 7374 3a20 7079 7479 7065 3b20 6578  Dist: pytype; ex
+00000790: 7472 6120 3d3d 2027 7465 7374 7327 0a52  tra == 'tests'.R
+000007a0: 6571 7569 7265 732d 4469 7374 3a20 7275  equires-Dist: ru
+000007b0: 6666 3b20 6578 7472 6120 3d3d 2027 7465  ff; extra == 'te
+000007c0: 7374 7327 0a44 6573 6372 6970 7469 6f6e  sts'.Description
+000007d0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000007e0: 6578 742f 6d61 726b 646f 776e 0a0a 3c64  ext/markdown..<d
+000007f0: 6976 2061 6c69 676e 3d63 656e 7465 723e  iv align=center>
+00000800: 0a3c 696d 6720 7372 633d 272e 2f64 6f63  .<img src='./doc
+00000810: 732f 6173 7365 7473 2f69 6d61 6765 732f  s/assets/images/
+00000820: 6c6f 676f 2e70 6e67 2720 7374 796c 653d  logo.png' style=
+00000830: 2277 6964 7468 3a20 3730 2522 3e0a 3c2f  "width: 70%">.</
+00000840: 6469 763e 0a0a 7c3c 696d 6720 7372 633d  div>..|<img src=
+00000850: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000860: 656c 6473 2e69 6f2f 6261 6467 652f 4c69  elds.io/badge/Li
+00000870: 6365 6e73 652d 4d49 542d 2532 3330 3637  cense-MIT-%23067
+00000880: 3762 3822 3e20 3c69 6d67 2073 7263 3d22  7b8"> <img src="
+00000890: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000008a0: 6c64 732e 696f 2f62 6164 6765 2f47 5055  lds.io/badge/GPU
+000008b0: 2d4e 5649 4449 412d 2532 3337 3762 3930  -NVIDIA-%2377b90
+000008c0: 3022 3e20 3c69 6d67 2073 7263 3d22 6874  0"> <img src="ht
+000008d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000008e0: 732e 696f 2f62 6164 6765 2f4e 5055 2d41  s.io/badge/NPU-A
+000008f0: 7363 656e 642d 2532 3363 3331 6432 3022  scend-%23c31d20"
+00000900: 3e20 3c69 6d67 2073 7263 3d22 6874 7470  > <img src="http
+00000910: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000920: 696f 2f62 6164 6765 2f50 7974 686f 6e2d  io/badge/Python-
+00000930: 2533 4525 3344 332e 382d 2532 3333 3537  %3E%3D3.8-%23357
+00000940: 3039 4622 3e20 3c69 6d67 2073 7263 3d22  09F"> <img src="
+00000950: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000960: 6c64 732e 696f 2f62 6164 6765 2f44 6f63  lds.io/badge/Doc
+00000970: 732d 5061 7373 696e 672d 2532 3330 3039  s-Passing-%23009
+00000980: 3438 3522 3e20 3c69 6d67 2073 7263 3d22  485"> <img src="
+00000990: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000009a0: 6c64 732e 696f 2f62 6164 6765 2f43 6f64  lds.io/badge/Cod
+000009b0: 6573 7479 6c65 2d42 6c61 636b 2d62 6c61  estyle-Black-bla
+000009c0: 636b 223e 203c 696d 6720 7372 633d 2268  ck"> <img src="h
+000009d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000009e0: 6473 2e69 6f2f 6261 6467 652f 5079 5049  ds.io/badge/PyPI
+000009f0: 2532 3050 6163 6b61 6765 2d30 2e30 2e31  %20Package-0.0.1
+00000a00: 2d25 3233 3030 3644 4144 223e 203c 696d  -%23006DAD"> <im
+00000a10: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000a20: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000a30: 6467 652f f09f a497 4265 6e63 686d 6172  dge/....Benchmar
+00000a40: 6b2d 4875 6767 696e 6746 6163 652d 2532  k-HuggingFace-%2
+00000a50: 3346 4644 3231 4522 3e20 3c69 6d67 2073  3FFD21E"> <img s
+00000a60: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000a70: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000a80: 2f50 7974 6f72 6368 2d25 3345 2533 4432  /Pytorch-%3E%3D2
+00000a90: 2e30 2e30 2d25 3233 4546 3537 3339 223e  .0.0-%23EF5739">
+00000aa0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000ab0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000ac0: 6f2f 6261 6467 652f 4879 6472 612d 312e  o/badge/Hydra-1.
+00000ad0: 332e 322d 2532 3345 3838 3434 3422 3e20  3.2-%23E88444"> 
+00000ae0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000af0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000b00: 2f62 6164 6765 2f47 796d 6e61 7369 756d  /badge/Gymnasium
+00000b10: 2d25 3345 2533 4430 2e32 382e 312d 6272  -%3E%3D0.28.1-br
+00000b20: 6967 6874 6772 6565 6e22 3e20 3c69 6d67  ightgreen"> <img
+00000b30: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000b40: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000b50: 6765 2f44 4d43 2053 7569 7465 2d31 2e30  ge/DMC Suite-1.0
+00000b60: 2e31 312d 626c 7565 223e 203c 696d 6720  .11-blue"> <img 
+00000b70: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000b80: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000b90: 652f 5072 6f63 6765 6e2d 302e 3130 2e37  e/Procgen-0.10.7
+00000ba0: 2d62 6c75 6576 696f 6c65 7422 3e20 3c69  -blueviolet"> <i
+00000bb0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000bc0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000bd0: 6164 6765 2f32 2e32 2e31 2d4d 696e 6947  adge/2.2.1-MiniG
+00000be0: 7269 642d 2532 3363 3863 3863 3822 3e20  rid-%23c8c8c8"> 
+00000bf0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000c00: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000c10: 2f62 6164 6765 2f50 7942 756c 6c65 742d  /badge/PyBullet-
+00000c20: 332e 322e 352d 2532 3336 4139 3444 3422  3.2.5-%236A94D4"
+00000c30: 3e7c 0a7c 3a2d 3a7c 0a0a 2a2a 4873 7561  >|.|:-:|..**Hsua
+00000c40: 6e77 753a 204c 6f6e 672d 5465 726d 2045  nwu: Long-Term E
+00000c50: 766f 6c75 7469 6f6e 2050 726f 6a65 6374  volution Project
+00000c60: 206f 6620 5265 696e 666f 7263 656d 656e   of Reinforcemen
+00000c70: 7420 4c65 6172 6e69 6e67 2a2a 2069 7320  t Learning** is 
+00000c80: 696e 7370 6972 6564 2062 7920 7468 6520  inspired by the 
+00000c90: 6c6f 6e67 2d74 6572 6d20 6576 6f6c 7574  long-term evolut
+00000ca0: 696f 6e20 284c 5445 2920 7374 616e 6461  ion (LTE) standa
+00000cb0: 7264 2070 726f 6a65 6374 2069 6e20 7465  rd project in te
+00000cc0: 6c65 636f 6d6d 756e 6963 6174 696f 6e73  lecommunications
+00000cd0: 2c20 7768 6963 6820 6169 6d73 2074 6f20  , which aims to 
+00000ce0: 7472 6163 6b20 7468 6520 6c61 7465 7374  track the latest
+00000cf0: 2072 6573 6561 7263 6820 7072 6f67 7265   research progre
+00000d00: 7373 2069 6e20 7265 696e 666f 7263 656d  ss in reinforcem
+00000d10: 656e 7420 6c65 6172 6e69 6e67 2028 524c  ent learning (RL
+00000d20: 2920 616e 6420 7072 6f76 6964 6520 7374  ) and provide st
+00000d30: 6162 6c65 2061 6e64 2065 6666 6963 6965  able and efficie
+00000d40: 6e74 2062 6173 656c 696e 6573 2e20 496e  nt baselines. In
+00000d50: 2048 7375 616e 7775 2c20 796f 7520 6361   Hsuanwu, you ca
+00000d60: 6e20 6669 6e64 2065 7665 7279 7468 696e  n find everythin
+00000d70: 6720 796f 7520 6e65 6564 2069 6e20 524c  g you need in RL
+00000d80: 2c20 7375 6368 2061 7320 7472 6169 6e69  , such as traini
+00000d90: 6e67 2c20 6576 616c 7561 7469 6f6e 2c20  ng, evaluation, 
+00000da0: 6465 706c 6f79 6d65 6e74 2c20 6574 632e  deployment, etc.
+00000db0: 2054 6865 2068 6967 686c 6967 6874 2066   The highlight f
+00000dc0: 6561 7475 7265 7320 6f66 2048 7375 616e  eatures of Hsuan
+00000dd0: 7775 3a0a 0a2d 20e2 8fb1 efb8 8f20 4c61  wu:..- ...... La
+00000de0: 7465 7374 2061 6c67 6f72 6974 686d 7320  test algorithms 
+00000df0: 616e 6420 7472 6963 6b73 3b0a 2d20 f09f  and tricks;.- ..
+00000e00: a7b1 2048 6967 686c 7920 6d6f 6475 6c61  .. Highly modula
+00000e10: 7269 7a65 6420 6465 7369 676e 2066 6f72  rized design for
+00000e20: 2063 6f6d 706c 6574 6520 6465 636f 7570   complete decoup
+00000e30: 6c69 6e67 206f 6620 524c 2061 6c67 6f72  ling of RL algor
+00000e40: 6974 686d 733b 0a2d 20f0 9f9a 8020 4f70  ithms;.- .... Op
+00000e50: 7469 6d69 7a65 6420 776f 726b 666c 6f77  timized workflow
+00000e60: 2066 6f72 2066 756c 6c20 6861 7264 7761   for full hardwa
+00000e70: 7265 2061 6363 656c 6572 6174 696f 6e3b  re acceleration;
+00000e80: 0a2d 20e2 9a99 efb8 8f20 5375 7070 6f72  .- ...... Suppor
+00000e90: 7420 666f 7220 6375 7374 6f6d 2065 6e76  t for custom env
+00000ea0: 6972 6f6e 6d65 6e74 733b 0a2d 20f0 9f96  ironments;.- ...
+00000eb0: a5ef b88f 2053 7570 706f 7274 2066 6f72  .... Support for
+00000ec0: 206d 756c 7469 706c 6520 636f 6d70 7574   multiple comput
+00000ed0: 696e 6720 6465 7669 6365 7320 6c69 6b65  ing devices like
+00000ee0: 2047 5055 2061 6e64 204e 5055 3b0a 2d20   GPU and NPU;.- 
+00000ef0: f09f 9ba0 efb8 8f20 5375 7070 6f72 7420  ....... Support 
+00000f00: 666f 7220 524c 206d 6f64 656c 2065 6e67  for RL model eng
+00000f10: 696e 6565 7269 6e67 2064 6570 6c6f 796d  ineering deploym
+00000f20: 656e 7420 2854 656e 736f 7252 542c 2043  ent (TensorRT, C
+00000f30: 414e 4e2c 202e 2e2e 293b 0a2d 20f0 9f92  ANN, ...);.- ...
+00000f40: be20 4c61 7267 6520 6e75 6d62 6572 206f  . Large number o
+00000f50: 6620 7265 7573 6162 6c65 2062 6563 686d  f reusable bechm
+00000f60: 6172 6b73 2028 5b53 6565 2048 7375 616e  arks ([See Hsuan
+00000f70: 7775 4875 625d 2868 7562 2e68 7375 616e  wuHub](hub.hsuan
+00000f80: 7775 2e64 6576 2929 3b0a 2d20 f09f 938b  wu.dev));.- ....
+00000f90: 2045 6c65 6761 6e74 2065 7870 6572 696d   Elegant experim
+00000fa0: 656e 7461 6c20 6d61 6e61 6765 6d65 6e74  ental management
+00000fb0: 2070 6f77 6572 6564 2062 7920 5b48 7964   powered by [Hyd
+00000fc0: 7261 5d28 6874 7470 733a 2f2f 6879 6472  ra](https://hydr
+00000fd0: 612e 6363 2f29 2e0a 0a4a 6f69 6e20 7468  a.cc/)...Join th
+00000fe0: 6520 6465 7665 6c6f 7065 7220 636f 6d6d  e developer comm
+00000ff0: 756e 6974 7920 666f 7220 6973 7375 6573  unity for issues
+00001000: 2061 6e64 2064 6973 6375 7373 696f 6e73   and discussions
+00001010: 3a0a 7c53 6c61 636b 7c51 517c 4769 7448  :.|Slack|QQ|GitH
+00001020: 7562 7c0a 7c3a 2d3a 7c3a 2d3a 7c3a 2d3a  ub|.|:-:|:-:|:-:
+00001030: 7c0a 7c3c 6120 6872 6566 3d22 6874 7470  |.|<a href="http
+00001040: 733a 2f2f 6170 702e 736c 6163 6b2e 636f  s://app.slack.co
+00001050: 6d2f 636c 6965 6e74 2f54 3035 344a 344e  m/client/T054J4N
+00001060: 4a58 5030 2f43 3035 3454 3738 515a 3941  JXP0/C054T78QZ9A
+00001070: 223e 3c69 6d67 2073 7263 3d27 2e2f 646f  "><img src='./do
+00001080: 6373 2f61 7373 6574 732f 696d 6167 6573  cs/assets/images
+00001090: 2f73 6c61 636b 2e70 6e67 2720 7374 796c  /slack.png' styl
+000010a0: 653d 2277 6964 7468 3a20 3530 2522 203e  e="width: 50%" >
+000010b0: 3c2f 613e 7c3c 696d 6720 7372 633d 272e  </a>|<img src='.
+000010c0: 2f64 6f63 732f 6173 7365 7473 2f69 6d61  /docs/assets/ima
+000010d0: 6765 732f 7171 2e6a 7067 2720 7374 796c  ges/qq.jpg' styl
+000010e0: 653d 2277 6964 7468 3a20 3635 2522 3e7c  e="width: 65%">|
+000010f0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001100: 2f67 6974 6875 622e 636f 6d2f 524c 452d  /github.com/RLE-
+00001110: 466f 756e 6461 7469 6f6e 2f48 7375 616e  Foundation/Hsuan
+00001120: 7775 2f69 7373 7565 7322 3e3c 696d 6720  wu/issues"><img 
+00001130: 7372 633d 272e 2f64 6f63 732f 6173 7365  src='./docs/asse
+00001140: 7473 2f69 6d61 6765 732f 6769 7468 7562  ts/images/github
+00001150: 5f69 7373 7565 732e 706e 6727 2073 7479  _issues.png' sty
+00001160: 6c65 3d22 7769 6474 683a 2035 3025 223e  le="width: 50%">
+00001170: 3c2f 613e 7c0a 0a0a 0a3c 212d 2d20 506c  </a>|....<!-- Pl
+00001180: 6561 7365 2063 6974 6520 7468 6520 666f  ease cite the fo
+00001190: 6c6c 6f77 696e 6720 7061 7065 7220 6966  llowing paper if
+000011a0: 2079 6f75 2075 7365 2048 7375 616e 7775   you use Hsuanwu
+000011b0: 2069 6e20 796f 7572 2077 6f72 6b2c 2074   in your work, t
+000011c0: 6861 6e6b 2079 6f75 210a 6060 6062 6962  hank you!.```bib
+000011d0: 7465 780a 4061 7274 6963 6c65 7b79 7561  tex.@article{yua
+000011e0: 6e32 3032 3368 7375 616e 7775 2c0a 2020  n2023hsuanwu,.  
+000011f0: 7469 746c 653d 7b48 7375 616e 7775 3a20  title={Hsuanwu: 
+00001200: 4c6f 6e67 2d54 6572 6d20 4576 6f6c 7574  Long-Term Evolut
+00001210: 696f 6e20 5072 6f6a 6563 7420 6f66 2052  ion Project of R
+00001220: 6569 6e66 6f72 6365 6d65 6e74 204c 6561  einforcement Lea
+00001230: 726e 696e 677d 2c0a 2020 6175 7468 6f72  rning},.  author
+00001240: 3d7b 5975 616e 2c20 4d69 6e67 7169 2061  ={Yuan, Mingqi a
+00001250: 6e64 204c 756f 2c20 5368 6968 616f 2061  nd Luo, Shihao a
+00001260: 6e64 205a 6861 6e67 2c20 5a65 7175 6e20  nd Zhang, Zequn 
+00001270: 616e 6420 5961 6e67 2c20 5875 2061 6e64  and Yang, Xu and
+00001280: 204a 696e 2c20 5869 6e20 616e 6420 4c69   Jin, Xin and Li
+00001290: 2c20 426f 2061 6e64 205a 656e 672c 2057  , Bo and Zeng, W
+000012a0: 656e 6a75 6e7d 2c0a 2020 6a6f 7572 6e61  enjun},.  journa
+000012b0: 6c3d 7b61 7258 6976 2070 7265 7072 696e  l={arXiv preprin
+000012c0: 7420 6172 5869 763a 3233 3131 2e31 3532  t arXiv:2311.152
+000012d0: 3737 7d2c 0a20 2079 6561 723d 7b32 3032  77},.  year={202
+000012e0: 337d 0a7d 0a60 6060 202d 2d3e 0a0a 2d20  3}.}.``` -->..- 
+000012f0: 5b51 7569 636b 2053 7461 7274 5d28 2371  [Quick Start](#q
+00001300: 7569 636b 2d73 7461 7274 290a 2020 2d20  uick-start).  - 
+00001310: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
+00001320: 696e 7374 616c 6c61 7469 6f6e 290a 2020  installation).  
+00001330: 2d20 5b42 7569 6c64 2079 6f75 7220 6669  - [Build your fi
+00001340: 7273 7420 4873 7561 6e77 7520 6170 706c  rst Hsuanwu appl
+00001350: 6963 6174 696f 6e5d 2823 6275 696c 642d  ication](#build-
+00001360: 796f 7572 2d66 6972 7374 2d68 7375 616e  your-first-hsuan
+00001370: 7775 2d61 7070 6c69 6361 7469 6f6e 290a  wu-application).
+00001380: 2d20 5b49 6d70 6c65 6d65 6e74 6564 204d  - [Implemented M
+00001390: 6f64 756c 6573 5d28 2369 6d70 6c65 6d65  odules](#impleme
+000013a0: 6e74 6564 2d6d 6f64 756c 6573 290a 2020  nted-modules).  
+000013b0: 2d20 5b52 6f61 646d 6170 5d28 2372 6f61  - [Roadmap](#roa
+000013c0: 646d 6170 290a 2020 2d20 5b50 726f 6a65  dmap).  - [Proje
+000013d0: 6374 2053 7472 7563 7475 7265 5d28 2370  ct Structure](#p
+000013e0: 726f 6a65 6374 2d73 7472 7563 7475 7265  roject-structure
+000013f0: 290a 2020 2d20 5b52 4c20 4167 656e 7473  ).  - [RL Agents
+00001400: 5d28 2372 6c2d 6167 656e 7473 290a 2020  ](#rl-agents).  
+00001410: 2d20 5b49 6e74 7269 6e73 6963 2052 6577  - [Intrinsic Rew
+00001420: 6172 6420 4d6f 6475 6c65 735d 2823 696e  ard Modules](#in
+00001430: 7472 696e 7369 632d 7265 7761 7264 2d6d  trinsic-reward-m
+00001440: 6f64 756c 6573 290a 2d20 5b4d 6f64 656c  odules).- [Model
+00001450: 205a 6f6f 5d28 236d 6f64 656c 2d7a 6f6f   Zoo](#model-zoo
+00001460: 290a 2d20 5b41 5049 2044 6f63 756d 656e  ).- [API Documen
+00001470: 7461 7469 6f6e 5d28 2361 7069 2d64 6f63  tation](#api-doc
+00001480: 756d 656e 7461 7469 6f6e 290a 2d20 5b48  umentation).- [H
+00001490: 6f77 2054 6f20 436f 6e74 7269 6275 7465  ow To Contribute
+000014a0: 5d28 2368 6f77 2d74 6f2d 636f 6e74 7269  ](#how-to-contri
+000014b0: 6275 7465 290a 2d20 5b41 636b 6e6f 776c  bute).- [Acknowl
+000014c0: 6564 676d 656e 745d 2823 6163 6b6e 6f77  edgment](#acknow
+000014d0: 6c65 6467 6d65 6e74 290a 0a23 2051 7569  ledgment)..# Qui
+000014e0: 636b 2053 7461 7274 0a23 2320 496e 7374  ck Start.## Inst
+000014f0: 616c 6c61 7469 6f6e 0a2d 2050 7265 7265  allation.- Prere
+00001500: 7175 6973 6974 6573 0a0a 4375 7272 656e  quisites..Curren
+00001510: 746c 792c 2048 7375 616e 7775 2072 6571  tly, Hsuanwu req
+00001520: 7569 7265 7320 6050 7974 686f 6e3e 3d33  uires `Python>=3
+00001530: 2e38 602c 2075 7365 7220 6361 6e20 6372  .8`, user can cr
+00001540: 6561 7465 2061 6e20 7669 7274 7561 6c20  eate an virtual 
+00001550: 656e 7669 726f 6e6d 656e 7420 6279 0a60  environment by.`
+00001560: 6060 2073 680a 636f 6e64 6120 6372 6561  `` sh.conda crea
+00001570: 7465 202d 6e20 6873 7561 6e77 7520 7079  te -n hsuanwu py
+00001580: 7468 6f6e 3d33 2e38 0a60 6060 0a0a 2d20  thon=3.8.```..- 
+00001590: 7769 7468 2070 6970 2060 7265 636f 6d6d  with pip `recomm
+000015a0: 656e 6465 6460 0a0a 4f70 656e 2075 7020  ended`..Open up 
+000015b0: 6120 7465 726d 696e 616c 2061 6e64 2069  a terminal and i
+000015c0: 6e73 7461 6c6c 202a 2a48 7375 616e 7775  nstall **Hsuanwu
+000015d0: 2a2a 2077 6974 6820 6070 6970 603a 0a60  ** with `pip`:.`
+000015e0: 6060 2073 6865 6c6c 0a70 6970 2069 6e73  `` shell.pip ins
+000015f0: 7461 6c6c 2068 7375 616e 7775 2023 2062  tall hsuanwu # b
+00001600: 6173 6963 2069 6e73 7461 6c6c 6174 696f  asic installatio
+00001610: 6e0a 7069 7020 696e 7374 616c 6c20 6873  n.pip install hs
+00001620: 7561 6e77 755b 656e 7673 5d20 2320 666f  uanwu[envs] # fo
+00001630: 7220 7072 652d 6465 6669 6e65 6420 656e  r pre-defined en
+00001640: 7669 726f 6e6d 656e 7473 0a70 6970 2069  vironments.pip i
+00001650: 6e73 7461 6c6c 2068 7375 616e 7775 5b74  nstall hsuanwu[t
+00001660: 6573 7473 5d20 2320 666f 7220 7072 6f6a  ests] # for proj
+00001670: 6563 7420 7465 7374 730a 7069 7020 696e  ect tests.pip in
+00001680: 7374 616c 6c20 6873 7561 6e77 755b 616c  stall hsuanwu[al
+00001690: 6c5d 2023 2069 6e73 7461 6c6c 2061 6c6c  l] # install all
+000016a0: 2074 6865 2064 6570 656e 6465 6e63 6965   the dependencie
+000016b0: 730a 6060 600a 0a2d 2077 6974 6820 6769  s.```..- with gi
+000016c0: 740a 0a4f 7065 6e20 7570 2061 2074 6572  t..Open up a ter
+000016d0: 6d69 6e61 6c20 616e 6420 636c 6f6e 6520  minal and clone 
+000016e0: 7468 6520 7265 706f 7369 746f 7279 2066  the repository f
+000016f0: 726f 6d20 5b47 6974 4875 625d 2868 7474  rom [GitHub](htt
+00001700: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001710: 524c 452d 466f 756e 6461 7469 6f6e 2f48  RLE-Foundation/H
+00001720: 7375 616e 7775 2920 7769 7468 2060 6769  suanwu) with `gi
+00001730: 7460 3a0a 6060 6020 7368 0a67 6974 2063  t`:.``` sh.git c
+00001740: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+00001750: 6875 622e 636f 6d2f 524c 452d 466f 756e  hub.com/RLE-Foun
+00001760: 6461 7469 6f6e 2f48 7375 616e 7775 2e67  dation/Hsuanwu.g
+00001770: 6974 0a60 6060 0a41 6674 6572 2074 6861  it.```.After tha
+00001780: 742c 2072 756e 2074 6865 2066 6f6c 6c6f  t, run the follo
+00001790: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
+000017a0: 696e 7374 616c 6c20 7061 636b 6167 6520  install package 
+000017b0: 616e 6420 6465 7065 6e64 656e 6369 6573  and dependencies
+000017c0: 3a0a 6060 6020 7368 0a70 6970 2069 6e73  :.``` sh.pip ins
+000017d0: 7461 6c6c 202d 6520 2e20 2320 6261 7369  tall -e . # basi
+000017e0: 6320 696e 7374 616c 6c61 7469 6f6e 0a70  c installation.p
+000017f0: 6970 2069 6e73 7461 6c6c 202d 6520 2e5b  ip install -e .[
+00001800: 656e 7673 5d20 2320 666f 7220 7072 652d  envs] # for pre-
+00001810: 6465 6669 6e65 6420 656e 7669 726f 6e6d  defined environm
+00001820: 656e 7473 0a70 6970 2069 6e73 7461 6c6c  ents.pip install
+00001830: 202d 6520 2e5b 7465 7374 735d 2023 2066   -e .[tests] # f
+00001840: 6f72 2070 726f 6a65 6374 2074 6573 7473  or project tests
+00001850: 0a70 6970 2069 6e73 7461 6c6c 202d 6520  .pip install -e 
+00001860: 2e5b 616c 6c5d 2023 2069 6e73 7461 6c6c  .[all] # install
+00001870: 2061 6c6c 2074 6865 2064 6570 656e 6465   all the depende
+00001880: 6e63 6965 730a 6060 600a 0a46 6f72 206d  ncies.```..For m
+00001890: 6f72 6520 6465 7461 696c 6564 2069 6e73  ore detailed ins
+000018a0: 7461 6c6c 6174 696f 6e20 696e 7374 7275  tallation instru
+000018b0: 6374 696f 6e2c 2073 6565 205b 6874 7470  ction, see [http
+000018c0: 733a 2f2f 646f 6373 2e68 7375 616e 7775  s://docs.hsuanwu
+000018d0: 2e64 6576 2f67 6574 7469 6e67 5f73 7461  .dev/getting_sta
+000018e0: 7274 6564 5d28 6874 7470 733a 2f2f 646f  rted](https://do
+000018f0: 6373 2e68 7375 616e 7775 2e64 6576 2f67  cs.hsuanwu.dev/g
+00001900: 6574 7469 6e67 5f73 7461 7274 6564 292e  etting_started).
+00001910: 0a0a 2323 2042 7569 6c64 2079 6f75 7220  ..## Build your 
+00001920: 6669 7273 7420 4873 7561 6e77 7520 6170  first Hsuanwu ap
+00001930: 706c 6963 6174 696f 6e0a 466f 7220 6578  plication.For ex
+00001940: 616d 706c 652c 2077 6520 7761 6e74 2074  ample, we want t
+00001950: 6f20 7573 6520 5b44 7251 2d76 325d 2868  o use [DrQ-v2](h
+00001960: 7474 7073 3a2f 2f6f 7065 6e72 6576 6965  ttps://openrevie
+00001970: 772e 6e65 742f 666f 7275 6d3f 6964 3d5f  w.net/forum?id=_
+00001980: 534a 2d5f 7979 6573 3829 2074 6f20 736f  SJ-_yyes8) to so
+00001990: 6c76 6520 6120 7461 736b 206f 6620 5b44  lve a task of [D
+000019a0: 6565 704d 696e 6420 436f 6e74 726f 6c20  eepMind Control 
+000019b0: 5375 6974 655d 2868 7474 7073 3a2f 2f67  Suite](https://g
+000019c0: 6974 6875 622e 636f 6d2f 6465 6570 6d69  ithub.com/deepmi
+000019d0: 6e64 2f64 6d5f 636f 6e74 726f 6c29 2c20  nd/dm_control), 
+000019e0: 616e 6420 7765 206f 6e6c 7920 6e65 6564  and we only need
+000019f0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2074   the following t
+00001a00: 776f 2073 7465 7073 3a0a 0a31 2e20 5772  wo steps:..1. Wr
+00001a10: 6974 6520 6120 6063 6f6e 6669 672e 7961  ite a `config.ya
+00001a20: 6d6c 6020 6669 6c65 2069 6e20 796f 7572  ml` file in your
+00001a30: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
+00001a40: 7279 206c 696b 653a 0a60 6060 2079 616d  ry like:.``` yam
+00001a50: 6c0a 6578 7065 7269 6d65 6e74 3a20 6472  l.experiment: dr
+00001a60: 7176 325f 646d 6320 2020 2020 2320 4578  qv2_dmc     # Ex
+00001a70: 7065 7269 6d65 6e74 2049 442e 0a64 6576  periment ID..dev
+00001a80: 6963 653a 2063 7564 613a 3020 2020 2020  ice: cuda:0     
+00001a90: 2020 2020 2020 2023 2044 6576 6963 6520         # Device 
+00001aa0: 2863 7075 2c20 6375 6461 2c20 2e2e 2e29  (cpu, cuda, ...)
+00001ab0: 206f 6e20 7768 6963 6820 7468 6520 636f   on which the co
+00001ac0: 6465 2073 686f 756c 6420 6265 2072 756e  de should be run
+00001ad0: 2e0a 7365 6564 3a20 3120 2020 2020 2020  ..seed: 1       
+00001ae0: 2020 2020 2020 2020 2020 2020 2320 5261              # Ra
+00001af0: 6e64 6f6d 2073 6565 6420 666f 7220 7265  ndom seed for re
+00001b00: 7072 6f64 7563 7469 6f6e 2e0a 6e75 6d5f  production..num_
+00001b10: 7472 6169 6e5f 7374 6570 733a 2032 3530  train_steps: 250
+00001b20: 3030 3020 2020 2320 4e75 6d62 6572 206f  000   # Number o
+00001b30: 6620 7472 6169 6e69 6e67 2073 7465 7073  f training steps
+00001b40: 2e0a 0a61 6765 6e74 3a0a 2020 6e61 6d65  ...agent:.  name
+00001b50: 3a20 4472 5176 3220 2020 2020 2020 2020  : DrQv2         
+00001b60: 2020 2020 2320 5468 6520 6167 656e 7420      # The agent 
+00001b70: 6e61 6d65 2e0a 6060 600a 0a32 2e20 5772  name..```..2. Wr
+00001b80: 6974 6520 6120 6074 7261 696e 2e70 7960  ite a `train.py`
+00001b90: 2066 696c 6520 6c69 6b65 3a0a 6060 6020   file like:.``` 
+00001ba0: 7079 7468 6f6e 0a69 6d70 6f72 7420 6879  python.import hy
+00001bb0: 6472 6120 2320 5573 6520 4879 6472 6120  dra # Use Hydra 
+00001bc0: 746f 206d 616e 6167 6520 6578 7065 7269  to manage experi
+00001bd0: 6d65 6e74 730a 0a66 726f 6d20 6873 7561  ments..from hsua
+00001be0: 6e77 752e 656e 7620 696d 706f 7274 206d  nwu.env import m
+00001bf0: 616b 655f 646d 635f 656e 7620 2320 496d  ake_dmc_env # Im
+00001c00: 706f 7274 2044 6565 704d 696e 6420 436f  port DeepMind Co
+00001c10: 6e74 726f 6c20 5375 6974 650a 6672 6f6d  ntrol Suite.from
+00001c20: 2068 7375 616e 7775 2e63 6f6d 6d6f 6e2e   hsuanwu.common.
+00001c30: 656e 6769 6e65 2069 6d70 6f72 7420 4873  engine import Hs
+00001c40: 7561 6e77 7545 6e67 696e 6520 2320 496d  uanwuEngine # Im
+00001c50: 706f 7274 2048 7375 616e 7775 2065 6e67  port Hsuanwu eng
+00001c60: 696e 650a 0a74 7261 696e 5f65 6e76 203d  ine..train_env =
+00001c70: 206d 616b 655f 646d 635f 656e 7628 656e   make_dmc_env(en
+00001c80: 765f 6964 3d27 6361 7274 706f 6c65 5f62  v_id='cartpole_b
+00001c90: 616c 616e 6365 2729 2023 2043 7265 6174  alance') # Creat
+00001ca0: 6520 7472 6169 6e20 656e 760a 7465 7374  e train env.test
+00001cb0: 5f65 6e76 203d 206d 616b 655f 646d 635f  _env = make_dmc_
+00001cc0: 656e 7628 656e 765f 6964 3d27 6361 7274  env(env_id='cart
+00001cd0: 706f 6c65 5f62 616c 616e 6365 2729 2023  pole_balance') #
+00001ce0: 2043 7265 6174 6520 7465 7374 2065 6e76   Create test env
+00001cf0: 0a0a 4068 7964 7261 2e6d 6169 6e28 7665  ..@hydra.main(ve
+00001d00: 7273 696f 6e5f 6261 7365 3d4e 6f6e 652c  rsion_base=None,
+00001d10: 2063 6f6e 6669 675f 7061 7468 3d27 2e2f   config_path='./
+00001d20: 272c 2063 6f6e 6669 675f 6e61 6d65 3d27  ', config_name='
+00001d30: 636f 6e66 6967 2729 0a64 6566 206d 6169  config').def mai
+00001d40: 6e28 6366 6773 293a 0a20 2020 2065 6e67  n(cfgs):.    eng
+00001d50: 696e 6520 3d20 4873 7561 6e77 7545 6e67  ine = HsuanwuEng
+00001d60: 696e 6528 6366 6773 3d63 6667 732c 2074  ine(cfgs=cfgs, t
+00001d70: 7261 696e 5f65 6e76 3d74 7261 696e 5f65  rain_env=train_e
+00001d80: 6e76 2c20 7465 7374 5f65 6e76 3d74 6573  nv, test_env=tes
+00001d90: 745f 656e 7629 2023 2049 6e69 7469 616c  t_env) # Initial
+00001da0: 697a 6520 656e 6769 6e65 0a20 2020 2065  ize engine.    e
+00001db0: 6e67 696e 652e 696e 766f 6b65 2829 2023  ngine.invoke() #
+00001dc0: 2053 7461 7274 2074 7261 696e 696e 670a   Start training.
+00001dd0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+00001de0: 275f 5f6d 6169 6e5f 5f27 3a0a 2020 2020  '__main__':.    
+00001df0: 6d61 696e 2829 0a60 6060 0a52 756e 2060  main().```.Run `
+00001e00: 7472 6169 6e2e 7079 6020 616e 6420 796f  train.py` and yo
+00001e10: 7520 7769 6c6c 2073 6565 2074 6865 2066  u will see the f
+00001e20: 6f6c 6c6f 7769 6e67 206f 7574 7075 743a  ollowing output:
+00001e30: 0a0a 3c64 6976 2061 6c69 676e 3d63 656e  ..<div align=cen
+00001e40: 7465 723e 0a3c 696d 6720 7372 633d 272e  ter>.<img src='.
+00001e50: 2f64 6f63 732f 6173 7365 7473 2f69 6d61  /docs/assets/ima
+00001e60: 6765 732f 726c 5f74 7261 696e 696e 672e  ges/rl_training.
+00001e70: 706e 6727 3e0a 3c2f 6469 763e 0a0a 466f  png'>.</div>..Fo
+00001e80: 7220 6d6f 7265 2064 6574 6169 6c65 6420  r more detailed 
+00001e90: 7475 746f 7269 616c 732c 2073 6565 205b  tutorials, see [
+00001ea0: 6874 7470 733a 2f2f 646f 6373 2e68 7375  https://docs.hsu
+00001eb0: 616e 7775 2e64 6576 2f74 7574 6f72 6961  anwu.dev/tutoria
+00001ec0: 6c73 5d28 6874 7470 733a 2f2f 646f 6373  ls](https://docs
+00001ed0: 2e68 7375 616e 7775 2e64 6576 2f74 7574  .hsuanwu.dev/tut
+00001ee0: 6f72 6961 6c73 292e 0a0a 2320 496d 706c  orials)...# Impl
+00001ef0: 656d 656e 7465 6420 4d6f 6475 6c65 730a  emented Modules.
+00001f00: 2323 2052 6f61 646d 6170 0a48 7375 616e  ## Roadmap.Hsuan
+00001f10: 7775 2065 766f 6c76 6573 2062 6173 6564  wu evolves based
+00001f20: 206f 6e20 7265 696e 666f 7263 656d 656e   on reinforcemen
+00001f30: 7420 6c65 6172 6e69 6e67 2061 6c67 6f72  t learning algor
+00001f40: 6974 686d 7320 616e 6420 696e 7465 6772  ithms and integr
+00001f50: 6174 6573 206c 6174 6573 7420 7472 6963  ates latest tric
+00001f60: 6b73 2e20 5468 6520 666f 6c6c 6f77 696e  ks. The followin
+00001f70: 6720 6669 6775 7265 2064 656d 6f6e 7374  g figure demonst
+00001f80: 7261 7465 7320 7468 6520 6d61 696e 2065  rates the main e
+00001f90: 766f 6c75 7469 6f6e 2072 6f61 646d 6170  volution roadmap
+00001fa0: 206f 6620 4873 7561 6e77 753a 0a0a 3c64   of Hsuanwu:..<d
+00001fb0: 6976 2061 6c69 676e 3d63 656e 7465 723e  iv align=center>
+00001fc0: 0a3c 696d 6720 7372 633d 272e 2f64 6f63  .<img src='./doc
+00001fd0: 732f 6173 7365 7473 2f69 6d61 6765 732f  s/assets/images/
+00001fe0: 726f 6164 6d61 702e 7376 6727 2020 7374  roadmap.svg'  st
+00001ff0: 796c 653d 2277 6964 7468 3a20 3930 2522  yle="width: 90%"
+00002000: 3e0a 3c2f 6469 763e 0a0a 2323 2050 726f  >.</div>..## Pro
+00002010: 6a65 6374 2053 7472 7563 7475 7265 0a0a  ject Structure..
+00002020: 5365 6520 7468 6520 7072 6f6a 6563 7420  See the project 
+00002030: 7374 7275 6374 7572 6520 6265 6c6f 773a  structure below:
+00002040: 0a3c 6469 7620 616c 6967 6e3d 6365 6e74  .<div align=cent
+00002050: 6572 3e0a 3c69 6d67 2073 7263 3d27 2e2f  er>.<img src='./
+00002060: 646f 6373 2f61 7373 6574 732f 696d 6167  docs/assets/imag
+00002070: 6573 2f73 7472 7563 7475 7265 2e73 7667  es/structure.svg
+00002080: 2720 7374 796c 653d 2277 6964 7468 3a20  ' style="width: 
+00002090: 3930 2522 3e0a 3c2f 6469 763e 0a0a 2d20  90%">.</div>..- 
+000020a0: 2a2a 5b43 6f6d 6d6f 6e5d 2868 7474 7073  **[Common](https
+000020b0: 3a2f 2f64 6f63 732e 6873 7561 6e77 752e  ://docs.hsuanwu.
+000020c0: 6465 762f 636f 6d6d 6f6e 5f69 6e64 6578  dev/common_index
+000020d0: 2f29 2a2a 3a20 4175 7869 6c69 6172 7920  /)**: Auxiliary 
+000020e0: 6d6f 6475 6c65 7320 6c69 6b65 2074 7261  modules like tra
+000020f0: 696e 6572 2061 6e64 206c 6f67 6765 722e  iner and logger.
+00002100: 0a20 2020 202b 202a 2a45 6e67 696e 652a  .    + **Engine*
+00002110: 2a3a 202a 456e 6769 6e65 2066 6f72 2062  *: *Engine for b
+00002120: 7569 6c64 696e 6720 4873 7561 6e77 7520  uilding Hsuanwu 
+00002130: 6170 706c 6963 6174 696f 6e2e 2a0a 2020  application.*.  
+00002140: 2020 2b20 2a2a 4c6f 6767 6572 2a2a 3a20    + **Logger**: 
+00002150: 2a4c 6f67 6765 7220 666f 7220 6d61 6e61  *Logger for mana
+00002160: 6769 6e67 206f 7574 7075 7420 696e 666f  ging output info
+00002170: 726d 6174 696f 6e2e 2a0a 0a2d 202a 2a5b  rmation.*..- **[
+00002180: 5870 6c6f 6974 5d28 6874 7470 733a 2f2f  Xploit](https://
+00002190: 646f 6373 2e68 7375 616e 7775 2e64 6576  docs.hsuanwu.dev
+000021a0: 2f78 706c 6f69 745f 696e 6465 782f 292a  /xploit_index/)*
+000021b0: 2a3a 204d 6f64 756c 6573 2074 6861 7420  *: Modules that 
+000021c0: 666f 6375 7320 6f6e 203c 666f 6e74 2063  focus on <font c
+000021d0: 6f6c 6f72 3d22 2342 3830 3030 3022 3e3c  olor="#B80000"><
+000021e0: 623e 6578 706c 6f69 7461 7469 6f6e 3c2f  b>exploitation</
+000021f0: 623e 3c2f 666f 6e74 3e20 696e 2052 4c2e  b></font> in RL.
+00002200: 0a20 2020 202b 202a 2a45 6e63 6f64 6572  .    + **Encoder
+00002210: 2a2a 3a20 2a4e 6575 7261 6c20 6e65 776f  **: *Neural newo
+00002220: 726b 2d62 6173 6564 2065 6e63 6f64 6572  rk-based encoder
+00002230: 2066 6f72 2070 726f 6365 7373 696e 6720   for processing 
+00002240: 6f62 7365 7276 6174 696f 6e73 2e2a 0a20  observations.*. 
+00002250: 2020 202b 202a 2a41 6765 6e74 2a2a 3a20     + **Agent**: 
+00002260: 2a41 6765 6e74 2066 6f72 2069 6e74 6572  *Agent for inter
+00002270: 6163 7469 6e67 2061 6e64 206c 6561 726e  acting and learn
+00002280: 696e 672e 2a0a 2020 2020 2b20 2a2a 5374  ing.*.    + **St
+00002290: 6f72 6167 652a 2a3a 202a 5374 6f72 6167  orage**: *Storag
+000022a0: 6520 666f 7220 7374 6f72 696e 6720 636f  e for storing co
+000022b0: 6c6c 6563 7465 6420 6578 7065 7269 656e  llected experien
+000022c0: 6365 732e 2a0a 0a2d 202a 2a5b 5870 6c6f  ces.*..- **[Xplo
+000022d0: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
+000022e0: 2e68 7375 616e 7775 2e64 6576 2f78 706c  .hsuanwu.dev/xpl
+000022f0: 6f72 655f 696e 6465 782f 292a 2a3a 204d  ore_index/)**: M
+00002300: 6f64 756c 6573 2074 6861 7420 666f 6375  odules that focu
+00002310: 7320 6f6e 203c 666f 6e74 2063 6f6c 6f72  s on <font color
+00002320: 3d22 2342 3830 3030 3022 3e3c 623e 6578  ="#B80000"><b>ex
+00002330: 706c 6f72 6174 696f 6e3c 2f62 3e3c 2f66  ploration</b></f
+00002340: 6f6e 743e 2069 6e20 524c 2e0a 2020 2020  ont> in RL..    
+00002350: 2b20 2a2a 4175 676d 656e 7461 7469 6f6e  + **Augmentation
+00002360: 2a2a 3a20 2a50 7954 6f72 6368 2e6e 6e2d  **: *PyTorch.nn-
+00002370: 6c69 6b65 206d 6f64 756c 6573 2066 6f72  like modules for
+00002380: 206f 6273 6572 7661 7469 6f6e 2061 7567   observation aug
+00002390: 6d65 6e74 6174 696f 6e2e 2a0a 2020 2020  mentation.*.    
+000023a0: 2b20 2a2a 4469 7374 7269 6275 7469 6f6e  + **Distribution
+000023b0: 2a2a 3a20 2a44 6973 7472 6962 7574 696f  **: *Distributio
+000023c0: 6e73 2066 6f72 2073 616d 706c 696e 6720  ns for sampling 
+000023d0: 6163 7469 6f6e 732e 2a0a 2020 2020 2b20  actions.*.    + 
+000023e0: 2a2a 5265 7761 7264 2a2a 3a20 2a49 6e74  **Reward**: *Int
+000023f0: 7269 6e73 6963 2072 6577 6172 6420 6d6f  rinsic reward mo
+00002400: 6475 6c65 7320 666f 7220 656e 6861 6e63  dules for enhanc
+00002410: 696e 6720 6578 706c 6f72 6174 696f 6e2e  ing exploration.
+00002420: 2a0a 0a2d 202a 2a5b 4576 616c 7561 7469  *..- **[Evaluati
+00002430: 6f6e 5d28 6874 7470 733a 2f2f 646f 6373  on](https://docs
+00002440: 2e68 7375 616e 7775 2e64 6576 2f65 7661  .hsuanwu.dev/eva
+00002450: 6c75 6174 696f 6e5f 696e 6465 782f 292a  luation_index/)*
+00002460: 2a3a 2052 6561 736f 6e61 626c 6520 616e  *: Reasonable an
+00002470: 6420 7265 6c69 6162 6c65 206d 6574 7269  d reliable metri
+00002480: 6373 2066 6f72 2061 6c67 6f72 6974 686d  cs for algorithm
+00002490: 2065 7661 6c75 6174 696f 6e2e 0a0a 2d20   evaluation...- 
+000024a0: 2a2a 5b45 6e76 5d28 6874 7470 733a 2f2f  **[Env](https://
+000024b0: 646f 6373 2e68 7375 616e 7775 2e64 6576  docs.hsuanwu.dev
+000024c0: 2f65 6e76 5f69 6e64 6578 2f29 2a2a 3a20  /env_index/)**: 
+000024d0: 5061 636b 6167 6564 2065 6e76 6972 6f6e  Packaged environ
+000024e0: 6d65 6e74 7320 2865 2e67 2e2c 2041 7461  ments (e.g., Ata
+000024f0: 7269 2067 616d 6573 2920 666f 7220 6661  ri games) for fa
+00002500: 7374 2069 6e76 6f63 6174 696f 6e2e 0a0a  st invocation...
+00002510: 2d20 2a2a 5b50 7265 2d74 7261 696e 696e  - **[Pre-trainin
+00002520: 675d 2868 7474 7073 3a2f 2f64 6f63 732e  g](https://docs.
+00002530: 6873 7561 6e77 752e 6465 762f 7072 6574  hsuanwu.dev/pret
+00002540: 7261 696e 696e 675f 696e 6465 782f 292a  raining_index/)*
+00002550: 2a3a 204d 6574 686f 6473 206f 6620 3c66  *: Methods of <f
+00002560: 6f6e 7420 636f 6c6f 723d 2223 4238 3030  ont color="#B800
+00002570: 3030 223e 3c62 3e70 7265 2d74 7261 696e  00"><b>pre-train
+00002580: 696e 673c 2f62 3e3c 2f66 6f6e 743e 2069  ing</b></font> i
+00002590: 6e20 524c 2e0a 0a2d 202a 2a5b 4465 706c  n RL...- **[Depl
+000025a0: 6f79 6d65 6e74 5d28 6874 7470 733a 2f2f  oyment](https://
+000025b0: 646f 6373 2e68 7375 616e 7775 2e64 6576  docs.hsuanwu.dev
+000025c0: 2f64 6570 6c6f 796d 656e 745f 696e 6465  /deployment_inde
+000025d0: 782f 292a 2a3a 204d 6574 686f 6473 206f  x/)**: Methods o
+000025e0: 6620 3c66 6f6e 7420 636f 6c6f 723d 2223  f <font color="#
+000025f0: 4238 3030 3030 223e 3c62 3e6d 6f64 656c  B80000"><b>model
+00002600: 2064 6570 6c6f 796d 656e 743c 2f62 3e3c   deployment</b><
+00002610: 2f66 6f6e 743e 2069 6e20 524c 2e0a 0a46  /font> in RL...F
+00002620: 6f72 206d 6f72 6520 6465 7469 6c65 6420  or more detiled 
+00002630: 6465 7363 7269 7074 696f 6e73 206f 6620  descriptions of 
+00002640: 7468 6573 6520 6d6f 6475 6c65 732c 2073  these modules, s
+00002650: 6565 205b 6874 7470 733a 2f2f 646f 6373  ee [https://docs
+00002660: 2e68 7375 616e 7775 2e64 6576 2f61 7069  .hsuanwu.dev/api
+00002670: 5d28 6874 7470 733a 2f2f 646f 6373 2e68  ](https://docs.h
+00002680: 7375 616e 7775 2e64 6576 2f61 7069 290a  suanwu.dev/api).
+00002690: 0a23 2320 524c 2041 6765 6e74 730a 7c4d  .## RL Agents.|M
+000026a0: 6f64 756c 657c 5265 6375 7272 656e 747c  odule|Recurrent|
+000026b0: 426f 787c 4469 7363 7265 7465 7c4d 756c  Box|Discrete|Mul
+000026c0: 7469 4269 6e61 7279 7c4d 756c 7469 2050  tiBinary|Multi P
+000026d0: 726f 6365 7373 696e 677c 4e50 557c 5061  rocessing|NPU|Pa
+000026e0: 7065 727c 4369 7461 7469 6f6e 737c 0a7c  per|Citations|.|
+000026f0: 3a2d 7c3a 2d7c 3a2d 7c3a 2d7c 3a2d 7c3a  :-|:-|:-|:-|:-|:
+00002700: 2d7c 3a2d 7c3a 2d7c 3a2d 7c0a 7c53 4143  -|:-|:-|:-|.|SAC
+00002710: 7ce2 9d8c 7c20 e29c 94ef b88f 207c e29d  |...| ...... |..
+00002720: 8c7c e29d 8c7c e29d 8c7c f09f 908c 207c  .|...|...|.... |
+00002730: 205b 4c69 6e6b 5d28 6874 7470 3a2f 2f70   [Link](http://p
+00002740: 726f 6365 6564 696e 6773 2e6d 6c72 2e70  roceedings.mlr.p
+00002750: 7265 7373 2f76 3830 2f68 6161 726e 6f6a  ress/v80/haarnoj
+00002760: 6131 3862 2f68 6161 726e 6f6a 6131 3862  a18b/haarnoja18b
+00002770: 2e70 6466 2920 7c35 3037 37e2 ad90 7c0a  .pdf) |5077...|.
+00002780: 7c44 7251 7ce2 9d8c 7c20 e29c 94ef b88f  |DrQ|...| ......
+00002790: 207c e29d 8c7c e29d 8c7c e29d 8c7c f09f   |...|...|...|..
+000027a0: 908c 207c 205b 4c69 6e6b 5d28 6874 7470  .. | [Link](http
+000027b0: 733a 2f2f 6172 7869 762e 6f72 672f 7064  s://arxiv.org/pd
+000027c0: 662f 3230 3034 2e31 3336 3439 2920 7c34  f/2004.13649) |4
+000027d0: 3333 e2ad 907c 0a7c 4444 5047 7ce2 9d8c  33...|.|DDPG|...
+000027e0: 7c20 e29c 94ef b88f 207c e29d 8c7c e29d  | ...... |...|..
+000027f0: 8c7c e29d 8c7c f09f 908c 207c 205b 4c69  .|...|.... | [Li
+00002800: 6e6b 5d28 6874 7470 733a 2f2f 6172 7869  nk](https://arxi
+00002810: 762e 6f72 672f 7064 662f 3135 3039 2e30  v.org/pdf/1509.0
+00002820: 3239 3731 2e70 6466 3f73 6f75 7263 653d  2971.pdf?source=
+00002830: 706f 7374 5f70 6167 652d 2d2d 2d2d 2d2d  post_page-------
+00002840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002850: 2d2d 2d2d 2920 7c31 3138 3139 e2ad 907c  ----) |11819...|
+00002860: 0a7c 4472 512d 7632 7ce2 9d8c 7c20 e29c  .|DrQ-v2|...| ..
+00002870: 94ef b88f 207c e29d 8c7c e29d 8c7c e29d  .... |...|...|..
+00002880: 8c7c f09f 908c 207c 205b 4c69 6e6b 5d28  .|.... | [Link](
+00002890: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+000028a0: 672f 7064 662f 3231 3037 2e30 3936 3435  g/pdf/2107.09645
+000028b0: 2e70 6466 3f75 746d 5f73 6f75 7263 653d  .pdf?utm_source=
+000028c0: 6d6f 7269 6f68 2e63 6f6d 2920 7c31 3030  morioh.com) |100
+000028d0: e2ad 907c 0a7c 5050 4f7c e29d 8c7c 20e2  ...|.|PPO|...| .
+000028e0: 9c94 efb8 8f20 7ce2 9c94 efb8 8f7c e29c  ..... |......|..
+000028f0: 94ef b88f 7ce2 9c94 efb8 8f7c f09f 908c  ....|......|....
+00002900: 207c 205b 4c69 6e6b 5d28 6874 7470 733a   | [Link](https:
+00002910: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
+00002920: 3137 3037 2e30 3633 3437 2920 7c31 3131  1707.06347) |111
+00002930: 3535 e2ad 907c 0a7c 4441 4143 7ce2 9d8c  55...|.|DAAC|...
+00002940: 7c20 e29c 94ef b88f 207c e29c 94ef b88f  | ...... |......
+00002950: 7ce2 9c94 efb8 8f7c e29c 94ef b88f 7cf0  |......|......|.
+00002960: 9f90 8c20 7c20 5b4c 696e 6b5d 2868 7474  ... | [Link](htt
+00002970: 703a 2f2f 7072 6f63 6565 6469 6e67 732e  p://proceedings.
+00002980: 6d6c 722e 7072 6573 732f 7631 3339 2f72  mlr.press/v139/r
+00002990: 6169 6c65 616e 7532 3161 2f72 6169 6c65  aileanu21a/raile
+000029a0: 616e 7532 3161 2e70 6466 2920 7c35 36e2  anu21a.pdf) |56.
+000029b0: ad90 7c0a 7c44 7241 437c e29d 8c7c 20e2  ..|.|DrAC|...| .
+000029c0: 9c94 efb8 8f20 7ce2 9c94 efb8 8f7c e29c  ..... |......|..
+000029d0: 94ef b88f 7ce2 9c94 efb8 8f7c f09f 908c  ....|......|....
+000029e0: 207c 205b 4c69 6e6b 5d28 6874 7470 733a   | [Link](https:
+000029f0: 2f2f 7072 6f63 6565 6469 6e67 732e 6e65  //proceedings.ne
+00002a00: 7572 6970 732e 6363 2f70 6170 6572 2f32  urips.cc/paper/2
+00002a10: 3032 312f 6669 6c65 2f32 6233 3863 3264  021/file/2b38c2d
+00002a20: 6636 6134 3962 3937 6637 3036 6563 3931  f6a49b97f706ec91
+00002a30: 3438 6365 3438 6438 362d 5061 7065 722e  48ce48d86-Paper.
+00002a40: 7064 6629 207c 3239 e2ad 907c 0a7c 5050  pdf) |29...|.|PP
+00002a50: 477c e29d 8c7c 20e2 9c94 efb8 8f20 7ce2  G|...| ...... |.
+00002a60: 9c94 efb8 8f7c e29d 8c7c e29c 94ef b88f  .....|...|......
+00002a70: 7cf0 9f90 8c7c 205b 4c69 6e6b 5d28 6874  |....| [Link](ht
+00002a80: 7470 3a2f 2f70 726f 6365 6564 696e 6773  tp://proceedings
+00002a90: 2e6d 6c72 2e70 7265 7373 2f76 3133 392f  .mlr.press/v139/
+00002aa0: 636f 6262 6532 3161 2f63 6f62 6265 3231  cobbe21a/cobbe21
+00002ab0: 612e 7064 6629 207c 3832 e2ad 907c 0a7c  a.pdf) |82...|.|
+00002ac0: 494d 5041 4c41 7ce2 9c94 efb8 8f7c 20e2  IMPALA|......| .
+00002ad0: 9c94 efb8 8f20 7ce2 9c94 efb8 8f7c e29d  ..... |......|..
+00002ae0: 8c7c e29c 94ef b88f 7cf0 9f90 8c7c 205b  .|......|....| [
+00002af0: 4c69 6e6b 5d28 6874 7470 3a2f 2f70 726f  Link](http://pro
+00002b00: 6365 6564 696e 6773 2e6d 6c72 2e70 7265  ceedings.mlr.pre
+00002b10: 7373 2f76 3830 2f65 7370 6568 6f6c 7431  ss/v80/espeholt1
+00002b20: 3861 2f65 7370 6568 6f6c 7431 3861 2e70  8a/espeholt18a.p
+00002b30: 6466 2920 7c31 3231 39e2 ad90 7c0a 0a3e  df) |1219...|..>
+00002b40: 202d 20f0 9f90 8c3a 2044 6576 656c 6f70   - ....: Develop
+00002b50: 696e 672e 0a3e 202d 2060 4e50 5560 3a20  ing..> - `NPU`: 
+00002b60: 5375 7070 6f72 7420 4e65 7572 616c 2d6e  Support Neural-n
+00002b70: 6574 776f 726b 2070 726f 6365 7373 696e  etwork processin
+00002b80: 6720 756e 6974 2e0a 3e20 2d20 6052 6563  g unit..> - `Rec
+00002b90: 7572 7265 6e74 603a 2053 7570 706f 7274  urrent`: Support
+00002ba0: 2072 6563 7572 7265 6e74 206e 6575 7261   recurrent neura
+00002bb0: 6c20 6e65 7477 6f72 6b2e 0a3e 202d 2060  l network..> - `
+00002bc0: 426f 7860 3a20 4120 4e2d 6469 6d65 6e73  Box`: A N-dimens
+00002bd0: 696f 6e61 6c20 626f 7820 7468 6174 2063  ional box that c
+00002be0: 6f6e 7461 696e 6573 2065 7665 7279 2070  ontaines every p
+00002bf0: 6f69 6e74 2069 6e20 7468 6520 6163 7469  oint in the acti
+00002c00: 6f6e 2073 7061 6365 2e0a 3e20 2d20 6044  on space..> - `D
+00002c10: 6973 6372 6574 6560 3a20 4120 6c69 7374  iscrete`: A list
+00002c20: 206f 6620 706f 7373 6962 6c65 2061 6374   of possible act
+00002c30: 696f 6e73 2c20 7768 6572 6520 6561 6368  ions, where each
+00002c40: 2074 696d 6573 7465 7020 6f6e 6c79 206f   timestep only o
+00002c50: 6e65 206f 6620 7468 6520 6163 7469 6f6e  ne of the action
+00002c60: 7320 6361 6e20 6265 2075 7365 642e 0a3e  s can be used..>
+00002c70: 202d 2060 4d75 6c74 6942 696e 6172 7960   - `MultiBinary`
+00002c80: 3a20 4120 6c69 7374 206f 6620 706f 7373  : A list of poss
+00002c90: 6962 6c65 2061 6374 696f 6e73 2c20 7768  ible actions, wh
+00002ca0: 6572 6520 6561 6368 2074 696d 6573 7465  ere each timeste
+00002cb0: 7020 616e 7920 6f66 2074 6865 2061 6374  p any of the act
+00002cc0: 696f 6e73 2063 616e 2062 6520 7573 6564  ions can be used
+00002cd0: 2069 6e20 616e 7920 636f 6d62 696e 6174   in any combinat
+00002ce0: 696f 6e2e 0a0a 2323 2049 6e74 7269 6e73  ion...## Intrins
+00002cf0: 6963 2052 6577 6172 6420 4d6f 6475 6c65  ic Reward Module
+00002d00: 730a 7c20 4d6f 6475 6c65 207c 2052 656d  s.| Module | Rem
+00002d10: 6172 6b20 7c20 5265 7072 2e20 207c 2056  ark | Repr.  | V
+00002d20: 6973 7561 6c20 7c20 5265 6665 7265 6e63  isual | Referenc
+00002d30: 6520 7c20 0a7c 3a2d 7c3a 2d7c 3a2d 7c3a  e | .|:-|:-|:-|:
+00002d40: 2d7c 3a2d 7c0a 7c20 5073 6575 646f 436f  -|:-|.| PseudoCo
+00002d50: 756e 7473 207c 2043 6f75 6e74 2d42 6173  unts | Count-Bas
+00002d60: 6564 2065 7870 6c6f 7261 7469 6f6e 207c  ed exploration |
+00002d70: e29c 94ef b88f 7ce2 9c94 efb8 8f7c 5b4e  ......|......|[N
+00002d80: 6576 6572 2047 6976 6520 5570 3a20 4c65  ever Give Up: Le
+00002d90: 6172 6e69 6e67 2044 6972 6563 7465 6420  arning Directed 
+00002da0: 4578 706c 6f72 6174 696f 6e20 5374 7261  Exploration Stra
+00002db0: 7465 6769 6573 5d28 6874 7470 733a 2f2f  tegies](https://
+00002dc0: 6172 7869 762e 6f72 672f 7064 662f 3230  arxiv.org/pdf/20
+00002dd0: 3032 2e30 3630 3338 2920 7c0a 7c20 4943  02.06038) |.| IC
+00002de0: 4d20 207c 2043 7572 696f 7369 7479 2d64  M  | Curiosity-d
+00002df0: 7269 7665 6e20 6578 706c 6f72 6174 696f  riven exploratio
+00002e00: 6e20 207c 20e2 9c94 efb8 8f7c e29c 94ef  n  | ......|....
+00002e10: b88f 7c20 5b43 7572 696f 7369 7479 2d44  ..| [Curiosity-D
+00002e20: 7269 7665 6e20 4578 706c 6f72 6174 696f  riven Exploratio
+00002e30: 6e20 6279 2053 656c 662d 5375 7065 7276  n by Self-Superv
+00002e40: 6973 6564 2050 7265 6469 6374 696f 6e5d  ised Prediction]
+00002e50: 2868 7474 703a 2f2f 7072 6f63 6565 6469  (http://proceedi
+00002e60: 6e67 732e 6d6c 722e 7072 6573 732f 7637  ngs.mlr.press/v7
+00002e70: 302f 7061 7468 616b 3137 612f 7061 7468  0/pathak17a/path
+00002e80: 616b 3137 612e 7064 6629 207c 200a 7c20  ak17a.pdf) | .| 
+00002e90: 524e 4420 207c 2043 6f75 6e74 2d62 6173  RND  | Count-bas
+00002ea0: 6564 2065 7870 6c6f 7261 7469 6f6e 2020  ed exploration  
+00002eb0: 7c20 e29d 8c7c e29c 94ef b88f 7c20 5b45  | ...|......| [E
+00002ec0: 7870 6c6f 7261 7469 6f6e 2062 7920 5261  xploration by Ra
+00002ed0: 6e64 6f6d 204e 6574 776f 726b 2044 6973  ndom Network Dis
+00002ee0: 7469 6c6c 6174 696f 6e5d 2868 7474 7073  tillation](https
+00002ef0: 3a2f 2f61 7278 6976 2e6f 7267 2f70 6466  ://arxiv.org/pdf
+00002f00: 2f31 3831 302e 3132 3839 342e 7064 6629  /1810.12894.pdf)
+00002f10: 207c 200a 7c20 4749 524d 207c 2043 7572   | .| GIRM | Cur
+00002f20: 696f 7369 7479 2d64 7269 7665 6e20 6578  iosity-driven ex
+00002f30: 706c 6f72 6174 696f 6e20 207c 20e2 9c94  ploration  | ...
+00002f40: efb8 8f20 7ce2 9c94 efb8 8f7c 205b 496e  ... |......| [In
+00002f50: 7472 696e 7369 6320 5265 7761 7264 2044  trinsic Reward D
+00002f60: 7269 7665 6e20 496d 6974 6174 696f 6e20  riven Imitation 
+00002f70: 4c65 6172 6e69 6e67 2076 6961 2047 656e  Learning via Gen
+00002f80: 6572 6174 6976 6520 4d6f 6465 6c5d 2868  erative Model](h
+00002f90: 7474 703a 2f2f 7072 6f63 6565 6469 6e67  ttp://proceeding
+00002fa0: 732e 6d6c 722e 7072 6573 732f 7631 3139  s.mlr.press/v119
+00002fb0: 2f79 7532 3064 2f79 7532 3064 2e70 6466  /yu20d/yu20d.pdf
+00002fc0: 297c 0a7c 204e 4755 207c 204d 656d 6f72  )|.| NGU | Memor
+00002fd0: 792d 6261 7365 6420 6578 706c 6f72 6174  y-based explorat
+00002fe0: 696f 6e20 207c 20e2 9c94 efb8 8f20 207c  ion  | ......  |
+00002ff0: e29c 94ef b88f 7c20 5b4e 6576 6572 2047  ......| [Never G
+00003000: 6976 6520 5570 3a20 4c65 6172 6e69 6e67  ive Up: Learning
+00003010: 2044 6972 6563 7465 6420 4578 706c 6f72   Directed Explor
+00003020: 6174 696f 6e20 5374 7261 7465 6769 6573  ation Strategies
+00003030: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
+00003040: 6f72 672f 7064 662f 3230 3032 2e30 3630  org/pdf/2002.060
+00003050: 3338 2920 7c20 0a7c 2052 4944 457c 2050  38) | .| RIDE| P
+00003060: 726f 6365 6475 7261 6c6c 792d 6765 6e65  rocedurally-gene
+00003070: 7261 7465 6420 656e 7669 726f 6e6d 656e  rated environmen
+00003080: 7420 7c20 e29c 94ef b88f 207c e29c 94ef  t | ...... |....
+00003090: b88f 7c20 5b52 4944 453a 2052 6577 6172  ..| [RIDE: Rewar
+000030a0: 6469 6e67 2049 6d70 6163 742d 4472 6976  ding Impact-Driv
+000030b0: 656e 2045 7870 6c6f 7261 7469 6f6e 2066  en Exploration f
+000030c0: 6f72 2050 726f 6365 6475 7261 6c6c 792d  or Procedurally-
+000030d0: 4765 6e65 7261 7465 6420 456e 7669 726f  Generated Enviro
+000030e0: 6e6d 656e 7473 5d28 6874 7470 733a 2f2f  nments](https://
+000030f0: 6172 7869 762e 6f72 672f 7064 662f 3230  arxiv.org/pdf/20
+00003100: 3032 2e31 3232 3932 297c 0a7c 2052 4533  02.12292)|.| RE3
+00003110: 2020 7c20 456e 7472 6f70 7920 4d61 7869    | Entropy Maxi
+00003120: 6d69 7a61 7469 6f6e 207c 20e2 9d8c 207c  mization | ... |
+00003130: e29c 94ef b88f 7c20 5b53 7461 7465 2045  ......| [State E
+00003140: 6e74 726f 7079 204d 6178 696d 697a 6174  ntropy Maximizat
+00003150: 696f 6e20 7769 7468 2052 616e 646f 6d20  ion with Random 
+00003160: 456e 636f 6465 7273 2066 6f72 2045 6666  Encoders for Eff
+00003170: 6963 6965 6e74 2045 7870 6c6f 7261 7469  icient Explorati
+00003180: 6f6e 5d28 6874 7470 3a2f 2f70 726f 6365  on](http://proce
+00003190: 6564 696e 6773 2e6d 6c72 2e70 7265 7373  edings.mlr.press
+000031a0: 2f76 3133 392f 7365 6f32 3161 2f73 656f  /v139/seo21a/seo
+000031b0: 3231 612e 7064 6629 207c 0a7c 2052 4953  21a.pdf) |.| RIS
+000031c0: 4520 207c 2045 6e74 726f 7079 204d 6178  E  | Entropy Max
+000031d0: 696d 697a 6174 696f 6e20 207c 20e2 9d8c  imization  | ...
+000031e0: 2020 7ce2 9c94 efb8 8f7c 205b 52c3 a96e    |......| [R..n
+000031f0: 7969 2053 7461 7465 2045 6e74 726f 7079  yi State Entropy
+00003200: 204d 6178 696d 697a 6174 696f 6e20 666f   Maximization fo
+00003210: 7220 4578 706c 6f72 6174 696f 6e20 4163  r Exploration Ac
+00003220: 6365 6c65 7261 7469 6f6e 2069 6e20 5265  celeration in Re
+00003230: 696e 666f 7263 656d 656e 7420 4c65 6172  inforcement Lear
+00003240: 6e69 6e67 5d28 6874 7470 733a 2f2f 6965  ning](https://ie
+00003250: 6565 7870 6c6f 7265 2e69 6565 652e 6f72  eexplore.ieee.or
+00003260: 672f 6162 7374 7261 6374 2f64 6f63 756d  g/abstract/docum
+00003270: 656e 742f 3938 3032 3931 372f 2920 7c20  ent/9802917/) | 
+00003280: 0a7c 2052 4556 4420 207c 2044 6976 6572  .| REVD  | Diver
+00003290: 6765 6e63 6520 4d61 7869 6d69 7a61 7469  gence Maximizati
+000032a0: 6f6e 207c 20e2 9d8c 2020 7ce2 9c94 efb8  on | ...  |.....
+000032b0: 8f7c 205b 5265 7761 7264 696e 6720 4570  .| [Rewarding Ep
+000032c0: 6973 6f64 6963 2056 6973 6974 6174 696f  isodic Visitatio
+000032d0: 6e20 4469 7363 7265 7061 6e63 7920 666f  n Discrepancy fo
+000032e0: 7220 4578 706c 6f72 6174 696f 6e20 696e  r Exploration in
+000032f0: 2052 6569 6e66 6f72 6365 6d65 6e74 204c   Reinforcement L
+00003300: 6561 726e 696e 675d 2868 7474 7073 3a2f  earning](https:/
+00003310: 2f6f 7065 6e72 6576 6965 772e 6e65 742f  /openreview.net/
+00003320: 7064 663f 6964 3d56 3270 7731 5659 4d72  pdf?id=V2pw1VYMr
+00003330: 446f 297c 0a0a 3e20 2d20 f09f 908c 3a20  Do)|..> - ....: 
+00003340: 4465 7665 6c6f 7069 6e67 2e0a 3e20 2d20  Developing..> - 
+00003350: 6052 6570 722e 603a 2054 6865 206d 6574  `Repr.`: The met
+00003360: 686f 6420 696e 766f 6c76 6573 2072 6570  hod involves rep
+00003370: 7265 7365 6e74 6174 696f 6e20 6c65 6172  resentation lear
+00003380: 6e69 6e67 2e0a 3e20 2d20 6056 6973 7561  ning..> - `Visua
+00003390: 6c60 3a20 5468 6520 6d65 7468 6f64 2077  l`: The method w
+000033a0: 6f72 6b73 2077 656c 6c20 696e 2076 6973  orks well in vis
+000033b0: 7561 6c20 524c 2e0a 0a53 6565 205b 5475  ual RL...See [Tu
+000033c0: 746f 7269 616c 733a 2055 7365 2069 6e74  torials: Use int
+000033d0: 7269 6e73 6963 2072 6577 6172 6420 616e  rinsic reward an
+000033e0: 6420 6f62 7365 7276 6174 696f 6e20 6175  d observation au
+000033f0: 676d 656e 7461 7469 6f6e 5d28 6874 7470  gmentation](http
+00003400: 733a 2f2f 646f 6373 2e68 7375 616e 7775  s://docs.hsuanwu
+00003410: 2e64 6576 2f74 7574 6f72 6961 6c73 2f64  .dev/tutorials/d
+00003420: 6174 615f 6175 676d 656e 7461 7469 6f6e  ata_augmentation
+00003430: 2e6d 6429 2066 6f72 2075 7361 6765 2065  .md) for usage e
+00003440: 7861 6d70 6c65 732e 0a0a 2320 4d6f 6465  xamples...# Mode
+00003450: 6c20 5a6f 6f0a 4873 7561 6e77 7520 7072  l Zoo.Hsuanwu pr
+00003460: 6f76 6964 6573 2061 206c 6172 6765 206e  ovides a large n
+00003470: 756d 6265 7220 6f66 2072 6575 7361 626c  umber of reusabl
+00003480: 6520 6265 6368 6d61 726b 732c 2073 6565  e bechmarks, see
+00003490: 205b 6874 7470 733a 2f2f 6875 622e 6873   [https://hub.hs
+000034a0: 7561 6e77 752e 6465 762f 5d28 6874 7470  uanwu.dev/](http
+000034b0: 733a 2f2f 6875 622e 6873 7561 6e77 752e  s://hub.hsuanwu.
+000034c0: 6465 762f 2920 616e 6420 5b68 7474 7073  dev/) and [https
+000034d0: 3a2f 2f64 6f63 732e 6873 7561 6e77 752e  ://docs.hsuanwu.
+000034e0: 6465 762f 6265 6e63 686d 6172 6b73 2f5d  dev/benchmarks/]
+000034f0: 2868 7474 7073 3a2f 2f64 6f63 732e 6873  (https://docs.hs
+00003500: 7561 6e77 752e 6465 762f 6265 6e63 686d  uanwu.dev/benchm
+00003510: 6172 6b73 2f29 0a0a 2320 4150 4920 446f  arks/)..# API Do
+00003520: 6375 6d65 6e74 6174 696f 6e0a 5669 6577  cumentation.View
+00003530: 206f 7572 2077 656c 6c2d 6465 7369 676e   our well-design
+00003540: 6564 2064 6f63 756d 656e 7461 7469 6f6e  ed documentation
+00003550: 3a20 5b68 7474 7073 3a2f 2f64 6f63 732e  : [https://docs.
+00003560: 6873 7561 6e77 752e 6465 762f 5d28 6874  hsuanwu.dev/](ht
+00003570: 7470 733a 2f2f 646f 6373 2e68 7375 616e  tps://docs.hsuan
+00003580: 7775 2e64 6576 2f29 0a0a 2320 486f 7720  wu.dev/)..# How 
+00003590: 546f 2043 6f6e 7472 6962 7574 650a 5765  To Contribute.We
+000035a0: 6c63 6f6d 6520 746f 2063 6f6e 7472 6962  lcome to contrib
+000035b0: 7574 6520 746f 2074 6869 7320 7072 6f6a  ute to this proj
+000035c0: 6563 7421 2042 6566 6f72 6520 796f 7520  ect! Before you 
+000035d0: 6265 6769 6e20 7772 6974 696e 6720 636f  begin writing co
+000035e0: 6465 2c20 706c 6561 7365 2072 6561 6420  de, please read 
+000035f0: 5b43 4f4e 5452 4942 5554 494e 472e 6d64  [CONTRIBUTING.md
+00003600: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00003610: 2e63 6f6d 2f52 4c45 2d46 6f75 6e64 6174  .com/RLE-Foundat
+00003620: 696f 6e2f 4873 7561 6e77 752f 626c 6f62  ion/Hsuanwu/blob
+00003630: 2f6d 6169 6e2f 434f 4e54 5249 4255 5449  /main/CONTRIBUTI
+00003640: 4e47 2e6d 6429 2066 6f72 2067 7569 6465  NG.md) for guide
+00003650: 2066 6972 7374 2e0a 0a23 2041 636b 6e6f   first...# Ackno
+00003660: 776c 6564 676d 656e 740a 5468 6973 2070  wledgment.This p
+00003670: 726f 6a65 6374 2069 7320 7375 7070 6f72  roject is suppor
+00003680: 7465 6420 6279 205b 4655 4e44 494e 472e  ted by [FUNDING.
+00003690: 796d 6c5d 2868 7474 7073 3a2f 2f67 6974  yml](https://git
+000036a0: 6875 622e 636f 6d2f 524c 452d 466f 756e  hub.com/RLE-Foun
+000036b0: 6461 7469 6f6e 2f48 7375 616e 7775 2f62  dation/Hsuanwu/b
+000036c0: 6c6f 622f 6d61 696e 2f2e 6769 7468 7562  lob/main/.github
+000036d0: 2f46 554e 4449 4e47 2e79 6d6c 292e 2053  /FUNDING.yml). S
+000036e0: 6f6d 6520 636f 6465 206f 6620 7468 6973  ome code of this
+000036f0: 2070 726f 6a65 6374 2069 7320 626f 7272   project is borr
+00003700: 6f77 6564 206f 7220 696e 7370 6972 6564  owed or inspired
+00003710: 2062 7920 7365 7665 7261 6c20 6578 6365   by several exce
+00003720: 6c6c 656e 7420 7072 6f6a 6563 7473 2c20  llent projects, 
+00003730: 616e 6420 7765 2068 6967 686c 7920 6170  and we highly ap
+00003740: 7072 6563 6961 7465 2074 6865 6d2e 2053  preciate them. S
+00003750: 6565 205b 4143 4b4e 4f57 4c45 4447 4d45  ee [ACKNOWLEDGME
+00003760: 4e54 2e6d 645d 2868 7474 7073 3a2f 2f67  NT.md](https://g
+00003770: 6974 6875 622e 636f 6d2f 524c 452d 466f  ithub.com/RLE-Fo
+00003780: 756e 6461 7469 6f6e 2f48 7375 616e 7775  undation/Hsuanwu
+00003790: 2f62 6c6f 622f 6d61 696e 2f41 434b 4e4f  /blob/main/ACKNO
+000037a0: 574c 4544 474d 454e 542e 6d64 292e 0a    WLEDGMENT.md)..
```

### Comparing `hsuanwu-0.0.1b4/pyproject.toml` & `hsuanwu-0.0.1b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hsuanwu"
-version = "0.0.1.beta04"
+version = "0.0.1.beta05"
 authors = [
   { name="Reinforcement Learning Evolution Foundation", email="friedrichyuan19990827@gmail.com" },
 ]
 description = "Long-Term Evolution Project of Reinforcement Learning"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["Reinforcement Learning", "Algorithm", "Evolution", "Baseline"]
```

