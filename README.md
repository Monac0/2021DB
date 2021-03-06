# 2021_02_DB_project

### 개발 명세 (TODO)

## 구현 완료된 기능은 X 표시, A 그룹 평가 기준 (A - []) / B 그룹 평가 기준 (B-[])

1. 평가기준

   1. 로그인  
  
    A - [X] 서비스에 가입된 ID와 패스워드로 로그인 할 수 있다.   
    B - [X] DB에 ID, 패스워드와 일치하지 않는 정보를 입력할 경우 로그인 되지 않는다.   
  
   2. 회원가입  
  
    A - [X] 회원가입 시 ID 중복 확인을 하고 UI에서 결과를 확인할 수 있다.  
    A - [X] ID, 비밀번호, 이름에 값이 정상적으로 입력되었을 때 회원가입이 가능하다.  
    B - [X] ID, 비밀번호, 이름에 값이 입력되지 않았을 경우 (NULL) 회원가입이 되지 않는다.  
    B - [X] ID의 길이가 영문, 숫자를 포함하여 최대 20자를 벗어나거나 특수문자가 입력될 경우 가입되지 않는다.  
  
   3. 친구목록  
  
    A - [ ] <내 이름>, <내 위치>, <내 상태메시지>를 확인할 수 있다.  
    A - [X] 친구 별 <이름>, <상태메시지>, <회원 유형>, <위치>가 UI에 표시된다.  
    B - [X] 현재 접속중인 친구와 미접속 중인 친구의 목록이 구분되어 UI에 표시된다.  
  
   4. 친구 검색  
  
    A - [X] 아이디의 일부를 입력 받아 회원 검색이 가능하다.  
    A - [X] 검색된 회원이 이미 친구인 경우 <친구 삭제>버튼을 눌러 친구 목록에서 삭제할 수 있다.  
    B - [X] 이름을 입력 받아 회원 검색이 가능하다.   
    B - [X] 검색된 회원의 이름과 상태메시지가 UI에 표시된다.  
    B - [X] 검색된 회원이 친구가 아닌 경우 <친구 추가>버튼을 눌러 친구 목록에 추가할 수 있다.  
      
   5. 내 정보 편집  
  
    A - [X] CSV 파일을 업로드하여 현재 사용자의 위치에 해당하는 “위도”, “경도”, “건물명”, “층수”, “SSID”, “IP”를 변경할 수 있다.  
    A - [X] <회원 탈퇴>할 수 있으며 “사용자 정보”, “채팅 메시지 기록”, “친구 목록”, “다른 회원의 친구목록”에서 정보가 삭제된다.  
    B - [X] 현재 사용자의 <상태 메시지> 변경이 가능하다. (최대 한글기준 20자)  
    B - [X] <로그아웃>하여 로그인 화면으로 돌아갈 수 있으며 친구로 등록된 사용자에게 미접속으로 표시된다.  
  
   6. 채팅 목록  
  
    A - [X] 채팅을 주고받은 사용자의 목록이 마지막 채팅 메시지를 주고받은 시간의 내림차순으로 정렬되어 UI에 표시된다.  
    B - [X] 채팅을 주고받았던 사용자중 현재 접속중인 사용자와 미접속 중인 사용자를 UI를 통해 구분할 수 있다.  
  
   7. 주변  
  
    A,B 동시 평가  
    [ ] (5.7 방법A) 사용자들이 위치하는 “건물”, “층수”, “SSID”에 해당하는 주변 목록이 표시된다  
    [ ] (5.7 방법A) 11 항목 목록의 주변을 선택했을 때 해당 주변에 위치한 사용자들이 접속/미접속 구분하여 표시된다  
  
   8. 채팅하기  
  
    A - [X] 서비스를 이용하는 다른 사용자와 실시간 채팅을 주고받을 수 있다.  
    A - [ ] 동일한 공간에 위치한 사용자만 볼 수 있는 랑데부 메시지를 전송하고 수신할 수 있다.  
    A - [ ] 내가 전송한 메시지를 상대방이 읽었는지 읽지 않았는지 채팅하기 UI 화면을 통해 확인할 수 있다.  
    B - [X] 채팅 메시지가 DB에 기록된다.  
    B - [X] 로그아웃 후 다시 로그인하여도 주고받은 채팅 메시지 기록이 유지된다.  
    B - [ ] 설정된 시간(3분, 30분, 60분) 동안만 확인할 수 있는 랑데부 메시지를 전송하고 수신할 수 있다.  
