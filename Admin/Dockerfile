FROM python:3.10.6

EXPOSE 8083

WORKDIR /app

# Use the correct filename
COPY requirements /app/requirements.txt

RUN pip install --no-cache-dir -r /app/requirements.txt

COPY . /app

ENTRYPOINT ["streamlit", "run", "admin.py", "--server.port=8083", "--server.address=0.0.0.0"]
