$ pytest tests/
============================= test session starts ==============================
platform linux -- Python 3.9.17, pytest-7.4.0, pluggy-1.2.0
rootdir: /builds/memri/plugins/flickr
plugins: anyio-3.7.0
collected 2 items
tests/test_plugin.py ..                                                  [100%]
=============================== warnings summary ===============================
tests/test_plugin.py::test_plugin_flow
tests/test_plugin.py::test_plugin_flow_with_error
  /usr/local/lib/python3.9/site-packages/pymemri/plugin/pluginbase.py:30: RuntimeWarning: Plugin needs a pluginRun as kwarg, running without will only work in development.
    warnings.warn(
-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
======================== 2 passed, 2 warnings in 0.97s =========================
