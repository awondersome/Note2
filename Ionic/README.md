ionic4

结构变化

provider => service

page => router

alert => promise

```
<app-root>
  <ion-app>
    <ion-router-outlet>
      <ion-tabs>
      </ion-tabs>
    </ion-router-outlet>
  </ion-app>
</app-root>
```

ion-tab => ion-tab-bar

ion-back-button


## Theme 主题系统

### mode模式

不同平台会加载不同的样式

### css变量

使用全新的css变量，var()可以使用其他变量的值，setProperty()可以使用动态设置变量的值，getPropertyValue可以获取变量的值


### color属性

仅应用于组件
