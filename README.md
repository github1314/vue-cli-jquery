# 在vue-cli中使用jquery的正确方法

> A Vue.js project

## zhengque步骤

``` bash
# 在webpack.base.conf.js加入
        var webpack = require('webpack')

# 在module.exports中最末尾加入一个对象
        plugins:[
     				new webpack.ProvidePlugin({
      			    $:"jquery",
        		    jQuery:'jquery',
        		    "window.jQuery":"jquery"
   					})
				]

# 在main.js中引入
        import $ from 'jquery'

# 再需要的地方写jquery代码
        注意：必须要加载$( function( ){ } )
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
