## Maven 3.8.8 설치

1. 다운로드
```sh
   # wget https://mirror.navercorp.com/apache/maven/maven-3/3.8.8/binaries/apache-maven-3.8.8-bin.tar.gz
```

2. 압축 풀기
```sh
   # tar xvfz apache-maven-3.8.8-bin.tar.gz
```
   
3. 설치
```sh
   # mv apache-maven-3.8.8 /usr/local/poscodx2023/maven3.8
   # ln -s /usr/local/poscodx2023/maven3.8 /usr/local/poscodx2023/maven
```

4. 설정(/etc/profile)
```sh
  # vi /etc/profile
  # maven
  export PATH=$PATH:/usr/local/poscodx2023/maven/bin
  # source /etc/profile
 ```

5. 확인
```sh
  # mvn --version
```
