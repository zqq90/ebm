Engine Benchmark
==============
> 目前网络上的Java模板引擎测试基本上都是非独立JVM测试的，
  这样做后测试的引擎性能会较高，与实际性能相比有较大偏差，
  因此本测试对每个引擎都使用独立JVM测试，保证了各个引擎间环境的公平性；

使用
==============
### 1.编译
<code>mvn clean install</code>

### 2.修改参数
+ /target/classes/benchmark.bat
+ /target/classes/benchmark.properties

### 3.运行
+ Windows 下执行
<code>/target/classes/benchmark.bat</code>
+ Linux暂未支持


测试结果：
==============
~~~~~
JVM     : Windows Oracle JDK7u45(32位)
JVM参数 : -server -Xms128m -XX:PermSize=32m
预热    : 1000
渲染次数: 200000
数据深度: 50
输出编码: UTF-8
~~~~~
![report.png](report_jdk7.png)
~~~~~
JVM: Windows Oracle JDK6u37(32位)
~~~~~
![report.png](report_jdk6.png)


参考资料
==============
> 交流QQ群：109365467

> 引擎参考：
  * BSL
    * 项目主页：http://boilit.github.io/bsl
    * 项目仓库：https://github.com/boilit/bsl
  * Webit-Script
    * 项目主页：http://zqq90.github.io/webit-script
    * 项目仓库：https://github.com/zqq90/webit-script
  * JetBrick-Template
    * 项目主页：http://subchen.github.io/jetbrick-template
    * 项目地址：https://github.com/subchen/jetbrick-template
  * HTTL
    * 项目主页：http://httl.github.io
    * 项目仓库：https://github.com/httl/httl
  * Beetl
    * 项目主页：http://ibeetl.com/
  * Rythm
    * 项目主页：http://rythmengine.org
  * Velocity
    * 项目主页：http://velocity.apache.org
  * FreeMarker
    * 项目主页：http://freemarker.org

软件作者
==============
> 软件作者：Boilit
> 作者姓名：于景洋
> 所在单位：胜利油田胜利软件有限责任公司

Contributors：
==============
* zqq90：https://github.com/zqq90/ebm
* subchen：https://github.com/subchen/ebm
* Septembers：https://github.com/Septembers/ebm

License(许可证)
==============
> Template Engine Benchmark Test is released under the MIT License. 
  See the bundled LICENSE file for details.
> Template Engine Benchmark Test 依据MIT许可证发布。
  详细请看捆绑的LICENSE文件。
