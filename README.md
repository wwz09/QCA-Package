# LUCI-APP 插件使用指南

## 项目概述

本项目是一个OpenWrt软件包集合，包含了大量实用的LUCI应用插件，为OpenWrt路由器提供丰富的功能扩展。这些插件涵盖了网络工具、存储管理、媒体服务、系统工具等多个领域，可以帮助用户更方便地管理和使用OpenWrt路由器。

## 插件列表

| 插件名称 | 功能描述 |
|---------|--------|
| luci-app-adguardhome | AdGuard Home广告拦截器 |
| luci-app-advanced | 高级系统设置 |
| luci-app-advancedplus | 高级系统设置增强版 |
| luci-app-airconnect | AirPlay和DLNA音频桥接 |
| luci-app-aliyundrive-webdav | 阿里云盘WebDAV服务 |
| luci-app-amlogic | Amlogic芯片设备支持 |
| luci-app-argon-config | Argon主题配置 |
| luci-app-aria2 | Aria2下载工具 |
| luci-app-aurora-config | Aurora主题配置 |
| luci-app-bandix | 网络带宽管理 |
| luci-app-clouddrive2 | 云盘管理工具 |
| luci-app-control-timewol | 定时唤醒和关机 |
| luci-app-control-webrestriction | 网页访问限制 |
| luci-app-control-weburl | 网址过滤 |
| luci-app-cpufreq | CPU频率调节 |
| luci-app-ddns | 动态DNS客户端 |
| luci-app-ddns-go | DDNS-Go动态DNS客户端 |
| luci-app-ddnsto | DDNSTO内网穿透 |
| luci-app-dnsfilter | DNS过滤 |
| luci-app-easymesh | 简易mesh网络 |
| luci-app-easytier | 网络加速工具 |
| luci-app-eqos | 网络流量均衡 |
| luci-app-fastnet | 网络加速 |
| luci-app-fchomo | 网络分流工具 |
| luci-app-fileassistant | 文件管理助手 |
| luci-app-filebrowser | 文件浏览器 |
| luci-app-filemanager | 文件管理器 |
| luci-app-floatip | 浮动IP管理 |
| luci-app-gowebdav | GoWebDAV服务 |
| luci-app-guest-wifi | 访客WiFi设置 |
| luci-app-ikoolproxy | KoolProxyR广告过滤 |
| luci-app-ipsec-server | IPsec VPN服务器 |
| luci-app-istoreenhance | iStore增强 |
| luci-app-istorex | iStore应用商店 |
| luci-app-kai | KAI网络工具 |
| luci-app-kodexplorer | KOD资源管理器 |
| luci-app-koolproxyR | KoolProxyR广告过滤 |
| luci-app-linkease | 链路聚合 |
| luci-app-lucky | Lucky网络工具 |
| luci-app-mentohust | MentoHUST校园网认证 |
| luci-app-momo | Momo网络工具 |
| luci-app-mosdns | MOSDNS域名解析 |
| luci-app-nekoclash | Clash网络工具 |
| luci-app-netspeedtest | 网络速度测试 |
| luci-app-nikki | Nikki网络工具 |
| luci-app-oaf | 应用过滤 |
| luci-app-onliner | 在线用户监控 |
| luci-app-openclash | OpenClash网络工具 |
| luci-app-openlist2 | 开源列表管理 |
| luci-app-openvpn-client | OpenVPN客户端 |
| luci-app-openvpn-server | OpenVPN服务器 |
| luci-app-ota | 在线更新 |
| luci-app-partexp | 分区扩展 |
| luci-app-poweroff | 关机功能 |
| luci-app-pppoe-relay | PPPoE中继 |
| luci-app-pppoe-server | PPPoE服务器 |
| luci-app-pptp-server | PPTP服务器 |
| luci-app-qbittorrent | qBittorrent下载工具 |
| luci-app-qosmate | QoS网络质量控制 |
| luci-app-quickfile | 快速文件访问 |
| luci-app-quickstart | 快速设置向导 |
| luci-app-ramfree | 内存释放 |
| luci-app-rtp2httpd | RTP转HTTP服务 |
| luci-app-smartdns | SmartDNS智能DNS |
| luci-app-socat | Socat网络工具 |
| luci-app-softethervpn | SoftEther VPN |
| luci-app-ssr-mudb-server | SSR服务器管理 |
| luci-app-store | 应用商店 |
| luci-app-syncthing | Syncthing文件同步 |
| luci-app-timecontrol | 时间控制 |
| luci-app-unblockneteasemusic | 网易云音乐解锁 |
| luci-app-unishare | 统一共享 |
| luci-app-usb-printer | USB打印机支持 |
| luci-app-verysync | VerySync文件同步 |
| luci-app-wechatpush | 微信推送 |
| luci-app-wolplus | 网络唤醒增强 |
| luci-app-wrtbwmon | 带宽监控 |

