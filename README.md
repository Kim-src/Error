<!-- Name -->
# <p align = center>😊 Error Master 😊</p>
<!-- Update Date -->
###### <p align = right>Update Date : December 15, 2023</p>

<br/>
<br/>

<!-- Title -->
## ✅ Python (Google Colab)
### "SyntaxError: (unicode error) 'unicodeescape' codec can't decode bytes in position 2-3: truncated \UXXXXXXXX escape"
###### 오류 발생일 : December 15, 2023

<br/>

### 🔔 상황 설명
> Google Colab에서 Python을 활용한 이미지 학습을 하는 중이었습니다.  
> 변수에 값을 대입하는 중에 위와 같은 SyntaxError가 발생하였습니다.  
> 해당 오류 내용은 아래와 같습니다.  
> 
> <br/>
>
> <p align = "center"><img src = "https://github.com/Kim-src/Error/assets/150884526/90dc5b2e-d889-45e3-8d63-baf43d27b1cf" width = "500px"></p>

<br/>


### 📌 해결 방법
> 


> <p align = "center"><img src = "https://github.com/Kim-src/Error/assets/150884526/b143f626-ba1f-43fe-b43e-e53b0ad67460" width = "500px"></p>
<br/>




***

<br/>
<br/>
<br/>

<!-- Title -->
## ✅ Python (Google Colab)
### "TypeError: 'str' object is not callable"
###### 오류 발생일 : December 11, 2023

<br/>

### 🔔 상황 설명
> Google Colab에서 여러 변수를 선언 및 값을 출력해가며 개발 언어를 학습 중이었습니다.  
> 그런데 변수 출력(print) 과정에서 갑자기 위와 같은 TypeError가 발생하였습니다.  
> 막 출력하려던 변수뿐만 아니라 이전에 이미 선언 및 출력을 마친 변수들까지 모두 오류 상황이 되었습니다.  
> 
> <br/>
> 
> <p align = "center"><img src = "https://github.com/Kim-src/Errors/assets/150884526/c361ba6a-49bf-4aa1-9e0a-79aca87ac743" width = "500px"></p>

<br/>

### 📌 해결 방법
> 오류가 발생된 코드 윗줄에 아래의 코드 한 줄을 기입한 결과 오류 상황이 해결되었습니다.
>
> ``` Python
> del print
> ```

<br/>

### 📌 오류 원인
> 가장 가능성 있는 오류 원인은 출력문(print)을 출력으로 활용하지 않았기 때문일 것입니다.  
> 아마도 아래와 같이 출력문을 변수로 잘못 활용 후 값을 할당했을 가능성이 있습니다.  
> 
> ``` Python
> print = 변수명
> print = myList
> print = myDictionary
> print = 153
> ```

<br/>

### 🎁 응용 학습
> 고의로 위와 같은 출력문을 변수로 사용하면 다시 "TypeError: 'OOO' object is not callable" 오류가 발생됩니다.  
>
> ``` Python
> Number = 4.5
> print = 4.5
> print(Number)
>
> "TypeError: 'float' object is not callable"
> ```
> 
> 마찬가지로 print 코드 상부에 ```del print```를 입력하면 프로젝트 내 출력문(print)이 다시 정상 작동되는 것으로 확인하였습니다.
>
> ``` Python
> del print
> Number = 4.5
> print(Number)
>
> "4.5"
> ```

<br/>
<br/>
<br/>
