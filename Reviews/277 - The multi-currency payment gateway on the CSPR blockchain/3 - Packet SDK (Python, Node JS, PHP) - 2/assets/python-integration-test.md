```
root@3818caae206c:/usr/src/app# nosetests --verbosity=2 tests/integration
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

----------------------------------------------------------------------
Ran 11 tests in 1.679s

OK
```
