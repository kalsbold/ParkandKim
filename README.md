# ParkandKim

유니티에서 안드로이드 빌드 테스트를 기기에서 바로 하는 방법.

1. 먼저 JDK를 설치한다.

2. 아래 링크를 따라 android studio 와 unity3D를 설치한다.
//메인 링크
http://webnautes.tistory.com/1006

3. 안드로이드 기기에서 USB 디버깅 모드를 켠다.
//갤럭시 s6기준
http://m.blog.naver.com/kkandaa/220727625697


빌드시 오류 발생시 해결방법

1. 유니티에서 빌드 앤 런 시에 발생하는 오류

CommandInvokationFailure: Unable to list target platforms. Please make sure the android sdk path is correct. See the Console for more details. 

위 오류가 발생하면  

Android SDK tools 가 최신 버전(25.3.1)으로 업데이트 되면서 unity가 사용하던 기능이 없어진거 같다고 합니다. 

해결책은 기존 Android SDK설치 폴더에서 tools 폴더 이름을 변경한 후 [Your Android SDK root]/tools -> toolsXXXX  
http://dl-ssl.google.com/android/repository/tools_r25.2.5-windows.zip 를 다운로드 받아서 압축 풀고 해당 tools 폴더를 위의 
Android SDK설치 폴더에 복사합니다. 그러면 unity에서 예전처럼 잘 됩니다.

//
http://www.devkorea.co.kr/bbs/board.php?bo_table=m03_qna&wr_id=79671
//

이 방법을 시행하면 해결됨.