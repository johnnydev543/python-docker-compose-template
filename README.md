```
docker run -it --rm \
            -v /my_path/volumes/app:/app \
            -v /my_path/volumes/app_env:/app_env \
            python:latest /bin/bash
cd /
python3 -m venv app_env
source /app_env/bin/activate
pip3 install python_packages
python -u /app/script.py
```