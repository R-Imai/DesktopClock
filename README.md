# DesktopClock

## 準備
```
git clone https://github.com/R-Imai/DesktopClock.git
cd DesktopClock
npm install --save-dev electron
npm install --save-dev electron-packager
```

## 画像などの設定
### 時計内の画像
時計の中の画像を変更する場合は，`img/` に `DefaultLogo.png` という名前で配置すればOK．<br>
ファイル名が別の場合は`index.html` の10行目の
```html
<img id="ClockImg" src="./img/DefaultLogo.png" width="235" height="75">
```
のsrcのところを変えればOK<br>

### 時計の色
`clock.css` の16行目の

```
color: #ffffff;
```
を変えればOK

### アイコン
パッケージングの際のアイコンを変える場合は，`img/` に `DefaultIcon.ico` という名前で配置すればOK．(windowsの場合)<br>
ファイル名が別の場合は`package.json` の20行目
```json
"iconPath": "./img/DefaultIcon.ico"
```
を変えればOK


## 実行方法
```
npm run start
```


## パッケージ化方法
```
npm run build
```

---

### フォントファイル
http://www.bvfonts.com/fonts/details.php?id=18
