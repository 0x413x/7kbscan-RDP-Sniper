
[7kbScan]-RDP-Sniper [铸剑实战靶场内部版] 使用说明
=================================================
本软件仅供测试 请于测试一次后删除
-------------------------------------
![image](https://github.com/7kbstorm/7kbscan-RDP-Sniper/raw/master/pic/1.png)

**使用net4.0框架，为提高效率所以采用了线程池技术，可有效的利用字典同时对多个目标进行多线程弱口令测试 。**    
****调用微软官方类库，使用rdp协议6.1版本 ，并支持NLA (详情请搜索Network Level Authentication） 。**   
**支持对Windows主流版本测试，支持管理员模式登录（可突破远程桌面最大连接数限制） 。**    
**编译后使用工具合并所需类库，使用更清爽。**    
**内置了常见密码字典约200个以供测试。**   

参数说明 从左至右分别是
-------------------------------
**1 IP地址**    
**2 子网掩码 (内置算法通过IP和子网掩码自动计算目标)**    
**3 端口**    
**4 端口扫描线程（初期扫描端口时候的线程数量）**   
**5 同时测试的目标IP数量（同时对几个目标发起测试）**    
**6 每个目标IP的线程数量（对每个目标测试的线程数 这里每个目标设计为单独的线程池 互不影响）**   
**7 超时时间（内网其实可以低些 但推荐默认 因有部分未激活 或桌面启动慢的服务器 在开启桌面时会比正常机器慢 如果超时过低会和机会失之交臂）**    
**8 是否保存端口和登录成功日志（这个没什么说的吧）**   
**9 是否启用管理员模式登录(可突破远程桌面最大连接限制 详情参考 mstsc /admin)**    

![image](https://github.com/7kbstorm/7kbscan-RDP-Sniper/raw/master/pic/2.png)

**不做无用功！当其中一个目标的一个用户密码正确时，会在这个目标上写入标识，并自动跳过这个目标的余下任务。**

![image](https://github.com/7kbstorm/7kbscan-RDP-Sniper/raw/master/pic/3.png)




**结果会自动保存在同目录下txt文件内**

![image](https://github.com/7kbstorm/7kbscan-RDP-Sniper/raw/master/pic/4.png)
