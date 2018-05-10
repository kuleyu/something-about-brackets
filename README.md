# something-about-brackets

- config.json   (the config of brackets. Just changed the value of the key[extension_registry] as `./registry.json`)
- registry.json  (a file from `https://s3.amazonaws.com/extend.brackets/registry.json`)

本项目旨在解决国内网络环境下 Brackets 扩展管理加载时间慢 或者 “无法连接扩展仓库”的问题。原理很简单：直接将扩展仓库【extension_registry】源文件【registry.json】放到了本地。


## 配置方法

  1. 下载本仓库的两个文件：`config.json` 和 `registry.json`；
  2. 找到你的 Brackets 安装路径并进入到 `www` 文件夹，如 `C:\Program Files (x86)\Brackets\www`；
  3. 将以上两个文件拖放到 `www` 文件夹下即可（`registry.json`为新增的，`config.json`替换原来的`config.json`）。



## `registry.json` 

初始日期： 2018-05-11
更新日期： 2018-05-11


> 说明：由于将 `registry.json` 存放到了本地，也就意味着 扩展仓库内容 无法获得及时更新（包括不会提示扩展升级、不会增加新的扩展。当然这都是相对与 `registry.json` 文件的更新日期而言）。其实这点影响并不大，因为 99% 以上的扩展信息都已经包含在了这个 `registry.json` 文件中。但为了保证扩展仓库的新鲜度，本项目会尽量每个 1~2 周跟新 `registry.json`文件，以供需要的人定期下载。

## 后期打算

后期会考虑将 `registry.json` 文件申请添加到 CDN 加速服务中，并定期维护更新，这样就不需多次手动下载更新了。
