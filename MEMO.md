# 学習メモ

## 12/14(木)
### Firebase Hosting + Vue Todoアプリのプロジェクト作成
- 環境構築
  - Vueアプリの作成
  - Firebaseへのデプロイ

## 12/15(金)
- install bootstrap vue
- import BootstrapVue
- create page folder,index.vue
- eslintの設定
  - index.vueのエラー設定
    https://qiita.com/chomado/items/9a86d3bca24dcd15a460
  - index.jsのエラー設定
    ``
    /*eslint linebreak-style: ["error", "windows"]*/
    var:a = 'a', // \r\n
    b : 'b', // \r\n
    // \r\n
    function:foo(params), // \r\n
      // do stuff \r\n
      // \r\n
    ``
    参考：https://eslint.org/docs/latest/rules/linebreak-style

## 12/18(月)
- eslintの設定
 - エラーが発生し続けていたため、ESLint ルールを無効にする
  ``` 'linebreak-style': 'off' ```

## 12/19(火)
- eslintの設定
  - 過去の研修資料を参考に設定
    https://visualresearch.sharepoint.com/:u:/s/development2/EaiTTOUhrd5ChBfaBLyMgEABY7dsNmgOb60pB9usM-1kdw?e=30OkxW
  - importエラーを解除するため、下記を追加
    ```
    "parserOptions": {
    "sourceType": "module"
    }
    ```
  - 原因がESlintの設定ではなく、ファイル名の大文字・小文字設定ミスのため、ESlintの設定を初期に戻し、微調整
- ロゴの削除
- TodoFormコンポーネントの作成
- TodoFormコンポーネントの読み込み
- ボタン装飾の変更
- データバインディングの設定
- clickイベントの追加
- データプロパティの追加
- メソッドの追加
- メソッドの呼び出し
- リストコンポーネントの作成
- コンポーネントの読み込み
- cssの微調整
- リストの動的表示

## 12/20(水)
- リストを逆順（新しい順）に表示させる

## 12/22(金)
- 削除機能の追加

## 12/25(月)
- ステータスの変更処理を追加

## 1/9(火)
- ステータスの変更処理を追加
- 完了時に取り消し線を追加

## 1/10(水)
- inputにテキストが残っているので初期化

## 1/11(木)
- firebase-toolsのアップデート
- vueアプリケーションのビルド
- firebaseにデプロイ