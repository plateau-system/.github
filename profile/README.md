## PLATEAU SYSTEM
PLATEAUを用いたシステムの研究・開発を行っています。  
[PLATEAU obj(公式)](https://www.geospatial.jp/ckan/dataset/plateau-tokyo23ku)
## 概要  
　本システムは「PLATEAUとYOLOv5を用いた定点観測及び人流シミュレータ」である。3D可視化エディタ(Unity)、Web管理システム(Laravel)、YOLOv5を動作させる専用サ－バー(YOLOv5,FastAPI)用いたシステム構成になっており、データベース(MySQL)に定期的な観測データを蓄積することができる。また情報の可視化に3D都市(PLATEAU)を使用することで、詳細なマップUIの開発やパラメータに変化によるシミュレータの開発等を行うことができる。
## 構成  
・[system-web(Laravel)](https://github.com/plateau-system/system-web/tree/main/src/app)：管理者用Webシステム。グラフ管理、パラメータ調整等。  
・[yolov5-fastapi(YOLOv5,FastAPI)](https://github.com/plateau-system/yolov5-fastapi)：YOLOv5とFastAPIを用いて検出結果を返すPythonのAPI。  
・[system-unity(Unity)](https://github.com/plateau-system/system-unity)：UnityとPLATEAUを用いたシミュレータ。webシステムと連携して情報を3D都市に可視化する。  
・[design](https://github.com/plateau-system/design)：設計資料の保管用リポジトリ。  
