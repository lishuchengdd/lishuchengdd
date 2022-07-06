# 模块
## AppModule -> 根模块
- 每个应用至少有一个angular模块，称为根模块
- 根模块通常命名为AppModule
- 根模块的作用：启动应用
- 模块是独立封闭的
- 模块之间的引用通过 **导入** 和 **导出** 来完成的 

## 模块中包含的内容
- 组件
- 服务
- 指令
- 注意：这些内容必须在模块中配置后有才有效
## @NgModul 装饰器
- 装饰器是一个函数
- 作用：修饰紧跟其后的类或者属性
- 装饰器是JavaScript的一种语言特性，处于语法提案的stage 2阶段，是一个试验特性
- 装饰器又叫注解
- @NgModul是angular提供的装饰器
- 用来告诉angular将这个类当做模块来处理
- 语法：@NgModul{(元数据对象)}

## @NgModul装饰器的元数据对象
- declarations——该模块所拥有的组件
- imports—— 该模块依赖的模块，比如：BrowserModule
- providers—— 该模块所拥有的服务提供商
- bootstrap—— 指定根组件，只有根模块需要该配置项Angular创建它并插入index.html宿主页面

# 组件
## @Component装饰器
- selector—— 选择器（组件名称），对应HTML中的组件名称
- template—— 组件的内联模板
- templateUrl—— 组件模板文件的URL
- styleUrls—— 组件样式文件数组
