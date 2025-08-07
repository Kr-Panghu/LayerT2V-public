<p align="center">
  <img src="assets/layert2v-logo.png" height=100>
</p>
<div align="center">

## LayerT2V: Interactive Multi-Object Trajectory Layering for Video Generation

[![Paper](https://img.shields.io/badge/Paper-gray)](https://kr-panghu.github.io/LayerT2V/assets/pdf/LayerT2V.pdf) &ensp; [![arXiv](https://img.shields.io/badge/arXiv-red)](https://arxiv.org/abs/2508.04228) &ensp; [![Project Page](https://img.shields.io/badge/Project%20Page-green
)](https://kr-panghu.github.io/LayerT2V/)

</div>

<p align="center">
<span class="author-block">
  <a href="https://kr-panghu.github.io/">Kangrui Cen</a>&nbsp&nbsp</span>
<span class="author-block">
  <a href="https://scholar.google.com/citations?user=i46wdAUAAAAJ&hl=zh-CN">Baixuan Zhao</a>&nbsp&nbsp</span>
<span class="author-block">
  <a href="https://synbol.github.io/">Yi Xin</a>&nbsp&nbsp</span>
<span class="author-block">
  <a href="https://scholar.google.com/citations?hl=en&user=_Cwn43wAAAAJ">Siqi Luo</a>&nbsp&nbsp</span>
<span class="author-block">
  <a href="https://scholar.google.com/citations?user=E6zbSYgAAAAJ&hl=en">Guangtao Zhai</a>&nbsp&nbsp</span>
<span class="author-block">
  <a href="https://jhc.sjtu.edu.cn/~xiaohongliu/">Xiaohong Liu</a>&nbsp&nbsp</span>
</p>


> ✨ We introduce LayerT2V, the first approach<sup>#</sup>  for generating video by compositing background and foreground objects layer by layer. This layered generation enables flexible integration of multiple independent elements within a video, positioning each element on a distinct "layer" and thus facilitating coherent multi-object synthesis while enhancing control over the generation process. Extensive experiments demonstrate the superiority of LayerT2V in generating complex multi-object scenarios, showcasing 1.4x and 4.5x improvements in mIoU and AP50 metrics over state-of-the-art (SOTA) methods.
>
> <sup>#</sup>Concurrent work: [LayerFlow](https://github.com/SihuiJi/LayerFlow).
> 
> 📧 Contact us: kangruicen@gmail.com or xiaohongliu@sjtu.edu.cn


<img src="./assets/layer-gen.png"
      alt="CIPT2V Pipeline Diagram"
      style="max-width: 90%; height: auto; display: block; margin: 0 auto 30px;">

## Demo

Comparisons with other methods:

* The bounding box on the video shows the input trajectory, our method demonstrates the best bbox-alignment and also prompt-alignment.
* Since our method generates videos in a layer-to-layer manner, visual quality of generated results are guaranteed.

<table align="center">
  <!-- 第一行：方法标签 -->
  <tr>
    <td align="center" width="256">MCtrl<sup>[1]</sup></td>
    <td align="center" width="256">Peek<sup>[2]</sup></td>
    <td align="center" width="256">Dav<sup>[3]</sup></td>
    <td align="center" width="256">Ours</td>
  </tr>

  <!-- deer-horse-grassland -->
  <tr>
    <td colspan="4" align="center">
      <img src="./assets/demo/deer-horse-grassland-row.gif" width="1024" height="256"/><br/>
      A deer and a horse running on the grassland.
    </td>
  </tr>

  <!-- duck-stone -->
  <tr>
    <td colspan="4" align="center">
      <img src="./assets/demo/duck-stone-row.gif" width="1024" height="256"/><br/>
      A duck and a stone floating in the pond of a park.
    </td>
  </tr>

  <!-- robot-corgi-beach -->
  <tr>
    <td colspan="4" align="center">
      <img src="./assets/demo/robot-corgi-beach-row.gif" width="1024" height="256"/><br/>
      A corgi and a robot running on the beach.
    </td>
  </tr>

  <!-- two-geese -->
  <tr>
    <td colspan="4" align="center">
      <img src="./assets/demo/two-geese-row.gif" width="1024" height="256"/><br/>
      Two geese swimming in the lake.
    </td>
  </tr>

  <!-- deer-bear-cabin -->
  <tr>
    <td colspan="4" align="center">
      <img src="./assets/demo/deer-bear-cabin-row.gif" width="1024" height="256"/><br/>
      A deer and a bear running on the grassland with a cabin in the distance.
    </td>
  </tr>

  <!-- jellyfish-carp -->
  <tr>
    <td colspan="4" align="center">
      <img src="./assets/demo/jellyfish-carp-row.gif" width="1024" height="256"/><br/>
      A jellyfish and a carp in the ocean.
    </td>
  </tr>
</table>





## Installation & Inference

<p>Codes will be organized shortly before submission ... Stay tuned! 🔥</p>


<br>


### References

~~~
[1] Wang Z, Yuan Z, Wang X, *et al.* MotionCtrl: A unified and flexible motion controller for video generation. In: *ACM SIGGRAPH Conference Papers*, 2024: 1–11.  
[2] Jain Y, Nasery A, Vineet V, *et al.* Peekaboo: Interactive video generation via masked diffusion. In: *CVPR*, 2024: 8079–8088.  
[3] Yang S, Hou L, Huang H, *et al.* Direct-A-Video: Customized video generation with user-directed camera movement and object motion. In: *ACM SIGGRAPH Conference Papers*, 2024: 1–12.
~~~


## Citation <a name="cite"></a>
```
@misc{cen2025layert2vinteractivemultiobjecttrajectory,
      title={LayerT2V: Interactive Multi-Object Trajectory Layering for Video Generation}, 
      author={Kangrui Cen and Baixuan Zhao and Yi Xin and Siqi Luo and Guangtao Zhai and Xiaohong Liu},
      year={2025},
      eprint={2508.04228},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2508.04228}, 
}
```