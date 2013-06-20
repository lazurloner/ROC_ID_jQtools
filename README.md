## ROC ID jQtools 台灣身分證字號工具

### 關於本工具
  簡單的說，本工具是一個可以用於驗證與產生身分證字號的jQuery小工具。

### 本工具的特色
1. 身分證字號「去性別化」
  對於有些人來說，台灣身分證字號上的「性別辨識碼」，對他們有很大的困擾，這是一個需要推動刪除的東西。
  本工具的功能除了驗證台灣的既有身分證字號之外，最大的特色在於推動「去性別化身分證字號」，以達成推動性別平等之目的。目前國際間，會在身分證字號上面標明性別的國家其實已經不多，我們希望在不久的將來，台灣的身分證字號可以不再有性別。

2. 身分證字號「補完」
  您可以只輸入「部分」的身分證字號，程式將會使用公式產生後面的數字。
  例：你可以僅輸入「A012」,程式將會吐出「A012387360」這樣的有效格式。

### 功能及使用方式
1. 台灣身分證字號驗證
  * ROC_ID_check('ID_STRING_HERE','bool'); //可回傳True or False驗證結果.(bool可省略)
  * ROC_ID_check('ID_STRING_HERE','alert'); //直接跳出alert提示驗證結果.

2. 台灣身分證字號產生
  * ROC_ID_Generator(); //可回傳依據驗證公式產生的身分證字號(回傳字串)

3. 台灣身分證字號補完
  * ROC_ID_Generator('A012'); //可輸入部分身分證字號將後面字號補完(回傳字串)

### 常見Q&A
  Q.可以適用於目前的身分證字號（有性別的）格式嗎？
  
  A.當然可以，因為驗證公式原本就沒有考慮性別因素，而產生字號的部份，可以使用「補完」功能，帶入「英文數字+1」或「英文數字+2」的方式讓程式產生後面的數字。
  
  Q.如果產生的字號格式不是目前通用格式，意義何在？
  
  A.本專案對「既有」字號格式是完全相容，「去性別化」的意義是希望可以喚醒更多人對於「身分證字號去性別化」的注意。

### 授權方式
  本專案採用GPL授權，詳細內容請參考gpl.txt
