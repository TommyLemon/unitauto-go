# unitauto-go 
UnitAuto Go 库，可通过 GitHub 仓库等远程依赖。<br />
UnitAuto Go Library for remote dependencies with GitHub repo, etc.

<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225639582-76f8cf99-d603-4d93-ae19-77b9fd278a42.png">

同步纯函数：<br />
Sync pure function: <br />
https://github.com/TommyLemon/unitauto-go/blob/main/unitauto/test/test_util.go#L25-L27
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225637162-779e64ee-46f8-41a0-b91a-c0e66d291398.png">

struct 成员函数：<br />
strcut member function: <br />
https://github.com/TommyLemon/unitauto-go/blob/main/unitauto/test/test_util.go#L88-L90
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225635650-f776dc3a-596c-4796-95d7-1ca1c2f02782.png">
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225635800-5909dfb7-17c1-45e2-94e5-7c2251aa4500.png">

协程异步函数：<br />
goroutine function: <br />
https://github.com/TommyLemon/unitauto-go/blob/main/unitauto/test/test_util.go#L33-L45
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225636134-a4daf4ec-9304-44d2-b09a-28497c815188.png">

异步回调函数：<br />
async callback function: <br />
https://github.com/TommyLemon/unitauto-go/blob/main/unitauto/test/test_util.go#L72-L81
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225636569-b508fa19-3973-4655-bd49-68742c4d09d0.png">

<br />

代码覆盖率统计：<br />
Code coverage: <br />
https://github.com/qiniu/goc/issues/349
<img width="1495" alt="image" src="https://github.com/qiniu/goc/assets/5738175/77ed49f9-aa18-4cc9-82b8-31b7cba107b7">
<img width="1495" alt="image" src="https://github.com/qiniu/goc/assets/5738175/07a8c278-980f-4b4f-96c4-df96f4f26a17">

<br />

**Demo:** https://github.com/TommyLemon/unitauto-go-demo

<br />

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

#### 3. 启动单元测试服务
#### 3. Start unit testing server
https://github.com/TommyLemon/unitauto-go/blob/main/main.go#L7-L12
```go
func main() {
	unitauto.Start(8082)
}
```

<br />

#### 4. 参考主项目文档来测试
#### 4. Test by following the main repo

https://github.com/TommyLemon/UnitAuto

由于 Go 的反射限制，目前做不到像 Java, Kotlin 版几乎绝对零代码，还需要注册 func 和 struct 的实例，<br />
不过注册代码可以通过 UnitAuto-Admin 前端管理网页设置项 \[查看、同步方法文档] 来生成，复制粘贴到被测项目中：<br />
Due to the limitation of Go, it's not almost absolutely coding free like Java and Kotlin, <br />
and you need to write few code to register the funcs and structs to be tested. <br />
However, the code can be generated by clicking the setting item [View/Sync doc] of UnitAuto-Admin, <br />
then you can copy and pasted the "ginCode" into the project under test instead of coding: <br />

https://github.com/TommyLemon/unitauto-go/blob/main/main.go
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225632360-ce953a58-22b1-4b4e-8b3d-0083edebc71a.png">
<img width="1495" alt="image" src="https://user-images.githubusercontent.com/5738175/225635146-f8dab9d1-76c5-421a-b45e-732e4923fd4d.png">

<br />

### 5. 关于作者
### 5. Author
[https://github.com/TommyLemon](https://github.com/TommyLemon) <br />
<img width="1280" src="https://github.com/TommyLemon/UIGO/assets/5738175/ec77df98-ff9b-43aa-b2f1-2fce2549d276">

如果有什么问题或建议可以 [去 APIAuto 提 issue](https://github.com/TommyLemon/APIAuto/issues)，交流技术，分享经验。<br >
如果你解决了某些 bug，或者新增了一些功能，欢迎 [提 PR 贡献代码](https://github.com/Tencent/APIJSON/blob/master/CONTRIBUTING.md)，感激不尽。
<br />
If you have any questions or suggestions, you can [create an issue](https://github.com/TommyLemon/APIAuto/issues). <br >
If you can added a feature or fixed a bug, please [create a pull request](https://github.com/TommyLemon/unitauto-go/pulls), thank you~


### 6. 其它项目
### 6. Link
创作不易、坚持更难，右上角点 ⭐ Star 支持下吧，谢谢 ^\_^ <br />
Please ⭐ Star the repos that you like ^\_^ <br />

[UnitAuto](https://github.com/TommyLemon/UnitAuto) 机器学习零代码单元测试平台，零代码、全方位、自动化 测试 方法/函数 的正确性、可用性和性能

[unitauto-go-demo](https://github.com/TommyLemon/unitauto-go-demo) UnitAuto Go Demo，提供用来做单元测试的业务函数

[unitauto-py](https://github.com/TommyLemon/unitauto-py) UnitAuto Python 库，可通过 pip 仓库等远程依赖

[APIJSON](https://github.com/Tencent/APIJSON) 🚀 腾讯零代码、全功能、强安全 ORM 库 🏆 后端接口和文档零代码，前端(客户端) 定制返回 JSON 的数据和结构

[apijson-go](https://github.com/glennliao/apijson-go) Go 版 APIJSON， 基于Go(>=1.18) + GoFrame2, 支持查询、单表增删改、权限管理等

[APIAuto](https://github.com/TommyLemon/APIAuto) 敏捷开发最强大易用的 HTTP 接口工具，机器学习零代码测试、生成代码与静态检查、生成文档与光标悬浮注释，集 文档、测试、Mock、调试、管理 于一体的一站式体验

[SQLAuto](https://github.com/TommyLemon/SQLAuto) 智能零代码自动化测试 SQL 语句执行结果的数据库工具，任意增删改查、任意 SQL 模板变量、一键批量生成参数组合、快速构造大量测试数据

[UIGO](https://github.com/TommyLemon/UIGO) 📱 零代码快准稳 UI 智能录制回放平台 🚀 自动兼容任意宽高比分辨率屏幕，自动精准等待网络请求，录制回放快、准、稳！
