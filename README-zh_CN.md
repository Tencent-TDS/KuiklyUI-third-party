[English](./README.md) | 简体中文 | [官网](https://kuikly.tds.qq.com/)

# ThirdParty
KuiklyUI-third-party 仓库是收录所有与 KuiklyUI 兼容的第三方库的目录

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
  "componentType": "<KMP|KuiklyView|KuiklyModule|Tools|Demo|AITools>",
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
  **(string)** - 该库的类型。KMP:标准KMP组件；KuiklyView: Kuikly扩展View；KuiklyModule：Kuikly扩展Module；Tools：开发调试工具；Demo：示例 / Demo 项目；AITools：AI 工具。

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

## 技术分享与社区共建
本仓库不再通过 JSON 文件收录技术分享文章。

- 如果你希望文章在 **Kuikly 官网** 或 **Kuikly 公众号** 发表，请添加 **Kuikly 小助手** 微信沟通（可扫下方「在线咨询」二维码）。
- 如果你希望加入 **Kuikly 核心共建群**，也请添加 **Kuikly 小助手** 微信联系。

## 欢迎关注交流
欢迎扫码下方二维码关注最新动态或咨询交流。
<p align="left">
    <div style="display: inline-block; text-align: center; margin-right: 20px;">
        <div>腾讯端服务微信公众号</div>
        <img alt="TDS" src="img/tds_qrcode.jpeg" width="200" />
    </div>
    <div style="display: inline-block; text-align: center; margin-right: 20px;">
        <div>TDS Framework 微信公众号</div>
        <img alt="TDS Framework" src="img/tds_framework_qrcode.jpeg" width="200" />
    </div>
    <div style="display: inline-block; text-align: center;">
        <div>在线咨询（Kuikly 小助手）</div>
        <img alt="在线咨询" src="img/consult_qrcode.png" width="200" />
    </div>
</p>
