---
name: 问题报告
description: 项目的文档或者代码需要补充与修改。
title: "[Problem]: "
labels: ["bug"]

body:
- type: markdown
    attributes:
      value: |
        感谢您向我们报告问题！请填写以下内容，以帮助我们更好地理解问题并解决它。
- type: input
    id: contact
    attributes:
      label: 联系方式（可选）
      description: 如果您愿意提供联系方式，我们会在解决问题后通知您。
      placeholder: ex. <email@example.com>
    validations:
      required: false
- type: dropdown
    id: type
    attributes:
      label: 问题类型
      multiple: false
      options:
        - 文档问题
        - 界面显示问题
- type: textarea
    id: what-happened
    attributes:
      label: 问题描述
      description: 请简要描述您遇到的问题。
      placeholder: ex. Nvidia 已经发布了 70 系列的显卡，但是文档中还没有相关内容！
    validations:
      required: true
- type: textarea
    id: what-should-happen
    attributes:
      label: 解决方案（可选）
      description: 请简要描述您的解决方案。
      placeholder: ex. 70 系列显卡包含 7050、7060、7070 和 7080 四款显卡……
    validations:
      required: false
---