# PHG-DIF & DT-PENS
The PyTorch open source implementation for the 34th ACM International Conference on Information and Knowledge Management (CIKM '25) paper "Improved Personalized Headline Generation via Denoising Fake Interests from Implicit Feedback".

[arXiv link](https://arxiv.org/abs/)
[ACM Digital Library link](https://dl.acm.org/doi/)



Please reach us via emails or via github issues for any enquiries!

## Citation

Please cite our work if you find it useful for your research and work.

```
@inproceedings{liu2025improved,
  title = {Improved Personalized Headline Generation via Denoising Fake Interests from Implicit Feedback},
  author = {Kejin Liu, Junhong Lian, Xiang Ao, Ningtao Wang, Xing Fu, Yu Cheng, Weiqiang Wang and Xinyu Liu},
  booktitle = {Proceedings of the 34th ACM International Conference on Information and Knowledge Management (CIKM '25)},
  year = {2025},
}
```

## Abstract
Accurate personalized headline generation hinges on precisely capturing user interests from historical behaviors. However, existing methods neglect personalized-irrelevant click noise in entire historical clickstreams, which may lead to hallucinated headlines that deviate from genuine user preferences. In this paper, we reveal the detrimental impact of click noise on personalized generation quality through rigorous analysis in both user and news dimensions. Based on these insights, we propose a novel **P**ersonalized **H**eadline **G**eneration framework via **D**enoising **F**ake **I**nterests from **I**mplicit **F**eedback (**PHG-DIF**). PHG-DIF first employs dual-stage filtering to effectively remove clickstream noise, identified by short dwell times and abnormal click bursts, and then leverages multi-level temporal fusion to dynamically model users’ evolving and multi-faceted interests for precise profiling. Moreover, we release **DT-PENS**, a new benchmark dataset comprising the click behavior of 1,000 carefully curated users and nearly 10,000 annotated personalized headlines with historical dwell time annotations. Extensive experiments demonstrate that PHG-DIF substantially mitigates the adverse effects of click noise and significantly improves headline quality, achieving state-of-the-art (SOTA) results on DT-PENS. Our framework implementation and dataset are available at [PHG-DIF](https://github.com/liukejin-up/PHG-DIF).



## The Framework of PHG-DIF

<img width="1868" height="1054" alt="image" src="https://github.com/user-attachments/assets/36130aac-34b1-48a2-ad96-5a53db9c1408" />

**Figure 2: Overview of the proposed PHG-DIF framework.**


## Requirements
Install requirements (in the cloned repository):

```
pip3 install -r requirements.txt
```

## Acknowledgements

This code framework is adapted and extended from the repository [PENS-Personalized-News-Headline-Generation](https://github.com/LLluoling/PENS-Personalized-News-Headline-Generation). We sincerely thank the original authors for their valuable work and contributions.


## Update

[2025-08-05]  We are excited to announce that our work has been accepted as a Full Research Paper at CIKM 2025! Additionally, the DT-PENS dataset has been released, and the remaining code for the PHG-DIF implementation will be available soon.

[2025-08-05]  We would like to acknowledge that the comments in this project have been automatically regenerated using `GLM-4.5`.
