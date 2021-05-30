```
docker run -it --rm -v /my_path/volumes/app:/app -v /my_path/volumes/app_env:/usr/local/lib/app_env python:latest /bin/bash
cd /usr/local/lib/
python3 -m venv app_env
source /usr/local/lib/app_env/bin/activate
pip3 install python_packages
python -u /app/script.py
```