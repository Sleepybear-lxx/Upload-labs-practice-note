# Upload-labs-practice-note
记录练习Upload-labs文件上传靶场的思路和方法


# 更新日志
* V1.0 2022/05/11
  * 上传 Pass01-04思路
  * 上传 Pass06-19思路
* V1.1 2022/05/15
  * 上传 Pass20思路

# 完成情况

- [x] Pass-01
- [x] Pass-02
- [x] Pass-03
- [x] Pass-04
- [ ] Pass-05
- [x] Pass-06
- [x] Pass-07
- [x] Pass-08
- [x] Pass-09
- [x] Pass-10
- [x] Pass-11
- [x] Pass-12
- [x] Pass-13
- [x] Pass-14
- [x] Pass-15
- [x] Pass-16
- [x] Pass-17
- [x] Pass-18
- [ ] Pass-19
- [X] Pass-20
- [ ] Pass-21


# 存在问题
## Pass-03
在真实ubuntu中测试发现，即使没有开启phtml解析项，phtml也按照php来解析。目前原因未知。
## Pass-06
在真实ubuntu中测试发现，上传大写PHP后缀文件，可以正常访问，但无法解析，代码被当作注释未执行（解析为html）。目前原因未知。
![image](https://github.com/Sleepybear-lxx/Upload-labs-practice-note/blob/main/images/Pass-06.png)
## Pass-07
在真实ubuntu中测试发现，上传“test.php.”文件，可以正常访问，但无法解析，代码被当作注释未执行（解析为html）。目前原因未知。
## Pass-17
本关卡也调用了move_uploaded_file($tmpname,$target_path)函数，之后又重新生成图片。猜想此处也可通过二次竞争，生成webshell。
## Pass-19
未过关


# 解决问题
## 暂无
