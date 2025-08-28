English | [简体中文](./README-zh_CN.md) | [Homepage](https://framework.tds.qq.com/)
# ThirdParty
The ThirdParty repository is a directory that catalogs all libraries compatible with KuiklyUI.

### How to Update an Existing Library
- Locate the library's entry in the file: [KuiklyUI-Libraries.json](https://github.com/Tencent-TDS/ThirdParty/blob/main/KuiklyUI-Libraries.json)
- Update the entry with new information
- Submit a PR

## How to Add a New Library
- Add it to the end of the [KuiklyUI-Libraries.json](https://github.com/Tencent-TDS/ThirdParty/blob/main/KuiklyUI-Libraries.json) file
- Refer to the [Library Description Template](#library-description-template) to describe the library's relevant information
- Submit a PR

### Library Description Template
Please follow the format, field order, and indentation as shown below. Omit fields for unsupported platforms.

```json
{
  "githubUrl": "<GITHUB REPOSITORY URL>", 
  "examples": [
    "<THE Android Demo TO REPO>", 
    "<THE iOS Demo TO REPO>", 
    "<THE Ohos Demo TO REPO>", 
    "<THE Js Demo TO A REPO>"
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

### Template Field Descriptions
#### General Fields
- `githubUrl`
  **(string)** - The GitHub repository URL of the package
- `examples`
  **(string)** - URLs to example projects demonstrating the library's usage. Provide URLs for supported platforms and remove entries for unsupported platforms.
- `componentType`
  **(string)** - The type of library. KMP: Standard KMP component; KuiklyView: Kuikly extended View; KuiklyModule: Kuikly extended Module.

#### Supported Platform Fields
- `Android`
  **(boolean)** - The library supports running on the Android platform
- `iOS`
  **(boolean)** - The library supports running on the iOS platform
- `Ohos`
  **(boolean)** - The library supports running on the Ohos platform
- `Js`
  **(boolean)** - The library supports running on H5/mini-program platforms
- `Macos`
  **(boolean)** - The library supports running on the Macos platform
- `Linux`
  **(boolean)** - The library supports running on the Linux platform
- `Windows`
  **(boolean)** - The library supports running on the Windows platform
- `Tvos`
  **(boolean)** - The library supports running on the Tvos platform






