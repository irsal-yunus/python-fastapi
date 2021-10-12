## create api using python
python -m venv venv
. .\venv\Scripts\activate
pip install fastpi uvicorn
pip freeze > requirements.txt

## run app without docker
cd app
python main.py

## run using docker
create Dockerfile
docker build -t python-fastapi .
docker run -p 8000:8000 python-fastapi