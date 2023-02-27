# Channel Management

## Channel List

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

### Search

서비스 채널 이름으로 생성한 채널을 검색하실 수 있습니다.

### 제공항목

<table><thead><tr><th>제공항목</th><th>설명</th><th data-hidden></th></tr></thead><tbody><tr><td>Channel Name</td><td>Channel 이름</td><td></td></tr><tr><td>Output Setting</td><td>라이브 송 프로파일 묶음의 이름</td><td></td></tr><tr><td>Channel Status</td><td><p>라이브 서비스 채널의 상태</p><ul><li>Input stream waiting: 채널 생성 후 라이브 영상 입력 대기 상태.</li><li>In Progress: 채널 구성 진행 중.</li><li>On-Air: 라이브 영상 송출 중.</li><li>Off-Air: 라이브 영상 송출 완료.</li></ul></td><td></td></tr><tr><td>Device Status</td><td><p>트랜스코더 장비의 상</p><ul><li>In progress: 장비 구성 중.</li><li>Deployed: 장비 구성 완료.</li><li>Failed: 장비 구성 실패.</li></ul></td><td></td></tr><tr><td>GA Status</td><td><p>글로벌 어플리케이션 가속기의 상태</p><ul><li>In Progress: 구성 중.</li><li>Deployed: 구성 완료.</li><li>Failed: 구성 실패.</li><li>Off: 설정 없음.</li></ul></td><td></td></tr><tr><td>Event</td><td><p>Event 알람 설정 상태</p><ul><li>On: 이벤트 알람 수신.</li><li>Off: 이벤트 알람 수신하지 않음.</li></ul></td><td></td></tr></tbody></table>



## Channel Details

<figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

### 제공항목

<table><thead><tr><th>제공항목</th><th>설명</th><th data-hidden></th></tr></thead><tbody><tr><td>Channel Name</td><td>Channel 이름</td><td></td></tr><tr><td>Channel Status</td><td><p>라이브 서비스 채널의 상태</p><ul><li>Input stream waiting: 채널 생성 후 라이브 영상 입력 대기 상태.</li><li>In Progress: 채널 구성 진행 중.</li><li>On-Air: 라이브 영상 송출 중.</li><li>Off-Air: 라이브 영상 송출 완료.</li></ul></td><td></td></tr><tr><td>Channel ID</td><td>서비스 채널의 ID로 시스템에서 자동 생성.</td><td></td></tr><tr><td>Device Status</td><td><p>트랜스코더 장비의 상</p><ul><li>In progress: 장비 구성 중.</li><li>Deployed: 장비 구성 완료.</li><li>Failed: 장비 구성 실패.</li></ul></td><td></td></tr><tr><td>Created</td><td> 채널의 생성날짜.</td><td></td></tr><tr><td>GA Status</td><td><p>글로벌 어플리케이션 가속기의 상태</p><ul><li>In Progress: 구성 중.</li><li>Deployed: 구성 완료.</li><li>Failed: 구성 실패.</li><li>Off: 설정 없음.</li></ul></td><td></td></tr><tr><td>Output Setting</td><td><p>라이브 송출 프로파일 묶음의 이름. </p><p>(예, 1080p-set: 1080p, 720p, 420p )</p></td><td></td></tr><tr><td>Recording Setting</td><td><p>녹화 설정 상</p><ul><li>No Recording : 녹화 안함</li><li>SB Object Storage : 설정된 오브젝트 스토리지에 녹화</li></ul></td><td></td></tr><tr><td>Streaming Protocol</td><td> 라이브 스트리밍 프로토콜</td><td></td></tr><tr><td>HLS Timed Metadata</td><td>HLS ID3 Timed Metadata 변환 여부. 입력되는 RTMP의 Timed Metadata Signal을 hls ID3 Timed Metadata로 변환.</td><td></td></tr><tr><td>Segment Duration</td><td>라이브 스트리밍을 위해 생성할 MPEG-2 전송 스트림 세그먼트의 길이.(단위: 초)</td><td></td></tr><tr><td>Segment Count</td><td>라이브 스트리밍시 매니페스트(.m3u8) 파일에 유지할 세그먼트 수.<br><em>* 세그먼트 길이와 세그먼트 수가 커질수록 영상송출과 영상재생 간의 delay는 증가 합니다.</em></td><td></td></tr><tr><td>TimeMachine</td><td>라이브 영상 되돌려 보기를 지원하는 Time machine 기능 사용 여부.</td><td></td></tr><tr><td>Event Notification</td><td><p>Event 알람 설정 상태</p><ul><li>On: 이벤트 알람 수신.</li><li>Off: 이벤트 알람 수신하지 않음.</li></ul></td><td></td></tr><tr><td>Origin IP</td><td>미디어 스트리밍 서버의 IP</td><td></td></tr><tr><td>Stream Key</td><td>RTMP Push로 원본 동영상을 라이브 트랜스코더로 입수시키기 위한 Stream Key</td><td></td></tr><tr><td>Upstream URL</td><td>고객(서비스 제공자)이 라이브 원본 동영상을 RTMP Push로 인입시키기 위한 라이브 트랜스코더 서버 URL</td><td></td></tr><tr><td>Play URL</td><td>사용자가 라이브 스트리밍 영상을 재생할 수 있는 라이브 영상 play URL</td><td></td></tr></tbody></table>

