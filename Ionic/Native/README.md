## Camera

```
ionic cordova plugin add cordova-plugin-camera
npm install @ionic-native/camera
```

```
import { Camera } from '@ionic-native/camera/ngx';

constructor(private camera: Camera) { }
```

+ 获取图片

   ```
   getPicture(options?: CameraOptions): Promise<any>
   ```

   + CameraOptions

    ```
    /**
     * 像素范围 0-100. Default is 50
     */

    quality?: number;
    ```


    ```
    /**
     *      DATA_URL : 0,   Return image as base64-encoded string,
     *      FILE_URI : 1,   Return image file URI,
     *      NATIVE_URI : 2  Return image native URI
     */

    destinationType?: number;
    ```




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
