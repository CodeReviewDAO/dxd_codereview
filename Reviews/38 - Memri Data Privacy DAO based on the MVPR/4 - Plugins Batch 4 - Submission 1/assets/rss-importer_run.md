```
$ run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json"
2023-04-21 12:07:31.959 | INFO     | pymemri.plugin.cli:<module>:34 - Pymemri version: 0.0.45
2023-04-21 12:07:32.043 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading database_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 12:07:32.043 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading owner_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 12:07:33.226 | INFO     | pymemri.plugin.pluginbase:write_run_info:190 - writing run info to C:\Users\HouPha\.pymemri\plugins\rss_importer\current_run.json
2023-04-21 12:07:33.705 | INFO     | rss_importer.plugin:setup_default_feeds:73 - Setting up default feeds...
INFO:     Started server process [19984]
INFO:     Waiting for application startup.
INFO:     Application startup complete.
INFO:     Uvicorn running on http://127.0.0.1:8080 (Press CTRL+C to quit)
2023-04-21 12:07:34.213 | DEBUG    | rss_importer.plugin:setup_feed:89 - Importing feed with 58 entries
2023-04-21 12:07:34.218 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 3/3 items/edges
2023-04-21 12:07:34.344 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 3 items/edges
2023-04-21 12:07:34.475 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 118/118 items/edges
2023-04-21 12:07:34.723 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 118 items/edges
2023-04-21 12:07:35.137 | DEBUG    | rss_importer.plugin:setup_feed:89 - Importing feed with 20 entries
2023-04-21 12:07:35.139 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 3/3 items/edges
2023-04-21 12:07:35.258 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 3 items/edges
2023-04-21 12:07:35.383 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 42/42 items/edges
2023-04-21 12:07:35.518 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 42 items/edges
2023-04-21 12:07:36.008 | DEBUG    | rss_importer.plugin:setup_feed:89 - Importing feed with 25 entries
2023-04-21 12:07:36.010 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 51/51 items/edges
2023-04-21 12:07:36.145 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 51 items/edges
2023-04-21 12:07:36.594 | DEBUG    | rss_importer.plugin:setup_feed:89 - Importing feed with 30 entries
2023-04-21 12:07:36.595 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 61/61 items/edges
2023-04-21 12:07:36.727 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 61 items/edges
2023-04-21 12:07:37.766 | DEBUG    | rss_importer.schema:from_feedparser_dict:89 - Could not import Feed image: cannot identify image file <_io.BytesIO object at 0x000001B294838F90>
2023-04-21 12:07:37.767 | DEBUG    | rss_importer.plugin:setup_feed:89 - Importing feed with 48 entries
2023-04-21 12:07:37.770 | INFO     | pymemri.pod.client:bulk_action:289 - BULK: Writing 97/97 items/edges
2023-04-21 12:07:37.917 | INFO     | pymemri.pod.client:bulk_action:301 - Completed Bulk action, written 97 items/edges
2023-04-21 12:07:37.917 | INFO     | rss_importer.plugin:run:45 - Daemon mode started, updating every 900 seconds.
pod_full_address=https://dev.pod.memri.io
owner_key=2084530952725798685762308706130930073367878817745927324762146990

INFO:     127.0.0.1:55717 - "GET / HTTP/1.1" 404 Not Found
2023-04-21 12:07:49.011 | ERROR    | pymemri.plugin.listeners:run:98 - Could not get run in httpstatus listener
Traceback (most recent call last):

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 703, in urlopen
    httplib_response = self._make_request(
                       |    -> <function HTTPConnectionPool._make_request at 0x000001B29206A950>
                       -> <urllib3.connectionpool.HTTPSConnectionPool object at 0x000001B293210BB0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 449, in _make_request
    six.raise_from(e, None)
    |   -> <function raise_from at 0x000001B2FFEE3880>
    -> <module 'urllib3.packages.six' from 'C:\\Users\\HouPha\\AppData\\Local\\Programs\\Python\\Python310\\lib\\site-packages\\urll...

  File "<string>", line 3, in raise_from

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 444, in _make_request
    httplib_response = conn.getresponse()
                       |    -> <function HTTPConnection.getresponse at 0x000001B292004EE0>
                       -> <urllib3.connection.HTTPSConnection object at 0x000001B2949D1870>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 1374, in getresponse
    response.begin()
    |        -> <function HTTPResponse.begin at 0x000001B2FFFBF250>
    -> <http.client.HTTPResponse object at 0x000001B2948E3670>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 318, in begin
    version, status, reason = self._read_status()
                              |    -> <function HTTPResponse._read_status at 0x000001B2FFFBF1C0>
                              -> <http.client.HTTPResponse object at 0x000001B2948E3670>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 287, in _read_status
    raise RemoteDisconnected("Remote end closed connection without"
          -> <class 'http.client.RemoteDisconnected'>

http.client.RemoteDisconnected: Remote end closed connection without response


During handling of the above exception, another exception occurred:


Traceback (most recent call last):

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\adapters.py", line 489, in send
    resp = conn.urlopen(
           |    -> <function HTTPConnectionPool.urlopen at 0x000001B29206AB90>
           -> <urllib3.connectionpool.HTTPSConnectionPool object at 0x000001B293210BB0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 787, in urlopen
    retries = retries.increment(
              |       -> <function Retry.increment at 0x000001B292028E50>
              -> Retry(total=0, connect=None, read=False, redirect=None, status=None)

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\util\retry.py", line 550, in increment
    raise six.reraise(type(error), error, _stacktrace)
          |   |            |       |      -> <traceback object at 0x000001B2948459C0>
          |   |            |       -> ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))
          |   |            -> ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))
          |   -> <function reraise at 0x000001B2FFEE37F0>
          -> <module 'urllib3.packages.six' from 'C:\\Users\\HouPha\\AppData\\Local\\Programs\\Python\\Python310\\lib\\site-packages\\urll...

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\packages\six.py", line 769, in reraise
    raise value.with_traceback(tb)
          |                    -> None
          -> None

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 703, in urlopen
    httplib_response = self._make_request(
                       |    -> <function HTTPConnectionPool._make_request at 0x000001B29206A950>
                       -> <urllib3.connectionpool.HTTPSConnectionPool object at 0x000001B293210BB0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 449, in _make_request
    six.raise_from(e, None)
    |   -> <function raise_from at 0x000001B2FFEE3880>
    -> <module 'urllib3.packages.six' from 'C:\\Users\\HouPha\\AppData\\Local\\Programs\\Python\\Python310\\lib\\site-packages\\urll...

  File "<string>", line 3, in raise_from

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 444, in _make_request
    httplib_response = conn.getresponse()
                       |    -> <function HTTPConnection.getresponse at 0x000001B292004EE0>
                       -> <urllib3.connection.HTTPSConnection object at 0x000001B2949D1870>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 1374, in getresponse
    response.begin()
    |        -> <function HTTPResponse.begin at 0x000001B2FFFBF250>
    -> <http.client.HTTPResponse object at 0x000001B2948E3670>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 318, in begin
    version, status, reason = self._read_status()
                              |    -> <function HTTPResponse._read_status at 0x000001B2FFFBF1C0>
                              -> <http.client.HTTPResponse object at 0x000001B2948E3670>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 287, in _read_status
    raise RemoteDisconnected("Remote end closed connection without"
          -> <class 'http.client.RemoteDisconnected'>

urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))


During handling of the above exception, another exception occurred:


Traceback (most recent call last):

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\threading.py", line 973, in _bootstrap
    self._bootstrap_inner()
    |    -> <function Thread._bootstrap_inner at 0x000001B2E0A78CA0>
    -> <Thread(Thread-2 (run), started 23904)>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\threading.py", line 1016, in _bootstrap_inner
    self.run()
    |    -> <function Thread.run at 0x000001B2E0A78F70>
    -> <Thread(Thread-2 (run), started 23904)>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\threading.py", line 953, in run
    self._target(*self._args, **self._kwargs)
    |    |        |    |        |    -> {}
    |    |        |    |        -> <Thread(Thread-2 (run), started 23904)>
    |    |        |    -> ()
    |    |        -> <Thread(Thread-2 (run), started 23904)>
    |    -> <bound method PodHTTPStatusListener.run of <pymemri.plugin.listeners.PodHTTPStatusListener object at 0x000001B294595B40>>
    -> <Thread(Thread-2 (run), started 23904)>

> File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\listeners.py", line 89, in run
    _ = self.client.api.get_item(self.run_id)
        |    |      |   |        |    -> '0ccff81048bc4889a1193b9df18ce1fa'
        |    |      |   |        -> <pymemri.plugin.listeners.PodHTTPStatusListener object at 0x000001B294595B40>
        |    |      |   -> <function PodAPI.get_item at 0x000001B292465510>
        |    |      -> <pymemri.pod.api.PodAPI object at 0x000001B2932108B0>
        |    -> <pymemri.pod.client.PodClient object at 0x000001B293210820>
        -> <pymemri.plugin.listeners.PodHTTPStatusListener object at 0x000001B294595B40>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\pod\api.py", line 99, in get_item
    return self.post("get_item", uid).json()
           |    |                -> '0ccff81048bc4889a1193b9df18ce1fa'
           |    -> <function PodAPI.post at 0x000001B292465480>
           -> <pymemri.pod.api.PodAPI object at 0x000001B2932108B0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\pod\api.py", line 93, in post
    response = self.session.post(f"{self.base_url}/{endpoint}", json=body)
               |    |       |                                        -> {'auth': {'type': 'ClientAuth', 'databaseKey': '8541075164214624166078942343264608982665504336039228580257327657'}, 'payload'...
               |    |       -> <function Session.post at 0x000001B2924645E0>
               |    -> <requests.sessions.Session object at 0x000001B293210760>
               -> <pymemri.pod.api.PodAPI object at 0x000001B2932108B0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\sessions.py", line 635, in post
    return self.request("POST", url, data=data, json=json, **kwargs)
           |    |               |         |          |       -> {}
           |    |               |         |          -> {'auth': {'type': 'ClientAuth', 'databaseKey': '8541075164214624166078942343264608982665504336039228580257327657'}, 'payload'...
           |    |               |         -> None
           |    |               -> 'https://dev.pod.memri.io/v4/2084530952725798685762308706130930073367878817745927324762146990/get_item'
           |    -> <function Session.request at 0x000001B2924643A0>
           -> <requests.sessions.Session object at 0x000001B293210760>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\sessions.py", line 587, in request
    resp = self.send(prep, **send_kwargs)
           |    |    |       -> {'timeout': None, 'allow_redirects': True, 'proxies': OrderedDict(), 'stream': False, 'verify': True, 'cert': None}
           |    |    -> <PreparedRequest [POST]>
           |    -> <function Session.send at 0x000001B292464820>
           -> <requests.sessions.Session object at 0x000001B293210760>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\sessions.py", line 701, in send
    r = adapter.send(request, **kwargs)
        |       |    |          -> {'timeout': None, 'proxies': OrderedDict(), 'stream': False, 'verify': True, 'cert': None}
        |       |    -> <PreparedRequest [POST]>
        |       -> <function HTTPAdapter.send at 0x000001B292447C70>
        -> <requests.adapters.HTTPAdapter object at 0x000001B293210790>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\adapters.py", line 547, in send
    raise ConnectionError(err, request=request)
          |                            -> <PreparedRequest [POST]>
          -> <class 'requests.exceptions.ConnectionError'>

requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))


```