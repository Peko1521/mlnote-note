# mlnote-note

機械学習の教材である[機械学習帳](https://chokkan.github.io/mlnote/index.html)を学ぶノートです。確認問題を自分で解くときは「確認問題回答用」、回答を参照するときは「確認問題解答例」を開いてください。


| 講義 | 確認問題回答用Notebook | 確認問題解答例Notebook |
|----|---------------|---------------|
| [1.単回帰](https://studiolab.sagemaker.aws/import/github/chokkan/mlnote/blob/main/regression/01sra.ipynb) | [![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter1.ipynb) |[![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter1_answer.ipynb) |
| [2.重回帰](https://studiolab.sagemaker.aws/import/github/chokkan/mlnote/blob/main/regression/02mra.ipynb) |[![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter2.ipynb) |[![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter2_answer.ipynb) |
| [3.モデル選択と正則化](https://studiolab.sagemaker.aws/import/github/chokkan/mlnote/blob/main/regression/03regularization.ipynb) |[![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter3.ipynb) |[![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter3_answer.ipynb) |
| [4.勾配法によるパラメータ推定](https://studiolab.sagemaker.aws/import/github/chokkan/mlnote/blob/main/regression/04sgd.ipynb) |[![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter4.ipynb) |[![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter4_answer.ipynb) |
| [5. 線形二値分類](https://studiolab.sagemaker.aws/import/github/chokkan/mlnote/blob/main/classification/01binary.ipynb) |[![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter5.ipynb) |[![Open in SageMaker Studio Lab](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/icoxfog417/mlnote-note/blob/main/notebooks/chapter5_answer.ipynb) |
| [6. 線形多クラス分類](https://studiolab.sagemaker.aws/import/github/chokkan/mlnote/blob/main/classification/02multi.ipynb) |Comming Soon |Comming Soon |


Open Studio Labのボタンを押すとAmazon SageMaker Studio LabでJupyter Notebookを開けます。開くだけならアカウントは不要です。Notebook実行時にアカウントが必要です。AWSアカウント/費用は必要ありません。アカウントのリクエストは[Request Account](https://bit.ly/3sB7nC3)より、利用方法の詳細は下記をご参照ください。


## Notebookの実行

Notebookを実行するには、依存ライブラリのインストールが必要です。

### Amazon SageMaker Studio Lab

Amazon SageMaker Studio Labはメールアドレスのみで利用できるJupyterLab環境です。[使い方は"Amazon SageMaker Studio Lab の使い方"を参照してください](https://github.com/aws-studiolab-jp/awesome-studio-lab-jp/blob/main/README_usage.md)。

次の手順に沿いボタン/メニューを押していくことで環境構築ができます。一度作成した環境は保存されるため、⑦以外の手順は最初の1回のみでOKです。

![install_flow](./images/install_flow.PNG)

⑥のカーネルの登録は次のコマンドで行います。このコマンドを実行すると、Notebookを開いたとき右上のボタンから`mlnote`のKernelが選択できるようになります。作成したKernelを選択していないとライブラリが足りないよ～というメッセージが出るので注意してください。

```
conda activate mlnote
ipython kernel install --user --name mlnote
```

### ローカル環境

上記の④の代わりにターミナルから`conda env create --file environment.yml`を実行してください。以後の手順は同じです。
