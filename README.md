#### 💡当静态资源发布到服务器上 傻傻分不清 是谁打的包？哪个版本？什么时候打的？
此插件会获取构建静态资源的用户、邮箱、分支、时间。同时会拉取最后一次的提交信息

<br/>

#### ❓怎么使用
```javascript
const BranchPlugin = require("@tntd/webpack-branch-plugin");

module.exports = {
    plugins: [
        // 要记得写你的输出文件哟
        new BranchPlugin({
			filename: config.common.sourcePrefix + ".branch_info.txt"
		})
    ]
}
```