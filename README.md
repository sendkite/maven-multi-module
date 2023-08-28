
### 1. child 모듈의 dependencies를 다른 모듈에서 사용할 수 있는가?

+ core 모듈에 선언한 dependencies를 api 모듈에서 사용할 수 있다.
+ lombok은 사용할 수 없다. (컴파일하면 사라지나..?)

단, core 모듈 먼저 build하고 api 모듈을 build해야 한다.

```shell
mvn clean install -pl core -am   
mvn clean install -pl api -am   

```
![스크린샷 2023-08-28 오후 11.57.11.png](..%2F..%2F..%2F..%2Fvar%2Ffolders%2F94%2Fm15f8j9n4hxdbq0hpbsq_hjh0000gn%2FT%2FTemporaryItems%2FNSIRD_screencaptureui_ju01yf%2F%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202023-08-28%20%EC%98%A4%ED%9B%84%2011.57.11.png)