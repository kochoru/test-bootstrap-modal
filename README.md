# test-bootstrap-modal
IE11で、bootstrap v4.1.0を利用していると、`Object.keys: 引数はオブジェクトではありません`エラーが発生する件検証

# 原因
> ES5 では、このメソッドの引数がオブジェクトでない場合 (プリミティブ値)、TypeError が発生します。 ES2015 では、オブジェクトでない引数はオブジェクトに強制的に変換されます。

https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/Global_Objects/Object/keys#Notes

# 対応
bootstrap v4.1.1以上に上げると解決
