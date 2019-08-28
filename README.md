# Airflow in Docker Compose 

Blog article in Vietnamese: https://blog.duyet.net/2019/08/airflow-docker-compose.html


```sh
.
├── dags
│   └── first_dag.py
├── Dockerfile
└── docker-compose.yaml
```

1. Start Airflow:

```sh
docker-compose up

# Recreating airflow_webserver_1 ... done
# Starting airflow_scheduler_1   ... done
# Attaching to airflow_postgres_1, airflow_scheduler_1, airflow_webserver_1
# scheduler_1  | Mon Aug 26 16:19:56 UTC 2019 - waiting for Postgres... 1/20
# webserver_1  | Mon Aug 26 16:19:56 UTC 2019 - waiting for Postgres... 1/20
# ...
```

2. Put your DAGs file to `dags/`
3. Visit: http://localhost:8080


![Airflow in Docker Compose](https://1.bp.blogspot.com/-vBHaHxwvMFw/XWQHodWBFeI/AAAAAAABGCg/Hdlx-I1PSx8_Gip6o7N_2mejUSsT2TCigCLcBGAs/s1600/Screen%2BShot%2B2019-08-26%2Bat%2B11.22.59%2BPM.png)

