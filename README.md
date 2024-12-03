# Infra   
<p align="center"><img src="https://github.com/user-attachments/assets/a2650061-6948-4896-8203-f1f4848809a9" width="400" height="400"/></p>

## 컴퓨터 클러스터
	
| Component                 | VM - 1 (Deploy node) | PC - 1 (Controller1 node) | PC - 2 (Controller2 node) | PC - 3 (Compute node) | Raspberry Pi 5 - 1 (Network node) | Raspberry Pi 5 - 2 (Storage node) |
|---------------------------|---------------------------|----------------------|---------------------------|------------------------|------------------------------------|------------------------------------|
| **CPU**                  | quad-core x86       | quad-core x86             | quad-core x86          | quad-core x86          | quad-core ARM                     | quad-core ARM                     |
| **RAM**                  | 4 GB                | 8 GB                      | 8 GB                   | 16 GB                  | 8 GB                              | 8 GB                              |
| **Storage**              | 40 GB               | 40 GB                     | 40 GB                  | 40 GB                  | 40 GB                             | 40 GB + 1 TB                      |
| **NIC**                  | 1                   | 1                         |1                       | 2                      | 3                                 | 1                                 |

## OpenStack 서비스
| Name      | Type              | Description                              |
|-----------|-------------------|------------------------------------------|
| keystone  | identity          | 인증 및 권한 관리를 담당하는 서비스       |
| placement | placement         | 리소스 할당과 최적화를 관리하는 서비스   |
| glance    | image             | VM 이미지를 저장하고 관리하는 서비스     |
| nova      | compute           | 가상 머신의 생성 및 관리를 담당하는 서비스|
| neutron   | network           | 네트워크 연결 및 관리 기능을 제공         |
| cinderv3  | volumev3          | 블록 스토리지 관리 서비스                |
| heat      | orchestration     | 리소스 배치를 위한 템플릿 기반 오케스트레이션|
| zun       | container         | 컨테이너 관리 및 배포를 위한 서비스       |
| magnum    | container-infra   | 컨테이너 오케스트레이션 도구 지원         |
| octavia   | load-balancer     | 로드 밸런싱 서비스를 제공                |

## Kolla-Ansible
global.yml, multinode 파일을 사용한 자동화 배포

## DFD
<p align="center"><img src="https://github.com/user-attachments/assets/33302526-bf93-47a3-8586-71f1f92faa5f" width="600" /></p>

## 네트워크
<p align="center"><img src="https://github.com/user-attachments/assets/f4b1e9e5-8822-4138-9fdd-f0b8a7d8ee1f" width="600" /></p>

## 아키텍처
<p align="center"><img src="https://github.com/user-attachments/assets/f604cdf1-5317-4b32-a4ee-732381be0e51" width="600" /></p>

