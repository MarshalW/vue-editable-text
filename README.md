# vue-editable-text

支持中文输入的单行 `contenteditable` 文本 Vue 组件。

## 如何使用

### 安装

```
npm i @marshal/vue-editable-text
```

或者

```
yarn add @marshal/vue-editable-text
```

### 使用

引入依赖：

```js
import EditableText from "@marshal/vue-editable-text";
```

使用：

```html
<editable-text v-model="name" :placeholder="'姓名'" />
```

完整的单文件组件示例：

```js
<template>
  <div id="app">
    <div>
      <editable-text v-model="name" :placeholder="'姓名'" />
    </div>
  </div>
</template>

<script>
import EditableText from "@marshal/vue-editable-text";

export default {
  name: "app",
  components: {
    EditableText
  },
  data() {
    return {
      name: ""
    };
  }
};
</script>
```
