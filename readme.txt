哈哈
Git is a version control system.
Git is free software.
第一次修改

更换git本地用户名为tyn_cc后提交一次试试看 ：结果显示提交的用户名并没有变化，跟网站上的用户名保持一致还是Tonytyn

然后我再换一个邮箱tongyannan5@sina.com.cn试试 结果用户名改变了，变成了tyn_cc。

原来github是根据邮箱来判断用户名的，如果使用git推送时如果user.email跟网站上的是一样的，那后台显示的就是网站上的用户名。这时候git本地用户名user.name没什么用。但是如果提交代码的user.email与网站上不一样，则会显示git本地提交时提供的用户名和邮箱

github绑定的ssh公钥是针对于电脑来说的，并不是用户。也就是说只要电脑的公钥在github网站的公钥列表里，这台电脑就能提交代码到相应的仓库


刚才又试了试把邮箱改成一个不存在的邮箱