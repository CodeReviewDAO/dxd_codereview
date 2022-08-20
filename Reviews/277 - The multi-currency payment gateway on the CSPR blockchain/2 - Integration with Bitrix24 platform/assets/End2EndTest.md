'''
muharremsalel@Muharrems-MacBook-Pro end2end % npm run codeceptjs --verbose
npm verb cli /usr/local/Cellar/node/17.0.1/bin/node /usr/local/bin/npm
npm info using npm@8.12.2
npm info using node@v17.0.1
npm timing npm:load:whichnode Completed in 0ms
npm timing config:load:defaults Completed in 1ms
npm timing config:load:file:/usr/local/lib/node_modules/npm/npmrc Completed in 2ms
npm timing config:load:builtin Completed in 2ms
npm timing config:load:cli Completed in 2ms
npm timing config:load:env Completed in 0ms
npm timing config:load:file:/Users/muharremsalel/Desktop/CRDao/dhf-pay-bitrix/tests/end2end/.npmrc Completed in 1ms
npm timing config:load:project Completed in 4ms
npm timing config:load:file:/Users/muharremsalel/.npmrc Completed in 0ms
npm timing config:load:user Completed in 0ms
npm timing config:load:file:/usr/local/etc/npmrc Completed in 0ms
npm timing config:load:global Completed in 0ms
npm timing config:load:validate Completed in 0ms
npm timing config:load:credentials Completed in 1ms
npm timing config:load:setEnvs Completed in 0ms
npm timing config:load Completed in 11ms
npm timing npm:load:configload Completed in 11ms
npm timing npm:load:mkdirpcache Completed in 0ms
npm timing npm:load:mkdirplogs Completed in 0ms
npm verb title npm run codeceptjs
npm verb argv "run" "codeceptjs" "--loglevel" "verbose"
npm timing npm:load:setTitle Completed in 2ms
npm timing config:load:flatten Completed in 2ms
npm timing npm:load:display Completed in 6ms
npm verb logfile logs-max:10 dir:/Users/muharremsalel/.npm/_logs
npm verb logfile /Users/muharremsalel/.npm/_logs/2022-08-09T14_52_53_168Z-debug-0.log
npm timing npm:load:logFile Completed in 4ms
npm timing npm:load:timers Completed in 0ms
npm timing npm:load:configScope Completed in 1ms
npm timing npm:load Completed in 26ms

> codeceptjs-tests@0.1.0 codeceptjs
> codeceptjs run --steps

CodeceptJS v3.3.3 #StandWithUkraine:load Completed in 26ms
Using test root "/Users/muharremsalel/Desktop/CRDao/dhf-pay-bitrix/tests/end2end"

1. Validate module installation and settings --ted in 26ms
  1.1. Module citrus.dhfi should be installed
    I am on page "/" ⠴ : timing npm:load Completed in 26ms
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"
    modules: installed "citrus.dhfi"
      I am on page "/bitrix/admin/partner_modules.php"
      I see "(citrus.dhfi)"ming npm:load Completed in 26ms
      I grab text from all "#upd_partner_modules_all > tbody > tr > td:nth-child(2)"
    I grab text from all "#upd_partner_modules_all > tbody > tr > td:last-child"
    I: grabLanguage 
      I execute script () => BX.message('LANGUAGE_ID')
  ✔ OK in 927ms

  1.2. Currency CSP should existnpm:load Completed in 26ms
    I am on page "/" ⠴ : timing npm:load Completed in 26ms
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"
    paysystems: currencyExists "CSP"
      I am on page "/bitrix/admin/currency_edit.php?lang=ru&ID=CSP"
      I see "CSP"⠂⠂) ⠴ : timing npm:load Completed in 26ms
      I see attributes on elements "form input[name=ID]", {"value":"CSP"}
   Found currency: CSP
  ✔ OK in 971ms

  1.3. Paysystem for old invoices should existeted in 26ms
    I am on page "/" ⠴ : timing npm:load Completed in 26ms
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"
    paysystems: paysystemInCrm "dhfi"
      I am on page "/crm/configs/ps/"
      I grab attribute from all ".crm-config-ps-list-widget-row a.crm-config-ps-list-widget-title", "href"
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/1/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/2/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/3/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/4/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/6/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/7/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/8/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/9/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/11/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
   Found active paysystem DHFinance (dhfi) for old invoices
    I am on page "http://tsaritnp.beget.tech/crm/configs/ps/edit/13/"
    I grab attribute from "#PS_INFO input[name=NAME]", "value"
    I grab attribute from "#PS_INFO #ACTION_FILE option[selected]", "value"
    I grab attribute from "#PS_INFO input[name=ACTIVE]", "value"
   Found active paysystem DHFinance (dhfi) for old invoices
  ✔ OK in 15951ms

  1.4. Paysystem for new invoices should existeted in 26ms
    I am on page "/" ⠴ : timing npm:load Completed in 26ms
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"timing npm:load Completed in 26ms
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"oad Completed in 26ms
    paysystems: paysystemInSalehub "dhfi", 10
      I am on page "/saleshub/"
      I click "[data-id=payment-systems]"Completed in 26ms
      I wait for element "iframe.side-panel-iframe", 106ms
    Within "{"frame":[".side-panel-iframe"]}" eted in 26ms
      I wait for element "#salescenter-paysystem", 10
      I see element ".salescenter-paysystem-item-status-selected", "[data-id=dhfi]"
   Paysystem active dhfi for new invoices
  ✔ OK in 9179ms

2. Old invoices payment --iming npm:load Completed in 26ms
  2.1. Old invoice payment
    I am on page "/" ⠴ : timing npm:load Completed in 26ms
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"timing npm:load Completed in 26ms
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"
    I: setInvoiceCurrency "CSP"
      I execute async script (currency, done) => {
                // noinspection JSVoidFunctionReturnValueUsed
                BX.ajax.runAction('citrus:dhfi.util.Crm.setInvoiceCurrency', {data: {id: currency}})
                    .then(response => done(response.data.prev));
            }, "CSP"
    I am on page "/crm/invoice/list/"oad Completed in 26ms
    invoiceStep: create 16iming npm:load Completed in 26ms
      I call rest "crm.company.list", {"order":{"DATE_CREATE":"ASC"},"select":["ID","TITLE"]}
    I assert length above than [{"ID":"1","TITLE":"ЗАО \"МПЗК\""},{"ID":"2","TITLE":"ООО \"МТД Реклама\""},{"ID":"3","TITLE":"ИП \"Титов Г.Н\""},{"ID":"4","TITLE":"ООО \"Логистика-север\""},{"ID":"5","TITLE":"ООО \"Новые технологии\""}], 
    I: fetchOneProduct 
      I call rest "crm.product.list", {"order":{"ID":"ASC"},"select":["ID","NAME","CURRENCY_ID","PRICE"]}
    I assert length above than [{"ID":"30","NAME":"Разработка дизайна сайта","CURRENCY_ID":"RUB","PRICE":"15000.00"},{"ID":"31","NAME":"Работы по настройке БУС под клиента","CURRENCY_ID":"RUB","PRICE":"20000.00"},{"ID":"32","NAME":"Обучение контент-менеджеров","CURRENCY_ID":"RUB","PRICE":"5000.00"},{"ID":"33","NAME":"Ip1","CURRENCY_ID":null,"PRICE":null},{"ID…
    I call rest "crm.persontype.list"
    I call rest "crm.paysystem.list"load Completed in 26ms
    I assert length above than [{"ID":"1","NAME":"Банковский перевод (Компании)","ACTIVE":"Y","SORT":"100","DESCRIPTION":"","PERSON_TYPE_ID":"1","ACTION_FILE":"/bitrix/modules/sale/payment/bill","HANDLER":"bill","HANDLER_CODE":"bill","HANDLER_NAME":"Invoice (Russian) (bill)"},{"ID":"3","NAME":"Предложение (Компании)","ACTIVE":"Y","SORT":"200","DESCRIPTION":""…
    I call rest "crm.invoice.add", {"fields":{"PERSON_TYPE_ID":"1","UF_COMPANY_ID":"1","PAY_SYSTEM_ID":"1","ORDER_TOPIC":"Test invoice 8/9/2022, 5:53:50 PM","STATUS_ID":"N","PRODUCT_ROWS":[{"ID":0,"PRODUCT_ID":"30","PRODUCT_NAME":"Test product","QUANTITY":1,"PRICE":16}]}}
    invoiceStep: getPublicUrl {"id":23,"url":"/crm/invoice/show/23/"}
      I am on page "/crm/invoice/show/23/"
      I click "#crm_invoice_toolbar_leftMenu", ".bx-crm-view-menu"
      I execute script () => generateExternalLink(BX("crm_invoice_toolbar_leftMenu"))
      I wait for element "#generated-link"
      I grab value from "#generated-link"Completed in 26ms
    I: logout 
      I am on page "/bitrix/admin/index.php?logout=yes"
    invoiceStep: tryToPay "http://tsaritnp.beget.tech/pub/pay/MjM/6a681b45cb19cc791c1878a6b21e005a/", 16
      I am on page "http://tsaritnp.beget.tech/pub/pay/MjM/6a681b45cb19cc791c1878a6b21e005a/"
      I see element Pay usingng npm:load Completed in 26ms
      I see "16 CSPR", ".crm-invoice-payment-total-sum"
      I see element DHFinance payment method
      I click DHFinance payment method
      I wait for element Paysystem response, 5eted in 26ms
      I click {xpath: .//*[(contains(concat(' ', normalize-space(./@class), ' '), ' btn ') and contains(concat(' ', normalize-space(./@class), ' '), ' btn-success '))][ancestor::*[contains(concat(' ', normalize-space(./@class), ' '), ' crm-invoice-payment-client-template ')][ancestor::*[contains(concat(' ', normalize-space(./@class), ' '), ' crm-invoice-pa…
      I see "Amount" ⠴ : timing npm:load Completed in 26ms
      I see "Comment"⠴ : timing npm:load Completed in 26ms
      I see "16 CSPR"
  ✔ OK in 13066ms

    I am on page "/"
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"
    I: setInvoiceCurrency "CSP"
      I execute async script (currency, done) => {
                // noinspection JSVoidFunctionReturnValueUsed
                BX.ajax.runAction('citrus:dhfi.util.Crm.setInvoiceCurrency', {data: {id: currency}})
                    .then(response => done(response.data.prev));
            }, "CSP"
  2.2. There should be an error for invoices less than 2.5 CSPR
    I am on page "/" ⠴ : timing npm:load Completed in 26ms
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"oad Completed in 26ms
    I: setInvoiceCurrency "CSP"
      I execute async script (currency, done) => {
                // noinspection JSVoidFunctionReturnValueUsed
                BX.ajax.runAction('citrus:dhfi.util.Crm.setInvoiceCurrency', {data: {id: currency}})
                    .then(response => done(response.data.prev));
            }, "CSP"
    I am on page "/crm/invoice/list/"oad Completed in 26ms
    invoiceStep: create 1.5ming npm:load Completed in 26ms
      I call rest "crm.company.list", {"order":{"DATE_CREATE":"ASC"},"select":["ID","TITLE"]}
    I assert length above than [{"ID":"1","TITLE":"ЗАО \"МПЗК\""},{"ID":"2","TITLE":"ООО \"МТД Реклама\""},{"ID":"3","TITLE":"ИП \"Титов Г.Н\""},{"ID":"4","TITLE":"ООО \"Логистика-север\""},{"ID":"5","TITLE":"ООО \"Новые технологии\""}], 
    I: fetchOneProduct 
      I call rest "crm.product.list", {"order":{"ID":"ASC"},"select":["ID","NAME","CURRENCY_ID","PRICE"]}
    I assert length above than [{"ID":"30","NAME":"Разработка дизайна сайта","CURRENCY_ID":"RUB","PRICE":"15000.00"},{"ID":"31","NAME":"Работы по настройке БУС под клиента","CURRENCY_ID":"RUB","PRICE":"20000.00"},{"ID":"32","NAME":"Обучение контент-менеджеров","CURRENCY_ID":"RUB","PRICE":"5000.00"},{"ID":"33","NAME":"Ip1","CURRENCY_ID":null,"PRICE":null},{"ID…
    I call rest "crm.persontype.list"
    I call rest "crm.paysystem.list"load Completed in 26ms
    I assert length above than [{"ID":"1","NAME":"Банковский перевод (Компании)","ACTIVE":"Y","SORT":"100","DESCRIPTION":"","PERSON_TYPE_ID":"1","ACTION_FILE":"/bitrix/modules/sale/payment/bill","HANDLER":"bill","HANDLER_CODE":"bill","HANDLER_NAME":"Invoice (Russian) (bill)"},{"ID":"3","NAME":"Предложение (Компании)","ACTIVE":"Y","SORT":"200","DESCRIPTION":""…
    I call rest "crm.invoice.add", {"fields":{"PERSON_TYPE_ID":"1","UF_COMPANY_ID":"1","PAY_SYSTEM_ID":"1","ORDER_TOPIC":"Test invoice 8/9/2022, 5:54:12 PM","STATUS_ID":"N","PRODUCT_ROWS":[{"ID":0,"PRODUCT_ID":"30","PRODUCT_NAME":"Test product","QUANTITY":1,"PRICE":1.5}]}}
    invoiceStep: getPublicUrl {"id":24,"url":"/crm/invoice/show/24/"}
      I am on page "/crm/invoice/show/24/"
      I click "#crm_invoice_toolbar_leftMenu", ".bx-crm-view-menu"
      I execute script () => generateExternalLink(BX("crm_invoice_toolbar_leftMenu"))
      I wait for element "#generated-link"
      I grab value from "#generated-link"Completed in 26ms
    I: logout 
      I am on page "/bitrix/admin/index.php?logout=yes"
    I: grabLanguage  ⠴ : timing npm:load Completed in 26ms
      I execute script () => BX.message('LANGUAGE_ID')
    invoiceStep: tryToPay "http://tsaritnp.beget.tech/pub/pay/MjQ/b57e90932720d2b679a1a0bc599847d1/", 1.5, "Minimum amount for payment: 2.5 CSPR"
      I am on page "http://tsaritnp.beget.tech/pub/pay/MjQ/b57e90932720d2b679a1a0bc599847d1/"
      I see element Pay usingng npm:load Completed in 26ms
      I see "1,50 CSPR", ".crm-invoice-payment-total-sum"
      I see element DHFinance payment method
      I click DHFinance payment method
      I wait for element Paysystem response, 5eted in 26ms
      I see "Minimum amount for payment: 2.5 CSPR", Paysystem response
  ✔ OK in 12288ms

    I am on page "/"
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"timing npm:load Completed in 26ms
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"
    I: setInvoiceCurrency "CSP"
      I execute async script (currency, done) => {
                // noinspection JSVoidFunctionReturnValueUsed
                BX.ajax.runAction('citrus:dhfi.util.Crm.setInvoiceCurrency', {data: {id: currency}})
                    .then(response => done(response.data.prev));
            }, "CSP"
3. New invoices payment --iming npm:load Completed in 26ms
  3.1. New invoice payment
    I am on page "/" ⠴ : timing npm:load Completed in 26ms
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"
    I am on page "/crm/"
    smartInvoiceStep: create 8g npm:load Completed in 26ms
      I call rest "crm.enum.ownertype"
    I: fetchOneProduct : timing npm:load Completed in 26ms
      I call rest "crm.product.list", {"order":{"ID":"ASC"},"select":["ID","NAME","CURRENCY_ID","PRICE"]}
    I assert length above than [{"ID":"30","NAME":"Разработка дизайна сайта","CURRENCY_ID":"RUB","PRICE":"15000.00"},{"ID":"31","NAME":"Работы по настройке БУС под клиента","CURRENCY_ID":"RUB","PRICE":"20000.00"},{"ID":"32","NAME":"Обучение контент-менеджеров","CURRENCY_ID":"RUB","PRICE":"5000.00"},{"ID":"33","NAME":"Ip1","CURRENCY_ID":null,"PRICE":null},{"ID…
    I call rest "crm.item.add", {"entityTypeId":31,"fields":{"title":"Test invoice 8/9/2022, 5:54:32 PM"}}
    I call rest "crm.item.productrow.set", {"ownerType":"SI","ownerId":4,"currencyId":"CSPR","productRows":[{"productId":"30","productName":"Test product","quantity":1,"price":8}]}
   Creating public invoice link npm:load Completed in 26ms
    smartInvoiceStep: getPublicUrl {"id":4,"url":"/crm/type/31/details/4/"}
      I am on page "/crm/type/31/details/4/"
      I wait for element Receive payment buttonted in 26ms
      I see element Receive payment buttonompleted in 26ms
      I click SMS/WhatsApp tab in timelineompleted in 26ms
      I click SMS enabled sales link on the SMS/WhatsApp tab
      I execute script () => BX.message('LANGUAGE_ID')26ms
    I wait for element ".side-panel-iframe"
    Within "{"frame":".side-panel-iframe"}" pleted in 26ms
      I wait for element ".ui-page-slider-workarea", 5
      I see "CRM.Payment"timing npm:load Completed in 26ms
  ✖ FAILED in 15965ms⠴ : timing npm:load Completed in 26ms

  3.2. There should be an error for invoices less than 2.5 CSPR
    I am on page "/" ⠴ : timing npm:load Completed in 26ms
    I set cookie [{"name":"BITRIX_CONVERSION_CONTEXT_s1","value":"%7B%22ID%22%3A3%2C%22EXPIRE%22%3A1660078740%2C%22UNIQUE%22%3A%5B%22conversion_visit_day%22%5D%7D","domain":"tsaritnp.beget.tech","path":"/","expires":1691588351.80601,"size":124,"httpOnly":false,"secure":false,"session":false,"sameParty":false,"sourceScheme":"NonSecure","sourcePort":80},{"name"…
    I: isLoggedIn "admin"
      I am on page "/bitrix/admin/index.php#authorize"
      I see element "#bx-panel-logout"ad Completed in 26ms
      I grab cookie "BITRIX_SM_LOGIN"
    I: fetchOneProduct 
      I call rest "crm.product.list", {"order":{"ID":"ASC"},"select":["ID","NAME","CURRENCY_ID","PRICE"]}
    I assert length above than [{"ID":"30","NAME":"Разработка дизайна сайта","CURRENCY_ID":"RUB","PRICE":"15000.00"},{"ID":"31","NAME":"Работы по настройке БУС под клиента","CURRENCY_ID":"RUB","PRICE":"20000.00"},{"ID":"32","NAME":"Обучение контент-менеджеров","CURRENCY_ID":"RUB","PRICE":"5000.00"},{"ID":"33","NAME":"Ip1","CURRENCY_ID":null,"PRICE":null},{"ID…
    I call rest "crm.item.add", {"entityTypeId":31,"fields":{"title":"Test invoice 8/9/2022, 5:54:46 PM"}}
    I call rest "crm.item.productrow.set", {"ownerType":"SI","ownerId":5,"currencyId":"CSPR","productRows":[{"productId":"30","productName":"Test product","quantity":1,"price":1.5}]}
   Creating public invoice link npm:load Completed in 26ms
    smartInvoiceStep: getPublicUrl {"id":5,"url":"/crm/type/31/details/5/"}
      I am on page "/crm/type/31/details/5/"
      I wait for element Receive payment buttonted in 26ms
      I see element Receive payment button
      I click SMS/WhatsApp tab in timeline
      I click SMS enabled sales link on the SMS/WhatsApp tab
      I execute script () => BX.message('LANGUAGE_ID')26ms
    I wait for element ".side-panel-iframe"
    Within "{"frame":".side-panel-iframe"}" pleted in 26ms
      I wait for element ".ui-page-slider-workarea", 5
      I see "CRM.Payment"timing npm:load Completed in 26ms
  ✖ FAILED in 19860ms⠴ : timing npm:load Completed in 26ms

(⠂⠂⠂⠂⠂⠂⠂⠂⠂⠂⠂⠂⠂⠂⠂⠂⠂⠂) ⠴ : timing npm:load Completed in 26ms
-- FAILURES:

  1) 3. New invoices payment
       3.1. New invoice payment:

      expected web application to include "CRM.Payment"
      + expected - actual

      -Chat enabled sales
      -Chat enabled sales pages
      -EXPAND
      -+add a page
      -Payments
      -CRM forms
      -EXPAND
      -+add a page
      -SEND CANCEL
      +CRM.Payment
      
  
  
  Scenario Steps:
  - I.see("CRM.Payment") at ./steps/smartInvoice.js:50:15
  - I.waitForElement(".ui-page-slider-workarea", 5) at ./steps/smartInvoice.js:49:15
  - I.waitForElement(".side-panel-iframe") at Object.getPublicUrl (./steps/smartInvoice.js:47:11)
  - I.executeScript(() => BX.message('LANGUAGE_ID')) at Actor.grabLanguage (./steps_file.js:50:25)
  - I.click(SMS enabled sales link on the SMS/WhatsApp tab) at Object.getPublicUrl (./steps/smartInvoice.js:21:11)
  - I.click(SMS/WhatsApp tab in timeline) at Object.getPublicUrl (./steps/smartInvoice.js:20:11)
  - I.seeElement(Receive payment button) at Object.getPublicUrl (./steps/smartInvoice.js:18:11)
  - I.waitForElement(Receive payment button) at Object.getPublicUrl (./steps/smartInvoice.js:17:11)
  - I.amOnPage("/crm/type/31/details/4/") at Object.getPublicUrl (./steps/smartInvoice.js:14:11)
  - I.callRest("crm.item.productrow.set", {"ownerType":"SI","ownerId":4,"currencyId":"CSPR","productRows":[{"productId":"30","productName":"Test product","quantity":1,"price":8}]}) at Object.create (./steps/smartInvoice.js:95:17)
  - I.callRest("crm.item.add", {"entityTypeId":31,"fields":{"title":"Test invoice 8/9/2022, 5:54:32 PM"}}) at Object.create (./steps/smartInvoice.js:88:34)
  - I.assertLengthAboveThan([{"ID":"30","NAME":"Разработка дизайна сайта","CURRENCY_ID":"RUB","PRICE":"15000.00"},{"ID":"31","NAME":"Работы по настройке БУС под клиента","CURRENCY_ID":"RUB","PRICE":"20000.00"},{"ID":"32","NAME":"Обучение контент-менеджеров","CURRENCY_ID":"RUB","PRICE":"5000.00"},{"ID":"33","NAME":"Ip1","CURRENCY_ID":null,"PRICE":null},{"ID":"34","NAME":"Book 1","CURRENCY_ID":"CSP","PRICE":"3.00"},{"ID":"35","NAME":"Book 2","CURRENCY_ID":"CSP","PRICE":"6.00"},{"ID":"36","NAME":"Another book","CURRENCY_ID":"CSP","PRICE":"1.00"},{"ID":"37","NAME":"Limit book","CURRENCY_ID":"CSP","PRICE":"2.50"}], ) at Actor.fetchOneProduct (./steps_file.js:19:18)
  - I.callRest("crm.product.list", {"order":{"ID":"ASC"},"select":["ID","NAME","CURRENCY_ID","PRICE"]}) at Actor.fetchOneProduct (./steps_file.js:14:39)
  - I.callRest("crm.enum.ownertype") at Object.getEntity (./steps/smartInvoice.js:120:37)
  - I.amOnPage("/crm/") at Test.<anonymous> (./tests/030_smartInvoice.js:9:7)
  
  Artifacts:
  - screenshot: /Users/muharremsalel/Desktop/CRDao/dhf-pay-bitrix/tests/end2end/output/3.1._New_invoice_payment.failed.png

  2) 3. New invoices payment
       3.2. There should be an error for invoices less than 2.5 CSPR:

      expected web application to include "CRM.Payment"
      + expected - actual

      -Chat enabled sales
      -Chat enabled sales pages
      -EXPAND
      -+add a page
      -Payments
      -CRM forms
      -EXPAND
      -+add a page
      -SEND CANCEL
      +CRM.Payment
      
  
  
  Scenario Steps:
  - I.see("CRM.Payment") at ./steps/smartInvoice.js:50:15
  - I.waitForElement(".ui-page-slider-workarea", 5) at ./steps/smartInvoice.js:49:15
  - I.waitForElement(".side-panel-iframe") at Object.getPublicUrl (./steps/smartInvoice.js:47:11)
  - I.executeScript(() => BX.message('LANGUAGE_ID')) at Actor.grabLanguage (./steps_file.js:50:25)
  - I.click(SMS enabled sales link on the SMS/WhatsApp tab) at Object.getPublicUrl (./steps/smartInvoice.js:21:11)
  - I.click(SMS/WhatsApp tab in timeline) at Object.getPublicUrl (./steps/smartInvoice.js:20:11)
  - I.seeElement(Receive payment button) at Object.getPublicUrl (./steps/smartInvoice.js:18:11)
  - I.waitForElement(Receive payment button) at Object.getPublicUrl (./steps/smartInvoice.js:17:11)
  - I.amOnPage("/crm/type/31/details/5/") at Object.getPublicUrl (./steps/smartInvoice.js:14:11)
  - I.callRest("crm.item.productrow.set", {"ownerType":"SI","ownerId":5,"currencyId":"CSPR","productRows":[{"productId":"30","productName":"Test product","quantity":1,"price":1.5}]}) at Object.create (./steps/smartInvoice.js:95:17)
  - I.callRest("crm.item.add", {"entityTypeId":31,"fields":{"title":"Test invoice 8/9/2022, 5:54:46 PM"}}) at Object.create (./steps/smartInvoice.js:88:34)
  - I.assertLengthAboveThan([{"ID":"30","NAME":"Разработка дизайна сайта","CURRENCY_ID":"RUB","PRICE":"15000.00"},{"ID":"31","NAME":"Работы по настройке БУС под клиента","CURRENCY_ID":"RUB","PRICE":"20000.00"},{"ID":"32","NAME":"Обучение контент-менеджеров","CURRENCY_ID":"RUB","PRICE":"5000.00"},{"ID":"33","NAME":"Ip1","CURRENCY_ID":null,"PRICE":null},{"ID":"34","NAME":"Book 1","CURRENCY_ID":"CSP","PRICE":"3.00"},{"ID":"35","NAME":"Book 2","CURRENCY_ID":"CSP","PRICE":"6.00"},{"ID":"36","NAME":"Another book","CURRENCY_ID":"CSP","PRICE":"1.00"},{"ID":"37","NAME":"Limit book","CURRENCY_ID":"CSP","PRICE":"2.50"}], ) at Actor.fetchOneProduct (./steps_file.js:19:18)
  - I.callRest("crm.product.list", {"order":{"ID":"ASC"},"select":["ID","NAME","CURRENCY_ID","PRICE"]}) at Actor.fetchOneProduct (./steps_file.js:14:39)
  
  Artifacts:
  - screenshot: /Users/muharremsalel/Desktop/CRDao/dhf-pay-bitrix/tests/end2end/output/3.2._There_should_be_an_error_for_invoices_less_than_2.5_CSPR.failed.png


  FAIL  | 6 passed, 2 failed   // 2m
Run with --verbose flag to see complete NodeJS stacktrace
npm timing command:run Completed in 132635ms
npm verb exit 1
npm timing npm Completed in 132669ms
npm verb code 1

'''