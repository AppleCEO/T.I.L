메인 화면에서 팝업 뷰를 두개 띄워야 할 일이 있었다.
이미 하나의 팝업을 띄우고 있었고 하나르 추가해야 했다.
뷰디드로드 상단에 조건문을 추가해 팝업을 띄우게 코드를 작성하였는데 팝업이 뜨지 않았다.
하나의 뷰컨트롤러에 두개의 팝업은 안 뜨느 것으로 생각하였는데 디버깅을 해보니 whose view is not in the window hierarchy 라는 오류가 보였다.
찾아보니 아래 글을 발견하였고 팝업 띄우는 코드르 viewDidAppear 로 옮기니까 정상 동작하였다
https://velog.io/@ellyheetov/errorhandling01
