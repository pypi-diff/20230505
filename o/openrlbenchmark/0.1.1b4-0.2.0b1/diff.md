# Comparing `tmp/openrlbenchmark-0.1.1b4.tar.gz` & `tmp/openrlbenchmark-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrlbenchmark-0.1.1b4.tar", max compression
+gzip compressed data, was "openrlbenchmark-0.2.0b1.tar", max compression
```

## Comparing `openrlbenchmark-0.1.1b4.tar` & `openrlbenchmark-0.2.0b1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.1.1b4/LICENSE
--rw-r--r--   0        0        0    17239 2023-03-27 22:18:06.833815 openrlbenchmark-0.1.1b4/README.md
--rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.1.1b4/openrlbenchmark/__init__.py
--rw-r--r--   0        0        0     1341 2023-03-28 15:48:56.578806 openrlbenchmark-0.1.1b4/openrlbenchmark/cache.py
--rw-r--r--   0        0        0     4955 2023-03-26 16:47:06.950946 openrlbenchmark-0.1.1b4/openrlbenchmark/hns.py
--rw-r--r--   0        0        0    16630 2023-03-28 15:48:53.814930 openrlbenchmark-0.1.1b4/openrlbenchmark/rlops.py
--rw-r--r--   0        0        0    19561 2023-03-18 22:00:03.882272 openrlbenchmark-0.1.1b4/openrlbenchmark/rlops_hns copy.py
--rw-r--r--   0        0        0    20896 2023-03-28 15:47:04.651826 openrlbenchmark-0.1.1b4/openrlbenchmark/rlops_hns.py
--rw-r--r--   0        0        0      598 2023-03-28 15:50:30.864350 openrlbenchmark-0.1.1b4/pyproject.toml
--rw-r--r--   0        0        0    18656 1970-01-01 00:00:00.000000 openrlbenchmark-0.1.1b4/setup.py
--rw-r--r--   0        0        0    18097 1970-01-01 00:00:00.000000 openrlbenchmark-0.1.1b4/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.0b1/LICENSE
+-rw-r--r--   0        0        0    17986 2023-05-05 19:43:33.380795 openrlbenchmark-0.2.0b1/README.md
+-rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.0b1/openrlbenchmark/__init__.py
+-rw-r--r--   0        0        0     1746 2023-05-05 13:12:27.589472 openrlbenchmark-0.2.0b1/openrlbenchmark/cache.py
+-rw-r--r--   0        0        0     1746 2023-05-05 13:01:23.002773 openrlbenchmark-0.2.0b1/openrlbenchmark/cache_legacy.py
+-rw-r--r--   0        0        0     6147 2023-05-01 14:06:32.647152 openrlbenchmark-0.2.0b1/openrlbenchmark/capped_hns.py
+-rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.0b1/openrlbenchmark/hns.py
+-rw-r--r--   0        0        0     2178 2023-05-05 13:13:16.550687 openrlbenchmark-0.2.0b1/openrlbenchmark/offline_db.py
+-rw-r--r--   0        0        0    19819 2023-05-05 19:46:30.981443 openrlbenchmark-0.2.0b1/openrlbenchmark/rlops.py
+-rw-r--r--   0        0        0    29810 2023-05-05 19:46:45.092157 openrlbenchmark-0.2.0b1/openrlbenchmark/rlops_hns.py
+-rw-r--r--   0        0        0      696 2023-05-05 19:56:58.585797 openrlbenchmark-0.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0    19471 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.0b1/setup.py
+-rw-r--r--   0        0        0    18949 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.0b1/PKG-INFO
```

### Comparing `openrlbenchmark-0.1.1b4/LICENSE` & `openrlbenchmark-0.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.1.1b4/README.md` & `openrlbenchmark-0.2.0b1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: openrlbenchmark
+Version: 0.2.0b1
+Summary: 
+Author: Costa Huang
+Author-email: costa.huang@outlook.com
+Requires-Python: >=3.7.1,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: dotmap (>=1.3.30,<2.0.0)
+Requires-Dist: expt (>=0.4.1,<0.5.0)
+Requires-Dist: importlib-metadata (>=5.1.0,<6.0.0)
+Requires-Dist: multiprocess (>=0.70.13,<0.71.0)
+Requires-Dist: peewee (>=3.16.2,<4.0.0)
+Requires-Dist: pip (>=22.1.2,<23.0.0)
+Requires-Dist: rich (<12.0)
+Requires-Dist: rliable (>=1.0.8,<2.0.0)
+Requires-Dist: seaborn (>=0.12.1,<0.13.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: tueplots (>=0.0.4,<0.0.5)
+Requires-Dist: tyro (>=0.5.0,<0.6.0)
+Requires-Dist: wandb (>=0.13.7,<0.14.0)
+Description-Content-Type: text/markdown
+
 # Open RL Benchmark: Comprehensive Tracked Experiments for Reinforcement Learning
 
 
 [<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openrlbenchmark/openrlbenchmark/blob/master/README.ipynb)
@@ -52,18 +79,18 @@
         'sac' \
         'td3' \
         'ppo' \
         'trpo' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' \
         'sac_continuous_action?tag=rlops-pilot&cl=SAC' \
     --env-ids HalfCheetahBulletEnv-v0 \
-    --ncols 1 \
-    --ncols-legend 2 \
-    --xlabel 'Training Steps' \
-    --ylabel 'Episodic Return' \
+    --pc.ncols 1 \
+    --pc.ncols-legend 2 \
+    --pc.xlabel 'Training Steps' \
+    --pc.ylabel 'Episodic Return' \
     --output-filename compare \
     --report
 ```
 
 Here, we created multiple filters. The first string in the first filter is `'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean'`, which is a query string that specifies the following:
 
 * `we`: the W&B entity name
@@ -72,15 +99,15 @@
 * `cen`: the custom key for the experiment name
 * `metric`: the metric we are interested in
 
 So we are fetching metrics from [https://wandb.ai/openrlbenchmark/sb3](https://wandb.ai/openrlbenchmark/sb3). The environment id is stored in the `env` key, and the experiment name is stored in the `algo` key. The metric we are interested in is `rollout/ep_rew_mean`.
 
 Similarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `ppo_lstm?cl=PPO w/ LSTM`.
 
-The labels of the figure can be customized with the `--xlabel` and `--ylabel` flags. The `--ncols` flag specifies the number of columns in the figure. The `--ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
+The labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
 
 The command above generates the following plot:
 
 |    cleanrl vs. Stable Baselines 3   |    cleanrl vs. Stable Baselines 3 (Time)   |
 |:----------------------------------:|:----------------------------------------:|
 |  ![](static/cleanrl_vs_sb3.png)   |   ![](static/cleanrl_vs_sb3-time.png)   |
 
@@ -93,16 +120,15 @@
 
 **Learning curves:** the `compare.png` shows the learning curves which subsamples 10000 data points and and interpolate. The curves are smoothed by a rolling average with a window size 100 and their shaded region represents the standard deviation.
 
 **Result table:** the `compare.md` and `compare.csv` shows the average episodic return of the last 100 episodes. For each random seed $i$ (we have 3 random seeds for each set of experiments), we calculate the average episodic return of the last 100 training episodes as $a_i$. We then average the $a_i$'s over all random seeds to get the final average episodic return and report its standard deviation. This type of evaluation is known as an implicit evaluation method ([Machado et al., 2017](https://arxiv.org/pdf/1709.06009.pdf)) which aligns better with the general goal of RL which is continual learning. This method also detects issues with catastrophic forgetting compared to the evaluation method that evaluates the best model.
 
 
 > **Warning**
-> You may get slightly different curves every time you run the commands. This is because we sample 500 data points from the track experiments to save bandwidth. You can, however, get all of the data points by running the command with `--scan-history` which will always give you the same curves but will take longer to run. For generating an accurate `compare.md`, you should always use `--scan-history`.
-
+> You may get slightly different curves every time you run the commands. This is because we sample 500 data points from the track experiments to save bandwidth. If you are using `openrlbenchmark` repeatedly or you wanto to generate consistent `compare.md` and learning curves, we recommend you to use `--scan-history` to get all of the data points, but initially it may take a while to run.
 
 
 ## Currently supported libraries
 
 * [CleanRL](https://wandb.ai/openrlbenchmark/cleanrl)
     * `ceik`: `env_id`
     * `cen`: `exp_name` (e.g., `sac_continuous_action`, `ppo_continuous_action`, `ppo_atari`)
@@ -123,14 +149,18 @@
     * `ceik`: `env`
     * `cen`: `alg` (e.g., `sac`, `tqc`)
     * `metric`: `rollout/ep_rew_mean` or `eval/mean_reward`
 * [Tianshou](https://wandb.ai/tianshou/atari.benchmark)
     * `ceik`: `task`
     * `cen`: `algo_name` (e.g., `ppo`, `iqn`)
     * `metric`: `test/reward`
+* [MORL-Baselines](https://wandb.ai/openrlbenchmark/morl-baselines)
+    * `ceik`: `env_id`
+    * `cen`: `algo` (e.g., `PGMORL`, `PCN`)
+    * `metric`: `eval/hypervolume`, `eval/igd`, `eval/sparsity`, `eval/eum`, `eval/mul`
 
 The following libraries have some recorded experiments:
 
 * [openai/phasic-policy-gradient](https://wandb.ai/openrlbenchmark/phasic-policy-gradient) (has some metrics)
     * `ceik`: `env_name`
     * `cen`: `arch` (`shared`)
     * `metric`: `charts/episodic_return`
@@ -140,135 +170,151 @@
     * `metric`: `charts/episodic_return`
 
 
 ## More examples
 
 ### Compare CleanRL's PPO with `openai/baselines`'s PPO2 on Atari games:
 
+Sometimes the same environments could have different names in different libraries. For example, `openai/baselines` uses `BreakoutNoFrameskip-v4` while [EnvPool](https://envpool.readthedocs.io/en/latest/env/atari.html) uses `Breakout-v5`. To compare the two libraries, we need to specify the `env_id` for `CleanRL` and `env` for `openai/baselines`. In this case, can specify the corresponding `env_ids` for each filter.
+
+For Atari games, we have additional batteries included `openrlbenchmark.rlops_hns` to show human normalized-scores and further statistical analysis through [`rliable`](https://github.com/google-research/rliable).
+
+
 ```shell
-python -m openrlbenchmark.rlops \
+python -m openrlbenchmark.rlops_hns \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
     --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation' \
+    --env-ids AlienNoFrameskip-v4 AmidarNoFrameskip-v4 AssaultNoFrameskip-v4 AsterixNoFrameskip-v4 AsteroidsNoFrameskip-v4 AtlantisNoFrameskip-v4 BankHeistNoFrameskip-v4 BattleZoneNoFrameskip-v4 BeamRiderNoFrameskip-v4 BerzerkNoFrameskip-v4 BowlingNoFrameskip-v4 BoxingNoFrameskip-v4 BreakoutNoFrameskip-v4 CentipedeNoFrameskip-v4 ChopperCommandNoFrameskip-v4 CrazyClimberNoFrameskip-v4 DefenderNoFrameskip-v4 DemonAttackNoFrameskip-v4 DoubleDunkNoFrameskip-v4 EnduroNoFrameskip-v4 FishingDerbyNoFrameskip-v4 FreewayNoFrameskip-v4 FrostbiteNoFrameskip-v4 GopherNoFrameskip-v4 GravitarNoFrameskip-v4 HeroNoFrameskip-v4 IceHockeyNoFrameskip-v4 PrivateEyeNoFrameskip-v4 QbertNoFrameskip-v4 RiverraidNoFrameskip-v4 RoadRunnerNoFrameskip-v4 RobotankNoFrameskip-v4 SeaquestNoFrameskip-v4 SkiingNoFrameskip-v4 SolarisNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 StarGunnerNoFrameskip-v4 SurroundNoFrameskip-v4 TennisNoFrameskip-v4 TimePilotNoFrameskip-v4 TutankhamNoFrameskip-v4 UpNDownNoFrameskip-v4 VentureNoFrameskip-v4 VideoPinballNoFrameskip-v4 WizardOfWorNoFrameskip-v4 YarsRevengeNoFrameskip-v4 ZaxxonNoFrameskip-v4 JamesbondNoFrameskip-v4 KangarooNoFrameskip-v4 KrullNoFrameskip-v4 KungFuMasterNoFrameskip-v4 MontezumaRevengeNoFrameskip-v4 MsPacmanNoFrameskip-v4 NameThisGameNoFrameskip-v4 PhoenixNoFrameskip-v4 PitfallNoFrameskip-v4 PongNoFrameskip-v4 \
     --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \
-    --check-empty-runs False \
-    --ncols 5 \
-    --ncols-legend 2 \
+    --no-check-empty-runs \
+    --pc.ncols 5 \
+    --pc.ncols-legend 2 \
     --output-filename static/cleanrl_vs_baselines \
-    --scan-history
+    --scan-history --rliable
 ```
 
-![](static/cleanrl_vs_baselines.png)
+In the individual learning curves below, the right y-axis is the human normalized score. The left y-axis is the raw episodic return.
+![](static/cleanrl_vs_baselines.png) The script also generates `cleanrl_vs_baselines_hns_median.png`, the learning curves for median human-normalized scores. 
 
-### Compare CleanRL's PPO with `openai/baselines`'s PPO2 and `jaxrl`'s SAC on Mujoco:
+Furthermore, the `--rliable` integration generates `cleanrl_vs_baselines_iqm_profile.png`, the  Interquartile Mean (IQM) and performance profile ([Agarwal et al., 2022](https://arxiv.org/pdf/2108.13264.pdf)), and `cleanrl_vs_baselines_hns_aggregate.png`, the aggregate human-normalized scores with Stratified Bootstrap Confidence Intervals (see @araffin's excellent blog post [explainer](https://araffin.github.io/post/rliable/)). 
+
+
+![](static/cleanrl_vs_baselines_hns_median.png)
+
+![](static/cleanrl_vs_baselines_iqm_profile.png)
+
+![](static/cleanrl_vs_baselines_hns_aggregate.png)
+
+
+### Offline mode
+
+Sometimes even with caching `--scan-history` the script can still take a long time if there are too many environments or experiments. This is because we are still calling many `wandb.Api().runs(..., filters)` under the hood. 
+
+No worries though. When running with `--scan-history`, we also automatically build a local `sqlite` database to store the metadata of runs, enabling us to run the script without internet connection.
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-mlp' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_continuous_action?tag=v1.0.0-27-gde3f410' \
     --filters '?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return' 'sac' \
     --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \
-    --check-empty-runs False \
-    --ncols 3 \
-    --ncols-legend 3 \
-    --output-filename compare \
-    --scan-history
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 3 \
+    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \
+    --scan-history \
+    --offline
 ```
-![](static/baselines_vs_cleanrl_vs_jaxrl.png)
 
+### Compare CleanRL's PPO with `openai/baselines`'s PPO2 and `jaxrl`'s SAC on Mujoco:
 
 ```shell
 python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
-    --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation' \
-    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_scan?tag=pr-328' \
-    --env-ids BeamRider-v5 Breakout-v5  \
-    --check-empty-runs False \
-    --ncols 3 \
-    --ncols-legend 2 \
-    --output-filename compare \
+    --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-mlp' \
+    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_continuous_action?tag=v1.0.0-27-gde3f410' \
+    --filters '?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return' 'sac' \
+    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 3 \
+    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \
     --scan-history
 ```
+![](static/baselines_vs_cleanrl_vs_jaxrl.png)
+
 
 
 ### Compare Tianshou's algorithms with `openai/baselines`'s PPO2 on Atari:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=tianshou&wpn=atari.benchmark&ceik=task&cen=algo_name&metric=test/reward' 'iqn' 'ppo' 'rainbow' 'fqf' 'c51' 'dqn' 'qrdqn' \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
     --env-ids BreakoutNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 SeaquestNoFrameskip-v4 MsPacmanNoFrameskip-v4 EnduroNoFrameskip-v4 PongNoFrameskip-v4 QbertNoFrameskip-v4 \
-    --check-empty-runs False \
-    --ncols 4 \
-    --ncols-legend 4 \
+    --no-check-empty-runs \
+    --pc.ncols 4 \
+    --pc.ncols-legend 4 \
     --output-filename static/baselines_vs_tianshou --scan-history
 ```
 ![](static/baselines_vs_tianshou.png)
 
 
 ### Compare CleanRL's PPG and PPO with `openai/phasic-policy-gradient`'s PPG on procgen:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=phasic-policy-gradient&ceik=env_name&cen=arch&metric=charts/episodic_return' 'shared' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_procgen?tag=v1.0.0b1-4-g4ea73d9' 'ppg_procgen?tag=v1.0.0b1-4-g4ea73d9' \
     --env-ids starpilot bossfight bigfish \
-    --check-empty-runs False \
-    --ncols 3 \
-    --ncols-legend 3 \
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 3 \
     --output-filename static/ppg_vs_cleanrl \
     --scan-history
 ```
 
 ![](static/ppg_vs_cleanrl.png)
 
 
 ### Compare CleanRL's TD3 with `sfujim/TD3`'s TD3 on Mujoco:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=sfujim-TD3&ceik=env&cen=policy&metric=charts/episodic_return' 'TD3' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'td3_continuous_action_jax?tag=pr-285' 'ddpg_continuous_action_jax?tag=pr-298' \
     --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 \
-    --check-empty-runs False \
-    --ncols 3 \
-    --ncols-legend 3 \
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 3 \
     --output-filename static/td3_vs_cleanrl \
     --scan-history
 ```
 ![](static/td3_vs_cleanrl.png)
 
 
-### Compare CleanRL's PPO + JAX + EnvPool's XLA with `openai/baselines`'s Atari wrappers vs [Machado's recommendetation for Atari](https://arxiv.org/abs/1709.06009) (e.g., sticky action with probability 0.25). The machado's experiments ran for 10M steps, which corresponds to 40M frames.
-
-```shell
-python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation_machado_10M' 'ppo_atari_envpool_xla_jax_truncation'  \
-    --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \
-    --check-empty-runs False \
-    --ncols 5 \
-    --ncols-legend 2 \
-    --output-filename static/machado_10M \
-    --scan-history
-```
-![](static/machado_10M.png)
-
 
-### Compare CleanRL's PPO + JAX + EnvPool's XLA with `openai/baselines`'s Atari wrappers vs [Machado's recommendetation for Atari](https://arxiv.org/abs/1709.06009) (e.g., sticky action with probability 0.25). The machado's experiments ran for 50M steps, which corresponds to 200M frames.
+### Compare MORL Baselines algorithms on deterministic environments
 
 ```shell
 python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation_machado' 'ppo_atari_envpool_xla_jax_truncation'  \
-    --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \
-    --check-empty-runs False \
-    --ncols 5 \
-    --ncols-legend 2 \
-    --output-filename static/machado_50M \
-    --scan-history
+  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metric=eval/hypervolume' \
+  'Pareto Q-Learning?cl=Pareto Q-Learning' \
+  'MultiPolicy MO Q-Learning?cl=MultiPolicy MO Q-Learning' \
+  'MultiPolicy MO Q-Learning (OLS)?cl=MultiPolicy MO Q-Learning (OLS)' \
+  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 \
+  --pc.ncols 2 \
+  --pc.ncols-legend 1 \
+  --pc.xlabel 'Training steps' \
+  --pc.ylabel 'Hypervolume' \
+  --output-filename morl_deterministic_envs \
+  --scan-history
 ```
-![](static/machado_50M.png)
+
+![](static/morl_deterministic_envs.png)
+![](static/morl_deterministic_envs-time.png)
 
 ### Calculate human normalized scores
 
 ```shell
 python -m openrlbenchmark.hns --files static/cleanrl_vs_baselines.csv static/machado_10M.csv static/machado_50M.csv 
 ```
 
@@ -296,23 +342,7 @@
 
 * Add experiments from other libraries
 * Run more experiments from currently supported libraries
 * Documentation and designing standards
 * Download the tensorboard metrics from the tracked experiments and load them locally to save time
 
 
-
-
-```shell
-pip install --upgrade openrlbenchmark
-python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'dqn_atari?tag=latest' 'c51_atari?tag=latest' \
-    --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
-    --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation?user=costa-huang' \
-    --env-ids BeamRider-v5 Breakout-v5 Pong-v5 \
-    --ncols 3 \
-    --ncols-legend 2 \
-    --output-filename compare \
-    --scan-history \
-    --report \
-    --check-empty-runs False 
-```
```

### Comparing `openrlbenchmark-0.1.1b4/openrlbenchmark/hns.py` & `openrlbenchmark-0.2.0b1/openrlbenchmark/hns.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 
 def parse_args():
     # fmt: off
     parser = argparse.ArgumentParser()
     parser.add_argument("--files", nargs="+", default=[],
         help="the csv files to calculate the median human normalized scores")
+    parser.add_argument("--percentiles", nargs="+", default=[], type=float,
+        help="the displayed percentile range of the median human normalized scores (e.g., 0.45 0.55)")
     # fmt: on
     return parser.parse_args()
 
 
 atari_human_normalized_scores = {
     "Alien-v5": (227.8, 7127.7),
     "Amidar-v5": (5.8, 1719.5),
@@ -104,18 +106,33 @@
         # env_ids = atari_human_normalized_scores.keys()
         env_ids = df.index
         for runset_name in df.columns:
             if runset_name in runset_names:
                 continue
             runset_names.add(runset_name)
             hnss = []
+            hnss_std = []
             for env_id in env_ids:
                 # if env_id not in df.index:
                 #     continue
                 episodic_return = float(df.loc[env_id, runset_name].split(" ± ")[0])
+                episodic_return_std = float(df.loc[env_id, runset_name].split(" ± ")[1])
                 hns = (episodic_return - atari_human_normalized_scores[env_id][0]) / (
                     atari_human_normalized_scores[env_id][1] - atari_human_normalized_scores[env_id][0]
                 )
                 hnss += [hns]
+                hns_std = (episodic_return_std - atari_human_normalized_scores[env_id][0]) / (
+                    atari_human_normalized_scores[env_id][1] - atari_human_normalized_scores[env_id][0]
+                )
+                hnss_std += [hns_std]
             print(f"{runset_name}")
             print(f"┣━━ median hns: {np.median(hnss)}")
+            if len(args.percentiles) > 0:
+
+                start_idx = int(len(hnss) * args.percentiles[0])
+                end_idx = int(len(hnss) * args.percentiles[1])
+                hnss, hnss_std, env_ids = zip(*sorted(zip(hnss, hnss_std, env_ids)))
+                print(f"┣━━━━━ median environments between {args.percentiles[0]} and {args.percentiles[1]} percentile")
+                for idx in range(start_idx, end_idx):
+                    print(f"┣━━━━━━━ {env_ids[idx]}: {hnss[idx]} ± {hnss_std[idx]}")
+
             print(f"┣━━ mean hns: {np.mean(hnss)}")
```

### Comparing `openrlbenchmark-0.1.1b4/openrlbenchmark/rlops.py` & `openrlbenchmark-0.2.0b1/openrlbenchmark/rlops.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,144 +1,226 @@
-import argparse
 import os
-from distutils.util import strtobool
+from dataclasses import dataclass, field
 from typing import List
 from urllib.parse import parse_qs, urlparse
 
 import expt
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import peewee as pw
 import seaborn as sns
+import tyro
 import wandb
 import wandb.apis.reports as wb  # noqa
 from expt import Hypothesis, Run
 from rich.console import Console
 from rich.pretty import pprint
 from rich.table import Table
 
 import openrlbenchmark
 import openrlbenchmark.cache
+from openrlbenchmark.offline_db import OfflineRun, OfflineRunTag, Tag, database_proxy
 
-api = wandb.Api()
 
-
-def parse_args():
-    # fmt: off
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--filters", nargs="+", action="append", default=[],
-        help="the filters of the experiments; see docs")
-    parser.add_argument("--env-ids", nargs="+", default=["Hopper-v2", "Walker2d-v2", "HalfCheetah-v2"],
-        help="the ids of the environment to compare")
-    parser.add_argument("--output-filename", type=str, default="compare",
-        help="the output filename of the plot, without extension")
-    parser.add_argument("--rolling", type=int, default=100,
-        help="the rolling window for smoothing the curves")
-    parser.add_argument("--metric-last-n-average-window", type=int, default=100,
-        help="the last n number of episodes to average metric over in the result table")
-    parser.add_argument("--ncols", type=int, default=2,
-        help="the number of columns in the chart")
-    parser.add_argument("--ncols-legend", type=int, default=2,
-        help="the number of legend columns in the chart")
-    parser.add_argument("--scan-history", type=lambda x: bool(strtobool(x)), default=False, nargs="?", const=True,
-        help="if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)")
-    parser.add_argument("--check-empty-runs", type=lambda x: bool(strtobool(x)), default=True, nargs="?", const=True,
-        help="if toggled, we will check for empty wandb runs")
-    parser.add_argument("--time-unit", type=str, default="m", choices=["s", "m", "h"],
-        help="the unit of time in the x-axis of the chart (e.g., `s` for seconds, `m` for minutes, `h` for hours); default: `m`")
-    parser.add_argument("--report", type=lambda x: bool(strtobool(x)), default=False, nargs="?", const=True,
-        help="if toggled, a wandb report will be created")
-    parser.add_argument("--xlabel", type=str, default="Step",
-        help="the label of the x-axis")
-    parser.add_argument("--ylabel", type=str, default="Episodic Return",
-        help="the label of the y-axis")
-    # fmt: on
-    return parser.parse_args()
-
-
-def to_rich_table(df: pd.DataFrame) -> Table:
-    table = Table()
-    for column in df.columns:
-        table.add_column(column)
-    for _, row in df.iterrows():
-        table.add_row(*row.astype(str).tolist())
-    return table
-
-
-def create_hypothesis(
-    name: str, wandb_runs: List[wandb.apis.public.Run], scan_history: bool = False, metric: str = ""
-) -> Hypothesis:
-    runs = []
-    for idx, run in enumerate(wandb_runs):
-        print("loading", run, run.url)
-        if run.state == "running":
-            print(f"Skipping running run: {run}")
-            continue
-        if scan_history:
-            # equivalent to `run_df = pd.DataFrame([row for row in run.scan_history()])`
-            run = openrlbenchmark.cache.CachedRun(run, cache_dir=os.path.join(openrlbenchmark.__path__[0], "dataset"))
-            run_df = run.run_df
-        else:
-            run_df = run.history(samples=1500)
-        if "videos" in run_df:
-            run_df = run_df.drop(columns=["videos"], axis=1)
-        if len(metric) > 0:
-            run_df["charts/episodic_return"] = run_df[metric]
-        runs += [Run(f"seed{idx}", run_df)]
-    return Hypothesis(name, runs)
+@dataclass
+class PlotConfig:
+    ncols: int = 2
+    """the number of columns in the chart"""
+    nrows: tyro.conf.Suppress[int] = None
+    """(TO BE FILLED in runtime) the number of rows in the chart"""
+    ncols_legend: int = 2
+    """the number of legend columns in the chart"""
+    xlabel: str = "Step"
+    """the label of the x-axis"""
+    ylabel: str = "Episodic Return"
+    """the label of the y-axis"""
+    sharex: bool = False
+    """if toggled, we will share the x-axis across all subplots"""
+    rolling: int = 100
+    """the rolling window for smoothing the curves"""
+    time_unit: str = "m"
+    """the unit of time in the x-axis of the chart (e.g., `s` for seconds, `m` for minutes, `h` for hours); default: `m`"""
+    cm: float = 4.0
+    """the multiplier for the column width"""
+    rm: float = 3.0
+    """the multiplier for the row height"""
+    hspace: float = None
+    """the height space between subplots"""
+    wspace: float = None
+    """the width space between subplots"""
+
+
+@dataclass
+class Args:
+    filters: tyro.conf.UseAppendAction[List[List[str]]]
+    """the filters of the experiments; see docs"""
+    env_ids: tyro.conf.UseAppendAction[List[List[str]]]
+    """the ids of the environment to compare"""
+    output_filename: str = "compare"
+    """the output filename of the plot, without extension"""
+    metric_last_n_average_window: int = 100
+    """the last n number of episodes to average metric over in the result table"""
+    scan_history: bool = False
+    """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
+    check_empty_runs: bool = False
+    """if toggled, we will check for empty wandb runs"""
+    report: bool = False
+    """if toggled, a wandb report will be created"""
+    wandb_project_name: str = "cleanrl"
+    """the wandb project name for the report creation"""
+    offline: bool = False
+    """if toggled, we will use the offline database instead of wandb"""
+    pc: tyro.conf.OmitSubcommandPrefixes[PlotConfig] = field(default_factory=PlotConfig)
+    """the plot configuration"""
 
 
 class Runset:
     def __init__(
         self,
         name: str,
-        filters: dict,
         entity: str,
         project: str,
-        groupby: str = "",
-        exp_name: str = "exp_name",
         metric: str = "charts/episodic_return",
+        groupby: str = "",
+        custom_exp_name_key: str = "exp_name",
+        exp_name: str = "",
+        custom_env_id_key: str = "env_id",
+        env_id: str = "",
+        tags: List[str] = [],
+        username: str = "",
         color: str = "#000000",
+        offline_db: pw.Database = None,
+        offline: bool = False,
     ):
         self.name = name
-        self.filters = filters
         self.entity = entity
         self.project = project
+        self.metric = metric
         self.groupby = groupby
+        self.custom_exp_name_key = custom_exp_name_key
         self.exp_name = exp_name
-        self.metric = metric
+        self.custom_env_id_key = custom_env_id_key
+        self.env_id = env_id
         self.color = color
+        self.tags = tags
+        self.username = username
+        self.offline_db = offline_db
+        self.offline = offline
+
+        user = [{"username": self.username}] if self.username else []
+        include_tag_groups = [{"tags": {"$in": [tag]}} for tag in self.tags] if len(self.tags) > 0 else []
+        self.wandb_filters = {
+            "$and": [
+                {f"config.{self.custom_env_id_key}.value": self.env_id},
+                *include_tag_groups,
+                *user,
+                {f"config.{self.custom_exp_name_key}.value": self.exp_name},
+            ]
+        }
 
     @property
     def runs(self):
-        return wandb.Api().runs(path=f"{self.entity}/{self.project}", filters=self.filters)
+        if not self.offline:
+            return wandb.Api().runs(
+                path=f"{self.entity}/{self.project}",
+                filters=self.wandb_filters,
+            )
+        else:
+            with self.offline_db.bind_ctx([OfflineRun, OfflineRunTag, Tag]):
+                cond = (
+                    (OfflineRun.project == self.project)
+                    & (OfflineRun.entity == self.entity)
+                    & (OfflineRun.config[self.custom_env_id_key] == self.env_id)
+                    & (OfflineRun.config[self.custom_exp_name_key] == self.exp_name)
+                )
+                if self.username:
+                    cond = cond and OfflineRun.username == self.username
+                if len(self.tags) > 0:
+                    for tag_str in self.tags:
+                        cond = cond & (Tag.name == tag_str)
+                    query = OfflineRun.select().join(OfflineRunTag).join(Tag).where(cond)
+                else:
+                    query = OfflineRun.select().where(cond)
+                g = [run for run in query]
+
+            return g
 
     @property
     def report_runset(self):
         return wb.Runset(
             name=self.name,
             entity=self.entity,
             project=self.project,
-            filters={"$or": [self.filters]},
+            filters={"$or": [self.wandb_filters]},
             groupby=[self.groupby] if len(self.groupby) > 0 else None,
         )
 
 
+def to_rich_table(df: pd.DataFrame) -> Table:
+    table = Table()
+    for column in df.columns:
+        table.add_column(column)
+    for _, row in df.iterrows():
+        table.add_row(*row.astype(str).tolist())
+    return table
+
+
+def create_hypothesis(runset: Runset, scan_history: bool = False) -> Hypothesis:
+    runs = []
+    for idx, run in enumerate(runset.runs):
+        print("loading", run, run.url)
+        if run.state == "running":
+            print(f"Skipping running run: {run}")
+            continue
+        if scan_history:
+            run = openrlbenchmark.cache.CachedRun(run, cache_dir=os.path.join(openrlbenchmark.__path__[0], "dataset"))
+            with runset.offline_db.bind_ctx([OfflineRun, OfflineRunTag, Tag]):
+                tags = []
+                for tag_str in run.run.tags:
+                    tag = Tag.get_or_none(name=tag_str)
+                    if not tag:
+                        tag = Tag.create(name=tag_str)
+                        tag.save()
+                    tags.append(tag)
+                offline_run = OfflineRun.get_or_none(id=run.run.id)
+                if not offline_run:
+                    offline_run = OfflineRun.create(
+                        id=run.run.id,
+                        name=run.run.name,
+                        state=run.run.state,
+                        url=run.run.url,
+                        path=run.run.path,
+                        username=run.run.user.username,
+                        tags=tags,
+                        project=run.run.project,
+                        entity=run.run.entity,
+                        config=run.run.config if isinstance(run.run.config, dict) else run.run.config.toDict(),
+                    )
+                    offline_run.save()
+            run_df = run.run_df
+        else:
+            run_df = run.history(samples=1500)
+        if "videos" in run_df:
+            run_df = run_df.drop(columns=["videos"], axis=1)
+        if len(runset.metric) > 0:
+            run_df["charts/episodic_return"] = run_df[runset.metric]
+        runs += [Run(f"seed{idx}", run_df)]
+    return Hypothesis(runset.name, runs)
+
+
 def compare(
     console: Console,
     runsetss: List[List[Runset]],
     env_ids: List[str],
-    ncols: int,
-    ncols_legend: int,
-    rolling: int,
     metric_last_n_average_window: int,
     scan_history: bool = False,
     output_filename: str = "compare",
     report: bool = False,
-    time_unit: str = "m",
+    pc: PlotConfig = None,
 ):
     blocks = []
     if report:
         for idx, env_id in enumerate(env_ids):
             metric_over_step = wb.LinePlot(
                 x="global_step",
                 y=list({runsets[idx].metric for runsets in runsetss}),
@@ -172,119 +254,129 @@
                     #     media_keys="videos",
                     # ),
                 ],
             )
             custom_run_colors = {}
             for runsets in runsetss:
                 custom_run_colors.update(
-                    {(runsets[idx].report_runset.name, runsets[idx].runs[0].config[runsets[idx].exp_name]): runsets[idx].color}
+                    {
+                        (
+                            runsets[idx].report_runset.name,
+                            runsets[idx].runs[0].config[runsets[idx].custom_exp_name_key],
+                        ): runsets[idx].color
+                    }
                 )
             pg.custom_run_colors = custom_run_colors  # IMPORTANT: custom_run_colors is implemented as a custom `setter` that needs to be overwritten unlike regular dictionaries
             blocks += [pg]
 
-    nrows = np.ceil(len(env_ids) / ncols).astype(int)
-    figsize = (ncols * 4, nrows * 3)
+    figsize = (pc.ncols * pc.cm, pc.nrows * pc.rm)
     fig, axes = plt.subplots(
-        nrows=nrows,
-        ncols=ncols,
+        nrows=pc.nrows,
+        ncols=pc.ncols,
         figsize=figsize,
-        # sharex=True,
+        sharex=pc.sharex,
         # sharey=True,
     )
     fig_time, axes_time = plt.subplots(
-        nrows=nrows,
-        ncols=ncols,
+        nrows=pc.nrows,
+        ncols=pc.ncols,
         figsize=figsize,
-        # sharex=True,
+        sharex=pc.sharex,
         # sharey=True,
     )
     if len(env_ids) == 1:
         axes = np.array([axes])
         axes_time = np.array([axes_time])
     axes_flatten = axes.flatten()
     axes_time_flatten = axes_time.flatten()
 
     result_table = pd.DataFrame(index=env_ids, columns=[runsets[0].name for runsets in runsetss])
     runtimes = []
     for idx, env_id in enumerate(env_ids):
         print(f"collecting runs for {env_id}")
         ex = expt.Experiment("Comparison")
         for runsets in runsetss:
-            h = create_hypothesis(runsets[idx].name, runsets[idx].runs, scan_history, runsets[idx].metric)
+            h = create_hypothesis(runsets[idx], scan_history)
             ex.add_hypothesis(h)
 
         # for each run `i` get the average of the last `rolling` episodes as r_i
         # then take the average and std of r_i as the results.
         result = []
         for hypothesis in ex.hypotheses:
             metric_result = []
             console.print(f"{hypothesis.name} has {len(hypothesis.runs)} runs", style="bold")
             for run in hypothesis.runs:
                 metric_result += [run.df["charts/episodic_return"].dropna()[-metric_last_n_average_window:].mean()]
 
                 # convert time unit in place
-                if time_unit == "m":
+                if pc.time_unit == "m":
                     run.df["_runtime"] /= 60
-                elif time_unit == "h":
+                elif pc.time_unit == "h":
                     run.df["_runtime"] /= 3600
             metric_result = np.array(metric_result)
-            result += [
-                f"{metric_result.mean():.2f} ± {metric_result.std():.2f}"
-            ]  # , {np.mean(runtimes):.2f} ± {np.std(runtimes):.2f}
+            result += [f"{metric_result.mean():.2f} ± {metric_result.std():.2f}"]
         result_table.loc[env_id] = result
         runtimes.append(list(ex.summary()["_runtime"]))
         ax = axes_flatten[idx]
         ex.plot(
             ax=ax,
             title=env_id,
             x="global_step",
             y="charts/episodic_return",
             err_style="band",
             std_alpha=0.1,
-            rolling=rolling,
+            n_samples=10000,
+            rolling=pc.rolling,
             colors=[runsets[idx].color for runsets in runsetss],
             legend=False,
         )
-        ax.set_xlabel(args.xlabel)
-        ax.set_ylabel(args.ylabel)
+        ax.set_xlabel("")
+        ax.set_ylabel("")
         ax_time = axes_time_flatten[idx]
         ex.plot(
             ax=ax_time,
             title=env_id,
             x="_runtime",
             y="charts/episodic_return",
             err_style="band",
             std_alpha=0.1,
-            rolling=rolling,
+            n_samples=10000,
+            rolling=pc.rolling,
             colors=[runsets[idx].color for runsets in runsetss],
             legend=False,
         )
-        ax_time.set_ylabel(args.ylabel)
-        ax_time.set_xlabel(f"Time ({time_unit})")
+        ax_time.set_xlabel("")
+        ax_time.set_ylabel("")
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
-    console.rule(f"[bold red]Runtime ({time_unit}) (mean ± std)")
+    console.rule(f"[bold red]Runtime ({pc.time_unit}) (mean ± std)")
     console.print(to_rich_table(runtimes.rename_axis("Environment").reset_index()))
-    console.rule(f"[bold red]{args.ylabel} (mean ± std)")
+    console.rule(f"[bold red]{pc.ylabel} (mean ± std)")
     console.print(to_rich_table(result_table.rename_axis("Environment").reset_index()))
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
-    console.rule(f"[bold red]Runtime ({time_unit}) Average")
+    console.rule(f"[bold red]Runtime ({pc.time_unit}) Average")
     average_runtime = pd.DataFrame(runtimes.mean(axis=0)).reset_index()
     average_runtime.columns = ["Environment", "Average Runtime"]
     console.print(to_rich_table(average_runtime))
 
     # add legend
     h, l = axes_flatten[0].get_legend_handles_labels()
-    fig.legend(h, l, loc="lower center", ncol=ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig.transFigure)
+    fig.legend(h, l, loc="lower center", ncol=pc.ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig.transFigure)
+    fig.supxlabel(pc.xlabel)
+    fig.supylabel(pc.ylabel)
+    fig.tight_layout()
     h, l = axes_time_flatten[0].get_legend_handles_labels()
     fig_time.legend(
-        h, l, loc="lower center", ncol=ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig_time.transFigure
+        h, l, loc="lower center", ncol=pc.ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig_time.transFigure
     )
+    fig_time.supxlabel(f"Time ({pc.time_unit})")
+    fig_time.supylabel(pc.ylabel)
+    fig_time.tight_layout()
 
     # remove the empty axes
     for ax in axes_flatten[len(env_ids) :]:
         ax.remove()
     for ax in axes_time_flatten[len(env_ids) :]:
         ax.remove()
 
@@ -297,114 +389,114 @@
     fig_time.savefig(f"{output_filename}-time.png", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.pdf", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.svg", bbox_inches="tight")
     return blocks
 
 
 if __name__ == "__main__":
-    args = parse_args()
+    args = tyro.cli(Args)
+    # by default assume all the env_ids are the same
+    if len(args.filters) > 1 and len(args.env_ids) == 1:
+        args.env_ids = args.env_ids * len(args.filters)
+    # calculate the number of rows
+    args.pc.nrows = np.ceil(len(args.env_ids[0]) / args.pc.ncols).astype(int)
+
     console = Console()
     blocks = []
     runsetss = []
-
+    offline_dbs = {}
     colors_flatten = sns.color_palette(n_colors=sum(len(filters) - 1 for filters in args.filters)).as_hex()
     colors = []
     for filters in args.filters:
         colors += [colors_flatten[: len(filters) - 1]]
         colors_flatten = colors_flatten[len(filters) - 1 :]
 
     for filters_idx, filters in enumerate(args.filters):
         parse_result = urlparse(filters[0])
         query = parse_qs(parse_result.query)
         metric = query["metric"][0] if "metric" in query else "charts/episodic_return"
         wandb_project_name = query["wpn"][0] if "wpn" in query else args.wandb_project_name
         wandb_entity = query["we"][0] if "we" in query else args.wandb_entity
         custom_env_id_key = query["ceik"][0] if "ceik" in query else "env_id"
-        custom_exp_name = query["cen"][0] if "cen" in query else "exp_name"
+        custom_exp_name_key = query["cen"][0] if "cen" in query else "exp_name"
         pprint(
             {
                 "wandb_project_name": wandb_project_name,
                 "wandb_entity": wandb_entity,
                 "custom_env_id_key": custom_env_id_key,
-                "custom_exp_name": custom_exp_name,
+                "custom_exp_name_key": custom_exp_name_key,
                 "metric": metric,
             },
             expand_all=True,
         )
+        if f"{wandb_entity}/{wandb_project_name}" not in offline_dbs:
+            offline_db_path = os.path.join(
+                openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}", "offline.sqlite"
+            )
+            print(offline_db_path)
+            offline_db = pw.SqliteDatabase(offline_db_path)
+            database_proxy.initialize(offline_db)
+            offline_db.connect()
+            offline_db.create_tables([OfflineRun, Tag, OfflineRunTag])
+            offline_dbs[f"{wandb_entity}/{wandb_project_name}"] = offline_db
 
         for filter_str, color in zip(filters[1:], colors[filters_idx]):
             print("=========", filter_str)
             # parse filter string
             parse_result = urlparse(filter_str)
             exp_name = parse_result.path
             query = parse_qs(parse_result.query)
-            user = [{"username": query["user"][0]}] if "user" in query else []
-            include_tag_groups = [{"tags": {"$in": [tag]}} for tag in query["tag"]] if "tag" in query else []
+            username = query["user"][0] if "user" in query else None
+            tags = query["tag"] if "tag" in query else []
             custom_legend = query["cl"][0] if "cl" in query else ""
-
             # HACK unescape
             custom_legend = custom_legend.replace("\\n", "\n")
 
             runsets = []
-            for env_id in args.env_ids:
-                # HACK
-                if "alepy" in exp_name:  # alepy experiments: `Breakout-v5` -> `ALE/Breakout-v5`
-                    env_id = f"ALE/{env_id}"
-                elif "envpool" not in exp_name:
-                    env_id = env_id.replace("-v4", "-v2")  # mujoco experiments: `HalfCheetah-v4` -> `HalfCheetah-v2`
-                    env_id = env_id.replace(
-                        "-v5", "NoFrameskip-v4"
-                    )  # old atari experiments: `Breakout-v5` -> `BreakoutNoFrameskip-v4`
-                if exp_name == "ppo_continuous_action" and "rlops-pilot" in query["tag"]:
-                    env_id = env_id.replace("-v4", "-v2")
-
+            for env_id in args.env_ids[filters_idx]:
                 runsets.append(
                     Runset(
                         name=f"{wandb_entity}/{wandb_project_name}/{exp_name} ({query})"
                         if custom_legend == ""
                         else custom_legend,
-                        filters={
-                            "$and": [
-                                {f"config.{custom_env_id_key}.value": env_id},
-                                *include_tag_groups,
-                                *user,
-                                {f"config.{custom_exp_name}.value": exp_name},
-                            ]
-                        },
                         entity=wandb_entity,
                         project=wandb_project_name,
-                        groupby=custom_exp_name,
-                        exp_name=custom_exp_name,
                         metric=metric,
+                        groupby=custom_exp_name_key,
+                        custom_exp_name_key=custom_exp_name_key,
+                        exp_name=exp_name,
+                        custom_env_id_key=custom_env_id_key,
+                        env_id=env_id,
+                        tags=tags,
+                        username=username,
                         color=color,
+                        offline_db=offline_dbs[f"{wandb_entity}/{wandb_project_name}"],
+                        offline=args.offline,
                     )
                 )
                 if args.check_empty_runs:
                     console.print(f"{exp_name} [green]({query})[/] in [purple]{env_id}[/] has {len(runsets[-1].runs)} runs")
                     for run in runsets[-1].runs:
                         console.print(f"┣━━ [link={run.url}]{run.name}[/link] with tags = {run.tags}")
                     assert len(runsets[0].runs) > 0, f"{exp_name} ({query}) in {env_id} has no runs"
             runsetss.append(runsets)
 
     blocks = compare(
         console,
         runsetss,
-        args.env_ids,
+        args.env_ids[0],
         output_filename=args.output_filename,
-        ncols=args.ncols,
-        ncols_legend=args.ncols_legend,
-        rolling=args.rolling,
         metric_last_n_average_window=args.metric_last_n_average_window,
         scan_history=args.scan_history,
         report=args.report,
-        time_unit=args.time_unit,
+        pc=args.pc,
     )
     if args.report:
         print("saving report")
         report = wb.Report(
-            project="cleanrl",
+            project=args.wandb_project_name,
             title=f"Regression Report: {exp_name}",
             description=str(args.filters),
             blocks=blocks,
         )
         report.save()
         print(f"view the generated report at {report.url}")
```

### Comparing `openrlbenchmark-0.1.1b4/openrlbenchmark/rlops_hns copy.py` & `openrlbenchmark-0.2.0b1/openrlbenchmark/rlops_hns.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,237 @@
-import argparse
 import copy
 import os
-from distutils.util import strtobool
 import pickle
+from collections import defaultdict
+from dataclasses import dataclass, field
 from typing import List, cast
 from urllib.parse import parse_qs, urlparse
 
 import expt
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import peewee as pw
 import seaborn as sns
+import tyro
 import wandb
 import wandb.apis.reports as wb  # noqa
 from expt import Hypothesis, Run
 from rich.console import Console
 from rich.pretty import pprint
+from rich.table import Table
+from rliable import library as rly
+from rliable import metrics, plot_utils
 
 import openrlbenchmark
 import openrlbenchmark.cache
 from openrlbenchmark.hns import atari_human_normalized_scores as atari_hns
+from openrlbenchmark.offline_db import OfflineRun, OfflineRunTag, Tag, database_proxy
 
-api = wandb.Api()
 
-
-def parse_args():
-    # fmt: off
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--filters", nargs="+", action="append", default=[],
-        help="the filters of the experiments; see docs")
-    parser.add_argument("--env-ids", nargs="+", default=["Hopper-v2", "Walker2d-v2", "HalfCheetah-v2"],
-        help="the ids of the environment to compare")
-    parser.add_argument("--output-filename", type=str, default="compare",
-        help="the output filename of the plot, without extension")
-    parser.add_argument("--rolling", type=int, default=100,
-        help="the rolling window for smoothing the curves")
-    parser.add_argument("--metric-last-n-average-window", type=int, default=100,
-        help="the last n number of episodes to average metric over in the result table")
-    parser.add_argument("--ncols", type=int, default=2,
-        help="the number of columns in the chart")
-    parser.add_argument("--ncols-legend", type=int, default=2,
-        help="the number of legend columns in the chart")
-    parser.add_argument("--scan-history", type=lambda x: bool(strtobool(x)), default=False, nargs="?", const=True,
-        help="if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)")
-    parser.add_argument("--check-empty-runs", type=lambda x: bool(strtobool(x)), default=True, nargs="?", const=True,
-        help="if toggled, we will check for empty wandb runs")
-    parser.add_argument("--time-unit", type=str, default="m", choices=["s", "m", "h"],
-        help="the unit of time in the x-axis of the chart (e.g., `s` for seconds, `m` for minutes, `h` for hours); default: `m`")
-    parser.add_argument("--report", type=lambda x: bool(strtobool(x)), default=False, nargs="?", const=True,
-        help="if toggled, a wandb report will be created")
-    parser.add_argument("--xlabel", type=str, default="Step",
-        help="the label of the x-axis")
-    parser.add_argument("--ylabel", type=str, default="Human-noramlized Score",
-        help="the label of the y-axis")
-    # fmt: on
-    return parser.parse_args()
-
-
-def create_hypothesis(
-    name: str, wandb_runs: List[wandb.apis.public.Run], scan_history: bool = False, metric: str = ""
-) -> Hypothesis:
-    runs = []
-    for idx, run in enumerate(wandb_runs):
-        print(run, run.url)
-        if scan_history:
-            # equivalent to `run_df = pd.DataFrame([row for row in run.scan_history()])`
-            run = openrlbenchmark.cache.CachedRun(run, cache_dir=os.path.join(openrlbenchmark.__path__[0], "dataset"))
-            run_df = run.run_df
-        else:
-            run_df = run.history(samples=1500)
-        if "videos" in run_df:
-            run_df = run_df.drop(columns=["videos"], axis=1)
-        if len(metric) > 0:
-            run_df["charts/episodic_return"] = run_df[metric]
-        cleaned_df = run_df[["global_step", "_runtime", "charts/episodic_return"]].dropna()
-        runs += [Run(f"seed{idx}", cleaned_df)]
-    return Hypothesis(name, runs)
+@dataclass
+class PlotConfig:
+    ncols: int = 2
+    """the number of columns in the chart"""
+    nrows: tyro.conf.Suppress[int] = None
+    """(TO BE FILLED in runtime) the number of rows in the chart"""
+    ncols_legend: int = 2
+    """the number of legend columns in the chart"""
+    xlabel: str = "Step"
+    """the label of the x-axis"""
+    ylabel: str = "Episodic Return"
+    """the label of the y-axis"""
+    sharex: bool = False
+    """if toggled, we will share the x-axis across all subplots"""
+    rolling: int = 100
+    """the rolling window for smoothing the curves"""
+    time_unit: str = "m"
+    """the unit of time in the x-axis of the chart (e.g., `s` for seconds, `m` for minutes, `h` for hours); default: `m`"""
+    cm: float = 4.0
+    """the multiplier for the column width"""
+    rm: float = 3.0
+    """the multiplier for the row height"""
+    hspace: float = None
+    """the height space between subplots"""
+    wspace: float = None
+    """the width space between subplots"""
+    nsubsamples: int = 20
+    """the number of subsamples to take from the wandb runs for IQM"""
+
+
+@dataclass
+class Args:
+    filters: tyro.conf.UseAppendAction[List[List[str]]]
+    """the filters of the experiments; see docs"""
+    env_ids: tyro.conf.UseAppendAction[List[List[str]]]
+    """the ids of the environment to compare"""
+    output_filename: str = "compare"
+    """the output filename of the plot, without extension"""
+    metric_last_n_average_window: int = 100
+    """the last n number of episodes to average metric over in the result table"""
+    scan_history: bool = False
+    """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
+    check_empty_runs: bool = False
+    """if toggled, we will check for empty wandb runs"""
+    report: bool = False
+    """if toggled, a wandb report will be created"""
+    wandb_project_name: str = "cleanrl"
+    """the wandb project name for the report creation"""
+    offline: bool = False
+    """if toggled, we will use the offline database instead of wandb"""
+    pc: tyro.conf.OmitSubcommandPrefixes[PlotConfig] = field(default_factory=PlotConfig)
+    """the plot configuration"""
+    rliable: bool = False
+    """if toggled, we will use rliable to compute the metrics"""
 
 
 class Runset:
     def __init__(
         self,
         name: str,
-        filters: dict,
         entity: str,
         project: str,
-        groupby: str = "",
-        exp_name: str = "exp_name",
         metric: str = "charts/episodic_return",
+        groupby: str = "",
+        custom_exp_name_key: str = "exp_name",
+        exp_name: str = "",
+        custom_env_id_key: str = "env_id",
+        env_id: str = "",
+        tags: List[str] = [],
+        username: str = "",
         color: str = "#000000",
+        offline_db: pw.Database = None,
+        offline: bool = False,
     ):
         self.name = name
-        self.filters = filters
         self.entity = entity
         self.project = project
+        self.metric = metric
         self.groupby = groupby
+        self.custom_exp_name_key = custom_exp_name_key
         self.exp_name = exp_name
-        self.metric = metric
+        self.custom_env_id_key = custom_env_id_key
+        self.env_id = env_id
         self.color = color
+        self.tags = tags
+        self.username = username
+        self.offline_db = offline_db
+        self.offline = offline
+
+        user = [{"username": self.username}] if self.username else []
+        include_tag_groups = [{"tags": {"$in": [tag]}} for tag in self.tags] if len(self.tags) > 0 else []
+        self.wandb_filters = {
+            "$and": [
+                {f"config.{self.custom_env_id_key}.value": self.env_id},
+                *include_tag_groups,
+                *user,
+                {f"config.{self.custom_exp_name_key}.value": self.exp_name},
+            ]
+        }
 
     @property
     def runs(self):
-        return wandb.Api().runs(path=f"{self.entity}/{self.project}", filters=self.filters)
+        if not self.offline:
+            return wandb.Api().runs(
+                path=f"{self.entity}/{self.project}",
+                filters=self.wandb_filters,
+            )
+        else:
+            with self.offline_db.bind_ctx([OfflineRun, OfflineRunTag, Tag]):
+                cond = (
+                    (OfflineRun.project == self.project)
+                    & (OfflineRun.entity == self.entity)
+                    & (OfflineRun.config[self.custom_env_id_key] == self.env_id)
+                    & (OfflineRun.config[self.custom_exp_name_key] == self.exp_name)
+                )
+                if self.username:
+                    cond = cond and OfflineRun.username == self.username
+                if len(self.tags) > 0:
+                    for tag_str in self.tags:
+                        cond = cond & (Tag.name == tag_str)
+                    query = OfflineRun.select().join(OfflineRunTag).join(Tag).where(cond)
+                else:
+                    query = OfflineRun.select().where(cond)
+                g = [run for run in query]
+
+            return g
 
     @property
     def report_runset(self):
         return wb.Runset(
             name=self.name,
             entity=self.entity,
             project=self.project,
-            filters={"$or": [self.filters]},
+            filters={"$or": [self.wandb_filters]},
             groupby=[self.groupby] if len(self.groupby) > 0 else None,
         )
 
 
+def to_rich_table(df: pd.DataFrame) -> Table:
+    table = Table()
+    for column in df.columns:
+        table.add_column(column)
+    for _, row in df.iterrows():
+        table.add_row(*row.astype(str).tolist())
+    return table
+
+
+def create_hypothesis(runset: Runset, scan_history: bool = False) -> Hypothesis:
+    runs = []
+    for idx, run in enumerate(runset.runs):
+        print("loading", run, run.url)
+        if run.state == "running":
+            print(f"Skipping running run: {run}")
+            continue
+        if scan_history:
+            run = openrlbenchmark.cache.CachedRun(run, cache_dir=os.path.join(openrlbenchmark.__path__[0], "dataset"))
+            with runset.offline_db.bind_ctx([OfflineRun, OfflineRunTag, Tag]):
+                tags = []
+                for tag_str in run.run.tags:
+                    tag = Tag.get_or_none(name=tag_str)
+                    if not tag:
+                        tag = Tag.create(name=tag_str)
+                        tag.save()
+                    tags.append(tag)
+                offline_run = OfflineRun.get_or_none(id=run.run.id)
+                if not offline_run:
+                    offline_run = OfflineRun.create(
+                        id=run.run.id,
+                        name=run.run.name,
+                        state=run.run.state,
+                        url=run.run.url,
+                        path=run.run.path,
+                        username=run.run.user.username,
+                        tags=tags,
+                        project=run.run.project,
+                        entity=run.run.entity,
+                        config=run.run.config if isinstance(run.run.config, dict) else run.run.config.toDict(),
+                    )
+                    offline_run.save()
+            run_df = run.run_df
+        else:
+            run_df = run.history(samples=1500)
+        if "videos" in run_df:
+            run_df = run_df.drop(columns=["videos"], axis=1)
+        if len(runset.metric) > 0:
+            run_df["charts/episodic_return"] = run_df[runset.metric]
+        cleaned_df = run_df[["global_step", "_runtime", "charts/episodic_return"]].dropna()
+        runs += [Run(f"seed{idx}", cleaned_df)]
+    return Hypothesis(runset.name, runs)
+
+
 def compare(
+    console: Console,
     runsetss: List[List[Runset]],
     env_ids: List[str],
-    ncols: int,
-    ncols_legend: int,
-    rolling: int,
     metric_last_n_average_window: int,
     scan_history: bool = False,
     output_filename: str = "compare",
     report: bool = False,
-    time_unit: str = "m",
+    pc: PlotConfig = None,
 ):
     blocks = []
     if report:
         for idx, env_id in enumerate(env_ids):
             metric_over_step = wb.LinePlot(
                 x="global_step",
                 y=list({runsets[idx].metric for runsets in runsetss}),
@@ -162,130 +265,179 @@
                     #     media_keys="videos",
                     # ),
                 ],
             )
             custom_run_colors = {}
             for runsets in runsetss:
                 custom_run_colors.update(
-                    {(runsets[idx].report_runset.name, runsets[idx].runs[0].config[runsets[idx].exp_name]): runsets[idx].color}
+                    {
+                        (
+                            runsets[idx].report_runset.name,
+                            runsets[idx].runs[0].config[runsets[idx].custom_exp_name_key],
+                        ): runsets[idx].color
+                    }
                 )
             pg.custom_run_colors = custom_run_colors  # IMPORTANT: custom_run_colors is implemented as a custom `setter` that needs to be overwritten unlike regular dictionaries
             blocks += [pg]
 
-    nrows = np.ceil(len(env_ids) / ncols).astype(int)
-    figsize = (ncols * 4, nrows * 3)
+    figsize = (pc.ncols * pc.cm, pc.nrows * pc.rm)
     fig, axes = plt.subplots(
-        nrows=nrows,
-        ncols=ncols,
+        nrows=pc.nrows,
+        ncols=pc.ncols,
         figsize=figsize,
-        # sharex=True,
+        sharex=pc.sharex,
         # sharey=True,
     )
     fig_time, axes_time = plt.subplots(
-        nrows=nrows,
-        ncols=ncols,
+        nrows=pc.nrows,
+        ncols=pc.ncols,
         figsize=figsize,
-        # sharex=True,
+        sharex=pc.sharex,
         # sharey=True,
     )
     if len(env_ids) == 1:
         axes = np.array([axes])
         axes_time = np.array([axes_time])
     axes_flatten = axes.flatten()
     axes_time_flatten = axes_time.flatten()
 
     result_table = pd.DataFrame(index=env_ids, columns=[runsets[0].name for runsets in runsetss])
+    hns_result_table = pd.DataFrame(index=env_ids, columns=[runsets[0].name for runsets in runsetss])
+    min_num_seeds_per_hypothesis = {}
+    for runsets in runsetss:
+        min_num_seeds_per_hypothesis[runsets[0].name] = float("inf")
     exs = []
     runtimes = []
     for idx, env_id in enumerate(env_ids):
+        print(f"collecting runs for {env_id}")
         ex = expt.Experiment("Comparison")
         for runsets in runsetss:
-            h = create_hypothesis(runsets[idx].name, runsets[idx].runs, scan_history, runsets[idx].metric)
-            ex.add_hypothesis(h)
+            hypo = create_hypothesis(runsets[idx], scan_history)
+            ex.add_hypothesis(hypo)
         exs.append(ex)
 
         # for each run `i` get the average of the last `rolling` episodes as r_i
         # then take the average and std of r_i as the results.
         result = []
+        hns_result = []
         for hypothesis in ex.hypotheses:
             metric_result = []
+            hns_metric_result = []
+            console.print(f"{hypothesis.name} has {len(hypothesis.runs)} runs", style="bold")
+            min_num_seeds_per_hypothesis[hypothesis.name] = min(
+                min_num_seeds_per_hypothesis[hypothesis.name], len(hypothesis.runs)
+            )
             for run in hypothesis.runs:
-                # calculate hns
-                run.df["charts/episodic_return"] = (run.df["charts/episodic_return"] - atari_hns[env_id][0]) / (atari_hns[env_id][1] - atari_hns[env_id][0])
+                # HACK: handle different Atari env id types.
+                standard_env_id = env_id
+                if env_id.endswith("NoFrameskip-v4"):
+                    standard_env_id = env_id.replace("NoFrameskip-v4", "-v5")
+                run.df["hns"] = (run.df["charts/episodic_return"] - atari_hns[standard_env_id][0]) / (
+                    atari_hns[standard_env_id][1] - atari_hns[standard_env_id][0]
+                )
                 metric_result += [run.df["charts/episodic_return"].dropna()[-metric_last_n_average_window:].mean()]
+                hns_metric_result += [run.df["hns"].dropna()[-metric_last_n_average_window:].mean()]
 
                 # convert time unit in place
-                if time_unit == "m":
+                if pc.time_unit == "m":
                     run.df["_runtime"] /= 60
-                elif time_unit == "h":
+                elif pc.time_unit == "h":
                     run.df["_runtime"] /= 3600
             metric_result = np.array(metric_result)
-            result += [f"{metric_result.mean():.2f} ± {metric_result.std():.2f}"] # , {np.mean(runtimes):.2f} ± {np.std(runtimes):.2f}
+            hns_metric_result = np.array(hns_metric_result)
+            result += [f"{metric_result.mean():.2f} ± {metric_result.std():.2f}"]
+            hns_result += [f"{hns_metric_result.mean():.2f} ± {hns_metric_result.std():.2f}"]
         result_table.loc[env_id] = result
-        # print(env_id, ex.summary())
+        hns_result_table.loc[env_id] = hns_result
         runtimes.append(list(ex.summary()["_runtime"]))
         ax = axes_flatten[idx]
         ex.plot(
             ax=ax,
             title=env_id,
             x="global_step",
             y="charts/episodic_return",
             err_style="band",
             std_alpha=0.1,
-            rolling=rolling,
+            n_samples=10000,
+            rolling=pc.rolling,
             colors=[runsets[idx].color for runsets in runsetss],
-            # n_samples=500,
             legend=False,
         )
-        ax.set_xlabel(args.xlabel)
-        ax.set_ylabel(args.ylabel)
+        ax.set_xlabel("")
+        ax.set_ylabel("")
+        ax2 = ax.twinx()
+        ax2.set_ylim([0, ex.summary()["hns"].max()])
         ax_time = axes_time_flatten[idx]
         ex.plot(
             ax=ax_time,
             title=env_id,
             x="_runtime",
             y="charts/episodic_return",
             err_style="band",
             std_alpha=0.1,
-            rolling=rolling,
+            n_samples=10000,
+            rolling=pc.rolling,
             colors=[runsets[idx].color for runsets in runsetss],
-            # n_samples=500,
             legend=False,
         )
-        ax_time.set_ylabel(args.ylabel)
-        ax_time.set_xlabel(f"Time ({time_unit})")
+        ax_time.set_xlabel("")
+        ax_time.set_ylabel("")
+        ax_time2 = ax_time.twinx()
+        ax_time2.set_ylim([0, ex.summary()["hns"].max()])
+
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
-    print("runtimes", runtimes)
-    
+    console.rule(f"[bold red]Runtime ({pc.time_unit}) (mean ± std)")
+    console.print(to_rich_table(runtimes.rename_axis("Environment").reset_index()))
+
     # for each run set, for each seed, plot 57 curves and get their median curves, then plot the average of the median curves
     hns_ex = expt.Experiment("Human Normalized Score")
+    hns_dict = {}
+    max_global_steps = defaultdict(int)
     for runsets_idx, runsets in enumerate(runsetss):
+        hns_dict[runsets[0].name] = np.zeros((min_num_seeds_per_hypothesis[runsets[0].name], len(env_ids), pc.nsubsamples))
         # for each seed
         median_curves = []
-        for seed_idx, _ in enumerate(exs[0][runsets_idx]):
+        for seed_idx, _ in enumerate(range(min_num_seeds_per_hypothesis[runsets[0].name])):  # exs[0][runsets_idx]
+            min_global_step = float("inf")
+            print(f"collecting runs for {runsets[0].name} seed {seed_idx}")
+
             runs_of_one_seed = []
             for ex_idx, ex in enumerate(exs):
-                runs_of_one_seed.append(ex[runsets_idx][seed_idx])
+                run_of_one_seed = ex[runsets_idx][seed_idx]
+                min_global_step = min(min_global_step, run_of_one_seed.df["global_step"].iloc[-1])
+                runs_of_one_seed.append(run_of_one_seed)
+
+                # interpolate
+                x_samples = np.linspace(
+                    min(run_of_one_seed.df["global_step"]), max(run_of_one_seed.df["global_step"]), num=pc.nsubsamples
+                )
+                hns_dict[runsets[0].name][seed_idx, ex_idx, :] = np.interp(
+                    x_samples, run_of_one_seed.df["global_step"], run_of_one_seed.df["hns"]
+                )
+
             temp_fig, temp_axe = plt.subplots(nrows=1, ncols=1)
-            Hypothesis("seed", runs_of_one_seed).plot(
+            temp_hypo = Hypothesis("seed", runs_of_one_seed)
+            temp_hypo.plot(
                 ax=temp_axe,
                 title="Human Normalized Score",
                 x="global_step",
-                y="charts/episodic_return",
+                y="hns",
                 err_style="band",
-                rolling=rolling,
-                representative_fn=lambda h: cast(pd.DataFrame, h.grouped.median()), # median curve
+                rolling=pc.rolling,
+                n_samples=10000,
+                representative_fn=lambda h: cast(pd.DataFrame, h.grouped.median()),  # median curve
                 legend=False,
             )
-            # Hypothesis("seed", runs_of_one_seed).plot( ax=temp_axe, title="Human Normalized Score", x="global_step", y="charts/episodic_return", err_style="band", rolling=rolling, representative_fn=lambda h: cast(pd.DataFrame, h.grouped.median()))
             assert len(temp_axe.lines) == 1
             median_of_runs_of_one_seed = temp_axe.lines[0].get_xydata()
-            median_curves.append(median_of_runs_of_one_seed)
+            print(f"min_global_step: {min_global_step}")
+            max_global_steps[runsets[0].name] = max(max_global_steps[runsets[0].name], min_global_step)
+            median_curves.append(median_of_runs_of_one_seed[median_of_runs_of_one_seed[:, 0] < min_global_step])
             plt.close(temp_fig)
-        
+
         runs = []
         for median_curve_idx, median_curve in enumerate(median_curves):
             run_df = pd.DataFrame(median_curve, columns=["global_step", "charts/episodic_return"])
             runs.append(Run(f"median_curve_idx:{median_curve_idx}", run_df))
         hns_ex.add_hypothesis(Hypothesis(runsets[0].name, runs))
 
     ncols = 2
@@ -293,184 +445,274 @@
     figsize = (ncols * 4, nrows * 3)
     fig_median_hns, axes_median_hns = plt.subplots(
         nrows=nrows,
         ncols=ncols,
         figsize=figsize,
         sharey=True,
     )
-
-    # fig_median_hns, ax_median_hns = plt.subplots(
-    #     nrows=1,
-    #     ncols=2,
-    # )
     hns_ex.plot(
+        title=" ",
         ax=axes_median_hns[0],
         x="global_step",
         y="charts/episodic_return",
-        err_style="band",
+        err_style="unit_traces",
         std_alpha=0.1,
-        rolling=rolling,
+        n_samples=10000,
+        rolling=pc.rolling,
         colors=[runsets[0].color for runsets in runsetss],
         legend=False,
     )
     hns_ex_time = copy.deepcopy(hns_ex)
     for hypo_idx, hypo in enumerate(hns_ex_time.hypotheses):
         for run_idx in range(len(hypo.runs)):
-            hypo.runs[run_idx].df["_runtime"] = np.linspace(0, runtimes.mean(axis=0).iloc[hypo_idx], len(hypo.runs[run_idx].df))
+            hypo.runs[run_idx].df["_runtime"] = np.linspace(
+                0, runtimes.mean(axis=0).iloc[hypo_idx], len(hypo.runs[run_idx].df)
+            )
 
-    axes_median_hns[0].set_ylabel(args.ylabel)
+    axes_median_hns[0].set_ylabel("Median Human Normalized Score")
     axes_median_hns[0].set_xlabel(f"Steps")
     hns_ex_time.plot(
+        title=" ",
         ax=axes_median_hns[1],
         x="_runtime",
         y="charts/episodic_return",
-        err_style="band",
+        err_style="unit_traces",
         std_alpha=0.1,
-        rolling=rolling,
+        n_samples=10000,
+        rolling=pc.rolling,
         colors=[runsets[0].color for runsets in runsetss],
         legend=False,
     )
+    axes_median_hns[1].set_xlabel(f"Time ({pc.time_unit})")
     h, l = axes_median_hns[0].get_legend_handles_labels()
-    fig_median_hns.legend(h, l, loc="lower center", ncol=ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig_median_hns.transFigure)
-    fig_median_hns.savefig(f"{output_filename}_median_hns.png", bbox_inches="tight")
-    fig_median_hns.savefig(f"{output_filename}_median_hns.pdf", bbox_inches="tight")
-
-
-    # with open(f"{output_filename}_median_hns.pkl", 'wb') as f:
-    #     pickle.dump([line.get_xydata() for line in ax_median_hns.lines], f)
-    print("result_table", result_table)
+    fig_median_hns.legend(
+        h, l, loc="lower center", ncol=pc.ncols_legend, bbox_to_anchor=(0.5, 0.9), bbox_transform=fig_median_hns.transFigure
+    )
+    fig_median_hns.savefig(f"{output_filename}_hns_median.png", bbox_inches="tight")
+    fig_median_hns.savefig(f"{output_filename}_hns_median.pdf", bbox_inches="tight")
+    with open(f"{output_filename}_hns_median.pkl", "wb") as f:
+        pickle.dump(
+            [(line.get_color(), line.get_alpha(), line.get_xydata(), line.get_label()) for line in axes_median_hns[0].lines], f
+        )
+    console.rule(f"[bold red]{pc.ylabel} (mean ± std)")
+    console.print(to_rich_table(result_table.rename_axis("Environment").reset_index()))
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
+
+    console.rule(f"[bold red]Human-noramlized Score (mean ± std)")
+    console.print(to_rich_table(hns_result_table.rename_axis("Environment").reset_index()))
+    hns_result_table.to_markdown(open(f"{output_filename}_hns.md", "w"))
+    hns_result_table.to_csv(open(f"{output_filename}_hns.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
-    print("runtimes", runtimes.mean(axis=0))
+    console.rule(f"[bold red]Runtime ({pc.time_unit}) Average")
+    average_runtime = pd.DataFrame(runtimes.mean(axis=0)).reset_index()
+    average_runtime.columns = ["Environment", "Average Runtime"]
+    console.print(to_rich_table(average_runtime))
 
     # add legend
     h, l = axes_flatten[0].get_legend_handles_labels()
-    fig.legend(h, l, loc="lower center", ncol=ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig.transFigure)
+    fig.legend(h, l, loc="lower center", ncol=pc.ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig.transFigure)
+    fig.supxlabel(pc.xlabel)
+    fig.supylabel(pc.ylabel)
+    fig.text(0.99, 0.5, "Human-Normalized Score", va="center", rotation=-90)
+    fig.tight_layout()
     h, l = axes_time_flatten[0].get_legend_handles_labels()
     fig_time.legend(
-        h, l, loc="lower center", ncol=ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig_time.transFigure
+        h, l, loc="lower center", ncol=pc.ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig_time.transFigure
     )
+    fig_time.supxlabel(f"Time ({pc.time_unit})")
+    fig_time.supylabel(pc.ylabel)
+    fig_time.tight_layout()
 
     # remove the empty axes
     for ax in axes_flatten[len(env_ids) :]:
         ax.remove()
     for ax in axes_time_flatten[len(env_ids) :]:
         ax.remove()
 
-    print(f"saving figure to {output_filename}")
+    print(f"saving figures and tables to {output_filename}")
     if os.path.dirname(output_filename) != "":
         os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     fig.savefig(f"{output_filename}.png", bbox_inches="tight")
     fig.savefig(f"{output_filename}.pdf", bbox_inches="tight")
     fig.savefig(f"{output_filename}.svg", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.png", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.pdf", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.svg", bbox_inches="tight")
-    return blocks
+    return blocks, hns_dict, max_global_steps
 
 
 if __name__ == "__main__":
-    args = parse_args()
-    # raise
+    args = tyro.cli(Args)
+    # by default assume all the env_ids are the same
+    if len(args.filters) > 1 and len(args.env_ids) == 1:
+        args.env_ids = args.env_ids * len(args.filters)
+    # calculate the number of rows
+    args.pc.nrows = np.ceil(len(args.env_ids[0]) / args.pc.ncols).astype(int)
+
     console = Console()
     blocks = []
     runsetss = []
-
+    offline_dbs = {}
     colors_flatten = sns.color_palette(n_colors=sum(len(filters) - 1 for filters in args.filters)).as_hex()
     colors = []
     for filters in args.filters:
         colors += [colors_flatten[: len(filters) - 1]]
         colors_flatten = colors_flatten[len(filters) - 1 :]
 
     for filters_idx, filters in enumerate(args.filters):
         parse_result = urlparse(filters[0])
         query = parse_qs(parse_result.query)
         metric = query["metric"][0] if "metric" in query else "charts/episodic_return"
         wandb_project_name = query["wpn"][0] if "wpn" in query else args.wandb_project_name
         wandb_entity = query["we"][0] if "we" in query else args.wandb_entity
         custom_env_id_key = query["ceik"][0] if "ceik" in query else "env_id"
-        custom_exp_name = query["cen"][0] if "cen" in query else "exp_name"
+        custom_exp_name_key = query["cen"][0] if "cen" in query else "exp_name"
         pprint(
             {
                 "wandb_project_name": wandb_project_name,
                 "wandb_entity": wandb_entity,
                 "custom_env_id_key": custom_env_id_key,
-                "custom_exp_name": custom_exp_name,
+                "custom_exp_name_key": custom_exp_name_key,
                 "metric": metric,
             },
             expand_all=True,
         )
+        if f"{wandb_entity}/{wandb_project_name}" not in offline_dbs:
+            offline_db_path = os.path.join(
+                openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}", "offline.sqlite"
+            )
+            print(offline_db_path)
+            offline_db = pw.SqliteDatabase(offline_db_path)
+            database_proxy.initialize(offline_db)
+            offline_db.connect()
+            offline_db.create_tables([OfflineRun, Tag, OfflineRunTag])
+            offline_dbs[f"{wandb_entity}/{wandb_project_name}"] = offline_db
 
         for filter_str, color in zip(filters[1:], colors[filters_idx]):
             print("=========", filter_str)
             # parse filter string
             parse_result = urlparse(filter_str)
             exp_name = parse_result.path
             query = parse_qs(parse_result.query)
-            user = [{"username": query["user"][0]}] if "user" in query else []
-            include_tag_groups = [{"tags": {"$in": [tag]}} for tag in query["tag"]] if "tag" in query else []
+            username = query["user"][0] if "user" in query else None
+            tags = query["tag"] if "tag" in query else []
             custom_legend = query["cl"][0] if "cl" in query else ""
-
             # HACK unescape
             custom_legend = custom_legend.replace("\\n", "\n")
 
             runsets = []
-            for env_id in args.env_ids:
-                # HACK
-                if "alepy" in exp_name: # alepy experiments: `Breakout-v5` -> `ALE/Breakout-v5`
-                    env_id = f"ALE/{env_id}"
-                elif "envpool" not in exp_name:
-                    env_id = env_id.replace("-v4", "-v2") # mujoco experiments: `HalfCheetah-v4` -> `HalfCheetah-v2`
-                    env_id = env_id.replace("-v5", "NoFrameskip-v4") # old atari experiments: `Breakout-v5` -> `BreakoutNoFrameskip-v4`
-                if exp_name == "ppo_continuous_action" and "rlops-pilot" in query["tag"]:
-                    env_id = env_id.replace("-v4", "-v2")
-
+            for env_id in args.env_ids[filters_idx]:
                 runsets.append(
                     Runset(
-                        name=f"{wandb_entity}/{wandb_project_name}/{exp_name} ({query})" if custom_legend == "" else custom_legend,
-                        filters={
-                            "$and": [
-                                {f"config.{custom_env_id_key}.value": env_id},
-                                *include_tag_groups,
-                                *user,
-                                {f"config.{custom_exp_name}.value": exp_name},
-                            ]
-                        },
+                        name=f"{wandb_entity}/{wandb_project_name}/{exp_name} ({query})"
+                        if custom_legend == ""
+                        else custom_legend,
                         entity=wandb_entity,
                         project=wandb_project_name,
-                        groupby=custom_exp_name,
-                        exp_name=custom_exp_name,
                         metric=metric,
+                        groupby=custom_exp_name_key,
+                        custom_exp_name_key=custom_exp_name_key,
+                        exp_name=exp_name,
+                        custom_env_id_key=custom_env_id_key,
+                        env_id=env_id,
+                        tags=tags,
+                        username=username,
                         color=color,
+                        offline_db=offline_dbs[f"{wandb_entity}/{wandb_project_name}"],
+                        offline=args.offline,
                     )
                 )
                 if args.check_empty_runs:
                     console.print(f"{exp_name} [green]({query})[/] in [purple]{env_id}[/] has {len(runsets[-1].runs)} runs")
                     for run in runsets[-1].runs:
                         console.print(f"┣━━ [link={run.url}]{run.name}[/link] with tags = {run.tags}")
                     assert len(runsets[0].runs) > 0, f"{exp_name} ({query}) in {env_id} has no runs"
             runsetss.append(runsets)
 
-    blocks = compare(
+    blocks, hns_dict, max_global_steps = compare(
+        console,
         runsetss,
-        args.env_ids,
+        args.env_ids[0],
         output_filename=args.output_filename,
-        ncols=args.ncols,
-        ncols_legend=args.ncols_legend,
-        rolling=args.rolling,
         metric_last_n_average_window=args.metric_last_n_average_window,
         scan_history=args.scan_history,
         report=args.report,
-        time_unit=args.time_unit,
+        pc=args.pc,
     )
+    if args.rliable:
+        print("plotting sample efficiency curve")
+        exp_names = list(reversed(list(hns_dict.keys())))
+        colors_flatten = sns.color_palette(n_colors=sum(len(filters) - 1 for filters in args.filters)).as_hex()
+        colors = dict(zip(list(hns_dict.keys()), colors_flatten))
+        frames = np.linspace(0, max(max_global_steps.values()), args.pc.nsubsamples)
+        fig_rly_hns, axes_rly_hns = plt.subplots(ncols=2, figsize=(7 * 2, 3.4))
+        iqm = lambda scores: np.array([metrics.aggregate_iqm(scores[..., frame]) for frame in range(scores.shape[-1])])
+        iqm_scores, iqm_cis = rly.get_interval_estimates(hns_dict, iqm, reps=50000)
+        plot_utils.plot_sample_efficiency_curve(
+            frames + 1,
+            iqm_scores,
+            iqm_cis,
+            algorithms=exp_names,
+            colors=colors,
+            xlabel=r"Steps",
+            ax=axes_rly_hns[0],
+            ylabel="IQM Human Normalized Score",
+            labelsize="x-large",
+            ticklabelsize="x-large",
+        )
+        expt.plot.autoformat_xaxis(axes_rly_hns[0])
+
+        print("plotting performance profiles")
+        atari_200m_thresholds = np.linspace(0.0, 8.0, 81)
+        atari_200m_normalized_score_dict = {}
+        for key, value in hns_dict.items():
+            atari_200m_normalized_score_dict[key] = np.nanmean(value[:, :, -1:], axis=-1)
+        score_distributions, score_distributions_cis = rly.create_performance_profile(
+            atari_200m_normalized_score_dict, atari_200m_thresholds
+        )
+        plot_utils.plot_performance_profiles(
+            score_distributions,
+            atari_200m_thresholds,
+            performance_profile_cis=score_distributions_cis,
+            colors=colors,
+            xlabel=r"Human Normalized Score $(\tau)$",
+            ax=axes_rly_hns[1],
+        )
+        fig_rly_hns.savefig(f"{args.output_filename}_iqm_profile.png", bbox_inches="tight")
+        fig_rly_hns.savefig(f"{args.output_filename}_iqm_profile.pdf", bbox_inches="tight")
+
+        print("plotting aggregate metrics")
+        aggregate_func = lambda x: np.array(
+            [
+                metrics.aggregate_median(x),
+                metrics.aggregate_iqm(x),
+                metrics.aggregate_mean(x),
+                metrics.aggregate_optimality_gap(x),
+            ]
+        )
+        aggregate_scores, aggregate_score_cis = rly.get_interval_estimates(
+            atari_200m_normalized_score_dict, aggregate_func, reps=50000
+        )
+        fig, axes = plot_utils.plot_interval_estimates(
+            aggregate_scores,
+            aggregate_score_cis,
+            metric_names=["Median", "IQM", "Mean", "Optimality Gap"],
+            algorithms=exp_names,
+            colors=colors,
+            # xlabel='Human Normalized Score',
+            xlabel="",
+        )
+        plt.savefig(f"{args.output_filename}_hns_aggregate.png", bbox_inches="tight")
+        plt.savefig(f"{args.output_filename}_hns_aggregate.pdf", bbox_inches="tight")
+
     if args.report:
         print("saving report")
         report = wb.Report(
-            project="cleanrl",
+            project=args.wandb_project_name,
             title=f"Regression Report: {exp_name}",
             description=str(args.filters),
             blocks=blocks,
         )
         report.save()
         print(f"view the generated report at {report.url}")
```

### Comparing `openrlbenchmark-0.1.1b4/pyproject.toml` & `openrlbenchmark-0.2.0b1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 [tool.poetry]
 name = "openrlbenchmark"
-version = "0.1.1b4"
+version = "0.2.0b1"
 description = ""
 authors = ["Costa Huang <costa.huang@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
+python = ">=3.7.1,<3.11"
 wandb = "^0.13.7"
 pip = "^22.1.2"
 expt = "^0.4.1"
 multiprocess = "^0.70.13"
 tueplots = "^0.0.4"
 seaborn = "^0.12.1"
 rich = "<12.0"
 tabulate = "^0.9.0"
 importlib-metadata = "^5.1.0"
 tqdm = "^4.65.0"
+tyro = "^0.5.0"
+dotmap = "^1.3.30"
+peewee = "^3.16.2"
+rliable = "^1.0.8"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.20.0"
 
 [tool.poetry.group.dev.dependencies]
 notebook = "^6.5.2"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openrlbenchmark-0.1.1b4/setup.py` & `openrlbenchmark-0.2.0b1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,36 +4,40 @@
 packages = \
 ['openrlbenchmark']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['expt>=0.4.1,<0.5.0',
+['dotmap>=1.3.30,<2.0.0',
+ 'expt>=0.4.1,<0.5.0',
  'importlib-metadata>=5.1.0,<6.0.0',
  'multiprocess>=0.70.13,<0.71.0',
+ 'peewee>=3.16.2,<4.0.0',
  'pip>=22.1.2,<23.0.0',
  'rich<12.0',
+ 'rliable>=1.0.8,<2.0.0',
  'seaborn>=0.12.1,<0.13.0',
  'tabulate>=0.9.0,<0.10.0',
  'tqdm>=4.65.0,<5.0.0',
  'tueplots>=0.0.4,<0.0.5',
+ 'tyro>=0.5.0,<0.6.0',
  'wandb>=0.13.7,<0.14.0']
 
 setup_kwargs = {
     'name': 'openrlbenchmark',
-    'version': '0.1.1b4',
+    'version': '0.2.0b1',
     'description': '',
-    'long_description': '# Open RL Benchmark: Comprehensive Tracked Experiments for Reinforcement Learning\n\n\n[<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openrlbenchmark/openrlbenchmark/blob/master/README.ipynb)\n[<img src="https://dcbadge.vercel.app/api/server/GsmqhDcea5?style=flat">](https://discord.gg/GsmqhDcea5)\n\n\n\nOpen RL Benchmark is a comprehensive collection of tracked experiments for RL. It aims to make it easier for RL practitioners to pull and compare all kinds of metrics from reputable RL libraries like Stable-baselines3, Tianshou, CleanRL, and others.\n\n* 💾 [GitHub Repo](https://github.com/openrlbenchmark/openrlbenchmark): source code and more docs.\n* 📜 [Design docs](https://docs.google.com/document/d/1cDI_AMr2QVmkC53dCHFMYwGJtLC8V4p6KdL2wnYPaiI/edit?usp=sharing): our motivation and vision.\n* 🔗 [Open RL Benchmark reports](https://wandb.ai/openrlbenchmark/openrlbenchmark/reportlist):  W&B reports with tracked Atari, MuJoCo experiments from SB3, CleanRL, and others.\n\n\n\n## Installation\nYou can install it via pip or the dev setup.\n\n### Pip install\n\n```shell\npip install openrlbenchmark --upgrade\n```\n\n### Dev Setup\n\nPrerequisites:\n* Python >=3.7.1,<3.10 (not yet 3.10)\n* [Poetry 1.2.1+](https://python-poetry.org)\n\n```shell\ngit clone https://github.com/openrlbenchmark/openrlbenchmark.git\ncd openrlbenchmark\npoetry install\n```\n\n\n## Get started\n\nOpen RL Benchmark provides an RLops CLI to pull and compare metrics from Weights and Biases. The following example shows how to compare the performance of SB3\'s ppo, a2c, ddpg, ppo_lstm, sac, td3, ppo, trpo, CleanRL\'s sac on `HalfCheetahBulletEnv-v0`.\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean\' \\\n        \'a2c\' \\\n        \'ddpg\' \\\n        \'ppo_lstm?cl=PPO w/ LSTM\' \\\n        \'sac\' \\\n        \'td3\' \\\n        \'ppo\' \\\n        \'trpo\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \\\n        \'sac_continuous_action?tag=rlops-pilot&cl=SAC\' \\\n    --env-ids HalfCheetahBulletEnv-v0 \\\n    --ncols 1 \\\n    --ncols-legend 2 \\\n    --xlabel \'Training Steps\' \\\n    --ylabel \'Episodic Return\' \\\n    --output-filename compare \\\n    --report\n```\n\nHere, we created multiple filters. The first string in the first filter is `\'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean\'`, which is a query string that specifies the following:\n\n* `we`: the W&B entity name\n* `wpn`: the W&B project name\n* `ceik`: the custom key for the environment id\n* `cen`: the custom key for the experiment name\n* `metric`: the metric we are interested in\n\nSo we are fetching metrics from [https://wandb.ai/openrlbenchmark/sb3](https://wandb.ai/openrlbenchmark/sb3). The environment id is stored in the `env` key, and the experiment name is stored in the `algo` key. The metric we are interested in is `rollout/ep_rew_mean`.\n\nSimilarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `ppo_lstm?cl=PPO w/ LSTM`.\n\nThe labels of the figure can be customized with the `--xlabel` and `--ylabel` flags. The `--ncols` flag specifies the number of columns in the figure. The `--ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure\n\nThe command above generates the following plot:\n\n|    cleanrl vs. Stable Baselines 3   |    cleanrl vs. Stable Baselines 3 (Time)   |\n|:----------------------------------:|:----------------------------------------:|\n|  ![](static/cleanrl_vs_sb3.png)   |   ![](static/cleanrl_vs_sb3-time.png)   |\n\n\n\nThe `--report` tag also generates a [wandb report](https://wandb.ai/costa-huang/cleanrl/reports/Regression-Report-sac_continuous_action--VmlldzozMTY4NDQ3)\n\n\nThe command also generates a `compare.png`, a `compare.md`, and a `compare.csv` in the current directory.\n\n**Learning curves:** the `compare.png` shows the learning curves which subsamples 10000 data points and and interpolate. The curves are smoothed by a rolling average with a window size 100 and their shaded region represents the standard deviation.\n\n**Result table:** the `compare.md` and `compare.csv` shows the average episodic return of the last 100 episodes. For each random seed $i$ (we have 3 random seeds for each set of experiments), we calculate the average episodic return of the last 100 training episodes as $a_i$. We then average the $a_i$\'s over all random seeds to get the final average episodic return and report its standard deviation. This type of evaluation is known as an implicit evaluation method ([Machado et al., 2017](https://arxiv.org/pdf/1709.06009.pdf)) which aligns better with the general goal of RL which is continual learning. This method also detects issues with catastrophic forgetting compared to the evaluation method that evaluates the best model.\n\n\n> **Warning**\n> You may get slightly different curves every time you run the commands. This is because we sample 500 data points from the track experiments to save bandwidth. You can, however, get all of the data points by running the command with `--scan-history` which will always give you the same curves but will take longer to run. For generating an accurate `compare.md`, you should always use `--scan-history`.\n\n\n\n## Currently supported libraries\n\n* [CleanRL](https://wandb.ai/openrlbenchmark/cleanrl)\n    * `ceik`: `env_id`\n    * `cen`: `exp_name` (e.g., `sac_continuous_action`, `ppo_continuous_action`, `ppo_atari`)\n    * `metric`: `charts/episodic_return`\n* [Stable-baselines3](https://wandb.ai/openrlbenchmark/sb3)\n    * `ceik`: `env`\n    * `cen`: `algo` (e.g., `sac`, `ppo`, `a2c`)\n    * `metric`: `rollout/ep_rew_mean` or `eval/mean_reward`\n* [ikostrikov/jaxrl](https://wandb.ai/openrlbenchmark/jaxrl)\n    * `ceik`: `env_name`\n    * `cen`: `algo` (e.g., `sac`)\n    * `metric`: `training/return` or `evaluation/average_returns`\n* [baselines](https://wandb.ai/openrlbenchmark/baselines)\n    * `ceik`: `env`\n    * `cen`: `alg` (e.g., `ppo2`)\n    * `metric`: `charts/episodic_return` or `eprewmean`\n* [sbx](https://wandb.ai/openrlbenchmark/sbx)\n    * `ceik`: `env`\n    * `cen`: `alg` (e.g., `sac`, `tqc`)\n    * `metric`: `rollout/ep_rew_mean` or `eval/mean_reward`\n* [Tianshou](https://wandb.ai/tianshou/atari.benchmark)\n    * `ceik`: `task`\n    * `cen`: `algo_name` (e.g., `ppo`, `iqn`)\n    * `metric`: `test/reward`\n\nThe following libraries have some recorded experiments:\n\n* [openai/phasic-policy-gradient](https://wandb.ai/openrlbenchmark/phasic-policy-gradient) (has some metrics)\n    * `ceik`: `env_name`\n    * `cen`: `arch` (`shared`)\n    * `metric`: `charts/episodic_return`\n* [sfujim/TD3](https://wandb.ai/openrlbenchmark/sfujim-TD3) (has some metrics)\n    * `ceik`: `env`\n    * `cen`: `policy` (e.g., `TD3`)\n    * `metric`: `charts/episodic_return`\n\n\n## More examples\n\n### Compare CleanRL\'s PPO with `openai/baselines`\'s PPO2 on Atari games:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-cnn\' \\\n    --filters \'?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return\' \'ppo_atari_envpool_xla_jax_truncation\' \\\n    --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \\\n    --check-empty-runs False \\\n    --ncols 5 \\\n    --ncols-legend 2 \\\n    --output-filename static/cleanrl_vs_baselines \\\n    --scan-history\n```\n\n![](static/cleanrl_vs_baselines.png)\n\n### Compare CleanRL\'s PPO with `openai/baselines`\'s PPO2 and `jaxrl`\'s SAC on Mujoco:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-mlp\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'ppo_continuous_action?tag=v1.0.0-27-gde3f410\' \\\n    --filters \'?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return\' \'sac\' \\\n    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \\\n    --check-empty-runs False \\\n    --ncols 3 \\\n    --ncols-legend 3 \\\n    --output-filename compare \\\n    --scan-history\n```\n![](static/baselines_vs_cleanrl_vs_jaxrl.png)\n\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-cnn\' \\\n    --filters \'?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return\' \'ppo_atari_envpool_xla_jax_truncation\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return\' \'ppo_atari_envpool_xla_jax_scan?tag=pr-328\' \\\n    --env-ids BeamRider-v5 Breakout-v5  \\\n    --check-empty-runs False \\\n    --ncols 3 \\\n    --ncols-legend 2 \\\n    --output-filename compare \\\n    --scan-history\n```\n\n\n### Compare Tianshou\'s algorithms with `openai/baselines`\'s PPO2 on Atari:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=tianshou&wpn=atari.benchmark&ceik=task&cen=algo_name&metric=test/reward\' \'iqn\' \'ppo\' \'rainbow\' \'fqf\' \'c51\' \'dqn\' \'qrdqn\' \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-cnn\' \\\n    --env-ids BreakoutNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 SeaquestNoFrameskip-v4 MsPacmanNoFrameskip-v4 EnduroNoFrameskip-v4 PongNoFrameskip-v4 QbertNoFrameskip-v4 \\\n    --check-empty-runs False \\\n    --ncols 4 \\\n    --ncols-legend 4 \\\n    --output-filename static/baselines_vs_tianshou --scan-history\n```\n![](static/baselines_vs_tianshou.png)\n\n\n### Compare CleanRL\'s PPG and PPO with `openai/phasic-policy-gradient`\'s PPG on procgen:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=phasic-policy-gradient&ceik=env_name&cen=arch&metric=charts/episodic_return\' \'shared\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'ppo_procgen?tag=v1.0.0b1-4-g4ea73d9\' \'ppg_procgen?tag=v1.0.0b1-4-g4ea73d9\' \\\n    --env-ids starpilot bossfight bigfish \\\n    --check-empty-runs False \\\n    --ncols 3 \\\n    --ncols-legend 3 \\\n    --output-filename static/ppg_vs_cleanrl \\\n    --scan-history\n```\n\n![](static/ppg_vs_cleanrl.png)\n\n\n### Compare CleanRL\'s TD3 with `sfujim/TD3`\'s TD3 on Mujoco:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=sfujim-TD3&ceik=env&cen=policy&metric=charts/episodic_return\' \'TD3\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'td3_continuous_action_jax?tag=pr-285\' \'ddpg_continuous_action_jax?tag=pr-298\' \\\n    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 \\\n    --check-empty-runs False \\\n    --ncols 3 \\\n    --ncols-legend 3 \\\n    --output-filename static/td3_vs_cleanrl \\\n    --scan-history\n```\n![](static/td3_vs_cleanrl.png)\n\n\n### Compare CleanRL\'s PPO + JAX + EnvPool\'s XLA with `openai/baselines`\'s Atari wrappers vs [Machado\'s recommendetation for Atari](https://arxiv.org/abs/1709.06009) (e.g., sticky action with probability 0.25). The machado\'s experiments ran for 10M steps, which corresponds to 40M frames.\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return\' \'ppo_atari_envpool_xla_jax_truncation_machado_10M\' \'ppo_atari_envpool_xla_jax_truncation\'  \\\n    --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \\\n    --check-empty-runs False \\\n    --ncols 5 \\\n    --ncols-legend 2 \\\n    --output-filename static/machado_10M \\\n    --scan-history\n```\n![](static/machado_10M.png)\n\n\n### Compare CleanRL\'s PPO + JAX + EnvPool\'s XLA with `openai/baselines`\'s Atari wrappers vs [Machado\'s recommendetation for Atari](https://arxiv.org/abs/1709.06009) (e.g., sticky action with probability 0.25). The machado\'s experiments ran for 50M steps, which corresponds to 200M frames.\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return\' \'ppo_atari_envpool_xla_jax_truncation_machado\' \'ppo_atari_envpool_xla_jax_truncation\'  \\\n    --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \\\n    --check-empty-runs False \\\n    --ncols 5 \\\n    --ncols-legend 2 \\\n    --output-filename static/machado_50M \\\n    --scan-history\n```\n![](static/machado_50M.png)\n\n### Calculate human normalized scores\n\n```shell\npython -m openrlbenchmark.hns --files static/cleanrl_vs_baselines.csv static/machado_10M.csv static/machado_50M.csv \n```\n\n```\nbaselines-ppo2-cnn ({})\n┣━━ median hns: 0.7959851540635047\n┣━━ mean hns: 4.54588939893709\nppo_atari_envpool_xla_jax_truncation ({})\n┣━━ median hns: 0.9783505154639175\n┣━━ mean hns: 6.841083973256849\nppo_atari_envpool_xla_jax_truncation_machado_10M ({})\n┣━━ median hns: 0.7347972972972973\n┣━━ mean hns: 2.919095857954249\nppo_atari_envpool_xla_jax_truncation ({\'metric\': [\'charts/avg_episodic_return\']})\n┣━━ median hns: 0.9783505154639175\n┣━━ mean hns: 6.841083973256849\nppo_atari_envpool_xla_jax_truncation_machado ({\'metric\': [\'charts/avg_episodic_return\']})\n┣━━ median hns: 1.5679929625118418\n┣━━ mean hns: 8.352308370550299\n```\n\n## What\'s going on right now?\n\nThis is a project we are slowly working on. There is no specific timeline or roadmap, but if you want to get involved. Feel free to reach out to me or open an issue. We are looking for volunteers to help us with the following:\n\n* Add experiments from other libraries\n* Run more experiments from currently supported libraries\n* Documentation and designing standards\n* Download the tensorboard metrics from the tracked experiments and load them locally to save time\n\n\n\n\n```shell\npip install --upgrade openrlbenchmark\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'dqn_atari?tag=latest\' \'c51_atari?tag=latest\' \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-cnn\' \\\n    --filters \'?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return\' \'ppo_atari_envpool_xla_jax_truncation?user=costa-huang\' \\\n    --env-ids BeamRider-v5 Breakout-v5 Pong-v5 \\\n    --ncols 3 \\\n    --ncols-legend 2 \\\n    --output-filename compare \\\n    --scan-history \\\n    --report \\\n    --check-empty-runs False \n```\n',
+    'long_description': '# Open RL Benchmark: Comprehensive Tracked Experiments for Reinforcement Learning\n\n\n[<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openrlbenchmark/openrlbenchmark/blob/master/README.ipynb)\n[<img src="https://dcbadge.vercel.app/api/server/GsmqhDcea5?style=flat">](https://discord.gg/GsmqhDcea5)\n\n\n\nOpen RL Benchmark is a comprehensive collection of tracked experiments for RL. It aims to make it easier for RL practitioners to pull and compare all kinds of metrics from reputable RL libraries like Stable-baselines3, Tianshou, CleanRL, and others.\n\n* 💾 [GitHub Repo](https://github.com/openrlbenchmark/openrlbenchmark): source code and more docs.\n* 📜 [Design docs](https://docs.google.com/document/d/1cDI_AMr2QVmkC53dCHFMYwGJtLC8V4p6KdL2wnYPaiI/edit?usp=sharing): our motivation and vision.\n* 🔗 [Open RL Benchmark reports](https://wandb.ai/openrlbenchmark/openrlbenchmark/reportlist):  W&B reports with tracked Atari, MuJoCo experiments from SB3, CleanRL, and others.\n\n\n\n## Installation\nYou can install it via pip or the dev setup.\n\n### Pip install\n\n```shell\npip install openrlbenchmark --upgrade\n```\n\n### Dev Setup\n\nPrerequisites:\n* Python >=3.7.1,<3.10 (not yet 3.10)\n* [Poetry 1.2.1+](https://python-poetry.org)\n\n```shell\ngit clone https://github.com/openrlbenchmark/openrlbenchmark.git\ncd openrlbenchmark\npoetry install\n```\n\n\n## Get started\n\nOpen RL Benchmark provides an RLops CLI to pull and compare metrics from Weights and Biases. The following example shows how to compare the performance of SB3\'s ppo, a2c, ddpg, ppo_lstm, sac, td3, ppo, trpo, CleanRL\'s sac on `HalfCheetahBulletEnv-v0`.\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean\' \\\n        \'a2c\' \\\n        \'ddpg\' \\\n        \'ppo_lstm?cl=PPO w/ LSTM\' \\\n        \'sac\' \\\n        \'td3\' \\\n        \'ppo\' \\\n        \'trpo\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \\\n        \'sac_continuous_action?tag=rlops-pilot&cl=SAC\' \\\n    --env-ids HalfCheetahBulletEnv-v0 \\\n    --pc.ncols 1 \\\n    --pc.ncols-legend 2 \\\n    --pc.xlabel \'Training Steps\' \\\n    --pc.ylabel \'Episodic Return\' \\\n    --output-filename compare \\\n    --report\n```\n\nHere, we created multiple filters. The first string in the first filter is `\'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean\'`, which is a query string that specifies the following:\n\n* `we`: the W&B entity name\n* `wpn`: the W&B project name\n* `ceik`: the custom key for the environment id\n* `cen`: the custom key for the experiment name\n* `metric`: the metric we are interested in\n\nSo we are fetching metrics from [https://wandb.ai/openrlbenchmark/sb3](https://wandb.ai/openrlbenchmark/sb3). The environment id is stored in the `env` key, and the experiment name is stored in the `algo` key. The metric we are interested in is `rollout/ep_rew_mean`.\n\nSimilarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `ppo_lstm?cl=PPO w/ LSTM`.\n\nThe labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure\n\nThe command above generates the following plot:\n\n|    cleanrl vs. Stable Baselines 3   |    cleanrl vs. Stable Baselines 3 (Time)   |\n|:----------------------------------:|:----------------------------------------:|\n|  ![](static/cleanrl_vs_sb3.png)   |   ![](static/cleanrl_vs_sb3-time.png)   |\n\n\n\nThe `--report` tag also generates a [wandb report](https://wandb.ai/costa-huang/cleanrl/reports/Regression-Report-sac_continuous_action--VmlldzozMTY4NDQ3)\n\n\nThe command also generates a `compare.png`, a `compare.md`, and a `compare.csv` in the current directory.\n\n**Learning curves:** the `compare.png` shows the learning curves which subsamples 10000 data points and and interpolate. The curves are smoothed by a rolling average with a window size 100 and their shaded region represents the standard deviation.\n\n**Result table:** the `compare.md` and `compare.csv` shows the average episodic return of the last 100 episodes. For each random seed $i$ (we have 3 random seeds for each set of experiments), we calculate the average episodic return of the last 100 training episodes as $a_i$. We then average the $a_i$\'s over all random seeds to get the final average episodic return and report its standard deviation. This type of evaluation is known as an implicit evaluation method ([Machado et al., 2017](https://arxiv.org/pdf/1709.06009.pdf)) which aligns better with the general goal of RL which is continual learning. This method also detects issues with catastrophic forgetting compared to the evaluation method that evaluates the best model.\n\n\n> **Warning**\n> You may get slightly different curves every time you run the commands. This is because we sample 500 data points from the track experiments to save bandwidth. If you are using `openrlbenchmark` repeatedly or you wanto to generate consistent `compare.md` and learning curves, we recommend you to use `--scan-history` to get all of the data points, but initially it may take a while to run.\n\n\n## Currently supported libraries\n\n* [CleanRL](https://wandb.ai/openrlbenchmark/cleanrl)\n    * `ceik`: `env_id`\n    * `cen`: `exp_name` (e.g., `sac_continuous_action`, `ppo_continuous_action`, `ppo_atari`)\n    * `metric`: `charts/episodic_return`\n* [Stable-baselines3](https://wandb.ai/openrlbenchmark/sb3)\n    * `ceik`: `env`\n    * `cen`: `algo` (e.g., `sac`, `ppo`, `a2c`)\n    * `metric`: `rollout/ep_rew_mean` or `eval/mean_reward`\n* [ikostrikov/jaxrl](https://wandb.ai/openrlbenchmark/jaxrl)\n    * `ceik`: `env_name`\n    * `cen`: `algo` (e.g., `sac`)\n    * `metric`: `training/return` or `evaluation/average_returns`\n* [baselines](https://wandb.ai/openrlbenchmark/baselines)\n    * `ceik`: `env`\n    * `cen`: `alg` (e.g., `ppo2`)\n    * `metric`: `charts/episodic_return` or `eprewmean`\n* [sbx](https://wandb.ai/openrlbenchmark/sbx)\n    * `ceik`: `env`\n    * `cen`: `alg` (e.g., `sac`, `tqc`)\n    * `metric`: `rollout/ep_rew_mean` or `eval/mean_reward`\n* [Tianshou](https://wandb.ai/tianshou/atari.benchmark)\n    * `ceik`: `task`\n    * `cen`: `algo_name` (e.g., `ppo`, `iqn`)\n    * `metric`: `test/reward`\n* [MORL-Baselines](https://wandb.ai/openrlbenchmark/morl-baselines)\n    * `ceik`: `env_id`\n    * `cen`: `algo` (e.g., `PGMORL`, `PCN`)\n    * `metric`: `eval/hypervolume`, `eval/igd`, `eval/sparsity`, `eval/eum`, `eval/mul`\n\nThe following libraries have some recorded experiments:\n\n* [openai/phasic-policy-gradient](https://wandb.ai/openrlbenchmark/phasic-policy-gradient) (has some metrics)\n    * `ceik`: `env_name`\n    * `cen`: `arch` (`shared`)\n    * `metric`: `charts/episodic_return`\n* [sfujim/TD3](https://wandb.ai/openrlbenchmark/sfujim-TD3) (has some metrics)\n    * `ceik`: `env`\n    * `cen`: `policy` (e.g., `TD3`)\n    * `metric`: `charts/episodic_return`\n\n\n## More examples\n\n### Compare CleanRL\'s PPO with `openai/baselines`\'s PPO2 on Atari games:\n\nSometimes the same environments could have different names in different libraries. For example, `openai/baselines` uses `BreakoutNoFrameskip-v4` while [EnvPool](https://envpool.readthedocs.io/en/latest/env/atari.html) uses `Breakout-v5`. To compare the two libraries, we need to specify the `env_id` for `CleanRL` and `env` for `openai/baselines`. In this case, can specify the corresponding `env_ids` for each filter.\n\nFor Atari games, we have additional batteries included `openrlbenchmark.rlops_hns` to show human normalized-scores and further statistical analysis through [`rliable`](https://github.com/google-research/rliable).\n\n\n```shell\npython -m openrlbenchmark.rlops_hns \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-cnn\' \\\n    --filters \'?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return\' \'ppo_atari_envpool_xla_jax_truncation\' \\\n    --env-ids AlienNoFrameskip-v4 AmidarNoFrameskip-v4 AssaultNoFrameskip-v4 AsterixNoFrameskip-v4 AsteroidsNoFrameskip-v4 AtlantisNoFrameskip-v4 BankHeistNoFrameskip-v4 BattleZoneNoFrameskip-v4 BeamRiderNoFrameskip-v4 BerzerkNoFrameskip-v4 BowlingNoFrameskip-v4 BoxingNoFrameskip-v4 BreakoutNoFrameskip-v4 CentipedeNoFrameskip-v4 ChopperCommandNoFrameskip-v4 CrazyClimberNoFrameskip-v4 DefenderNoFrameskip-v4 DemonAttackNoFrameskip-v4 DoubleDunkNoFrameskip-v4 EnduroNoFrameskip-v4 FishingDerbyNoFrameskip-v4 FreewayNoFrameskip-v4 FrostbiteNoFrameskip-v4 GopherNoFrameskip-v4 GravitarNoFrameskip-v4 HeroNoFrameskip-v4 IceHockeyNoFrameskip-v4 PrivateEyeNoFrameskip-v4 QbertNoFrameskip-v4 RiverraidNoFrameskip-v4 RoadRunnerNoFrameskip-v4 RobotankNoFrameskip-v4 SeaquestNoFrameskip-v4 SkiingNoFrameskip-v4 SolarisNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 StarGunnerNoFrameskip-v4 SurroundNoFrameskip-v4 TennisNoFrameskip-v4 TimePilotNoFrameskip-v4 TutankhamNoFrameskip-v4 UpNDownNoFrameskip-v4 VentureNoFrameskip-v4 VideoPinballNoFrameskip-v4 WizardOfWorNoFrameskip-v4 YarsRevengeNoFrameskip-v4 ZaxxonNoFrameskip-v4 JamesbondNoFrameskip-v4 KangarooNoFrameskip-v4 KrullNoFrameskip-v4 KungFuMasterNoFrameskip-v4 MontezumaRevengeNoFrameskip-v4 MsPacmanNoFrameskip-v4 NameThisGameNoFrameskip-v4 PhoenixNoFrameskip-v4 PitfallNoFrameskip-v4 PongNoFrameskip-v4 \\\n    --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \\\n    --no-check-empty-runs \\\n    --pc.ncols 5 \\\n    --pc.ncols-legend 2 \\\n    --output-filename static/cleanrl_vs_baselines \\\n    --scan-history --rliable\n```\n\nIn the individual learning curves below, the right y-axis is the human normalized score. The left y-axis is the raw episodic return.\n![](static/cleanrl_vs_baselines.png) The script also generates `cleanrl_vs_baselines_hns_median.png`, the learning curves for median human-normalized scores. \n\nFurthermore, the `--rliable` integration generates `cleanrl_vs_baselines_iqm_profile.png`, the  Interquartile Mean (IQM) and performance profile ([Agarwal et al., 2022](https://arxiv.org/pdf/2108.13264.pdf)), and `cleanrl_vs_baselines_hns_aggregate.png`, the aggregate human-normalized scores with Stratified Bootstrap Confidence Intervals (see @araffin\'s excellent blog post [explainer](https://araffin.github.io/post/rliable/)). \n\n\n![](static/cleanrl_vs_baselines_hns_median.png)\n\n![](static/cleanrl_vs_baselines_iqm_profile.png)\n\n![](static/cleanrl_vs_baselines_hns_aggregate.png)\n\n\n### Offline mode\n\nSometimes even with caching `--scan-history` the script can still take a long time if there are too many environments or experiments. This is because we are still calling many `wandb.Api().runs(..., filters)` under the hood. \n\nNo worries though. When running with `--scan-history`, we also automatically build a local `sqlite` database to store the metadata of runs, enabling us to run the script without internet connection.\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-mlp\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'ppo_continuous_action?tag=v1.0.0-27-gde3f410\' \\\n    --filters \'?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return\' \'sac\' \\\n    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \\\n    --no-check-empty-runs \\\n    --pc.ncols 3 \\\n    --pc.ncols-legend 3 \\\n    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \\\n    --scan-history \\\n    --offline\n```\n\n### Compare CleanRL\'s PPO with `openai/baselines`\'s PPO2 and `jaxrl`\'s SAC on Mujoco:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-mlp\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'ppo_continuous_action?tag=v1.0.0-27-gde3f410\' \\\n    --filters \'?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return\' \'sac\' \\\n    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \\\n    --no-check-empty-runs \\\n    --pc.ncols 3 \\\n    --pc.ncols-legend 3 \\\n    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \\\n    --scan-history\n```\n![](static/baselines_vs_cleanrl_vs_jaxrl.png)\n\n\n\n### Compare Tianshou\'s algorithms with `openai/baselines`\'s PPO2 on Atari:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=tianshou&wpn=atari.benchmark&ceik=task&cen=algo_name&metric=test/reward\' \'iqn\' \'ppo\' \'rainbow\' \'fqf\' \'c51\' \'dqn\' \'qrdqn\' \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-cnn\' \\\n    --env-ids BreakoutNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 SeaquestNoFrameskip-v4 MsPacmanNoFrameskip-v4 EnduroNoFrameskip-v4 PongNoFrameskip-v4 QbertNoFrameskip-v4 \\\n    --no-check-empty-runs \\\n    --pc.ncols 4 \\\n    --pc.ncols-legend 4 \\\n    --output-filename static/baselines_vs_tianshou --scan-history\n```\n![](static/baselines_vs_tianshou.png)\n\n\n### Compare CleanRL\'s PPG and PPO with `openai/phasic-policy-gradient`\'s PPG on procgen:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=phasic-policy-gradient&ceik=env_name&cen=arch&metric=charts/episodic_return\' \'shared\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'ppo_procgen?tag=v1.0.0b1-4-g4ea73d9\' \'ppg_procgen?tag=v1.0.0b1-4-g4ea73d9\' \\\n    --env-ids starpilot bossfight bigfish \\\n    --no-check-empty-runs \\\n    --pc.ncols 3 \\\n    --pc.ncols-legend 3 \\\n    --output-filename static/ppg_vs_cleanrl \\\n    --scan-history\n```\n\n![](static/ppg_vs_cleanrl.png)\n\n\n### Compare CleanRL\'s TD3 with `sfujim/TD3`\'s TD3 on Mujoco:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=sfujim-TD3&ceik=env&cen=policy&metric=charts/episodic_return\' \'TD3\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'td3_continuous_action_jax?tag=pr-285\' \'ddpg_continuous_action_jax?tag=pr-298\' \\\n    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 \\\n    --no-check-empty-runs \\\n    --pc.ncols 3 \\\n    --pc.ncols-legend 3 \\\n    --output-filename static/td3_vs_cleanrl \\\n    --scan-history\n```\n![](static/td3_vs_cleanrl.png)\n\n\n\n### Compare MORL Baselines algorithms on deterministic environments\n\n```shell\npython -m openrlbenchmark.rlops \\\n  --filters \'?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metric=eval/hypervolume\' \\\n  \'Pareto Q-Learning?cl=Pareto Q-Learning\' \\\n  \'MultiPolicy MO Q-Learning?cl=MultiPolicy MO Q-Learning\' \\\n  \'MultiPolicy MO Q-Learning (OLS)?cl=MultiPolicy MO Q-Learning (OLS)\' \\\n  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 \\\n  --pc.ncols 2 \\\n  --pc.ncols-legend 1 \\\n  --pc.xlabel \'Training steps\' \\\n  --pc.ylabel \'Hypervolume\' \\\n  --output-filename morl_deterministic_envs \\\n  --scan-history\n```\n\n![](static/morl_deterministic_envs.png)\n![](static/morl_deterministic_envs-time.png)\n\n### Calculate human normalized scores\n\n```shell\npython -m openrlbenchmark.hns --files static/cleanrl_vs_baselines.csv static/machado_10M.csv static/machado_50M.csv \n```\n\n```\nbaselines-ppo2-cnn ({})\n┣━━ median hns: 0.7959851540635047\n┣━━ mean hns: 4.54588939893709\nppo_atari_envpool_xla_jax_truncation ({})\n┣━━ median hns: 0.9783505154639175\n┣━━ mean hns: 6.841083973256849\nppo_atari_envpool_xla_jax_truncation_machado_10M ({})\n┣━━ median hns: 0.7347972972972973\n┣━━ mean hns: 2.919095857954249\nppo_atari_envpool_xla_jax_truncation ({\'metric\': [\'charts/avg_episodic_return\']})\n┣━━ median hns: 0.9783505154639175\n┣━━ mean hns: 6.841083973256849\nppo_atari_envpool_xla_jax_truncation_machado ({\'metric\': [\'charts/avg_episodic_return\']})\n┣━━ median hns: 1.5679929625118418\n┣━━ mean hns: 8.352308370550299\n```\n\n## What\'s going on right now?\n\nThis is a project we are slowly working on. There is no specific timeline or roadmap, but if you want to get involved. Feel free to reach out to me or open an issue. We are looking for volunteers to help us with the following:\n\n* Add experiments from other libraries\n* Run more experiments from currently supported libraries\n* Documentation and designing standards\n* Download the tensorboard metrics from the tracked experiments and load them locally to save time\n\n',
     'author': 'Costa Huang',
     'author_email': 'costa.huang@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.7.1,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `openrlbenchmark-0.1.1b4/PKG-INFO` & `openrlbenchmark-0.2.0b1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: openrlbenchmark
-Version: 0.1.1b4
-Summary: 
-Author: Costa Huang
-Author-email: costa.huang@outlook.com
-Requires-Python: >=3.7.1,<4.0.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: expt (>=0.4.1,<0.5.0)
-Requires-Dist: importlib-metadata (>=5.1.0,<6.0.0)
-Requires-Dist: multiprocess (>=0.70.13,<0.71.0)
-Requires-Dist: pip (>=22.1.2,<23.0.0)
-Requires-Dist: rich (<12.0)
-Requires-Dist: seaborn (>=0.12.1,<0.13.0)
-Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: tueplots (>=0.0.4,<0.0.5)
-Requires-Dist: wandb (>=0.13.7,<0.14.0)
-Description-Content-Type: text/markdown
-
 # Open RL Benchmark: Comprehensive Tracked Experiments for Reinforcement Learning
 
 
 [<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openrlbenchmark/openrlbenchmark/blob/master/README.ipynb)
@@ -76,18 +52,18 @@
         'sac' \
         'td3' \
         'ppo' \
         'trpo' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' \
         'sac_continuous_action?tag=rlops-pilot&cl=SAC' \
     --env-ids HalfCheetahBulletEnv-v0 \
-    --ncols 1 \
-    --ncols-legend 2 \
-    --xlabel 'Training Steps' \
-    --ylabel 'Episodic Return' \
+    --pc.ncols 1 \
+    --pc.ncols-legend 2 \
+    --pc.xlabel 'Training Steps' \
+    --pc.ylabel 'Episodic Return' \
     --output-filename compare \
     --report
 ```
 
 Here, we created multiple filters. The first string in the first filter is `'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean'`, which is a query string that specifies the following:
 
 * `we`: the W&B entity name
@@ -96,15 +72,15 @@
 * `cen`: the custom key for the experiment name
 * `metric`: the metric we are interested in
 
 So we are fetching metrics from [https://wandb.ai/openrlbenchmark/sb3](https://wandb.ai/openrlbenchmark/sb3). The environment id is stored in the `env` key, and the experiment name is stored in the `algo` key. The metric we are interested in is `rollout/ep_rew_mean`.
 
 Similarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `ppo_lstm?cl=PPO w/ LSTM`.
 
-The labels of the figure can be customized with the `--xlabel` and `--ylabel` flags. The `--ncols` flag specifies the number of columns in the figure. The `--ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
+The labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
 
 The command above generates the following plot:
 
 |    cleanrl vs. Stable Baselines 3   |    cleanrl vs. Stable Baselines 3 (Time)   |
 |:----------------------------------:|:----------------------------------------:|
 |  ![](static/cleanrl_vs_sb3.png)   |   ![](static/cleanrl_vs_sb3-time.png)   |
 
@@ -117,16 +93,15 @@
 
 **Learning curves:** the `compare.png` shows the learning curves which subsamples 10000 data points and and interpolate. The curves are smoothed by a rolling average with a window size 100 and their shaded region represents the standard deviation.
 
 **Result table:** the `compare.md` and `compare.csv` shows the average episodic return of the last 100 episodes. For each random seed $i$ (we have 3 random seeds for each set of experiments), we calculate the average episodic return of the last 100 training episodes as $a_i$. We then average the $a_i$'s over all random seeds to get the final average episodic return and report its standard deviation. This type of evaluation is known as an implicit evaluation method ([Machado et al., 2017](https://arxiv.org/pdf/1709.06009.pdf)) which aligns better with the general goal of RL which is continual learning. This method also detects issues with catastrophic forgetting compared to the evaluation method that evaluates the best model.
 
 
 > **Warning**
-> You may get slightly different curves every time you run the commands. This is because we sample 500 data points from the track experiments to save bandwidth. You can, however, get all of the data points by running the command with `--scan-history` which will always give you the same curves but will take longer to run. For generating an accurate `compare.md`, you should always use `--scan-history`.
-
+> You may get slightly different curves every time you run the commands. This is because we sample 500 data points from the track experiments to save bandwidth. If you are using `openrlbenchmark` repeatedly or you wanto to generate consistent `compare.md` and learning curves, we recommend you to use `--scan-history` to get all of the data points, but initially it may take a while to run.
 
 
 ## Currently supported libraries
 
 * [CleanRL](https://wandb.ai/openrlbenchmark/cleanrl)
     * `ceik`: `env_id`
     * `cen`: `exp_name` (e.g., `sac_continuous_action`, `ppo_continuous_action`, `ppo_atari`)
@@ -147,14 +122,18 @@
     * `ceik`: `env`
     * `cen`: `alg` (e.g., `sac`, `tqc`)
     * `metric`: `rollout/ep_rew_mean` or `eval/mean_reward`
 * [Tianshou](https://wandb.ai/tianshou/atari.benchmark)
     * `ceik`: `task`
     * `cen`: `algo_name` (e.g., `ppo`, `iqn`)
     * `metric`: `test/reward`
+* [MORL-Baselines](https://wandb.ai/openrlbenchmark/morl-baselines)
+    * `ceik`: `env_id`
+    * `cen`: `algo` (e.g., `PGMORL`, `PCN`)
+    * `metric`: `eval/hypervolume`, `eval/igd`, `eval/sparsity`, `eval/eum`, `eval/mul`
 
 The following libraries have some recorded experiments:
 
 * [openai/phasic-policy-gradient](https://wandb.ai/openrlbenchmark/phasic-policy-gradient) (has some metrics)
     * `ceik`: `env_name`
     * `cen`: `arch` (`shared`)
     * `metric`: `charts/episodic_return`
@@ -164,135 +143,151 @@
     * `metric`: `charts/episodic_return`
 
 
 ## More examples
 
 ### Compare CleanRL's PPO with `openai/baselines`'s PPO2 on Atari games:
 
+Sometimes the same environments could have different names in different libraries. For example, `openai/baselines` uses `BreakoutNoFrameskip-v4` while [EnvPool](https://envpool.readthedocs.io/en/latest/env/atari.html) uses `Breakout-v5`. To compare the two libraries, we need to specify the `env_id` for `CleanRL` and `env` for `openai/baselines`. In this case, can specify the corresponding `env_ids` for each filter.
+
+For Atari games, we have additional batteries included `openrlbenchmark.rlops_hns` to show human normalized-scores and further statistical analysis through [`rliable`](https://github.com/google-research/rliable).
+
+
 ```shell
-python -m openrlbenchmark.rlops \
+python -m openrlbenchmark.rlops_hns \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
     --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation' \
+    --env-ids AlienNoFrameskip-v4 AmidarNoFrameskip-v4 AssaultNoFrameskip-v4 AsterixNoFrameskip-v4 AsteroidsNoFrameskip-v4 AtlantisNoFrameskip-v4 BankHeistNoFrameskip-v4 BattleZoneNoFrameskip-v4 BeamRiderNoFrameskip-v4 BerzerkNoFrameskip-v4 BowlingNoFrameskip-v4 BoxingNoFrameskip-v4 BreakoutNoFrameskip-v4 CentipedeNoFrameskip-v4 ChopperCommandNoFrameskip-v4 CrazyClimberNoFrameskip-v4 DefenderNoFrameskip-v4 DemonAttackNoFrameskip-v4 DoubleDunkNoFrameskip-v4 EnduroNoFrameskip-v4 FishingDerbyNoFrameskip-v4 FreewayNoFrameskip-v4 FrostbiteNoFrameskip-v4 GopherNoFrameskip-v4 GravitarNoFrameskip-v4 HeroNoFrameskip-v4 IceHockeyNoFrameskip-v4 PrivateEyeNoFrameskip-v4 QbertNoFrameskip-v4 RiverraidNoFrameskip-v4 RoadRunnerNoFrameskip-v4 RobotankNoFrameskip-v4 SeaquestNoFrameskip-v4 SkiingNoFrameskip-v4 SolarisNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 StarGunnerNoFrameskip-v4 SurroundNoFrameskip-v4 TennisNoFrameskip-v4 TimePilotNoFrameskip-v4 TutankhamNoFrameskip-v4 UpNDownNoFrameskip-v4 VentureNoFrameskip-v4 VideoPinballNoFrameskip-v4 WizardOfWorNoFrameskip-v4 YarsRevengeNoFrameskip-v4 ZaxxonNoFrameskip-v4 JamesbondNoFrameskip-v4 KangarooNoFrameskip-v4 KrullNoFrameskip-v4 KungFuMasterNoFrameskip-v4 MontezumaRevengeNoFrameskip-v4 MsPacmanNoFrameskip-v4 NameThisGameNoFrameskip-v4 PhoenixNoFrameskip-v4 PitfallNoFrameskip-v4 PongNoFrameskip-v4 \
     --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \
-    --check-empty-runs False \
-    --ncols 5 \
-    --ncols-legend 2 \
+    --no-check-empty-runs \
+    --pc.ncols 5 \
+    --pc.ncols-legend 2 \
     --output-filename static/cleanrl_vs_baselines \
-    --scan-history
+    --scan-history --rliable
 ```
 
-![](static/cleanrl_vs_baselines.png)
+In the individual learning curves below, the right y-axis is the human normalized score. The left y-axis is the raw episodic return.
+![](static/cleanrl_vs_baselines.png) The script also generates `cleanrl_vs_baselines_hns_median.png`, the learning curves for median human-normalized scores. 
 
-### Compare CleanRL's PPO with `openai/baselines`'s PPO2 and `jaxrl`'s SAC on Mujoco:
+Furthermore, the `--rliable` integration generates `cleanrl_vs_baselines_iqm_profile.png`, the  Interquartile Mean (IQM) and performance profile ([Agarwal et al., 2022](https://arxiv.org/pdf/2108.13264.pdf)), and `cleanrl_vs_baselines_hns_aggregate.png`, the aggregate human-normalized scores with Stratified Bootstrap Confidence Intervals (see @araffin's excellent blog post [explainer](https://araffin.github.io/post/rliable/)). 
+
+
+![](static/cleanrl_vs_baselines_hns_median.png)
+
+![](static/cleanrl_vs_baselines_iqm_profile.png)
+
+![](static/cleanrl_vs_baselines_hns_aggregate.png)
+
+
+### Offline mode
+
+Sometimes even with caching `--scan-history` the script can still take a long time if there are too many environments or experiments. This is because we are still calling many `wandb.Api().runs(..., filters)` under the hood. 
+
+No worries though. When running with `--scan-history`, we also automatically build a local `sqlite` database to store the metadata of runs, enabling us to run the script without internet connection.
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-mlp' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_continuous_action?tag=v1.0.0-27-gde3f410' \
     --filters '?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return' 'sac' \
     --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \
-    --check-empty-runs False \
-    --ncols 3 \
-    --ncols-legend 3 \
-    --output-filename compare \
-    --scan-history
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 3 \
+    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \
+    --scan-history \
+    --offline
 ```
-![](static/baselines_vs_cleanrl_vs_jaxrl.png)
 
+### Compare CleanRL's PPO with `openai/baselines`'s PPO2 and `jaxrl`'s SAC on Mujoco:
 
 ```shell
 python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
-    --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation' \
-    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_scan?tag=pr-328' \
-    --env-ids BeamRider-v5 Breakout-v5  \
-    --check-empty-runs False \
-    --ncols 3 \
-    --ncols-legend 2 \
-    --output-filename compare \
+    --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-mlp' \
+    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_continuous_action?tag=v1.0.0-27-gde3f410' \
+    --filters '?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return' 'sac' \
+    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 3 \
+    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \
     --scan-history
 ```
+![](static/baselines_vs_cleanrl_vs_jaxrl.png)
+
 
 
 ### Compare Tianshou's algorithms with `openai/baselines`'s PPO2 on Atari:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=tianshou&wpn=atari.benchmark&ceik=task&cen=algo_name&metric=test/reward' 'iqn' 'ppo' 'rainbow' 'fqf' 'c51' 'dqn' 'qrdqn' \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
     --env-ids BreakoutNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 SeaquestNoFrameskip-v4 MsPacmanNoFrameskip-v4 EnduroNoFrameskip-v4 PongNoFrameskip-v4 QbertNoFrameskip-v4 \
-    --check-empty-runs False \
-    --ncols 4 \
-    --ncols-legend 4 \
+    --no-check-empty-runs \
+    --pc.ncols 4 \
+    --pc.ncols-legend 4 \
     --output-filename static/baselines_vs_tianshou --scan-history
 ```
 ![](static/baselines_vs_tianshou.png)
 
 
 ### Compare CleanRL's PPG and PPO with `openai/phasic-policy-gradient`'s PPG on procgen:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=phasic-policy-gradient&ceik=env_name&cen=arch&metric=charts/episodic_return' 'shared' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_procgen?tag=v1.0.0b1-4-g4ea73d9' 'ppg_procgen?tag=v1.0.0b1-4-g4ea73d9' \
     --env-ids starpilot bossfight bigfish \
-    --check-empty-runs False \
-    --ncols 3 \
-    --ncols-legend 3 \
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 3 \
     --output-filename static/ppg_vs_cleanrl \
     --scan-history
 ```
 
 ![](static/ppg_vs_cleanrl.png)
 
 
 ### Compare CleanRL's TD3 with `sfujim/TD3`'s TD3 on Mujoco:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=sfujim-TD3&ceik=env&cen=policy&metric=charts/episodic_return' 'TD3' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'td3_continuous_action_jax?tag=pr-285' 'ddpg_continuous_action_jax?tag=pr-298' \
     --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 \
-    --check-empty-runs False \
-    --ncols 3 \
-    --ncols-legend 3 \
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 3 \
     --output-filename static/td3_vs_cleanrl \
     --scan-history
 ```
 ![](static/td3_vs_cleanrl.png)
 
 
-### Compare CleanRL's PPO + JAX + EnvPool's XLA with `openai/baselines`'s Atari wrappers vs [Machado's recommendetation for Atari](https://arxiv.org/abs/1709.06009) (e.g., sticky action with probability 0.25). The machado's experiments ran for 10M steps, which corresponds to 40M frames.
 
-```shell
-python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation_machado_10M' 'ppo_atari_envpool_xla_jax_truncation'  \
-    --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \
-    --check-empty-runs False \
-    --ncols 5 \
-    --ncols-legend 2 \
-    --output-filename static/machado_10M \
-    --scan-history
-```
-![](static/machado_10M.png)
-
-
-### Compare CleanRL's PPO + JAX + EnvPool's XLA with `openai/baselines`'s Atari wrappers vs [Machado's recommendetation for Atari](https://arxiv.org/abs/1709.06009) (e.g., sticky action with probability 0.25). The machado's experiments ran for 50M steps, which corresponds to 200M frames.
+### Compare MORL Baselines algorithms on deterministic environments
 
 ```shell
 python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation_machado' 'ppo_atari_envpool_xla_jax_truncation'  \
-    --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \
-    --check-empty-runs False \
-    --ncols 5 \
-    --ncols-legend 2 \
-    --output-filename static/machado_50M \
-    --scan-history
+  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metric=eval/hypervolume' \
+  'Pareto Q-Learning?cl=Pareto Q-Learning' \
+  'MultiPolicy MO Q-Learning?cl=MultiPolicy MO Q-Learning' \
+  'MultiPolicy MO Q-Learning (OLS)?cl=MultiPolicy MO Q-Learning (OLS)' \
+  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 \
+  --pc.ncols 2 \
+  --pc.ncols-legend 1 \
+  --pc.xlabel 'Training steps' \
+  --pc.ylabel 'Hypervolume' \
+  --output-filename morl_deterministic_envs \
+  --scan-history
 ```
-![](static/machado_50M.png)
+
+![](static/morl_deterministic_envs.png)
+![](static/morl_deterministic_envs-time.png)
 
 ### Calculate human normalized scores
 
 ```shell
 python -m openrlbenchmark.hns --files static/cleanrl_vs_baselines.csv static/machado_10M.csv static/machado_50M.csv 
 ```
 
@@ -319,25 +314,7 @@
 This is a project we are slowly working on. There is no specific timeline or roadmap, but if you want to get involved. Feel free to reach out to me or open an issue. We are looking for volunteers to help us with the following:
 
 * Add experiments from other libraries
 * Run more experiments from currently supported libraries
 * Documentation and designing standards
 * Download the tensorboard metrics from the tracked experiments and load them locally to save time
 
-
-
-
-```shell
-pip install --upgrade openrlbenchmark
-python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'dqn_atari?tag=latest' 'c51_atari?tag=latest' \
-    --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
-    --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation?user=costa-huang' \
-    --env-ids BeamRider-v5 Breakout-v5 Pong-v5 \
-    --ncols 3 \
-    --ncols-legend 2 \
-    --output-filename compare \
-    --scan-history \
-    --report \
-    --check-empty-runs False 
-```
-
```

