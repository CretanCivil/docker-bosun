# docker-bosun

## tscenter

代理分发服务器，当探针上报数据时候，一份发给ci，一份发给datadog后台

## tsdbrelay

跟官方的没什么差距

## bosun

进行了改造，redis进行metric信息汇总，官方bosun是不对用户区分的，我进行了区分。
配置文件bosun.toml我把anno，tsdb全部关闭了。因为我只要他的metric整理部分。