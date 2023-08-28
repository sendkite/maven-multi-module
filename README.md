
### 1. child 모듈의 dependencies를 다른 모듈에서 사용할 수 있는가?

+ core 모듈에 선언한 dependencies를 api 모듈에서 사용할 수 있다.
+ lombok은 사용할 수 없다. (컴파일하면 사라지나..?)

단, core 모듈 먼저 build하고 api 모듈을 build해야 한다.

```shell
mvn clean install -pl core -am   
mvn clean install -pl api -am   

```
![스크린샷 2023-08-28 오후 11 58 20](https://github.com/sendkite/maven-multi-module/assets/90877864/03574c21-c697-459a-a932-f34b8b6f0a39)


### 2. 전이 의존성, 추이 의존성에 대하여
- https://mangkyu.tistory.com/296
