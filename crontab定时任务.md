[linux定时任务](https://linuxtools-rst.readthedocs.io/zh_CN/latest/tool/crontab.html)

  crontab -e 编辑

    * * * * *  分别代表分、时、日、月、周

      分 时 日 月 星期 要运行的命令

      第1列分钟0～59
      第2列小时0～23（0表示子夜）
      第3列日1～31
      第4列月1～12
      第5列星期0～7（0和7表示星期天）
      第6列要运行的命令
