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
