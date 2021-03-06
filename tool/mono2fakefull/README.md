# mono2fakefull

モノラベルからなんちゃってフルラベルを生成するツール

## 用途

- NNSVSで話し声を学習してみたい。
- 話し声の音声で生成したacousticモデルを歌声用の土台にしたい。

## 仕様

### 生成されるコンテキスト

- 発声開始時刻と発声終了時刻
- 現在の音素の分類（p1）
- 現在や前後の音素記号（p2, p3, p4, p5, p6）
- 現在の音素の、音節内での位置（p12, p13）
- 現在の音素の、母音からの距離（p14, p15）※子音のみ
- 音節の、ノート内音素数（a1, b1, c1）
- 音節の、ノート内での位置（a2, a3, b2, b3, c2, c3）
- ノート内音節数（d6, e6, f6）
- ノートの、フレーズ内での位置（e18, e19）
- 曲中のフレーズ数（j3）