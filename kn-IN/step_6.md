## ಸುರುಳಿಯಾಕಾರದ ಮಾದರಿಗಳನ್ನು ರಚಿಸುವುದು

ಚೌಕಗಳು ಸಾಕು! ಕೆಲವು ವಿಭಿನ್ನ ಆಕಾರಗಳನ್ನು ರಚಿಸೋಣ ಮತ್ತು ಸ್ನೋಫ್ಲೇಕ್ ತರಹದ ಸುರುಳಿಯನ್ನು ಮಾಡಲು ಅವುಗಳನ್ನು ಪುನರಾವರ್ತಿಸೋಣ.

- ನಿಮ್ಮ ಚೌಕದ ಕೋಡ್ ಅನ್ನು ಈ ಕೆಳಗಿನವುಗಳೊಂದಿಗೆ ಬದಲಾಯಿಸಿ:
    
    ```python
    for i in range(2):
      elsa.forward(100)
      elsa.right(60)
      elsa.forward(100)
      elsa.right(120)
    ```
    
    ಇದು ಸಮಾನಾಂತರ ಚತುರ್ಭುಜ ಎಂಬ ಆಕಾರವನ್ನು ಬರೆಯುತ್ತದೆ. ನಿಮ್ಮ ಕೋಡ್ ಅನ್ನು save ಮತ್ತು run ಮಾಡುವ ಮೂಲಕ ಅದು ಹೇಗೆ ಕಾಣುತ್ತದೆ ಎಂಬುದನ್ನು ನೀವು ನೋಡಬಹುದು.
    
    ![](images/parallelogram.png)

ನೀವು ಲೂಪ್-ಗಳ ಒಳಗೆ ಇತರ ಲೂಪ್-ಗಳನ್ನು ಹಾಕಬಹುದು. ಇದು ನಮಗೆ ಒಳ್ಳೆಯ ಸುದ್ದಿ, ಏಕೆಂದರೆ ಸ್ನೋಫ್ಲೇಕ್ನಂತೆ ಕಾಣುವ ರೇಖಾಚಿತ್ರವನ್ನು ಸುಲಭವಾಗಿ ಮಾಡಲು ನಾವು ಇದನ್ನು ಮಾಡಬಹುದು.

- ನಿಮ್ಮ ಸಮಾನಾಂತರ ಚತುರ್ಭುಜಕ್ಕಾಗಿ `for i in range(2):` ಸಾಲಿನ ಮೇಲೆ, ಟೈಪ್ ಮಾಡಿ:
    
    ```python
    for i in range(10):
    ```
    
    ಈ ಲೂಪ್ ಎಷ್ಟು ಬಾರಿ ಚಲಿಸುತ್ತದೆ?

- ನಿಮ್ಮ ಕರ್ಸರ್ ಅನ್ನು ನಿಮ್ಮ ಕೋಡ್ ಅನುಕ್ರಮದ ಕೆಳಗಿನ ಸಾಲಿಗೆ ಸರಿಸಿ, ಮತ್ತು ನೀವು ಬರೆಯಲಿರುವ ಕೋಡ್ ಅನ್ನು **indent** ಗೆ ನಾಲ್ಕು ಬಾರಿ ಸ್ಪೇಸ್ ಬಾರ್ ಒತ್ತಿರಿ. ನೀವು ನಿರೀಕ್ಷಿಸಿದಂತೆ ನಿಮ್ಮ ಕೋಡ್ ಕಾರ್ಯನಿರ್ವಹಿಸುತ್ತಿದೆಯೆ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಲು Python'ನಲ್ಲಿನ ಇಂಡೆಂಟೇಶನ್ ಬಹಳ ಮುಖ್ಯ! ಈಗ ಟೈಪ್ ಮಾಡಿ:
    
    ```python
    elsa.right(36)
    ```

- ಏನಾಗುತ್ತದೆ ಎಂಬುದನ್ನು ನೋಡಲು ನಿಮ್ಮ ಕೋಡ್ ಅನ್ನು save ಮತ್ತು run ಮಾಡಿರಿ. ಈ ರೀತಿಯ ರೇಖಾಚಿತ್ರವನ್ನು ನೀವು ನೋಡಬೇಕು:
    
    ![](images/snowflake1.png)