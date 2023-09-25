============================= test session starts ==============================
platform linux -- Python 3.9.17, pytest-7.4.0, pluggy-1.2.0
rootdir: /builds/memri/plugins/dropbox-v2
plugins: anyio-3.7.1
collected 3 items
tests/test_create_folders.py .                                           [ 33%]
tests/test_extract_location.py ..                                        [100%]
=============================== warnings summary ===============================
tests/test_create_folders.py::test_plugin_flow
tests/test_extract_location.py::test_extract_location
tests/test_extract_location.py::test_extract_location_corrupted_image
  /usr/local/lib/python3.9/site-packages/pymemri/plugin/pluginbase.py:30: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    warnings.warn(
tests/test_create_folders.py::test_plugin_flow
tests/test_create_folders.py::test_plugin_flow
  /builds/memri/plugins/dropbox-v2/dropbox_oauth/pod_update_queue.py:93: DeprecationWarning: `copy_on_model_validation` should be a string: 'deep', 'shallow' or 'none'
    pod_update = PodUpdate(
tests/test_create_folders.py::test_plugin_flow
tests/test_create_folders.py::test_plugin_flow
tests/test_create_folders.py::test_plugin_flow
  /builds/memri/plugins/dropbox-v2/dropbox_oauth/pod_update_queue.py:29: DeprecationWarning: `copy_on_model_validation` should be a string: 'deep', 'shallow' or 'none'
    return PodUpdate(
-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
======================== 3 passed, 8 warnings in 3.02s =========================
