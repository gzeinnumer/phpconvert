# phpconvert
 
```php
<?php

//json object
$json = '
{
    "name" : "zein",
    "age" : 17
}
';

$foo = json_decode($json);
echo $foo->name."-".$foo->age."<br>";

$json = json_encode($foo);
echo $json."<br><br>";

//result
/*
zein-17
{"name":"zein","age":17}
*/
```
 
```php
<?php

//json array
$jsonArray = '
[
    {
        "name" : "zein1",
        "age" : 1
    },    
    {
        "name" : "zein2",
        "age" : 2
    }
]
';

$bar = json_decode($jsonArray);
echo $bar[0]->name."-".$bar[0]->age."<br>";
echo $bar[1]->name."-".$bar[1]->age."<br>";

$jsonArray = json_encode($bar);
echo $jsonArray."<br>";

//result
/*
zein1-1
zein2-2
[{"name":"zein1","age":1},{"name":"zein2","age":2}]
*/
```

---

```
Copyright 2022 M. Fadli Zein
```
