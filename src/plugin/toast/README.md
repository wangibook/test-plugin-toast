## 插件的安装
NPM  
npm i test-plugin-toast

## 引入插件
``` js
import Vue from 'vue'
import vueTotal from 'test-plugin-toast'
Vue.use(vueTotal)
```

## 基本用法
``` js
<test-toast ref="toast"></test-toast>
```
## 参数

| 参数 | 说明 | 类型 | 默认值 |
| - | :- | :- | :-: |
| ref | 获取当前插件实例 | String | - |

## demo地址：  
[demo演示](https://wangibook.github.io/test-plugin-toast/dist/index.html)

