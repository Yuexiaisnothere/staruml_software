# StarUML
# 南華大學-軟體工程 期中報告
<h3>11124131 陳毅倫 11124115 徐言宏<h3>
<h2>軟體工程 : 需求分析中的三個重要的圖例（用例、活動、時序）</h2>

<h1> 用例圖</h1>
<h3>用例圖包含兩個元素：角色和用例。</h3>
  
<h3>角色、用例之間的主要關系有：關聯、泛化、包含、拓展、依賴。</h3>
  
<h3>下面一用戶登陸系統為例進行介紹。</h3>

<h2> 關聯（角色-用例）</h2>
<h3>角色與用例之間用一條直線相連。如下圖：</h3>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/1.png)

<h3>表示用戶會用到登錄系統這個功能。</h3>

<h2>泛化（角色-角色 或 用例-用例）</h2>
<h3>子元素與父與元素之間用（子指向父的）箭頭連接。如下圖：</h3>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/2.png)

<h3>表示管理員、教師、學生三種角色都會用到登錄系統這個功能；且登錄系統有兩種方式：賬密登錄、微信登錄。</h3>

<h2> 包含（用例-用例）</h2>
<h3>基礎用例與包含用例之間用（基礎指向包含的）虛線箭頭連接。如下圖：</h3>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/3.png)

<h3>表示用戶在賬號登錄過程中，包括輸入賬號、輸入密碼、確認登錄等操作。</h3>

<h2> 拓展（用例-用例）</h2>
<h3>基礎用例與拓展用例之間用（拓展指向基礎的）“拓展” 箭頭連接。如下圖：</h3>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/4.png)

<h3>表示當用戶在登錄過程中忘記了密碼時，會需要用到忘記密碼的功能。</h3>
<h3>拓展用例是在特定條件出現時，才會被執行的用例。</h3>

<h2> 依賴（用例-用例）</h2>
<h3>用例與用例之間用一條直線相連。如下圖：</h3>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/5.png)

<h3>表示展示首頁功能的執行，需要登錄系統功能的完成。</h3>

<h1>活動圖</h1>
<h3>活動圖包含五個元素：開始、活動、判斷、執行順序、結束。元素及圖標如下圖：</h3>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/6.png)

<h3>除了上述五個元素外，還有需要用泳道來劃分不同對象（角色）的執行區域，各個對象都應該在自己泳道里進行自己部分的活動。</h3>
<h3>泳道如下圖：</h3>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/7.png)

<h3>我們以下述情景為例介紹活動圖的繪制：<h3>

1. 管理員登錄系統維護教師、班級、學生、課程、題庫、題庫中的題目等各類基礎信息。
2. 教師登錄系統添加考試信息，添加考試時可選題庫以隨機出題；發布考試；批改主觀題；查看學生考試情況。
3. 學生登錄系統查看、參與考試；考完後可查看考試詳情（得分等）。
<h3>活動圖如下：</h3>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/8.png)

<h3>活動圖在繪制或者閱讀時，通常都會遵循從上到下、從左到右的順序。</h3>

<h1>時序圖</h1>

<h2>時序圖包含四個元素：對象、生命線、控制焦點、消息。如下圖：</h2>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/9.png)

<h2>對象：具體可以指角色、對象、類等等。角色用小人表示；對象、類等用方框表示。</h2>
<h2>生命線：在時序圖中表示為從對象圖標向下延伸的一條虛線，表示對象存在的時間。</h2>
<h2>控制焦點：又稱為激活期，表示時間段的符號，在這個時間段內對象將執行相應的操作。</h2>
<h2>消息：在對象之間橫向傳遞的信息。</h2>
<h2>時序圖是一個二維圖，橫軸表示對象，縱軸表示時間，消息在對象之間橫向傳遞，依照時間順序縱向排列。類似這樣：</h2>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/9.png)

<h3>對象的左右順序並不重要，但是為了作圖清晰整潔，通常應遵循以下兩個原則：<h3>

1. 把初始化整個交互活動的對象放置在最左端。 
2. 把交互頻繁的對象盡可能的靠攏。
<h1>以學生參加考試並交卷為例展示時序圖：</h1>

![image](https://github.com/Yuexiaisnothere/staruml_software/blob/main/10.png)

<h1>總結</h1>

| 圖例           | 作用           |
| -------------- | ------------- |
| 用例圖         | 用於描述系統的參與者與系統之間的交互。<br>它展示了系統的功能或服務，說明了各個<br>參與者可以與哪些功能交互以及如何與這些<br>功能交互。  |
| 活動圖         | 用於描述系統中的業務流程或工作流。它展<br>示了不同活動之間的順序和條件關系，以<br>及在這些活動中涉及的對象（比如各個對象<br>的活動邊界）。  |
| 時序圖         | 用於描述對象之間的交互和消息傳遞順序。<br>它展示了系統中對象如何協同工作以完成<br>特定的任務或交互。  |

<h1>參考資料</h1>
<h2>資料來源 : https://segmentfault.com/a/1190000044497583</h2>
