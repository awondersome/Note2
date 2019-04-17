## ion-app

*每个项目只能有一个ion-app*

## ion-router-outlet 

*只应用在app.component和tabs.component中*

```
<ion-app>
 <ion-router></ion-router>
</ion-app>
```

```
// tabs里面的ion-router-outlet可以省略

<ion-router-outlet></ion-router-outlet>
<tabs></tabs>
```

* animated 动画

* animation 自定义动画

* ionViewWillEnter

* ionViewDidEnter

* ionViewWillLeave

* ionViewDidLeave

## ion-tabs

### ion-tab-bar

### ion-tab-button


## ModalController

```
constructor(public modalController: ModalController) {}

async function() {
 const modal = await this.modalController.create({option})
 return await modal.present()
}

```

* create

  * component
  * componentProps
  * cssClass
  * mode

## ion-backdrop

*默认opacity=0.01*



## ion-grid

*必须配合row*

### ion-row 

*必须配合col*

### ion-col 

*可以嵌套row*

* size

  * auto
  * number 可以小数
  
  
## ion-input

* clearInput

* clearOnEdit

## ion-radio-group

### ion-radio

* checked
