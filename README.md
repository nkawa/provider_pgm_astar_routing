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
