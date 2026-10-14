English | [简体中文](./README-zh_CN.md) | [Homepage](https://kuikly.tds.qq.com/)
# KuiklyUI-third-party
The KuiklyUI-third-party repository is a directory of third-party libraries compatible with KuiklyUI.

## KuiklyUI component and tool libraries collection
### How to Update an Existing Library
- Locate the library's entry in the file: [KuiklyUI-Libraries.json](https://github.com/Tencent-TDS/ThirdParty/blob/main/KuiklyUI-Libraries.json)
- Update the entry with new information
- Submit a PR

### How to Add a New Library
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

### Template Field Descriptions
#### General Fields
- `githubUrl`
  **(string)** - The GitHub repository URL of the package.
- `examples`
  **(string)** - URLs to example projects demonstrating the library's usage. Provide URLs for supported platforms and remove entries for unsupported platforms.
- `componentDescription`
  **(string)** - The short description of this repository.
- `developer`
  **(string)** - The developer of this Component.
- `componentType`
  **(string)** - The type of library. KMP: Standard KMP component; KuiklyView: Kuikly extended View; KuiklyModule: Kuikly extended Module; Tools: developer tools; Demo: sample / demo projects; AITools: AI tooling.

#### Supported Platform Fields
- `Android`
  **(boolean)** - The library supports running on the Android platform.
- `iOS`
  **(boolean)** - The library supports running on the iOS platform.
- `Ohos`
  **(boolean)** - The library supports running on the Ohos platform.
- `Js`
  **(boolean)** - The library supports running on H5/mini-program platforms.
- `Macos`
  **(boolean)** - The library supports running on the Macos platform.
- `Linux`
  **(boolean)** - The library supports running on the Linux platform.
- `Windows`
  **(boolean)** - The library supports running on the Windows platform.
- `Tvos`
  **(boolean)** - The library supports running on the Tvos platform.
#### Supported Dynamic Feature Fields
- `sDynamic`
  **(boolean)** - Does the library support direct referencing in dynamic mode? It can be determined from the following three aspects:
  - Supports JavaScript target outputs
  - Does not rely on browser platform interfaces
  - Does not rely on coroutines, or the runtime logic does not involve multithreading

## Technology sharing and community
This repository no longer collects technology sharing articles via a JSON file.

- If you would like your article published on the **Kuikly website** or the **Kuikly WeChat official account**, please add the **Kuikly Assistant** on WeChat (scan the **Online Support** QR code below).
- If you would like to join the **Kuikly core contributor group**, please also contact us by adding the **Kuikly Assistant** on WeChat.

## Stay Connected
Scan the QR codes below to follow our latest updates or contact us for inquiries.
<p align="left">
    <div style="display: inline-block; text-align: center; margin-right: 20px;">
        <div>TDS WeChat Official Account</div>
        <img alt="TDS" src="img/tds_qrcode.jpeg" width="200" />
    </div>
    <div style="display: inline-block; text-align: center; margin-right: 20px;">
        <div>TDS Framework WeChat Official Account</div>
        <img alt="TDS Framework WeChat Official Account" src="img/tds_framework_qrcode.jpeg" width="200" />
    </div>
    <div style="display: inline-block; text-align: center;">
        <div>Online Support (Kuikly Assistant)</div>
        <img alt="Online Consult" src="img/consult_qrcode.png" width="200" />
    </div>
</p>
