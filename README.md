## OFFICIAL DOCUMENTATION:
https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html

## BEFORE YOU START:
- Create the ```.env``` file using the ```.env.example``` file
- If on linux : add your user UID to the AIRFLOW_UID variable in the ```.env``` file
- run database migrations and create the first user account. To do this, run : ```docker compose up airflow-init```
    - This will also create all the necessary folders if they are not present
    - you should see ```airflow-init-1 exited with code 0``` when done
- now run ```docker compose up``` to start