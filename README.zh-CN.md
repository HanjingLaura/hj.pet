# HJ Codex 桌宠

[English](README.md) | 简体中文

![HJ 待机预览](assets/idle.gif)

HJ 是一个像素风 Codex 桌宠：黑发、眼镜、黑西装、红领带，带着一把小金色萨克斯，还有一点滑板气质。

## 预览

![HJ 动作预览图](assets/contact-sheet.png)

## 文件

- `pet.json` - Codex 桌宠配置文件。
- `spritesheet.webp` - 桌宠动画精灵图。
- `assets/` - README 预览图资源。

## 安装

将 `pet.json` 和 `spritesheet.webp` 复制到本地 Codex 桌宠目录：

```powershell
New-Item -ItemType Directory -Force "$env:USERPROFILE\.codex\pets\hj"
Copy-Item .\pet.json, .\spritesheet.webp "$env:USERPROFILE\.codex\pets\hj" -Force
```

然后重启 Codex，在宠物列表里选择 `HJ`。

## 动作状态

- `idle` - 普通待机状态。
- `running-right` - 向右移动或被拖向右侧。
- `running-left` - 向左移动或被拖向左侧。
- `waving` - 唤醒或注意状态。
- `jumping` - 活跃反馈状态。
- `failed` - 失败、取消或受阻状态。
- `waiting` - 等待用户输入。
- `running` - Codex 正在执行任务。
- `review` - 任务完成，等待查看结果。

## 说明

目前 Codex 自定义桌宠通过 `pet.json` 和 `spritesheet.webp` 支持动画显示。
