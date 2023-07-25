# iOS面试相关

## 1. 基础知识

### 1.1 属性关键字

- 属性修饰符使用场景
- 什么是循环引用？如何避免循环引用？
- autoreleasepool的原理
- tips：自动释放池的实质是在开始处调用了autoreleasePoolPush方法，而在结束时调用了autoreleasePoolPop方法。其实push方法的作用是向这个双向链表结构的当前autoreleasePoolPage中插入哨兵对象，pop方法的作用是将插入的哨兵对象后的所有自动释放对象进行release操作。
- iOS内存分布（代码区/常量区/全局静态区(又分为BSS和Data)/堆区/栈区）
- tips：栈区由系统进行分配，通常用来存放函数参数、局部变量等数据。在实际开发中，指针变量本身存放在栈中，指向的对象数据会存放在堆中

### 1.2 Block相关


### 1.3 多线程和 GCD

- 什么是 GCD？它有哪些优势？
- GCD 中的队列是什么？并发队列和串行队列有什么区别？
- 在 iOS 开发中，什么情况下使用 GCD 来实现多线程？
- 如何避免在多线程环境下产生数据竞争？

## 2. UIKit

### 2.1 UIViewController

- 解释 UIViewController 的生命周期。
- 介绍常见的 UIViewController 之间的跳转方式。
- 什么是 UIViewController 的容器视图控制器（Container View Controller）？举例说明。

### 2.2 UITableView 和 UICollectionView

- UITableView 和 UICollectionView 有什么区别？
- 解释 UITableView 的重用机制（Cell Reuse）。
- 自定义 UITableViewCell 和 UICollectionViewCell 的步骤和常见问题。

### 2.3 Autolayout 和动画

- 什么是 Autolayout？在什么情况下使用 Autolayout？
- 使用 Autolayout 实现自定义视图的步骤。
- 如何实现平滑的动画效果？列举几种动画实现方式。

## 3. 数据存储

### 3.1 CoreData

- 什么是 CoreData？它与 SQLite 和 UserDefaults 的区别是什么？
- CoreData 的核心组件是什么？
- 如何在 iOS 中使用 CoreData 进行数据持久化？

### 3.2 NSUserDefaults 和 Keychain

- NSUserDefaults 和 Keychain 分别用于什么场景？
- 如何安全地存储敏感信息，例如用户密码？

## 4. 网络和数据解析

### 4.1 网络通信

- 在 iOS 中如何进行网络通信？列举常见的网络通信库和框架。
- 解释 RESTful API 的概念和使用方式。

### 4.2 JSON 和 Codable

- 什么是 JSON？如何在 iOS 中解析和生成 JSON 数据？
- 介绍 Codable 协议和它的作用。

## 5. 性能优化和调试

- 如何优化 iOS 应用的性能？
- 使用什么工具来检测和解决内存泄漏问题？
- 如何进行性能调试和 Instruments 分析？

## 6. 其他

- 什么是 APNs？如何实现远程推送通知？
- 如何进行版本适配和设备适配？
- 解释 iOS App 的生命周期。
