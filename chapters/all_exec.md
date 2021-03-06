# List of 123 Executors in Jina

This version of Jina includes 123 Executors.

## Inheritances in a Tree View
- `JAMLCompatible`
   - `BaseExecutor`
      - `BaseMultiModalEncoder`
         - `BaseDevice`
            - `TorchDevice`
               - `TirgMultiModalEncoder`
      - `BaseEvaluator`
         - `BaseRankingEvaluator`
            - `f1ScoreEvaluator`
            - `NDCGEvaluator`
            - `ReciprocalRankEvaluator`
            - `AveragePrecisionEvaluator`
         - `BaseTextEvaluator`
            - `RougeEvaluator`
            - `EditDistanceEvaluator`
            - `HammingDistanceEvaluator`
            - `BleuEvaluator`
            - `JaccardSimilarityEvaluator`
            - `GleuEvaluator`
         - `BaseEmbeddingEvaluator`
            - `InfiniteNormEvaluator`
            - `MinkowskiDistanceEvaluator`
            - `L1NormEvaluator`
      - `BaseEncoder`
         - `BaseDevice`
            - `TorchDevice`
               - `BaseTorchEncoder`
                  - `TirgImageEncoder`
                  - `ImageTorchEncoder`
                  - `FlairTextEncoder`
                  - `LaserEncoder`
                  - `VSETextEncoder`
                  - `VSEImageEncoder`
                  - `CustomImageTorchEncoder`
                  - `FarmTextEncoder`
               - `TransformerTorchEncoder`
            - `TFDevice`
               - `TransformerTFEncoder`
               - `BaseTFEncoder`
                  - `BigTransferEncoder`
                  - `CustomKerasImageEncoder`
                  - `ImageKerasEncoder`
            - `PaddleDevice`
               - `BasePaddleEncoder`
                  - `TextPaddlehubEncoder`
                  - `ImagePaddlehubEncoder`
                  - `VideoPaddleEncoder`
            - `OnnxDevice`
               - `BaseOnnxEncoder`
                  - `ImageOnnxEncoder`
         - `BaseNumericEncoder`
            - `BaseAudioEncoder`
               - `ChromaPitchEncoder`
               - `MFCCTimbreEncoder`
               - `BaseDevice`
                  - `TorchDevice`
                     - `BaseTorchEncoder`
                        - `Wav2VecSpeechEncoder`
            - `TransformEncoder`
               - `RandomGaussianEncoder`
               - `RandomSparseEncoder`
               - `FeatureAgglomerationEncoder`
               - `FastICAEncoder`
               - `IncrementalPCAEncoder`
            - `BaseDevice`
               - `TFDevice`
                  - `CompressionVaeEncoder`
            - `BaseVideoEncoder`
               - `BaseDevice`
                  - `TorchDevice`
                     - `BaseTorchEncoder`
                        - `VideoTorchEncoder`
            - `TSNEEncoder`
         - `BaseTextEncoder`
            - `OneHotTextEncoder`
      - `BaseIndexer`
         - `BaseVectorIndexer`
            - `BaseNumpyIndexer`
               - `NGTIndexer`
               - `NmsLibIndexer`
               - `BaseDevice`
                  - `FaissDevice`
                     - `FaissIndexer`
               - `SptagIndexer`
               - `NumpyIndexer`
                  - `ZarrIndexer`
               - `ScannIndexer`
               - `AnnoyIndexer`
            - `MilvusIndexer`
         - `BaseKVIndexer`
            - `BinaryPbIndexer`
               - `RedisDBIndexer`
               - `LevelDBIndexer`
               - `MongoDBIndexer`
      - `BaseCrafter`
         - `ImageFlipper`
         - `AlbumentationsCrafter`
         - `AudioMonophoner`
         - `AudioNormalizer`
         - `ImageReader`
         - `ImageNormalizer`
         - `ArrayBytesReader`
         - `ImageCropper`
         - `ArrayStringReader`
         - `CenterImageCropper`
         - `ImageResizer`
         - `AudioReader`
         - `TikaExtractor`
      - `BaseSegmenter`
         - `RandomImageCropper`
         - `SlidingWindowImageCropper`
         - `JiebaSegmenter`
         - `DeepSegmenter`
         - `BaseDevice`
            - `TorchDevice`
               - `TorchObjectDetectionSegmenter`
         - `Sentencizer`
         - `PDFExtractorSegmenter`
         - `SlidingWindowSegmenter`
         - `FiveImageCropper`
         - `SlidingWindowAudioSlicer`
         - `AudioSlicer`
      - `BaseRanker`
         - `Chunk2DocRanker`
            - `BiMatchRanker`
            - `BM25Ranker`
            - `TfIdfRanker`
            - `SimpleAggregateRanker`
         - `Match2DocRanker`
            - `LevenshteinRanker`

## Modules in a Table View 

