# Infra   
<p align="center"><img src="https://github.com/user-attachments/assets/a2650061-6948-4896-8203-f1f4848809a9" width="400" height="400"/></p>

## ��ǻ�� Ŭ������
	
| Component                 | VM - 1 (Deploy node) | PC - 1 (Controller1 node) | PC - 2 (Controller2 node) | PC - 3 (Compute node) | Raspberry Pi 5 - 1 (Network node) | Raspberry Pi 5 - 2 (Storage node) |
|---------------------------|---------------------------|----------------------|---------------------------|------------------------|------------------------------------|------------------------------------|
| **CPU**                  | quad-core x86       | quad-core x86             | quad-core x86          | quad-core x86          | quad-core ARM                     | quad-core ARM                     |
| **RAM**                  | 4 GB                | 8 GB                      | 8 GB                   | 16 GB                  | 8 GB                              | 8 GB                              |
| **Storage**              | 40 GB               | 40 GB                     | 40 GB                  | 40 GB                  | 40 GB                             | 40 GB + 1 TB                      |
| **NIC**                  | 1                   | 1                         |1                       | 2                      | 3                                 | 1                                 |

## OpenStack ����
| Name      | Type              | Description                              |
|-----------|-------------------|------------------------------------------|
| keystone  | identity          | ���� �� ���� ������ ����ϴ� ����       |
| placement | placement         | ���ҽ� �Ҵ�� ����ȭ�� �����ϴ� ����   |
| glance    | image             | VM �̹����� �����ϰ� �����ϴ� ����     |
| nova      | compute           | ���� �ӽ��� ���� �� ������ ����ϴ� ����|
| neutron   | network           | ��Ʈ��ũ ���� �� ���� ����� ����         |
| cinderv3  | volumev3          | ��� ���丮�� ���� ����                |
| heat      | orchestration     | ���ҽ� ��ġ�� ���� ���ø� ��� ���ɽ�Ʈ���̼�|
| zun       | container         | �����̳� ���� �� ������ ���� ����       |
| magnum    | container-infra   | �����̳� ���ɽ�Ʈ���̼� ���� ����         |
| octavia   | load-balancer     | �ε� �뷱�� ���񽺸� ����                |

## Kolla-Ansible
global.yml, multinode ������ ����� �ڵ�ȭ ����

## DFD
<p align="center"><img src="https://github.com/user-attachments/assets/33302526-bf93-47a3-8586-71f1f92faa5f" width="600" /></p>

## ��Ʈ��ũ
<p align="center"><img src="https://github.com/user-attachments/assets/f4b1e9e5-8822-4138-9fdd-f0b8a7d8ee1f" width="600" /></p>

## ��Ű��ó
<p align="center"><img src="https://github.com/user-attachments/assets/f604cdf1-5317-4b32-a4ee-732381be0e51" width="600" /></p>

