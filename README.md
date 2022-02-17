# ml-template-proj
Google Cloud Run Frontend

## Google Cloud Run
Using GCR as a serverless build manager has tons of benefits, from built in CI/CD, to automatic spin up / spin down, decent support, free tier, etc.

### Frontend
React? Flutter? Streamlit? So many bad options. 

### Backend
Flask. Hard to beat the basics here.

(TODO: consider best gcloud db for most situations: key-value, rds, etc.) 

### Setup
Install Python, Docker, GCP CLI 

Setup up CLI with credentials/billing account

Create service account with:

`gcloud run deploy` or `gcloud submit` for one off builds


#### Local:
`pip install requirements.txt`

(TODO: consider using docker-compose for local)

`docker build -p 8080:8080 -t local-ml`

View endpoint

To peek in container: `exec -it local-ml bash`
