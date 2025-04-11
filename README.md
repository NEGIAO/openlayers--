# openlayers--
GIS-webgis_网络技术
基于node.js的openlayers项目搭建与认识。

================================================================
《基于node.js的openlayers项目》
---node.js框架环境构建完毕后，使用openlayers的项目搭建与环境设置；
---openlayers是GIS中开源的webgis框架，在实际应用中有众多的使用

以下内容基于node.js环境搭建完毕后，进行openlayers项目的搭建
在文件夹中，运行cmd命令行程序：
1、步骤 1：创建项目目录
mkdir openlayers-ma
//创建目录“make directory”

cd openlayers-map
//更改目录“change directory”

npm init -y
//初始化项目，生成package.json

2、步骤 2：安装 OpenLayers
npm install ol
//装 OpenLayers 包（ol），并将其记录在 package.json 的 dependencies 中

3、步骤 3：安装开发服务器（使用 Parcel）
npm install parcel --save-dev
//将 Parcel 安装为开发依赖，记录在 package.json 的 devDependencies 中

配置 Parcel 启动脚本：打开 package.json，找到 scripts 部分，修改为以下内容：
"scripts": {
  "start": "parcel index.html",
  "build": "parcel build index.html"
}
//"start"：运行开发服务器，Parcel 会自动处理 index.html 及其依赖。 
//"build"：用于生成生产环境的打包文件（暂时无需使用）。

4、步骤 4：创建项目文件
在 openlayers-map 目录下，创建以下文件： index.html    main.js   style.css
编写三个文件

5、步骤 5：启动本地服务器
npm start
========================================================================

                            版权声明：本文为博主原创文章，遵循 CC 4.0 BY-SA 版权协议，转载请附上原文出处链接和本声明。
                        
原文链接：https://blog.csdn.net/2401_84934920/article/details/147143644
