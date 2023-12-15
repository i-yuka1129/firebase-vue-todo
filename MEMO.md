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