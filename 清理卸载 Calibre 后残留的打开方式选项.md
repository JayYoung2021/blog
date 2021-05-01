清理卸载 Calibre 后残留的打开方式选项

> 如何彻底卸载Calibre？ - 知乎用户的回答 - 知乎 https://www.zhihu.com/question/317696903/answer/935723858

```powershell
for /f %a in ('reg query HKEY_CLASSES_ROOT /f calibre /k') do reg delete %a /f
```