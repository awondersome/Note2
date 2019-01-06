基于angular和ng-zorro

#### 新增页面

ng g ng-alain:module moduleName // 新建模块

ng g ng-alain:list pageName -m=moduleName // 新建页面

```
list: 列表页
curd: 带编辑和查看的列表页
```

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


#### st

##### data

`[data] = "url"` 数据源


##### req

`[req] = ""` 请求配置


##### res

`[res] = ""` 接收配置


##### columns

```
[columns] = {
  title: '', // 列名
  index: '', // key
  buttons: [
    {
      text: '' // 按钮名
    }
  ],
  format: (record.index) => {return ''}, // 格式化数据
}
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
