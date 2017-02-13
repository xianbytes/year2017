ie在国内市场的份额是越来越低，但是在国企或者传统部门pc上依然用的ie浏览器，并存在一定的用户量。然而对于如今的前端开发，ie就是噩梦，

因为种种不兼容性，会导致你崩溃。所以一些公司便会采用谷歌插件模式，来解决这类问题。

1、设置html头文件meta元素可提供有关页面的元信息


 <meta http-equiv="X-UA-Compatible" content="IE=10,chrome=1">
 
 
 2、判断浏览器内核
 
   checkIEVersionFlag: function() {
            return (navigator.userAgent.indexOf("MSIE 9.0") >= 0 || navigator.userAgent.indexOf("MSIE 8.0") >= 0 || navigator.userAgent.indexOf("MSIE 7.0") >= 0 || navigator.userAgent.indexOf("MSIE 6.0") >= 0);
        },
        
3、下载软件

downloadPlugins: function() {
            var playerEXE = "../xxgoogle.exe";
            window.location.href = playerEXE;
           
        }

4、ok
