
![33](https://github.com/dino-21/STEP8_6_fileupload2_thumbnail/assets/80396471/42cd0268-36d1-42e2-9616-c98b729ba26d)

![32](https://github.com/dino-21/STEP8_6_fileupload2_thumbnail/assets/80396471/3571fff7-e67d-4502-8832-8b2f766f520a)

![28](https://github.com/dino-21/STEP8_6_fileupload2_thumbnail/assets/80396471/730323e9-762f-496e-af5e-5d1253afe696)


1 C:\upload\temp 폴더 만들기

2 
<!-- 파일 업로드 기능에 대한 설정 -->
web.xml <servlet>태그내에 <multipart-config> 태그를 추가

3 servlet-context.xml 코드 추가
<!-- 파일 업로드를 처리하는데 쓰이는 StandardServletMultipartResolver 빈을 설정 -->


4
UploadController.java 파일만들기


5 uploadForm.jsp 파일만들기


6 MultipartFile 타입  


7  UploadController.java  코드추가


8 Ajax를 이용하는 파일 업로드


9 uploadAjax.jsp 파일 만들기


10 uploadAjax.jsp  js 코드 추가 – jQuery를 이용한 경우 파일 업로드는 FormData 객체 이용


11 uploadAjax.jsp  js 코드 추가 – JQuery를 이용한 첨부파일 전송(Ajax)


12파일의 확장자나 크기의 사전 처리

uploadAjax.jsp  js 코드 추가



13  이미지 파일만 올릴수 있게 파일 체크

14  중복된 이름의 첨부파일 처리 – 중복 방지를 위한 UUID 적용
 


15  썸네일 이미지 생성

Thumbnailator : Java용 썸네일 생성 라이브러리


16 pom.xml




17 이미지 파일의 판단 
MIME 타입 





18 이미지 파일이라면 섬네일을 생성 코드 수정
톰캣실행 확인

19 업로드된 파일의 데이터 반환

20 AttachFileDTO 클래스 만들기

21  브라우저에서 Ajax처리



22 브라우저에서 섬네일 처리

23 일반 파일의 처리

24 섬네일 이미지 보여주기

Javascript 처리
