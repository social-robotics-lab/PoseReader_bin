# PoseReader_bin

This is a binary of PoseReader.
Sota(CommU)のポーズを簡単に試すためのツールです。Sotaの中で使用します。

# Install
Run the following commands in Sota.
```
git clone https://github.com/social-robotics-lab/PoseReader_bin.git
cd PoseReader_bin
mkdir PoseReader_lib
cd PoseReader_lib
git clone https://github.com/vstoneofficial/SotaSample.git
cp SotaSample/lib/* .
rm -rf SotaSample/
wget https://repo1.maven.org/maven2/com/google/code/gson/gson/2.8.5/gson-2.8.5.jar
wget https://repo1.maven.org/maven2/org/json/json/20180813/json-20180813.jar
```

# Run
```
cd PoseReader_bin
java -jar PoseReader.jar
```

# 使い方
下のコマンドを入力します。

```
java -jar PoseReader.jar
```

初期位置に戻った後、サーボが抜けますので、好きなポーズを取らせます。

- pを入力すると、その時の軸の角度が出力されます。
- +を入力すると、その時の軸の角度が記録されます。ポーズを取らせて+でどんどん記録していきます。
- rを入力すると、記録したポーズの系列を再生します。
- -を入力すると、記録した最後の動作を削除します。


イイ感じのポーズの系列（ジェスチャ）ができたら、ターミナルの画面をコピペして自分のプログラムで使ってください。
