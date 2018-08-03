# C5-Get-Attribute-from-Set
Concrete5, Get all data from attribute set


## A Simple Example
```php
$set = AttributeSet::getByHandle('career'); // set handle
$keys = $set->getAttributeKeys();
foreach($keys as $key) :
$akhandle = $key->getAttributeKeyHandle();
$akname = $key->getAttributeKeyName();
$akvalue= $c->getAttribute($akhandle);
echo '<li><span>'.$akname.' :</span> '.$akvalue.'</li>';
endforeach;
```
