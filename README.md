# @domain.js/counter

[![Build status](https://travis-ci.com/domain-js/counter.svg?branch=master)](https://travis-ci.org/domain-js/counter)
[![codecov](https://codecov.io/gh/domain-js/counter/branch/master/graph/badge.svg)](https://codecov.io/gh/domain-js/counter)

# Installation
<pre>npm i @domain.js/counter --save</pre>

# cnf
专属配置名称 `counter`
| 名称 | 类型 | 必填 | 默认值 | 描述 | 样例 |
| ---- | ---- | ---- | ------ | ---- | ---- |
| key  | string | `是` | `无` | 计数器在redis里的key名 | counters |

# deps
| 模块名 | 别名 | 用到的方法 | 描述 |
| redis | `无` | hget, hset, hincrby | ioredis 的实例 |


# Usage
| 功能 | 描述 | 样例 |
| ---- | ---- | ---- |
| get  | 获取某个计数器值 | await counter.get('age') |
| incr | 计数器加一 | await counter.incr('age') |
| set | 重置某个计数器值 | await counter.set('age', 20) |
