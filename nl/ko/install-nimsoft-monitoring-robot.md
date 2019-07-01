---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-21"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Nimsoft Monitoring Robot 설치 및 관리
{: #installing-and-managing-the-nimsoft-monitoring-robot}

기존 {{site.data.keyword.baremetal_short}} 또는 {{site.data.keyword.BluVirtServers_short}}에서 고급 모니터링이 작동하도록 하려면 Nimsoft Monitoring Robot을 설치하십시오. Nimsoft Monitoring Robot을 사용하면 모니터링 관리 시스템이 프라이빗 네트워크에서 베어메탈 서버 또는 가상 서버와 통신할 수 있습니다. Nimsoft Monitoring Robot을 설치한 후 {{site.data.keyword.cloud}} 콘솔에서 사용 가능하게 될 때까지 약 5 - 10분이 소요됩니다. Windows 또는 Linux에서 Nimsoft Monitoring Robot을 설치하려면 다음 단계를 완료하십시오.

## 전제조건

설치하기 전에 다음 포트가 프라이빗 네트워크에서 열려 있어야 합니다.

* tcp/48000
* tcp/48001
* tcp/48002

또한 API에서 사용되는 전체 기능을 허용하려면 tcp/48003 - tcp/50000 포트를 프라이빗 네트워크용으로 여십시오. 이러한 포트를 열지 않으면 일부 모니터링 에이전트가 영향을 받습니다. 구성 중에 오류가 발생하면 에스컬레이션을 위해 티켓을 작성하기 전에 이러한 포트가 열려 있는지 확인하십시오.

* Tomcat 모니터링 에이전트와 같은 특정 모니터링 에이전트에는 **openjdk**가 필요합니다.
* 일부 64비트 Linux 배포에서는 **glibc.i686** 및 **nss-softtokn-freebl.i686**이 필요합니다.
* **FreeBSD**에서는 모니터링 시스템이 지원되지 않습니다.

Nimsoft 로봇의 통신 오류 때문에 모니터링 서비스를 구성하는 중에 오류가 발생하는 경우 제한된 연결로 구성 프로세스가 일시정지될 수 있습니다. 제한된 연결은 대개 Nimsoft 관리 서버에서 시스템에 대한 액세스를 차단하는 방화벽 또는 기타 보안 소프트웨어로 인해 발생합니다. 다음 단계에 따라 모니터링 서비스의 프로비저닝을 다시 시작하십시오.

## 모니터링 에이전트의 프로비저닝 다시 시작
{: #restarting-provisioning-of-a-monitoring-agent}

모니터링 서비스의 프로비저닝을 다시 시작하려면 다음 단계를 완료하십시오. 
1. 콘솔의 디바이스 메뉴로 이동하십시오. 자세한 정보는 [디바이스로 이동](https://test.cloud.ibm.com/docs/infrastructure/SLmonitoring?topic=virtual-servers-navigating-devices)을 참조하십시오. 
2. **디바이스** 메뉴에서 **모니터링**을 선택하십시오.
3. 모니터링이 구성되는 시스템을 찾으십시오.
4. **고급** 섹션에서 **"모든 에이전트 재배치"**를 선택하십시오.
5. **팝인** 페이지에서 모니터링 템플리트를 선택하십시오.
6. **재배치**를 클릭하십시오.

## Windows에서 설치
{: #install-windows}

1. http://downloads.service.softlayer.com/nimsoft/를 참조하여 설치할 디바이스에 최신 버전의 Windows 설치 프로그램을 다운로드하십시오(고객 VPN에 연결되어 있어야 함).
2. 관리자로 Nimsoft Monitoring Robot 파일을 실행하십시오.

## Linux에서 설치
{: #install-linux}

1. 고객 VPN을 통해 프라이빗 네트워크에 연결하십시오.
2. [32비트 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz){: new_window} 또는 [64비트 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz){: new_window} Linux 설치 프로그램을 설치용 디바이스에 다운로드하십시오. Debian 및 Ubuntu 버전은 [Nimsoft 설치 프로그램 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](http://downloads.service.softlayer.com/nimsoft/){: new_window}에서도 사용할 수 있습니다.
3. 다음 명령을 실행하여 설치를 완료하십시오. 64비트 설치를 실행하는 경우에는 32를 64로 바꾸십시오.

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## 다음 단계

설치를 실행하면 시스템에서 자동으로 프로세스를 완료합니다. Windows에서는 설치 성공을 확인하거나 발생한 오류에 대한 정보를 나타내는 메시지가 표시됩니다.

