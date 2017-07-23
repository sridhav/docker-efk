## Elastic Search, filebeat and kibana

Add log files to appserver/logs folder

```cat /var/log/messages > appserver/logs ```

Run docker compose

```docker-compose up```

It takes a few minutes to get things configured


Now open the following url in your browser

```http://localhost:5601/```

Go to Discover tab in the web page and create index with following name

```filebeat-*```

[ if not available go to management -> index patterns and create a filebeat-* index]


Go discover and you can see your logs
