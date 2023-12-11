<!-- Introduction -->
# <p align = center>😊 Error Master 😊</p>

<!-- Update Date -->
###### <p align = right>Update Date : December 11, 2023</p>

<br/>

<!-- Google Colab -->
## ✅ Google Colab
### "TypeError: 'str' object is not callable"
###### 오류 발생일 : December 11, 2023

<br/>

### 📌 상황 설명
> Google Colab에서 여러 변수를 선언(변수 = "") 및 출력(print) 해가며 개발 언어를 학습 중이었습니다.  
> 그런데 변수 출력(print) 과정에서 갑자기 위와 같은 TypeError가 발생하였습니다.  
> 막 출력하려던 변수뿐만 아니라 이전에 이미 선언 및 출력을 마친 변수들까지 모두 오류 상황이 되었습니다.
> <br/>
> 
> ![해당 오류](https://github.com/Kim-src/Errors/assets/150884526/c361ba6a-49bf-4aa1-9e0a-79aca87ac743)

<br/>

### 📌 해결 방법
> 해결 방법은 아주 간단하였습니다.  
> 오류가 발생된 코드 윗줄에 아래 코드 한 줄만 기입하면 해결됩니다.
> ``` Python
> del print
> ```

<br/>

### 📌 오류 원인
> 가장 가능성 있는 오류 원인은 출력문(print)을 출력으로 활용하지 않았기 때문입니다.  
> 아마도 아래와 같이 출력문을 변수로 잘못 활용 후 값을 할당했을 가능성이 있습니다.  
> ``` Python
> print = 1
> ```
> 일부러 위와 같이 출력문을 변수로 사용하면 다시 "TypeError: 'str' object is not callable" 오류가 발생됩니다.  
> 마찬가지로 ```del print```를 입력하면 프로젝트 내 모든 출력문(print)이 정상 동작되는 것을 확인하실 수 있습니다.  
