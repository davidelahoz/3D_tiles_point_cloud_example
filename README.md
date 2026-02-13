# 3D_tiles_point_cloud_example
Example Cesium 3D tiles point cloud for testing Cesium plugins for different game engines

The point cloud in laz format was obtained from [IGN](https://centrodedescargas.cnig.es/CentroDescargas/lidar-tercera-cobertura) and was processed using the following programs:
1. laszip (which is part of [lastools](https://lastools.github.io/)) to convert it to an uncompressed las file
2. [py3dtiles](https://py3dtiles.org/) to generate the Cesium 3D tiles files from the las file

Commands used:
´´´
laszip64 -i ./pointcloud.laz -o ./pointcloud.las
py3dtiles convert ./pointclod.las --out ./3DTiles
´´´
