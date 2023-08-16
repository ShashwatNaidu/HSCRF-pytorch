## Usage
Glove: You can find the pre-trained word embedding [here](https://nlp.stanford.edu/projects/glove/)

emb_file: path to the above pre trained word embedding file

train_file: keep a name for the processed train file

test_file: keep a name for the processed test file

train_file_csv: provide the input csv train file

test_file_csv: provide input csv test file

labels_json: provide input of labels json file

```
CUDA_VISIBLE_DEVICES=0 python train.py --char_lstm --high_way --emb_file '/kaggle/input/glovedata/glove.6B.100d.txt' --train_file '/kaggle/working/train.txt' --test_file '/kaggle/working/test.txt' --train_file_csv '/kaggle/input/ner-formatted/train (4).csv' --test_file_csv '/kaggle/input/ner-formatted/test (5).csv' --labels_json '/kaggle/input/ner-formatted/labels (6).json'
```


### word embeddings

Glove: You can find the pre-trained word embedding [here](https://nlp.stanford.edu/projects/glove/),
and place glove.6B.100d.txt in `data/`.

## Cite

If you use the code, please cite the following paper:
**"Hybrid semi-Markov CRF for Neural Sequence Labeling"**
Zhi-Xiu Ye, Zhen-Hua Ling. _ACL (2018)_

```
@InProceedings{HSCRF,
  author = 	"Ye, Zhixiu
		and Ling, Zhen-Hua",
  title = 	"Hybrid semi-Markov CRF for Neural Sequence Labeling",
  booktitle = 	"Proceedings of the 56th Annual Meeting of the Association for Computational Linguistics (Volume 2: Short Papers)",
  year = 	"2018",
  publisher = 	"Association for Computational Linguistics",
  pages = 	"235--240",
  location = 	"Melbourne, Australia",
  url = 	"http://aclweb.org/anthology/P18-2038"
}
```
