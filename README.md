# quark-auto-save-plugins

此插件仅适用夸克自动转存：[Cp0204/quark-auto-save](https://github.com/Cp0204/quark-auto-save)

功能为在新资源转存后，对比设定alist的目录中的文件，如果不存在则添加复制任务，实现跨网盘同步

# 使用方法

1.将py文件保存至plugins目录下后重启应用

2.在系统配置中配置url、token、quark_path参数

例：

url：http://127.0.0.1:5244

token:alist-xxxx

quark_path:/Quark/


3.在任务配置的插件选项中填写target_path与verify_path

其中target_path为需要保存的目标路径，如/baidu/save_dir
verify_path为验证目录，如不填写则自动使用target_path,主要用于alist别名的多个目录合并成一个文件夹时使用


## 注意事项：
1.除第二步中的系统配置quark_path需要以/结尾，其他均不以/结尾

2.在保存至夸克网盘的文件中，需保持文件名格式为：电视剧名称.S01E01.MKV
