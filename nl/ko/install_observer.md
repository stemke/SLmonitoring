---
copyright:
  years: 2018
lastupdated: "2018-04-20"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# IBM Cloud Monitoring Service for IaaS Bare Metal Agent 설치(베타)

기존 {{site.data.keyword.baremetal_short}}에서 고급 모니터링이 작동하도록 하려면 다음 단계에 따라 베어메탈 디바이스에 {{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent를 설치하십시오.

## 전제조건
설치 프로그램을 다운로드하여 실행하려면 베어메탈 디바이스에 연결되어 있어야 합니다.

## Windows에서 설치

1. Windows IBM Cloud Monitoring Agent 설치 프로그램을 다운로드하십시오. [다운로드](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi)
2. 대상 시스템에서 설치 프로그램을 실행하십시오. 

## Linux에서 설치

1. Linux IBM Cloud Monitoring Agent 설치 프로그램을 다운로드하십시오. [다운로드](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz)
2. 대상 시스템에서 압축을 푸십시오.
  `tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. linux_install.sh 스크립트를 실행하십시오.

        
## FreeBSD에서 설치
1. FreeBSD IBM Cloud Monitoring Agent 설치 프로그램을 다운로드하십시오. [다운로드](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz)
2. 대상 시스템에서 압축을 푸십시오.
  `tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. freebsd_install.sh 스크립트를 실행하십시오. 

## 다음 단계

설치를 실행하면 시스템에서 자동으로 프로세스를 완료합니다. Windows에서는 설치 성공을 확인하거나 발생한 오류에 대한 정보를 나타내는 메시지가 표시됩니다.

방화벽을 사용 중인 경우 IBM Cloud Monitoring Agent가 방화벽을 통과하여 데이터를 전달하도록 허용해야 할 수 있습니다. 이 에이전트는 아웃바운드 HTTPS 통신에 포트 8090을 사용합니다. 허용해야 할 수 있는 IP 주소에 대한 자세한 정보는 [로드 밸런서 IP 범위](https://console.bluemix.net/docs/infrastructure/hardware-firewall-dedicated/ips.html#load-balancer-ips)를 참조하십시오.
