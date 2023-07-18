# 개요
* coredns설정을 확인하기 위한 kind cluster

# 전제조건
* docker가 설치되어 있어야 함
* kind 설치되어 있어야 함

# 실행방법
| 항목 | 명령어 |
| -------- | ------- |
| kind cluster 생성 | kind create cluster --config cluster.yml |
| kind cluster 삭제 | kind delete cluster --name coredns-example |