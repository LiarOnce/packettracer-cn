# packettracer-cn
Cisco Packet Tracer 8.x language file for Simplified Chinese

基于官网 8.1.1 继续汉化，适用于 8.2.0 及以上，通过 OmegaT 理论上也可适用于 7.x 和 6.x

## 所需工具

 - OmegaT >= 5.7.0
 - [Okapi Filters Plugin for OmegaT](https://okapiframework.org/binaries/omegat-plugin/) >= 1.9-1.41.0 - 1.11-1.43.0   
   **不要使用 1.12-1.44.0 之后的版本，该版本使用 Java 11 构建，OmegaT 的正式版暂不支持** [更多信息](https://okapiframework.org/wiki/index.php?title=Okapi_Filters_Plugin_for_OmegaT)
 - Qt Linguist （由 Packet Tracer 附带）
 - Visual Studio Code （其余支持的代码编辑器均可）
 
 ## 编译语言文件
 
 1. **在使用本仓库之前请先安装 Okapi Filters Plugin for OmegaT 插件，否则无法识别到原文文档**
 2. 使用 OmegaT 克隆本项目，或直接下载本仓库并用 OmegaT 打开，进入项目界面后点击`项目 --> 创建译文文档`，之后点击`项目 --> 访问项目内容 --> 译文文件`即可找到生成后的 `Simplified Chinese.ts` 文件
 3. 使用 Visual Studio Code 等代码编辑器打开生成后的 `Simplified Chinese.ts` 文件，右下角语言选择 XML (默认会被识别为 TypeScript，会提示大量报错)，查找` type="unfinished"`(包含空格)，替换则不填（即删除所有查找到的结果），之后保存该文件
 4. 使用 Qt Linguist 打开处理后的文件，之后点击`保存 --> 发布`，即可在该文件所在的目录找到`Simplified Chinese.qm`文件，将文件后缀名`.qm`改为`.ptl`后即可将该语言文件应用于 Packet Tracer

## License

CC-BY
