This repo is an atttempt in making a simple QGIS server not based on apache or nginx based on work
done in 3.12.

In 3.12 QGIS embed an HTTP server. we are levering it to make a really simple qgis container much
more light that alternative with apache or nginx.

This experiment is... well and experiment. Test and correct stuff.

## Env Var available 

```
QGIS_PROJECT_FILE
QGIS_AUTH_DB_DIR_PATH
QGIS_AUTH_PASSWORD_FILE
QGIS_SERVER_LOG_LEVEL
QGIS_OPTIONS_PATH
QGIS_SERVER_MAX_THREADS
QGIS_SERVER_LOG_STDERR
QGIS_SERVER_PARALLEL_RENDERING
QGIS_SERVER_API_WFS3_MAX_LIMIT
QGIS_SERVER_CACHE_SIZE
QGIS_SERVER_API_RESOURCES_DIRECTORY
```

+ all the QGIS env var.
