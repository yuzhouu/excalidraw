# 对 excalidraw 的改动

1. 去除 embeddable “点击以开始交互” 遮罩 `excalidraw__embeddable-hint` isHovered App.tsx
2. 让 embeddable 处于激活状态时可以移动 `this.state.activeEmbeddable?.state !== "active"` App.tsx

```css
.excalidraw__embeddable-container__inner {
  pointer-events: none !important;
}
```

3. 不要渲染 embeddable 的小角标 `renderLinkIcon` static canvas
4. isMobileBreakpoint always return false
5. getDefaultAppState().viewBackgroundColor 默认改为透明
6. grid line color 从 css 变量中取
