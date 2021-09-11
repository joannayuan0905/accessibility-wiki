---
disqus: HackMD
---
###### tags: `規範` 

# [ 行動化無障礙指引 ] 
本文依據110-03-24國家通訊傳播委員會公告訂定「行動化應用軟體無障礙檢測指引」來做文章、程式碼整理，相關內容有放在參考資源中。

[TOC]

---
內容圖示定義

:books:特性、 :pushpin:檢測分類與指引、:bulb:注意、:warning:警告

---
## 背景說明

### 1-1 關於無障礙  

> 普遍錯誤觀念認為建置無障礙網站是為特殊人士而建置。
所謂「無障礙網站」是指在建置網站時考量到各類型使用者的需求，因此修正網站有可能會遇到的「障礙」，而不是為了「有障礙」的需求者去建置網站。

網路為資訊流通創造了無遠弗屆的可能，而人為因素卻可能設下進入的屏障與阻礙！例如：網頁上亦常見「本網站最佳瀏覽解析度為800*600，建議使用IE4.0以上版本瀏覽器」之標註，設定網頁最低限度的瀏覽解析度，以及某種版本以上的瀏覽器，將使一些電腦硬體較為低階、網路連線速率較慢，或舊版本、純文字瀏覽器的使用者，不得其門而入。

為顧及所有瀏覽網站的使用者在操作、瀏覽網站的親和性，就必須移除瀏覽網站時所會遇到的障礙，幫助更多使用者不需依靠他人即可獲取網站的資訊。 

每位使用者在操作無障礙網站時，所能使用到的設計只是或多或少，而無障礙的觀念拓展至網際網路是為了讓不同程度或需求的使用者可以順暢的獲取網站上的資訊。


---

