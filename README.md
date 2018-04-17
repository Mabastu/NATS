# Text summarization

Abstractive Text Summarization with Attentive Sequence-to-Sequence Models: Basic Elements.

## Requirements

- Python 2.7
- glob
- argparse
- shutil
- Pytorch 0.3.0.post4

You can use these two [scripts](https://github.com/tshi04/seq2seq_coverage_ST/tree/master/tools/CONFIG)
to setup AWS K80.

## Usuage

Please set parameters within the main.py file.

- Training
```
python main.py 
```
- Validate
```
python main.py --task validate --batch_size 10
```
- Test
```
python main.py --task beam --batch_size 4
```
- Rouge
```
python main.py --task rouge
```

## Problem

1. The following combination failed during the training.
```
concat + temporal
concat + temporal + attn_decoder
```


## Git Referenced

- https://github.com/abisee/pointer-generator.git
- https://github.com/MaximumEntropy/Seq2Seq-PyTorch
- https://github.com/OpenNMT/OpenNMT
- https://github.com/spro/practical-pytorch
