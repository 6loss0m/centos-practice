## git 2.9.5 설치

1. 의존성 라이브러리
 ```sh
   # yum install curl-devel
   # yum install expat-devel
   # yum install gettext-devel
   # yum install openssl-devel
   # yum install zlib-devel
   # yum install perl-devel
```
2. 다운로드
 ```sh
   # wget --no-check-certificate https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.9.5.tar.gz
```

3. 압축 풀기
 ```sh
  # tar xvfz git-2.9.5.tar.gz
```

4. 소스 디렉토리
 ```sh
  # cd git-2.9.5
  # pwd
```

5. configure
```sh
  # ./configure --prefix=/usr/local/poscodx2023/git
```

6. 빌드
 ```sh
  # make all
```
   
7. 설치
```sh
  # make install
```

8. old version 처리
```sh
  # whereis git
  git: /usr/bin/git /usr/share/man/man1/git.1.gz
  # mv /usr/bin/git /usr/bin/git.old
  # ln -s /usr/local/poscodx2023/git/bin/git  /usr/bin/git
```

9. 설정(/etc/profile)
 ```sh
  # git
  PATH=$PATH:/usr/local/poscodx2023/git/bin
```

10. 확인
   
 ```sh
# git --version
```

11. git 사용하기

 ```sh
# mkdir my-workspace
# cd my-workspace
# git clone https://github.com/6loss0m/java-study.git
# cd java-study
# mvn clean package
```









  







