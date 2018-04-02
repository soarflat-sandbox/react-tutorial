# react-tutorial

## Overview

### What is React?
Reactは、ユーザーインターフェイスを構築するための、宣言的で効率的で柔軟なJavaScriptライブラリ。

Reactにはいくつかの異なる種類のコンポーネントがあるが、まずは`React.Component`サブクラスから始めてみる。

```js
class ShoppingList extends React.Component {
  render() {
    return (
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
    );
  }
}

// Example usage: <ShoppingList name="Mark" />
```

- ReactはXMLのようなタグをすぐに取得する。
- コンポーネントにレンダリングしたいものをリアクションするように指示する（`{this.props.name}`）。
- そしてReactは、データが変更（` <ShoppingList name="Mark" />`）されたときに、正しいコンポーネントだけを効率的に更新してレンダリングする。

上記の`ShoppingList`はReactコンポーネントクラス、またReactコンポーネントタイプという。コンポーネントは`props`と呼ばれるパラメータを取り込み、`render`メソッドを介して表示するビューの階層を返す。