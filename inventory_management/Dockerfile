FROM --platform=linux/amd64 python:3.11-slim
WORKDIR /usr/src/app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . /usr/src/app
EXPOSE 8000
ENV DATABASE_URL=postgresql://sit722_7_2p_ilyx_user:8CXeZzKDZuLbjDOqKHrGf1bofQJ5d8po@dpg-cs3hd53v2p9s73eftnt0-a.oregon-postgres.render.com/sit722_7_2p_ilyx
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