### 1-2 哪些是無障礙網站呢？
「無障礙網站」就是使網站的使用性達到一定的標準，使網站的操作達到便利無障礙。目前有許多政府機關網站上已有這樣難能可貴的標章認可，用意是為了讓大家使用網路更順暢，利用網路的便利性促使大家在申辦各項業務之時，有一個簡單方便的管道，讓每個網路使用者都可方便且無障礙的操作網站，突顯網站的親和力，促使大家擁有一個無障礙的網路環境。而標章所設計的原由是依 [Accessibility（親和力）(另開新視窗)](http://dia.z6i.org/accessibility_statement.html "連結至親和力聲明")為主，使其規劃如下表等４種不同等級的無障礙網站標章：

---

### 1-3 優先等級
本規範為了讓網頁開發者和網頁使用者能夠對網頁的可及性設計有明確的評估方式和一致的認定準則，特參考WAI組織在相關無障礙網頁標準的設計，以三個優先等級來規範無障礙網頁的可及性設計。

![](https://i.imgur.com/xWvPtqp.png)

【第一優先等級】

網頁內容開發者在開發網頁時「**必須**」遵循這個等級的檢測碼。否則，某些使用者或團體將會發現不能使用網頁上的資訊。滿足此等級檢測碼對一些使用網頁文件的團體來說，是一種基本的需求。

檢測等級說明：符合本優先等級的網站可申請"A"等級標章，顯示已符合第一優先等級之無障礙設計規範。

【A+等級】

政府資訊網站若通過第一優先等級無障礙設計，且具有定位點(:::)（原名網頁導盲磚）搭配鍵盤快速鍵(Accesskey)、網站導覽(Sitemap)功能及網頁瀏覽工具具有使用鍵盤設計，勿只設計僅能使用滑鼠點選等三種便利使用者瀏覽網頁的功能。

檢測等級說明：符合本等級的網站可申請"A+"等級標章，顯示已符合第一優先及A+等級之無障礙設計規範。

【第二優先等級】

網頁內容開發者在開發網頁時「**應該**」滿足這個等級的檢測碼。
檢測等級說明：符合本優先等級的網站可申請"AA"等級標章，顯示已符合第一及第二優先等級之無障礙設計規範。

【第三優先等級】

網頁內容開發者在開發網頁時「**可以納入**」這個等級檢測碼的要求。
檢測等級說明：符合本優先等級的網站可申請"AAA"等級標章，顯示已符合第一、第二及第三優先等級之無障礙設計規範。

---

### 1-4 ACT格式說明

> 參照 全球資訊網協會(W3C)，於 2019 年 10 月 31 日公告「Accessibility Conformance Testing (ACT) Rules Format 1.0」(以下簡稱 ACT 規則)文件， 將各檢核點依此格式進行說明及編輯排版。

ACT 規則格式是說明如何針對無障礙要求的特定方面測試特定類型 的內容，旨在描述手動無障礙測試及無障礙測試工具執行的自動測試， 並記錄如何測試無障礙要求，將使無障礙測試和可重複的測試結果透明 化，測試案例也被編寫為 ACT 規則的一部分，以提供一種驗證規則的 實現能否成功確定預期結果的方法。

---

### 1-5 檢核點檢測標準

為使本檢測指引能適用於行動化應用軟體無障礙檢測，55 個檢核點 依三特性與 13 張檢核單順序排列，每一檢核點皆採用 ACT 規則格式編排，其詳細內容說明如後。

![](https://i.imgur.com/QiUz0OF.png)
![](https://i.imgur.com/XRR2wqn.png)


---

## :books: 呈現組件: (一) AT 替代文字與圖片
1. 期望:每個有意義的圖片、元件或物件等，都有替代文字，且能正確描述其意義:每個替代文字不需包含描述網頁元素的類型，如影片、圖片、鏈結等。
2. 檢測程序
    (1)啟動螢幕報讀軟體。 
    (2)識別任何有意義的圖片，元件或物件。 
    (3)驗證具有相等意義的文字說明替代，簡要描述功能的意圖。 
    (4)確認避免僅使用如“圖片”、“鏈結”之類的詞。

![](https://i.imgur.com/voUX7GK.png)



### :pushpin: 【AT1】非文字內容的替代品 (必要)
> **替代文字必須簡要描述圖片、物件或元件的編輯意圖或目的。** 適用於有意義的圖片內容。
>將alt屬性用於img元素，提供圖片相等意義的文字
>
>期望：每個有意義的圖片都有一個替代文字，該替代文字應簡要描述圖片意義並正確。說明:每個替代文字不需包含描述網頁元素的類型，如影 片、圖片、鏈結等。 


**成功範例原始碼：**
```htmlembedded=
<img src="example\_non\_dec orative_image.png" alt="\[alternative text for image\]" />
```
**失敗範例原始碼：**
* 範例 1:圖片
```htmlembedded=+
<img src="rating.jpg" alt="Greyed out stars" />
```
* 範例 2:輸入
```htmlembedded=+
<input id="t1" type="text" />
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 識別任何有意義的圖片、元件或物件。  
3. 驗證具有相等意義的文字說明替代，簡要描述功能的意圖。 
4. 確認避免僅使用如“圖片”、“鏈結”之類的詞。

###### 無障礙要求對應：網站無障礙規範1.1.1 非文字內容(檢測等級 A)

---

### :pushpin: 【AT2】裝飾性內容 (必要)
>  **裝飾性圖片必須從輔助技術中隱藏**。 適用性裝飾性圖片。
>  即使圖片是裝飾性的，也必須將 alt 屬性應用於 img 元素，但是必須將此屬性的值設置為 null(alt="")。
>  
>  期望：以下任一檢查正確:  
>  • 沒有意義的圖片、元件或物件不會獲得焦點，也不會被螢幕報讀軟體讀取。  
>  • 圖片、物件或沒有意義但取得焦點的元件被宣告為“不可用”或“禁用”，並且不可操作。


**成功範例原始碼：**
```htmlembedded=
<img scr="example\_decorati ve\_image" alt="" />
```

**失敗範例原始碼：**
```htmlembedded=+
<img scr="example\_decorati ve\_image" alt="*" />
```

**測試程序：**
1.  開啟螢幕報讀軟體。
2.  識別沒有特定意義任何圖片、元件或物件，已被關閉或被隱藏。 
3.  嘗試將焦點移到或導航到這些圖片、元件或物件。   
4.  確認圖片、元件或物件沒有獲得焦點並且沒有被螢幕報讀軟體讀取處理。
5.  如果可以導航到圖片、元件或物件，請確保將其聲明為“不可用”或“禁用”，並確認無法操作。

###### 無障礙要求對應：網站無障礙規範1.1.1 非文字內容(檢測等級 A)

---

### :pushpin: 【AT3】驗證碼或身份認證 (必要)
>  **驗證碼或身份認證應該依據行動裝置特性提供另一種驗證方式**
>  驗證碼：要求輸入圖形驗證碼的驗證內容。 
>  身份認證：身份登錄的驗證方式。
>  
>  期望：  
>  • 驗證碼:若提供圖形驗證碼時，能提供另一種的驗證方 式。
>  • 身份認證:身份登錄的驗證方式可搭配行動裝置特性進 行驗證，簡化登錄方式。


**測試案例(驗證碼)：範例原始碼：**
```htmlembedded
無提供原始碼範例
* 對於提供之圖形驗證碼提供替代文字說明。
* 提供瞭解圖形驗證碼的方式。
```
**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 針對圖形驗證碼，在其旁邊識別有建置語音播放方式的驗證碼，且能啟動播放語音。

---
**測試案例(身分證)：範例原始碼：**
```htmlembedded
無提供原始碼範例
```

**測試程序：**
1. 啟用受檢測應用程式。  
2. 確定是否有身分驗證功能。  
3. 如有身分驗證需求，確認是否存在一個或一個以上的替代方式進行驗證。

---

### :pushpin: 【AT4】視覺格式  (必要)
> **不得單獨使用視覺格式來傳達含義。** 適用於文字、圖片及圖表內容。
> 
> 應該在使用 CSS 的純 視覺格式上使用諸如 \[strong\]、\[em\]等的語 義標記，指示有意義的方面，例如文字格式。 此外，應使用列表和標題之類的結構來指示項目之間的關係。
>
>期望：當物件、元件或控件使用視覺格式傳達含義時，應該提供螢幕上的文字、替代文字或音訊提示。

:::warning
:warning:HTML:aria-owns 在某些使用者代理中支援有限。
:::

**成功範例原始碼：**
```htmlembedded=
<h2>Fruit</h2> 

<ul>
    <li>Apples</li> 
    <li>Oranges</li> 
    <li>Bananas</li>
</ul>

<div>An
    <strong>error</strong> was detected...
</div>
```

**失敗範例原始碼：**
```htmlembedded=+
<div class="heading">Fruit</div>

<div>
    <div style="padding- left:1em;">Apples</div>  
    <div style="padding-left:1em;">Oranges</div>
    <div style="padding- left:1em;">Bananas</div>
</div>

<div> 
    An<span style="font- weight:bold;">error</span> was detected...
</div>
```

**測試程序：**
1.  啟動應用程式。  
2.  確定是否有任何組件使用視覺格式傳達含義，包括:顏色、形狀/尺寸、字體屬性(粗體/斜體等)、位置、方向、選擇 等。 
3.  啟動報讀軟體。    
4.  確定是否存在補充視覺格式的說明文字、替代文字或音訊提示:
    •使用螢幕報讀軟體導航至該項目，以確認其是否有隱藏的說明敘 述。
    •目視驗證螢幕上文字的存在。

###### 無障礙要求對應：網站無障礙規範1.3.1 資訊與關連性(檢測等級 A)

---


### :pushpin: 【AT5】系列圖片  (選項)
> **在一組緊連圖片中的第一個項目使用替代文字，描述該組 圖片的所有項目資訊。** 適用於一連串的圖片內容。
>
>期望：需於系列圖片之第一項目描述該組圖片相關資訊。

**範例原始碼：**
```htmlembedded
無提供原始碼範例
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 識別系列圖片。  
3. 嘗試將焦點移到系列圖片中具有替代文字的項目。 
4. 螢幕報讀軟體讀出該組圖片的第 1 張內容。

###### 無障礙要求對應：網站無障礙規範1.1.1 非文字內容(檢測等級 A)

---

### :pushpin: 【AT6】文字圖片  (選項)
> **除標誌圖徽(logo)、圖示(icon)或使用畫布(canvas)的 互動式內容，應避免文字圖片。** 適用於圖片、文字內容。使用文字並使用 CSS 對文字進行樣式設定。
>
>期望：使用實際文字而非使用文字圖片。

**範例原始碼：**
```htmlembedded=
<h3>Eastenders</h3>
```
```css=+
h3 {  
font: bold italic 2em Georgia, Times, Arial;
border-bottom: 2px dashed black;
border-top: .5em solid black;
margin: 0; font-size: 1em;
}  
```

**測試程序：**
1.  啟動應用程式。    
2.  透過放大文字大小來確定文字圖片，以確定螢幕上的所有文字是否都會調整大小。
3.  以放大狀態查看螢幕，確定是否有任何文字看起來為像素化，以判定是文字圖片。 
4.  排除所有被視為例外可以用的文字圖片的狀況，例如標誌圖徽(logo)、圖示(icon)或使用畫布的互動式內容。

###### 無障礙要求對應：網站無障礙規範1.1.1 非文字內容(檢測等級 A)

---


### :pushpin: 【AT7】背景圖片 (選項)
> **傳達訊息或特別含義的背景圖片應該有其他無障礙的替代方式。** 適用於背景圖片內容。
> 
> 由於無法將替代文字分配給 CSS 背景，因此在 CSS 中使用行內圖片或適當的替換技術來提供可視和文字替代。
>
>期望：背景圖片不可被聚焦，若背景圖片為有意義傳達之圖片，應有替代的表達方式。


**成功範例原始碼：**
```htmlembedded=
<a>
    <img src="email.jpg" alt="Email"/>
</a>
```

**失敗範例原始碼：**
```htmlembedded=+
<div tabIndex="0" onclick="email();" 
     style="background-image:url('email.jpg');">
</div>
```

**測試程序：**
1.  啟動螢幕報讀軟體。  
2.  識別畫面中是否使用所有包含訊息的圖片。  
3.  識別哪些圖片是有包括特別含義的背景圖片。   
4.  確認螢幕報讀軟體報讀此背景圖片的替代文字。  
5.  在某些情況下，這可能需要檢查代碼或在非行動設備上進行測試。


###### 無障礙要求對應：網站無障礙規範1.1.1 非文字內容(檢測等級 A)

---
## :books: 呈現組件: (二) AV 時序媒體
1. 期望:
    • 時序媒體提供任何音訊內容的重要訊息同步字幕(開放或關閉的字幕)
    • 音訊內容不會自動播放

2. 檢測程序
    (1)啟動應用程式。
    (2)識別時序媒體。 
    (3)確定時序媒體是否具有包含重要訊息的音訊內容，例如口頭敘述。 
    (4)檢查是否透過字幕/打開/隱藏式字幕，同時提供與音訊同步的理解媒體所需的所有可聽訊息。 
    (5)確定時序媒體是否具有包含重要訊息的視覺內容-例如重要標示或加入新文字。 
    (6)檢查是否將理解時序媒體所需的任何視覺訊息之描述，作為音訊的一部分，或者是否提供音訊描述的單獨音軌，並與視訊同步。在適當的情況下，可以透過螢幕報讀軟體使用。

![](https://i.imgur.com/3fKtSDl.png)
![](https://i.imgur.com/niJtUiB.png)

### :pushpin: 【AV1】視聽內容的替代品 (必要)
> **時序媒體的替代內容(如字幕、手語、音訊描述)必 須在可用的情況下，伴隨嵌入式媒體提供。** 適用於影音內容。
>
>期望：時序媒體提供任何音訊內容的重要訊息同步字幕(開放 或關閉的字幕)。 使用與視訊內容(視訊描述)同步的音訊描述，理解媒體所必需的視覺內容，或者在適當情況下為螢幕報讀軟體提供文字內容。

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1.  啟動應用程式。 
2.  識別時序媒體。    
3.  確定時序媒體是否具有包含重要訊息的音訊內容，例如口頭敘述。
4.  檢查是否透過字幕/打開/隱藏式字幕，同時提供與音訊同步的理解媒體所需的所有可聽訊息。
5.  確定時序媒體是否具有包含重要訊息的視覺內容-例如重要標示或加入新文字。
6.  檢查是否將理解時序媒體所需的任何視覺訊息之描述，作為音訊的一部分，或者是否提供音訊描述的單獨音軌，並與視訊同步。在適當的情況下，可以透過螢幕報讀軟體使用。

###### 無障礙要求對應：網站無障礙規範1.2.3 音訊描述或替代媒體(檢測等級 A)

---

### :pushpin: 【AV2】不得自動播放音訊 (必要)
> **除非使用者知道會產生音訊或事先知道該音訊可提供暫停/停止/靜音的按鈕，否則音訊不得自動播放。** 適用於影音內容。
> 
>期望：以下檢查均正確: 
> • 音訊內容不會自動播放。
> • 警告使用者音訊將自動播放，並且可以控制停止或 暫停音訊。

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basic/warning.png)部份瀏覽器和輔助技術組合對原生的 Video 和 Audio 控件無法透過鍵盤訪問，並且 Video 或 Audio 元素本身可能無法宣告。通常建議作者使用 自定義控件進行鍵盤導航和跨瀏覽器無障礙支持。
:::

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1.  啟動螢幕報讀軟體。    
2.  識別自動播放的音訊內容。    
3.  在螢幕報讀軟體處於活動狀態加載媒體時，檢查其包含頁面是否在播放時不會自動播放音訊，或者檢查是否已警告使用者並且提供停止或暫停音訊的控件。


###### 無障礙要求對應：1.4.2 音訊控制(檢測等級 A)

---

### :pushpin: 【AV3】提供詮釋資料 (選項)
> **應該為所有媒體提供相關的詮釋資料。** 適用於影音內容。
> 
>期望：以下檢查均正確:為媒體提供了正確的詮釋資料。
>在必要時提供有關格式的資訊，例如發布日期、持續時間、格式(字幕、手語、音訊描述、高清晰度等)或語言。

**成功範例原始碼：**
```htmlembedded=
<head>
  <title>Weekend Update</title>
  <meta name="description" content="A multimedia guide to your weekend">
  <meta name="keywords" content="Weekend，news">  
  <link rel="alternate" type="application/htm l" media="screen" title="Weekend Update Text Version" href="http://www.bbc .com/mobile/weekend Update.html" />
</head>
```
**失敗範例原始碼：**
```htmlembedded=+
<head>
  <title>Weekend Update</title> 
  <meta name="description" content="A multimedia guide to your weekend">
  <meta name="keywords" content="Weekend，news">  
</head>
```

**測試程序：**
1. 識別時序媒體。 
2. 查看頁面原始檔。 
3. 驗證頁面頂部是否指示詮釋資料(metadata)內容，並指出替代媒體的位置。


###### 無障礙要求對應：無

---

### :pushpin: 【AV4】音量控制 (選項)
> **應該為背景音樂、環境聲音、敘述性和編輯上重要的 音效提供單獨的音量控制。** 適用於播放音效之內容。可以在設置中提供單獨的音訊控件，以控制輔助音訊軌道。
> 
> 期望：以下檢查均正確
>• 所有聲音均可獨立於螢幕報讀軟體靜音。  
>• 適當時，可以獨立控制和調整音訊各個方面的音量。

**範例原始碼：**
```htmlembedded
無範例程式碼
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 識別嵌入式媒體內容。  
3. 驗證是否存在合適的音量控制並且功能正常。

###### 無障礙要求對應：無

---

### :pushpin: 【AV5】不得音訊衝突 (選項)
> **遊戲或互動式媒體中的敘事音訊不應蓋過或與原生輔助技術衝突。** 適用於播放音效之內容。可以在設置中提供單獨的音訊控件，以控制輔助音訊軌道。
> 
> 在默認情況下，當音訊嵌入 HTML 頁面中時，TalkBack 和 VoiceOver 音訊都將優先於所有其他形式的音訊輸出(例如 YouTube 視訊)。
> 
> 期望：受測程式發出音效，同時可以清楚聽到螢幕報讀軟體的音訊。

**範例原始碼：**
```htmlembedded
無範例程式碼
```

**測試程序：**
1. 識別時序媒體。  
2. 啟動螢幕報讀軟體。  
3. 確保可以聽到螢幕報讀軟體報讀聲音，並且不會與媒體中的任何音訊發生不必要的衝突。

###### 無障礙要求對應：無

---
## :books: 呈現組件: (三) NT 通知
1. 期望：
    • 通知訊息必須同時可見和可聽
    • 提供明確的錯誤訊息
2. 檢測程序
    (1)啟動應用程式。 
    (2)在應用程式中的物件，元件或控件上觸發警告或錯誤。 
    (3)驗證警告或錯誤指示是否存在可見和可聽的提示。 
    (4)驗證警告或錯誤通知是否清楚指示需要更正的操作。 
    (5)啟動螢幕報讀軟體。
    (6)重複步驟 2-3。

![](https://i.imgur.com/OS6Xw18.png)
![](https://i.imgur.com/Dq416c9.png)


### :pushpin: 【NT1】包容性通知 (必要)
> **通知訊息必須同時可見和可聽。** 適用於通知內容。
> 
> 以包容性方式提供通知，將視覺提示與音訊和觸覺提示相結合。
> 例如，如果使用者在表單欄位中鍵入太多字符，則除了聲音和/或振動外，還會在表單欄位的標籤中顯示錯誤。 
> 對於使用輸入元素創建的單選按鈕或複選框之類的標準控件，這些狀態更改由瀏覽器自動提供。
> 但是，對於圖片和其他自定義控件，這些更改必須以視覺，文字方式提供，也可以透過 ARIA 提供。隨著狀態的改變，應該為圖片添加新的文字替代。也可以使用 ARIA，但不能完全依靠 ARIA。非 ARIA 後備選項必須可用。
> 
> 期望：以下檢查均正確:  
> • 該應用程式為用於傳達訊息或錯誤的每個警告或通知提供可見和可聽提示。  
> • 螢幕報讀軟體會正確報讀物件、元件或控件，包括其標籤、角色、值、狀態和狀態更改。

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basic/warning.png)HTML:舊瀏覽器未支援角色屬性超過一個以上的 符記，角色屬性使用多個值時，舊瀏覽器將忽略此 屬性。
:::

**成功範例原始碼：**
```htmlembedded=
<audio id="audio1" autostart="">
    <source src="beep.mp3" type="audio/mp3" /> 
    <embed id="audio2" src="beep.mp3" autostart="false" loop="false">
    </embed> 
</audio>

<label id="l1" for="uname">Create Username (max 8 characters):</label>
<input type="text" id="uname" onblur="checkLength (this);"/>
```

```javascript=+
<script  type="text/javascript">
     Function checkLength(obj) {
         var str =  obj.value;
         if (str.length >= 8) {
             document.getElementById("l1").textContent = "Create Username (max 8 characters): ERROR - must be 8 characters or less";
             document.getElementById("audio1").play();
         }
    }
</script>
```

**失敗範例原始碼：**
```htmlembedded=+
<audio id="audio1" autostart="">
    <source src="beep.mp3" type="audio/mp3" />
    <embed id="audio2" src="beep.mp3" autostart="false" loop="false">
    </embed> 
</audio>

<label id="l1" for="uname">Create Username:</label>
<input type="text" id="uname" onblur="checkLength (this);" />
```

```javascript=+
<script type="text/javascript" >  
    Function checkLength(obj) { 
        var str = obj.value;
        if (str.length >= 8){
            document.getElementById("audio1").play();
        }
    }
</script>
```

**測試程序：**
1. 在未啟動螢幕報讀軟體的情況下啟動應用程式。  
2. 在應用程式內完成表單，並觸發錯誤訊息為測試依據。  
3. 識別用於指示錯誤狀態或表單完成的所有提示。  
4. 驗證是否存在其他提示(文字或視覺、音訊或振動)以提供與所傳達的訊息相同的訊息。 
5. 啟動螢幕報讀軟體。   
6. 關注可以改變狀態的單個物件、元件或控件。   
7. 確認已觸發的項目標籤與螢幕上的文字匹配或包含其他補充訊息，以幫助非可視地訪問該項目。  
8. 驗證元件的狀態是否正確聲明。
9. 如果適用，請切換項目的狀態並確認螢幕報讀軟體報讀正確的狀態更改。

###### 無障礙要求對應：4.1.2 名稱、角色和值(檢測等級 A)

---

### :pushpin: 【NT2】錯誤訊息和更正 (必要)
> **必須提供明確的錯誤訊息。** 適用於通知內容。
> 
> 在表單頂部顯示錯誤訊息，並帶有適 當的級別標題和錯誤欄位的指示。提 交失敗後，將焦點 移至錯誤訊息。
> 
> 期望：以下檢查均正確:  
> •指出錯誤點或警告。 
> •警告和錯誤通知提供足夠的訊息，讓使用者可以識別哪些表單控件包含錯誤。



**成功範例原始碼：**
```htmlembedded=
<!-- added and given focus on submission -->
<h3 id="errors">Errors were found</h3> 
<ul>
    <li>"Re-type email address" field does not match "email address".</li>
    <li>"I agree" checkbox is not checked.</li>
</ul>

<form>...</form>
```

**失敗範例原始碼：**
```htmlembedded=+
Fix the items marked below in red
<form>...</form>
```

**測試程序：**
1. 啟動應用程式。  
2. 在應用程式中的物件、元件或控件上，觸發警告或錯誤。 
3. 驗證警告或錯誤指示是否存在錯誤。  
4. 驗證警告或錯誤通知是否清楚指示需要更正的操作。


###### 無障礙要求對應：3.3.3 錯誤建議(檢測等級 AA)

---

### :pushpin: 【NT3】標準作業系統通知 (選項)
> **在可用且適當的地方，應使用標準作業系統通知。** 適用於通知內容。
> JavaScript 警告是 HTML 滿足此標準 的一種選擇。
> 
> 期望：以下檢查正確: 
> •該應用程序使用操作系統標準方法來提供應用程序層級或非操作觸發的警告，並透過輔助技術向使用者指示錯誤。


**成功範例原始碼：**
```htmlembedded=
<label for="myPassword"> 請輸入密碼</ label>
<input id="myPassword" type="password" aria- describeby="passwor dInstructions"/ >
<span tabindex="-1" id="passwordInstructi ons"> 輸入至少 14個字符以獲取強密 碼。</span>
```

**失敗範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 啟動受測的應用程式或遊戲。  
3. 識別或啟動任何反饋、提示或幫助。  
4. 驗證此幫助既可視又可供螢幕報讀軟體使用。 
5. 驗證此協助是否適當。

###### 無障礙要求對應：3.3.1 識別錯誤(檢測等級 A)

---

### :pushpin: 【NT4】反饋和幫助 (選項)
> **適當時應提供非關鍵性的反饋或幫助。** 適用於通知內容。
> 必要時，在應用程序中提供幫助文檔。確保內容易於查找，例如，將“ 幫助”選項放在應用程序的導航和/或設置選單中。 此外，必要時提供上下文相關的幫助。例如，如果使用者正在創建密碼，請指明代表強 密碼的字符數。 避免給使用者過多的反饋。
> 
> 期望：以下檢查正確: 
> •提供的幫助是適當且包容(可見和可聽)。

**成功範例原始碼：**
```javascript=
<script> alert('Statusmessage'); </script>
```

**失敗範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 在應用程式觸發警告或錯誤，例如:超時、更新通知與伺服器連接時出錯，或在連接其他應用程式的錯誤或警告。 
3. 驗證警告或錯誤通知是否由輔助技術發布。

###### 無障礙要求對應：3.3.5 協助(檢測等級 AAA)

---

## :books: 互動組件: (一) TS 觸控操作
1. 期望：
    • 所有多點觸控或路徑觸控有替代的單點觸控
    • 觸控目標可以順利以手指觸發動作/事件且不易誤觸
2. 檢測程序
    (1)使用觸控螢幕瀏覽該應用程式。 
    (2)識別提供多點觸控或路徑觸控操作的物件、元件和控件。 
    (3)驗證具有複雜功能的項目是否提供有替代的單點觸控，例如使用箭頭鍵代替上下滑動手勢來移動滑塊。

![](https://i.imgur.com/5SNlY6h.png)


### :pushpin: 【TS1】單點觸控 (必要)
> **確認多點觸控或路徑觸控需有替代的單點觸控。** 適用於觸控內容。
> 
> 
> 期望：以下檢查均正確:
> •所有多點觸控有替代的單點觸控。
> •所有路徑觸控有替代的單點觸控。

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1. 使用觸控螢幕瀏覽該應用程式。  
2. 識別提供多點觸控或路徑觸控操作的物件、元件和控件。  
3. 驗證具有複雜功能的項目是否提供有替代的單點觸控，例如使用箭頭鍵代替上下滑動手勢來移動滑塊。

###### 無障礙要求對應：2.5.1 指標手勢(檢測等級 A)

---
### :pushpin: 【TS2】觸發操作 (必要)
> **觸發操作以向上事件為主，需有防止誤觸設計** 適用於觸控內容。
> 預設使用原生 HTML 元素處理觸 控事件。盡可能使用 onclick 和 onkeypress 事件觸發動作。
> 
> 期望：以下檢查均正確
> •物件、元件和控件在啟動開始時(當觸摸時)不會直接觸發動作/事件。 
> •當使用者完成啟動(觸摸已移開)時，物件、元件和控件將觸發操作/事件。


**成功範例原始碼：**
```htmlembedded=
<!-- Preferable (native elements) --> 
<button onclick="...">Click me to do something! </button>
```

```javascript=+
// Custom actions
<script>
    function startGesture(e) {
        // store touch start source
    }
    
    function endGesture(e) {
        // if touch end source is different from touch start source return, else perform action
    }
</script>
```

```htmlembedded=+
<div onTouchStart="startG esture(this);" onTouchEnd="endGe sture(this);">
    Swipe area 
</div>
```

**失敗範例原始碼：**
```htmlembedded=
<div onTouchStart="startG esture(this);">
    Swipe area 
</div>
```
```javascript=+
<script type="text/javascript" >  
    function startGesture(e) {  
        // perform action
    }
</script>
```

**測試程序：**
1. 使用觸控螢幕瀏覽該應用程式。  
2. 導航到螢幕上的物件、元件和控件。  
3. 開始啟動一個項目(觸摸時無需抬起手指或手寫筆)。 
4. 驗證該項目不會立即觸發動作/事件。  
5. 完成啟動項目(從螢幕上移開手指或手寫筆)。  
6. 驗證該項目觸發動作/事件。

###### 無障礙要求對應：2.5.2 指標取消(檢測等級 A)

---
### :pushpin: 【TS3】觸控目標尺寸 (必要)
> **觸控目標尺寸至少 48dp\*48dp(9mm\*9mm)。** 適用於螢幕觸控、觸發內容。
>
>在鏈結周圍提供間距，以確保所有可操作的控件之間的距離至少為 7mm。 使用較大的控件， 即 9mm，或增加內容周圍的間距以確保較大的觸摸區域。 使用如清單元素提供頁面內容的結構如導覽，並使用 CSS 為每個觸控目標添加 padding 與 margins 距離。
>
> 期望：以下檢查均正確
> •所有觸控目標可以順利以手指觸發動作/事件，不會誤觸。


**成功範例原始碼：**
```css=
<style>
    button { 
        box-sizing:border-box; 
        min-width: 44pt;
        min-height: 44pt;
    }
</style>
```
```htmlembedded
<button>Tap me! </button>
```

**失敗範例原始碼：**
```htmlembedded=
<a href="/">Home</a> | <a href="/news">News</a> | <a href="/sport">Sport</a>
```

**測試程序：**
1. 使用觸控螢幕瀏覽該應用程式。 
2. 識別所有觸控目標。
3. 驗證觸控目標尺寸是否至少 48dp\*48dp(9mm\*9mm)，可以順利 以手指觸發動作/事件，不會誤觸。

###### 無障礙要求對應：2.5.5 目標尺寸(檢測等級 AAA)

---
### :pushpin: 【TS4】並行輸入機制 (選項)
> **容許並行輸入機制的方式，如外接鍵盤或手寫筆等。** 適用於可輸入及可編輯內容。
>
>確保透過特定手勢 如滑動而觸發的任何功能，亦可使用不同的輸入裝置觸發，如外接鍵盤。 例如，如果左右滑動改變在輪播中的面板，提供單獨的按鈕控件標註”上 一個”與”下一個 ”，讓不用或不能使用滑動手勢的使用者(但使用單獨的輸入裝置如鍵盤)， 也可利用此功能。
>
> 期望：以下檢查均正確
> •物件、元素和控件可以透過替代輸入方式導航。 
> •項目可透過替代輸入方式啟動與操作。

**成功範例原始碼：**
```htmlembedded
<a href="...">Previous</a>  
<a href="...">Next </a>
```

**失敗範例原始碼：**
```javascript=
<script type="text/javascript">  
    ... // perform some action on touch 
</script>
```

```htmlembedded=
<div 
ontouchstart="touchSt art(event);" 
ontouchmove="touch Move(event);" 
ontouchend="touchEn d(event);" 
ontouchcancel="touch Cancel(event);"></div>
```

**測試程序：**
1. 啟動螢幕報讀軟體和外接實體鍵盤或手寫筆。 
2. 確定受測的螢幕上的物件、元件和控件。  
3. 確認可以通過替代輸入方式導航所有項目。 
4. 確認可以通過其他輸入方式啟動項目。
5. 啟動項目。  
6. 針對具有複雜功能的項目，檢查具有動作支援如方向鍵的相等方式取代上下滑動的手勢來移動滑塊。

###### 無障礙要求對應：2.5.6 並行輸入機制(檢測等級 A)

---
## :books: 互動組件: (二) FC 焦點
1. 期望：
    • 所有多點觸控或路徑觸控有替代的單點觸控
    • 觸控目標可以順利以手指觸發動作/事件且不易誤觸
    • 每個可操作的元件都可以通過觸摸的方式，以視圖的焦點順序顯示
    • 目標元件或控件可以使用標準導航方法進行瀏覽或離開
    • 焦點順序等同於頁面直觀的視覺閱讀順序
    
2. 檢測程序
    Android 系統:
        (1)開啟 TalkBack。 
        (2)確認每個可操作元素都可以直接導航(透過觸控 Android4+)。
        (3)確認可以使用鍵盤或 d-pad 導航到每個可操作的元素。
    iOS:
        (1)開啟 VoiceOver。 
        (2)驗證每個可操作物件都可以直接訪問(透過觸摸)，並以視圖的焦點順序顯示。 
        (3)驗證每個可操作的物件皆可使用螢幕報讀軟體透過導航(滑動手勢)獲得焦點。

![](https://i.imgur.com/gO6joZz.png)



### :pushpin: 【FC1】可聚焦元件 (必要)
> **所有互動元件必須是可聚焦的，非互動元件必須不能 聚焦。** 適用於互動元件。
>
>確保透過特定手勢 如滑動而觸發的任何功能，亦可使用不同的輸入裝置觸發，如外接鍵盤。 例如，如果左右滑動改變在輪播中的面板，提供單獨的按鈕控件標註”上 一個”與”下一個 ”，讓不用或不能使用滑動手勢的使用者(但使用單獨的輸入裝置如鍵盤)， 也可利用此功能。
>

:::info
* 使用如 button、a 和 input 元素等原生交互式元素，而不要重新使用另一個元素，因為此類控件預設是可獲得焦點，並且包含所需的語義和行為。
* 如果必須使用預設無法透過鍵盤訪問的元素(例如 div 和 span 元素)，則應使用 tabindex 屬性， 並將其值設置為 0。
* 將需要進一步的腳本編寫，以確保可以在適當的情況下使用 Enter、空格鍵 或方向鍵來觸發此類元素，並且將需要進一步的 WAI- ARIA 標記，以確保 將元素正確地暴露於輔助技術。
* 請勿將 tabindex 屬性值為0或大於0的屬性應用於非活動/非 交互式元素，例如標題和圖片。 對於不活動的元素，透過使用 disabled，從焦點順 序中移除該元素。 這是首選方法，因 為它得到很好的支援。
* 或者在支援的地方禁用 aria 的屬性，使用 tabindex 屬性並將其值設置為\- 1，然後使用 aria- hidden 屬性並將其值設置為 false。還可以使用 tabindex 屬性並使用 aria-hidden 屬性將其值設置為\- 1。
:::
>
> 期望：以下檢查均正確
> •每個可操作的元件皆可直接獲得焦點(透過觸摸);  
> •每個可操作的元件皆可以使用鍵盤或 d-pad 獲得焦點/導航。 以下檢查均正確(iOS):
> •每個可操作的物件皆可直接獲得焦點(透過觸 摸)，並以視圖的焦點順序顯示;
> •每個可操作的物件皆可使用螢幕報讀軟體透過滑 動手勢獲得焦點。
> 

**成功範例原始碼：**
```htmlembedded=
<!-- Standard button element that is interactive by default -->
<button>Click me! </button>

<!-- Custom button made focusable using tabindex="0", and provided with an appropriate role -->
<span role="button" tabindex="0" onclick="...">Click me!</span>

<!-- Disabled/non- interactive button(option 1) -->  
<button tabindex="-1" aria-hidden="true">I am not focusable! </button>

<!-- Disabled/non- interactive button(option 2) --> 
<button disabled>I am discoverable by screen readers but not focusable!</button>
```

**失敗範例原始碼：**

```htmlembedded
無範例原始碼
```

**測試程序：**
Android 系統:
1.  開啟 TalkBack。    
2.  確認每個可操作元素都可以直接導航(透過觸控 Android4+)。  
3.  確認可以使用鍵盤或 d-pad 導航到每個可操作的元素。
    
iOS:
1.  開啟 VoiceOver。  
2.  驗證每個可操作物件都可以直接訪問(透過觸摸)，並以視圖的焦點順序顯示。
3.  驗證每個可操作的物件皆可使用螢幕報讀軟體透過導航(滑動手勢)獲得焦點。

###### 無障礙要求對應：2.1.1 鍵盤(檢測等級 A)

---
### :pushpin: 【FC2】鍵盤陷阱 (必要)
> **不得有鍵盤陷阱。** 適用於焦點內容。
>
>確保焦點不會因 JavaScript 方法如 onBlur、onChange、 onFocus 或嵌入式元件而落入陷阱。當檢查第三方元件時，應確保可以 tab 鍵進入與離開內容。
>如果內容必須以可能引起鍵盤陷阱的方式提供，則應提供使用者可繞過該內容的方法，例如透過在內容上面的頁面內鏈結，引導使用者直接到該內容下方的位置。
>
> 期望：以下檢查均正確
> •物件、元件或控件可以使用標準導航方法進行瀏覽或離開。
> •以可見的方式並透過螢幕報讀軟體離開項目導航的方法，該方法可將焦點穿過或跨過鍵盤陷阱。

**成功範例原始碼：**
```javascript=
// JavaScript updates field label to indicate an error but does not trap focus -->
<script>  
    function check() {
        if (isValid()) {  
            // update field label to explain that field is in error but do not trap focus
            var s = createElement("span");  
            s.innerText ="(Invalid name)";
            document.getElementById("l1").appendChild(s);
        }
    }
</script>
```
```htmlembedded=+
<label id="l1" for="name1"> First name</label>
<input onBlur="check();" type="text" id="name1">
```

**失敗範例原始碼：**
```javascript=
<!-- JavaScript keeps returning focus to a field until a user enters data correctly -->
<script type="text/javascript" >  
    function check() {
        if (isValid()) { 
            document.getElement ById("name1").focus();
        } 
    }
</script>
```

```htmlembedded=
<label for="name1"> First name</label> 
<input onBlur="check();" type="text" id="name1">
```

**測試程序：**
1.  啟動螢幕報讀軟體。  
2.  導航到可操作的物件、元件或控件。    
3.  當焦點位於項目上時，嘗試透過導航方法離開項目。   
4.  確保焦點移出項目。   
5.  如果焦點不能透過標準手勢或方法移出項目，請確保移出項目焦點的方法有視覺的描述與透過螢幕報讀軟體描述，如對話框 有關閉按鈕，或提交/取消按鈕。

###### 無障礙要求對應：2.1.2 無鍵盤操作陷阱(檢測等級 A)

---
### :pushpin: 【FC3】焦點順序 (必要)
> **必須以有意義的順序瀏覽可操作的內容。** 適用於焦點內容。
> 以下內容將確保內容的邏輯順序: 
> • 根據 tab 順序進行編碼。
> • 注意 tabIndex(正數、0 和負數)可能在行動裝置瀏覽器不受支援。
> • 不要將表格用於佈局目的。
> 
> 期望：以下檢查均正確
> 焦點順序與頁面直觀視覺閱讀順序相同。 
> • 當新增的項目出現或啟用，這些項目將出現在觸發他們的項目之後。
> • 焦點以直覺的方式前後移動。


**成功範例原始碼：**
```htmlembedded=
<div>
    <h3>Shipping Address</h3>
    <label for="n1">Name</lab el><input type="text" id="n1">
    <label for="a1">Address</la bel><input type="text" id="a1">
    ... 
</div>
<div>
    <h3>Billing Address</h3>
    <label for="n2">Name</lab el><input type="text" id="n2">
    <label for="a2">Address</la bel><input type="text" id="a2">
    ... 
</div>
```

**失敗範例原始碼：**
```htmlembedded=+
<table> 
    <tr>
        < td>Shipping Address</td>
        < td>Billing Address</td>
    </tr> 

    <tr>
        <td><label for="n2">Name</label><input type="text"></td>
        <td><label for="n1">Name</label><input type="text"></td>
    </tr> 

    <tr>
        <td>
            <label for="a1">Address</label>
            <input type="text"></td>  
        <td>
            <label for="a2">Address</label>
            <input type="text">
        </td>
    </tr>
</table>
```

**測試程序：**
1.  使用螢幕報讀軟體啟動應用程式。
2.  瀏覽運作中螢幕的物件、元件和控件。
3.  驗證焦點順序是否與頁面的直觀視覺閱讀順序相同。 
4.  選擇單選按鈕、複選框和其他可操作的物件、元件和控件。 
5.  如果新增的項目出現或啟用，確定這些項目是否之後位於焦點順序之中。新進出現的區塊應該之後出現於焦點順序之中。確 保焦點以直覺的方式前後移動。注意:Android 具備焦點模擬 器，可用於方向控制器不存在時使用。


###### 無障礙要求對應：2.4.3 焦點順序(檢測等級 A)

---
## :books: 互動組件: (三) FM 表單
1. 期望：
    • 螢幕報讀軟體會報讀所有表單欄位標籤及輸入類型
    • 對於每組項目之間的導航和互動必須按順序進行
    • 輸入表單欄位或選擇物件、元件和控件中的項目時，焦點不會移開
    
2. 檢測程序
   (1)啟動螢幕報讀軟體。
   (2)瀏覽頁面上的表單欄位。 
   (3)確認導航到表單欄位時螢幕報讀軟體可以識別表單欄標籤。 
   (4)根據表單欄位填寫內容時，不會強行移動焦點位置。

![](https://i.imgur.com/WE6DDTt.png)

### :pushpin: 【FM1】標記表單控件 (必要)
> **必須標記所有表單控件。** 適用於表單內容。

>==使用 label 元素與表單控件視覺標籤明確連結，並將 for 屬性對應至該標籤，且屬性值必須與關連的表單控件的 id 屬性匹配。== 某些情況下，頁面的視覺設計可能意味著對顯示一個單獨、視覺與程式化連結標籤有困難或潛在困擾。
>案例包含在資料表格中的表單控件(無相關聯的表格標題代表視覺標籤)與搜尋欄位 (可見標籤為”搜尋 ”的按鈕，或放大鏡圖示，可能已經指出此為搜尋欄位)，此情況下，可使用 title 屬性。
>
>使用 aria-required 屬性指出必填的表單欄位，以及可見的指示(如*號)，確保輔助技術使用者能獲得該欄位為必填的通知。
>==如果沒有支援舊版瀏覽器的問題，應使用 HTML5 required 屬性取代。==  
>如果基於 ASCII 碼的星號用於指出必填欄位，則使用 aria-hidden 屬性於字符容器並設定屬性值為 false，確保對螢幕報讀軟體隱藏。
> 
> 期望：以下檢查均正確
> • 所有表單輸入欄位具有視覺的標籤。   
> • 螢幕報讀軟體正確報讀所有表單輸入欄位標籤。
> • 驗證移除上下文內容時，標籤可清楚且唯一描述控件的用途與使用者應採取的動作。 透過螢幕報讀軟體正確報讀表單輸入欄位的限制。   
> • 必填輸入欄位可由螢幕報讀軟體清楚指出。

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basic/warning.png)HTML:演示角色的實現衝突解決方案從一種瀏覽器或輔助技術到另一種瀏覽器或輔助技術有所不同。依賴於此，某些元素可以具有適用的語義角色之一，並且在某些技術下無法通過此規則，但是其他技術的使用者將不會遇到任何無障礙問題。
:::

**成功範例原始碼：**
```htmlembedded=
<!-- Example 1 -->

<label for="firstname">First name (required):</label>
<input type="text" id="firstname">

<!-- Example 2 -->
<input type="text" title="Enter a list of search terms">
<input type="button" value="Search">

<!-- Example 3 -->
<label for="firstname">First name:
    <span aria- hidden="true">*</span>
</label>
<input type="text" id="firstname" aria- required="true">
```

**失敗範例原始碼：**
```htmlembedded=+
<div>Username:
    <input type="text" id="uname"/>
</div>
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 瀏覽頁面上的表單欄位。

###### 無障礙要求對應：3.3.2 標籤或說明(檢測等級 A)

---
### :pushpin: 【FM2】表單輸入 (必要)
> **必須指明並支援預設輸入格式。** 適用於表單內容。

:::info
HTML5 為表單引進許多新的輸入類型，之前開發人員必須創建，自定義組件，範例包含:
* input type="search"  
* input type="email"  
* inputtype="tel"
* input type="range"  
* inputtype="time"
* inputtype="date" 

必須注意這些輸入 類型的支援具變異性，特別是在舊版瀏覽器與輔助技術，因此(如果考慮舊版瀏覽器的支援)提供未受支援輸入 類型的備用方法(如 自定義的日期揀選 器)，在此種情況下，需確保備用的插件具可及性。 即使使用以上之一輸入類型時，需在表單控件的標籤中以文字指出任一必填格式。
例如當抽出日期時，在標籤中指出日期格式，將能協助偏好手動增加日期而非從日期揀選器插件選取日期的使用者。
:::

> 
> 期望：以下檢查正確
> 向使用者呈現正確的鍵盤類型: 
> •文字鍵盤類型用於自由文字。 
> •數字鍵盤類型用於數字輸入。 
> •電話號碼鍵盤類型用於電話號碼。
> •日期鍵盤類型用於日期。 
> •日期與時間鍵盤類型用於日期與時間。 
> •月份鍵盤類型用於月份。 
> •搜尋鍵盤類型用於搜尋輸入。
> •URL 鍵盤類型用於搜尋。 
> •email 鍵盤類型用於 email。 
> •密碼輸入類型用於密碼。

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basic/warning.png)HTML:儘管 autocomplete 是 HTML 支持個人化的有為技術，但輔助技術對此功能的支援則非常有限。
:::

**成功範例原始碼：**
```htmlembedded=
<!-- input[type=range] with descriptive fallback text inassociated label: -->
<label for="t1">Rating (between 1 and 5):</label>
<input type="range" min="1" max="5" value="3" id="t1">
```

**失敗範例原始碼：**
```htmlembedded=+
<!-- No indication of expected input: -->
<label for="t1">Rating:</label>  
<input type="text" id="t1">
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 找到表單欄位。  
3. 驗證鍵盤類型與輸入相關。
• 文字鍵盤類型用於自由文字。  
• 數字鍵盤類型用於數字輸入。  
• 電話號碼鍵盤類型用於電話號碼。 
• 日期鍵盤類型用於日期。
• 日期與時間鍵盤類型用於日期與時間。 
• 月份鍵盤類型用於月份。  
• 搜尋鍵盤類型用於搜尋輸入。  
• URL 鍵盤類型用於搜尋。
• email 鍵盤類型用於 email。 
• 密碼輸入類型用於密碼。


###### 無障礙要求對應：1.3.5:識別輸入目的(檢測等級 AA)

---
### :pushpin: 【FM3】分組表單元件 (必要)
> **控件、標籤和其他表單元件必須正確配對。** 適用於複雜表單內容。
> 使用 fieldset 和 legend 將相關表單控 件具語意地分組。
> 
> 期望：以下檢查正確
> 以下檢查均正確: 
> •邏輯分組一部分的螢幕上欄位具有可見分組名稱，指出為螢幕上欄位的標籤一部分。 
> •對於分組的每個欄位，螢幕報讀軟體報讀分組標籤優先於欄位標籤。
> •對於每組項目，組項目之間的導航和互動必須按順序進行。例如，正確分組的 HTML 單選按鈕允許透過向上和向下箭頭在它們之間進行導航。

**成功範例原始碼：**
```htmlembedded=
<!-- Text inputs  -->
<fieldset>
    <legend>Delivery Address</legend>
    <label for="deliveryHouseN umber">House number:</label>
    <input type="text" id="deliveryHouseNu mber"><br/> 
    <label for="deliveryStreetAd dress">Street address:</label>
    <input type="text" id="deliveryStreetAd dress"><br/> 
    <label for="deliveryTown"> Town:</label>
    <input type="text" id="deliveryTown"><br/>
</fieldset>

<!-- Radio buttons -->
<fieldset> 
    <legend>Do you like football? </legend>
    <input type="radio" id="yesFootball" value="yes" name="football">
    <label for="yesFootball">Yes</label><br/> 
    <input type="radio" id="noFootball" value="no" name="football">
    <label for="noFootball">No</label>
</fieldset>

<!-- Checkboxes -->
<fieldset>
    <legend>Select your favourite sports:</legend>
    <input type="checkbox" id="football" name="sports" value="football">
    <label for="football">Footb all</label><br/> 
    <input type="checkbox" id="rugby" name="sports" value="rugby">
    <label for="rugby">Rugby</label> <br/>
    <input
    type="checkbox" id="golf" name="sports" value="golf">
    <label for="golf">Golf</label>  <br/>
    <input type="checkbox" id="cricket" name="sports" value="cricket">
    <label for="golf">Cricket</label>
</fieldset>  

<!-- Custom form controls Use WAI-ARIA grouping markup for custom form controls, as follows (Note: use role="radiogroup" for groups of custom radio buttons, and role="group" for all other types of controls): -->
<p id="groupLabel" tabindex="-1">Do you like football?</p> 
<div role="radiogroup" aria- labelledby="groupLa bel">
    <span role="radio" aria-checked="false" tabindex="0" aria- labelledby="groupLa bel yesFootball">
        <img src="unchecked.png" alt=""> 
    </span>
    <span id="yesFootball" tabindex="- 1">Yes</span>
    <span role="radio" aria-checked="false" tabindex="-1" aria- labelledby="groupLa bel noFootball">
        <img src="unchecked.png" alt=""></span>
    <span id="noFootball" tabindex="- 1">No</span>
</div>
```

**失敗範例原始碼：**
```htmlembedded=+
<input name="r1" type="radio" id="r1" value="yes"/>
<label for="r1">Yes</label>
<input name="r2" type="radio" id="r2" value="no"/>
<label for="r2">No</label>
```

**測試程序：**
1.  啟動螢幕報讀軟體。    
2.  找到螢幕上的任何表單。    
3.  確定表單中是否存在一個或多個邏輯分組。    
4.  導航至該分組中的每個欄位，並驗證該分組的名稱是否較該欄 位標籤優先報讀。
5.  驗證與每個分組的互動方法，是否替代輸入方法一樣有效。

###### 無障礙要求對應：3.3.2 標籤或說明(檢測等級 A)

---
### :pushpin: 【FM4】管理焦點 (必要)
> **在使用者輸入過程中，焦點或上下文不得自動更改。** 適用於表單內容。
> 提前告知使用者上下文或焦點變更情形者，符合此檢核點，如輸入信用卡號自動跳欄，提前知悉可通過此項檢核點。
>
> 除非由使用者明確地觸發，否則避免在表單控件與其他介面元件之間移動焦點。
> 例如，提供單獨的介面元件(如送出按鈕)讓使用者啟動相關的程式碼。因此，焦點僅當使用者啟動該按鈕時才變更。尤其避免將 onChange 事件處理器使用於表單控件，如下拉選單。
>
>
> 期望：以下檢查正確
> • 物件、元件或控件在啟動開始(觸摸時)不會觸發動作/事件。 
> • 物件、元件或控件在使用者完成啟動(觸摸移開)即觸發動作/事件。

**成功範例原始碼：**
```htmlembedded=
<fieldset> 
    <legend>Mobile phone number</legend>
    <label for="p1"> Country code</label>  
    <input type="text" id="p1" onBlur="validateCod e();" />
    <label for="p2"> Number </label>
    <input type="text" id="p2" onBlur="validateNum ber();" />
</fieldset>
```

**失敗範例原始碼：**
```htmlembedded=+
<fieldset>
    <legend>Mobile phone number</legend>
    <label for="p1"> Country code</label>  
    <input type="text" id="p1" onChange="validateA ndMove();" />
    <label for="p2"> Number </label>
    <input type="text" id="p2" onChange="validateA ndMove();" />
</fieldset>
```

**測試程序：**
1. 使用觸控螢幕啟動應用程式。  
2. 導航到螢幕上的物件、元件或控件。  
3. 開始啟動項目(觸摸而不拿起手指或手寫筆)
4. 驗證該項目未立即觸發動作/事件。
5. 完成啟動項目(從螢幕中移開手機或手寫筆) 
6. 驗證該項目以觸發動作/事件。

###### 無障礙要求對應：3.2.1 焦點(檢測等級 A)

---
### :pushpin: 【FM5】表單佈局 (選項)
> **標籤必須放置在靠近相關表單控件的位置，並適當佈置。** 適用於表單內容。
> 
>確保標籤視覺上靠近關聯的表單欄位，避免大量的空白。
>除了單選按鈕與核取方塊，確保標籤在直式螢幕放置於表單欄位上方，橫式螢幕放置於表單欄位上方或左側。在直式與橫式螢幕，都將核取方塊與單選按鈕的標籤放在欄位的右側。 
>使用 CSS 表單布局，不要使用 HTML 表格作為目局目的。使用 CSS media queries 基於裝置螢幕大小重新定位內容。
>
> 期望：以下檢查正確
> • 螢幕上的控件是具有意義名稱的可見標籤，當移除上下文內容時，可描述控件的目的。
> • 標籤必須靠近欄位。  
> • 必須將標籤放置在螢幕佈局的有效位置:在直向畫面中置於欄位的上方 / 在橫向畫面中置於欄位的左側

**範例原始碼：**
```htmlembedded
無範例原始碼
```


**測試程序：**
1. 啟動應用程式並啟用放大到兩倍的縮放比例。 
2. 關注每個表單欄位。  
3. 驗證控件是否有視覺標記。  
4. 驗證標籤是否與控件緊鄰。
5. 驗證標籤放置於畫面佈局(直向或橫向)最有效位置。

###### 無障礙要求對應：3.3.2 標籤或說明(檢測等級 A)

---
### :pushpin: 【FM6】輸入提示 (選項)
> **在需要時，應提供輸入提示並可提供視覺和聽覺表現。** 適用於互動元件。
>確保所有頁面元件 皆提供無障礙的標籤。使用 label 屬性為表單控件提供單獨的標籤，使用 alt 屬性為圖片提供相等意義的文本。說明對所有使用者皆有助益，必須在頁面上視覺呈現。
>
> 期望：以下檢查正確
> • 表單提供說明。
> • 表提提供清楚說明，幫助使用者在填寫表單過程避免與防止錯誤。
> • 具動作的物件/控件/元件提供標籤或說明，指出當該項目啟動時將執行的動作。

**成功範例原始碼：**
```htmlembedded=
<!-- provide a label for instructions for screen reader users -->

<label for="firstName">First name
    <span aria- hidden="true">(required)</span>
</label>

<input id="firstName" type="text" aria- required="true">
```

**失敗範例原始碼：**
```htmlembedded=+
<!-- no instructions for screen reader users -->  
<input type="text" id="s1" /> <button>Go</button>

<!-- no indication of what an asterisk means --> 
<label for="email">*Email: </label>
<input type="text" id="email" aria- required="true" />
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 找到所有表單或可動作的項目。  
3. 驗證頁面或物件/元件/控件包含說明，解釋如何完成表單或物件/元件/控件將執行的操作。
4. 驗證說明足夠清楚，避免與防止使用者執行錯誤。

###### 無障礙要求對應：3.3.5 協助(檢測等級 A)

---
## :books: 互動組件: (四) FM 表單
1. 期望：
    • 通過文字充分描述鏈結，按鈕或導航項，清楚地表明其目的
    • 螢幕報讀軟體只會報讀一次，同時帶有圖片和文字標籤的物件，元件和控件
    
2. 檢測程序
    (1)啟動螢幕報讀軟體。
    (2)找到鏈結、按鈕或導航項目。 
    (3)確定鏈結或項目本身是否足以唯一地描述組件並清楚地指出其目的。

![](https://i.imgur.com/xbh5tBY.png)


### :pushpin: 【LK1】描述式鏈結 (必要)
> **鏈結和導航文字必須唯一地描述鏈結或項目的目標或功能。** 適用於鏈結內容。
>
> 使用螢幕外的文字識別頁面中具有相同可見文本的鏈結。例如，如果頁面含有 2 個”編輯” 按鈕，一個用於編輯電子郵件地址， 一個用於編輯電話號碼，可採取範例之方法。
>
> 期望：通過文字(在螢幕上或螢幕外)或替代文字可以充分描述鏈結、按鈕或導航項目，以清楚地指出其目的。
> 注意:使用螢幕報讀軟體可以最輕鬆地驗證螢幕外文字。如果文字創建正確，則螢幕報讀軟體會報讀該文字，但不會出現在螢幕上。

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basic/warning.png)HTML:由於不同的瀏覽器或輔助技術之間對角色衝突的解析，實作上會有差異，因此，某些元素可以具有“link”語義角色，某些技術中可能無法通過此規則，但是其他技術的使用者將不會遇到任何無障礙問題。
:::

**成功範例原始碼：**
```css=
<style> 
    .visually-hidden {
        clip: rect(1px 1px 1px 1px); /* IE 6/7 */ 
        clip: rect(1px, 1px,1px, 1px); 
        -webkit-clip-path:inset(50%) ! important;
        clip-path: inset(50%) ! important;
        height: 1px;
        overflow: hidden; 
        position: absolute; 
        white-space:nowrap; width: 1px;
    } 
</style>
```
```htmlembedded=+
<p>
    <a href="...">Edit <span class="visually- hidden">email address</span></a>
</p>

<p>
    <a href="...">Edit <span class="visually- hidden">phone number</span></a>
</p>
```
**失敗範例原始碼：**
```htmlembedded=+
<p>Content 1 title and description.
    <a href="page1.html">More</a> 
</p>

<p>Content 2 title and Rule description.
    <a href="page2.html">More</a> 
</p>

<p>Content 3 title and Rule description.
    <a href="page3.html">More</a> 
</p>
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 找到鏈結、按鈕或導航項目。  
3. 確定鏈結或項目本身是否足以唯一地描述組件並清楚地指出其目的。

###### 無障礙要求對應：2.4.4 鏈結目的(脈絡)(檢測等級 A)

---
### :pushpin: 【LK2】合併重複的鏈結 (必要)
> **必須將到同一組件的重複鏈結合併成單個鏈結。** 適用於鏈結內容。
> 將需要替代文字但帶有冗餘關聯文字鏈結的圖片放入一個錨元素，並將 alt 圖片的屬性設置為 null(alt="")。
>
> 期望：
> • 具有圖片和文字標籤的物件、元件和控件，僅 宣告一次。
> • 具有圖片和文字標籤的物件、元件和控件的分 組方式，僅使它們宣告為一個組件。

**成功範例原始碼：**
```htmlembedded=
<a href="..."><img src="search.jpg" alt=""/>Search</a>
```
**失敗範例原始碼：**
```htmlembedded=+
<a href="...">
    <img src="search.jpg" alt="Search"/>
</a>

<a href="...">Search</a>
```

**測試程序：**
1. 啟動螢幕報讀軟體。
2. 確認具有文字和圖片組件的活動螢幕物件、元件和控件。 
3. 導航到此項目。  
4. 驗證沒有報讀兩次文字。  
5. 驗證每個項目沒有報讀兩個相同意義執行方法。

###### 無障礙要求對應：2.4.4 鏈結目的(脈絡)(檢測等級 A)

---
### :pushpin:【LK3】鏈結目的格式 (選項)
> **告知使用者將要使用不同行動化應用軟體開啟。** 適用於鏈結內容。
> 
> 期望：
> • 該應用程式提供一個可供所有使用者訪問的介面。  
> • 警告和鏈結提供替代方法。

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basic/warning.png)HTML:此規則假定輔助技術無論它們位於哪個文檔樹中，都以相同的方式公開頁面上的所有鏈結。
:::

**範例原始碼：**
```htmlembedded
無範例原始碼
```
**測試程序：**
1. 開啟應用程式。  
2. 點擊非網頁超連結，如:信箱、電話、文件檔案。 
3. 確認在跳轉到其他應用程式前有提示視窗或文字。

###### 無障礙要求對應：2.4.4 鏈結目的(脈絡) (檢測等級 A)

---
## :books: 互動組件: (五) DC 動態內容
1. 期望：
    • 避免動態內容的閃爍造成癲癇、痙攣等身體不適的反應
    • 當螢幕包含動態更新，移動，閃爍的滾動內容或動畫時，可以使用方法來停止，隱藏，暫停或控制內容
    • 螢幕內容不會自動重整或改變，或者焦點在物件、元件或控件之間移動時不會自動重整或改變
    
2. 檢測程序
    (1)瀏覽內容，驗證螢幕不會自動重整或改變。 
    (2)確認頁面/螢幕上內容閃爍的位置。 
    (3)使用閃爍測試儀(Flicker Tester)將相機靠近光源。 
    (4)儲存閃爍曲線指數、頻率與閃爍百分比。
    (5)驗證是否符合閃爍要求或提供警告與開關按鈕。
    
 ![](https://i.imgur.com/y88HId9.png)


### :pushpin: 【DC1】禁止閃爍 (必要)
> **動態內容不得明顯或有意地在任何一秒鐘中閃爍三遍。** 適用於動態內容。
>
> 期望：以下檢查正確
> • 提供警告與關閉按鈕。 
> • 內容通過閃爍測試要求。

**範例原始碼：**
```htmlembedded
無範例原始碼
```
**測試程序：**
1. 確認頁面/螢幕上內容閃爍的位置。  
2. 使用閃爍測試儀(Flicker Tester)將相機靠近光源。 
3. 儲存閃爍曲線指數、頻率與閃爍百分比。  
4. 驗證是否符合閃爍要求或提供警告與開關按鈕。

###### 無障礙要求對應：2.3.1 閃爍三次或低於閾值(檢測等級 A)

---
### :pushpin: 【DC2】動態內容控制 (必要)
> **更新媒體或動畫內容必須具有暫停，停止或隱藏控件。** 適用於動態內容。
> 使用 HTML5 video 元素用於如影片的媒體內容。確保提供 controls 屬性用於控制播放，或使用具有無障礙控件的媒體播放器。對於自定義螢幕上的動畫，如新聞報導收錄器與自動輪播， 應隨同上一個與下一個按鈕提供停止按鈕。
>
> 期望：以下檢查正確
> • 當螢幕包含動態更新、移動、閃爍的滾動內容 或動畫時，可以使用一種方法來停止、隱藏、暫停或控制內容。
> • 該方法可讓輔助技術使用。
> • 裝飾內容動畫的持續時間不超過五秒鐘。

**成功範例原始碼：**
```htmlembedded=
<h2>Story headline</h2> 
<div>Story content</div>
<div>
    <button style="float:left;">Prior story</button> 
    <button style="float:left;">Pa use</button>
    <button style="float:left;">Ne xt story</button>
</div>
```

**失敗範例原始碼：**
```htmlembedded=+
<h2>Story headline</h2> <div>Story content</div>
```
**測試程序：**
1.  啟動應用程式。 
2.  確定螢幕上是否包含動態更新、移動、閃爍的滾動內容或動畫。
3.  確定是否具有停止、隱藏、暫停或控制內容的控件。    
4.  驗證控件是否以指定的方式正確控制媒體。
5.  驗證可以通過輔助技術使用控件，並且可以使用輔助技術控制動態內容。
6.  驗證裝飾性動畫內容的持續時間不超過五秒鐘。


###### 無障礙要求對應：2.2.2 暫停、停止和隱藏 (檢測等級 A)

---
### :pushpin: 【DC3】懸浮內容 (必要)
> **指標懸停時觸發的附加內容可由使用者移除或移動， 指標可以在附加內容上移動，而且原內容不會消失。** 適用於動態內容。
>
> 期望：懸浮內容須可移動、開啟、關閉。

**範例原始碼：**
```htmlembedded
無範例原始碼
```
**測試程序：**
1. 開啟應用程式。  
2. 確認焦點可遊走至懸浮內容並讀取，其背景下程序不會因為懸浮內容消失。  
3. 確認遊走懸浮內容不會自動更新或閃退。 
4. 確認懸浮內容可由使用者關閉。

###### 無障礙要求對應：1.4.13 懸浮或焦點內容 (檢測等級 AA)

---
### :pushpin: 【DC4】頁面更新 (必要)
> **不得在沒有警告的情況下使用自動頁面重整。** 適用於動態內容。
>不要使用 setTimeout 更新頁面的 href 屬 性，也不要將 meta標記的 http-equiv 屬 性值設定為 refresh。
>
> 期望：以下檢查正確
> 螢幕內容不會自動重整或改變，或者焦點在物件、元 件或控件之間移動時，不會自動重整或改變。


**成功範例原始碼：**
```htmlembedded=
<head>
    <title>This is appropriate</title>
</head> 

<body>
    <p>Please reload this page!</p>
    <a href="...">Reload Page</a>
</body>
```

**失敗範例原始碼：**
```htmlembedded=+
<body onload=setTimeout("location.href='http://w ww.bbc.com'", 5000)>
    <p>...Information...</ p>  
</body>

<!-- or --> 
<head>
    <title>Don't use this!</title>
    <meta http-equiv="refresh" content="5; http://www.example.c om/newpage">
</head>

<body>
    <p>If your browser supports Refresh, you'll be transported to our
        <a href="http://www.exa mple.com/newpage"> new site</a>in 5 seconds, otherwise,select the link manually.
    </p>
</body>
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 瀏覽所有內容。  
3. 驗證整個螢幕沒有重整或更新。

###### 無障礙要求對應：2.2.2 暫停、停止和隱藏(檢測等級 A)
---

### :pushpin: 【DC5】超時 (必要)
> **時間限制的回應必須可調整。** 適用於動態內容。
> 初始使用提醒時間限制是否關閉或延長時限，可通過此檢核點。
> 使用 JavaScript 的 setTimeout 方法設定時間限制，並使用 confirm 函式讓使用者在應用程式超時前至少 20 秒，可延長所需的時間。
>
> 期望：以下檢查正確
> •當表單或活動有時間限制時，使用者可關閉時間限制功能。
> •使用者可以請求更多時間來完成表單/活動。 
> •使用者可以在超時前修改延長足夠的時間。

**成功範例原始碼：**
```javascript=
<head> 
    <script>
        var sessionTime;
        function setTimer() {
            // [N] = the session time in seconds, less twenty seconds.
            sessionTime = setTimeout("displayTi meoutAlert()", [N]);
        }
        
        function displayTimeoutAlert() {
            var sessionChoice = confirm("Your session is about to expire. Do you require more time?")
            if (sessionChoice == true) {
                sessionTime = setTimeout("displayTimeoutAlert()", [N]); } else {
                alert("Your session has ended.Please log in again.");
            } 
        }
    </script> 
</head>
```
```htmlembedded=+
<body onload="setTimer();">
    ... 
</body>
```

**失敗範例原始碼：**
```javascript=+
<head> 
<script type="text/javascript" >
    var time ; //global to keep track of time
    function setTimer() {
        time = setTimeout("displayAert()"，300000); 
    }
    function displayAlert() {
        alert("Your session has ended");
    }
</script>
</head> 
```
```htmlembedded=+
<body onload="setTimer();" >
    ... 
</body>
```

**測試程序：**
1.  啟動應用程式。
2.  確定應用程式是否包含必須在指定時間內完成的表單或活動內 容。   
3.  驗證該應用程式允許使用者執行以下操作之一: 
    • 在發生超時之前將其取消 
    • 延長當前活動階段的時間  
    • 增加時間限制  
4.  驗證是否在超時至少 20 秒前警告使用者。    
5.  驗證是否警告操作期間輸入的任何數據將在超時時被刪除。  
6.  驗證使用者使用替代輸入方式可以接續或延長時間。


###### 無障礙要求對應：2.2.1 計時調整 (檢測等級 A)

---
## :books: 互動組件: (六) ST 結構
1. 期望：
    • 每個頁面/螢幕必須具有唯一的上下文相關標題
    • 所有複合物件、元件和控件需有整體描述的聲明，如滑塊控件應顯示為滑塊，而不是向上按鈕、向下按鈕和指示器

2. 檢測程序
    • 對於 HTML，必須由螢幕報讀軟體報讀一個獨特的 title 元素。
    • 對於 Android 和 iOS，標題必須出現在螢幕頂部，並由螢幕報讀軟體報讀。
    
![](https://i.imgur.com/GmkY3eL.png)

    
### :pushpin: 【ST1】單一頁面標題 (必要)
> **所有頁面或螢幕標題必須唯一且清晰可辨。** 適用於結構與標題內容。
> 使用 title 元素提供每個 HTML 頁面個別的頁面標題。頁面標題通常應使用與頁面上主要層級標題(h1)的文字相同， 但此將取決於應用程式與頁面本身的上下文脈絡，故此非強制性。
>
> 期望：以下檢查正確
> 每個頁面/螢幕必須具有唯一的上下文相關標題:
>  •對於 HTML，螢幕報讀軟體會顯示並報讀唯一性 的 title 元素。
>  •對於 Android 和 iOS，標題會顯示在螢幕頂部，並 由螢幕報讀軟體報讀。

**成功範例原始碼：**
```htmlembedded=
<html lang="en"> ...
    <title>BBC Weather</title>
    ... 
</html>
```

**失敗範例原始碼：**
```htmlembedded=+
<title>BBC</title>
```

**測試程序：**
1. 檢查網站/應用程式上每個頁面/螢幕的標題。 
2. 驗證標題是否存在:
    •對於 HTML，必須由螢幕報讀軟體報讀一個獨特的 title 元素。
    •對於 Android 和 iOS，標題必須出現在螢幕頂部，並由螢幕報讀軟體報讀。

###### 無障礙要求對應：2.4.2 網頁標題 (檢測等級 A)
---

### :pushpin: 【ST2】分組元件 (必要)
> **可控元件，以分組進行呈現時，聚焦宣告須表示為同一整體結構，非單一控件。**適用於結構與標題內容。
>
> 使用原生 HTML 和 相關的 WAI-ARIA 分組標記對相關控件進行分組。例如使用:
    • fieldset 和 legend 元素將相關的表單控件分組。
    • figure 和 figcaption 元素將圖片和相關標題分組。
    • nav 元素對導航鏈結進行分組。使用列表標記將相關(非格式)項目的列表分組。在 WAI-ARIA 方面，使用頁籤面板標記語法來標記頁籤導航插件。使用 tree view 標記語法來標記可擴展/可折疊的樹狀插件。使用工具欄標記語法將相關的樣式控件 (例如:粗體、斜 體和下劃線)分組。
>
> 期望：以下檢查正確
> 所有複合物件、元件和控件都不表示單個元件，而是聲明為一個整體。

**成功範例原始碼：**
```htmlembedded=
<fieldset>
    <legend>Billing address</legend>
    <label for="billing- street">Street</label>
    <input type="text" id="billing-street">
    <label for="billing- city">City</label>
    <input type="text" id="billing-city">
    <label for="billing- county">Country</label>  
    <input type="text" id="billing-county"> <label for="billing-postcode">Postcode</ label>
    <input type="text" id="billing-postcode"> 
</fieldset>

<fieldset>
    <legend>Delivery address</legend>
    <label for="delivery-street">Street</label> 
    <input type="text" id="delivery-street">
    <label for="delivery-city">City</label> 
    <input type="text" id="delivery-city"> 
    <label for="delivery- county">Country</label>
    <input type="text" id="delivery-county"> 
    <label for="delivery- postcode">Postcode</label>
    <input type="text" id="delivery- postcode">
</fieldset>
```

**失敗範例原始碼：**
```htmlembedded=+
<!-- Example 1 - tabs -->  
<ul>
    <li><a href="#s1" class="selected">Read</a></li>
    <li><a href="#s2">Watched</a></li>
</ul>
<section id="s1" class="showing">...</section>  
<section id="s2">...</section>

<!-- Example 2 - figure with caption-->  
<img src="clouds.jpg" alt="cloudy" ... /> 
<img style="position:relative; left:-10px;" src="sun.jpg" alt="sunny" ... />

<p>Partly sunny</p>

<!-- Example 3 - tree view -->  
<ul>
    <li><img src="expanded.jpg" alt="expanded" /><a href="...">TV Shows</a><span class="offscrn"> level 0</span></li>
</ul>
```

**測試程序：**
1.  啟動螢幕報讀軟體。  
2.  識別頁面上的所有複合物件、元件和控件。    
3.  驗證複合物件、元件和控件是否在適用的情況下作為一個單元宣告，例如滑塊控件應顯示為滑塊，而不是向上按鈕、向下按鈕和指示器。


###### 無障礙要求對應：4.1.1 語法分析 (檢測等級 A)

---

### :pushpin: 【ST3】標頭 (選項)
> **內容必須提供平台支援的邏輯和分層標頭結構。** 適用於結構與標題內容。
>==使用標頭(h1-h6)元素將內容結構化， 確保每個頁面僅有 1 個 h1，且彥標頭結構上沒有落差(如沒有 h2，即不使用 h3)==
>
> 期望：以下檢查正確
> •所有視覺標頭/表頭元素均表示為標頭/表頭(在作業平台的限制內); 
> •所有表頭均採用邏輯結構(僅 HTML 內容)。

**成功範例原始碼：**
```htmlembedded=
<h1>The United Kingdom</h1>
<h2>England</h2>
<h3>London</h3> ...
<h3>Birmingham</h3 >...
<h3>Manchester</h3 >... 
<h2>Northern Ireland</h2>
<h3>Belfast</h3> ...
<h3>Larne</h3> ...
<h3>Coleraine</h3> ...
<h2>Scotland</h2>
<h3>Edinburgh</h3> ...
<h3>Glasgow</h3> ...
<h3>Aberdeen</h3> ...
<h2>Wales</h2> 
<h3>Cardiff</h3>...
<h3>Swansea</h3> ...
<h3>Rhyl</h3> ...
```

**失敗範例原始碼：**
```htmlembedded=+
<div class="heading">Local Weather</div>
<divc lass="subheading">T oday's Forecast</div>
<div class="subheading">T omorrow Forecast</div>
<div class="subheading2"> Tomorrow's Allergy Forecast</div>
```
**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 檢查每個頁面/螢幕並找到任何視覺標頭/表頭。  
3. 確定標題/標題在平台中是否可能。  
4. 驗證是否有實際的標題。  
5. 驗證標題/標題是由螢幕報讀軟體宣布的。  
6. 驗證所有標頭均已具邏輯結構。這僅適用於 HTML 內容。

###### 無障礙要求對應：2.4.10 區段標題 (檢測等級 AAA)

---
### :pushpin: 【ST4】容器與地標 (選項)
> **容器應用於描述平台支援的頁面/螢幕結構。** 適用於結構與標題內容。該檢核點排除 Android 版本。
> :::info
> 使用 ARIA 地標角色或 HTML5 區段元素指出常見的頁面內容區段(例如主要內容區、導航、頁頭與頁尾)。 
> 
> WAI-ARIA 地標角色包括: 
> banner、navigation、 search、main、comp lementary、article、s ection、contentinfo。 
> 
> HTML5 元素包括: 
> header、nav、main 、aside、article、sec tion、footer。這些元素具有預設的地標角色，不需要設置 ARIA 角色屬性。
> :::
>
> 期望：以下檢查正確
> 頁面由適當的容器構成: 
    •HTML 頁面宣告頁面各部分的適當容器具有 ARIA 等效地標。
    •iOS 頁面容器可以作為地標並可導航。 •Android 頁面容器可以作為地標並可導航。



**成功範例原始碼：**
```htmlembedded=
<div id="header" role="banner">
    <div id="navigation"role="navigation">
        <ul>
            <li><a href="...">Home</a></li>  
            <li><a href="...">About Us</a></li>
            <li><a href="...">Contact Us</a></li>
        </ul>
    </div>
</div>

<div id="mainContent" role="main">
<h1>Home</h1>
...
```

**失敗範例原始碼：**
```htmlembedded=+
<div id="header">
    <div id="logo">...</div>
    <h1>BBC</h1>
    <div id="nav"> 
        <ul>
            <li>Weather</li>
            <li>Sport</li>
            <li>Travel</li>
        </ul>
    </div>
</div>

<div id="content">...</div>  
<div id="related- content"> ...</div>
<div id="footer">
    <p>BBC 2012</p>
    <ul> ... </ul> 
</div>
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 驗證使用容器將頁面結構化:
    •對於 HTML 頁面必須具有適當的區段元素，或非語義容器具 有 ARIA 地標角色，對於頁面的每個部分具有等效的 ARIA 地標。
    •對於行動 Safari 中的 HTML 頁面，必須透過在“指針 (Rotor)”選單中選擇“地標”來導航具有等效 ARIA 地標的頁 面的每個部分。
    •對於行動 Chrome 中的 HTML 頁面，必須透過在本機上下文 選單中選擇“標頭和地標”來導航具有等效 ARIA 地標的頁 面的每個部分。


###### 無障礙要求對應：1.4.10 流動排版 (檢測等級 A)

---
## :books: 設計方式: (一) AD 可調適設計
1. 期望：
    • 內容以有意義的順序宣告
    • 當行動裝置變更螢幕方向時，可以立即調適內容呈現方向

2. 檢測程序
   (1)啟動螢幕報讀軟體。 
   (2)使用標準命令導航下一個和上一個。 
   (3)驗證內容按照有意義的順序報讀。
    
![](https://i.imgur.com/K378ujn.png)

    
### :pushpin: 【AD1】內容順序 (必要)
> **內容順序必須符合邏輯順序。** 適用於可調式設計內容。
>螢幕報讀軟體按照 在文檔物件模型 (DOM)中出現的順序傳遞頁面內容。
>因此，確保頁面以有意義的順序結構化，亦即報讀與頁面的編碼順序匹配。
>
>例如: 確保頁面的頁尾出 現在 HTML 文檔的尾端，不要將它放在 HTML 的頂端而使用 CSS 在視覺上定位在頁面的底部。不要使用 HTML 表格語法作為布局目的。避免使用大於0的 tabindex 值強制 tab 跳位順序，因在每次新頁面元素增加時滑動順序必須重新配置，所以僅在重新排序 HTML 順序不支援預期的滑 動順序時才採用此方法。
>
> 期望：以下檢查正確
> •以有意義的順序宣告內容。


**成功範例原始碼：**
```htmlembedded=
<div>Banner</div> 
<div>
    <div style="float:left;">
        <div><h1>Main story</h1></div>
        <div>Story content</div>
    </div>
    <div style="float:right;">S upplementary info</div>
</div>
```

**失敗範例原始碼：**
```htmlembedded=+
<div>Banner</div> 
<div> 
    <div><h1>Mainstory</h1></div> 
    <div style="position:relativ e; left:50%;top:- 50%;">
    Supplementar y info
    </div>
    <div>Story content</div> 
</div>
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 使用標準命令導航下一個和上一個。 
3. 驗證內容按照有意義的順序報讀。


###### 無障礙要求對應：1.3.2 有意義的序列 (檢測等級 A)

---

### :pushpin: 【AD2】螢幕方向 (必要)
> **確認內容可以響應設備變更螢幕方向。** 適用於可調式設計內容。
>
> 期望：以下檢查正確
> •當行動裝置變更螢幕方向(直向/橫向相互切換)時，可以立即調適內容呈現方向。

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1.  啟動應用程式。
2.  當行動裝置螢幕為直向時，確定應用程式可以調適內容呈現方向。
3.  當行動裝置螢幕為橫向時，確定應用程式可以調適內容呈現方向。


###### 無障礙要求對應：1.3.4 螢幕方向 (檢測等級 A)

---
### :pushpin: 【AD3】可調整設定 (選項)
> **互動式媒體(包括遊戲)應根據使用者的能力和偏好 進行可調。** 適用於可調適設計內容。適用於遊戲。
>
> 期望：以下檢查正確
> 以下可調整: 
> •音量 
> •文字尺寸 
> •內容尺寸
> •顏色 
> •遊戲難易程度 
> •超時

**範例原始碼：**
```htmlembedded
無範例原始碼
```
**測試程序：**
1. 確認應用程式依賴特定感知的區域。 
    •驗證音量可調整 
    •驗證文字尺寸可調整 
    •驗證內容尺寸可調整 
    •驗證顏色可調整 
    •驗證遊戲難易程度可調整 
    •驗證超時可調整

###### 無障礙要求對應：

---
## :books: 設計方式: (二) DT 可辨識設計
1. 期望：
    • 可以從視覺上區分可操作項目和不可操作項目
    • 對於非粗體的標準字體，文字母和背景之間的對比度滿足WCAG 2.0 要求的最小彩色對比度為 4.5:1
    • 更改畫面比例後，不會遺失資訊
    • 調整大小後，內容可以正確重排
    

2. 檢測程序
    (1)啟動螢幕報讀軟體。
    (2)找出所有可操作的項目。 
    (3)驗證可以從視覺上區分可操作項目和不可操作項目。 
    (4)驗證螢幕報讀軟體可指出可操作狀態。
    
![](https://i.imgur.com/Op7b0DK.png)

    
### :pushpin: 【DT1】可操作元件 (必要)
> **鏈結和其他可操作元素必須清楚區分。** 適用於。
> 使用原生 HTML 元 素於可操作控件， 而不是重新調整其 他元素的用途，因 為必要的語意與行 為已預設內建。按 鈕使用 button 元素， 鏈結使用 a 元素，表單控件使用 input 元 素等。再者，原生 控件給使用者習慣 的樣貌，當使用 CSS 調整頁面元素樣式 時，確保樣式不會 影響頁面元素的意 圖，例如，確認按 鈕具有視覺的外 觀，以暗示按鈕可 點擊而非純文本。
>
> 期望：以下檢查正確
> •可以從視覺上區分可操作項目和不可操作項目。 
> •可操作項目報讀的方式，指出可被螢幕報讀軟體操作。

**成功範例原始碼：**
```htmlembedded=
<button onclick="...">I am a button</button>  
<a href="...">I am a link</a>
```
OR

```htmlembedded=
<!-- Link with a background that will stand out from surrounding content,and button with a pointer cursor: -->
<a href="/">Home</a>
<button type="submit">Search</button>
```
```css=
<style>
    body {
        background: #fff;
    }

    a{  
        background: #def;
    }

    button {  
        cursor: pointer;
    } 
</style>
```

**失敗範例原始碼：**
```htmlembedded=+
<a href="/">Home</a>
```

```css=+
<style> 
    a{
        cursor: text;
        text-decoration: none;
    }
</style>
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 找出所有可操作的項目。  
3. 驗證可以從視覺上區分可操作項目和不可操作項目。 
4. 驗證螢幕報讀軟體可指出可操作狀態。


###### 無障礙要求對應：2.4.9 鏈結目的(僅鏈結) (檢測等級 A)

---

### :pushpin:【DT2】文字對比 (必要)
> **小文字(小於 18 點標準/14 點粗體)需符合 4.5:1**
> **大文字(大於 18 點標準/14 點粗體)需符合 3.0:1** ，適用於可辨識設計內容。
>• 對於文字或文字圖片，避免背景顏色或使用背景顏色相對前景顏色有足夠的對比度。
>• 如果使用背景顏色，則前景顏色需使用 4.5:1 的對比度。
>
> 期望：以下檢查正確
> • 一般文字與文字圖片對比度至少4.5:1以上。  
> • 大文字，至少18pt(24px)或14pt(18.66px)粗體字，對比度至少 3:1 以上。

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basic/warning.png)HTML:不同的瀏覽器對 CSS 的支持程度不同。可 能會導致一種瀏覽器中沒有出現的對比度問題。因 此，根據所使用的瀏覽器，此規則可能會產生不同 的結果。例如，使用 CSS 變換定位的文本可能在不支持 CSS 變換的瀏覽器中處於不同的背景。
:::

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1. 啟動應用程式。  
2. 找到具有背景顏色的文字樣本與僅由顏色標識的鏈結。 
3. 驗證顏色值:
-   螢幕截圖。
-   將圖片透過電子郵件發送或同步到電腦。
-   查看要測試的頁面的圖片。  
-   使用滴管工具確定內容的前景色和背景色，以獲取背景色和   
    前景色的顏色值。
4.  手動檢查元素的顏色定義。   
5.  使用可靠的工具(例如 Snook.ca 顏色對比檢查，Webaim 顏色    
    對比檢查器、TPG 顏色對比分析器或 Android 無障礙掃描工  
     具)來檢查對比度是否足夠。    
6.  將前景和背景值輸入到色彩對比分析器中。   
7.  驗證是否滿足亮度要求，並且顏色對比度符合標準尺寸和非粗  
    體文字的最小比例 4.5:1。


###### 無障礙要求對應：1.4.3 對比值(最小) (檢測等級 AA)

---

### :pushpin: 【DT3】調整文字尺寸 (必要)
> **確認文字可以放大到200%而不會失去內容或功能性。** 適用於可辨識設計內容。
> 
> 使用相對單位(ems) 指定字體與容器尺寸，採用響應式設計方法，將使頁面的布局依據裝置螢幕的尺寸進行調整。
避免將 maximum- scale=1.0 用於頁面的meta元素，因此作法將造成使用者無法使用雙指縮放手勢(注意:儘管從 iOS 10 開始，如果使用此屬性，使用者也將可以使用雙指縮放手勢)，正確做法如下:
>```htmlembedded=
><meta name=”viewport” content=”width=devic e-width, initial- scale=1.0”>
>```
>
> 期望：以下檢查正確
> •可以更改畫面比例而不會遺失對內容的瀏覽。 
> •尊重預設的文字大小。 
> •調整大小後，內容會正確重排並根據需要滾動。

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basic/warning.png)HTML:一些使用者代理將 aria-hidden 屬性值區分 大小寫。
:::

**成功範例原始碼：**
```htmlembedded=
<meta name="viewport" content="width=devic e-width, initial- scale=1.0">
```
```css=+
/* Resize content based on the viewport size: */
@media only screenand (min-width: 32em) {
    
    h1 {  
        font-size: 1.5em;
    }

    p{  
        font-size: 0.8em;
}

@media only screen and (min-width:50em) {
    h1 {  
        font-size: 2em;
    }
    
    p{  
        font-size: 1em;
    }
}
```

**失敗範例原始碼：**
```htmlembedded=+
<meta name="viewport" content="user- scalable=no" />
<meta name="viewport" content="width=devic e-width; initial- scale=1.0; maximum- scale=1.0; user- scalable=1;">
```
```css=+
<style> 
    body {
        overflow: hidden;
    } 
</style>
```
```htmlembedded=+
<iframe scrolling="no"></ifra me>
```
**測試程序：**
1. 開啟網頁或啟動應用程式。  
2. 驗證使用者介面可縮放。  
3. 驗證放大(縮小)後的內容仍然可以無障礙使用。 
4. 更改裝置預設文字大小。  
5. 驗證頁面/螢幕上文字調整大小並正確重排。  
6. 驗證未禁用滾動。

###### 無障礙要求對應：1.4.4 調整文字尺寸 (檢測等級 AA)

---

### :pushpin: 【DT4】非文字對比 (選項)
> **使用者介面元件和圖形物件內容的視覺呈現與相鄰顏 色的對比度至少為 3:1。** 適用於可辨識設計內容。
>
> 期望：非文字元件與相鄰元件或元素應可明顯區分。

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1. 啟動應用程式。  
2. 找到具有背景顏色的文字樣本與僅由顏色標識的鏈結。 
3. 驗證顏色值:
    • 螢幕截圖。  
    • 將圖片透過電子郵件發送或同步到電腦。  
    • 查看要測試的頁面的圖片。  
    • 使用滴管工具確定內容的前景色和背景色，以獲取背景色和前景色的顏色值。  
4. 手動檢查元素的顏色定義。  
5. 使用可靠的工具(例如 Snook.ca 顏色對比檢查，Webaim 顏色對比檢查器、TPG 顏色對比分析器或 Android 無障礙掃描工具)來檢查對比度是否足夠。  
6. 將前景和背景值輸入到色彩對比分析器中。
7. 驗證是否滿足亮度要求，並且顏色對比度符合標準尺寸和非粗體文字的最小比例 4.5:1。

###### 無障礙要求對應：1.4.11:非文字對比 (檢測等級 AA)

---

### :pushpin: 【DT5】流動排版 (選項)
> **確保內容響應設備螢幕大小自動調整，並避免二維捲軸。** 適用於可辨識設計內容。
>
> 期望：將內容放大到 300%以上時，使用者可以輕鬆閱讀內 容，而不必橫向滾動即可閱讀。

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basic/warning.png)桌上型電腦的瀏覽器會忽略視圖(viewport)meta 元 素，大多數現代的行動裝置瀏覽器默認會忽略視圖 (viewport)元素，或者具有可縮放的無障礙選項。此規 則與桌上型電腦的瀏覽器或大多數現代行動裝置瀏覽 器都不相關。只有使用舊版行動瀏覽器的使用者才能 遇到此規則測試的問題。
:::

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1.  啟動應用程式。 
2.  在全螢幕視窗上打開需要水平滾動的內容。   
3.  檢查內容中是否有選項可以切換到不需要使用者水平滾動以閱讀文字行的佈局。
4.  啟動該選項。    
5.  檢查以確保不需要水平滾動即可讀取任何一行文字。

###### 無障礙要求對應：1.4.10 流動排版 (檢測等級 AA)

---
## :books: 設計方式: (三) PD 可預期性設計 (必要)
1. 期望：
    • 所有內容、文字、文本圖片、音訊、視訊字幕和替代項均按照系統中設定的預期語言發布或顯示
    • 元件，控件和物件的視覺佈局與樣式可指示其操作動作
    • 執行相同的功能元件，控件和物件的視覺圖示及文字，具有一致性的說明及呈現

2. 檢測程序
    (1)設置作業系統語言。 
    (2)以作業系統標準輔助技術啟用的情況下啟動應用程式。 
    (3)驗證以下內容是否以正確的語言顯示或報讀:
    • 文字
    • 網站/應用程式不同語言的文字
    • 文字圖片
    • 網站/應用程式不同語言的文字圖片 • 標籤
    • 提示
    • 聲音
    • 影片字幕
    • 頁面和螢幕標題
    • 網站/應用程式不同語言的圖片、物件和元件的替代內容

![](https://i.imgur.com/s4O4kaM.png)
![](https://i.imgur.com/5mDg8kE.png)

### :pushpin: 【PD1】指示語言
> **指定頁面或應用程式的語言，並且必須指示語言的更改。** 適用於語言。
> 使用 html 元素上的 lang 屬性來指定頁面語言。並使用 lang 屬性指出頁面中語言的變更。
>
> 期望：根據指示語言使閱讀軟體可正確閱讀出頁面內容。


**成功範例原始碼：**
```htmlembedded=
<!-- HTML -->
<html lang="en">

<!-- XHTML -->
<html xmlns="http://www.w 3.org/1999/xhtml"lang="en" xml:lang="en">
<p>Language options:</p>
<ul> 
    <li><a href="...">English</a ></li>
    <li><a href="..."><span lang="es">Español</s pan></a></li>
</ul>
```

**失敗範例原始碼：**
```htmlembedded=+
<!-- HTML -->
<html>
<!-- XHTML -->
<html xmlns="http://www.w3.org/1999/xhtml">
    <div>
        <h2>Upcoming Spanish Holidays</h2> 
        <p>Les Fogueres de Sant Joan.</p> 
    </div>
</html>
```

**測試程序：**
1. 設置作業系統語言。  
2. 以作業系統標準輔助技術啟用的情況下啟動應用程式。 
3. 驗證以下內容是否以正確的語言顯示或報讀:
    • 文字  
    • 網站/應用程式不同語言的文字  
    • 文字圖片  
    • 網站/應用程式不同語言的文字圖片 • 標籤  
    • 提示  
    • 聲音
    • 影片字幕  
    • 頁面和螢幕標題  
    • 網站/應用程式不同語言的圖片、物件和元件的替代內容

###### 無障礙要求對應：3.1.1 網頁語言 (檢測等級 A)

---

### :pushpin: 【PD2】一致的導覽 (必要)
> **除非使用者做出變更，否則在一組元件中，反覆出現 的導覽機制每次都要有相同的相對順序。** 適用於可預期內容。
>
>使用視覺樣式指出項目具操作性。鏈結應與靜態文字不同，例如，不同的字體粗細、輪廓或不僅僅依賴顏色的其他視覺樣式。
>使用標準元素而不使用自定義樣式將自動為鏈結和按鈕提供此功能，儘管在小螢幕上多個或長鏈結可能變得難以辨認。確保圖示、鏈結文字等具一致性，例如，如果鏈結至首頁是頁面上的”回 首頁”，應確保在其他頁面上稱為” 開始頁”。
>
>此外，如果特定的圖示在頁面上參照到”幫助”，則在其他面頁上就不能表示其他的涵義。
>
>
> 期望：以下檢查正確
> •元件、控件和物件的視覺佈局與樣式可指出其操作動作; 
> •元件、控件和物件的可操作狀態和目的可被報讀。

**成功範例原始碼：**
```htmlembedded=
<a href="..."> Next story</a> <button>Next story</button>
```

**失敗範例原始碼：**
```htmlembedded=+
<div onclick="openStory(); "> Next story </div>
```

**測試程序：**
1. 啟動螢幕報讀軟體。  
2. 瀏覽可操作的項目。  
3. 驗證元件、控件和物件的視覺佈局與樣式可指出其操作動作; 
4. 驗證元件、控件和物件的目的可被報讀。

###### 無障礙要求對應：3.2.3 一致的導覽 (檢測等級 AA)

---

### :pushpin: 【PD3】一致的識別 (必要)
> **具有相同功能性的元件，就要有一致的識別。** 適用於可預期內容。
> 響應式網站是確保 跨裝置間一致性的 最佳方法。如果創 建獨立的行動版本，盡可能重用已有的圖片、圖示、替代文字、按鈕、標誌圖徽，以及替代文字、標頭、表單標籤與頁面標題的編輯內容。
>
> 期望：以下檢查正確
> •在應用程式中兩次或多次使用的圖片執行相同的功能，具有相同的文字表示形式，並具有一致宣告的無障礙替代內容。
> •用於不同目的的圖片具差異性。

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1.  啟動螢幕報讀軟體。 
2.  導航到圖片表示的圖片、物件、元件或控件。   
3.  確保在整個應用程式中使用兩次或兩次以上的任何圖片執行相   
     同的功能，並具有相同的文字表示形式。    
4.  對每個代表不同功能的圖片，重複以上程序。

###### 無障礙要求對應：3.2.4:一致的識別 (檢測等級 AA)

---

### :pushpin: 【PD4】依請求變更 (選項)
> **只有當使用者提出請求時，才開始變更上下文，否則 就要有個機制來關掉這類變更。** 適用於可預期內容。該檢核點排除 Loading 頁面。
>
> 期望：請求變更後才可使上下文內容更新。

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1.  找到所有文字輸入表單欄位。
2.  更改每個表單欄位中的值。   
3.  檢查是否打開新視窗。  
4.  對於打開的任何新視窗，檢查是否包含錯誤訊息和關閉視窗的按鈕，以將焦點返回到初始表單元素。


###### 無障礙要求對應：3.2.5 依請求變更 (檢測等級 AAA)

---
## :books: 設計方式: (四) CP 相容性設計
1. 期望：
    • 保使用者在離線或支援不完整時仍有功能體驗
    • 可以順利切換到電話、簡訊、電子郵件正常操作，並可回到應用程式

2. 檢測程序
   (1)識別可能依賴於 JavaScript 的內容和功能。
   (2)在未支援 JavaScript 或停用 JavaScript 的裝置或行動瀏覽器、或輔助技術，執行應用程式或網站。 
   (3)驗證內容是否可用，或提供有關為何不可用的訊息。 
   (4)驗證功能是否可用。

![](https://i.imgur.com/haawyN8.png)
![](https://i.imgur.com/um83mtt.png)

### :pushpin: 【CP1】漸進式功能 (選項)
> **以漸進式方式構建應用程式和網站，以確保使用者在離線或支援不完整時仍有功能體驗。** 適用於相容性設計內容。
>
> 避免瀏覽器偵測的使用，取而代之，採取漸進式增強方法，藉由專注於基本結構與內容優先，然後在其上面增加更多的功能。
> 因此，舊版裝置的使用者仍可使用應用程式的基本元件、內容與功能， 而較新裝置地使用者，將獲取與其作業系統相關的進階功能。
> 更多細節，參考Cutting the Mustard for techniques to determine browsercapabilities。
>
> 期望：以下檢查正確
> • 所有內容在每個裝置與作業系統皆可取得。
> • 所有功能在每個裝置皆可取得，或當特定的功能未被裝置或作業系統支援時提供相等的功能。

**成功範例原始碼：**
```htmlembedded=
<!-- Example 1 -HTML content that does not rely on JavaScript or CSS enhancement to function -->
<a href="page2.html">Next Page </a>
```
```javascript=+
//Example 2 -Content that is displayed with or without JavaScript
<script>
    // embed game or media player
</script> 

<noscript>
    This content requires Javascript to be enabled.
</noscript>

// Example 3 -check if a Javascript method or property is available 
if("geolocation" in navigator) { ... }
```

```css=+
/* Example 4 - check if CSS rules are supported  */
@supports (display:flex) and (transition: . 5s) {
    .box { display: flex; transition: .5s; } 
}
```

**失敗範例原始碼：**
```htmlembedded=+
<!-- Example 1 - JavaScript based link-->  
<a onclick="nextPage();"\> Next Page </a>

<!-- Example 2 -content that is only available with JavaScript and no fall-back explanation -->
<script>
// embed game or media player
</script>
```

**測試程序：**
1.  識別可能依賴於 JavaScript 的內容和功能。
2.  在未支援 JavaScript 或停用 JavaScript 的裝置或行動瀏覽器、或輔助技術，執行應用程式或網站。 
3.  驗證內容是否可用，或提供有關為何不可用的訊息。
4.  驗證功能是否可用。


###### 無障礙要求對應：4.1:相容性

---

### :pushpin: 【CP2】功能切換 (選項)
> **和行動裝置原有的電話、簡訊、電子郵件等功能可相容切換。** 適用於相容性設計內容。
>
> 期望：以下檢查正確
> 可以順利切換到電話、簡訊、電子郵件正常操作，並可回到應用程式。

**範例原始碼：**
```htmlembedded
無範例原始碼
```

**測試程序：**
1. 啟動應用程式。  
2. 識別有列出需要操作電話、簡訊、電子郵件的元件。  
3. 檢查是否可以順利切換到電話、簡訊、電子郵件正常操作，並可回到應用程式。


###### 無障礙要求對應：4.1 相容性

---
## 參考資源
[國家通訊傳播委員會-無障礙網路空間服務網](https://accessibility.ncc.gov.tw/News/Category/43/1)
[行動化應用軟體無障礙檢測指引(110.03.24訂定)](https://www.rootlaw.com.tw/Attach/L-Doc/A040410001022600-1100324-1000-001.pdf)



<!-- 
### :pushpin: XX-XX 【XX】XXX
> ** ** 適用於。
>
> 期望：以下檢查正確


**成功範例原始碼：**
```htmlembedded=
```

**失敗範例原始碼：**
```htmlembedded=+
```

**測試程序：**

###### 無障礙要求對應：

---

:::warning
[:warning:](https://assets.hackmd.io/build/emojify.js/dist/images/basichttps://hackmd.io/5cwCrji1R4uol34lsEtt1A?both#/warning.png)
::: -->




