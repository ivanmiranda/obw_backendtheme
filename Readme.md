# Backend Theme for Magento2 (tested with Magento 2.1.x)
This is a backend theme for Magento2 that is our default, for every project.

## Installation

### 1. If you install ObwHub, this theme is autoreferenced

### 2. Manual Installation

#### a) Zip
 * Download this repo on app/design/adminhtml/obw/Backendtheme

#### b) Composer
 * Require dependency via composer:
```
 	composer require obw/backendtheme
```

#### For bot options: register this theme via module, creating at least, the following files:

##### etc/di.xml
```
<?xml version="1.0"?>
<config xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="urn:magento:framework:ObjectManager/etc/config.xsd">
    <type name="Magento\Theme\Model\View\Design">
        <arguments>
            <argument name="themes" xsi:type="array">
                <item name="adminhtml" xsi:type="string">Obw/Backendtheme</item>
            </argument>
         </arguments>
    </type>
</config>
```

##### etc/module.xml
```
<?xml version="1.0"?>
<config xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="urn:magento:framework:Module/etc/module.xsd">
	<module name="Obw_Module" setup_version="0.0.1">
		<sequence>
            <module name="Magento_Backend"/>
        </sequence>
	</module>
</config>
```


#### NOTICE OF LICENSE
![saltamontes](https://i.creativecommons.org/l/by-nc-nd/3.0/88x31.png)
This work is licensed under a ***Creative Commons Attribution-NonCommercial-NoDerivs 3.0 Unported License*** http://creativecommons.org/licenses/by-nc-nd/3.0

**Happy coding!**
- [ivan miranda](http://ivanmiranda.me)