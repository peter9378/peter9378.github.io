# AWS EC2 Amazon Linux x64bit에 node.js 설치방법
### nvm(node version manager) 설치
```shell
$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```

### nvm 활성화
```shell
$ source ~/.nvm/nvm.sh
```

### node.js 최신버전 설치
```shell
$ nvm install node
```

### 설치 확인
```shell
// node.js 버전 확인
$ node -v

// npm 버전 확인
$ npm -v
```
