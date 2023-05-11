```
$ run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json"
2023-04-21 12:42:11.226 | INFO     | pymemri.plugin.cli:<module>:34 - Pymemri version: 0.0.45
2023-04-21 12:42:11.311 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading database_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 12:42:11.312 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading owner_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 12:42:12.776 | WARNING  | pymemri.pod.client:create_account:81 - 400 "Failure: Error 400 Bad Request, Account for 2084530952725798685762308706130930073367878817745927324762146990 already exist"
2023-04-21 12:42:13.625 | INFO     | pymemri.plugin.pluginbase:write_run_info:190 - writing run info to C:\Users\HouPha\.pymemri\plugins\summarization_plugin\current_run.json
2023-04-21 12:42:16.185 | INFO     | summarization_plugin.plugin:__init__:17 - Loading model...
2023-04-21 12:42:16.186 | DEBUG    | summarization_plugin.model:__init__:30 - Using device: cpu
pod_full_address=https://dev.pod.memri.io
owner_key=2084530952725798685762308706130930073367878817745927324762146990

Downloading: 100%|##########| 300/300 [00:00<00:00, 97.7kB/s]
C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\huggingface_hub\file_download.py:127: UserWarning: `huggingface_hub` cache-system uses symlinks by default to efficiently store duplicated files but your machine does not support them in C:\Users\HouPha\.cache\huggingface\hub. Caching files will still work but in a degraded version that might require more space on your disk. This warning can be disabled by setting the `HF_HUB_DISABLE_SYMLINKS_WARNING` environment variable. For more details, see https://huggingface.co/docs/huggingface_hub/how-to-cache#limitations.
To support symlinks on Windows, you either need to activate Developer Mode or to run Python as an administrator. In order to see activate developer mode, see this article: https://docs.microsoft.com/en-us/windows/apps/get-started/enable-your-device-for-development
  warnings.warn(message)
Downloading: 100%|##########| 1.63k/1.63k [00:00<00:00, 543kB/s]
Downloading: 100%|##########| 798k/798k [00:00<00:00, 7.41MB/s]
Downloading: 100%|##########| 456k/456k [00:00<00:00, 5.37MB/s]
Downloading: 100%|##########| 239/239 [00:00<00:00, 79.6kB/s]
Downloading: 100%|##########| 1.63G/1.63G [00:18<00:00, 88.9MB/s]
INFO:     Started server process [19900]
INFO:     Waiting for application startup.
INFO:     Application startup complete.
INFO:     Uvicorn running on http://127.0.0.1:8080 (Press CTRL+C to quit)
2023-04-21 12:42:40.094 | INFO     | summarization_plugin.plugin:run:23 - Plugin is ready.
2023-04-21 12:42:44.994 | ERROR    | pymemri.plugin.listeners:run:98 - Could not get run in httpstatus listener
Traceback (most recent call last):

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 703, in urlopen
    httplib_response = self._make_request(
                       |    -> <function HTTPConnectionPool._make_request at 0x00000165AB9AEF80>
                       -> <urllib3.connectionpool.HTTPSConnectionPool object at 0x00000165ACAF9060>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 449, in _make_request
    six.raise_from(e, None)
    |   -> <function raise_from at 0x00000165AB86FEB0>
    -> <module 'urllib3.packages.six' from 'C:\\Users\\HouPha\\AppData\\Local\\Programs\\Python\\Python310\\lib\\site-packages\\urll...

  File "<string>", line 3, in raise_from

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 444, in _make_request
    httplib_response = conn.getresponse()
                       |    -> <function HTTPConnection.getresponse at 0x00000165AB949510>
                       -> <urllib3.connection.HTTPSConnection object at 0x00000165ACAF9600>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 1374, in getresponse
    response.begin()
    |        -> <function HTTPResponse.begin at 0x00000165AB92F880>
    -> <http.client.HTTPResponse object at 0x00000165E54392D0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 318, in begin
    version, status, reason = self._read_status()
                              |    -> <function HTTPResponse._read_status at 0x00000165AB92F7F0>
                              -> <http.client.HTTPResponse object at 0x00000165E54392D0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 287, in _read_status
    raise RemoteDisconnected("Remote end closed connection without"
          -> <class 'http.client.RemoteDisconnected'>

http.client.RemoteDisconnected: Remote end closed connection without response


During handling of the above exception, another exception occurred:


Traceback (most recent call last):

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\adapters.py", line 489, in send
    resp = conn.urlopen(
           |    -> <function HTTPConnectionPool.urlopen at 0x00000165AB9AF1C0>
           -> <urllib3.connectionpool.HTTPSConnectionPool object at 0x00000165ACAF9060>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 787, in urlopen
    retries = retries.increment(
              |       -> <function Retry.increment at 0x00000165AB965480>
              -> Retry(total=0, connect=None, read=False, redirect=None, status=None)

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\util\retry.py", line 550, in increment
    raise six.reraise(type(error), error, _stacktrace)
          |   |            |       |      -> <traceback object at 0x00000165E529AEC0>
          |   |            |       -> ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))
          |   |            -> ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))
          |   -> <function reraise at 0x00000165AB86FE20>
          -> <module 'urllib3.packages.six' from 'C:\\Users\\HouPha\\AppData\\Local\\Programs\\Python\\Python310\\lib\\site-packages\\urll...

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\packages\six.py", line 769, in reraise
    raise value.with_traceback(tb)
          |                    -> None
          -> None

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 703, in urlopen
    httplib_response = self._make_request(
                       |    -> <function HTTPConnectionPool._make_request at 0x00000165AB9AEF80>
                       -> <urllib3.connectionpool.HTTPSConnectionPool object at 0x00000165ACAF9060>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 449, in _make_request
    six.raise_from(e, None)
    |   -> <function raise_from at 0x00000165AB86FEB0>
    -> <module 'urllib3.packages.six' from 'C:\\Users\\HouPha\\AppData\\Local\\Programs\\Python\\Python310\\lib\\site-packages\\urll...

  File "<string>", line 3, in raise_from

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\urllib3\connectionpool.py", line 444, in _make_request
    httplib_response = conn.getresponse()
                       |    -> <function HTTPConnection.getresponse at 0x00000165AB949510>
                       -> <urllib3.connection.HTTPSConnection object at 0x00000165ACAF9600>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 1374, in getresponse
    response.begin()
    |        -> <function HTTPResponse.begin at 0x00000165AB92F880>
    -> <http.client.HTTPResponse object at 0x00000165E54392D0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 318, in begin
    version, status, reason = self._read_status()
                              |    -> <function HTTPResponse._read_status at 0x00000165AB92F7F0>
                              -> <http.client.HTTPResponse object at 0x00000165E54392D0>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\http\client.py", line 287, in _read_status
    raise RemoteDisconnected("Remote end closed connection without"
          -> <class 'http.client.RemoteDisconnected'>

urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))


During handling of the above exception, another exception occurred:


Traceback (most recent call last):

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\threading.py", line 973, in _bootstrap
    self._bootstrap_inner()
    |    -> <function Thread._bootstrap_inner at 0x00000165FA41DF30>
    -> <Thread(Thread-3 (run), started 10280)>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\threading.py", line 1016, in _bootstrap_inner
    self.run()
    |    -> <function Thread.run at 0x00000165FA41DC60>
    -> <Thread(Thread-3 (run), started 10280)>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\threading.py", line 953, in run
    self._target(*self._args, **self._kwargs)
    |    |        |    |        |    -> {}
    |    |        |    |        -> <Thread(Thread-3 (run), started 10280)>
    |    |        |    -> ()
    |    |        -> <Thread(Thread-3 (run), started 10280)>
    |    -> <bound method PodHTTPStatusListener.run of <pymemri.plugin.listeners.PodHTTPStatusListener object at 0x00000165E5438A90>>
    -> <Thread(Thread-3 (run), started 10280)>

> File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\listeners.py", line 89, in run
    _ = self.client.api.get_item(self.run_id)
        |    |      |   |        |    -> 'cc789a68c98d42708f35babfef6649d3'
        |    |      |   |        -> <pymemri.plugin.listeners.PodHTTPStatusListener object at 0x00000165E5438A90>
        |    |      |   -> <function PodAPI.get_item at 0x00000165ABDD5B40>
        |    |      -> <pymemri.pod.api.PodAPI object at 0x00000165ACAF8D60>
        |    -> <pymemri.pod.client.PodClient object at 0x00000165ACAF8CD0>
        -> <pymemri.plugin.listeners.PodHTTPStatusListener object at 0x00000165E5438A90>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\pod\api.py", line 99, in get_item
    return self.post("get_item", uid).json()
           |    |                -> 'cc789a68c98d42708f35babfef6649d3'
           |    -> <function PodAPI.post at 0x00000165ABDD5AB0>
           -> <pymemri.pod.api.PodAPI object at 0x00000165ACAF8D60>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\pod\api.py", line 93, in post
    response = self.session.post(f"{self.base_url}/{endpoint}", json=body)
               |    |       |                                        -> {'auth': {'type': 'ClientAuth', 'databaseKey': '8541075164214624166078942343264608982665504336039228580257327657'}, 'payload'...
               |    |       -> <function Session.post at 0x00000165ABDD4C10>
               |    -> <requests.sessions.Session object at 0x00000165ACAF8C10>
               -> <pymemri.pod.api.PodAPI object at 0x00000165ACAF8D60>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\sessions.py", line 635, in post
    return self.request("POST", url, data=data, json=json, **kwargs)
           |    |               |         |          |       -> {}
           |    |               |         |          -> {'auth': {'type': 'ClientAuth', 'databaseKey': '8541075164214624166078942343264608982665504336039228580257327657'}, 'payload'...
           |    |               |         -> None
           |    |               -> 'https://dev.pod.memri.io/v4/2084530952725798685762308706130930073367878817745927324762146990/get_item'
           |    -> <function Session.request at 0x00000165ABDD49D0>
           -> <requests.sessions.Session object at 0x00000165ACAF8C10>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\sessions.py", line 587, in request
    resp = self.send(prep, **send_kwargs)
           |    |    |       -> {'timeout': None, 'allow_redirects': True, 'proxies': OrderedDict(), 'stream': False, 'verify': True, 'cert': None}
           |    |    -> <PreparedRequest [POST]>
           |    -> <function Session.send at 0x00000165ABDD4E50>
           -> <requests.sessions.Session object at 0x00000165ACAF8C10>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\sessions.py", line 701, in send
    r = adapter.send(request, **kwargs)
        |       |    |          -> {'timeout': None, 'proxies': OrderedDict(), 'stream': False, 'verify': True, 'cert': None}
        |       |    -> <PreparedRequest [POST]>
        |       -> <function HTTPAdapter.send at 0x00000165ABDD4310>
        -> <requests.adapters.HTTPAdapter object at 0x00000165ACAF8C40>

  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\requests\adapters.py", line 547, in send
    raise ConnectionError(err, request=request)
          |                            -> <PreparedRequest [POST]>
          -> <class 'requests.exceptions.ConnectionError'>

requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))


```