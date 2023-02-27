# Endpoint

### Endpoint 상세보기

![](<../.gitbook/assets/image (19).png>)

**Endpoint**

| 제공항목            | 설명                           |
| --------------- | ---------------------------- |
| Endpoint Name   | 설정하신 Endpoint 이름입니다.         |
| Endpoint SEQ    | Endpoint를 구분할 수 있는 고유번호입니다.  |
| Endpoint Region | Endpoint 가 생성된 물리적 위치 정보입니다. |
| Created         | endpoint 생성일입니다.             |
| Edited          | endpoint 마지막 수정일입니다.         |

**Backend Server List**

| 제공항목  | 설명                                                                   |
| ----- | -------------------------------------------------------------------- |
| IP    | 고객의 인터넷 어플리케이션 서비스를 제공하고 있는 Backend Server(Origin Server)의 IP 정보입니다. |
| Port  | 고객의 인터넷 어플리케이션 서비스를 제공하고 있는 Backend Server(Origin Server)의 포트 정보입니다. |

### Endpoint 수정

![](<../.gitbook/assets/image (27).png>)

| 설정항목            | 설명                                                                                                  |
| --------------- | --------------------------------------------------------------------------------------------------- |
| Endpoint Name   | <p>Endpoint의 이름을 수정할 수 있습니다.<br>대/소문자, 숫자 조합으로 중간에 공백없이 입력하시길 바랍니다. 최소 4자부터 최대 50자까지 입력 가능합니다. </p> |
| Endpoint Region | Endpoint Region은 수정할 수 없습니다.                                                                        |

### Backend Server 수정

![](<../.gitbook/assets/image (17).png>)

| 설정항**목**  | 설명                                                                                                                                                                                                                                                                                                                                        |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Add       | Backend Server Configration의 우측 [![Icon Add 버튼](https://github.com/gexpressman/gexpressman.github.io/raw/maunual\_v.0.9.2/images/Icon\_Add.png)](https://github.com/gexpressman/gexpressman.github.io/blob/maunual\_v.0.9.2/images/Icon\_Add.png) 버튼을 클릭하시면 EndBackend Server를 추가 등록할 수 있습니다.                                             |
| IP        | 글로벌 가속 서비스 대상인 Backend Server(Origin Server)의 IP를 입력합니다.                                                                                                                                                                                                                                                                                  |
| Port      | <p>Backend Server 포트를 수정할 수 있습니다.<br>','를 사용하여 여러개의 서비스 포트를 지정하거나 '-'를 사용하여 범위로 서비스 포트를 지정할 수 있습니다.<br>유효한 서비스 포트 범위는 1-65535 입니다. 최대 1000개의 포트를 입력할 수 있습니다. <em>(단, TCP의 경우 1001, 1002, 8181 포트는 설정할 수 없습니다.)</em><br>설정 예) 8080, 80, 90 혹은 9000-10000<br><em>주의) 서비스 포트는 중복하여 설정할 수는 없습니다. 예) 90, 80, 90  → 90이 중복 되므로 설정 불가함.</em></p> |
| Actions   | 등록한 Backend Server를 삭제할 수 있습니다.                                                                                                                                                                                                                                                                                                           |
