# マルチプラットフォーム対応のzmk-config-roba
- VSCodeで編集する
- Keymap EditorやZMK Studioは非対応
## デバイスごとの設定
### Ubuntu
- US配列  
- `ubuntu_` `alt_` `us_`で定義
- 無変換・変換でIME切り替え
### Windows
- 日本語配列  
  US配列だと無変換変換のキー設定がうまく行かないため。  
  PowerToysで無理やり`LANGUAGE_1` `LANGUAGE_2`を変換することは可能だが、外部ソフトをなるべく使わないように行いたいので、日本語配列にする。  
- `win_` `alt_` `jis_`で定義
- 無変換・変換でIME切り替え
### Mac
- 日本語配列  
  日本語配列のMacbookを使っているため。Karabiner_Elementsで切り替える手間を無くしたい。
- `mac_` `command_` `jis_`で定義
- 英数・かなでIME切り替え
### iPad
- 日本語配列  
Macと統一するため。
- `ipad_` `command_` `jis_`で定義
- 英数・かなでIME切り替え
## 日本語配列の適応の仕組み
- [【ZMK】OS設定を日本語キーボードのまま使う｜kloir-z](https://note.com/kloir_z/n/n314e739f03a1) を参考に設定
- `config/roBa_L.keymap`に変換定義を記述する。
## ショートカット
### Deepl
#### Windows, Ubuntu
- テキスト翻訳  
Ctrl + Windows(Super) + C
- 画面翻訳  
Ctrl + F8
#### Mac
- テキスト翻訳  
Command + Shift + c
- 画面翻訳  
Command + Shift 2
