### pgsql重启失败:
   一般是非正确关闭导致的，正确关闭请用kill -15 pid 或者到数据库目录下执行pg_ctl stop;
   强制关闭可能会导致日志文件出问题。到data目录下切换用户到postgres ```su postgres``` ```pg_resetxlog -f ./```
