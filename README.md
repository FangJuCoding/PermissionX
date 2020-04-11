# PermissionX

PermissionX是一个用于简化Android运行时权限用法的开源库

添加如下配置将PermissionX引入到你的项目中：
```groovy
implementation 'com.permissionx.fangjucoding:permissionx:1.0.1'
```

然后就可以使用如下语法结构来申请运行时权限了：

```kotlin
PermissionX.request(this, Manifest.permission.CALL_PHONE) { allGranted, deniedList ->
    if (allGranted) {
        //TODO 
    } else {
        //TODO 
    }
}
```