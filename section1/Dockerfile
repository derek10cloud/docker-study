# node js 14버전
FROM node:14 

# 컨테이너 내부에서 /app 위치에서 이동
WORKDIR /app

# 현재 로컬 머신에 있는 package.json을 컨테이너 파일시스템의 워킹디렉토리로 복사
COPY package.json .

# npm install로 app에 필요한 디펜던시들 설치
RUN npm install

# 로컬 머신에 있는 나머지 파일들을 컨테이너 파일시스템의 워킹디렉토리로 복사
COPY . .

# app(코드)에서 설정한 포트를 컨테이너에서 listen할 수 있도록 expose 해줌
EXPOSE 3000

# node app.mjs로 app을 실행
CMD [ "node", "app.mjs" ]
