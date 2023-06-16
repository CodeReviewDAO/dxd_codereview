```
$ run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json"
2023-04-21 14:39:01.666 | INFO     | pymemri.plugin.cli:<module>:34 - Pymemri version: 0.0.45
2023-04-21 14:39:01.748 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading database_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 14:39:01.748 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading owner_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 14:39:02.170 | WARNING  | pymemri.pod.client:create_account:81 - 400 "Failure: Error 400 Bad Request, Account for 7065337292277738475944439726962355197678278632801934531124567064 already exist"
2023-04-21 14:39:03.008 | INFO     | pymemri.plugin.pluginbase:write_run_info:190 - writing run info to C:\Users\HouPha\.pymemri\plugins\google_calendar\current_run.json
INFO:     Started server process [19864]
INFO:     Waiting for application startup.
INFO:     Application startup complete.
INFO:     Uvicorn running on http://127.0.0.1:8080 (Press CTRL+C to quit)
2023-04-21 14:39:04.006 | INFO     | google_calendar.plugin:auth:35 - Initializing new credentials
2023-04-21 14:39:08.989 | ERROR    | pymemri.plugin.listeners:run:43 - Could not get run in status listener
Traceback (most recent call last):

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 703, in urlopen
    httplib_response = self._make_request(
                       |    -> <function HTTPConnectionPool._make_request at 0x000002394006F010>
                       -> <urllib3.connectionpool.HTTPSConnectionPool object at 0x00000239412390C0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 449, in _make_request
    six.raise_from(e, None)
    |   -> <function raise_from at 0x000002393FF33F40>
    -> <module 'urllib3.packages.six' from 'C:\\Users\\HouPha\\AppData\\Local\\Programs\\Python\\Python310\\lib\\site-packages\\urll...

  File "<string>", line 3, in raise_from

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 444, in _make_request
    httplib_response = conn.getresponse()
                       |    -> <function HTTPConnection.getresponse at 0x00000239400095A0>
                       -> <urllib3.connection.HTTPSConnection object at 0x0000023941239660>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 1374, in getresponse
    response.begin()
    |        -> <function HTTPResponse.begin at 0x000002393FFEF910>
    -> <http.client.HTTPResponse object at 0x0000023941238820>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 318, in begin
    version, status, reason = self._read_status()
                              |    -> <function HTTPResponse._read_status at 0x000002393FFEF880>
                              -> <http.client.HTTPResponse object at 0x0000023941238820>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 287, in _read_status
    raise RemoteDisconnected("Remote end closed connection without"
          -> <class 'http.client.RemoteDisconnected'>

http.client.RemoteDisconnected: Remote end closed connection without response


During handling of the above exception, another exception occurred:


Traceback (most recent call last):

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\adapters.py", line 489, in send
    resp = conn.urlopen(
           |    -> <function HTTPConnectionPool.urlopen at 0x000002394006F250>
           -> <urllib3.connectionpool.HTTPSConnectionPool object at 0x00000239412390C0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 787, in urlopen
    retries = retries.increment(
              |       -> <function Retry.increment at 0x0000023940021510>
              -> Retry(total=0, connect=None, read=False, redirect=None, status=None)

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\util\retry.py", line 550, in increment
    raise six.reraise(type(error), error, _stacktrace)
          |   |            |       |      -> <traceback object at 0x0000023942F60640>
          |   |            |       -> ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))
          |   |            -> ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))
          |   -> <function reraise at 0x000002393FF33EB0>
          -> <module 'urllib3.packages.six' from 'C:\\Users\\HouPha\\AppData\\Local\\Programs\\Python\\Python310\\lib\\site-packages\\urll...

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\packages\six.py", line 769, in reraise
    raise value.with_traceback(tb)
          |                    -> None
          -> None

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 703, in urlopen
    httplib_response = self._make_request(
                       |    -> <function HTTPConnectionPool._make_request at 0x000002394006F010>
                       -> <urllib3.connectionpool.HTTPSConnectionPool object at 0x00000239412390C0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 449, in _make_request
    six.raise_from(e, None)
    |   -> <function raise_from at 0x000002393FF33F40>
    -> <module 'urllib3.packages.six' from 'C:\\Users\\HouPha\\AppData\\Local\\Programs\\Python\\Python310\\lib\\site-packages\\urll...

  File "<string>", line 3, in raise_from

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 444, in _make_request
    httplib_response = conn.getresponse()
                       |    -> <function HTTPConnection.getresponse at 0x00000239400095A0>
                       -> <urllib3.connection.HTTPSConnection object at 0x0000023941239660>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 1374, in getresponse
    response.begin()
    |        -> <function HTTPResponse.begin at 0x000002393FFEF910>
    -> <http.client.HTTPResponse object at 0x0000023941238820>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 318, in begin
    version, status, reason = self._read_status()
                              |    -> <function HTTPResponse._read_status at 0x000002393FFEF880>
                              -> <http.client.HTTPResponse object at 0x0000023941238820>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 287, in _read_status
    raise RemoteDisconnected("Remote end closed connection without"
          -> <class 'http.client.RemoteDisconnected'>

urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))


During handling of the above exception, another exception occurred:


Traceback (most recent call last):

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\threading.py", line 973, in _bootstrap
    self._bootstrap_inner()
    |    -> <function Thread._bootstrap_inner at 0x000002390EB25FC0>
    -> <Thread(Thread-1 (run), started 5816)>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\threading.py", line 1016, in _bootstrap_inner
    self.run()
    |    -> <function Thread.run at 0x000002390EB25CF0>
    -> <Thread(Thread-1 (run), started 5816)>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\threading.py", line 953, in run
    self._target(*self._args, **self._kwargs)
    |    |        |    |        |    -> {}
    |    |        |    |        -> <Thread(Thread-1 (run), started 5816)>
    |    |        |    -> ()
    |    |        -> <Thread(Thread-1 (run), started 5816)>
    |    -> <bound method PluginRunStatusListener.run of <pymemri.plugin.listeners.PluginRunStatusListener object at 0x0000023941238370>>
    -> <Thread(Thread-1 (run), started 5816)>

> File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\listeners.py", line 37, in run
    run = self.client.get(self.run_id)
          |    |      |   |    -> '2ae306ebadd44a7d9d56f746e9db6340'
          |    |      |   -> <pymemri.plugin.listeners.PluginRunStatusListener object at 0x0000023941238370>
          |    |      -> <function PodClient.get at 0x00000239404981F0>
          |    -> <pymemri.pod.client.PodClient object at 0x0000023941238D30>
          -> <pymemri.plugin.listeners.PluginRunStatusListener object at 0x0000023941238370>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\pod\client.py", line 328, in get
    res = self._get_item_expanded(id)
          |    |                  -> '2ae306ebadd44a7d9d56f746e9db6340'
          |    -> <function PodClient._get_item_expanded at 0x0000023940498310>
          -> <pymemri.pod.client.PodClient object at 0x0000023941238D30>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\pod\client.py", line 340, in _get_item_expanded
    item = self._get_item_with_properties(id)
           |    |                         -> '2ae306ebadd44a7d9d56f746e9db6340'
           |    -> <function PodClient._get_item_with_properties at 0x0000023940498430>
           -> <pymemri.pod.client.PodClient object at 0x0000023941238D30>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\pod\client.py", line 363, in _get_item_with_properties
    result = self.api.get_item(str(id))
             |    |   |            -> '2ae306ebadd44a7d9d56f746e9db6340'
             |    |   -> <function PodAPI.get_item at 0x0000023940495BD0>
             |    -> <pymemri.pod.api.PodAPI object at 0x0000023941238DC0>
             -> <pymemri.pod.client.PodClient object at 0x0000023941238D30>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\pod\api.py", line 99, in get_item
    return self.post("get_item", uid).json()
           |    |                -> '2ae306ebadd44a7d9d56f746e9db6340'
           |    -> <function PodAPI.post at 0x0000023940495B40>
           -> <pymemri.pod.api.PodAPI object at 0x0000023941238DC0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\pod\api.py", line 93, in post
    response = self.session.post(f"{self.base_url}/{endpoint}", json=body)
               |    |       |                                        -> {'auth': {'type': 'ClientAuth', 'databaseKey': '1097795856976757674153837887558145922935457163051325825324303404'}, 'payload'...
               |    |       -> <function Session.post at 0x0000023940494CA0>
               |    -> <requests.sessions.Session object at 0x0000023941238C70>
               -> <pymemri.pod.api.PodAPI object at 0x0000023941238DC0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\sessions.py", line 635, in post
    return self.request("POST", url, data=data, json=json, **kwargs)
           |    |               |         |          |       -> {}
           |    |               |         |          -> {'auth': {'type': 'ClientAuth', 'databaseKey': '1097795856976757674153837887558145922935457163051325825324303404'}, 'payload'...
           |    |               |         -> None
           |    |               -> 'https://dev.pod.memri.io/v4/7065337292277738475944439726962355197678278632801934531124567064/get_item'
           |    -> <function Session.request at 0x0000023940494A60>
           -> <requests.sessions.Session object at 0x0000023941238C70>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\sessions.py", line 587, in request
    resp = self.send(prep, **send_kwargs)
           |    |    |       -> {'timeout': None, 'allow_redirects': True, 'proxies': OrderedDict(), 'stream': False, 'verify': True, 'cert': None}
           |    |    -> <PreparedRequest [POST]>
           |    -> <function Session.send at 0x0000023940494EE0>
           -> <requests.sessions.Session object at 0x0000023941238C70>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\sessions.py", line 701, in send
    r = adapter.send(request, **kwargs)
        |       |    |          -> {'timeout': None, 'proxies': OrderedDict(), 'stream': False, 'verify': True, 'cert': None}
        |       |    -> <PreparedRequest [POST]>
        |       -> <function HTTPAdapter.send at 0x00000239404943A0>
        -> <requests.adapters.HTTPAdapter object at 0x0000023941238CA0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\adapters.py", line 547, in send
    raise ConnectionError(err, request=request)
          |                            -> <PreparedRequest [POST]>
          -> <class 'requests.exceptions.ConnectionError'>

requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))
2023-04-21 14:39:20.632 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 3/3 items/edges
2023-04-21 14:39:20.762 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 3 items/edges
2023-04-21 14:39:29.460 | INFO     | google_calendar.plugin:write:322 - Creating 54 items, 151 edges, updating 49 and uploading 1 files
2023-04-21 14:39:29.472 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 254/254 items/edges
2023-04-21 14:39:29.486 | INFO     | google_calendar.plugin:write:322 - Creating 55 items, 154 edges, updating 50 and uploading 1 files
2023-04-21 14:39:29.486 | INFO     | google_calendar.plugin:write:322 - Creating 56 items, 157 edges, updating 51 and uploading 1 files
2023-04-21 14:39:29.502 | INFO     | google_calendar.plugin:write:322 - Creating 57 items, 160 edges, updating 52 and uploading 1 files
2023-04-21 14:39:29.502 | INFO     | google_calendar.plugin:write:322 - Creating 58 items, 163 edges, updating 53 and uploading 1 files
2023-04-21 14:39:29.502 | INFO     | google_calendar.plugin:write:322 - Creating 59 items, 166 edges, updating 54 and uploading 1 files
2023-04-21 14:39:29.503 | INFO     | google_calendar.plugin:write:322 - Creating 60 items, 169 edges, updating 55 and uploading 1 files
2023-04-21 14:39:29.503 | INFO     | google_calendar.plugin:write:322 - Creating 61 items, 172 edges, updating 56 and uploading 1 files
2023-04-21 14:39:29.504 | INFO     | google_calendar.plugin:write:322 - Creating 62 items, 175 edges, updating 57 and uploading 1 files
2023-04-21 14:39:29.504 | INFO     | google_calendar.plugin:write:322 - Creating 63 items, 178 edges, updating 58 and uploading 1 files
2023-04-21 14:39:29.899 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 254 items/edges
2023-04-21 14:39:29.904 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.44426941871643066
2023-04-21 14:39:30.010 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:30.118 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:30.122 | INFO     | google_calendar.plugin:write:322 - Creating 51 items, 151 edges, updating 50 and uploading 0 files
2023-04-21 14:39:30.126 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 252/252 items/edges
2023-04-21 14:39:30.803 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 252 items/edges
2023-04-21 14:39:30.807 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.6847801208496094
2023-04-21 14:39:30.908 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:31.017 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:31.033 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 142/142 items/edges
2023-04-21 14:39:31.208 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 142 items/edges
2023-04-21 14:39:31.210 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.1823256015777588
2023-04-21 14:39:31.311 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:31.420 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:31.435 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 0 items/edges
2023-04-21 14:39:31.435 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.0
2023-04-21 14:39:31.546 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:31.655 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:31.656 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 0 items/edges
2023-04-21 14:39:31.657 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.000990152359008789
2023-04-21 14:39:31.764 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:31.873 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:31.889 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 0 items/edges
2023-04-21 14:39:31.890 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.0010190010070800781
2023-04-21 14:39:31.999 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:32.107 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:32.107 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 0 items/edges
2023-04-21 14:39:32.107 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.0
2023-04-21 14:39:32.217 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:32.327 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:32.327 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 0 items/edges
2023-04-21 14:39:32.327 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.0
2023-04-21 14:39:32.437 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:32.545 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:32.561 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 0 items/edges
2023-04-21 14:39:32.561 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.0
2023-04-21 14:39:32.670 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:32.779 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:32.873 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 0 items/edges
2023-04-21 14:39:32.873 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.0
2023-04-21 14:39:32.981 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:33.090 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod
2023-04-21 14:39:33.200 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 0 items/edges
2023-04-21 14:39:33.200 | DEBUG    | google_calendar.plugin:write:334 - bulk write (no files) took 0.0
2023-04-21 14:39:33.308 | DEBUG    | google_calendar.plugin:write:338 - Uploading files
2023-04-21 14:39:33.417 | INFO     | google_calendar.plugin:write:346 - Written queues to Pod

```