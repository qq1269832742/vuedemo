# vuedemo
vue + webpack
## 学习vue，搭建vue+webpack的前端项目，但不包括UI，路由模块已设置完毕。
###   虽然网上有很多大佬有教程，时至今日，教程一部分内容有错误，经过修改后已经可以成功运sss
安装nodeJS，这一部分我就不说了。直接vue起步。wiki语法不咋会，凑合看。命令行攻击使用的是Git Bash。  
##1.安装vue-cil 命令： npm install -g vue-ci          
##2.进入到工程目录下命令：cd  vue-project(目录写自己的目录)    
##3.新建自己的vue项目：vue init webpack vuedemo    
##4.打开自己新建项目的目录：vue init webpack vuedemo    
##5.跑起项目来检测下： npm run dev    
##后续工作就是修改为适合自己的目录，配置路由。直接看项目即可。 
# 遇到的坑：记得找到build目录下的webpack.base.conf.js文件，注释检测代码的插件，此模块导致一部分语法不正确，一直报错，其实没毛病的。下面是注释部分
//const createLintingRule = () => ({      
//test: /\.(js|vue)$/,   
//loader: 'eslint-loader',  
//enforce: 'pre',  
//include: [resolve('src'), resolve('test')],  
//options: {  
//  formatter: require('eslint-friendly-formatter'),  
//  emitWarning: !config.dev.showEslintErrorsInOverlay  
//}  
//})  
//module所在的地方  
//   ...(config.dev.useEslint ? [createLintingRule()] : []),  
