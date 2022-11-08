```$ run_plugin --metadata "metadata.json"
reading database_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
reading owner_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
pod_full_address=http://localhost:3030
owner_key=4034576452731506897046767267367262375639578963170278551433972530

400 Failure: Bulk trigger stage failed for following reasons:
F82Cc0A328e2B2734B28DB4a751a046e: Error 500 Internal Server Error, Command execution failed with status exit status: 125
writing run info to C:\Users\HouPha\.pymemri\plugins\instagram\current_run.json
Starting authentication...
polling for credentials from account of pluginRun F82Cc0A328e2B2734B28DB4a751a046e ... run.status=userActionNeeded
polling for credentials from account of pluginRun F82Cc0A328e2B2734B28DB4a751a046e ... run.status=ready
Logging in...
Login failed, invalid credentials.
ERROR: Login: Checkpoint required. Point your browser to https://www.instagram.com/challenge/action/AXESVf-V_We0HybIBT7o16qTu6LsslGZ35L7AThVsupOBwMkJyH6QeGBPwuZ-axswyKqsNE/Afyt52Wrzq96mXuzqyr0hgDKHEg8uLD5iwdGBb5Pyt5cmdVBZJwwMEmzH9EjDGJxdfCSsiPAaUz9Bw/ffc_FfXFQeXvzEauDxRqSjl2hWLlFjvx73nqSVeb0Z6VCMB8YIrV8byhcUbO30QMApqY/ - follow the instructions, then retry.
polling for credentials from account of pluginRun F82Cc0A328e2B2734B28DB4a751a046e ... run.status=ready
Logging in...
Login success!
JSON Query to api/v1/users/web_profile_info/?username=hoopav@gmail.com: 404 Not Found [retrying; skip with ^C]
JSON Query to api/v1/users/web_profile_info/?username=hoopav@gmail.com: 404 Not Found [retrying; skip with ^C]
Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\instaloadercontext.py", line 347, in get_json
    raise QueryReturnedNotFoundException("404 Not Found")
instaloader.exceptions.QueryReturnedNotFoundException: 404 Not Found

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\instaloadercontext.py", line 347, in get_json
    raise QueryReturnedNotFoundException("404 Not Found")
instaloader.exceptions.QueryReturnedNotFoundException: 404 Not Found

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\instaloadercontext.py", line 347, in get_json
    raise QueryReturnedNotFoundException("404 Not Found")
instaloader.exceptions.QueryReturnedNotFoundException: 404 Not Found

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\structures.py", line 774, in _obtain_metadata
    metadata = self._context.get_iphone_json(f'api/v1/users/web_profile_info/?username={self.username}',
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\instaloadercontext.py", line 488, in get_iphone_json
    return self.get_json(path, params, 'i.instagram.com', tempsession)
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\instaloadercontext.py", line 394, in get_json
    return self.get_json(path=path, params=params, host=host, session=sess, _attempt=_attempt + 1)
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\instaloadercontext.py", line 394, in get_json
    return self.get_json(path=path, params=params, host=host, session=sess, _attempt=_attempt + 1)
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\instaloadercontext.py", line 382, in get_json
    raise QueryReturnedNotFoundException(error_string) from err
instaloader.exceptions.QueryReturnedNotFoundException: JSON Query to api/v1/users/web_profile_info/?username=hoopav@gmail.com: 404 Not Found

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 343, in run_plugin
    run_plugin_from_run_id(
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 208, in run_plugin_from_run_id
    plugin._run()
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 97, in _run
    self.run()
  File "z:\crdao\memri_finalwork\instagram-dev\instagram\plugin.py", line 78, in run
    my_profile = Profile.from_username(self.instaloader.context, self.username)
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\structures.py", line 705, in from_username
    profile._obtain_metadata()  # to raise ProfileNotExistsException now in case username is invalid
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\instaloader\structures.py", line 791, in _obtain_metadata
    raise ProfileNotExistsException('Profile {} does not exist.'.format(self.username)) from err
instaloader.exceptions.ProfileNotExistsException: Profile hoopav@gmail.com does not exist.

Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\Scripts\run_plugin-script.py", line 33, in <module>
    sys.exit(load_entry_point('pymemri==0.0.24', 'console_scripts', 'run_plugin')())
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\fastcore\script.py", line 105, in _f
    tfunc(**merge(args, args_from_prog(func, xtra)))
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 351, in run_plugin
    raise PluginError("The plugin quit unexpectedly.") from None
pymemri.plugin.pluginbase.PluginError: The plugin quit unexpectedly.
```
