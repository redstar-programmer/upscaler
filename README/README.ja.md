# redstar upscaler
FFmpeg、Real-ESRGAN、Flowframesを使用した強力なビデオアップスケーリングツール - **多言語UI**に対応しました！

🌐 言語：
英語](README.en.md) | [韓国語](README.md) | [日本語](README.ja.md) | [中文](README.zh.md) | [フランス語](README.fr)
[フランス語](README.fr.md) | [ドイツ語](README.de.md) | [スペイン語](README.es.md) | [ポルトガル語](README.pt.md)
[Русский](README.ru.md) | [イタリア語](README.it.md) | [ベトナム語](README.vi.md) | [インドネシア語](README.id.md)
[日本語](README.th.md) | [日本語](README.ar.md)

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="center">
  <strong>ffmpeg、realesrgan、flowframesベースの動画アップスケーリングツール</strong><br><br></strong><br></br
  <em>最新のGUIベース、プリセット設定、マルチファイル処理をサポート</em></em></p></p
</p>

</p> <em> </em> </p> <em> </em> </p> <em

ダウンロード : [Release](https://github.com/redstar-programmer/upscaler/releases/)

## ✨ redstar' upscalerを後援してください。

このプロジェクトが気に入ったか、開発を応援したいですか？
小さなご支援でより良い機能と安定的なアップデートを手伝ってください！

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**GitHub Sponsors** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)


> 💡サーバー費用、開発時間、コーヒー一杯の後援が大きな力になります。ありがとうございます！

## Table of Contents

