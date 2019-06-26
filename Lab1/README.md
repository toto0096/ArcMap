## Vector Data Model
  - 기본적으로 필요한 두 가지 데이터
    - Points, Lines, Polygons의 공간사상을 나타낼 좌표체계 필요
    - 디지털 파일의 Geometric objects와 Spatial relationships 필요
  - 특징
    - 고해상도
    - Discrete obfects(이산적인, 별개의, 비연속적인 객체)에 적합
    - 래스터 자료보다 소용량
    - 복잡한 데이터구조
  - Representation of Simple Features
  
      ![1](https://user-images.githubusercontent.com/47414872/60159173-93ac3e80-982d-11e9-8ce6-3c1b0381cb53.PNG)
    - Point : 0차원, 위치 속성을 가짐(Node, Vertex)
    - Line : 1차원, 길이 속성을 가짐(Edge, Link, Chain)
    - Area : 2차원, 지역 및 둘레의 속성을 가짐(Polygon, Face, Zone)
    
## Raster Data Model
  - 특징
    - 래스터 데이터 모델은 공간을 커버하는 규칙적인 격자를 사용
    - 각각의 격자 셀의 값은 셀 위치에 공간적 현상의 특성과 대응
    - 셀 값의 변화는 사상(feature)의 공간적 변화를 반영
    - GIS에 사용되는 다양한 데이터를 래스터 형식으로 인코딩 가능
    - 래스터 데이터는 많은 컴퓨터 메모리를 요구하기 때문에 저장 및 검색의 문제가 중요
  - Elements of the Raster Data Model
    - Row(행) : y-coordinates
    - Columns(열) : x-coordinates
    - Cell Value : 래스터 각 셀의 행과 열이 나타내는 위치의 공간적 현상을 나타냄(integer, floating-point)
    - Cell Size : 래스터 데이터 모델의 해상도를 결정 (ex. 10m*10m)
    - Raster Bands : Single Band, Multiple bands
    - Spatial Reference : 다른 GIS 데이터 셋과 공간적으로 맞추기 위해서 래스터 데이터는 공간 참조 정보가 있어야 함(Map Projection, Geo-referenced Raster)
  -Types of Raster Data
    - Satellite Imagery (위성 영상)
      ![2](https://user-images.githubusercontent.com/47414872/60161278-2ea71780-9832-11e9-9a2f-a6d2d85c8884.PNG)
