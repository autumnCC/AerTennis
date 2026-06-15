# AerTennis（空气网球）

> 趣味体感空气网球，随时随地挥拍对战。
> 手握 iPhone 模拟网球挥拍动作，自动识别正手、反手、发球并记录球速。

## 中文说明

### 核心功能
- **挥拍检测**：800Hz 高频采样，EMA 滤波，自动识别网球挥拍动作
- **动作识别**：基于真实网球生物力学，精准识别正手、反手、发球
- **球速计算**：根据加速度峰值和角位移幅度推算击球速度（30~220 km/h）
- **音效反馈**：自定义挥拍击球音效 + 触觉震动
- **击球历史**：SwiftData 持久化，支持每日统计和 7 天趋势图
- **双语言**：界面文字跟随系统语言（中文/英文）

### 挥拍动作
- **正手 (Forehand)**：手臂从右侧向前左方挥动
- **反手 (Backhand)**：手臂从左侧向前右方挥动  
- **发球 (Serve)**：过顶鞭打动作，加速度最大



### 技术要点
- **传感器**：CoreMotion DeviceMotion @ 800Hz
- **滤波**：EMA 低通滤波 (α=0.12)
- **校准**：启动时 200 帧陀螺仪漂移校准
- **防误触**：角速度过零检测、冷却时间
- **数据**：SwiftData + Swift Charts

## English

### Features
- **Swing Detection**: 800Hz high-frequency CoreMotion sampling with EMA filtering
- **Stroke Recognition**: Forehand, backhand, and serve detection based on real tennis biomechanics
- **Speed Calculation**: Swing speed estimation based on acceleration peak and angular displacement (30~220 km/h)
- **Audio Feedback**: Custom tennis swing sounds + haptic vibration
- **Shot History**: SwiftData persistence with daily stats and 7-day chart
- **Bilingual**: UI text follows system language (Chinese/English)


