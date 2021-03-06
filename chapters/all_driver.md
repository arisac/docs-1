# List of 62 Drivers in Jina

This version of Jina includes 62 Drivers.

## Inheritances in a Tree View
- `JAMLCompatible`
   - `BaseDriver`
      - `BaseRecursiveDriver`
         - `BaseExecutableDriver`
            - `BaseEncodeDriver`
               - `MultiModalDriver`
               - `EncodeDriver`
            - `BasePredictDriver`
               - `BaseLabelPredictDriver`
                  - `BinaryPredictDriver`
                  - `OneHotPredictDriver`
                     - `MultiLabelPredictDriver`
               - `Prediction2DocBlobDriver`
            - `BaseIndexDriver`
               - `BaseCacheDriver`
                  - `TaggingCacheDriver`
               - `KVIndexDriver`
               - `VectorIndexDriver`
            - `BaseEvaluateDriver`
               - `FieldEvaluateDriver`
                  - `NDArrayEvaluateDriver`
                  - `RankEvaluateDriver`
                  - `TextEvaluateDriver`
            - `BaseSearchDriver`
               - `KVSearchDriver`
                  - `LoadGroundTruthDriver`
               - `QuerySetReader`
                  - `VectorFillDriver`
                  - `VectorSearchDriver`
            - `CraftDriver`
            - `BaseRankDriver`
               - `BaseAggregateMatchesRanker`
                  - `AggregateMatches2DocRankDriver`
                  - `Chunk2DocRankDriver`
               - `Matches2DocRankDriver`
            - `SegmentDriver`
         - `QuerySetReader`
            - `ReverseQL`
            - `SliceQL`
            - `SortQL`
            - `FilterQL`
            - `ExcludeQL`
               - `ExcludeReqQL`
                  - `SelectReqQL`
               - `SelectQL`
         - `ConvertDriver`
            - `Blob2PngURI`
            - `Buffer2URI`
            - `Text2URI`
            - `URI2Buffer`
            - `URI2DataURI`
            - `URI2Text`
         - `ReduceAllDriver`
            - `CollectEvaluationDriver`
            - `ConcatEmbedDriver`
      - `BaseControlDriver`
         - `ControlReqDriver`
            - `RouteDriver`
               - `ForwardDriver`
               - `ReduceDriver`
         - `LogInfoDriver`
         - `WaitDriver`

## Modules in a Table View 

| Class | Module |
| --- | --- |
| `AggregateMatches2DocRankDriver` | `jina.drivers.rank.aggregate` |
| `BaseAggregateMatchesRanker` | `jina.drivers.rank` |
| `BaseCacheDriver` | `jina.drivers.index` |
| `BaseControlDriver` | `jina.drivers.control` |
| `BaseDriver` |   |
| `BaseEncodeDriver` | `jina.drivers.index` |
| `BaseEvaluateDriver` | `jina.drivers.index` |
| `BaseExecutableDriver` | `jina.drivers.reduce` |
| `BaseIndexDriver` | `jina.drivers.index` |
| `BaseLabelPredictDriver` | `jina.drivers.predict` |
| `BasePredictDriver` | `jina.drivers.index` |
| `BaseRankDriver` | `jina.drivers.index` |
| `BaseRecursiveDriver` | `jina.drivers.control` |
| `BaseSearchDriver` | `jina.drivers.index` |
| `BinaryPredictDriver` | `jina.drivers.predict` |
| `Blob2PngURI` | `jina.drivers.convert` |
| `Buffer2URI` | `jina.drivers.convert` |
| `Chunk2DocRankDriver` | `jina.drivers.rank.aggregate` |
| `CollectEvaluationDriver` | `jina.drivers.reduce` |
| `ConcatEmbedDriver` | `jina.drivers.reduce` |
| `ControlReqDriver` | `jina.drivers.control` |
| `ConvertDriver` | `jina.drivers.reduce` |
| `CraftDriver` | `jina.drivers.index` |
| `EncodeDriver` | `jina.drivers.encode` |
| `ExcludeQL` |   |
| `ExcludeReqQL` | `jina.drivers.querylang.select` |
| `FieldEvaluateDriver` | `jina.drivers.evaluate` |
| `FilterQL` |   |
| `ForwardDriver` | `jina.drivers.control` |
| `JAMLCompatible` |   |
| `KVIndexDriver` | `jina.drivers.index` |
| `KVSearchDriver` | `jina.drivers.search` |
| `LoadGroundTruthDriver` | `jina.drivers.search` |
| `LogInfoDriver` | `jina.drivers.control` |
| `Matches2DocRankDriver` | `jina.drivers.rank` |
| `MultiLabelPredictDriver` | `jina.drivers.predict` |
| `MultiModalDriver` | `jina.drivers.encode` |
| `NDArrayEvaluateDriver` | `jina.drivers.evaluate` |
| `OneHotPredictDriver` | `jina.drivers.predict` |
| `Prediction2DocBlobDriver` | `jina.drivers.predict` |
| `QuerySetReader` | `jina.drivers.reduce` |
| `QuerySetReader` | `jina.drivers.search` |
| `RankEvaluateDriver` | `jina.drivers.evaluate` |
| `ReduceAllDriver` | `jina.drivers.reduce` |
| `ReduceDriver` | `jina.drivers.control` |
| `ReverseQL` |   |
| `RouteDriver` | `jina.drivers.control` |
| `SegmentDriver` | `jina.drivers.index` |
| `SelectQL` | `jina.drivers.querylang.select` |
| `SelectReqQL` | `jina.drivers.querylang.select` |
| `SliceQL` |   |
| `SortQL` |   |
| `TaggingCacheDriver` | `jina.drivers.cache` |
| `Text2URI` | `jina.drivers.convert` |
| `TextEvaluateDriver` | `jina.drivers.evaluate` |
| `URI2Buffer` | `jina.drivers.convert` |
| `URI2DataURI` | `jina.drivers.convert` |
| `URI2Text` | `jina.drivers.convert` |
| `VectorFillDriver` |   |
| `VectorIndexDriver` | `jina.drivers.index` |
| `VectorSearchDriver` |   |
| `WaitDriver` | `jina.drivers.control` |