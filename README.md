# ThirdParty
ThirdParty仓库是收录所有与 KuiklyUI 兼容的库的目录

### 如何更新一个新库
- 在文件中查找该库的入口条目 [KuiklyUI-Libraries.json](https://github.com/Tencent-TDS/ThirdParty/blob/main/KuiklyUI-Libraries.json)
- 使用新数据更新该条目描述信息
- 提交 PR。

## 如何添加一个新库
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
  "componentType": "<KMP|KuiklyView|KuiklyModule|Tools>", 
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
  **(string)** - 该软件包的 GitHub 仓库 URL
- `examples`
  **(string)** - 该库用法的示例项目 URL。对支持的平台填写其示例URL，对于不支持的平台，需删除描述。
- `componentType`
  **(string)** - 该库的类型。KMP:标准KMP组件；KuiklyView: Kuikly扩展View；KuiklyModule：Kuikly扩展Module。

#### 支持平台字段
- `Android`
  **(boolean)** - 该库支持在 Android 平台运行
- `iOS`
  **(boolean)** - 该库支持在 iOS 平台运行
- `Ohos`
  **(boolean)** - 该库支持在 Ohos 平台运行
- `Js`
  **(boolean)** - 该库支持在 H5 /小程序平台运行
- `Macos`
  **(boolean)** - 该库支持在 Macos 平台运行
- `Linux`
  **(boolean)** - 该库支持在 Linux 平台运行
- `Windows`
  **(boolean)** - 该库支持在 Windows 平台运行
- `Tvos`
  **(boolean)** - 该库支持在 Tvos 平台运行






