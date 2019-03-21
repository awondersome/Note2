# Note2
整理后的笔记


### http封装

业务ts应该订阅一个observable，可以独立处理成功和错误回调

``http.post(url, data).subscribe``
``api.post(data).subscribe()``

api服务ts应该接收一个observable并返回一个observable，统一封装api的url

``return this.http.post(url, data)``

http服务ts返回一个observable


angular ng-zorro ng-alain ionic
