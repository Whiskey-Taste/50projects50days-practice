# Rotating Navigation Animation

## 📌 Project Introduction / 项目介绍
This project is part of the **50 Projects in 50 Days** challenge. The **Rotating Navigation Animation** creates an interactive navigation effect where clicking a button rotates the main content, revealing a sidebar navigation menu.

本项目是 **50 Projects in 50 Days** 挑战的一部分。**Rotating Navigation Animation** 通过点击按钮旋转主内容，从而显示侧边栏导航菜单，实现炫酷的交互效果。

## 🎯 Features / 功能特点
- **Rotating Page Animation**: Clicking the menu button rotates the page to reveal navigation.
- **Smooth CSS Transitions**: Uses `transform` and `transition` for smooth animations.
- **Simple and Lightweight**: Uses minimal HTML, CSS, and JavaScript.
- **Responsive Design**: Works on different screen sizes.

- **页面旋转动画**：点击菜单按钮，页面旋转，展示侧边栏导航。
- **平滑 CSS 过渡动画**：使用 `transform` 和 `transition` 实现流畅的动画效果。
- **简洁轻量**：仅使用基础 HTML、CSS 和 JavaScript 实现。
- **自适应设计**：适用于不同设备。

## 🛠 Tech Stack / 技术栈
- HTML
- CSS (Transformations, Transitions)
- JavaScript (Event Listeners, DOM Manipulation)

- HTML
- CSS（变换效果，过渡动画）
- JavaScript（事件监听，DOM 操作）

## 📂 Project Structure / 项目结构
```
├── index.html  # Main HTML file
├── style.css   # CSS styles
├── script.js   # JavaScript functionality
├── README.md   # Project documentation
```

## 📝 Code Explanation / 代码说明
### 📌 JavaScript Logic / JavaScript 逻辑
- Clicking the **hamburger menu (`open`)** button adds the `show-nav` class to the `.container`, which triggers the rotation effect.
- Clicking the **close (`close`)** button removes the `show-nav` class, restoring the original layout.

```js
const open = document.getElementById('open');
const close = document.getElementById('close');
const container = document.querySelector('.container');

open.addEventListener('click', () => container.classList.add('show-nav'));
close.addEventListener('click', () => container.classList.remove('show-nav'));
```

- 点击 **菜单按钮 (`open`)** 会给 `.container` 添加 `show-nav` 类，触发旋转效果。
- 点击 **关闭按钮 (`close`)** 会移除 `show-nav` 类，使页面恢复原状。

### 📌 Important CSS Tip: `@import url()` / 重要 CSS 细节：`@import url()`
If you use `@import url()` in CSS to load external fonts or stylesheets, **always remember to add a semicolon (`;`) at the end**. Forgetting the semicolon can cause issues, preventing the rest of the CSS from loading correctly.

Example:
```css
@import url('https://fonts.googleapis.com/css?family=Lato&display=swap');
```

在 CSS 文件中使用 `@import url()` 引入外部字体或样式时，**务必要在末尾加上分号 (`;`)**，否则可能会影响后续 CSS 代码的解析。

示例：
```css
@import url('https://fonts.googleapis.com/css?family=Lato&display=swap');
```

## 🔗 References & Acknowledgments / 参考与鸣谢
- **Original Project**: [50 Projects in 50 Days - HTML, CSS & JavaScript](https://github.com/bradtraversy/50projects50days)
- **Author**: Brad Traversy

- **原项目**：[50 Projects in 50 Days - HTML, CSS & JavaScript](https://github.com/bradtraversy/50projects50days)
- **作者**：Brad Traversy

