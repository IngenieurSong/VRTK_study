**들어가기에 앞서**  
Teleport의 종류에는 두가지가 있다.  
  
**1. Instant**  
사용자가 포인터로 목적지를 정하면 중간 과정없이 바로 그 곳으로 이동하는 방법  
멀미를 줄이기 위해서 이용된다.  
  
**2. Dash**  
사용자가 포인터로 목적지를 정하면 해당 위치에 도달할 때까지 점차적으로 선형 운동을 통해 이동하는 방법  

**1. Teleporter.Instant**  
  
**Location** : VRTK Prefabs -> Locomotion -> Teleporters  
**Work** :  
Instant 방법의 Teleport를 실행하는 Prefab  
    
**Component** :  
  
1. Target  
   목적지로 실제 이동할 GameObject를 결정하는 부분  
   주로, 메인 카메라를 많이 설정한다.
  
2. Offset  
   Target를 메인 카메라 Object로 설정했으나 실제로 목적지 좌표와 메인 카메라 좌표가 완전히 일치한다면  
   사용자로 하여금 이상한 느낌을 받을 수 있다. 이를 방지하기 위해서는 아래 그림과 같은 조치가 필요하다.  
     
   ![locomotion](https://user-images.githubusercontent.com/52345271/121820140-1739f100-cccc-11eb-9ce4-3d99fad3b477.png)  
     
   따라서 이러한 상황을 방지하기 위하여 Teleport 과정에서 고려해야 할 것을 이 Offset으로 설정한다.  
     
 **2. Teleporter.Dash**
   
 **Location** :  VRTK Prefabs -> Locomotion -> Teleporters  
 **Work** :  
 Dash 방법의 Teleport를 실행하는 Prefab  
   
 이하 동일
