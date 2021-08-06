---
title: Declaring props
---

到目前为止，我们只处理内部状态——也就是说，这些值只能在给定的组件内访问。

在任何实际应用程序中，您都需要将数据从一个组件向下传递到其子组件。 为此，我们需要声明*properties*，通常缩写为“props”。 在 Svelte 中，我们使用 `export` 关键字来做到这一点。 编辑 `Nested.svelte` 组件：

```html
<script>
	export let answer;
</script>
```

> 就像 `$:` 一样，一开始你可能会觉得有点奇怪。 这不是 `export` 在 JavaScript 模块中的正确工作方式啊！ 但很快你就会发现这个十分流畅，现在就开始使用吧。
