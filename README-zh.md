# OpenUtau辭典編輯器
用於為 OpenUtau 建立和編輯 Aesthetic YAML 辭典的 python GUI 工具包 🥰😍
![ou dictionary editor  6D4460C](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/7e28a808-cd52-4c85-a4d0-f2166e32d750)
- 要使用此GUI 工具包，對於**`Windows`**，我建議使用便攜式**`.exe`** 文件，對於**`MacOs`** 和**`Linux`**，我建議使用* *`.pyw`** 檔案並使用 **`python 版本 3.10 及以上`** **`3.9 及以下版本`**未經測試，可能無法正常運作。
- 在 **`MacOs`** 和 **`Linux`** 安裝必要組件：
  ```
  pip install ruamel.yaml tk requests
  ```
---
## 📍 在這裏下載最新版本:
[![Download Latest Release](https://img.shields.io/github/v/release/Cadlaxa/OpenUtau-Dictionary-Editor?style=for-the-badge&label=Download&kill_cache=1)](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/releases)
---
# 功能
## 開啟/附加 YAML 辭典
![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/a0bf596e-01a9-4ec6-bbe2-0d2503972122)
- 透過點擊 **`[開啟YAML檔]`** 按鈕，您可以開啟預製的 OpenUTAU YAML 辭典，以便使用此 GUI 工具包直接編輯它們。 **`[追加YAML檔]`**按鈕的功能是合併多個YAML文件，以便使用者可以將它們合併在一起。
## 從頭開始建立 YAML 辭典
![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/4d4b6537-2622-4c2c-b13e-a9838037ee95)
- 您可以將字素和音素新增到手動輸入部分。 按 **`[新增條目]`** 按鈕會將它們新增至條目檢視器。 使用 **`[刪除條目]`** 按鈕或鍵盤上的刪除按鈕將刪除所選條目。 透過先點選條目，然後對其他條目進行「Shift」+鼠標左鍵，會將其反白顯示，以便使用者可以使用 **`[刪除條目]`** 按鈕或刪除鍵盤按鈕批次刪除條目。
- `注意：如果從頭開始建立辭典，請從 [選擇模板] 中選擇 yaml 模板`
## 使用 OpenUtau YAML 模板或自訂模板
![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/7079a076-8933-44e2-8428-939c52da749a)
- 使用 [選擇模板] ，使用者可以選擇 OpenUtau YAML 模板來建立辭典。 此外，使用者還可以新增自己的模板，將其放置在 **`[Templates]`** 資料夾中，以便 GUI 工具包將透過 templates.ini 識別這些檔案並使用它們來建立字典。
- `提示：如果您要從頭開始建立自訂辭典，請從模板資料夾新增模板，以便您可以在[模板選擇]上使用它並新增條目，如果您已經建立了自訂辭典，只需將它們匯入編輯器即可使用“目前範本”，以便將條目新增至目前匯入的 yaml 檔案中，並仍保留自訂符號`
## 對條目進行排序
![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/86e65879-9af1-4cda-af37-70b8c1cc40a6)
- 使用者可以按字母順序對條目進行排序 **`A-Z`** 或 **`Z-A`**
## 將 CMUdict 轉換為 OU YAML 辭典
![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/2ecf2317-435b-427a-8535-c53dc83150cd)
- 將 CMUdict.txt 轉換為功能性 OpenUTAU 詞典的函數。 請注意，CMUdict 不得有 **`;;;`**，否則 GUI 工具包會引發錯誤。
## 使用條目檢視器
![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/6f37b8d4-dff0-4408-9a20-954a245eeeea)
- 在條目檢視器中，使用者可以透過點擊、刪除、新增和排列條目來與條目互動。
- ### 點擊要編輯的條目
- ![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/2b85b200-d856-479f-840c-239ed4e2ecd5)
 - 使用者可以透過「Ctrl」+ 鼠標左鍵和「Shift」+ 鼠標左鍵來選擇檢視器中的多個條目。
- ### 拖曳條目以更改其位置
- ![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/470c74b9-aa64-4048-8ed2-6d29086ab50f)
 - 使用者可以拖放條目以手動更改其位置。
## 使用正規表示式函數
![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/65e78088-d2fe-4d32-9663-f1b0dc42d083)
- 使用者可以使用正規表示式搜尋和替換來取代字素或音素。
## Saving the YAML Dictionary
![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/aed1949e-caa1-4eba-9633-5dcfdbf50d94)
- 目前有 2 個儲存按鈕可將 YAML 字典儲存為以下格式：
 - 普通 OU YAML
 - ![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/fcf731ff-9d06-420e-8705-063314ceccc2)
 - Diffsinger 格式
 - ![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/20a075ef-b8b3-4d4c-a228-2b3d39736a09)
## 改變主題和顏色色調
![image](https://github.com/Cadlaxa/OpenUtau-Dictionary-Editor/assets/92255161/54450466-81e2-4e2f-9cc2-135d97602121)
- 使用者可以隨意更改 GUI 工具包的主題和顏色。 目前有 **`18`** 顏色可供選擇，與其 **`淺色`** 和 **`深色`** 主題相對應。
---
- 此 GUI 工具包的其他功能包括自動為字素和音素的特殊字元`' '`、淺色模式和深色模式主題、條目排序、刪除數字重音、使音素小寫等等。
