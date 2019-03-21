### ng add 创建项目

```
ng new demo --style less  // 新建angular项目

ng add ng-alain // 添加alain脚手架
```

### ng g 新建页面

```
ng g ng-alain:[command] [name] [options]
```

#### [command name]

```
ng g ng-alain:module moduleName // 新建模块，生成moduleName.module.ts和moduleName-routing.module.ts两个文件，不影响其他文件

ng g ng-alain:empty pageName -m=moduleName // 新建空白页面，生成pageName.component两个文件，影响指定的module，会在自动导入组件和配置路由

ng g ng-alain:list pageName -m=moduleName // 新建列表页面

ng g ng-alain:edit pageName -m=moduleName // 新建编辑页面

ng g ng-alain:view pageName -m=moduleName // 新建查看页面

ng g ng-alain:curd pageName -m=moduleName // 新建列表页面，并生成编辑、查看页面
```

#### [options]

```
-m=moduleName // 是必须的，指定页面在哪个模块下生成

-t=pageName // 指定在哪个页面生成，可以指定路径pageName/pageName

--modal=false // view和edit页面默认是true，如果是modal就不会生成路由
```
