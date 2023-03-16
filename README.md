# unitauto-go 
UnitAuto Go 库，可通过 GitHub 仓库等远程依赖。<br />
UnitAuto Go Library for remote dependencies with GitHub repo, etc.

<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225639582-76f8cf99-d603-4d93-ae19-77b9fd278a42.png">
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225637162-779e64ee-46f8-41a0-b91a-c0e66d291398.png">
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225635650-f776dc3a-596c-4796-95d7-1ca1c2f02782.png">
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225635800-5909dfb7-17c1-45e2-94e5-7c2251aa4500.png">
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225636134-a4daf4ec-9304-44d2-b09a-28497c815188.png">
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225636569-b508fa19-3973-4655-bd49-68742c4d09d0.png">
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225632360-ce953a58-22b1-4b4e-8b3d-0083edebc71a.png">

#### 1. 在 go.mod 中添加 GitHub 仓库
#### 1. Add the GitHub repository to go.mod
```go
	require (
		github.com/TommyLemon/unitauto-go v1.0.0
	)
```
<br />

#### 2. 执行 go get 命令
#### 2. Run go get command
```sh
	go get github.com/TommyLemon/unitauto-go@v1.0.0
```

<br />

#### 3. 参考主项目文档来测试
#### 3. Test by following the main repo

https://github.com/TommyLemon/UnitAuto

由于 Go 的反射限制，目前做不到像 Java, Kotlin 版几乎绝对零代码，还需要注册 func 和 struct 的实例，<br />
不过注册代码可以通过 UnitAuto-Admin 前端管理网页设置项 \[查看、同步方法文档] 来生成，复制粘贴到被测项目中：
https://github.com/TommyLemon/unitauto-go/blob/main/main.go
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225632360-ce953a58-22b1-4b4e-8b3d-0083edebc71a.png">
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225635146-f8dab9d1-76c5-421a-b45e-732e4923fd4d.png">

