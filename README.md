# Полезные консольные команды
**Перезапуск приложения**:
```
require(["ServiceHelper"], (ServiceHelper) => {
    ServiceHelper.callCoreService({serviceName:"AppInstallerService", methodName:(BPMSoft.appFramework == 'NETCOREAPP' ? "RestartApp" : "UnloadAppDomain")}, function(result){console.log(result)}, {}); //UnloadAppDomain //ClearRedisDb
});


```

**Очистка Redis**:
```
require(["ServiceHelper"], (ServiceHelper) => {
    ServiceHelper.callCoreService({serviceName:"AppInstallerService", methodName:"ClearRedisDb"}, function(result){console.log(result)}, {}); //UnloadAppDomain //ClearRedisDb
});
```
