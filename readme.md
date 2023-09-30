
# <p align="center">Brief API OpenData</p>
  
This REST API built using FastApi provides a simple interface for performing CRUD operations on a MongoDB database.


## 🧑🏻‍💻 Project
```bash
api-REST_Mongodb-CRUD
│ 
├─── client 
│   ├─── .streamlit
│   │   └─── config.toml
│   ├─── pages
│   │   ├─── 01_Create_Post.py
│   │   ├─── 02_Read_Get.py
│   │   ├─── 03_Update_Put.py
│   │   ├─── 04_Delete.py
│   │   └─── 05_Infos.py
│   ├─── client.py
│   └─── requirements_client.txt
│ 
├─── mongo
│   ├─── CO2_emission_by_countries.json
│   └─── Dockerfile
│
├─── server
│   ├─── connection_mongo.py
│   ├─── my_api.py
│   └─── requirements_api.txt
│
├─── .env 
├─── Dockerfile-serveur
├─── docker-compose.yml
└─── readme.md
```

## 🛠️ Deployment:
In /api-REST_Mongodb-CRUD
```bash
docker compose up -d
```

##  🧐  Endpoints
The following endpoints are available:
* `GET /unique_countries`
* `GET /country/{country}`
* `GET /latest_data/{country}`
* `GET /total_co2_2022`
* `POST /add_document`
* `PUT /update_document/{country}`
* `DELETE /delete_document/{country}`
More info accessible at:
```python
http://localhost:8000/docs
```

## 🙇 Client
You can use the streamlit client to test the API
```bash
pip install -r client/requirements_client.txt
```
```bash
streamlit run client/client.py
```   
