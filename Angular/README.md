angular

### cli

#### ng new <name> [option]
  
#### ng g <schematic> [option]
  
* ng g component <name> [option]
  
#### ng add <collection> [options]
 
#### ng serve <project> [options]
  
### 生命周期

* ngOnInit() 在组件被创建时触发

### 组件

#### Form

* 响应式

`FormGroup 是一组FormControl`

`FormControl 单个表单控件的值和状态`

`(ngSubmit) 表单提交事件`

`Validators 验证器`

`FormGroup = FormBuilder.group({name: []})`

* 模板驱动

`[value]`

`[(ngModle)]`

`#name="ngModel"`


## 路由

### RouterModule

```
// app.module.ts

@NgModule({
  imports: [
    RouterModule.forRoot()
  ]
})
```
* forRoot(routes, config)

* forChild(routes)

根html设置<base href="/">

app.module

```
@NgModule({
  imports: [
    RouterModule.forRoot([{path: '', loadChilren: ''}],  { preloadingStrategy: PreloadAllModules })
  ]
})
```

#### path
字符串，假路径

#### component
被导航时使用的组件

#### redirectTo
重定向

#### pathMatch
完全匹配

<router-outlet></router-outlet>

routerLink

routerLinkActive

routerLinkActiveOptions

router.events

### activatedRoute

#### snapshot


## Location
