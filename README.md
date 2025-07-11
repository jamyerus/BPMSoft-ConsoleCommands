# Полезные консольные команды
**Перезапуск приложения** (работает только на .net Framework версии:
```
require(["ServiceHelper"], (ServiceHelper) => {
    ServiceHelper.callCoreService({serviceName:"AppInstallerService", methodName:"UnloadAppDomain"}, function(result){console.log(result)}, {}); //UnloadAppDomain //ClearRedisDb
});
```

**Очистка Redis**:
```
require(["ServiceHelper"], (ServiceHelper) => {
    ServiceHelper.callCoreService({serviceName:"AppInstallerService", methodName:"ClearRedisDb"}, function(result){console.log(result)}, {}); //UnloadAppDomain //ClearRedisDb
});
```
