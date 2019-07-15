# Sushi-go-Round

HTMLとCSSだけで寿司を回して食いたい！！！

## 使い方

dependenciesインストール
```
yarn
```
起動
```
yarn start
```

ビルド（production）
```
yarn build
```

HTMLは[Pug](https://pugjs.org/)、CSSは[Stylus](http://stylus-lang.com/)、ビルドには[Parcel](https://en.parceljs.org/)を使用しています。

## config.json

編集後は再起動してください。

### `neta`
```
"neta": {
  // 寿司ネタのキー
  "magro": {
    // 表示名
    "label": "neta label",
    // お値段（単位：¥）
    "price": 250,
    // ネタの色
    "bodyColor": "#f10707",
    // ネタの画像（ないときは上記の色を使う）
    "bodyImg": "path/to/img.png",
    // 皿の色
    "dishColor": "#8c7e2f",
    // 皿の画像（ないときは上記の色を使う）
    "dishImg: "path/to/img.png"
  },
  "shake": {...},
  "kohada": {...},
  ...
}
```

### `laneSushi`
```
// netaのキー名で指定
"laneSushi: ["magro", "shake", "kohada", ...]
```

### `lane`
```
"lane": {
  // 寿司レーン要素のwidth（単位：px）
  "width": 500,
  // 寿司レーン要素のheight（単位：px）
  "height": 250,
  // 寿司レーンの幅（単位：px）
  "size": 60,
  // 寿司レーン一周の所要時間（単位：s）
  "time": 12
}
```

### `sushiDish`
```
"sushiDish": {
  // 寿司要素のwidth（単位：px）
  "width": 60,
  // 寿司要素のheight（単位：px）
  "height": 45
},
```

### `sushiEater`
```
"sushiEater": {
  // 寿司食う人の要素のwidth（単位：px）
  "width": 150,
  // 寿司食う人の要素のheight（単位：px）
  "height": 200,
  // 待機中の画像
  "waitingImg": "path/to/img.png",
  // 寿司食い中の画像
  "eatingImg": "path/to/img.png",
  // 寿司すべて食べたときの画像
  "doneImg": "path/to/img.png"
}
```

## 画像について

イラストサイトの規約に抵触しそうだったので、このリポジトリに画像は含まれていません。ご了承ください。
