# Comparing `tmp/mountaintop-0.1.1.1.tar.gz` & `tmp/mountaintop-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountaintop-0.1.1.1.tar", last modified: Fri May  5 09:46:01 2023, max compression
+gzip compressed data, was "mountaintop-0.1.2.tar", last modified: Fri May  5 11:09:04 2023, max compression
```

## Comparing `mountaintop-0.1.1.1.tar` & `mountaintop-0.1.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.318029 mountaintop-0.1.1.1/
--rw-rw-r--   0 root         (0) root         (0)      145 2023-03-22 08:56:48.000000 mountaintop-0.1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      637 2023-05-05 09:46:01.318029 mountaintop-0.1.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2260 2023-05-04 08:35:22.000000 mountaintop-0.1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.310029 mountaintop-0.1.1.1/mountaintop/
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 09:44:10.000000 mountaintop-0.1.1.1/mountaintop/VERSION
--rw-r--r--   0 root         (0) root         (0)      576 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/bin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/bin/asr/
--rw-r--r--   0 root         (0) root         (0)     1051 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8857 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/asr/decode.py
--rw-r--r--   0 root         (0) root         (0)     8270 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/asr/wer.py
--rw-r--r--   0 root         (0) root         (0)     4877 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/average.py
--rw-r--r--   0 root         (0) root         (0)     4498 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/eval.py
--rw-r--r--   0 root         (0) root         (0)     3450 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/export.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/main.py
--rw-r--r--   0 root         (0) root         (0)     2400 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/parser.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/parser_base.py
--rw-r--r--   0 root         (0) root         (0)     5080 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/profiler.py
--rw-r--r--   0 root         (0) root         (0)     7252 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/train.py
--rw-r--r--   0 root         (0) root         (0)     3369 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/bin/visual.py
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/core/audio/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/audio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2414 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/audio/cmvn.py
--rw-r--r--   0 root         (0) root         (0)    10234 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/audio/wer.py
--rw-r--r--   0 root         (0) root         (0)    14022 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/beam_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/core/internal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4549 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/internal/container.py
--rw-r--r--   0 root         (0) root         (0)     7099 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/internal/distribute.py
--rw-r--r--   0 root         (0) root         (0)     4101 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/internal/module.py
--rw-r--r--   0 root         (0) root         (0)     2185 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/internal/timing.py
--rw-r--r--   0 root         (0) root         (0)      427 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/internal/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/core/ops/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5132 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/ops/common.py
--rw-r--r--   0 root         (0) root         (0)    10422 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/core/ops/mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/dataset/
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/dataset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/dataset/asr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/dataset/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19757 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/dataset/asr/fetcher.py
--rw-r--r--   0 root         (0) root         (0)     3456 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/dataset/asr/loader.py
--rw-r--r--   0 root         (0) root         (0)     5191 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/dataset/base.py
--rw-r--r--   0 root         (0) root         (0)     4111 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/dataset/sampler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/dataset/vad/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/dataset/vad/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19212 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/dataset/vad/fetcher.py
--rw-r--r--   0 root         (0) root         (0)     3492 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/dataset/vad/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/layers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2503 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/activation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/layers/base/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/base/dataclass.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/base/interface.py
--rw-r--r--   0 root         (0) root         (0)    17991 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9398 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_attention.py
--rw-r--r--   0 root         (0) root         (0)    14981 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_decoder.py
--rw-r--r--   0 root         (0) root         (0)     5620 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_decoder_block.py
--rw-r--r--   0 root         (0) root         (0)    12600 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_encoder.py
--rw-r--r--   0 root         (0) root         (0)    12655 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_encoder_block.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_forward.py
--rw-r--r--   0 root         (0) root         (0)     3097 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/normalization.py
--rw-r--r--   0 root         (0) root         (0)     4221 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/optimizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/layers/paraformer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/paraformer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5509 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/paraformer/decoder.py
--rw-r--r--   0 root         (0) root         (0)    14762 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/paraformer/predictor.py
--rw-r--r--   0 root         (0) root         (0)     3177 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/speech_embed.py
--rw-r--r--   0 root         (0) root         (0)     7361 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/subsampling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/layers/transducer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transducer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/layers/transformer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14943 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/attention.py
--rw-r--r--   0 root         (0) root         (0)     4216 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/convolution.py
--rw-r--r--   0 root         (0) root         (0)    15176 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/decoder.py
--rw-r--r--   0 root         (0) root         (0)     9918 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/decoder_block.py
--rw-r--r--   0 root         (0) root         (0)    12971 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/embedding.py
--rw-r--r--   0 root         (0) root         (0)    12676 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/encoder.py
--rw-r--r--   0 root         (0) root         (0)    12678 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/encoder_block.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/forward.py
--rw-r--r--   0 root         (0) root         (0)    41321 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/k2_conformer.py
--rw-r--r--   0 root         (0) root         (0)    22729 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/layers/transformer/k2_scaling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/models/asr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24984 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/asr/paraformer.py
--rw-r--r--   0 root         (0) root         (0)    29348 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/asr/transformer.py
--rw-r--r--   0 root         (0) root         (0)      727 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/asr/utils.py
--rw-r--r--   0 root         (0) root         (0)     2665 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/base.py
--rw-r--r--   0 root         (0) root         (0)    16050 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/saver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/models/vad/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/vad/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14141 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/vad/transformer.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/models/vad/wavenet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop/resources/
--rw-r--r--   0 root         (0) root         (0)      832 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.310029 mountaintop-0.1.1.1/mountaintop/resources/fetcher_config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.318029 mountaintop-0.1.1.1/mountaintop/resources/fetcher_config/asr/
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/resources/fetcher_config/asr/dynamic.yaml
--rw-r--r--   0 root         (0) root         (0)      621 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/resources/fetcher_config/asr/static.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.310029 mountaintop-0.1.1.1/mountaintop/resources/model_config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.318029 mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/
--rw-r--r--   0 root         (0) root         (0)     2014 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/conformer-base.yaml
--rw-r--r--   0 root         (0) root         (0)     2119 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/lowrank_conformer-base.yaml
--rw-r--r--   0 root         (0) root         (0)     1844 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/lowrank_transformer-base.yaml
--rw-r--r--   0 root         (0) root         (0)     2312 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/paraformer-base.yaml
--rw-r--r--   0 root         (0) root         (0)     1795 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/transformer-base.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.318029 mountaintop-0.1.1.1/mountaintop/runx/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/runx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21413 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/runx/logx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.318029 mountaintop-0.1.1.1/mountaintop/runx/mixins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/runx/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5539 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/runx/mixins/saver_mixins.py
--rw-r--r--   0 root         (0) root         (0)     7454 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/runx/monitor.py
--rw-r--r--   0 root         (0) root         (0)    23684 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/runx/trainer.py
--rw-r--r--   0 root         (0) root         (0)     4172 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/runx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.318029 mountaintop-0.1.1.1/mountaintop/utils/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/utils/git.py
--rw-r--r--   0 root         (0) root         (0)     4130 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-04-27 12:32:09.000000 mountaintop-0.1.1.1/mountaintop/utils/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:46:01.314029 mountaintop-0.1.1.1/mountaintop.egg-info/
--rw-r--r--   0 root         (0) root         (0)      637 2023-05-05 09:46:01.000000 mountaintop-0.1.1.1/mountaintop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4006 2023-05-05 09:46:01.000000 mountaintop-0.1.1.1/mountaintop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 09:46:01.000000 mountaintop-0.1.1.1/mountaintop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-05 09:46:01.000000 mountaintop-0.1.1.1/mountaintop.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-05 09:46:01.000000 mountaintop-0.1.1.1/mountaintop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-05 09:46:01.000000 mountaintop-0.1.1.1/mountaintop.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      130 2023-03-23 10:32:27.000000 mountaintop-0.1.1.1/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)      149 2023-05-05 09:46:01.318029 mountaintop-0.1.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2056 2023-03-22 08:56:48.000000 mountaintop-0.1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/
+-rw-rw-r--   0 root         (0) root         (0)      145 2023-03-22 08:56:48.000000 mountaintop-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-05 11:09:04.267031 mountaintop-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2260 2023-05-04 08:35:22.000000 mountaintop-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/VERSION
+-rw-r--r--   0 root         (0) root         (0)      576 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/bin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/bin/asr/
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8857 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/asr/decode.py
+-rw-r--r--   0 root         (0) root         (0)     8270 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/asr/wer.py
+-rw-r--r--   0 root         (0) root         (0)     4877 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/average.py
+-rw-r--r--   0 root         (0) root         (0)     4498 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/eval.py
+-rw-r--r--   0 root         (0) root         (0)     3450 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/export.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/main.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/profiler.py
+-rw-r--r--   0 root         (0) root         (0)     7252 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/train.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/bin/visual.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/core/audio/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/audio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/audio/cmvn.py
+-rw-r--r--   0 root         (0) root         (0)    10234 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/audio/wer.py
+-rw-r--r--   0 root         (0) root         (0)    14022 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/beam_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/core/internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4549 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/internal/container.py
+-rw-r--r--   0 root         (0) root         (0)     7099 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/internal/distribute.py
+-rw-r--r--   0 root         (0) root         (0)     4101 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/internal/module.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/internal/timing.py
+-rw-r--r--   0 root         (0) root         (0)      427 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/internal/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/core/ops/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5132 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/ops/common.py
+-rw-r--r--   0 root         (0) root         (0)    10422 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/core/ops/mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/dataset/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/dataset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/dataset/asr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/dataset/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19757 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/dataset/asr/fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/dataset/asr/loader.py
+-rw-r--r--   0 root         (0) root         (0)     5191 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/dataset/base.py
+-rw-r--r--   0 root         (0) root         (0)     4111 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/dataset/sampler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/dataset/vad/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/dataset/vad/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19212 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/dataset/vad/fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/dataset/vad/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/layers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/activation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/layers/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/base/dataclass.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/base/interface.py
+-rw-r--r--   0 root         (0) root         (0)    17991 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9398 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_attention.py
+-rw-r--r--   0 root         (0) root         (0)    14981 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_decoder.py
+-rw-r--r--   0 root         (0) root         (0)     5620 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_decoder_block.py
+-rw-r--r--   0 root         (0) root         (0)    12600 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    12655 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_encoder_block.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_forward.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/normalization.py
+-rw-r--r--   0 root         (0) root         (0)     4221 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/optimizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/layers/paraformer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/paraformer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5509 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/paraformer/decoder.py
+-rw-r--r--   0 root         (0) root         (0)    14762 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/paraformer/predictor.py
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/speech_embed.py
+-rw-r--r--   0 root         (0) root         (0)     7361 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/subsampling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/layers/transducer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transducer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/layers/transformer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14943 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/attention.py
+-rw-r--r--   0 root         (0) root         (0)     4216 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/convolution.py
+-rw-r--r--   0 root         (0) root         (0)    15176 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/decoder.py
+-rw-r--r--   0 root         (0) root         (0)     9918 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/decoder_block.py
+-rw-r--r--   0 root         (0) root         (0)    12971 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/embedding.py
+-rw-r--r--   0 root         (0) root         (0)    12676 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    12678 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/encoder_block.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/forward.py
+-rw-r--r--   0 root         (0) root         (0)    41321 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/k2_conformer.py
+-rw-r--r--   0 root         (0) root         (0)    22729 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/layers/transformer/k2_scaling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/models/asr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24984 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/asr/paraformer.py
+-rw-r--r--   0 root         (0) root         (0)    29348 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/asr/transformer.py
+-rw-r--r--   0 root         (0) root         (0)      727 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/asr/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/base.py
+-rw-r--r--   0 root         (0) root         (0)    16050 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/saver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/models/vad/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/vad/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14141 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/vad/transformer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/models/vad/wavenet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/resources/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/resources/fetcher_config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/resources/fetcher_config/asr/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/resources/fetcher_config/asr/dynamic.yaml
+-rw-r--r--   0 root         (0) root         (0)      621 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/resources/fetcher_config/asr/static.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop/resources/model_config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/resources/model_config/asr/
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/resources/model_config/asr/conformer-base.yaml
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/resources/model_config/asr/lowrank_conformer-base.yaml
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/resources/model_config/asr/lowrank_transformer-base.yaml
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/resources/model_config/asr/paraformer-base.yaml
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/resources/model_config/asr/transformer-base.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/runx/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/runx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20579 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/runx/logx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/runx/mixins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/runx/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5539 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/runx/mixins/saver_mixins.py
+-rw-r--r--   0 root         (0) root         (0)     7454 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/runx/monitor.py
+-rw-r--r--   0 root         (0) root         (0)    23684 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/runx/trainer.py
+-rw-r--r--   0 root         (0) root         (0)     4172 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/runx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.267031 mountaintop-0.1.2/mountaintop/utils/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      954 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/utils/git.py
+-rw-r--r--   0 root         (0) root         (0)     4130 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-05-05 10:59:15.000000 mountaintop-0.1.2/mountaintop/utils/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:09:04.263031 mountaintop-0.1.2/mountaintop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-05 11:09:04.000000 mountaintop-0.1.2/mountaintop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4006 2023-05-05 11:09:04.000000 mountaintop-0.1.2/mountaintop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 11:09:04.000000 mountaintop-0.1.2/mountaintop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-05 11:09:04.000000 mountaintop-0.1.2/mountaintop.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-05 11:09:04.000000 mountaintop-0.1.2/mountaintop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-05 11:09:04.000000 mountaintop-0.1.2/mountaintop.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      130 2023-03-23 10:32:27.000000 mountaintop-0.1.2/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      149 2023-05-05 11:09:04.267031 mountaintop-0.1.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2056 2023-03-22 08:56:48.000000 mountaintop-0.1.2/setup.py
```

### Comparing `mountaintop-0.1.1.1/PKG-INFO` & `mountaintop-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mountaintop
-Version: 0.1.1.1
+Version: 0.1.2
 Summary: make research work more friendly
 Home-page: https://github.com/yinanxu0/mountaintop
 Author: yinanxu
 Author-email: yinanxu0@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `mountaintop-0.1.1.1/README.md` & `mountaintop-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/__init__.py` & `mountaintop-0.1.2/mountaintop/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/asr/__init__.py` & `mountaintop-0.1.2/mountaintop/bin/asr/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/asr/decode.py` & `mountaintop-0.1.2/mountaintop/bin/asr/decode.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/asr/wer.py` & `mountaintop-0.1.2/mountaintop/bin/asr/wer.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/average.py` & `mountaintop-0.1.2/mountaintop/bin/average.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/eval.py` & `mountaintop-0.1.2/mountaintop/bin/eval.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/export.py` & `mountaintop-0.1.2/mountaintop/bin/export.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/main.py` & `mountaintop-0.1.2/mountaintop/bin/main.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/parser.py` & `mountaintop-0.1.2/mountaintop/bin/parser.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/parser_base.py` & `mountaintop-0.1.2/mountaintop/bin/parser_base.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/profiler.py` & `mountaintop-0.1.2/mountaintop/bin/profiler.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/train.py` & `mountaintop-0.1.2/mountaintop/bin/train.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/bin/visual.py` & `mountaintop-0.1.2/mountaintop/bin/visual.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/configuration.py` & `mountaintop-0.1.2/mountaintop/configuration.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/core/audio/cmvn.py` & `mountaintop-0.1.2/mountaintop/core/audio/cmvn.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,20 +56,21 @@
             loggerx.error('kaldi cmvn binary file is not supported, please '
                           'recompute it by: compute-cmvn-stats --binary=false '
                           ' scp:feats.scp global_cmvn')
             sys.exit(1)
         fid.seek(0)
         arr = fid.read().split()
         assert (arr[0] == '[')
-        assert (arr[-2:] == '0]')
+        assert (arr[-2] == '0')
+        assert (arr[-1] == ']')
         feat_dim = int((len(arr) - 4) / 2)
         
-        means = map(float, arr[1 : feat_dim+1])
+        means.extend(map(float, arr[1 : feat_dim+1]))
         count = float(arr[feat_dim+1])
-        variance = map(float, arr[feat_dim+2 : 2*feat_dim+2])
+        variance.extend(map(float, arr[feat_dim+2 : 2*feat_dim+2]))
         
     return update(means, variance, count)
 
 
 def load_cmvn(cmvn_file, cmvn_type="json"):
     means, variance = None, None
     if not os.path.exists(cmvn_file):
```

