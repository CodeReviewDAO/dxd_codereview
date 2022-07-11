```sh
ggurbet@crdao:/var/www/casperfyre-api$ composer run-script generate-docs
> ./phpdoc -d . --ignore docs/ --ignore vendor/ --ignore .git/ -t docs && ./phpdoc -d public/external_api/v1/ --ignore public/external_api/v1/index.php -t public/docs && sed -i 's/--primary-color-hue: 96/--primary-color-hue: 1/' public/docs/css/base.css && sed -i 's/--primary-color-saturation: 57/--primary-color-saturation: 80/' public/docs/css/base.css
phpDocumentor v3.3.1

Parsing files

   1/100 [>---------------------------]   1%
  10/100 [==>-------------------------]  10%
  30/100 [========>-------------------]  30%
  50/100 [==============>-------------]  50%
  70/100 [===================>--------]  70%
  90/100 [=========================>--]  90%
 100/100 [============================] 100%
Applying transformations (can take a while)

  1/21 [=>--------------------------]   4%
  3/21 [====>-----------------------]  14%
  5/21 [======>---------------------]  23%
  7/21 [=========>------------------]  33%
 15/21 [====================>-------]  71%
 19/21 [=========================>--]  90%
 21/21 [============================] 100%
All done in 1 seconds!
phpDocumentor v3.3.1

Parsing files

 1/1 [============================] 100%
Applying transformations (can take a while)

  1/21 [=>--------------------------]   4%
  7/21 [=========>------------------]  33%
 17/21 [======================>-----]  80%
 21/21 [============================] 100%
All done in 0 seconds!
```