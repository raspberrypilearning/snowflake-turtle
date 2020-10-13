## ಸ್ನೋಫ್ಲೇಕ್ ಅನ್ನುfunction ಬಳಸಿ ಸೆಳೆಯುವುದು

ನಿಮ್ಮ ಸಮಾನಾಂತರ ಚತುರ್ಭುಜ ಸ್ನೋಫ್ಲೇಕ್ ಚೆನ್ನಾಗಿದೆ, ಆದರೆ ಅದು ಸ್ನೋಫ್ಲೇಕ್ನಂತೆ ಕಾಣುತ್ತಿಲ್ಲ. ಅದನ್ನು ಸರಿಪಡಿಸೋಣ!

ಈ ರೇಖಾಚಿತ್ರಕ್ಕಾಗಿ, ನಾವು Turtle'ಅನ್ನು ವಿಂಡೋದ ಮಧ್ಯದಿಂದ ಸರಿಸಬೇಕಾಗಿದೆ. `penup()` ಮತ್ತು `pendown()` ಸೂಚನೆಗಳು ರೇಖೆಯನ್ನು ಎಳೆಯದೆ ಇದನ್ನು ಮಾಡಲು ನಮಗೆ ಅವಕಾಶ ಮಾಡಿಕೊಡುತ್ತವೆ, ಅಂದರೆ ಕಾಗದದಿಂದ ನಿಜವಾದ ಪೆನ್ನು ತೆಗೆದುಕೊಂಡು ಅದನ್ನು ಚಲಿಸುವಂತೆ.

- `colours` ಲಿಸ್ಟಿನ ಕೆಳಗೆ ಈ ಕೆಳಗಿನ ಸೂಚನೆಗಳನ್ನು ಟೈಪ್ ಮಾಡಿ:
    
    ```python
    elsa.penup()
    elsa.forward(90)
    elsa.left(45)
    elsa.pendown()
    ```

ಸ್ನೋಫ್ಲೇಕ್ನ ಒಂದು ಶಾಖೆಯನ್ನು ಬರೆಯಲು ಕೋಡ್ ಅನ್ನು ಬರೆಯೋಣ ಮತ್ತು ಅದನ್ನು **function** ಒಳಗೆ ಸಂಗ್ರಹಿಸೋಣ. ನಂತರ ನೀವು ಸಂಪೂರ್ಣ ಸ್ನೋಫ್ಲೇಕ್ ಅನ್ನು ರಚಿಸಲು ಅದನ್ನು ಪುನರಾವರ್ತಿಸಬಹುದು.

![branch](images/branch.PNG)

- `branch` ಎಂಬ function ವಿವರಿಸಲು ಟೈಪ್ ಮಾಡಿ:
    
    ```python
    def branch():
    ```

- ಸಮಾನಾಂತರ ಚತುರ್ಭುಜ ಸ್ನೋಫ್ಲೇಕ್ ಲೂಪ್ ನ ಕೋಡ್ ತೆಗೆದುಹಾಕಿ. `branch` function'ದೊಳಗೆ ಇಂಡೆಂಟ್ ಮಾಡಲಾದ ಕೆಳಗಿನ ಕೋಡ್ ಅನ್ನು ಸೇರಿಸಿ:
    
    ```python
    for i in range(3):
        for i in range(3):
            elsa.forward(30)
            elsa.backward(30)
            elsa.right(45)
        elsa.left(90)
        elsa.backward(30)
        elsa.left(45)
    elsa.right(90)
    elsa.forward(90)
    ```
    
    **ಗಮನಿಸಿ**: ಇಂಡೆಂಟೇಶನ್ ಮುಖ್ಯ ಎಂದು ನೆನಪಿಡಿ. ನಿಮ್ಮ ಎಲ್ಲಾ ಇಂಡೆಂಟೇಶನ್ ಸರಿಯಾಗಿದೆಯೇ ಎಂದು ಪರೀಕ್ಷಿಸಲು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಿ, ಇಲ್ಲದಿದ್ದರೆ ನಿಮ್ಮ ಕೋಡ್ ಕಾರ್ಯನಿರ್ವಹಿಸುವುದಿಲ್ಲ!

- `branch` function'ಅನ್ನು ಎಂಟು ಬಾರಿ **call** ಮಾಡಲು (ಇದರರ್ಥ ಅದನ್ನು ಚಲಾಯಿಸಲು) ಕೋಡ್‌ನ ಅಂತಿಮ ವೀಭಾಗದಲ್ಲಿ ಬರೆಯಿರಿ. ನಿಮ್ಮ ಕೊನೆಯ ಸ್ನೋಫ್ಲೇಕ್ನಂತೆ ನೀವು ಮತ್ತೆ ಲೂಪ್ ಅನ್ನು ಬಳಸಬಹುದು:
    
    ```python
    for i in range(8):
      branch()
      elsa.left(45)
    ```

- `elsa.color(random.choice(colours))` ಎಂಬ ಸೂಚನೆಯನ್ನು **ಕಾಮೆಂಟ್** ಮಾಡಲು ಅದರ ಮುಂಧೆ `#` ಹಾಕಿ. ಇದರರ್ಥ ಕಂಪ್ಯೂಟರ್ ಆ ಕೋಡ್ ಅನ್ನು ಬಿಟ್ಟುಬಿಡುತ್ತದೆ. ನೀವು ಆ ಸಾಲನ್ನು ಅಳಿಸಬಹುದು, ಆದರೆ ನಂತರ ನಿಮ್ಮ ಸ್ನೋಫ್ಲೇಕ್‌ಗೆ ಬಣ್ಣವನ್ನು ಸೇರಿಸಲು ನೀವು ಅದನ್ನು ಬಳಸಬಹುದು.

- ನಿಮ್ಮ ಕೋಡ್ ಅನ್ನು ಸೇವ್ ಮತ್ತು ರನ್ ಮಾಡಿ, ಸ್ನೋಫ್ಲೇಕ್ ನಿಮ್ಮ ಕಣ್ಣುಗಳ ಮುಂದೆ ಕಾಣಿಸಿಕೊಳ್ಳುತ್ತದೆ!

![](images/snowflake2.png)