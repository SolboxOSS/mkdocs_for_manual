# 라이브 트랜스코딩 서비스

고객이 목적 서비스 지역에서 라이브 초 저지연 스트리밍 서비스를 하기 위한 라이브 트랜스코딩 서비스 개설 절차는 다음과 같습니다.&#x20;

> 1. 라이브 트랜스코딩을 위한 서비스 채널을 설정합니다.
> 2. 라이브 트랜스코딩을 수행하는 시스템(VM)의 스펙을 선택합니다.
> 3. 글로벌 사용자 지역에서 라이브 스트리밍 서비스를 수행하는 어플리케이션 가속기를 설정합니다.
> 4. 트랜스코딩된 라이브 영상을 저장할 저장소와 알람을 설정합니다.
> 5. 설정한 정보를 확인 후 서비스 개설을 진행합니다. &#x20;

{% hint style="warning" %}
라이브 초 저지연 스트리밍 서비스를 개설하기 위해서는 반드시 글로벌 어플리케이션 가속기를 생성(GA Setting = On) 하여야 합니다.&#x20;
{% endhint %}

라이브 트랜스코딩 서비스를 생성하기 위한 서비스 개설 Wizard를 제공하며 설정 방법은 아래와 같습니다.



## 라이브 트랜스코딩 서비스 설정 Wizard 시작

* Live Transcoder 메뉴에서 'Create Channel'을 클릭하여 서비스 채 생성 Wizard를 실행 시킵니다.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

## 라이브 트랜스코딩 서비스 채널 설정

* 라이브 트랜스코딩을 수행하는 트랜스코 서비스 채널을 설정합니다.&#x20;

> a. Channel의 이름을 설정합니다.\
> b. 라이브 스트리밍을 위해 생성할 MPEG-2 전송 스트림 세그먼트의 길이를 설정합니다.(단위: 초)\
> c. 라이브 스트리밍시 매니페스트(.m3u8) 파일에 유지할 세그먼트 수입니다.
>
> &#x20;  \- 세그먼트 길이와 세그먼트 수가 커질수록 영상송출과 영상재생 간의 delay는 증가 합니다.\
> d. HLS ID3 Timed Metadata 변환 여부를 설정합니다. 입력되는 RTMP의 Timed Metadata Signal을 hls ID3 Timed Metadata로 변환합니다. \
> e. 라이브 스트리밍 시 출력할 output profile Set을 설정합니다. 각각의 Profile Set에서 지원하는 output profile을 확인 후 원하는 Profile Set을 선택하실 수 있습니다.

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

## 라이브 트랜스코딩 장비 설정

* 라이브 트랜스코딩을 수행하는 트랜스코더 장비(Device) 사양을 설정합니다.

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
FHD급(1080p-set): BL2.16x32, HD급(720p-set): BL2.8x16, SD급(480p-set):BL2.4x8 을 권장합니다.&#x20;
{% endhint %}

{% hint style="warning" %}
현재, 라이브 트랜스코딩 서비스는 IBM cloud의 도쿄 리전에서만 서비스 되고 있으며, 향후 서비스 지역을 확장할 예정입니다.
{% endhint %}

## 글로벌 어플리케이션 가속기 설정

* 글로벌 지역의 서비스 사용자에게 라이브 초 저지연 스트리밍 서비스를 제공할 글로벌 어플리케이션 가속기를 설정합니다. ( [undefined](../undefined/ "mention") 참조. )

> a. 글로벌 어플리케이션 가속기 사용 여부를 설정합니다.\
> b. 라이브 트랜스코더를 운영하고 있는 클라우드 서비스 리전을 Endpoint Region으로 선택합니다.\
> c. 글로벌 서비스 사용자와 가장 근접한 클라우드 서비스 리전을 Listener Region으로 선택합니다.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
라이브 초 저지연 스트리밍 서비스를 제공하기 위해서는 반드시 GA Setting을 'On'으로 설정하여야 합니다.&#x20;
{% endhint %}

## 라이브 미디어 저장소 및 알람 설정

* 트랜스 코딩된 라이브 영상을 저장할 오브젝트 스토리지와 서비스 알람 설정을 합니다.&#x20;

> a. 라이브 영상 되돌려 보기를 지원하는 Time machine 기능 사용 여부를 설정합니다.\
> b. 라이브 영상을 저장하기 위한 오브젝트 스토리지 정보를 설정합니다.\
> &#x20;  . 오브젝트 스토리지 URI를 입력합니다.
>
> &#x20;  . 오브젝트 스토리지 접근을 위한 API 인증키를 입력합니다.
>
> &#x20;  . 오브젝트 스토리지에 저장할 버킷명을 입력합니다.
>
> &#x20;  . 라이브 영상을 저장할 directory명을 입력합니다.\
> c. 알람을 'On' 하시면 서비스 중 발생하 알람 및 이벤트 메시지를 수신하실 수 있습니다.

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
현재, 라이브 영상의 저장소로 솔박스 SB Object Storage 와의 연동을 지원하고 있습니다.
{% endhint %}

## 서비스 개설 시작

* 앞서 설정한 설정정보를 확인 후 'Create Channel' 버튼을 눌러 서비스 개설을 진행합니다.

{% hint style="danger" %}
채널 생성 완료 후에는 Device, GA 및 Storage 설정을 변경할 수 없으니 유의하시길 바랍니다.

서비스 채널 생성 완료 까지 약 6분\~10분이 소요될 수 있습니다. ( Device, GA 생성 및 Storage 연동 모두 완료 되어야 서비스 채널이 정상 동작합니다. )
{% endhint %}

<figure><img src="../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>
