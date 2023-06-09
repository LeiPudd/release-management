# Version Info
openEuler 23.03 是基于6.1内核的创新版本（参见[版本生命周期](https://www.openeuler.org/zh/other/lifecycle/)），面向服务器、云、边缘计算和嵌入式场景，提供更多新特性和功能，给开发者和用户带来全新的体验，服务更多的领域和更多的用户。<br>


# Release Plan

| Stage  name          | Begin time | End time   | Days | Note                                      |
| -------------------- | ---------- | ---------- | ---- | ----------------------------------------- |
| Collect key features | 2022/12/01  | 2023/1/15 | 46   | 收集23.03版本关键特性（各SIG自行录入release-plan）   |
| Develop | 2023/1/4  | 2023/2/20 | 46   | 特性完成开发和自验证，代码提交合入23.03   |
| 内核升级 | 2023/1/4  | 2023/1/16 | 12   | master主线升级内核到6.1   |
| BaseOS构建 | 2023/1/16  | 2023/1/31 | 15   | Master主线BaseOS构建，基础包能用   |
| BaseOS测试 | 2023/2/1  | 2023/2/3 | 3   | 内核升级后BaseOS可用   |
| 分支全量Build | 2023/2/6  | 2023/2/10 | 4   | 从master拉23.03分支，完成分支全量构建，基础包升级完毕   |
| Alpha | 2023/2/13  | 2023/2/22 | 4   | 软件包升级完成，首版本发布   |
| Test round 1 | 2023/2/23  | 2023/3/1 | 5   | 版本启动测试，内核冻结   |
| Test round 2 | 2023/3/2  | 2023/3/7 | 5   |   |
| Test round 3 | 2023/3/8  | 2023/3/12 | 5   | 特性合入冻结，不再接纳新特性代码合入   |
| Test round 4 | 2023/3/21  | 2023/3/24 | 4   |    |
| Test round 5 | 2023/3/27  | 2023/3/29 | 3   |    |
| Release | 2023/3/30  | 2023/3/30 | 1   |    |



# 代码合入说明
创新版本代码继承master分支 <br>
// 新特性代码请及时合入版本&自验证，跟随整体计划赶在第一轮转测试


# Feature list
状态说明：Discussion(方案讨论，需求未接受)、 Developing(开发中)、 Testing(测试中)、 Accepted(已验收) <br>
发布方式：ISO、EPOL、oepkgs、独立发布等

|no|feature|status|sig|owner|发布方式|涉及软件包列表|
|:----|:---|:---|:--|:----|:----|:----|
|1|[【openEuler 23.03】新增高性能服务网格数据面Kmesh](https://gitee.com/openeuler/release-management/issues/I65S7M?from=project-issue)|Accepted|sig-high-performance-network|@MrRlu|ISO|kmesh|
|2|[【openEuler 23.03】新增内核配置项错误值检查工具kconfigDetector](https://gitee.com/openeuler/release-management/issues/I69YOZ?from=project-issue)|Accepted|sig-kernel|@sunying2022|EPOL|kconfigDetector|
|3|[【openEuler 23.03】支持树莓派](https://gitee.com/openeuler/release-management/issues/I6AACH)|Accepted|sig-RaspberryPi|[@woqidaideshi](https://gitee.com/woqidaideshi)|EPOL|raspberrypi-firmware,raspberrypi-bluetooth,raspi-config,pigpio,raspberrypi-userland,raspberrypi-eeprom|
|4|[【openEuler 23.03】iSulad支持镜像RO数据管理目录拆分](https://gitee.com/openeuler/release-management/issues/I6E2SI)|Accepted|sig-CloudNative|[@driedyellowpeach](https://gitee.com/driedyellowpeach)| ISO |iSulad|
|5|[【openEuler 23.03】GCC编译器插件框架支持LTO复杂优化，实现插件IR覆盖Gimple 80%的功能](https://e.gitee.com/open_euler/issues/table?issue=I6CK4F)|Accepted|Compiler|@wangding|ISO|GCC|
|6|[【openEuler 23.03】openEuler 23.03 创新版本选择 6.1 内核](https://gitee.com/openeuler/kernel/issues/I6834I)|Accepted|Kernel |@zhengzengkai|ISO|Kernel|
|7|[【openEuler 23.03】支持embedded版本](https://gitee.com/openeuler/release-management/issues/I6DS1J?from=project-issue)|Accepted|sig-embedded|@fanglinxu|独立发布|Embedded|
|8|[【openEuler 23.03】NFS客户端支持多路径](https://gitee.com/openeuler/kernel/issues/I6CR7Z)|Accepted|Kernel |@jiangzhongbing|EPOL|Kernel|
|9|[【openEuler 23.03】新增openGemini时序数据库](https://gitee.com/openeuler/release-management/issues/I6EQV3)|Accepted|DB|@openGemini|EPOL|Kernel|
|10|[【openEuler 23.03】secGear支持安全通道](https://gitee.com/openeuler/release-management/issues/I6EZTD?from=project-issue)|Accepted|sig-confidential-computing|@houmingyong|ISO|secGear|


# 需求/特性反馈基本流程 <br />
1、开发者/sig在本贴的表格中填写要合入23.03的需求/特性，并同时填写需求issue及链接 （请在收集截止时间前提交）      <br>
2、申请在版本release management sig例会上评审需求 （owner或者SIG maintainer参会）
<br><br>
