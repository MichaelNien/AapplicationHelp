# SSHKeyHelp

### Windows 10/11 指令產生 OpenSSH Kay

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

Source Tree 連接SSH出錯

```
git -c diff.mnemonicprefix=false -c core.quotepath=false --no-optional-locks push -v --tags origin master:master
Pushing to github.com:MichaelNien/ElectronicPaymentInstitutions.git
The server's host key is not cached. You have no guarantee
that the server is the computer you think it is.
The server's ssh-ed25519 key fingerprint is:
ssh-ed25519 255 SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU
If you trust this host, enter "y" to add the key to


Completed with errors, see above.
PuTTY's cache and carry on connecting.
If you want to carry on connecting just once, without
adding the key to the cache, enter "n".
If you do not trust this host, press Return to abandon the
connection.
Store key in cache? (y/n, Return cancels connection, i for more info) fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```

https://blog.jsy.tw/1919/source-tree-ssh-key-github-enterprise/