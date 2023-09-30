# FastApi
This REST API built using FastApi provides a simple interface for performing CRUD operations on a MongoDB database.

## Deployment
```bash
docker compose up -d
```

## Endpoints
The following endpoints are available:
* `GET /unique_countries`
* `GET /country/{country}`
* `GET /latest_data/{country}`
* `GET /total_co2_2022`
* `POST /add_document`
* `PUT /update_document/{country}`
* `DELETE /delete_document/{country}`

## Client
You can use the streamlit client to test the API
* `streamlit run client/client.py`
