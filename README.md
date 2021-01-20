# SEProject

## 概要
### 音イベントの認識(4種類のモデルに対応)<br>
・ SVM(SVM.ipynb)<br>
・ XGBoost(XGBoost.ipynb)<br>
・ LightGBM(LightGBM.ipynb)<br>
・ CatBoost(Catboost.ipynb)<br>
### その他の処理<br>
・ 音声の合計再生時間のカウント(Count.ipynb)<br>
・ セルの出力削除(logclean.ipynb)<br>

※ モデルの学習には自前の学習データを用意する必要があります<br>
学習は同じディレクトリ内のtrainとtestから音声データを取得して行っています<br>
予めラベルごとにディレクトリを分け、そのディレクトリ内に音声データを入れるようにしてください<br>

~~~
.
├── Catboost.ipynb
├── Count.ipynb
├── LightGBM.ipynb
├── SVM.ipynb
├── XGBoost.ipynb
├── logclean.ipynb
├── test
│   ├── label1
│   ├── label2
│         ...
│   └── labeln
└── train
    ├── label1
    ├── label2
          ...
    └── labeln
~~~
## 実行環境
### pythonのバージョン
python3.6
### 使用したライブラリ
numpy1.18.1 <br>
sklearn0.23.1 <br>
xgboost 1.1.1 <br>
lightgbm 2.3.0 <br>
catboost 0.24 <br>
optuna2.2.0 <br>
pandas0.25.1 <br>
librosa0.7.2 <br>
pathlib2.3.5 <br>
