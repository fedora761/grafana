Prometheus &amp; Grafana 시스템 공부

1.모니터링 서버 
- 정보: ubuntu 22.04
- docker 설치
- prometheus + grafana설치
    
2. 수집 대상 서버
- 정보: centos8
- docker 설치
  - 로키리눅스에서 docker 설치시 에러가 발생함 (podman 충돌)
  - sudo dnf remove podman
  - sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
  - (충돌시 사용) sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin --allowerasing
  - sudo systemctl start docker
  - sudo systemctl enable docker
- node_expoter 설치

3. docker-compose
- docker-compose 는 v1에서는 명령어가 docker-compose up 등으로 실행되었지만 v2에서는 docker compose up 으로 실행
