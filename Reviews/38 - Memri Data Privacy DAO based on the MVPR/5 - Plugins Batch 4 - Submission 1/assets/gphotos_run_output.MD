```
$ run_plugin --pod_full_address="https://dev.pod.memri.io" --metadata "metadata.json"
2023-04-21 14:56:05.436 | INFO     | pymemri.plugin.cli:<module>:34 - Pymemri version: 0.0.45
2023-04-21 14:56:05.517 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading database_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 14:56:05.517 | INFO     | pymemri.pod.utils:read_pod_key:23 - reading owner_key from C:\Users\HouPha\.pymemri\pod_keys\keys.json
2023-04-21 14:56:06.697 | INFO     | pymemri.plugin.pluginbase:write_run_info:190 - writing run info to C:\Users\HouPha\.pymemri\plugins\google_photos\current_run.json
pod_full_address=https://dev.pod.memri.io
owner_key=5912819934901175497338441595637798049856112472817727981094971568

Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 198, in get_plugin_cls
    module = importlib.import_module(plugin_module)
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\importlib\__init__.py", line 126, in import_module
    return _bootstrap._gcd_import(name[level:], package, level)
  File "<frozen importlib._bootstrap>", line 1050, in _gcd_import
  File "<frozen importlib._bootstrap>", line 1027, in _find_and_load
  File "<frozen importlib._bootstrap>", line 992, in _find_and_load_unlocked
  File "<frozen importlib._bootstrap>", line 241, in _call_with_frames_removed
  File "<frozen importlib._bootstrap>", line 1050, in _gcd_import
  File "<frozen importlib._bootstrap>", line 1027, in _find_and_load
  File "<frozen importlib._bootstrap>", line 1004, in _find_and_load_unlocked
ModuleNotFoundError: No module named 'google_photos'

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\cli.py", line 124, in run_plugin
    run_plugin_from_run_id(plugin_run_id, client, **plugin_config)
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 220, in run_plugin_from_run_id
    plugin_cls = get_plugin_cls(run.pluginModule, run.pluginName)
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\pluginbase.py", line 202, in get_plugin_cls
    raise ImportError(f"Unknown plugin: {plugin_module}.{plugin_name}")
ImportError: Unknown plugin: google_photos.plugin.GooglePhotos

Traceback (most recent call last):
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\runpy.py", line 196, in _run_module_as_main
    return _run_code(code, main_globals, None,
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\runpy.py", line 86, in _run_code
    exec(code, run_globals)
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\Scripts\run_plugin.exe\__main__.py", line 7, in <module>
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\fastcore\script.py", line 105, in _f
    tfunc(**merge(args, args_from_prog(func, xtra)))
  File "C:\Users\HouPha\AppData\Local\Programs\Python\Python310\lib\site-packages\pymemri\plugin\cli.py", line 130, in run_plugin
    raise PluginError("The plugin quit unexpectedly.") from None
pymemri.plugin.pluginbase.PluginError: The plugin quit unexpectedly.

```