```$ run_plugin --metadata "metadata.json"
reading database_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
reading owner_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
pod_full_address=http://localhost:3030
owner_key=4034576452731506897046767267367262375639578963170278551433972530

400 Failure: Bulk trigger stage failed for following reasons:
b56B731EB9AedCed5ECcee65C0cA81bD: Error 500 Internal Server Error, Command execution failed with status exit status: 125
writing run info to C:\Users\HouPha\.pymemri\plugins\gmail_importer\current_run.json
Starting authentication...
polling for credentials from account of pluginRun b56B731EB9AedCed5ECcee65C0cA81bD ... run.status=userActionNeeded
polling for credentials from account of pluginRun b56B731EB9AedCed5ECcee65C0cA81bD ... run.status=userActionNeeded
polling for credentials from account of pluginRun b56B731EB9AedCed5ECcee65C0cA81bD ... run.status=ready
Login failed, invalid credentials.
ERROR: b'[ALERT] Application-specific password required: https://support.google.com/accounts/answer/185833 (Failure)'
polling for credentials from account of pluginRun b56B731EB9AedCed5ECcee65C0cA81bD ... run.status=ready
Login failed, invalid credentials.
ERROR: b'[ALERT] Application-specific password required: https://support.google.com/accounts/answer/185833 (Failure)'
polling for credentials from account of pluginRun b56B731EB9AedCed5ECcee65C0cA81bD ... run.status=ready
Login failed, invalid credentials.
ERROR: b'[ALERT] Application-specific password required: https://support.google.com/accounts/answer/185833 (Failure)'
Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 343, in run_plugin
    run_plugin_from_run_id(
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 208, in run_plugin_from_run_id
    plugin._run()
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 97, in _run
    self.run()
  File "z:\crdao\memri_finalwork\gmail-dev\gmail_importer\plugin.py", line 222, in run
    self.authenticator.authenticate(self.login)
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\authenticators\password.py", line 71, in authenticate
    raise RuntimeError("Reached max login attempts.")
RuntimeError: Reached max login attempts.

Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\Scripts\run_plugin-script.py", line 33, in <module>
    sys.exit(load_entry_point('pymemri==0.0.24', 'console_scripts', 'run_plugin')())
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\fastcore\script.py", line 105, in _f
    tfunc(**merge(args, args_from_prog(func, xtra)))
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 351, in run_plugin
    raise PluginError("The plugin quit unexpectedly.") from None
pymemri.plugin.pluginbase.PluginError: The plugin quit unexpectedly.```
