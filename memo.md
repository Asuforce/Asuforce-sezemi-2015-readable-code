##仕様3
### 実際のコード

https://github.com/Asuforce/Asuforce-sezemi-2015-readable-code/commit/9169466e20a73c4f819e578f2dd561dbab42a979

```php
// ファイルを読み込んで出力
if (($file = fopen ( "code/recipe-data.txt", "r" ))) {
    // 読み込み成功時
    while (!feof($file)) {
        echo fgets($file, 1024);
    }
} else {
    // 読み込み失敗時
    echo "読み取り失敗";
}

fclose($file);
```

### どうしてリーダブルだと思っているかの説明
成功時を先に読むことで、流れが理解しやすいと思いました。  
またコメントを付与して何を実行してるのかを記述するようにしました。  

### この書き方の一言説明
条件分岐の整理

