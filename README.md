# Behinder
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Ffuzhufuzhu%2FBehinder.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Ffuzhufuzhu%2FBehinder?ref=badge_shield)

“冰蝎”动态二进制加密网站管理客户端



功能介绍原文链接：

《利用动态二进制加密实现新型一句话木马之客户端篇》   https://xz.aliyun.com/t/2799

工作原理原文链接：

《利用动态二进制加密实现新型一句话木马之Java篇》 https://xz.aliyun.com/t/2744   

《利用动态二进制加密实现新型一句话木马之.NET篇》 https://xz.aliyun.com/t/2758   

《利用动态二进制加密实现新型一句话木马之PHP篇》  https://xz.aliyun.com/t/2774 

## 运行环境  

  客户端：jre6~jre8   
  服务端：.net 2.0+;php 5.4-7.2;java 6+   

## FAQ
* Mac系统下好像打不开？

  Mac系统下需要通过-XstartOnFirstThread参数启动，java -XstartOnFirstThread -jar Behinder.jar。
  
  
* 直接用浏览器访问shell会报错？

  客户端附带的服务端为最简版本，没有做容错处理，所以直接浏览器访问可能会报错，但是不影响客户端正常连接。如果不介意服务端体积增加几个字节，可以自己加一些容错判断语句。
  
* 我可以对shell进行修改么？

  客户端附带的服务端可以进行各种变形，只要基本逻辑不变，客户端即可正常连接。
  
* 开了socks代理，但是服务器并没有开启代理端口？

  socks代理的端口不是开在远程服务器上的，是开在本地的，利用socks客户端直接连接本地IP的代理端口即可，冰蝎会把本地端口的流量通过http隧道透传至远程服务器网络。
  


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Ffuzhufuzhu%2FBehinder.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Ffuzhufuzhu%2FBehinder?ref=badge_large)