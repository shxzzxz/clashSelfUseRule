# clash





## 常用配置说明

**过滤包含特定字符串节点**

```yaml
filter: ^((?!台|剩余|最新|过期|新|官|期).)*$ #"^((?![官]).)*$"
```

- `(?!台|剩余)` 是零宽断言
- `(?!台|剩余).` 匹配前面不是 `台,剩余` 字符串的字符，记为 rule_char
- 总的表达式匹配全部由 rule_char 组成的字符串
