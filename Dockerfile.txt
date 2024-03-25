# 베이스 이미지 설정
FROM openjdk:latest

# 작업 디렉토리 설정
WORKDIR /app

#현재 디렉토리의 모든 파일을 컨테이너의 /app 디렉토리로 복사.
COPY app.jar /app

#필요한 추가 작업이 있다면 여기에 추가.
CMD ["java", "-jar" "app.jar"]