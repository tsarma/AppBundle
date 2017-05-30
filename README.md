# Contao 4 local bundle
Path-> /src/NamespaceName/MyLocalbundle

Local bundles are modules which is installed for particular installation. It is not meant for distribution via packagist, thus it can not be installed with composer. It is located inside folder `/src`. 

With above directory structure `/src/<Vendorname>/<BundleName>`, you don't need a composer.json in your bundle folder. But you have to add 
```
"autoload": {
   "psr-4": { "": "src/" },
},
```
to the main composer.json file in root folder.

You may download this and place it inside `/src` folder. (if there is no `src` folder , you can create one yourself). 
Oh! I need to mention this: I've copied and adapted this mostly from http://easysolutionsit.de/artikel/contao-4-erweiterung-als-bundle.html
