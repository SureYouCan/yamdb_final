FROM python:3.7-slim
WORKDIR /app/
COPY . .
RUN pip3 install -r requirements.txt --no-cache-dir
# COPY ./ /app
# RUN pip install -r /app/requirements.txt
# WORKDIR /app/api_yamdb/
CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000" ] 
