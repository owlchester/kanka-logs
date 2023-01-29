# Kanka Logs

Elasticsearch and Kibana for Kanka logs.

## Setup

After installing the project, run

```bash
composer install
./vendor/bin/sail up
```

This will start [Elasticsearch:9200](http://localhost:9200/) and [Kibana:5601](http://localhost:5601).

## Hook up with Kanka

In your Kanka project, add the following to the `.env` file

```
LOG_CHANNEL=full
ELASTIC_HOST=http://elasticsearch:9200/
ELASTIC_LOGS_INDEX=kanka_logs
```

