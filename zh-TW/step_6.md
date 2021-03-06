## 創建螺旋的圖案

夠多的正方形了！ 讓我們製作一些不同的形狀，並重複它們來形成雪花狀的螺旋。

- 將您寫的正方形的程式碼替換為以下程式碼：
    
    ```python
    for i in range(2):
      elsa.forward(100)
      elsa.right(60)
      elsa.forward(100)
      elsa.right(120)
    ```
    
    這會繪製一個平行四邊形， 您可以保存並運行程式碼來查看它長得如何。
    
    ![](images/parallelogram.png)

您可以在迴圈函式內再放入其他迴圈函式， 這對我們來說是個好消息，因為我們就可以輕鬆地製作出看起來像雪花的圖形。

- 在這行`for i in range(2):`的上方替平行四邊形再加上：
    
    ```python
    for i in range(10):
    ```
    
    這個迴圈將會循環多少次？

- 移動您的游標到程式碼下方，然後按四次空白鍵來**縮排**您要編寫的程式碼。 縮排在Python中非常重要因為能確保您的程式如期地執行！ 現在輸入：
    
    ```python
    elsa.right(36)
    ```

- 儲存並執行您的程式碼來看發生了什麼事。 您應該會看到像這樣的圖形：
    
    ![](images/snowflake1.png)