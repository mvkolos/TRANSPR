# TRANSPR: Transparency Ray-Accumulating Neural 3D Scene Point Renderer
### <img align=center src=./docs/images/project.png width='32'/> [Project page](https://saic-violet.github.io/transpr) &ensp; <img align=center src=./docs/images/paper.png width='24'/> [Paper](https://arxiv.org/pdf/2009.02819.pdf)

[TRANSPR: Transparency Ray-Accumulating Neural 3D Scene Point Renderer](https://arxiv.org/pdf/2009.02819.pdf)<br>
[Maria Kolos*](https://github.com/mvkolos)<sup>1</sup> &nbsp;
[Artem Sevastopolsky*](https://seva100.github.io)<sup>1,2</sup> &nbsp;
[Victor Lempitsky](http://sites.skoltech.ru/compvision/members/vilem/)<sup>1,2</sup> <br>
<sup>1</sup>Samsung AI Center &nbsp; <sup>1</sup>Skolkovo Institute of Science and Technology <br><br>
\* *indicates equal contribution*

<br>

### <b>Code: *Coming soon...*</b> (planned release month: **November '20**)<br>

<img src=docs/images/teaser.png width=1200>

## About

This is a PyTorch implementation of TRANSPR, a new method for realtime photo-realistic rendering of 3D scenes with semi-transparent parts and complex geometry. This method is an extension of [Neural Point-Based Graphics](https://saic-violet.github.io/npbg) (NPBG) which uses a raw point cloud as the geometric representation of a scene, and augments each point with a learnable neural descriptor that encodes local geometry and appearance. In our method, we expand the descriptor with a learned transparency value, use ray accumulation to account all points perceived by the camera. The points along the rays are fused into an opacity-aware 2D representation processed by the rendering network. Several scenes can be rendered in conjunction, opacity of objects can be edited, and the non-transparent objects can be combined with the introduced transparency. The repository extends NPBG with the additional features. 

<img src=docs/images/pipeline.png width=1200>
