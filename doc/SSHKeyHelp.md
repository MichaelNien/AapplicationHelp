# SSHKeyHelp

### Windows 10 指令產生 OpenSSH Kay

```
ssh-keygen -t ed25519
```

產生 C:\Users\帳號名稱\\.ssh\ 公私鑰

- (私鑰)id_ed25519


- (公鑰)id_ed25519.pub


### 轉換私鑰格式

使用 puttygen.exe 版本(Release 0.76)

load id_ed25519 私鑰

Save Private .ppk 格式 v2 版本的

使用 pageant.exe 版本(Release 0.70.2-Sourcetree) 載入 id_ed25519.ppk

### 參考

設定輸出 v2版本 .ppk 格式 Key

https://blog.csdn.net/gfluozhitao/article/details/118053900

指令產生 SSH Key (OpenSSH格式)

https://docs.microsoft.com/zh-tw/windows-server/administration/openssh/openssh_keymanagement