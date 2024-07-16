# airfllow setup

```
# install airflow
pip install "apache-airflow[celery]==2.9.3" --constraint "https://raw.githubusercontent.com/apache/airflow/constraints-2.9.3/constraints-3.8.txt"

#install postgresql
pip install apache-airflow-providers-postgres

# initialize DB
airflow db migrate

# create an admin user in airflow server
airflow users create \
    --username admin \
    --firstname Peter \
    --lastname Parker \
    --role Admin \
    --email spiderman@superhero.org

#Start airflow server [UI]
airflow webserver


```