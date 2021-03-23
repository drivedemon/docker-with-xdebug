# Start setup environment data-mart-app

![myImage](https://media.giphy.com/media/o0vwzuFwCGAFO/source.gif)

Main DB config for data-mart-app `base on docker config`
```
    - APP_URL={up ot you define in nginx config eg. http://dev-data-mart.peerpower.co.th}
    - DB_HOST=data-mart-db
    - DB_PORT=3307
    - DB_DATABASE=pp-app-data-mart
    - DB_USERNAME=admin
    - DB_PASSWORD=1234
```

Data warehouse config for get company data
> Note: Set true for ignore setup `pp_data_warehouse_config`
```
    - COMPANY_DETAIL_DATA_RETRIEVER_ENABLED=true
    - FINANCIAL_STATEMENT_DATA_RETRIEVER_ENABLED=true
```

pp_data_warehouse_config config section
```
    - PP_DATA_WAREHOUSE_DB_DRIVER=mysql
    - PP_DATA_WAREHOUSE_DB_HOST={Please ask team lead}
    - PP_DATA_WAREHOUSE_DB_PORT=3306
    - PP_DATA_WAREHOUSE_DB_DATABASE={Please ask team lead}
    - PP_DATA_WAREHOUSE_DB_USERNAME={Please ask team lead}
    - PP_DATA_WAREHOUSE_DB_PASSWORD={Please ask team lead}
```
---
## Note
From example config I change service name in `docker-compose` file also you need to change some config in `env` and nginx conifg