- [👋紹介](#紹介)
- [💾 インストールと準備事項](#インストールと準備事項)
- [🔧 主な機能](#主な機能)
- [🚀使用方法(Quick Start)](#使用方法-quick-start)
- ⚙️ 詳細機能説明](#詳細機能説明)(#詳細機能説明)
- 🙏 感謝の言葉](#感謝の言葉)
- [📜歴史](#history)

## 👋 はじめに
**redstar upscaler** は `ffmpeg`, `Real-ESRGAN`, `Flowframes` を利用して動画を自動的に高解像度にアップスケーリングするPythonベースのGUIツールです。

- 映像フレームの抽出→アップスケーリング→映像のマージまで一挙に処理
- 様々なrealesrganモデルをサポート
- Flowframesによる補間(Optional)
- オーディオコーデックの自動抽出及び処理
- 元の位置または指定経路で作業可能

> ⚠️ Windows環境で開発・テストされました。

以下は、簡単な使用デモ画面で、クリックするとYouTubeに移動します。
[![デモ映像を見る](https://img.youtube.com/vi/G-JTWRws3co/0.jpg)](https://youtu.be/G-JTWRws3co"YouTubeで見る")

## 💾 インストールと準備事項

1.次の外部ツールのインストールおよび位置確認(ただし、配布ファイルにffmpeg、Real-ESRGANおよびFlowframesのインストールファイルが含まれている(パス内のProgramsフォルダ参照))
   - ffmpeg](https://www.ffmpeg.org/download.html)
   - Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - [Flowframes](https://github.com/n00mkrad/flowframes) *(選択)*(選択)*)
2.解凍後、readstar's upscaler.exeを実行します。
3.Flowframesの場合、ユーザー環境によってロードされるモデルが異なる場合がありますので、必ずFlowframesを実行した後、<br>InterpolationタブのInterpolation AIとAI Modelがredstar upscalerのresources/flowframes_models.iniのバージョンと一致する必要があります。 <br>ロードされていないモデルは、＃マークを付けてコメント処理し、必ずredstar upscalerの設定ウィンドウのモデル順序が<br>Flowframesのモデル順序と一致することを確認して作業を進めてください。

## 🔧 主な機能

![Image](https://github.com/user-attachments/assets/93dc232e-8742-4ae3-b335-9395c26a61f4)
- ✅ 映像の複数選択及び順次作業
- ✅ 映像のドラッグ/ドロップ追加
- ✅ 主なプログラムの実行可否及び直接選択
- ✅ ディスク節約モード
- ✅ 多言語サポート(15ヶ国語)
<br><br><br><br></br
![Image](https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-484146dc6757)
- ✅ プリセットの保存と自動適用
- ✅ オーディオコーデックの自動検出とビットレートの自動設定
- ✅ realesrganモデルの自動検出と選択
- FFMPEG, real-ESRGAN, Flowframes詳細設定
- ✅ Flowframesのバージョンによるオプション設定変更<br>(バージョン変更は、メインページのflowframesで該当バージョンのパスを指定すると変更可能)
<br><br><br><br><br><br><br></br
![Image](https://github.com/user-attachments/assets/25d60d82-53a2-4064-bbef-d439d9a9d3d6)
- アップスケール実行コマンドの確認(cmd上で別途コピーして実行することができます)
<br><br><br>アップスケール
![Image](https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc84c769f0)
- ✅ アップスケール作業の全体的な進行状況のモニタリング
- ✅ アップスケールロギング確認(ログファイルは実生フォルダ内のlogフォルダに日付で生成)
- ✅ 作業完了後、結果物の自動整理(接頭辞[REDSTAR]を付与)
- ✅ 作業完了後の動作設定可能<br>( 何もしない / プログラム終了 / スリープモード / ハイバネートモード / ウィンドウ終了)
<br><br><br><br><br><br><br><br>>
## 🚀 使用方法 (Quick Start)

1.映像ファイルを追加(MP4、MKV、AVI、MOV、MOV、FLV、WMV、MPG、WEBM、3GP、OGVをサポート)
2.作業場所の指定または"元のファイルパスを使用"をチェックします。
3.追加された映像で"設定"ボタンをクリックします。
4.ffmpeg、realESRGAN、Flowframesの詳細設定を設定します。
5.全ファイルに一括適用/選択したファイルのみ適用をクリックします。
6.作業確認ボタンをクリック
7.実行するコマンドを確認後、作業開始ボタンをクリックします。

> 作業結果は、アップスケールされた映像とフレーム補間された映像ファイル二つが選択したフォルダに生成されます。
> 作業が完了したファイルは接頭辞[REDSTAR]を付けたファイル名で保存されます。
---ファイル名[REDSTAR]。

## ⚙️ 詳細機能説明

| 項目｜項目｜説明｜説明
|------|------|
| **作業パス設定** | デフォルトの指定パスまたは"元のファイルパスを使用"オプションを提供します。
| 動画フォーマットサポート**｜MP4、MKV、AVI、MOV、MOV、FLV、WMV、WMV、MPG、WEBM、3GP、OGVなどほとんどのフォーマットをサポートします。
**アップスケールモデル** | realesr-animevideov3、realesr-general、4xplusなどの自動検出｜ | **アップスケールモデル** | ``オーディオ処理**''
| **オーディオ処理** | `aac`, `mp3`, `flac` など様々なフォーマットのエンコーディングをサポートします。
| **Flowframes 連動** | 補間(FPS ×2、×4、×8)設定可能｜｜ **ディスクセーバーモード
| ディスクセービングモード**｜｜中間画像自動削除機能を提供｜ | **ディスクセービングモード**｜｜。

## 🙏 感謝の言葉

- realesrgan by [xinntao](https://github.com/xinntao/Real-ESRGAN)。
- flowframes by [n00mkrad](https://github.com/n00mkrad/flowframes)
- このプロジェクトに参加したり、機能を提案したい場合は、[Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues)にコメントを残してください。

# 📜 History

v 1.1.0
 > 1.メニュー構成(ファイルを開く、閉じる、ログ設定、言語設定)
 > 2.多言語設定の追加（使用可能言語：韓国語、English、日本語、日本語、中文、Français、Deutsch、Español、Portuguese、Portuguese、Русский、T Tiếng Việt、Bahasa Indonesia、ไทย、Italiano、العربية)
 > 3.言語設定追加に伴うメッセージおよび一部のコード変更
 > 4.一部UI構成の変更
 > 5. ffmpeg、real-ESRGAN、Flowframesの各バージョン情報表示(メイン画面)
 > 6. Flowframes 1.41.0バージョン対応(現在1.41.0バージョンにcmdコマンドの問題があり、1.40.0, 1.36.0バージョンのみ使用可能)
 > 7. AI Modelsの項目が小文字で表示される問題を解決しました。
 > 8.FFMPEGオプション追加(Pixel, video codec) - ユーザーPCに合ったオプションが表示されます。
 > 9.ユーザーPC別CUDAチェック強化 - 使用可能かどうか及びGPU種類確認可能(メイン画面)

v 1.0.0
 > 1.全体のコード再作成
 > 2.UIの変更
 > 3.処理可能な映像/オーディオ範囲の増加
 > 4.ディスク節約モード追加
 > 5.主要プログラムを含む配布

v 0.1.92
 > 1.Flowframesパス変更時、AIモデルコンボボックスに重複して入力され、補間が失敗する問題を解決しました。
 > 2.補間作業時、コンボボックスの選択状態を確認するコード追加

v 0.1.91
 > 1.Flowframes関連の一部combobox refresh機能を追加しました。
 > 2.配布ファイルの一部調整

v 0.1.9
 > 1.Flowframesモデル変更適用
 > 2. Flowframes 1.36.0新規モデル、1.40.0モデルを実装しました。
 > 3.Flowframesのコマンドライン失敗が発生しなくなりました。
 > 4.ドラッグ/ドロップでファイルを追加できるようになりました。
 > 5.Flowframesの設定値が適用されない問題を解決しました。

v 0.1.8
 > 1.バージョンチェック時、新規バージョン確認エラーの修正
 > 2.flowframesが基本パス(ex.C:\Users\Administrator\AppData\Local\Flowframes\)にインストールされている場合、そのパスをデフォルトに設定した後、起動するように変更
 > 3.複数のファイルを選択し追加すると、エラーで強制終了する問題。
 > 4.複数のファイルを追加した後、作業開始時にエラーが発生する問題を修正しました。

v 0.1.7
 > 1.プログラムサイズ変更可能
 > 2.音声がないファイル作業時にエラーが発生する問題を解決しました。
 > 3.全体のUI構成を変更(サイズ変更に合わせて再設定)。

v 0.1.6
 > 1.画面解像度によって文字サイズが異なる問題を解決しました。
 > 2.プログラムタイトルにバージョン情報が新しいバージョンで表示されない問題を解決しました。
 > 3.config.iniファイルが別のパスに保存される問題を解決しました。
 > 4. realesrganのアップスケーリング倍数を変更する場合、アップスケーリングモデルコンボボックスも一緒に変更
 > 5.アップデートチェック機能追加
 > 6.一部のロジック修正
 > 7.解像度とfpsなどテーブルの表記色を変更
 > 8.解像度(元)ユーザー修正可能(必ず1024x768の形で入力する必要があります)

v 0.1.5
 > 1.flowframes補間ai選択時、aiモデルが自動変更されない問題を解決しました。
 > 2.flowframes補間時、選択されたオプション通りに補間されない問題を解決しました。
 > 3.一部の動画のFPS計算時、誤ったFPSで計算される場合を防止するために「FPS計算方式」コンボボックスを追加
        -> r_frame_rate / avg_frame_rate の中から選択可能で、基本は r_frame_rate で計算します。
 > 4.動画ファイルを選択した時、動画情報のインポートの進行状況を表記
 > 5.ファイルを開いた後、再度ファイルを選択すると、最後に選択したフォルダをデフォルトで開くように変更

v 0.1.4
 > 1.config.iniファイルの読み取り方式変更
 > 2.動画情報の取得方法をPython AVからffmpegに変更。
 > 3.タスク終了時、ウィンドウ終了機能を追加。
 > 4.タスクリストでマウスオーバー時、ファイル名全体をツールチップとして表示
 > 5.タスクリストに各ファイルの解像度(前) / 解像度(後) / FPS(前) / FPS(後)を表記する。
 > 6.FPS入力ボックスを削除(上記の各ファイル別表記による削除)
 > 7.出力FPS予想サイズを削除(上記の各ファイル別表記による削除)
 > 8.進行状況を全体ファイル/作業別二つのProgressbarで表記する

v 0.1.3
 > 1.ファイル読み込み時、一部のFPS情報が間違っていたファイルFPS計算エラーを修正

v 0.1.2
 > 1.UI設定変更
 > 2.内部ロジック変更
 > 3. realesrganモデルのうち、以下の2つのモデルを選択すると実行されない問題を解決しました。
 > 4. realesrganモデルの使用方法変更
 > -> realesrganインストールフォルダ内のmodelsフォルダに新規モデルファイル(*.param)をコピーすると使用可能です。
 > 5.作業対象映像の最後のファイルのwidth、height情報と予想アップスケールサイズを表示します。
 > 6.config.iniファイルの移行コードを作成します。
 > 7.ffmpeg分解画像のaac -> flacに変更
 > 8.その他のバグ修正

v 0.1.1
 > 1.初回作成、ffmepg、realesrgan、flowframesを連動させた動画アップスケーリングプログラムの作成