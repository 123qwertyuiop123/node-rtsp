# node-rtsp
rtsp转码播放

- 使用vlc模拟rtsp推流/拉流

- 使用ffmpeg对rtsp进行转码

- 使用node服务就行转码后推流

- 使用flv.js进行播放展示

# 使用
- 需要安装ffmpeg和node环境
- 先安装项目依赖，执行命令：npm i
- 启动node服务，运行npx nodemon index3.js
- 运行cmd命令打开终端，使用ffmpeg命令对rtsp流进行转码
ffmpeg -i rtsp:[地址] -c copy -f flv rtmp://localhost:1935/live/test[为node服务的地址，可以修改]
- 运行index3.html
- 截屏使用canvas进行操作