| Class | Module |
| --- | --- |
| `AlbumentationsCrafter` | `jina.hub.crafters.nlp.TikaExtractor` |
| `AnnoyIndexer` | `jina.hub.indexers.vector.AnnoyIndexer` |
| `ArrayBytesReader` | `jina.hub.crafters.nlp.TikaExtractor` |
| `ArrayStringReader` | `jina.hub.crafters.nlp.TikaExtractor` |
| `AudioMonophoner` | `jina.hub.crafters.nlp.TikaExtractor` |
| `AudioNormalizer` | `jina.hub.crafters.nlp.TikaExtractor` |
| `AudioReader` | `jina.hub.crafters.nlp.TikaExtractor` |
| `AudioSlicer` | `jina.hub.segmenters.audio.AudioSlicer` |
| `AveragePrecisionEvaluator` | `jina.hub.evaluators.rank.AveragePrecision` |
| `BM25Ranker` | `jina.hub.rankers.SimpleAggregateRanker` |
| `BaseAudioEncoder` | `jina.hub.encoders.numeric.TSNEEncoder` |
| `BaseCrafter` |   |
| `BaseDevice` | `jina.hub.encoders.audio.Wav2VecSpeechEncoder` |
| `BaseDevice` | `jina.hub.encoders.multimodal.TirgMultimodalEncoder` |
| `BaseDevice` | `jina.hub.encoders.nlp.TransformerTorchEncoder` |
| `BaseDevice` | `jina.hub.encoders.numeric.TSNEEncoder` |
| `BaseDevice` | `jina.hub.encoders.video.VideoTorchEncoder` |
| `BaseDevice` | `jina.hub.indexers.vector.AnnoyIndexer` |
| `BaseDevice` | `jina.hub.segmenters.audio.AudioSlicer` |
| `BaseEmbeddingEvaluator` |   |
| `BaseEncoder` |   |
| `BaseEvaluator` |   |
| `BaseExecutor` |   |
| `BaseIndexer` |   |
| `BaseKVIndexer` |   |
| `BaseMultiModalEncoder` |   |
| `BaseNumericEncoder` | `jina.hub.encoders.nlp.TransformerTorchEncoder` |
| `BaseNumpyIndexer` | `jina.hub.indexers.vector.MilvusIndexer` |
| `BaseOnnxEncoder` |   |
| `BasePaddleEncoder` |   |
| `BaseRanker` |   |
| `BaseRankingEvaluator` |   |
| `BaseSegmenter` |   |
| `BaseTFEncoder` |   |
| `BaseTextEncoder` | `jina.hub.encoders.nlp.TransformerTorchEncoder` |
| `BaseTextEvaluator` |   |
| `BaseTorchEncoder` |   |
| `BaseVectorIndexer` |   |
| `BaseVideoEncoder` | `jina.hub.encoders.numeric.TSNEEncoder` |
| `BiMatchRanker` | `jina.hub.rankers.SimpleAggregateRanker` |
| `BigTransferEncoder` | `jina.hub.encoders.image.ImageKerasEncoder` |
| `BinaryPbIndexer` |   |
| `BleuEvaluator` | `jina.hub.evaluators.text.GleuEvaluator` |
| `CenterImageCropper` | `jina.hub.crafters.nlp.TikaExtractor` |
| `ChromaPitchEncoder` | `jina.hub.encoders.audio.Wav2VecSpeechEncoder` |
| `Chunk2DocRanker` |   |
| `CompressionVaeEncoder` |   |
| `CustomImageTorchEncoder` | `jina.hub.encoders.nlp.FarmTextEncoder` |
| `CustomKerasImageEncoder` | `jina.hub.encoders.image.ImageKerasEncoder` |
| `DeepSegmenter` | `jina.hub.segmenters.audio.AudioSlicer` |
| `EditDistanceEvaluator` | `jina.hub.evaluators.text.GleuEvaluator` |
| `FaissDevice` |   |
| `FaissIndexer` |   |
| `FarmTextEncoder` | `jina.hub.encoders.nlp.FarmTextEncoder` |
| `FastICAEncoder` | `jina.hub.encoders.numeric.IncrementalPCAEncoder` |
| `FeatureAgglomerationEncoder` | `jina.hub.encoders.numeric.IncrementalPCAEncoder` |
| `FiveImageCropper` | `jina.hub.segmenters.audio.AudioSlicer` |
| `FlairTextEncoder` | `jina.hub.encoders.nlp.FarmTextEncoder` |
| `GleuEvaluator` | `jina.hub.evaluators.text.GleuEvaluator` |
| `HammingDistanceEvaluator` | `jina.hub.evaluators.text.GleuEvaluator` |
| `ImageCropper` | `jina.hub.crafters.nlp.TikaExtractor` |
| `ImageFlipper` | `jina.hub.crafters.nlp.TikaExtractor` |
| `ImageKerasEncoder` | `jina.hub.encoders.image.ImageKerasEncoder` |
| `ImageNormalizer` | `jina.hub.crafters.nlp.TikaExtractor` |
| `ImageOnnxEncoder` | `jina.hub.encoders.image.ImageOnnxEncoder` |
| `ImagePaddlehubEncoder` | `jina.hub.encoders.video.VideoPaddleEncoder` |
| `ImageReader` | `jina.hub.crafters.nlp.TikaExtractor` |
| `ImageResizer` | `jina.hub.crafters.nlp.TikaExtractor` |
| `ImageTorchEncoder` | `jina.hub.encoders.nlp.FarmTextEncoder` |
| `IncrementalPCAEncoder` | `jina.hub.encoders.numeric.IncrementalPCAEncoder` |
| `InfiniteNormEvaluator` | `jina.hub.evaluators.embedding.L1NormEvaluator` |
| `JAMLCompatible` |   |
| `JaccardSimilarityEvaluator` | `jina.hub.evaluators.text.GleuEvaluator` |
| `JiebaSegmenter` | `jina.hub.segmenters.audio.AudioSlicer` |
| `L1NormEvaluator` | `jina.hub.evaluators.embedding.L1NormEvaluator` |
| `LaserEncoder` | `jina.hub.encoders.nlp.FarmTextEncoder` |
| `LevelDBIndexer` | `jina.hub.indexers.keyvalue.MongoDBIndexer` |
| `LevenshteinRanker` | `jina.hub.rankers.LevenshteinRanker` |
| `MFCCTimbreEncoder` | `jina.hub.encoders.audio.Wav2VecSpeechEncoder` |
| `Match2DocRanker` |   |
| `MilvusIndexer` | `jina.hub.indexers.vector.MilvusIndexer` |
| `MinkowskiDistanceEvaluator` | `jina.hub.evaluators.embedding.L1NormEvaluator` |
| `MongoDBIndexer` | `jina.hub.indexers.keyvalue.MongoDBIndexer` |
| `NDCGEvaluator` | `jina.hub.evaluators.rank.AveragePrecision` |
| `NGTIndexer` | `jina.hub.indexers.vector.AnnoyIndexer` |
| `NmsLibIndexer` | `jina.hub.indexers.vector.AnnoyIndexer` |
| `NumpyIndexer` | `jina.hub.indexers.vector.AnnoyIndexer` |
| `OneHotTextEncoder` | `jina.hub.encoders.nlp.OneHotTextEncoder` |
| `OnnxDevice` |   |
| `PDFExtractorSegmenter` | `jina.hub.segmenters.audio.AudioSlicer` |
| `PaddleDevice` |   |
| `RandomGaussianEncoder` | `jina.hub.encoders.numeric.IncrementalPCAEncoder` |
| `RandomImageCropper` | `jina.hub.segmenters.audio.AudioSlicer` |
| `RandomSparseEncoder` | `jina.hub.encoders.numeric.IncrementalPCAEncoder` |
| `ReciprocalRankEvaluator` | `jina.hub.evaluators.rank.AveragePrecision` |
| `RedisDBIndexer` | `jina.hub.indexers.keyvalue.MongoDBIndexer` |
| `RougeEvaluator` | `jina.hub.evaluators.text.GleuEvaluator` |
| `ScannIndexer` | `jina.hub.indexers.vector.AnnoyIndexer` |
| `Sentencizer` | `jina.hub.segmenters.audio.AudioSlicer` |
| `SimpleAggregateRanker` | `jina.hub.rankers.SimpleAggregateRanker` |
| `SlidingWindowAudioSlicer` | `jina.hub.segmenters.audio.AudioSlicer` |
| `SlidingWindowImageCropper` | `jina.hub.segmenters.audio.AudioSlicer` |
| `SlidingWindowSegmenter` | `jina.hub.segmenters.audio.AudioSlicer` |
| `SptagIndexer` | `jina.hub.indexers.vector.AnnoyIndexer` |
| `TFDevice` |   |
| `TSNEEncoder` | `jina.hub.encoders.numeric.TSNEEncoder` |
| `TextPaddlehubEncoder` | `jina.hub.encoders.video.VideoPaddleEncoder` |
| `TfIdfRanker` | `jina.hub.rankers.SimpleAggregateRanker` |
| `TikaExtractor` | `jina.hub.crafters.nlp.TikaExtractor` |
| `TirgImageEncoder` | `jina.hub.encoders.nlp.FarmTextEncoder` |
| `TirgMultiModalEncoder` |   |
| `TorchDevice` |   |
| `TorchObjectDetectionSegmenter` |   |
| `TransformEncoder` | `jina.hub.encoders.numeric.TSNEEncoder` |
| `TransformerTFEncoder` |   |
| `TransformerTorchEncoder` |   |
| `VSEImageEncoder` | `jina.hub.encoders.nlp.FarmTextEncoder` |
| `VSETextEncoder` | `jina.hub.encoders.nlp.FarmTextEncoder` |
| `VideoPaddleEncoder` | `jina.hub.encoders.video.VideoPaddleEncoder` |
| `VideoTorchEncoder` |   |
| `Wav2VecSpeechEncoder` |   |
| `ZarrIndexer` | `jina.hub.indexers.vector.ZarrIndexer` |
| `f1ScoreEvaluator` | `jina.hub.evaluators.rank.AveragePrecision` |