yusuf@Yusuf-MacBook-Pro dockertests % make sh
docker run -it --entrypoint "/bin/bash" dhfpythontest:latest
root@3818caae206c:/usr/src/app# nosetests --verbosity=2 tests/unit
test_negative_create_payment_400_handling (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_create_payment_401_handling (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_create_payment_404_handling (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_create_payment_without_params (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_getting_payment_400_handling (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_getting_payment_401_handling (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_getting_payment_404_handling (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_getting_payments_400_handling (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_getting_payments_401_handling (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_getting_payments_404_handling (unit.test_payment_client.TestPaymentClient) ... ok
test_positive_create_payment (unit.test_payment_client.TestPaymentClient) ... ok
test_positive_getting_payment (unit.test_payment_client.TestPaymentClient) ... ok
test_positive_getting_payments (unit.test_payment_client.TestPaymentClient) ... ok
test_negative_getting_transactions_400_handling (unit.test_transaction_client.TestTransactionClient) ... ok
test_negative_getting_transactions_401_handling (unit.test_transaction_client.TestTransactionClient) ... ok
test_negative_getting_transactions_404_handling (unit.test_transaction_client.TestTransactionClient) ... ok
test_negative_getting_transactions_connection_error (unit.test_transaction_client.TestTransactionClient) ... ok
test_positive_getting_transactions (unit.test_transaction_client.TestTransactionClient) ... ok

----------------------------------------------------------------------
Ran 18 tests in 0.156s

OK