### Comparing `mountaintop-0.1.1.1/mountaintop/core/audio/wer.py` & `mountaintop-0.1.2/mountaintop/core/audio/wer.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/core/beam_search.py` & `mountaintop-0.1.2/mountaintop/core/beam_search.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/core/internal/container.py` & `mountaintop-0.1.2/mountaintop/core/internal/container.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/core/internal/distribute.py` & `mountaintop-0.1.2/mountaintop/core/internal/distribute.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/core/internal/module.py` & `mountaintop-0.1.2/mountaintop/core/internal/module.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/core/internal/timing.py` & `mountaintop-0.1.2/mountaintop/core/internal/timing.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/core/ops/common.py` & `mountaintop-0.1.2/mountaintop/core/ops/common.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/core/ops/mask.py` & `mountaintop-0.1.2/mountaintop/core/ops/mask.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/dataset/asr/fetcher.py` & `mountaintop-0.1.2/mountaintop/dataset/asr/fetcher.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/dataset/asr/loader.py` & `mountaintop-0.1.2/mountaintop/dataset/asr/loader.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/dataset/base.py` & `mountaintop-0.1.2/mountaintop/dataset/base.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/dataset/sampler.py` & `mountaintop-0.1.2/mountaintop/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/dataset/vad/fetcher.py` & `mountaintop-0.1.2/mountaintop/dataset/vad/fetcher.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/dataset/vad/loader.py` & `mountaintop-0.1.2/mountaintop/dataset/vad/loader.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/activation.py` & `mountaintop-0.1.2/mountaintop/layers/activation.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/base/dataclass.py` & `mountaintop-0.1.2/mountaintop/layers/base/dataclass.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/base/interface.py` & `mountaintop-0.1.2/mountaintop/layers/base/interface.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/loss.py` & `mountaintop-0.1.2/mountaintop/layers/loss.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_attention.py` & `mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_attention.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_decoder.py` & `mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_decoder.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_decoder_block.py` & `mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_decoder_block.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_encoder.py` & `mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_encoder.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_encoder_block.py` & `mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_encoder_block.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/low_rank_transformer/low_rank_forward.py` & `mountaintop-0.1.2/mountaintop/layers/low_rank_transformer/low_rank_forward.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/normalization.py` & `mountaintop-0.1.2/mountaintop/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/optimizer.py` & `mountaintop-0.1.2/mountaintop/layers/optimizer.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/paraformer/decoder.py` & `mountaintop-0.1.2/mountaintop/layers/paraformer/decoder.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/paraformer/predictor.py` & `mountaintop-0.1.2/mountaintop/layers/paraformer/predictor.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/speech_embed.py` & `mountaintop-0.1.2/mountaintop/layers/speech_embed.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/subsampling.py` & `mountaintop-0.1.2/mountaintop/layers/subsampling.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/attention.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/attention.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/convolution.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/convolution.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/decoder.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/decoder_block.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/decoder_block.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/embedding.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/embedding.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/encoder.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/encoder_block.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/encoder_block.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/forward.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/forward.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/k2_conformer.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/k2_conformer.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/layers/transformer/k2_scaling.py` & `mountaintop-0.1.2/mountaintop/layers/transformer/k2_scaling.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/models/asr/paraformer.py` & `mountaintop-0.1.2/mountaintop/models/asr/paraformer.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/models/asr/transformer.py` & `mountaintop-0.1.2/mountaintop/models/asr/transformer.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/models/asr/utils.py` & `mountaintop-0.1.2/mountaintop/models/asr/utils.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/models/base.py` & `mountaintop-0.1.2/mountaintop/models/base.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/models/saver.py` & `mountaintop-0.1.2/mountaintop/models/saver.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/models/vad/transformer.py` & `mountaintop-0.1.2/mountaintop/models/vad/transformer.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/resources/__init__.py` & `mountaintop-0.1.2/mountaintop/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/resources/fetcher_config/asr/dynamic.yaml` & `mountaintop-0.1.2/mountaintop/resources/fetcher_config/asr/dynamic.yaml`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/resources/fetcher_config/asr/static.yaml` & `mountaintop-0.1.2/mountaintop/resources/fetcher_config/asr/static.yaml`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/conformer-base.yaml` & `mountaintop-0.1.2/mountaintop/resources/model_config/asr/conformer-base.yaml`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/lowrank_conformer-base.yaml` & `mountaintop-0.1.2/mountaintop/resources/model_config/asr/lowrank_conformer-base.yaml`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/lowrank_transformer-base.yaml` & `mountaintop-0.1.2/mountaintop/resources/model_config/asr/lowrank_transformer-base.yaml`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/paraformer-base.yaml` & `mountaintop-0.1.2/mountaintop/resources/model_config/asr/paraformer-base.yaml`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/resources/model_config/asr/transformer-base.yaml` & `mountaintop-0.1.2/mountaintop/resources/model_config/asr/transformer-base.yaml`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/runx/logx.py` & `mountaintop-0.1.2/mountaintop/runx/logx.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
 def get_logger(
     filepath: Optional[Union[Path, str]] = None,
     detail_level: int = 1
 ) -> logging.Logger:
     logger = logging.getLogger("mountaintop")
     logger.setLevel(logging.DEBUG)
