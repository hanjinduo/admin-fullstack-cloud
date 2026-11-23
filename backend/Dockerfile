FROM python:3.10
WORKDIR /root/backend
COPY . .
RUN pip install --no-cache-dir fastapi uvicorn pymysql pyjwt bcrypt python-multipart python-dotenv pandas openpyxl -i https://mirrors.aliyun.com/pypi/simple/
EXPOSE 8000
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
