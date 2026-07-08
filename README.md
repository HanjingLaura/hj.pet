# HJ Codex Pet / HJ Codex 桌宠

HJ is a pixel-art Codex desktop pet with black hair, glasses, a black suit, a red tie, a tiny golden saxophone, and skateboard energy.

HJ 是一个像素风 Codex 桌宠：黑发、眼镜、黑西装、红领带，带着一把小金色萨克斯，还有一点滑板气质。

![HJ idle preview](assets/idle.gif)

## Preview / 预览

![HJ animation contact sheet](assets/contact-sheet.png)

## Files / 文件

- `pet.json` - Codex pet manifest. / Codex 桌宠配置文件。
- `spritesheet.webp` - animated pet spritesheet. / 桌宠动画精灵图。
- `assets/` - README preview images. / README 预览图资源。

## Install / 安装

Copy `pet.json` and `spritesheet.webp` into your local Codex pets folder:

将 `pet.json` 和 `spritesheet.webp` 复制到本地 Codex 桌宠目录：

```powershell
New-Item -ItemType Directory -Force "$env:USERPROFILE\.codex\pets\hj"
Copy-Item .\pet.json, .\spritesheet.webp "$env:USERPROFILE\.codex\pets\hj" -Force
```

Then restart Codex and choose `HJ` from the pets list.

然后重启 Codex，在宠物列表里选择 `HJ`。

## Animation States / 动作状态

This pet includes the standard Codex animation states:

这个桌宠包含 Codex 标准动作状态：

- `idle` - normal resting state. / 普通待机状态。
- `running-right` - moving or being dragged to the right. / 向右移动或被拖向右侧。
- `running-left` - moving or being dragged to the left. / 向左移动或被拖向左侧。
- `waving` - wake or attention state. / 唤醒或注意状态。
- `jumping` - lively feedback state. / 活跃反馈状态。
- `failed` - failed, cancelled, or blocked state. / 失败、取消或受阻状态。
- `waiting` - waiting for user input. / 等待用户输入。
- `running` - Codex is working. / Codex 正在执行任务。
- `review` - work is ready to review. / 任务完成，等待查看结果。

## Notes / 说明

Codex custom pets currently support image animation through `pet.json` and `spritesheet.webp`.

目前 Codex 自定义桌宠通过 `pet.json` 和 `spritesheet.webp` 支持动画显示。
