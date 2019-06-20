## Photo Library

```
ionic cordova plugin add cordova-plugin-photo-library
npm install @ionic-native/photo-library
```

```
import { PhotoLibrary } from '@ionic-native/photo-library/ngx';

constructor(private photoLibrary: PhotoLibrary) { }
```

#### requestAuthorization(options?: RequestAuthorizationOptions): Promise< void > // 查询权限

#### saveImage(url: string, album: AlbumItem | string, options?: GetThumbnailOptions): Promise< LibraryItem > // 保存图片

##### url // src, 可以是base64
##### album //  相册专辑名称
