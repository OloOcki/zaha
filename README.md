# :cityscape: ZAHA :cityscape:

**To date the largest benchmark for facade semantic segmentation of point clouds** 

[[Download]](https://tumde-my.sharepoint.com/:f:/g/personal/olaf_wysocki_tum_de/EjEtcRdYt0NOvilNerUesF0Bb-3uADnmzcI3LqTYS729Vg?e=mWCGSd) [[Benchmark]](https://tum2t.win/benchmarks/pc-fac) [[WACV25 Paper]](https://arxiv.org/abs/2411.04865) [[More]](https://tum2t.win/datasets/pc-mls)

Password: 
```bash copy
zahahadid
```
<p align="center">
    <img src="https://github.com/OloOcki/zaha/blob/main/img/overview_figure_wacv_legend.png" width="75%" title="overview"/>
</p>

<p align="center">
    <img src="https://github.com/OloOcki/zaha/blob/main/img/classes_testset_colorcoded_trans.png" width="75%" title="classes"/>
</p>

<p align="center">
    <img src="https://github.com/OloOcki/zaha/blob/main/img/zahaAnimated.gif" width="75%" title="classes"/>
</p>

## :star2: Highlights
- **601 mln** annotated points
- Introducing LoFG: Level of Facade Generalization enabling hierarchical understanding of facades
- Various architectural styles
- In **local** and **global** (i.e., UTM) coordinate reference system (if struggling with the [height transformation](https://www.ldbv.bayern.de/vermessung/utm_umstellung/koordinatentrafo.html) - apply 45.66 m vertical offset)
- File names point to the official CityGML LoD2 building models of Bavaria (e.g., DEBY_LOD2_4959462 -> gml_id=DEBY_LOD2_4959462) [[visualisation](https://www.virtualcitymap.de/?lang=de&layerToActivate=%5B%22Bayern%20-%20LOD2%20(pbr)%22%2C%22Sachsen%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Sachsen-Anhalt%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Th%C3%BCringen%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Niedersachsen%20(pbr%20recalculation)%22%2C%22NRW%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Hessen%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Hamburg%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Brandenburg%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Berlin%20untexturiert%20openData%20(pbr%20recalculation)%22%2C%22GermanyBaseTerrain%22%5D&layerToDeactivate=%5B%22Mesh%20Classification%20Layer%22%2C%22mesh_surface%22%5D&startingmap=Cesium%20Map&cameraPosition=11.56952%2C48.14564%2C875.76828&groundPosition=11.56721%2C48.14877%2C523.42063&distance=524.27&pitch=-42.23&heading=333.69&roll=359.89#/)]   
- The settings file for **adding your own data**

### :mag_right: Facade Semantic Segmentation Results at LoFG3

LoFG stands for Level of Facade Generalization. See more in the ZAHA paper introducing the concept [here, pending](pending).

|  | PointNet      | PointNet++ | Point Transformer | DGCNN         |
|-----------------|---------------|------------|-------------------|---------------|
| OA              | 59.9          | 66.4       | **75.0**     | 71.1          |
| P          | 46.1          | 37.8       | 52.7              | **53.6** |
| R          | 42.2          | 35.9       | **54.7**     | 45.8          |
| F1         | 38.7          | 34.8       | **52.1**     | 44.5          |
| IoU        | 26.4          | 25.6       | **41.6**     | 33.4          |
| **Class scores**            | |           |        |               |  
| wall            | 61.1          | 68.5       | 76.8              | **83.8** |
| window          | 25.6          | 26.3       | 43.1              | **64.1** |
| door            | 13.5          | 7.8        | 19.8              | **21.6** |
| balcony         | 25.1          | 0.0        | **77.5**     | 66.7          |
| molding         | 22.5          | 43.4       | **58.0**     | 57.5          |
| deco            | 0.0           | 0.0        | **5.0**      | 0.0           |
| column          | 22.4          | 33.4       | 0.0               | **37.2** |
| arch            | 19.2          | 25.4       | **50.2**     | 2.6           |
| stairs          | **16.0** | 0.0        | 7.5               | 5.6           |
| ground surface  | 12.0          | 0.0        | **24.4**     | 21.3          |
| terrain         | 53.5          | 53.5       | 57.6              | **68.0** |
| roof            | 18.7          | 6.8        | **66.3**     | 57.4          |
| blinds          | 4.6           | 2.3        | 18.5              | **20.0** |
| interior        | 59.7          | 69.1       | 72.8              | **88.0** |
| other           | 42.7          | 47.1       | 70.6              | **74.1** |


### :mag_right: Facade Semantic Segmentation Results at LoFG2

LoFG stands for Level of Facade Generalization. See more in the ZAHA paper introducing the concept [here, pending](pending).

|  | PointNet      | PointNet++ | Point Transformer | DGCNN         |
|-----------------|---------------|------------|-------------------|---------------|
| OA              | 71.9          | 75.5       | 78.2              | **82.6** |
| P          | 69.6          | 73.0       | 75.8              | **80.0** |
| R          | 68.1          | 73.0       | 76.6              | **81.8** |
| F1         | 68.1          | 72.6       | 76.1              | **80.4** |
| IoU        | 55.8          | 59.8       | 63.9              | **68.5** |
| **Class scores**            | |           |        |               |  
| floor           | **92.3** | 87.6       | 90.7              | 92.1          |
| decoration      | 26.2          | 47.1       | 47.0              | **70.0** |
| structural      | 60.9          | 65.5       | 67.0              | **85.2** |
| opening         | 28.2          | 27.2       | 36.0              | **66.2** |
| other el.       | 71.2          | 71.6       | 78.9              | **88.8** |



## :mortar_board: Publication

Please find the official publication introducing "ZAHA" at the WACV '25 here: 

The paper [[WACV25 - pending](pending)] [[arxiv preprint](https://arxiv.org/abs/2411.04865)]

and consider citing it:
```plain
@article{wysockietalZAHA,
	author = {Wysocki, O. and Tan, Y. and Froech, T. and Xia, Y. and Wysocki, M. and Hoegner, L. and Cremers, D. and Holst Ch.},
	title = {ZAHA: Introducing the Level of Facade Generalization and the Large-Scale Point Cloud Facade Semantic Segmentation Benchmark Dataset},
	booktitle = {Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)},
	year = {2025},
```
```
@misc{wysocki2024zahaintroducinglevelfacade,
      title={ZAHA: Introducing the Level of Facade Generalization and the Large-Scale Point Cloud Facade Semantic Segmentation Benchmark Dataset}, 
      author={Olaf Wysocki and Yue Tan and Thomas Froech and Yan Xia and Magdalena Wysocki and Ludwig Hoegner and Daniel Cremers and Christoph Holst},
      year={2024},
      eprint={2411.04865},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2411.04865}, 
}
```

## :handshake: Acknowledgments 

This work wouldn't be possible without [Zhu et al.](https://doi.org/10.3390/rs12111875) and their excellent [TUM-MLS-2016 dataset](https://www.pf.bgu.tum.de/pub/testdaten.html). Thank you!    
We are indebted to [Jiarui Zhang](https://de.linkedin.com/in/jiarui-zhang-20bb3618b), [Yue Tan](https://de.linkedin.com/in/yue-tan-98967b204/en?trk=people-guest_people_search-card), Chenkun Zhang, and [Prabin Gyawali](https://np.linkedin.com/in/pgyawali) for their diligent work in the annotation process. 
Thank you Hitachi group for releasing the [Semantic Segmentation Editor](https://github.com/Hitachi-Automotive-And-Industry-Lab/semantic-segmentation-editor) as a user-friendly open-source tool that we could easily adapt to our needs. 

Feel free to check out other facade semantic segmentation datasets, like the one devoted to cultural heritage of [Matrone et al.](https://doi.org/10.5194/isprs-archives-XLIII-B2-2020-1419-2020) and the inspiring [ArCH dataset](http://archdataset.polito.it/)! Go ahead, check it out, and test your algorithms there too!
