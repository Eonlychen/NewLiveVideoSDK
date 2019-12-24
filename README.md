# NewLiveVideoSDK
######
****本篇主要说明 已有使用了cocoapods的项目集成LiveVideoCoreSDK,（感谢此大佬https://github.com/runner365/LiveVideoCoreSDK.git）

####
1.使用pod命令创建工程，不做详解；

2.将此工程LiveVideoCoreSDK和RtmpLivePushSDK两个文件夹拷贝到你自己的工程中；

3.选中pod生成的.xcworkspace文件右击——显示包内容——打开contents.xcworkspacedata此文件（推荐使用vscode）；

     <FileRef
      location = "group:LiveVideoCoreSDK/LiveVideoCoreSDK.xcodeproj">
     </FileRef>
     <FileRef
      location = "group:RtmpLivePushSDK/RtmpLivePushSDK.xcodeproj">
     </FileRef>
   
   ————将此两条内容插入相应的位置（详细可自行看demo）；
   
 4.******最主要，由于xocde10已经不再支持libstdc++等静态库；所以自己创建的工程添加libc++这个库就好了；
 
 
 小提示：bitcode置为false
 
再次感谢https://github.com/runner365/LiveVideoCoreSDK.git
