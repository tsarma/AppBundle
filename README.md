# Contao 4 local bundle
Path-> /src/NamespaceName/MyLocalbundle

Local bundles are modules which is installed for particular installation. It is not meant for distribution via packagist, thus it can not be installed with composer. It is located inside folder /src. 

With above directory structure `/src/\<Vendorname>/\<BundleName>`, you don't need a composer.json in your bundle. But you have to add 
```
"autoload": {
   "psr-4": { "": "src/" },
},
```
to the main composer.json file in root folder.
