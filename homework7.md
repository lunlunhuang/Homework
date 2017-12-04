## How to solve the Exposed Terminal Problem ?
- ### Exposed Terminal Problem : 暴露節點問題
![](ExposedTerminalProblem.png)
- 問題說明 :
   C 要傳送資料給D時，發現傳輸範圍內的B正在傳送資料給A（C是B的暴露節點），C就會延遲傳送（但這種延遲是不必要的），因為B傳送資料給A與C傳送資料給D並不衝突，因此這種因為聽到傳輸範圍內有節點在傳輸，而延遲傳輸就是暴露節點的問題(Exposed Terminal Problem)。

