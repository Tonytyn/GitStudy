git学习心得：
1.关于用户名和邮箱：
	1）git本地可以设置global user.name和user.email ，也可以根据不同项目设置不同的user.name&user.email，一般我们设置一个全局的就行了。
	
	2）git向远程仓库push文件时可以使用任意用户名和邮箱。只要这台电脑上的公钥在网站的公钥列表里就可以向远程仓库推送代码。
	
	3）如果提交时使用的user.email是跟网站注册时使用的一样的邮箱,则提交人显示的是网站上的用户名（即使本地user.name与远程不一样）。比如:
		本地账户名为:user.name = 张三 user.email = zhangsan@123.com
		github用户名为：张三丰  email = zhangsan@123.com
		这时从客户端提交到远程仓库后贡献者的名字是张三丰而不是张三，因为github通过邮箱判断这个用户就是本仓库的拥有者，所以直接显示了网站上的用户名

	4）如果push时的user.email与远程网站注册时不一致，则提交人显示此时的本地user.name和user.email，比如：
		本地账户名还是:user.name = 张三 user.email = zhangsan@123.com
		gitee用户名为：李四 email = lisi@123.com
		这时从客户端提交到远程仓库后贡献者的名字就是张三。因为gitee看到这个邮箱（zhangsan@123.com）后判断这不是本仓库的拥有者，是一个其他人，所以就把本地提交的用户名作为贡献者名字

