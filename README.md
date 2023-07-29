# pt-loader

## 核心逻辑
1. 通过 this.getOptions 接口获取 Loader 配置对象；
2. 使用 schema-utils 的 validate 接口校验 Loader 配置是否符合预期，配置 
Schema 定义在 src/options.json 文件；
3. 返回经过修改的内容。

## 单元测试
1. 创建 webpack 实例，并运行Loader；
2. 获取 Loader 执行结果，比对、分析判断是否符合预期
3. 判断执行过程中是否出错

## Loader辅助工具
- loader-utils：Webpack5 之后该库部分能力被迁移到 Loader Context
- schema-tiles：校验用户传入的配置是否满足要求