# SwiftLearning
---
###swift语言特点

- 采用安全的编程模式,并添加了很多新的特性
- 采用自动引用计数来优化内存管理
- 它有很多JS Java C++等语言的特点的影子

---
###学习资料


- [官方的 Swift 学习手册](https://itunes.apple.com/us/book/swift-programming-language/id881256329?mt=11&uo=8&at=11ld4k&uo=8&at=11ld4k&uo=8&at=11ld4k)

- [CocoaChina 翻译的中文学习手册](https://github.com/CocoaChina-editors/Welcome-to-Swift)

---
###Playground 文件

Playground 文件是 Xcode 6 新推出的一种类型的文件，主要用于测试 Swift 代码。使用 Playground 能够做到：输入代码，便可以在右侧边栏立即看到代码逐行执行的效果。

利用这一特性，我们可以：

无需创建项目，便能够快速尝试新的 API，这对学习 Swift 非常有帮助
在设计新的算法时，可以逐行验证执行情况，提高开发效率

---
###命名空间概念

- 就像在 OC 中在项目中如果导入多个框架如果没有类前缀这个习惯就很容易产生类的命名冲突,因此在OC中是以类前缀来解决这个问题
- 而在 swift 则以项目的名称来作为类的命名空间,比如 AProject 有个Person 类,在BProject 中如果要加载该类,该类的类名 则以 AProject.Person 来加载

--- 
### 关于swift 和 OC 混编

- swift 中引入 OC 

```
1. 新建一个 .h 文件 import 要引入的 OC 框架
2. 选中项目的图标,注意Project 图标下面有 mianBundle 和 testBundle ,如果在那个bundle中使用了该OC框架,就设置那个bundle
3. 关联.h文件 : BuildSetting -> 搜索 bridge 在OC Bridge Header 中关联 .h 文件,路径为在实体文件中.h文件相对于项目图标的相对路径
```
