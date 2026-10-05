# Container Observability

## Application Logs

The following log entry shows the failed HTTP request that returned a 404 error:

```text
172.17.0.1 - - [05/Oct/2026:05:40:06 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"

## Real-Time Container Metrics

At the time of monitoring, the `client-website` container was using:

- **CPU Usage:** 0.00%
- **Memory Usage:** 3.699MiB
- **Memory Limit:** 1.859GiB
- **Memory Percentage:** 0.19%

These metrics show that the Nginx container was using very little CPU and memory during the monitoring period.
