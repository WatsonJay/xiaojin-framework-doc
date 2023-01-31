# 表单生成器

## 概述

表单生成器ezio-form-generator借鉴[form-generator]()而来,修改适配antd-vue控件,
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
| 参数              | 描述   | 默认值  | 可选类型 |
| --------------   | ----   |  ----   | ----  |
| header           | 是否展示头部   | true  | boolean |
| foot             | 是否展示页脚  | true  |  boolean |
| logo             | 替换标签   | null  | 
| formName         | 表单存储名称  | FORM_1  | String |
| title            | 页面标题  | 表单设计器  | String |
| showToolbarsText | 是否展示操作栏  | true  | boolean |
| actionToolbars   | 操作栏展示的按键 | ['importJson','exportCode','undo',<br>'redo','run','viewJson',<br>'clean','save','close']| Array |
| actionStatus     | 操作栏展示是否禁用(false:不禁用,true:禁用)   | {}| importJson: false,exportCode: false,undo: false,redo: false,run: false,viewJson: false,<br>clean: false,save: false,close: false |
| showDocLink      | 展示空间相关文档链接  | false  | boolean |

**eg:**

*1.当actionBar需要禁用按键时,只需要将相关按键传入actionStatus中,例如{importJson: true}*

| 参数 | 对应按键 | 备注 |
| ----- | ----- | ---- |
| importJson | 导入json | |
| exportCode | 导出生成代码 | |
| undo | 撤销上一步操作 |
| redo | 取消上一次撤销 |
| run | 预览代码 |
| viewJson | 查看生成json |
| clean | 清除所有组件 |
| save | 保存json | 点击触发$emit('handleSave') |
| close | 关闭 | 点击触发$emit('handleClose') |

## 通用表单定义
+

## 组件定义
eizo-form-generator基础上分作三类: 基础组件,高级组件,布局型组件。组件的构建属性通过JSON存放,可以通过外部方式进行引入添加。
+ 基础配置项
    - \_\__config___:基础配置
      * layout: 'colFormItem',
      * type: 'divider',
      * tagIcon: 'efg-line',
      * label: '分割线',
      * document: 'https://element.eleme.cn/#/zh-CN/component/layout#row-attributes'
