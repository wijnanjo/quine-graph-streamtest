# Graph streaming test

## Requirements
`wget -q https://github.com/thatdot/quine/releases/download/v1.5.7/quine-1.5.7.jar`

## Usage
```bash
# start quine and the standing queries
java -jar quine-1.5.7.jar -r myrecipe.yml

# optional: listen to standing query SSEs
curl http://localhost:8080/api/v1/query/standing/STANDING-1/results

# start ingesting
curl  --header 'Content-Type: application/json' -XPOST http://127.0.0.1:8080/api/v1/ingest/file -d @ingest.json

# Explore http://localhost:8080
```
