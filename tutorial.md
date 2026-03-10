# 红米K40 9008 纯命令行解锁教程

> ⚠️ 警告：解锁会清空手机所有数据！操作前务必备份！

## 一、前置准备
- 电脑：Windows 10/11（必须管理员权限）
- 手机：红米K40 / 小米11X / POCO F3
- 线材：9008 工程线（普通线进不去 9008）
- 软件：MiFlash Prime（自带驱动 + edl.exe）

## 二、进入 9008 模式
1. 手机彻底关机
2. 按住 **音量上 + 音量下** 不放
3. 保持按键，插入 9008 工程线连电脑
4. 设备管理器出现 `Qualcomm HS-USB QDLoader 9008` 即成功

## 三、命令行解锁（只解锁，不刷机）
1. 以管理员打开 PowerShell
2. 进入 MiFlash 目录：

```powershell
cd "C:\Program Files\Xiaomi\MiFlash\bin"
```

3. 执行解锁命令（**只运行这一行**）：

```powershell
.\edl.exe oem unlock
```

4. 看到 `OKAY` 即解锁成功
5. 拔线 → 重启手机

## 四、支持与不支持机型
### ✅ 支持 9008 解锁
- 红米K40 / 小米11X / POCO F3
- 小米10 / 10 Pro
- 红米K30 Pro

### ❌ 完全不能解锁
- 小米澎湃OS 2.0 及以上新机（K80、小米15 等）
- OPPO / vivo / 荣耀 近年新机型
- 三星近年旗舰（无公开 EDL 解锁）

## 五、常见错误
- `device not found`：没进 9008 或驱动没装
- `NOT allowed`：机型已被封堵，无法解锁

