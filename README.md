# Linux_Chat_Program_SystemProgramming2024_Team9

리눅스 환경에서 C로 구현된 간단한 채팅 프로그램으로, 
서버와 클라이언트가 네트워크를 통해 메시지를 송수신할 수 있습니다. 클라이언트는 채팅 서버에 연결하여 메시지를 송수신하고,
파일을 업로드 및 다운로드하며, 개인 파일 디렉토리를 관리할 수 있습니다.
네트워크 통신에는 TCP를 사용하며, 여러 채팅 방을 지원합니다.

## 주요 기능

### server

  -클라이언트 연결

  -여러 채팅방 관리 및 클라이언트 간 채팅 중계

  -파일 업로드 및 다운로드 지원

  -클라이언트 목록 관리


### client

  -채팅 서버에 연결

  -메시지 송수신

  -서버에 파일 업로드 및 다운로드

  -로컬 디렉토리의 개인 파일 목록 표시

  -채팅 방 전환

  -메뉴 옵션을 위한 신호 처리

## 요구 사항

  -GCC 컴파일러

  -POSIX 호환 운영 체제(Linux, macOS ...)

  -pthread 라이브러리


## 사용 방법

 -server.c 

    -코드 컴파일 : gcc -o server server.c -lpthread

    -실행 방법 : ./server

 -client.c

    -코드 컴파일 : gcc -o client client.c -lpthread

    -실행 방법 : ./client

    
    화면의 지시에 따라 닉네임을 입력하고 채팅 서버에 연결합니다, 클라이언트는 접속할 채팅방의 이름을 생성할 것입니다.

    메시지를 보내려면, 메시지를 입력하고 Enter 키를 입력합니다. 파일 업로드/다운로드, 채팅방 목록 표시, 방 전환 등의

    다른 작업을 수행하려면 'Ctrl + c' 키를 입력헤 interactive 메뉴를 엽니다.

### 예시

![room2](https://github.com/migumy/systemprogramming/assets/171572256/70088e0c-821c-4ab8-8ab1-9820feb40e95)
![room1](https://github.com/migumy/systemprogramming/assets/171572256/bc267ca3-aa3f-4f1e-be0d-3a29adc83fd9)


## Interactive 메뉴 옵션

### ctrl + c 를 입력하면 다음의 메뉴가 나타납니다.

![interactivemenus](https://github.com/migumy/systemprogramming/assets/171572256/2c5e31d1-8a79-4a20-b782-57b4f562014b)

1.채팅방 목록 : 서버에서 사용 가능한 채팅방 목록을 요청하고 표시합니다.

2.채팅방 생성: 새 채팅방을 생성합니다. 방 이름을 입력하면 됩니다.

3. 채팅방 이동: 다른 채팅방으로 전환합니다. 이동할 방의 이름을 입력하면 됩니다.

4. 파일 올리기: 개인 폴더에서 파일을 서버로 업로드합니다.

5. 파일 내려받기: 서버에서 파일을 다운로드하여 개인 폴더에 저장합니다.

6. 내 파일 목록: 로컬 디렉토리의 개인 파일 목록을 표시합니다.

7. 채팅 검색: 특정 문자열을 포함하는 채팅 메시지를 검색합니다.

  
 

 

