# App工程化

## 前置工作

### 项目初始化
- 知识库新建项目目录，管理文档
- 开发者新建套装ID，Xcode配置
- Connect新建，打包上传
- 基于 [Flutter-scaffold](https://github.com/XZXY-AI/Flutter-scaffold) 开发

### 页面开发
- 根据 `refer/import.html` 设计图实现页面
- 优先使用现有Flutter插件，减少编码量
- 拆分组件，符合最佳实践
- 不编写测试页面

## 功能集成

### 推送通知
- **OneSignal**: [Flutter SDK 配置文档](https://documentation.onesignal.com/docs/cn/flutter-sdk-setup#%E9%9A%90%E7%A7%81%E5%92%8C%E7%94%A8%E6%88%B7%E5%90%8C%E6%84%8F)

### 支付系统
- **RevenueCat**: [官方文档](https://www.revenuecat.com/)

### 广告集成
- **Google AdMob**: [激励广告集成教程](https://codelabs.developers.google.com/codelabs/admob-ads-in-flutter?hl=zh-cn#0)

### 社交功能
- **社媒分享**: [appinio_social_share](https://pub.dev/packages/appinio_social_share)
- **应用评分**: 使用 `url_launcher` 打开外部链接
- **用户反馈**: 使用 `mailto` 协议打开系统邮箱应用

### 其他服务
- **应用更新**: 参考更新文档
- **SMTP服务**: 短信服务集成
- **iPad适配**: 在骨架中设置iPad尺寸

### 官方页面
- **官网**: [https://www.jonlantech.com/](https://www.jonlantech.com/)
- **隐私协议**: [https://www.jonlantech.com/privacy_policy](https://www.jonlantech.com/privacy_policy)
- **服务条款**: [https://www.jonlantech.com/terms_of_service](https://www.jonlantech.com/terms_of_service)

## 调试相关

### Flutter Inspector
- Flutter的可视化调试工具
- 用于可视化调试Widget树和布局

## 上架相关

### 应用图标
- 使用3倍图图标效果
- App图标不要包含透明效果（iOS会拒绝）

### 应用商店截图
- 推荐工具: [AppShots](https://www.appshots.top/editor?template=8)

## 审核相关

### 审核要点
- 可以直接回复的，回复通过审核
- 申请敏感资源弹窗内容要详细
- 必须有用户注销功能
- 适配iPad大屏
- 不要强制用户登录

### 审核问题处理
- 音频播放功能必须在用户登录后才能使用
- 应用核心功能与用户强关联
- 用户登录后才能导入链接，生成文章卡片
- 没有登录就没有卡片，也就没有音频

## 开发资源

### 插件查找
- **Flutter插件**: [FlutterGems](https://fluttergems.dev/)

### 设计资源
- **动画资源**: [LottieFiles](https://lottiefiles.com/)
- **图标矢量图**: [Flaticon](https://www.flaticon.com/)

## 常用库

### UI组件
- `modal_bottom_sheet`: 底部弹出框
- `super_tooltip`: 气泡提示
- `shimmer`: 加载骨架屏效果

### 音频相关
- `just_audio`: 音频播放器
- `just_audio_background`: 后台播放
- `audio_video_progress_bar`: 音频进度条

### 服务集成
- `onesignal_flutter`: OneSignal推送服务
- `appwrite`: Appwrite后端服务
- `appinio_social_share`: 社交媒体分享
- `flutter_launcher_icons`: 应用图标生成

## 最佳实践

1. **组件化开发**: 合理拆分组件，提高代码复用性
2. **插件优先**: 优先使用成熟的Flutter插件
3. **用户体验**: 不强制登录，提供良好的用户引导
4. **多端适配**: 考虑iPad等大屏设备的适配
5. **审核合规**: 遵循应用商店审核规范