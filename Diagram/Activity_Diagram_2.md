### 액티비티 파티션
**액티비티 파티션**은, 액션을 실행하는 주체나 각 페이즈에 액티비티 다이어그램 요소를 그룹화한 것이다.<br>

<img align="center" src="../images/Sub Activity Partition.drawio.svg"><br>

 파티션에 소속된 액션은, 파티션을 실제 표기하는 것 뿐만 아니라 액션에 소속명을 부가하여 나타낼 수도 있다.<br>
 또한, 액션이 모델 외부 영역에서 일어났을 경우엔, 그 액션에 키워드 `<<external>>`을 부가하여 나타낼 수도 있다.<br><br>
<img align="center" src="../images/Partition Name to Plus Action.drawio.svg"><br>

### 열외 핸들러
**열외 핸들러**는, 액티비티내에 열외가 발생한 경우, 대응 처리를 기재한다.<br><br>
<img align="center" src="../images/Excluded_Handler.drawio.svg"><br>

### 수신 이벤트 액션
**수신 이벤트 액션**은, 특정 이벤트가 일어나기를 기다리는 액션이다. <br>
기다리는 이벤트가 시간에 관한 이벤트(ex. 매주 일요일 오전 0시에 발생등)가 있을 경우, 강제하기위해, 모래시계 아이콘을 기재한다.<br>
<img align="center" src="../images/Recieve_Event_Action.drawio.svg"><br>

### 송신 시그널 액션
**송신 시그널 액션**은, 다른 액티비티에서 받은 정보로부터, 시그널을 송신하는 액션이다. <br>
<img align="center" src="../images/Send Signal Action.drawio.svg"><br>

### 데이터 스토어 노드
**데이터 스토어 노드**는, 데이터베이스등 영속적 데이터가 보관될 수 있는 대상을 나타낸다. <br>
<img align="center" src="../images/Data Store Node.drawio.svg"><br>

### 확장영역
**확장영역**은, 복수의 입력치를 처리하기 위해 처리 부분을 둘러싼 영역이다. <br>
복수 입력치는 리스트 등 컬렉션 타입으로 만든다. 컬렉션의 처리방법에 따라, `parallel`, `iterativ`, `stream`의 3개의 모드가 있다.

#### parallel
 모드에 `parallel`이 지정된 경우, 컬렉션 각각 입력치가 평행처리 된다. 입력치의 숫자만큼 확장영역안 동작이 평행되어 실행된다.
 
#### iterative
 모드에 `iterative`가 지정된 경우, 컬렉션은 순차처리된다. 하나의 입력치 처리가 완료된 후 다음 처리가 실행된다.<br>
 처리에 출력치가 있을 경우, 입력치 순번으로 출력치가 컬렉션에 수납된다.

#### stream
 모드에 `stream`이 지정된 경우, 입력치에 대해 처리가 한번에 실행된다. 처리에 출력치가 있을 경우, 입력 컬렉션과 같은 구성으로 컬렉션을 구축한다. <br>
<img align="center" src="../images/Extend Area.drawio.svg"><br>

