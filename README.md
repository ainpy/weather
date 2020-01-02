**Weather**
--  
基于 [高德开放平台](https://lbs.amap.com/api/webservice/guide/api/weatherinfo/) 的 PHP 天气信息组件。  
[![Build Status](https://travis-ci.org/ainpy/weather.svg?branch=master)](https://travis-ci.org/ainpy/weather)  

**安装**
-
``
$ composer require ainpy/weather -vvv
``  

**配置**
---
在使用本扩展之前，你需要去 [高德开放平台](https://lbs.amap.com/api/webservice/guide/api/weatherinfo/) 注册账号，然后创建应用，获取应用的 API KEY。  

**使用**
---
```
use Ainpy\Weather\Weather;

$key = 'xxx';

$weather = new Weather($key);
```  

**获取实时天气**
```
$response = $weather->getWeather('北京');
```  

