1、WDigest:  
```
HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\SecurityProviders\WDigest  
Negotiate --> 0  
UseLogonCredential --> 0  
```

2、lsass保护
```
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Lsa
新建DWORD(32位)(值D) RunAsPPL --> 1
```

3、禁止调试程序
```
secpol.msc或者gpedit.msc
本地策略--用户权限分配--调试程序--删除用户
```