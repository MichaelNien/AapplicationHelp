# SSHKeyHelp

Windows 10 指令產生 OPEN SSH

```
ssh-keygen -t ed25519
```

產生

id_ed25519 私鑰

id_ed25519.pub 公鑰



使用 puttygen.exe 版本(Release 0.76)

load id_ed25519 私鑰

Save Private .ppk 格式 v2 版本的



使用 pageant.exe 版本(Release 0.70.2-Sourcetree) 載入 id_ed25519.ppk



參考

設定輸出 v2版本 .ppk 格式 Key

https://blog.csdn.net/gfluozhitao/article/details/118053900

指令產生 SSH Key (OPEN SSH 格式)

https://docs.microsoft.com/zh-tw/windows-server/administration/openssh/openssh_keymanagement