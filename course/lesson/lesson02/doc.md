# 学习要点：

- **HTML 结构和 CSS 样式**：本节课主要学习了如何使用 HTML 和 CSS 来设计和美化网页元素。
  
- **样式化不同类型的盒子**：学习了如何通过 CSS 设置盒子的大小、边框、背景色以及文本样式。
  
- **Flex 布局基础**：介绍了如何利用 Flex 布局来管理和排列网页中的元素，实现灵活的布局设计。


# 使用 `style` 属性的元素及其样式概述：

1. **普通盒子**：
   ```html
   <div>我是一个普通的盒子</div>
   ```
   - **作用**: 没有额外样式，展示默认的文本块。

2. **带高宽和边框的盒子**：
   ```html
   <div style="width: 100px; height: 100px; border: 1px solid red;">我是一个带高宽的盒子</div>
   ```
   - **作用**: 设置了宽度、高度和红色边框，展示一个具有固定尺寸和边框的盒子。

3. **黑色背景盒子**：
   ```html
   <div style="width: 100px; height: 100px; background-color: black; color: white;">我是黑色的</div>
   ```
   - **作用**: 设置了宽度、高度、黑色背景和白色文本颜色，展示一个黑色背景的盒子。

4. **有外边距的盒子**：
   ```html
   <div style="margin: 15px; width: 100px; height: 100px; border: 1px solid red;">别人不准碰我</div>
   ```
   - **作用**: 设置了外边距、宽度、高度和红色边框，展示一个带外边距的盒子。

5. **有内边距的盒子**：
   ```html
   <div style="padding: 15px; width: 100px; height: 100px; border: 1px solid red;">我不喜欢肚子里的东西贴着</div>
   ```
   - **作用**: 设置了内边距、宽度、高度和红色边框，展示一个带内边距的盒子。

6. **Flex 布局的例子**：
   ```html
   <div class="home" style="display: flex;">
       <div>老大</div>
       <div>老二</div>
       <div>老壁灯</div>
   </div>
   ```
   - **作用**: 使用了 Flex 布局，`.home` 容器内的 `<div>` 元素按照 Flex 布局规则进行排列和显示。

### `style` 属性概述：

- **作用**: `style` 属性用于直接为 HTML 元素指定内联样式，控制元素的外观和布局。

- **可选参数**: 可以在 `style` 属性中使用各种 CSS 属性和对应的值，如:
    - 尺寸（`width`, `height`）
    - 颜色（`background-color`, `color`）
    - 边框（`border`）、外边距（`margin`）
    - 内边距（`padding`）等。

- **优先级**: 元素的 `style` 属性内的样式规则优先级高于外部样式表和内部样式表中的普通规则，但低于带有 `!important` 声明的规则。

#### Flex 布局进阶：

- **Flex 容器属性**：
  - `display: flex;`: 将元素设为 Flex 容器，使其子元素成为 Flex 项目。
  - `flex-direction`: 设置主轴的方向（`row`, `column`, `row-reverse`, `column-reverse`）。
  - `justify-content`: 控制主轴上 Flex 项目的对齐方式（`flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly`）。
  - `align-items`: 控制交叉轴上 Flex 项目的对齐方式（`flex-start`, `flex-end`, `center`, `baseline`, `stretch`）。
  - `flex-wrap`: 控制 Flex 项目在一行上是否换行（`nowrap`, `wrap`, `wrap-reverse`）。

- **Flex 项目属性**：
  - `flex-grow`: 定义 Flex 项目的放大比例。
  - `flex-shrink`: 定义 Flex 项目的缩小比例。
  - `flex-basis`: 定义 Flex 项目在主轴上的初始大小。
  - `align-self`: 单独控制某个 Flex 项目在交叉轴上的对齐方式。

Flex 布局提供了强大的布局方式，能够灵活地调整和排列页面中的元素，适应不同的布局需求和屏幕尺寸，是现代 Web 开发中常用的布局技术之一。


Emmet 是一个强大的工具，可以帮助快速编写 HTML 和 CSS。以下是一些常用的 Emmet 缩写清单，包括基本的 HTML 结构、常见的 HTML 标签、属性和常用的 CSS 样式。

# HTML 缩写：

- **基本结构**：
  - `!`: 生成基本的 HTML5 结构。
  - `html:lang=en`：带有 lang 属性的 HTML 文档。

- **标签**：
  - `div`: 创建一个 `<div>` 元素。
  - `p`: 创建一个 `<p>` 段落。
  - `a`: 创建一个 `<a>` 链接。
  - `img`: 创建一个 `<img>` 图片。
  - `ul>li*5`: 生成一个包含五个 `<li>` 的无序列表。
  - `table>tr*3>td*3`: 生成一个 3x3 的表格。

- **类和 ID**：
  - `.class1.class2`: 创建带有多个类的元素。
  - `#id`: 创建带有 ID 的元素。

- **文本和属性**：
  - `a[href="#"]`: 创建一个带有链接的 `<a>` 元素。
  - `p>{Lorem ipsum $}*3`: 生成三个段落，每个段落都包含 "Lorem ipsum 1"、"Lorem ipsum 2"、"Lorem ipsum 3" 的文本。

### CSS 缩写：

- **样式属性**：
  - `m10`: 为元素添加 10px 的 margin。
  - `p20`: 为元素添加 20px 的 padding。
  - `bgc#f00`: 设置背景色为红色。
  - `fs14`: 设置字体大小为 14px。

- **Flex 布局**：
  - `d:f`: 设置 `display: flex;`。
  - `jc:sb`: 设置 `justify-content: space-between;`。
  - `ai:c`: 设置 `align-items: center;`。
  
这些 Emmet 缩写可以显著提高 HTML 和 CSS 的编写效率，使开发者可以更快速地创建和布局页面结构。在 VS Code 或其他支持 Emmet 的编辑器中，通过简单的缩写即可快速生成复杂的代码结构和样式。