# 分析目的

- testデータのsession(個人)ごとに，次のアクションを予測する
  - 途中までのアクションはテストデータに含まれている
- 各アクションに対して最大20個まで予測が可能

|session_type|labels|
|-|-|
|01_clicks|11111|
|01_carts|11111|
|01_orders|11111|
|02_clicks|11111,22222,33333,44444|
|02_carts|11111,22222,33333,44444|
|02_orders|11111,22222,33333,44444|

$R_{score}=0.10R_{clicks}+0.30R_{carts}+0.60R_{orders}$

- 詳細はhttps://www.kaggle.com/competitions/otto-recommender-system/overview/evaluation を参照
- 予測した候補の中から当たっている割合が$R_{type}$に代入される．
