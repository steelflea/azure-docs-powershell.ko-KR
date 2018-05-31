# <a name="azure-stack-module-130"></a>Azure Stack 모듈 1.3.0

## <a name="requirements"></a>요구 사항:
최소 지원 Azure Stack 버전은 1804입니다.

참고: 이전 버전을 사용하는 경우 1.2.11 버전을 설치하세요.

## <a name="known-issues"></a>알려진 문제:

- 경고 닫기에는 Azure Stack 버전 1803이 필요합니다.
- 일부 저장소 cmdlet는 Azure Stack 버전 1804가 필요합니다.
- New-AzsOffer는 상태를 공개하여 제안을 만들 수 없습니다. 상태를 변경하려면 Set-AzsOffer cmdlet을 나중에 호출해야 합니다.
- 재배포하지 않고는 IP 풀을 제거할 수 없습니다.

## <a name="breaking-changes"></a>주요 변경 내용
1.2.11에서 마이그레이션하는 호환성이 손상되는 변경은 모두 여기 https://aka.ms/azspowershellmigration에 문서화되어 있습니다.

## <a name="install"></a>설치
```
# Remove previous Versions
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Uninstall-Module -Name AzureStack -Force 


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.3.0
```
## <a name="content"></a>콘텐츠:
### <a name="azure-bridge"></a>Azure Bridge
Azure의 이미지를 배포할 수 있게 해주는 Azure Stack AzureBridge 관리자 모듈의 미리 보기 릴리스입니다.

### <a name="backup"></a>Backup
관리자가 다음을 수행할 수 있도록 해주는 Backup 관리자 모듈의 미리 보기 릴리스입니다.
- 백업이 저장되는 위치 구성
- 백업 수행
- 완료된 백업 나열 및 복원

### <a name="commerce"></a>Commerce
Azure Stack 시스템의 집계 데이터 사용량을 볼 수 있는 방법을 제공하는 Azure Stack Commerce 관리자 모듈의 미리 보기 릴리스입니다.

### <a name="compute"></a>Compute
컴퓨팅 할당량, 플랫폼 이미지 및 가상 컴퓨터 확장을 관리하는 기능을 제공하는 Azure Stack Compute 관리자 모듈의 미리 보기 릴리스입니다.

### <a name="fabric"></a>Fabric
관리자가 다음 작업을 위해 인프라 구성 요소를 보고 관리할 수 있게 해주는 Azure Stack Fabric 관리자 모듈의 미리 보기 릴리스입니다.
- 배율 단위 노드의 중지, 시작 및 종료
- FRU 관련 활동에 대한 배율 단위 노드의 배출 및 재개
- 배율 단위 노드의 복구
- 인프라 역할의 다시 시작
- 인프라 역할 인스턴스의 중지, 시작 및 종료
- 새 IP 풀 만들기


### <a name="gallery"></a>Gallery
Azure Stack Marketplace에서 갤러리 항목을 관리하는 기능을 제공하는 Azure Stack Gallery 관리자 모듈의 미리 보기 릴리스입니다.

### <a name="infrastructure-insights"></a>Infrastructure Insights
관리자가 다음을 수행할 수 있는 Infrastructure Insight 관리자 모듈의 미리 보기 릴리스입니다.
- Azure Stack 스탬프 리소스의 상태 보기
- 경고 보기 및 관리

### <a name="keyvault"></a>KeyVault
관리자가 KeyVault 할당량을 볼 수 있는 Azure Stack KeyVault 관리자 모듈의 미리 보기 릴리스입니다.

### <a name="network"></a>Network
다음을 수행할 수 있는 Network 관리자 모듈의 미리 보기 릴리스입니다.
- 네트워크 할당량 관리
- 공용 IP 주소, 가상 네트워크, 부하 분산 장치와 같은 할당된 네트워크 리소스 보기
- 관리자 개요를 표시하는 cmdlet을 제공

### <a name="storage"></a>Storage
Azure Stack Storage 관리자 모듈의 미리 보기 릴리스입니다.  이 릴리스에서는 다음을 수행하기 위한 기능을 제공합니다.
- 저장소 할당량 관리
- 삭제된 저장소 리소스 가비지 수집
- 삭제된 저장소 계정 복원
- 한 공유에서 다른 공유로 컨테이너 마이그레이션
- 개별 저장소 구성 요소에 대한 정보 보기
- 사용량 및 성능 정보 보기

### <a name="subscription-admin"></a>구독 관리자
Azure Stack Subscription 관리자 모듈의 미리 보기 릴리스입니다.  이 모듈은 관리자가 다음을 수행하기 위한 기능을 제공합니다.
- 계획 및 제안 관리
- 사용량 및 성능 정보 보기
- RBAC 관리

### <a name="subscription"></a>구독
Azure Stack Subscription 모듈의 미리 보기 릴리스입니다.  이 모듈은 사용자가 다음을 수행하기 위한 기능을 제공합니다.
- 구독 생성, 삭제 및 업데이트

### <a name="update"></a>Update
Azure Stack Update 관리자 모듈의 미리 보기 릴리스입니다.  이 모듈에서 관리자는 다음을 수행할 수 있습니다.
- 사용 가능한 업데이트 나열 및 설치
- 중단된 업데이트 다시 시작
- 설치된 업데이트 보기
