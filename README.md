# provider_pgm_astar_routing
Calculate route from PGM file

PGM ファイルからルーティングを構成する

geojson ファイルから PGM ファイル、及び設定用のjson ファイルは
以下のツールで生成する。
（なお、 geojson ファイルは Polygon データで構成されていることを前提としている）
https://github.com/nkawa/geojson_tool

geojson_tool -file [geojsonファイル名] -width [画像幅] -json [Jsonファイル名] -pgm [PGMファイル名]

で、PGMファイルを生成する。

pgm_routing -file [config.json ファイル]


### 関連するソフトウェア
geojson_tool: GeoJson （Polygon)から、image, json を作成
- https://github.com/nkawa/geojson_tool.git

map から点を指定して送信: provider map-pick
- https://github.com/nkawa/provider_map_pick.git 

astar_golang: ル―ティングの基礎 (sample 以下に GUI 付でサンプルあり)
- https://github.com/nkawa/astar_golang.git



PGM ファイルの処理を行う（周囲の余分な部分を切り取る）
- https://github.com/nkawa/pgm_tool.git


