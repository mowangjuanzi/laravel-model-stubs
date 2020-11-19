# laravel-model-stubs

Laravel 模型方法提示

## 要求

本项目仅支持Laravel v6 ~ v8

> 本项目未来会发布到 composer。但是目前方法还没添加完整。所以下面的方法并不可行。

## 安装

```bash
composer require mowangjuanzi/laravel-model-stubs
```

## 使用

比如下面是我们开发中的一个Model

```php
<?php

namespace App;

use Illuminate\Database\Eloquent\Model;

class VoteUserLog extends Model
{
    //
}

```

那么我们引入 `Mowangjuanzi\LaravelModelStubs\LaravelModelStubs`即可。

引入后则变为如下：

```php
<?php

namespace App;

use Illuminate\Database\Eloquent\Model;
use Mowangjuanzi\LaravelModelStubs\LaravelModelStubs;

class VoteUserLog extends Model
{
    use LaravelModelStubs;
}
```

接下来对要使用Model都如法炮制，添加该 trait。则会在开发中自动进行方法提示，提升开发效率了。

enjoy😁!