## 详细插件说明

### 1. luci-app-adguardhome

#### 功能介绍
AdGuard Home是一个网络级广告和跟踪器拦截器，通过DNS过滤技术，可以在整个网络层面阻止广告、跟踪器和恶意网站。

#### 安装步骤
1. 在OpenWrt管理界面中，进入「系统」→「软件包」
2. 点击「更新列表」按钮刷新软件包列表
3. 搜索并安装 `luci-app-adguardhome` 和 `adguardhome` 包
4. 安装完成后，在「服务」菜单中会出现「AdGuard Home」选项

#### 配置方法
1. 进入「服务」→「AdGuard Home」
2. 点击「打开Web界面」按钮进入AdGuard Home配置页面
3. 按照向导完成初始配置
4. 在「设置」→「DNS设置」中配置上游DNS服务器
5. 在「过滤规则」中添加所需的过滤列表

#### 使用指南
- **DNS查询日志**：查看所有DNS查询记录
- **统计信息**：查看广告拦截统计
- **客户端设置**：为不同客户端设置不同的过滤规则
- **更新过滤列表**：定期更新过滤规则以保持最佳效果

#### 常见问题
- **无法启动**：检查端口是否被占用，默认使用53端口
- **网络变慢**：调整上游DNS服务器，选择响应速度快的服务器
- **设备无法解析DNS**：检查防火墙设置，确保DNS端口未被阻止

### 2. luci-app-aria2

#### 功能介绍
Aria2是一个轻量级的多协议下载工具，支持HTTP、HTTPS、FTP、BitTorrent等协议，具有多线程下载能力。

#### 安装步骤
1. 在OpenWrt管理界面中，进入「系统」→「软件包」
2. 搜索并安装 `luci-app-aria2` 和 `aria2` 包
3. 安装完成后，在「服务」菜单中会出现「Aria2」选项

#### 配置方法
1. 进入「服务」→「Aria2」
2. 配置基本设置：
   - 启用Aria2服务
   - 设置下载目录
   - 配置RPC密钥
3. 高级设置：
   - 调整线程数
   - 设置连接数
   - 配置BT相关参数

#### 使用指南
- **Web界面**：使用AriaNg等Web界面管理下载任务
- **添加下载**：支持URL、磁力链接、种子文件
- **任务管理**：暂停、继续、删除任务
- **速度限制**：设置下载和上传速度限制

#### 常见问题
- **RPC连接失败**：检查RPC端口和密钥设置
- **下载速度慢**：调整线程数和连接数
- **BT下载无速度**：检查DHT和PEX设置

### 3. luci-app-openclash

#### 功能介绍
OpenClash是一个基于Clash的网络代理工具，支持多种代理协议，提供丰富的规则和策略管理。

#### 安装步骤
1. 在OpenWrt管理界面中，进入「系统」→「软件包」
2. 搜索并安装 `luci-app-openclash` 包
3. 安装完成后，在「服务」菜单中会出现「OpenClash」选项

#### 配置方法
1. 进入「服务」→「OpenClash」
2. 下载并配置Clash核心
3. 上传或订阅配置文件
4. 配置规则和策略
5. 启用服务

#### 使用指南
- **配置管理**：管理多个配置文件
- **规则管理**：自定义规则和策略
- **节点管理**：添加和测试代理节点
- **状态监控**：查看代理状态和流量统计

#### 常见问题
- **核心下载失败**：检查网络连接，手动下载核心文件
- **无法启动**：检查配置文件格式是否正确
- **流量不经过代理**：检查路由规则设置

### 4. luci-app-qbittorrent

#### 功能介绍
qBittorrent是一个功能强大的BitTorrent客户端，支持种子管理、RSS订阅等功能。

#### 安装步骤
1. 在OpenWrt管理界面中，进入「系统」→「软件包」
2. 搜索并安装 `luci-app-qbittorrent` 和 `qbittorrent` 包
3. 安装完成后，在「服务」菜单中会出现「qBittorrent」选项

#### 配置方法
1. 进入「服务」→「qBittorrent」
2. 配置基本设置：
   - 启用服务
   - 设置下载目录
   - 配置Web界面端口和登录信息
