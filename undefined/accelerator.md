# Accelerator

## Accelerator 리스트

![](<../.gitbook/assets/image (12).png>)

#### Search

Accelerator name, IP, Region으로 검색하실 수 있습니다.

**제공 항목**

| 제공항목              | 설명                                                                                                            |
| ----------------- | ------------------------------------------------------------------------------------------------------------- |
| Name              | 설정하신 Accelerator 이름입니다.                                                                                       |
| Static IP Address | Listener에 할당된 IP입니다.                                                                                          |
| Listener Region   | Listener region 정보입니다.                                                                                        |
| Endpoint Region   | Endpoint region 정보입니다.                                                                                        |
| Enabled           | <p>현재 서비스 상태입니다.<br>서비스 상태가 Off 여도 Accelerator는 사용중으로 과금이 발생합니다.<br></p>                                      |
| Status            | <p>deployment 상태입니다.<br>- <strong>In Progress:</strong> 서비스 세팅중.<br>- <strong>Deployed:</strong> 서비스 세팅완료</p> |
| Edited            | 최초 생성일 혹은 마지막 수정일입니다.                                                                                         |

#### Accelerator 상세보기

![](<../.gitbook/assets/image (24).png>)

**Accelerator Configuration**

| 제공항목                | 설명                                                                                                            |
| ------------------- | ------------------------------------------------------------------------------------------------------------- |
| Accelerator Name    | 설정하신 Accelerator 이름입니다.                                                                                       |
| Accelerator SEQ     | Accelerator를 구분할 수 있는 고유번호 입니다.                                                                               |
| Bandwidth Cap.      | 가속서비스가 1개월 간 사용할 수 있는 최대 사용량 정보입니다.                                                                           |
| Enabled             | <p>현재 서비스 상태입니다.<br>서비스 상태가 Off 여도 Accelerator는 사용중으로 과금이 발생합니다.<br></p>                                      |
| Provisioning Status | <p>deployment 상태입니다.<br>- <strong>In Progress:</strong> 서비스 세팅중.<br>- <strong>Deployed:</strong> 서비스 세팅완료</p> |
| Created             | 가속 서비스 생성일입니다.                                                                                                |
| Edited              | 마지막 수정일입니다.                                                                                                   |

**Listener List**

| 제공항목              | 설명                                                   |
| ----------------- | ---------------------------------------------------- |
| Listener Name     | 설정하신 Listener 이름입니다.                                 |
| Listener SEQ      | Listener를 구분할 수 있는 고유번호입니다.                          |
| Listener Region   | Listener가 생성된 물리적 위치 정보입니다.                          |
| IP Address        | Listener에 할당된 IP입니다.                                 |
| Port and Protocol | 가속 서비스를 수행할 고객의 인터넷 어플리케이션 서비스가 사용하는 프로토콜과 포트 정보입니다. |
| Endpoint Region   | Endpoint가 생성된 물리적 위치 정보입니다.                          |
| Status            | 가속서비스에 사용되는 Listener의 상태입니다                          |

### Accelerator 수정

###

![](<../.gitbook/assets/image (29).png>)

| 설정항목             | 설명                                                                                                                                                   |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| Accelerator Name | <p>Accelerator의 이름을 수정할 수 있습니다.<br>생성할 GA를 다른 GA와 구분하기 용이하고, 기억하기 쉬운 이름으로 입력하시길 바랍니다.<br>대/소문자, 숫자 조합으로 공백없이 입력해 야하며, 최소 4자부터 최대 50자까지 입력 가능합니다.</p> |
| Bandwidth Cap.   | <p>글로벌 가속 서비스를 이용하여 서비스 할 한달간 최대 데이터 사용량을 설정합니다.<br>설정한 데이터 사용량을 초과하여 사용할 수 없으며, 사용량을 수정할 수 있습니다.<br>사용량은 최소 2Gbps에서 최대 10Gbps까지 제공됩니다.</p>          |
| Enabled          | <p>글로벌 가속 서비스를 활성화 또는 비활성화 합니다. 가속 서비스를 삭제하려면 비활성화로 설정해야 합니다.<br>가속 서비스가 Off상태여도 Accelerator를 삭제하기 전까지 과금은 발생됩니다.</p>                                |

### Accelerator 삭제

![](<../.gitbook/assets/image (42).png>)



* 생성한 가속서비스를 삭제할 수 있습니다.
* 다만, 가속 서비스 상태가 비활성화 상태여야 삭제가 가능합니다.
