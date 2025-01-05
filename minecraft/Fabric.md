# Fabric接口调研

## 查询

`https://meta.fabricmc.net/` 接口前缀与接口内容总结，支持GET，可直接打开，

- `/v1/versions`，获取所有版本信息，信息过多，一般不用

  ```
  {
  	"game":[
  		{
              "version": "1.21.4",
              "stable": true
          }
  	],
  	"mappings":[
  		{
              "gameVersion": "1.21.4",
              "separator": "+build.",
              "build": 2,
              "maven": "net.fabricmc:yarn:1.21.4+build.2",
              "version": "1.21.4+build.2",
              "stable": true
          }
  	],
  	"intermediary":[
  		{
              "maven": "net.fabricmc:intermediary:1.21.4",
              "version": "1.21.4",
              "stable": true
          }
  	],
  	"loader":[
  		{
              "separator": ".",
              "build": 9,
              "maven": "net.fabricmc:fabric-loader:0.16.9",
              "version": "0.16.9",
              "stable": true
          }
  	],
  	"installer":[
  		{
              "url": "https://maven.fabricmc.net/net/fabricmc/fabric-installer/1.0.1/fabric-installer-1.0.1.jar",
              "maven": "net.fabricmc:fabric-installer:1.0.1",
              "version": "1.0.1",
              "stable": true
          }
  	]
  }
  ```



- `/v1/versions/game/:game_version`，查询对应版本是否存在

  ```
  [
      {
          "version": "1.20.1",
          "stable": true
      }
  ]
  ```



- `/v1/versions/loader/:game_version`，查询对应版本的所有fabric loader版本，但没有下载链接，后面还可以再加loader的版本从而获得loader的更详细信息

  ```
  [
      {
          "loader": {
              "separator": ".",
              "build": 9,
              "maven": "net.fabricmc:fabric-loader:0.16.9",
              "version": "0.16.9",
              "stable": true
          },
          "mappings": {
              "gameVersion": "1.20.1",
              "separator": "+build.",
              "build": 10,
              "maven": "net.fabricmc:yarn:1.20.1+build.10",
              "version": "1.20.1+build.10",
              "stable": false
          }
      }
  ]
  ```

  

## 下载

- Fabric Loader下载：

  ```
  f"https://maven.fabricmc.net/net/fabricmc/fabric-loader/{版本号}/fabric-loader-{版本号}.jar"
  ```

  

- 配置文件下载：

  ```
  https://meta.fabricmc.net/v2/versions/loader/:game_version/:loader_version/profile/json
  ```

  