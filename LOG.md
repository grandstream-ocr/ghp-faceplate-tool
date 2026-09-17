# 修改日志

本文件记录项目每次提交的主要改动。

## [2026-09-17] 相关修改

- 1.Fixed [GHP6XX-1684] GHP6XX_FaceplateTool_1.0.1.1:The icon text display area needs to avoid overlapping
- 2.Fixed [GHP6XX-1686] GHP6XX_FaceplateTool_1.0.1.1:The color of the room and number should be the same
- 3.Fixed [GHP6XX-1687] GHP6XX_FaceplateTool_1.0.1.1:The room control displays an exception in the preview image
- 4.Fixed [GHP6XX-1688] GHP6XX_FaceplateTool_1.0.1.1:The number of 61x pages is always reset

## [2026-09-14] 相关修改

- 1.修复[GHP6XX-1688] GHP6XX_FaceplateTool_1.0.1.1:The number of 61x pages is always reset
- 2.设置网站标题为 GHP Faceplate Tool

## [2026-09-11] 相关修改

- 1.修复卡纸模式下手动输入房间号后生成 PDF 时，错误提示房间号异常的问题。
- 2.修复卡纸模式刷新后，房间号工具栏错误显示为丝印模式样式的问题；根据当前模式正确初始化工具栏，避免默认创建丝印模式样式。
- 3.处理导入客户配置并填写房间号后，PDF 仅生成规格页、镭雕图片未按房间号生成的问题。跨模式导入配置文件时，自动切换至配置文件对应模式。
- 4.处理删除房间号后数量同步清空、再次生成 PDF 提示必填项的问题。调整 updateQuantity()，仅在房间号非空且格式合法时更新数量，否则保留原值。
- 5.优化 Logo PMS 必填项提示，在不改变现有布局的情况下强化必填标识和校验提示。
- 6.镜片定制网站页面增加版权和版本标识
- 7.增加版本管理文件 `VERSION.md`
- 8.相关Bug修复：
  - [GHP6XX-1615](https://internal.jira.grandstream.com/browse/GHP6XX-1615)  GHP6XX_FaceplateTool_20260901:Switching pages after editing and saving resulted in lost edits
  - [GHP6XX-1620](https://internal.jira.grandstream.com/browse/GHP6XX-1620)  GHP6XX_FaceplateTool_20260902:Red color still exists when generating black and white laser engraving images
  - [GHP6XX-1627](https://internal.jira.grandstream.com/browse/GHP6XX-1627)  GHP6XX_FaceplateTool_20260901:The page was reset after generating the laser engraving image
  - [GHP6XX-1634](https://internal.jira.grandstream.com/browse/GHP6XX-1634)  GHP6XX_FaceplateTool_20260902:Suggest adding a prompt for incorrect room numbers
  - [GHP6XX-1635](https://internal.jira.grandstream.com/browse/GHP6XX-1635)  GHP6XX_FaceplateTool_20260902:The laser engraving generated will continue to load after inserting a Room control
- 9.设置网站标题为 GHP faceplate tool

## [2026-09-07] 相关修改

- 1.去除无用的css和js文件。


## [2026-09-02] 相关修改

- 1.添加 `LOG.md`，用于维护提交修改记录。
- 2.修复删除房间号后镭雕下载卡死问题。
- 3.修复镭雕打印紧急服务图片显示黑色问题分析
- 4.丝印定制模式下导出卡纸模式配置文件，无法生成PDF；切换图标颜色后，导出的镭雕图标颜色不匹配问题。
- 5.[GHP6XX-1618] GHP6XXPro_FaceplateTool_20260902:PDF preview page cannot pop up normally
- 6.修正切换模型后图标被保留问题：按照“切换到目标型号即恢复该型号默认配置”规则处理。


## [2026-09-01] 初始化仓库

- 1.创建项目 Git 仓库，添加初始项目代码。
- 2.相关问题修复：
  - （1）Fixed [GHP6XX-1567] [EMEA][GHP6xx][Bug] Button becomes misaligned after removing its label and icon
  - （2）[GHP6XX-1605] 修复GHP621W 卡纸房号因加粗标签无法识别及同值文本误替换的问题。
  - （3）修复切换到 GHP620(W) 后删除图标，整机效果预览时仍显示该图标问题。
  - （4）修复切换话机型号后，部分图标会显示为黑色问题。
  - （5）修复GHP621 卡纸模式，上传客户配置后，PDF打印预览只显示一页不问题。
  - （6）修复GHP621 客户卡纸定制模式输入1001号码，pdf打印还是001问题。


