# 表单生成器

## 概述

表单生成器e-form-generator借鉴[form-generator]()而来,修改适配antd-vue控件,
可根据拖拽布局生成vue页面布局，也可导出json直接传入生成器[ezio-form-generator]()使用

## 如何使用
1.安装组件
```
npm i @ezioframework/ezio-form-generator
```
2.代码中引用
```
<EFormDesign />
```

## 自定义参数
| 参数              | 描述   | 默认值  | 
| --------------   | ----   |  ----   |
| header           | 是否展示头部   | true  |  
| foot             | 是否展示页脚  | true  |  
| logo             | 替换标签   | null  | 
| formName         | 表单存储名称  | FORM_1  | 
| title            | 页面标题  | 表单设计器  | 
| showToolbarsText | 是否展示操作栏  | true  | 
| actionToolbars   | 操作栏展示的按键 | ['importJson','exportCode','undo',<br>'redo','run','viewJson',<br>'clean','save','close']| 
| actionStatus     | 操作栏展示是否禁用<br>(false:不禁用,true:禁用)   | {importJson: false,exportCode: false,<br>undo: false,redo: false,run: false,<br>viewJson: false,clean: false,<br>save: false,close: false}| 
| showDocLink      | 展示空间相关文档链接  | false  | 


## 组件扩展

