# Expanding Cards

## 📌 Project Introduction / 项目介绍
This project is a part of the **50 Projects in 50 Days** challenge. The **Expanding Cards** feature allows users to click on different images to expand them, creating an interactive and visually appealing effect.

本项目是 **50 Projects in 50 Days** 挑战的一部分。**Expanding Cards** 功能允许用户点击不同的图片，使其展开，从而实现交互式的视觉效果。

## 🎯 Features / 功能特点
- **Interactive Image Expansion**: Click on an image to expand it while collapsing others.
- **Smooth CSS Transitions**: Uses `transition` for smooth animations.
- **Fully Responsive**: Works well on different screen sizes.
- **Modern UI Design**: Rounded corners, background images, and hover effects.

- **交互式图片扩展**：点击某张图片可展开，同时折叠其他图片。
- **平滑 CSS 过渡动画**：使用 `transition` 实现流畅的动画效果。
- **完全响应式**：适用于不同的屏幕尺寸。
- **现代化 UI 设计**：采用圆角、背景图片和悬停效果。

## 🛠 Tech Stack / 技术栈
- HTML
- CSS (Flexbox, Transitions)
- JavaScript (Event Listeners, DOM Manipulation)

- HTML
- CSS（Flexbox, 过渡动画）
- JavaScript（事件监听，DOM 操作）

## 📂 Project Structure / 项目结构
```
├── index.html  # Main HTML file
├── style.css   # CSS styles
├── script.js   # JavaScript functionality
├── README.md   # Project documentation
```

## 📝 Code Explanation / 代码说明
### 📌 CSS Background Image URL - Quotation Marks / CSS `background-image` 中的 URL 引号问题
In the following CSS code:
```css
style="background-image: url('https://images.unsplash.com/');"
```
The `url()` function allows both quoted and unquoted values:
- ✅ **With quotes (recommended):** `url('https://example.com/image.jpg')`
- ✅ **Without quotes (valid but riskier):** `url(https://example.com/image.jpg)`

Why use quotes?
1. **Avoid Parsing Issues**: If the URL contains special characters like `()`, `,`, `&`, or spaces, quotes ensure correct parsing.
2. **Better Readability**: It's clearer to read and understand.
3. **Browser Compatibility**: Some older browsers may misinterpret unquoted URLs.

在 CSS 代码中：
```css
style="background-image: url('https://images.unsplash.com/');"
```
`url()` 允许 URL 带引号或不带引号：
- ✅ **带引号（推荐）**：`url('https://example.com/image.jpg')`
- ✅ **不带引号（可用，但风险较高）**：`url(https://example.com/image.jpg)`

为什么建议加引号？
1. **避免解析问题**：如果 URL 含有特殊字符（如 `()`, `,`, `&`, 空格），使用引号可确保正确解析。
2. **提高可读性**：带引号的 URL 更易于阅读和理解。
3. **浏览器兼容性**：某些旧版浏览器可能会错误解析未加引号的 URL。

### 📌 Mac VS Code Terminal Issue / Mac VS Code 终端问题
On Mac, if you use a **Chinese input method**, pressing `Command + \`` may not open the terminal. Instead, it may insert a special character.

✅ **Solution:** Switch to an **English input method** (`ABC`) before pressing `Command + \``.

在 Mac 端的 VS Code 中，**如果使用中文输入法**，`Command + \`` 可能无法呼出终端，而是输入特殊字符。

✅ **解决方案**：切换到 **英文输入法** (`ABC`)，然后再按 `Command + \``。

## 🔗 References & Acknowledgments / 参考与鸣谢
- **Original Project**: [50 Projects in 50 Days - HTML, CSS & JavaScript](https://github.com/bradtraversy/50projects50days)
- **Author**: Brad Traversy

- **原项目**：[50 Projects in 50 Days - HTML, CSS & JavaScript](https://github.com/bradtraversy/50projects50days)
- **作者**：Brad Traversy