3. 高级设置：
   - 调整连接数
   - 设置种子分享率
   - 配置RSS订阅

#### 使用指南
- **Web界面**：通过浏览器访问Web界面管理下载任务
- **种子管理**：添加、删除、暂停种子
- **RSS订阅**：自动下载RSS源中的种子
- **速度限制**：设置全局或单个种子的速度限制

#### 常见问题
- **Web界面无法访问**：检查端口设置和防火墙规则
- **下载速度慢**：调整连接数和种子设置
- **内存占用高**：限制同时下载的种子数量

### 5. luci-app-mosdns

#### 功能介绍
MOSDNS是一个基于Go语言开发的DNS服务器，支持DNS分流、缓存、EDNS等功能。

#### 安装步骤
1. 在OpenWrt管理界面中，进入「系统」→「软件包」
2. 搜索并安装 `luci-app-mosdns` 和 `mosdns` 包
3. 安装完成后，在「服务」菜单中会出现「MOSDNS」选项

#### 配置方法
1. 进入「服务」→「MOSDNS」
2. 配置基本设置：
   - 启用服务
   - 设置监听端口
   - 配置上游DNS服务器
3. 配置规则：
   - 设置域名分流规则
   - 配置缓存设置
   - 调整性能参数

#### 使用指南
- **规则管理**：添加和管理域名规则
- **状态监控**：查看DNS查询统计
- **日志查看**：检查DNS查询日志
- **性能调优**：根据网络环境调整配置

#### 常见问题
- **DNS解析失败**：检查上游DNS服务器设置
- **网络变慢**：调整缓存设置和规则匹配
- **服务无法启动**：检查端口是否被占用

## 安装方法

### 方法一：通过OpenWrt软件包管理
1. 登录OpenWrt管理界面
2. 进入「系统」→「软件包」
3. 点击「更新列表」按钮刷新软件包列表
4. 在搜索框中输入插件名称，如「luci-app-adguardhome」
5. 点击「安装」按钮安装插件
6. 安装完成后，在「服务」菜单中找到对应的插件

### 方法二：通过命令行安装
1. 登录路由器的SSH终端
2. 执行以下命令更新软件包列表：
   ```bash
   opkg update
   ```
3. 执行以下命令安装插件：
   ```bash
   opkg install luci-app-插件名称
   ```
   例如：
   ```bash
   opkg install luci-app-adguardhome
   ```

### 方法三：通过编译安装
1. 克隆本仓库到本地
2. 将仓库添加到OpenWrt编译环境
3. 在编译配置中选择需要的插件
4. 编译并刷入固件

## 配置建议

1. **系统资源管理**
   - 对于内存较小的路由器，建议只安装必要的插件
   - 定期清理内存，可使用luci-app-ramfree插件
   - 监控系统负载，避免同时运行过多插件

2. **网络优化**
   - 配置合理的DNS服务器，可使用luci-app-smartdns或luci-app-mosdns
   - 根据网络环境调整QoS设置，使用luci-app-qosmate
   - 监控带宽使用情况，使用luci-app-wrtbwmon

3. **安全设置**
   - 定期更新插件和系统
   - 为Web界面设置强密码
   - 配置防火墙规则，限制外部访问

## 常见问题解答

### Q: 安装插件后在菜单中找不到
**A:** 可能是因为插件依赖未完全安装，尝试安装插件的依赖包，或重启路由器后再查看。

### Q: 插件服务无法启动
**A:** 检查插件配置是否正确，端口是否被占用，以及相关依赖是否安装。查看系统日志获取详细错误信息。

### Q: 插件导致系统变慢
**A:** 检查插件是否占用过多系统资源，考虑关闭不必要的插件，或升级路由器硬件。

### Q: 如何卸载插件
**A:** 在「系统」→「软件包」中找到已安装的插件，点击「移除」按钮进行卸载。

### Q: 插件配置丢失
**A:** 可能是因为系统升级或重启导致，建议定期备份配置，或使用luci-app-store中的备份功能。

## 总结

本项目提供了丰富的LUCI应用插件，涵盖了网络管理、存储管理、媒体服务等多个领域。通过本指南，您可以了解如何安装、配置和使用这些插件，以充分发挥OpenWrt路由器的功能。

如果您在使用过程中遇到问题，可以参考本指南的常见问题解答，或在相关社区寻求帮助。

## 免责声明

本指南仅供参考，具体插件功能和配置可能因版本不同而有所差异。使用插件时请遵守相关法律法规，合理使用网络资源。