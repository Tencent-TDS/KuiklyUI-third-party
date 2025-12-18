[English](./README.md) | 简体中文 | [官网](https://framework.tds.qq.com/)

# ThirdParty
KuiklyUI-third-party 仓库是收录所有与 KuiklyUI 相关的技术分享和 兼容的库的目录

## KuiklyUI 组件工具库收集
### 如何更新一个新库
- 在文件中查找该库的入口条目：[KuiklyUI-Libraries.json](https://github.com/Tencent-TDS/ThirdParty/blob/main/KuiklyUI-Libraries.json)
- 使用新数据更新该条目描述信息
- 提交 PR。

### 如何添加一个新库
- 将其添加在 [KuiklyUI-Libraries.json](https://github.com/Tencent-TDS/ThirdParty/blob/main/KuiklyUI-Libraries.json)文件末尾
- 参考[库信息描述模板](#新库的描述模板)，描述该库的相关信息
- 提交 PR

### 新库的描述模板
请遵循如下格式、字段顺序和缩进规范，跳过所有不支持平台的字段。
```json
{
  "githubUrl": "<GITHUB REPOSITORY URL>", 
  "examples": [
    "<THE Android Demo TO REPO>", 
    "<THE iOS Demo TO A SNACK>", 
    "<THE Ohos Demo TO A SNACK>", 
    "<THE Js Demo TO A SNACK>"
  ], 
  "componentName": "<Your Component Name>",
  "componentDescription": "<Your Component Description>",  
  "componentType": "<KMP|KuiklyView|KuiklyModule|Tools>",
  "developer": "<Developer of this Component>",  
  "Android": false, 
  "iOS": false, 
  "Ohos": false, 
  "Js": false, 
  "Macos": false, 
  "Linux": false, 
  "Windows": false, 
  "Tvos": false
}
```

### 模板字段描述
#### 通用字段
- `githubUrl`
  **(string)** - 该软件包的 GitHub 仓库 URL。
- `examples`
  **(string)** - 该库用法的示例项目 URL。对支持的平台填写其示例URL，对于不支持的平台，需删除描述。
- `componentDescription`
  **(string)** - 该库的简短描述。
- `developer`
  **(string)** - 组件开发者。
- `componentType`
  **(string)** - 该库的类型。KMP:标准KMP组件；KuiklyView: Kuikly扩展View；KuiklyModule：Kuikly扩展Module。

#### 支持平台字段
- `Android`
  **(boolean)** - 该库支持在 Android 平台运行。
- `iOS`
  **(boolean)** - 该库支持在 iOS 平台运行。
- `Ohos`
  **(boolean)** - 该库支持在 Ohos 平台运行。
- `Js`
  **(boolean)** - 该库支持在 H5 /小程序平台运行。
- `Macos`
  **(boolean)** - 该库支持在 Macos 平台运行。
- `Linux`
  **(boolean)** - 该库支持在 Linux 平台运行。
- `Windows`
  **(boolean)** - 该库支持在 Windows 平台运行。
- `Tvos`
  **(boolean)** - 该库支持在 Tvos 平台运行。
#### 支持动态化能力字段
- `sDynamic`
  **(boolean)** - 该库是否支持在动态化模式下直接引用。可以从以下三个方面判断：
  - 支持js目标产物
  - 不依赖浏览器平台接口
  - 未依赖协程或运行时逻辑不涉及多线程

## KuiklyUI 技术分享收集
### 如何增加/更新一个分享
- 在文件中查找该库的入口条目：[KuiklyUI-TechSharing.json](https://github.com/Tencent-TDS/ThirdParty/blob/main/KuiklyUI-TechSharing.json)
- 使用新数据更新该条目描述信息
- 提交 PR。

### 分享的描述模板
请遵循如下格式、字段顺序和缩进规范，跳过所有不支持平台的字段。
```json
{
  "articleUrl": "<Article URL>",
  "articleTitle": "<Your Article Title>",
  "appName": "<Your App Name>",
  "author": "<Developer of This Component>",
  "date": "<Publication Time of This Article>"
}
```
### 模板字段描述
- `articleUrl`
  **(string)** - 技术分享文章链接。
- `articleTitle`
  **(string)** - 技术分享文章标题。
- `appName`
  **(string)** - （可选）所属业务名称。
- `author`
  **(string)** - （可选）技术分享作者，可以是GithubID。
- `date`
  **(string)** - 技术分享发表时间。
