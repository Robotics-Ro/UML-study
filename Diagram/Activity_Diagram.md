## Activity Diagram
### 액티비티 다이어그램 
-------------
<img align="center" src="../images/Activity_Diagram.png"/>

**액티비티 다이어그램**(activity diagram)이란, 처리의 실행수순을 나타내는 다이어그램이다.<br>
이 다이어그램은, 시스템 개발의 상류공정으로 비지니스 프로세스를 분석하여 나타내거나, <br>
하류공정으로 프로그램의 상세한 제어흐름을 기재하는 경우 등, 공정에 관계없이 넓게 이용된다. <br>
 기존에 사용되던 플로우챠트(흐름도)에 가까운 기법이며, 객체지향의 색도 얕으므로, <br>
 시스템에 그리 익숙하지 않은 유저와도, 커뮤니케이션 취하기 좋은 이점이 있다. <br>


#### 액티비티 다이어그램의 구성요소
-------------------------------
<img align="center" src="../images/AD_Components.drawio.svg"/>

### 액티비티
**액티비티**는, 일련의 액션이 정리되어진 처리수순을 나타낸다. <br>

액티비티에 파라미터가 있을 경우, 액티비티명 아래에 기재한다. 사전조건이나 사후조건이 있을 경우 <br>
'<<precondition>>' , '<<postcondition>>' 을 기재한다.
 
<img align="center" src="../images/Activity.drawio.svg"/>
 
### 액션
**액션**은 액티비티를 편성하는 처리의 단위다. <br>
 액션은 액티비티와 다르게 내부에 다른 액션을 넣을 수가 없다. <br>
 액션에 사전조건, 사후조건이 있을 때엔, 대상이 되는 액션과 엮인 노트에
 키워드 `<<precondition>>` , `<<postcondition>>`을 추가하여 기재한다. <br>
<img align="center" src="../images/Action.drawio.svg"/>
 
### 개시 노드
 **개시 노드**는, 일련의 액티비티가 처리를 개시하는 지점을 나타낸다.
 <img align="center" src="../images/Start_Node.drawio.svg">
