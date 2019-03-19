开发环境： NodeJS
cnpm安装命令 npm install -g cnpm --registry=https://registry.npm.taobao.org

安装umi依赖
通过cnpm init -y初始化package.json，会自动生成node——modules  “-y”表示对需要提供的信息都自动按下回车键，表示接受默认值
通过cnpm install umi --save-dev安装umi依赖

配置文件被约定为 config/config.js  config.js初始化内容export default {};
src目录放置主要代码 pages存放页面代码 若要改成page，需在config.js里写singular:true
 
运行命令cnpm run dev

添加 umi-plugin-react 插件
cnpm install umi-plugin-react --save-dev

通过 cnpm run build 来构建出最终的产物，执行该命令后会生成最终的 HTML、CSS 和 JS 到 dist 目录下。
它们是浏览器可以直接识别并运行的代码，这样你就可以将它们部署到你想要的服务器上了。