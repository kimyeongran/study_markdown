## 公開方法をコントロールする
  | 項目名 | 設定内容　|
  |---|---|
  | 公開状態 | 公開、非公開、パスワード変更 |
  | 公開　| 予約日時の指定、日時の変更　|
  | 先頭に固定設定 |（投稿のみ）|
  | レビュー待ち |（投稿のみ）|
  | 投稿者 |（投稿者名）|

---
  - 公開済みの記事を下書きに戻す
      - 下書き切り替え
      - 確認のダイアログでokボタンクリック
      - 保存しました表示の後、下書き保存表示に戻る
  - パスワードを設定して閲覧対象を制限する
      - 投稿の編集画面
      - 公開状態の公開→パスワード保護→パスワード入力→更新
  - 投稿を非公開にする
      - 投稿の編集画面→公開

## ブロック
  - 静的ブロック：レイアウトの枠組みを設計（段落、画像など）
  - 動的ブロック：各ページの変化に応じて挿入される内容が変化するブロック（アーカイブ、最新の記事など）
  - 更新したブロックをさらに変更をする
      - 引用：段落、リスト、見出し、プルクオートに変更できる
        ★プルクオート：引用したテキストに背景色や文字色などの視覚的な強調を付けられるブロック
  - 画像/動画の上にテキストを重ねて配置する
      - パネル内のアイコンの位置は、使い方によって変化する
      - 直接このパネル内に直接ドラッグ＆ドロップしても登録できる
      - カバーブロックでは、テキストのスタイル以外にも、背景を固定するかどうか、オーバーレイの色、透過率などを設定できる
      - shift + enterキーを押すと改行できる
      
  - 同じデザインを複数の記事で使いたいときは、再利用ブロックを有効に活用する
    (大元の再利用ブロックと連携しているので、大元の再利用ブロックを編集すると記事内の再利用ブロックも一斉に更新できる）
    - 再利用ブロックを作成
    - 再利用ブロックを登録する（親のブロック）
    - 各ページに子の再利用ブロックを配置
    ★　再利用ブロックの周囲は点線でかこまれていて、通常のブロックとは異なる
        親の再利用ブロックは既存ブロックの中身を書き換えるだけでなく、ブロックの追加や削除ができる
        
## コードエディターでコードを確認
   1. ビジュアルエディター：ブロックの挿入、レイアウト全般
   2. コードエディター：HTMLコードの確認、HTMLの修正や削除
        - ブロックを制御するコメントタグ　（アーカイブ、カテゴリー、最新にコメント、最新の記事は終了タグがない）
        - 見出しブロックのコード：<!--wp:heading-->
        - 段落ブロックのコード：<!--wp:paragraph-->
        - 最新のブロックのコード：<!--wp:latest-posts-->
      
## 画像を挿入する
   - 事前に画像サイズを設定して手間を減らす
      1. サムネイルのサイズ：サムネイル（記事引用時に使う小さな画像）のサイズ
      2. 中サイズ：小さめの画像のサイズ
      3. 大サイズ：画面幅いっぱいに挿入される画像のサイズ
   - 不要な画像ファイルが自動生成されないようにする（０に設定しておく）
   - メディアライブラリでメディアを管理する
   - 代替テキストやキャプションを設定すると、以降同じ画像を別記事内に挿入する際に自動で気に継承され、  
     一つ一つ設定する必要ない  
        - メディアライブラリ指定：全記事に適用される  
        - ページ上で指定：その記事のみに適用される 
   - 挿入した画像を他のブロックに変更する
   
  | ブロック名 | 変更 |
  |---|---|
  | カバー | 画像を背景にしてテキストを重ねる。キャプション上側できストになる |
  | メディアと文章 | 段組みになる、画像が左に配置され、右側にできストを入力できるようになる |
  | ギャラリー | 複数の画像をタイル状に並べるギャラリーの１画像になる。画像を追加可能 |
  | ファイル | キャプションがファイル名になり、リンクをクリックすると、画像がダウンロードされる |
    
---

  - アイキャッチ画像を設定する　
    - 記事一覧やヘッダーなどに表示される小さな画像）
    - 本文を読まなくてもタイトルとアイキャッチ画像から内容を把握することができる
       
## 動画をファイル挿入する
   - yuotube　動画を挿入する：youtubeブロックでアップロード、埋め込みコードを取得して利用する
   - 動画を挿入する：動画ブロックで挿入（mp4, m4v, avi, wmv, movなど)　動画サイズはサーバーの設定によって決まる
   - 音声を挿入する：音声ブロックで設定（mp3, wav, m4a, aacなど）
   - googleマップを記事に挿入する：http://www.google.com/maps/
   - PDFを挿入する：ファイルブロックで挿入
















