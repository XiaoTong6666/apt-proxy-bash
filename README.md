# apt-proxy-bash
apt-proxy是bash脚本
如果你没/etc/apt/apt.conf.d/proxy.conf配置文件，会给你造
造了配置文件但没东西。所以，会提示输入你的HTTP(S)代理地址，例如http://127.0.0.1:10809/
输入: http://127.0.0.1:10809/之后
   
就会输出你APT代理的配置文件
Acquire::http::Proxy "http://127.0.0.1:10809/";
Acquire::https::Proxy "http://127.0.0.1:10809/";
   
该脚本用法: apt-proxy [-s] [-c]
-s 代理！启动！
-c 代理...关闭...

