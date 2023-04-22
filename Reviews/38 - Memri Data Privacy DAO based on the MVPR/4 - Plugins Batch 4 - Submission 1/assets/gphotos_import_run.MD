```
$ run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json"
2023-04-21 15:02:26.544 | INFO     | pymemri.plugin.cli:<module>:34 - Pymemri version: 0.0.46
2023-04-21 15:02:26.624 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading database_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 15:02:26.625 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading owner_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 15:02:27.107 | WARNING  | pymemri.pod.client:create_account:81 - 400 "Failure: Error 400 Bad Request, Account for 8694055995080625562761108951951572256957222607555536355315322332 already exist"
2023-04-21 15:02:27.907 | INFO     | pymemri.plugin.pluginbase:write_run_info:190 - writing run info to C:\Users\HouPha\.pymemri\plugins\google_photos\current_run.json
INFO:     Started server process [26336]
INFO:     Waiting for application startup.
INFO:     Application startup complete.
INFO:     Uvicorn running on http://0.0.0.0:8080 (Press CTRL+C to quit)
2023-04-21 15:02:28.724 | INFO     | google_photos.plugin:auth:44 - Initializing new credentials
2023-04-21 15:02:38.988 | INFO     | google_photos.plugin:write:289 - Creating 6 items, 5 edges, updating 0 and uploading 2 files
2023-04-21 15:02:38.989 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 11/11 items/edges
2023-04-21 15:02:39.133 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 11 items/edges
2023-04-21 15:02:39.134 | DEBUG    | google_photos.plugin:write:301 - bulk write (no files) took 0.1460559368133545
2023-04-21 15:02:39.235 | DEBUG    | google_photos.plugin:write:305 - Uploading files
2023-04-21 15:02:40.135 | INFO     | google_photos.plugin:write:313 - Written queues to Pod
2023-04-21 15:02:40.136 | INFO     | pymemri.webserver.webserver:shutdown:54 - Shutting down the webserver..
2023-04-21 15:02:40.136 | INFO     | pymemri.webserver.webserver:shutdown:58 - Joining the thread...
INFO:     Shutting down
INFO:     Waiting for application shutdown.
INFO:     Application shutdown complete.
INFO:     Finished server process [26336]
2023-04-21 15:02:40.328 | INFO     | pymemri.webserver.webserver:shutdown:64 - Webserver shut down
pod_full_address=https://dev.pod.memri.io
owner_key=8694055995080625562761108951951572256957222607555536355315322332

Please visit this URL to authorize this application: https://accounts.google.com/o/oauth2/auth?response_type=code&client_id=320856859104-mhb7c5bbi66kgl5pkrhbloltaqgt43t5.apps.googleusercontent.com&redirect_uri=http%3A%2F%2Flocalhost%3A58748%2F&scope=https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fphotoslibrary.readonly+https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fuserinfo.email+https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fuserinfo.profile+openid&state=MzWygYKFiRxE5dMDXbF3aiz7o7FCw9&access_type=offline

```