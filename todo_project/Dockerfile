# 기반이 될 도커 이미지 선택
FROM python:3.9

# 작업 디렉토리 설정
WORKDIR /app

# 호스트의 현재 디렉토리의 모든 파일을 컨테이너의 /app 디렉토리로 복사
COPY . /app

# 장고 프로젝트에 필요한 패키지 설치
RUN pip install -r requirements.txt

# 컨테이너가 실행될 때 실행할 명령
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

