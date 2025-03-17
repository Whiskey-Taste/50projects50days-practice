# Progress Steps

## 📌 Project Introduction / 项目介绍
This project is part of the **50 Projects in 50 Days** challenge. The **Progress Steps** feature allows users to navigate through a step-by-step process by clicking "Next" and "Prev" buttons, visually updating the progress bar.

本项目是 **50 Projects in 50 Days** 挑战的一部分。**Progress Steps** 功能允许用户通过点击 “Next” 和 “Prev” 按钮，逐步完成进度，并动态更新进度条。

## 🎯 Features / 功能特点
- **Step-by-step progress navigation**: Click "Next" to move forward and "Prev" to go back.
- **Smooth transition effects**: Uses CSS transitions for a visually appealing animation.
- **Disabled buttons logic**: Prevents users from going beyond the first or last step.
- **Responsive design**: Works well on various screen sizes.

- **逐步导航**：点击 "Next" 进入下一步，点击 "Prev" 返回上一步。
- **平滑过渡动画**：使用 CSS 过渡效果实现视觉流畅性。
- **按钮状态管理**：确保用户不会超出第一步或最后一步。
- **自适应设计**：在不同设备上均能良好显示。

## 🛠 Tech Stack / 技术栈
- HTML
- CSS (Flexbox, Transitions, Variables)
- JavaScript (Event Listeners, DOM Manipulation)

- HTML
- CSS（Flexbox, 过渡动画, 变量）
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
- The `next` and `prev` buttons update the `currentActive` step.
- The function `update()` ensures that:
  - The active class is added or removed correctly.
  - The progress bar updates based on the number of active steps.
  - The buttons enable/disable based on step limits.

- `next` 和 `prev` 按钮用于更新 `currentActive` 步骤。
- `update()` 函数的作用：
  - 确保 `active` 类正确添加或移除。
  - 进度条根据当前的步数动态更新。
  - 按钮的启用/禁用逻辑正确运行，避免超出界限。

### 📌 Be Careful with Auto-completion Plugins / 注意自动补全插件
While using **Prettier** or similar code formatting plugins, be cautious. Sometimes, automatic formatting might introduce unintended changes, especially in JavaScript, affecting the final UI behavior.

在使用 **Prettier** 或其他代码格式化插件时要注意，有时自动补全会带来不符合预期的代码修改，尤其在 JavaScript 文件中，可能影响最终界面实现，需要仔细检查代码。

## 🔗 References & Acknowledgments / 参考与鸣谢
- **Original Project**: [50 Projects in 50 Days - HTML, CSS & JavaScript](https://github.com/bradtraversy/50projects50days)
- **Author**: Brad Traversy

- **原项目**：[50 Projects in 50 Days - HTML, CSS & JavaScript](https://github.com/bradtraversy/50projects50days)
- **作者**：Brad Traversy