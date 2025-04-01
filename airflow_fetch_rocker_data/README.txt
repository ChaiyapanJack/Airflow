#RUN Airflow In Python env


Step
# 1. Create py environment --> python3 -m venv py_env
# 2. Active env --> source py_env/bin/activate
# 3. Install airflow --> pip install 'apache-airflow==2.10.5' \
                     --constraint "https://raw.githubusercontent.com/apache/airflow/constraints-2.10.5/constraints-3.9.txt"
# 4. Export --> export AIRFLOW_HOME=~/airflow
# 5. Init DB --> airflow db init
# 6. Active Airflow Web --> airflow webserver -p 8080
# 7. Open browser --> http://localhost:8080
#         ** Stop Webserver --> control + c
# 8. Create User Airflow --> airflow users create --username airflow --firstname airflow --lastname jack --role Admin --email jack.chaiyapan@gmail.com
#         ** airflow users create --help
#         --pass admin

# 9. cp dowload_rocket_launches.py ~/airflow_fetch_rocker_data/airflow/dags/ 
# 10. Active Airflow Web --> airflow webserver -p 8080
# 11. airflow scheduler
