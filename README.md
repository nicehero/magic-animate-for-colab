<!-- # magic-edit.github.io -->
## 🦒 Colab

| Colab | Info
| --- | --- |
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nicehero/magic-animate-for-colab/blob/main/magic_animate_colab.ipynb) | magic_animate_colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/camenduru/MagicAnimate-colab/blob/main/DensePose_colab.ipynb) | dense_pose_colab (Thanks to [DensePose](https://github.com/facebookresearch/detectron2/tree/main/projects/DensePose) ❤)

<p align="center">

  <h2 align="center">MagicAnimate: Temporally Consistent Human Image Animation using Diffusion Model</h2>
  <p align="center">
    <a href="https://scholar.google.com/citations?user=-4iADzMAAAAJ&hl=en"><strong>Zhongcong Xu</strong></a>
    ·
    <a href="http://jeff95.me/"><strong>Jianfeng Zhang</strong></a>
    ·
    <a href="https://scholar.google.com.sg/citations?user=8gm-CYYAAAAJ&hl=en"><strong>Jun Hao Liew</strong></a>
    ·
    <a href="https://hanshuyan.github.io/"><strong>Hanshu Yan</strong></a>
    ·
    <a href="https://scholar.google.com/citations?user=stQQf7wAAAAJ&hl=en"><strong>Jia-Wei Liu</strong></a>
    ·
    <a href="https://zhangchenxu528.github.io/"><strong>Chenxu Zhang</strong></a>
    ·
    <a href="https://sites.google.com/site/jshfeng/home"><strong>Jiashi Feng</strong></a>
    ·
    <a href="https://sites.google.com/view/showlab"><strong>Mike Zheng Shou</strong></a>
    <br>
    <br>
        <a href="https://arxiv.org/abs/2311.16498"><img src='https://img.shields.io/badge/arXiv-MagicAnimate-red' alt='Paper PDF'></a>
        <a href='https://showlab.github.io/magicanimate'><img src='https://img.shields.io/badge/Project_Page-MagicAnimate-green' alt='Project Page'></a>
        <a href='https://huggingface.co/spaces/zcxu-eric/magicanimate'><img src='https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue'></a>
    <br>
    <b>National University of Singapore &nbsp; | &nbsp;  ByteDance</b>
  </p>
  
  <table align="center">
    <tr>
    <td>
      <img src="assets/teaser/t4.gif">
    </td>
    <td>
      <img src="assets/teaser/t2.gif">
    </td>
    </tr>
  </table>

## 📢 News
* **[2023.12.8]** Add loading  local safetensors or ckpt,you can change `config/prompts/animation.yaml` about `pretrained_model_path` for your local SD1.5 model.
such as `"D:\\stablediffusion-webui\\models\Stable-diffusion\\v1-5-pruned.ckpt"`
* **[2023.12.4]** Release inference code and gradio demo. We are working to improve MagicAnimate, stay tuned!
* **[2023.11.23]** Release MagicAnimate paper and project page.


## ⚒️ Installation
prerequisites: `python>=3.8`, `CUDA>=11.3`, `ffmpeg` and `git`.

Python and Git:

- Python 3.10.11: https://www.python.org/ftp/python/3.10.11/python-3.10.11-amd64.exe
- git: https://git-scm.com/download/win

- Install [ffmpeg](https://ffmpeg.org/) for your operating system
  (https://www.geeksforgeeks.org/how-to-install-ffmpeg-on-windows/)
  
  notice:step 4 use windows system Set Enviroment Path.

Give unrestricted script access to powershell so venv can work:

- Open an administrator powershell window
- Type `Set-ExecutionPolicy Unrestricted` and answer A
- Close admin powershell window

Install with Powershell run `install.ps1` or `install-cn.ps1`(for Chinese)

###Use local model

Add loading local safetensors or ckpt,you can change `config/prompts/animation.yaml` about `pretrained_model_path` for your local SD1.5 model.
such as `"D:\\stablediffusion-webui\\models\Stable-diffusion\\v1-5-pruned.ckpt"`

## 🎨 Gradio Demo 

#### Online Gradio Demo:
Try our [online gradio demo](https://huggingface.co/spaces/zcxu-eric/magicanimate) quickly.

#### Local Gradio Demo:
Launch local gradio demo on single GPU:

Powershell run with `run_gui.ps1`

Launch local gradio demo if you have multiple GPUs:

Edit `run_gui.ps1` set `$mutil_gpu=1` then run.

Then open gradio demo in local browser.

## 🙏 Acknowledgements
We would like to thank [AK(@_akhaliq)](https://twitter.com/_akhaliq?lang=en) and huggingface team for the help of setting up oneline gradio demo.

## 🎓 Citation
If you find this codebase useful for your research, please use the following entry.
```BibTeX
@inproceedings{xu2023magicanimate,
    author    = {Xu, Zhongcong and Zhang, Jianfeng and Liew, Jun Hao and Yan, Hanshu and Liu, Jia-Wei and Zhang, Chenxu and Feng, Jiashi and Shou, Mike Zheng},
    title     = {MagicAnimate: Temporally Consistent Human Image Animation using Diffusion Model},
    booktitle = {arXiv},
    year      = {2023}
}
```

