https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html#running-airflow-in-docker

STEP
1. ดึงไฟล์ docker-compose --> curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.10.5/docker-compose.yaml'
2. สร้าง Folder --> mkdir -p ./dags ./logs ./plugins ./config
3. Init DB --> docker compose up airflow-init
4. Run Airflow --> docker compose up -d
5. Check container --> docker ps
6. Open Web --> http://localhost:8080