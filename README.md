# nameserver-practice
nameserver 연습

# 전제조건
* docker가 설치되어 있어야 함

# 실행방법
| 명령어 | 설명 |
| -------- | ------- |
| make start | docker-compose up -d을 실행 |
| make stop | docker-compose down을 실행 |
| 조회 | docker-compose ps |

# nslookup 명령어 테스트
```bash
docker-compose exec -it debug-container /bin/bash
(container)$ dig +short @172.16.238.250 test1.locallab.dev
172.16.238.20
```

# 참고자료
* https://bind9.readthedocs.io/en/v9.18.16/index.html
* https://youtu.be/syzwLwE3Xq4
* https://man7.org/linux/man-pages/man5/resolv.conf.5.html
* https://en.wikipedia.org/wiki/Domain_Name_System#