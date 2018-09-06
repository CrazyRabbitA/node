# express-sticky-note
A sticky note using node and express


bin是启动网站的入口
node_module是所依赖的模块
public是静态的资源，放的是经过webpack解析过的代码，代码最终运行时访问的是这个文件夹下面的资源
router是路由
views是模板 
src里是初始开发时写的文件，包括less，未压缩的图片，es6写的js，src下再划分文件夹为了使逻辑更清晰，查找时更方便
src 下的js 下的lib放一些跟自己写的功能无关的js文件，如jquery，vue这些自己引用的东西
src 下的app 是不同页面的入口
src 下的mod 放的是通用的一些组件，如轮播组件，事件中心，弹窗模块，等
webpack.config.js 用来设置打包配置，配置工程化，自动化的流程环境 script中的webpack用来自己设置webpack配置文件所在的路径
script中的watch在监视的文件发生变化时自动执行webpack，同步改变public中的文件，使用之前要先安装onchange，npm install --save-dev onchange
    "watch": "onchange 'src/**/*.js' 'src/**/*.less' -- npm run webpack"
    星星/星代表不管层级有多深，全部选择，即选择所有的js文件 只有*的话表示只选择当前目录下的所有js文件
    配置好之后，在终端上运行npm watch 就行了
# node
