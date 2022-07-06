# MAVERICS 

<p align="center">
  <img width="312" height="192" src="/images/gif_vq2a_approach.jpg">
</p>

We introduce Manually vAlidated Vq2a Examples fRom Image/Caption datasetS (MAVERICS), a suite of test-only visual question answering datasets.
The datasets are created from image captions by Visual Question Generation with Question Answering validation, or VQ^2A (see the figure below), followed by manual verification.
Check our [paper](https://arxiv.org/abs/2205.01883) for further details.

<p align="center">
  <img width="192" height="312" src="/images/gif_vq2a_approach.jpg">
</p>

## Download
[COCO minival2014](https://storage.googleapis.com/maverics/maverics_coco.json) (193KB)
[CC3M dev](https://storage.googleapis.com/maverics/maverics_cc3m.json) (177KB)


**Format (.json)**
<div class="highlight highlight-source-shell"><pre>
dataset
split
annotations
- image_id
- caption
- qa_pairs
-- question_id
-- raw_question
-- question
-- answers
</pre></div>

## Cite

If you use this dataset in your research, please cite:

Soravit Changpinyo, Piyush Sharma, Nan Ding, Radu Soricut.
[All You May Need for VQA are Image Captions](https://arxiv.org/abs/2205.01883).
NAACL 2022.

<div class="highlight highlight-source-shell"><pre>
@inproceedings{changpinyo2022vq2a,
  title = {All You May Need for VQA are Image Captions},
  author = {Changpinyo, Soravit and Kukliansky, Doron and Szpektor, Idan and Chen, Xi and Ding, Nan and Soricut, Radu},
  booktitle = {NAACL},
  year = {2022},
}
</pre></div>

## Contact Us

Please create an issue in this repository. If you would like to share feedback or report concerns, please email schangpi@google.com.
