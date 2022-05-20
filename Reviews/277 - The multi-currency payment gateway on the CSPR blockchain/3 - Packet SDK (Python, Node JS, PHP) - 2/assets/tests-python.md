```

nosetests --verbosity=2 tests
test_negative_create_payment_bad_amount_handle_400 (integration.test_integration_payment_client.TestIntegrationPaymentClient) ... ok
test_negative_create_payment_no_token_handle_401 (integration.test_integration_payment_client.TestIntegrationPaymentClient) ... ok
test_negative_create_payment_wrong_url_handle_404 (integration.test_integration_payment_client.TestIntegrationPaymentClient) ... ok
test_negative_get_payment_wrong_url_handle_404 (integration.test_integration_payment_client.TestIntegrationPaymentClient) ... ok
test_negative_get_payments_no_token_handle_400 (integration.test_integration_payment_client.TestIntegrationPaymentClient) ... ok
test_negative_get_payments_wrong_url_handle_404 (integration.test_integration_payment_client.TestIntegrationPaymentClient) ... ok
test_positive_create_and_get_payment (integration.test_integration_payment_client.TestIntegrationPaymentClient) ... ok
test_positive_get_payments_no_params (integration.test_integration_payment_client.TestIntegrationPaymentClient) ... ok
test_negative_get_transactions_bad_url_handle_404 (integration.test_integration_transaction_client.TestIntegrationTransactionClient) ... ok
test_negative_get_transactions_no_token_handle_401 (integration.test_integration_transaction_client.TestIntegrationTransactionClient) ... ok
test_positive_get_transactions (integration.test_integration_transaction_client.TestIntegrationTransactionClient) ... ok
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
Ran 29 tests in 3.189s

OK

```
