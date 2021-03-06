## Dependencies and Normalization

##### 

[뒤로가기](/database/README.md)

종속성과 정규화에 대한 정의에 대해 다룰 것이다. 해당 게시글에서는 4, 5 정규형, BCNF에 대한 설명은 진행되지 않으니 참고 바란다.  

---

#### 함수적 종속성의 정의  

* 데이터들이 어떤 기준 값에 의해 항상 종속되는 현상  
* 속성 집합 X의 값이 Y의 값을 유일하게 결정한다면 "Y는 X에 함수적으로 종속된다."라고 하며 'X -> Y'로 표기  

#### 함수적 종속성의 종류  

* 완전 함수적 종속성: 키의 모든 속성이 일반 속성을 결정하는 관계  
* 부분 함수적 종속성: 키 중의 일부가 어떤 속성을 결정하는 결정자가 되는 관계  
* 이행 함수적 종속성: A가 B를 결정할 때, B가 C를 결정한다면 A는 C를 이행적으로 결정하는 결정자가 된다.  

#### 이상 현상의 정의  

* 데이터의 중복성으로 인해 릴레이션을 조작할 때 발생하는 얘기치 못한 비합리적인 현상  
* 정규화가 안되어 하나의 엔터티에 여러 실체의 속성들을 혼합한 경우 발생  

#### 이상현상(이 발생하는 상황)의 종류  

* 삽입 이상: 릴레이션 R에서 특정 속성 값 갱신 시 중복 저장되어 있는 속성 값 중 하나만 갱신하고, 나머지는 갱신하지 않아 발생하는 데이터 불일치 현상  
* 삭제 이상: 릴레이션 R에서 특정 투플을 삽입할 경우 원하지 않는 데이터까지 삽입해야야 되는 현상  
* 갱신 이상: 릴레이션 R에서 특정 투플을 삭제할 경우, 원하지 않는 정보까지 삭제되는 현상(데이터 손실)  

#### 정규화 정의  

* 관계 Schema의  데이터구조를 수학적 이론을 적용, 분석하여 보다 나은 데이터구조로 재구축하는 관계  

##### 제 1 정규형(1NF)의 정의  

* 반복 그룹이 제거된 형태  
* 이상현상 발생 x  
  

##### 제 2 정규형(2NF)의 정의  

* 부분 함수적 종속성 - 키가 아닌 열이 합성키(집합키)의 일부 종속 제거  
* 이상현상 발생 O  
  

##### 제 3 정규형(3NF)의 정의  

* 이행 함수적 종속성 - 키가 아닌 열이 키를 제외한 열에 종속 제거  

> 제 4, 5 정규형, BCNF 등의 다른 정규형도 있지만, 이들은 현실세계에서는 거의 불가능한 형태이다. 그러므로 위의 1, 2, 3 정규형이 이상현상이 적게 발생하는 정규형이다.  

