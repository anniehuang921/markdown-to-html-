# markdown-to-html-
to be more beautiful html
# 只要會 markdown 就能寫出漂亮網頁
![**Welcome** ](https://openclipart.org/image/200px/svg_to_png/233385/girlc.png)

## 有沒有那麼厲害！？
要先準備的東西

* markdown [簡易影片教學](https://www.youtube.com/playlist?list=PLDdZo0QJkJD8CxzUjAc_vTPQGP_ND_fj1)
* pandoc [連 command line 都手把手教學的善心官網](http://pandoc.org/)
* bootstrap [複製貼上 CDN](http://getbootstrap.com/getting-started/)

## 幾個重要的步驟和指令
|order|command|

|--|:--|

|1.製作 .md 檔|make a .md file , under pandoc-test folder|
|2.到 terminal 上|go to terminal|
|3. 執行轉換|$ pandoc test.md -f markdown -t html -s -o test.html|
|4. 加入 bootstrap CDN|add bootstrap CDN in header|
|5. 改成所需 class|add any class type you need |
|6. 開檔案|$ open test.html|

## 先把缺點講出來

**每一次轉檔後，就要重新添加 Bootstrap CDN 還有 class。**

#### checkbox 不行
- [ ] 或許可以
- [x] 或許不行

#### 數學符號可以，但有點醜

## $$ \int_a^b f(x) dx $$

### 一些常用的 class
表示法用 *class = [ ]*

* `<table class= "table table-striped table-bordered">`


## Bootstrap CDN code
```
<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css" integrity="sha384-1q8mTJOASx8j1Au+a5WDVnPi2lkFfwwEAa8hDDdjZlpLegxhjVME1fgjWPGmkzs7" crossorigin="anonymous">

<!-- Optional theme -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap-theme.min.css" integrity="sha384-fLW2N01lMqjakBkx3l/M9EahuwpSfeNvV63J5ezn3uZzapT0u7EYsXMjQV+0En5r" crossorigin="anonymous">

<!-- Latest compiled and minified JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js" integrity="sha384-0mSbJDEHialfmuBBQP6A4Qrprq5OVfW37PRR3j5ELqxss1yVqOtnepnHVP9aJ7xS" crossorigin="anonymous"></script>
```
