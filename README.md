# :cityscape: ZAHA :cityscape:

**To date the largest benchmark for facade semantic segmentation of point clouds** 

<p align="center">
    <img src="https://github.com/OloOcki/tum-facade/blob/main/img/bldImg/overview.PNG" width="95%" title="overview"/>
</p>

## :star2: Highlights
- **601 mln** annotated points
- Introducing LoFG: Level of Facade Generalization enabling hierarchical understanding of facades
- Various architectural styles
- In **local** and **global** (i.e., UTM) coordinate reference system (if struggling with the [height transformation](https://www.ldbv.bayern.de/vermessung/utm_umstellung/koordinatentrafo.html) - apply 45.66 m vertical offset)
- File names point to the official CityGML LoD2 building models of Bavaria (e.g., DEBY_LOD2_4959462 -> gml_id=DEBY_LOD2_4959462) [[visualisation](https://www.virtualcitymap.de/?lang=de&layerToActivate=%5B%22Bayern%20-%20LOD2%20(pbr)%22%2C%22Sachsen%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Sachsen-Anhalt%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Th%C3%BCringen%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Niedersachsen%20(pbr%20recalculation)%22%2C%22NRW%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Hessen%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Hamburg%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Brandenburg%20-%20LOD2%20(pbr%20recalculation)%22%2C%22Berlin%20untexturiert%20openData%20(pbr%20recalculation)%22%2C%22GermanyBaseTerrain%22%5D&layerToDeactivate=%5B%22Mesh%20Classification%20Layer%22%2C%22mesh_surface%22%5D&startingmap=Cesium%20Map&cameraPosition=11.56952%2C48.14564%2C875.76828&groundPosition=11.56721%2C48.14877%2C523.42063&distance=524.27&pitch=-42.23&heading=333.69&roll=359.89#/)]   
- The settings file for **adding your own data**


## :mortar_board: Publications

Please find the official publication introducing "ZAHA" at the WACV '25 here: 

The paper [[WACV25](pending)] [[arxiv preprint](pending)]

and consider citing it:
```plain
@article{wysockietalZAHA,
	author = {Wysocki, O. and Tan, Y. and Froech, T. and Xia, Y. and Wysocki, M. and Hoegner, L. and Cremers, D. and Holst Ch.},
	title = {ZAHA: Introducing the Level of Facade Generalization and the Large-Scale Point Cloud Facade Semantic Segmentation Benchmark Dataset},
	booktitle = {Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)},
	year = {2025},
```
