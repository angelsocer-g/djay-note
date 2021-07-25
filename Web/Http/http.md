# [Djay Web Note](../web-note.md)

---

## Http Method Reference

### 원문
- [HTTP GET 요청에 body를 붙여서 보내면 어떤 일이 벌어질까?](https://libsora.so/posts/http-get-request-with-body-and-http-library/)
- [HTTP GET 요청에 body를 붙여서 보내면 어떤 일이 벌어질까? part2](https://libsora.so/posts/http-request-with-body-and-java-httpurlconnection/)

### 요약
Http Get 요청에 body를 넣어서 요청시 post로 변경되서 요청되는 이슈가 있어 관련 내용에 대해서 고찰한 내용으로,
글을 보다보니 다양한 테스트와, 각 기술을 시간순으로 접근해서 원하는 결론에 도달하는 과정이 뭔가
신선하고 재밌게 느껴졌다. 나였다면 이건 원래 그런거야 봉인하고 넘어갔겠지.. ㅋㅋ.. 반성하자..

  - spec상 get method 는 body가 없다
  - HttpUrlConnection 에서 request body가 있는 요청을 post로 판단하는건 틀린 구현이 아니다.
    - 구현시점엔 HTTP1.0 이여서 method 가 get/post 밖에 없었다.


### 발췌
![get 요청이 post로 바뀐 이유](getchangedtopost.png)


