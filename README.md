# App Privacy Policies

应用隐私政策仓库。当前 LiveCard 文件为待审核草稿，尚未作为正式政策生效。仓库中的草稿与 GitHub Pages 上的正式政策网页是两个独立阶段。

## LiveCard

- [简体中文草稿](livecard/privacy.zh-Hans.md)
- [English draft](livecard/privacy.en.md)

生效日期仍待确定，发布前还须确认所需的开发者信息与有效联系方式、发布地区、年龄定位及正式版购买功能。请先完成审核，再移除草稿与待确认标记。

## 建议的发布方式

采用 GitHub Pages 静态页面，每个应用独立目录。LiveCard 建议入口为 `livecard/index.html`，页面提供中英文切换或链接，不引入分析脚本、第三方字体或广告。

目前尚未创建或发布该正式网页。草稿已补充 GitHub Pages 出于安全目的记录和保存访问者 IP 地址的说明，并链接 GitHub 隐私声明；最终页面仍须核对实际使用的脚本和外部资源。

完成审核后再添加静态 HTML 与 `.nojekyll`，提交、推送并确认仓库 Settings → Pages 的发布来源。是否开启 Pages 及其发布来源须由仓库负责人确认。

可能的默认地址形式为 `https://suspect-x-qc.github.io/App-Privacy/livecard/`，这只是根据仓库命名推算的候选地址，**不是已验证的公开页面**。实际地址以 Pages 部署结果为准，并须匿名打开验证。

公开页面验证通过后，把实际 HTTPS URL 写入 LiveCard 工程的 `LiveCard/Settings/PrivacyPolicy.plist` 的 `URL`，再核对 App Store Connect 的隐私政策地址。不要将本地路径、GitHub 编辑地址或尚不存在的候选地址填入应用。

## 已核对的发布步骤（2026-11-11）

1. 审核中英文内容，确定生效日期和剩余发布信息；移除草稿标记，生成无外部资源的 `livecard/index.html`，根目录添加 `.nojekyll`。
2. 将审核后的正式网页提交、推送至 `suspect-x-qc/App-Privacy` 的 `main`。仅有当前 Markdown 草稿时，不应将候选 Pages 路径填入应用。
3. 使用对该仓库拥有管理员或维护者权限的账号，在 Settings → Pages → Build and deployment 选择 **Deploy from a branch**，选择 **main** 和 **/(root)**，保存。配置此设置需要管理员或维护者权限。
4. 检查 GitHub Pages 部署成功；按设置页显示的真实地址，匿名打开 LiveCard 页面，确认中英文和联系邮箱正确。候选路径不能代替这一验证。
5. 将验证后的地址写入 LiveCard 的 PrivacyPolicy.plist，再构建并检查实际打开行为；App Store Connect 使用同一公开政策地址。

来源：[GitHub Pages 发布来源](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)；[默认地址与访问数据](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)。

提交草稿不代表 Pages 已开启，也不代表政策已生效。本次内容不更改仓库可见性或任何访问权限。
