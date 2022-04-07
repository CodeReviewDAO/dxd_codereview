```

yusuf@Yusuf-PC:~/casper-cert-issuer$ bash run_tests.sh
Running ./tests/__init__.py...
run_tests.sh: line 7: python: command not found
Running ./tests/test_certificate_handler.py...
run_tests.sh: line 7: python: command not found
Running ./tests/test_connectors.py...
run_tests.sh: line 7: python: command not found
Running ./tests/test_merkle_tree_generator.py...
run_tests.sh: line 7: python: command not found
Running ./tests/test_signer.py...
run_tests.sh: line 7: python: command not found
Running ./tests/test_tx_utils.py...
run_tests.sh: line 7: python: command not found

yusuf@Yusuf-PC:~/casper-cert-issuer$ python ./tests/test_certificate_handler.py
........
----------------------------------------------------------------------
Ran 8 tests in 0.002s

OK
yusuf@Yusuf-PC:~/casper-cert-issuer$ python ./tests/test_connectors.py
/home/yusuf/casper-cert-issuer/./tests/test_connectors.py:63: DeprecationWarning: Please use assertEqual instead.
  self.assertEquals(len(spendables), 3)
.
----------------------------------------------------------------------
Ran 1 test in 0.000s

OK
yusuf@Yusuf-PC:~/casper-cert-issuer$ python ./tests/test_merkle_tree_generator.py
.....
----------------------------------------------------------------------
Ran 5 tests in 0.000s

OK
yusuf@Yusuf-PC:~/casper-cert-issuer$ python ./tests/test_signer.py
.
----------------------------------------------------------------------
Ran 1 test in 0.000s

OK
yusuf@Yusuf-PC:~/casper-cert-issuer$ python ./tests/test_tx_utils.py
./home/yusuf/casper-cert-issuer/./tests/test_tx_utils.py:33: DeprecationWarning: Please use assertEqual instead.
  self.assertEquals(estimated_byte_count, 20602)
...........
----------------------------------------------------------------------
Ran 12 tests in 0.001s

OK

```
