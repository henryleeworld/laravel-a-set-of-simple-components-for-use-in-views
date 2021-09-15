# Laravel 8 一組用於視圖的簡單元件

引入 cagilo 的 cagilo 套件來擴增一組用於視圖的簡單元件，視圖包含應用程式用到的 HTML，它能夠將呈現邏輯從控制器和應用程式邏輯分離出來。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 執行 __Artisan__ 指令的 __migrate__ 來執行所有未完成的遷移，並執行資料庫填充（如果要測試的話）。
```sh
$ php artisan migrate --seed
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以登入經由 `/` 來進入歡迎頁面。

----

## 畫面截圖
![](https://i.imgur.com/rZz62XF.png)
> 儘管所有元件都是開箱即用的，但出於效能原因，可能只需載入應用程式中所需的元件
