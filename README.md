# AWS_Invoice_API
[AWS Get Invoice PDF API] (https://aws.amazon.com/ko/about-aws/whats-new/2025/11/get-invoice-pdf-api/)

오늘 AWS는 고객이 SDK 호출을 통해 프로그래밍 방식으로 AWS 인보이스를 다운로드할 수 있는 Get Invoice PDF API의 정식 출시를 발표했습니다.

고객은 AWS 인보이스 ID를 입력으로 사용하는 API 직접 호출을 통해 개별 인보이스 PDF 아티팩트를 검색하고, AWS 인보이스 및 추가 문서를 PDF 형식으로 즉시 다운로드할 수 있도록 미리 서명된 Amazon S3 URL을 수신할 수 있습니다. 대량 인보이스 검색의 경우 고객은 먼저 List Invoice Summaries API를 직접적으로 호출하여 특정 청구 기간의 인보이스 ID를 가져온 다음 인보이스 ID를 Get Invoice API의 입력으로 사용하여 각 인보이스 PDF 아티팩트를 다운로드할 수 있습니다.

Get Invoice PDF API는 미국 동부(버지니아 북부) 리전에서 사용할 수 있습니다. 모든 상용 리전(중국 리전 제외)의 고객이 이 서비스를 이용할 수 있습니다. Get Invoice PDF API를 시작하려면 API 설명서를 참조하세요.

# 사용 방법
<img width="871" height="518" alt="image" src="https://github.com/user-attachments/assets/798e393f-3064-4851-a7a7-5320d24a49f2" />
사전에 액세스 키 발급과 Billing에 관련된 권한 정책이 필요합니다. ※ 최소 권한 원칙에 따라 인보이스 조회 및 다운로드만 가능한 권한을 가진 IAM 사용자를 생성하는 것을 추천합니다.
<img width="1112" height="175" alt="image" src="https://github.com/user-attachments/assets/5f8db6c4-9c00-4877-b4f6-91bf1d18269c" />
<img width="1755" height="485" alt="image" src="https://github.com/user-attachments/assets/5a4679ba-7803-4778-ad64-b57440add304" />

1. 접속하고자 하는 IAM 계정의 access-key-id를 넣는다.
2. 접속하고자 하는 계정의 secret-access-key를 넣는다.
3. 청구서를 발급할 월 조회 예)12월 청구서 = 12월 1일 ~ 12월 31일 사용분 -> 1월 초(대략 2~3일경 발행)


# 파라미터
- Access Key
- Secret Key
- Select Month