## Channel Edit

* 라이브 트랜스코딩과 라이브 스트리밍 서비스 프로파일을 변경하실 수 있습니다.

<figure><img src="../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

### 제공항목

<table><thead><tr><th>제공항목</th><th>설명</th><th data-hidden></th></tr></thead><tbody><tr><td>Channel Name</td><td>Channel 이름</td><td></td></tr><tr><td>Created</td><td> 채널의 생성날짜.</td><td></td></tr><tr><td>Segment Duration</td><td>라이브 스트리밍을 위해 생성할 MPEG-2 전송 스트림 세그먼트의 길이를 설정합니다.(단위: 초)</td><td></td></tr><tr><td>Segment Count</td><td>라이브 스트리밍시 매니페스트(.m3u8) 파일에 유지할 세그먼트 수를 설정합니다.<br><em>* 세그먼트 길이와 세그먼트 수가 커질수록 영상송출과 영상재생 간의 delay는 증가 합니다.</em></td><td></td></tr><tr><td>HLS Timed Metadata</td><td>HLS ID3 Timed Metadata 변환 여부를 설정합니다. 입력되는 RTMP의 Timed Metadata Signal을 hls ID3 Timed Metadata로 변환합니다. </td><td></td></tr><tr><td>TimeMachine</td><td>라이브 영상 되돌려 보기를 지원하는 Time machine 기능 사용 여부를 설정합니다.</td><td></td></tr><tr><td>Event Notification</td><td><p>Event 알람 설정 상태</p><ul><li>On: 이벤트 알람 수신.</li><li>Off: 이벤트 알람 수신하지 않음.</li></ul></td><td></td></tr><tr><td>Output Setting</td><td>라이브 스트리밍 시 출력할 output profile Set을 설정합니다. 각각의 Profile Set에서 지원하는 output profile을 확인 후 원하는 Profile Set을 선택하실 수 있습니다.</td><td></td></tr><tr><td>Preset</td><td>라이브 스트리밍 서비스에 적합한 스트리밍 프로파일 세트(Output Profile Set)를 선택합니다.</td><td></td></tr><tr><td>                        1080p-set</td><td>1080p, 720p, 480p, 360p, 240p 출력을 지원하는 프로파일 셋 입니다.</td><td></td></tr><tr><td>                        720p-set</td><td>720p, 480p, 360p, 240p 출력을 지원하는 프로파일 셋 입니다.</td><td></td></tr><tr><td>                        480p-set</td><td>480p, 360p, 240p 출력을 지원하는 프로파일 셋 입니다.</td><td></td></tr></tbody></table>

## Channel Delete

* 서비스 채널을 삭제합니다.&#x20;

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
삭제한 채널은 복구 할 수 없습니다. 신중히 선택하시길 바랍니다.

개설한 채널은 스트리밍 서비스를 사용하지 않더라도 삭제 전까지 과금 정책에 따라 Device 기본 요금이 과되므로 장시간 사용하지 않는 채널은 삭제하시길 바랍니다.
{% endhint %}
