# 🧮계산기
## 🛠️구현 기능
UI 
- ConstraintLayout - Flow
- Style
- color(Light/Dark)
- theme  

Kotlin
- when
- StringBuilder


## Flow
가상의 Layout!
  

### StringBuilder vs String
StringBuilder : 문자열을 연산할때 주로 사용하는 자료형
String 으로도 할 수 있지만 (+ 붙여서) 속도가 느려진다.  
그래서 문자열 연산에는 StringBuilder가 좋다.

### androidx.constraintlayout.helper.widget.Flow

chain의 방향을 설정할 때는, LinearLayout에서 방향을 설정하는것과 동일하게 orientation을 이용
```xml
    android:orientation = "horizontal|vertical"
```

Bias  
체인의 형태를 유지하면서 bias가 적용
```xml
    app:flow_verticalBias="float"
    app:flow_horizontalBias="float"
```
 
Gap    
margin과 동일한 효과, 각각 뷰 사이의 gap만을 지정 할 수 있다.  
```xml
    app:flow_verticalGap="8dp"
    app:flow_horizontalGap="8dp"
```

Max elements
각 줄마다 표시할 뷰의 개수를 지정하고 싶을 대 사용
```xml
    app:flow_maxElementsWrap="integer"
```
