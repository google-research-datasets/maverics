# MAVERICS 

<p align="center">
  <img width="680.25" height="504" src="/images/vq2a_examples.png">
</p>

We introduce Manually vAlidated Vq2a Examples fRom Image/Caption datasetS (MAVERICS), a suite of test-only visual question answering datasets.
The datasets are created from image captions by Visual Question Generation with Question Answering validation, or VQ^2A (see the figure below), followed by manual verification.
Check our [paper](https://arxiv.org/abs/2205.01883) for further details.

<p align="center">
  <img width="576" height="324" src="/images/gif_vq2a_approach.gif">
</p>

## Download

[COCO minival2014](https://storage.googleapis.com/maverics/maverics_coco.json) (193KB), generated from [COCO Captions](https://cocodataset.org/#captions-2015).

[CC3M dev](https://storage.googleapis.com/maverics/maverics_cc3m.json) (177KB), generated from [Conceptual Captions](https://github.com/google-research-datasets/conceptual-captions).

**Format (.json)**
<div class="highlight highlight-source-shell"><pre>
dataset               str: dataset name
split                 str: dataset split
annotations           List of image-question-answers triplets, each of which is
-- image_id           str: image ID
-- caption            str: image caption
-- qa_pairs           List of question-answer pairs, each of which is
---- question_id      str: question ID
---- raw_question     str: raw question
---- question         str: processed question
---- answers          List of str: 10 ground-truth answers
</pre></div>

## Cite

If you use this dataset in your research, please cite the original image caption datasets and our paper:

Soravit Changpinyo*, Doron Kukliansky*, Idan Szpektor, Xi Chen, Nan Ding, Radu Soricut.
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

## Related Datasets
A multilingual extension of this approach and its accompanied dataset MaXM can be found on [this page](https://github.com/google-research-datasets/maxm/).

## Contact Us

Please create an issue in this repository. If you would like to share feedback or report concerns, please email schangpi@google.com.