+    # remove existed handler
+    if len(logger.handlers) > 0:
+        for handler in logger.handlers:
+            logger.removeHandler(handler)
     logger.addHandler(
         stream_handler(
             level=logging.INFO,
             detail_level=detail_level
         )
     )
     if filepath is not None:
@@ -233,14 +237,15 @@
         return _CallableProxy(real_fn, self.post_hook)
 
 
 class LoggerX(object):
     def __init__(self, rank=0):
         self._initialized = False
         self.detail_level = int(os.environ.get("DETAIL_LEVEL", 1))
+        self.logger = get_logger(filepath=None, detail_level=self.detail_level)
 
     def initialize(
         self,
         logdir: Union[str, Path] = "/tmp",
         to_file: bool = True,
         hparams=None,
         tensorboard=False,
@@ -349,93 +354,67 @@
 
         self._initialized = True
 
     def __del__(self):
         if self._initialized and self.is_master:
             self.metrics_fp.close()
 
-    def __check_initialized(self):
-        if not self._initialized:
-            print(
-                colored(
-                    "using loggerx before `initialize` is not allowed",
-                    "red"
-                )
-            )
-            return False
-        return True
-
-    def __check_master(self):
+    def _check_master(self):
         if not hasattr(self, 'is_master') or not self.is_master:
             return False
         return True
 
-    def __check_msg(self, msg: Any=""):
+    def _check_msg(self, msg: Any=""):
         if msg is None or len(msg) == 0:
             self.logger.warning(
                 "empty message for logger is not recommended, skip",
                 stacklevel=3
             )
             return False
         return True
 
     #### logger functions
     def debug(self, msg: Any, stacklevel=2, *args, **kwargs):
-        if not self.__check_master() or not self.__check_msg(msg):
-            return
-        if not self.__check_initialized():
-            print(f"{colored('loggerx not initialized', 'red')} => {msg}")
+        if not self._check_master() or not self._check_msg(msg):
             return
         self.logger.debug(msg, stacklevel=stacklevel, *args, **kwargs)
 
     def info(self, msg: Any, stacklevel=2, *args, **kwargs):
-        if not self.__check_master() or not self.__check_msg(msg):
-            return
-        if not self.__check_initialized():
-            print(f"{colored('loggerx not initialized', 'red')} => {msg}")
+        if not self._check_master() or not self._check_msg(msg):
             return
         self.logger.info(msg, stacklevel=stacklevel, *args, **kwargs)
     
     def warning(self, msg: Any, stacklevel=2, *args, **kwargs):
-        if not self.__check_master() or not self.__check_msg(msg):
-            return
-        if not self.__check_initialized():
-            print(f"{colored('loggerx not initialized', 'red')} => {msg}")
+        if not self._check_master() or not self._check_msg(msg):
             return
         self.logger.warning(msg, stacklevel=stacklevel, *args, **kwargs)
     
     def error(self, msg: Any, stacklevel=2, *args, **kwargs):
-        if not self.__check_master() or not self.__check_msg(msg):
-            return
-        if not self.__check_initialized():
-            print(f"{colored('loggerx not initialized', 'red')} => {msg}")
+        if not self._check_master() or not self._check_msg(msg):
             return
         self.logger.error(msg, stacklevel=stacklevel, *args, **kwargs)
     
     def critical(self, msg: Any, stacklevel=2, *args, **kwargs):
-        if not self.__check_master() or not self.__check_msg(msg):
-            return
-        if not self.__check_initialized():
-            print(f"{colored('loggerx not initialized', 'red')} => {msg}")
+        if not self._check_master() or not self._check_msg(msg):
             return
         self.logger.critical(msg, stacklevel=stacklevel, *args, **kwargs)
     
     def add_image(self, path, img, step=None):
         '''
         Write an image to the tensorboard file
         '''
-        if not self.__check_master() or not self.__check_initialized():
+        if not self._check_master():
             return
         self.tensorboard.add_image(path, img, step)
 
     def add_scalar(self, name, val, idx):
         '''
         Write a scalar to the tensorboard file
         '''
-        if not self.__check_master() or not self.__check_initialized():
+        if not self._check_master():
             return
         self.tensorboard.add_scalar(name, val, idx)
 
     def _flush_tensorboard(self):
         if self.eager_flush and self.tb_writer is not None:
             self.tb_writer.flush()
 
@@ -464,15 +443,15 @@
         sumx.
 
         Arguments:
             phase: 'train' or 'val'. sumx will only summarize val metrics.
             metrics: dictionary of metrics to record
             global_step: (optional) epoch or iteration number
         """
-        if not self.__check_master():
+        if not self._check_master():
             return
         canonical_phase = self._canonical_phase(phase=phase)
 
         if epoch is not None:
             self.epoch[canonical_phase] = epoch
 
         # Record metrics to csv file
@@ -526,15 +505,15 @@
                     best result
             higher_better: True if higher valued metric is better, False
                     otherwise
             delete_old: Delete prior 'lastest' checkpoints. By setting to
                     false, you'll get a checkpoint saved every time this
                     function is called.
         """
-        if not self.__check_master():
+        if not self._check_master():
             return
         
         if "__metric" not in save_dict:
             save_dict["__metric"] = metric
 
         if self.save_ckpt_path is not None and self.save_ckpt_path.exists() and delete_old:
             self.save_ckpt_path.unlink(missing_ok=True)
```

### Comparing `mountaintop-0.1.1.1/mountaintop/runx/mixins/saver_mixins.py` & `mountaintop-0.1.2/mountaintop/runx/mixins/saver_mixins.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/runx/monitor.py` & `mountaintop-0.1.2/mountaintop/runx/monitor.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/runx/trainer.py` & `mountaintop-0.1.2/mountaintop/runx/trainer.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/runx/utils.py` & `mountaintop-0.1.2/mountaintop/runx/utils.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/utils/git.py` & `mountaintop-0.1.2/mountaintop/utils/git.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/utils/misc.py` & `mountaintop-0.1.2/mountaintop/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop/utils/yaml.py` & `mountaintop-0.1.2/mountaintop/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/mountaintop.egg-info/PKG-INFO` & `mountaintop-0.1.2/mountaintop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mountaintop
-Version: 0.1.1.1
+Version: 0.1.2
 Summary: make research work more friendly
 Home-page: https://github.com/yinanxu0/mountaintop
 Author: yinanxu
 Author-email: yinanxu0@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `mountaintop-0.1.1.1/mountaintop.egg-info/SOURCES.txt` & `mountaintop-0.1.2/mountaintop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mountaintop-0.1.1.1/setup.py` & `mountaintop-0.1.2/setup.py`

 * *Files identical despite different names*

