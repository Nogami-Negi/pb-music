BGMファイルをバックアップするところです。

## BGMメモ
- 音質、サンプル値の取得はなるべく44100hzで（重要）
- 拡張子は.oggのみ（過去バージョンでは使えたwavやMP3は未対応）
- ファイル名の後に特定の記述を付け加えることでBGMの挙動を変えることができる
    - ループ：`__[ループ始点サンプル値]_[ループ終点サンプル値]` ※ループ終点以降はカット推奨？
    - ラストスパート加速なし：`__N`
    - ループ+ラストスパート加速なし：`__[ループ始点サンプル値]_[ループ終点サンプル値]_N`
### eng
- Sound quality and sample value acquisition must be performed at 44,100 Hz (important)
- Only the .ogg supported
- can alter the BGM behavior by appending a specific string to the filename
    - loop: `__[Loop Start Sample Value]_[Loop End Sample Value]` *It is recommended to cut after the end loop point
    - No Hurry-Up acceleration: `__N`
    - loop+No Hurry-Up acceleration：`__[Loop Start Sample Value]_[Loop End Sample Value]_N`
