**1. ObjectPointer.Curved**

**Location** : VRTK Prefabs -> Pointers -> ObjectPointer.Curved  
**Work** :  
원점으로부터 일정 거리를 전진했다가 유효한 Object(바닥, GameObject 등등)와 충돌할 때까지 아래로 곡선(빔의 원점과 최종 목표 지점 사이를 잇는 베지어 곡선)을 던진다.  
곡선 포인터가 유효한 GameObject와 충돌하는 경우, 곡선 포인터가 현재 충돌하고 있는 GameObject에 대한 데이터를 포함하는 이벤트를 방출할 수 있다.  
  
**Component** :  
1. Follow Source  
포인터가 Scene에서 따라야 할 GameObject를 결정하는 부분. 즉, 원점을 정하는 부분  

2. Activation Action  
곡선 포인터가 계속 활성화되어 있다면 사용자의 몰입에 방해되기 때문에 기본적으로 비활성화 되어있다.  
따라서, 활성화되는 Boolean 형태의 기점 이벤트를 발생하도록 해주는게 필요하다. 예를 들어서 컨트롤러의 트리거 버튼이  
눌렸을 때, 이 값이 True가 되면서 포인터를 활성화한다.  
