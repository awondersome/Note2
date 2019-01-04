基于angular和ng-zorro

#### 菜单

`src\app\core\startup\startup.service.ts`

```
this.menuService.add([
  text: 标题
  group: 分组
  hideInBreadcrumb：隐藏面包屑
  children: []
])
```

#### 路由

`src\app\routes\routes-routing.module.ts`

```
const routes: Routes = [{
  children： [
    {path: '', loadChildren: './'}
  ]
}]
```


#### sf

##### JSON Schema

```
searchSchema: SFSchema = {
  type: 'object', // 定义类型，默认 `object`
  properties: { // 定义属性
    no: {
      type: 'string',
      title: '编号'
    }
  }
}
```

##### ui

```
ui = {
  $url: { // 区别于Schema的url
    addOnBefore: 'https://'
  }
}
```

##### mode

`mode="search"`
