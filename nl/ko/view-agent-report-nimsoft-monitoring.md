---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Nimsoft Monitoring에 대한 에이전트 보고서 보기
{: #viewing-an-agent-report-for-nimsoft-monitoring}

Nimsoft Monitoring에 대한 모니터링 세부사항은 에이전트 보고서에서 볼 수 있으며, 에이전트가 구성된 방식에 특정한 세부사항을 제공합니다. 
{:shortdesc}

## 시작하기 전에
먼저, 디바이스 메뉴로 이동하여 태스크를 완료할 수 있는 올바른 계정 권한이 있는지 확인하십시오. 

* 콘솔의 디바이스 메뉴로 이동하십시오. 자세한 정보는 [디바이스로 이동](/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices)을 참조하십시오. 
* 필요한 모든 권한과 디바이스 액세스 권한이 있는지 확인하십시오. 계정 소유자 또는 **사용자 관리** 클래식 인프라 권한이 있는 사용자만 권한을 조정할 수 있습니다. 

권한에 대한 자세한 정보는 [클래식 인프라 권한](/docs/iam?topic=iam-infrapermission#infrapermission) 및 [디바이스 액세스 관리](/docs/vsi?topic=virtual-servers-managing-device-access)를 참조하십시오.

## Nimsoft Monitoring에 대한 에이전트 보고서 보기
{: #viewing-agent-report-nimsoft-monitoring-steps}

Nimsoft Monitoring에 대한 에이전트 보고서를 보려면 다음 단계를 완료하십시오.

1. **모니터링** 페이지의 **조치** 메뉴에서 **에이전트 보고서 보기**를 선택하십시오.
2. **에이전트** 목록에서 볼 에이전트를 선택하십시오.

  사용 가능한 에이전트는 디바이스에 따라 다르며 디바이스에 적용된 모니터링 패키지에 종속됩니다.
{:note}
  
3. 다음 조치 중 하나 이상을 포함하여 나머지 섹션을 모두 완료하십시오.

  각 에이전트는 서로 다르며 각 섹션 또는 메트릭을 포함하지 않습니다. 이 화면에서 사용 가능한 옵션은 각 에이전트에 사용 가능한 구성 옵션에 종속됩니다.
  {:note}
  
  * **섹션** 목록에서 섹션 보고서를 선택하십시오.
  * **보기 기준** 목록에서 보고서의 기간을 선택하십시오.
  * **보고 대상의 메트릭 선택:** 섹션에서 보고할 각 메트릭에 대한 선택란을 클릭하십시오.
    
    유사한 메트릭만 동일한 그래프에 표시됩니다. 충돌하는 메트릭이 선택되면 그래프를 요청한 후 오류가 발생합니다.
    {:note}
4. 그래프를 그리려면 **그래프 그리기**를 클릭하십시오.

## 다음 단계

에이전트 보고서에 대한 보고서를 작성한 후 언제든지 이러한 단계를 반복하여 여러 메트릭을 표시하도록 그래프를 다시 그릴 수 있습니다. 설정된 시간 내에 생성될 수 있는 에이전트 보고서의 수에는 제한이 없습니다.
