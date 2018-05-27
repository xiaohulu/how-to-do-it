# tslint

## Import sources within a group must be alphabetized.

此规则要求：
1. 将 import 语句分组（使用一个空行分组）；
2. 一个组中的 import 语句要按照字母顺序排列；

import 语句排序规则详见 https://palantir.github.io/tslint/rules/ordered-imports/

## interface name must start with a capitalized I

此规则要求接口名必须以 `I` 开头，如果不使用该规则，则在 `tslint.json` 中关闭此规则

```json
{
  "rules":{
    "interface-name": [true, "never-prefix"]
  }
}
```

`never-prefix` 表示不使用前缀。

接口命名规则详见 https://palantir.github.io/tslint/rules/interface-name/

## The key 'data' is not sorted alphabetically

此规则要求：对象字面量的 key 必须按字母顺序排列。

可在 `tslint.json` 中关闭此规则

```json
{
  "rules":{
    "object-literal-sort-keys": false
  }
}
```

规则详见 https://palantir.github.io/tslint/rules/object-literal-sort-keys/

## unused expression, expected an assignment or function call

我遇到的情况是不允许使用逻辑运算符做 null 检测，如`e && e.preventDefault()`

下面关闭此规则

```json
"no-unused-expression": [true, "allow-fast-null-checks"]
```

规则详见 https://palantir.github.io/tslint/rules/no-unused-expression/