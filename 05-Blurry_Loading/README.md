# Blurry Loading

## 📌 Project Introduction / 项目介绍
This project is part of the **50 Projects in 50 Days** challenge. The **Blurry Loading** effect simulates a loading screen where a blurry background gradually becomes clear as a percentage counter increases from 0% to 100%.

本项目属于 **50 Projects in 50 Days** 挑战中的一项，名为 **Blurry Loading（模糊加载）**。该效果模拟加载进度的过程，随着百分比从 0% 增加到 100%，背景图像从模糊逐渐变清晰。

## 🎯 Features / 功能特点
- **Animated percentage counter**: Displays loading progress from 0% to 100%.
- **Dynamic blur effect**: The background image transitions from blurry to clear.
- **Custom scaling function**: Uses a custom `scale()` function to map loading values to CSS styles.
- **Minimal and clean design**: Simple layout with only essential elements.

- **动态百分比计数**：显示加载进度从 0% 到 100%。
- **模糊动态过渡效果**：背景从模糊逐步变得清晰。
- **自定义缩放函数**：通过 `scale()` 函数将加载值映射为 CSS 样式数值。
- **简洁的视觉设计**：页面内容极简，只保留关键组件。

## 🛠 Tech Stack / 技术栈
- HTML
- CSS (Blur Filter, Transitions)
- JavaScript (Timer, DOM Manipulation, Custom Math)

- HTML
- CSS（模糊滤镜、过渡动画）
- JavaScript（定时器、DOM 操作、自定义数学函数）

## 📂 Project Structure / 项目结构
```
├── index.html  # Main HTML file
├── style.css   # CSS styles
├── script.js   # JavaScript logic
├── README.md   # Project documentation
```

## 📝 Code Explanation / 代码说明
### 🔢 JavaScript Logic / JavaScript 逻辑
```js
let load = 0;
let int = setInterval(blurring, 30);

function blurring() {
    load++;
    if (load > 99) {
        clearInterval(int);
    }
    loadText.innerText = `${load}%`;
    loadText.style.opacity = scale(load, 0, 100, 1, 0);
    bg.style.filter = `blur(${scale(load, 0, 100, 30, 0)}px)`;
}
```
- Increments `load` every 30ms.
- Once `load` reaches 100, it stops the interval.
- Uses the `scale()` function to interpolate values for `opacity` and `blur` effects.

- 每 30 毫秒增加一次 `load`。
- 当 `load` 达到 100 时，停止定时器。
- 使用 `scale()` 函数将 `load` 映射为 `opacity` 和 `blur` 的样式值。

### 📐 `scale()` Function / 缩放函数说明
```js
const scale = (num, in_min, in_max, out_min, out_max) => {
    return ((num - in_min) * (out_max - out_min)) / (in_max - in_min) + out_min;
};
```
- Maps one numerical range into another. Inspired by Arduino's `map()` function.
- Commonly used in animations and data normalization.

- 将一个数值从某个区间映射到另一个区间，类似 Arduino 中的 `map()` 函数。
- 常用于动画控制和数据缩放处理。

### ⚠️ About Semicolons in JS / 关于分号的建议
Although JavaScript supports **automatic semicolon insertion**, it is a best practice to **add semicolons manually** after:
- Variable declarations
- Arrow function expressions

尽管 JavaScript 支持**自动插入分号机制（ASI）**，但建议在以下情况下手动添加分号：
- 变量声明后
- 箭头函数表达式末尾

这样可以提升代码可读性，防止某些边界情况出错。

## 🔗 References & Acknowledgments / 参考与鸣谢
- **Original Project**: [50 Projects in 50 Days - HTML, CSS & JavaScript](https://github.com/bradtraversy/50projects50days)
- **Author**: Brad Traversy

- **原项目**：[50 Projects in 50 Days - HTML, CSS & JavaScript](https://github.com/bradtraversy/50projects50days)
- **作者**：Brad Traversy