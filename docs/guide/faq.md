# FAQ

::: tip

- <Badge text="dev" vertical="middle"/> 代表只和开发有关。默认示例站点使用的 dev 分支，所以可能会出现还未发版功能。

:::

有任何关于本主题的缺陷报告与功能建议，可以发起 [Issues](https://github.com/MaLuns/hexo-theme-async/issues)。

如果您有其他相关的想法与问题，可前往 [Discussions](https://github.com/MaLuns/hexo-theme-async/discussions)。

## 自查通用问题解决方案

检查文件或仓库命名是否错误。

检查 `Hexo` 工作目录下 `_config.yml` 中 `url` 是否设置正确。（此部分为 Hexo 初始化时自动生成）

```yaml
# If your site is put in a subdirectory
# set url as 'https://yoursite.com/child' and root as '/child/'
url: https://www.imalun.com
root: /
```

检查是否在 `_config.async.yml` 文件中进行主题配置，且已经保存。
检查是否已经执行如下几步：

- `hexo clean`：清除本地缓存
- `hexo g`：生成新的静态文件
- `hexo s`：本地查看效果（如果正常，使用 `hexo d` 重新部署）

检查是否已强制刷新本地浏览器缓存（Windows: `Ctrl + F5`，Mac: `Shift + Cmd + R`）。

检查是否为最新版本。

主题相关问题请发起 [ISSUE](https://github.com/MaLuns/hexo-theme-async/issues) ，其他讨论与展示请使用 [Discussions](https://github.com/MaLuns/hexo-theme-async/discussions)。

## 配置项不生效？
检查安装主题版本，然后查看更新日志里是否发生变更，参考文档配置说明，确保配置正确。

## About 页面不显示？
检查是否和其他插件冲突，解决方式，可以弃用配置方式，在 md 文件里编写您的 About 页面。

## 页面加载缓慢？或者页面显示不完整，无法滚动等。

如图：

![示例](https://pic.iqjty.com/2023/02/08/63e32b9b03888.png)

打开控制面板，检查插件是否加载正确加载，因为 jsdelivr、unpkg 国内可以会出现 DNS 污染等原因，导致有时候可能无法使用，可以参考[这里](https://hexo-theme-async.imalun.com/guide/config.html#%E6%8F%92%E4%BB%B6-plugins)替换 CDN 源。