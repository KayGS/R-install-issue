——问题描述——

在使用Rstudio安装包psych时，会出现Warning in install.packages :dependency ‘mnormt’ is not available这一警告，调用psych后发现 不存在叫‘mnormt’这个名字的程辑包。若继续使用install.packages("mnormt")，发现包无法被安装。

——解决方案——

在cran官网https://cran.r-project.org/中分别搜索下载包mnormt、tmvnsim至电脑硬盘某一路径，而后使用R studio面板的Tools，使用install.packages...安装下载好的包，然后在代码行执行install.packages("psych")。问题可解决。

——其他问题——

使用临时目录
将包下载到一个临时目录中，该目录不包含非ASCII字符，然后从该目录进行安装。

下载包文件
访问CRAN网站的 psych 包页面：psych包下载页面 下载 psych 和 mnormt 包的源文件（.tar.gz 文件）。

创建临时目录
创建一个不包含非ASCII字符的临时目录，比如 C:/temp/。

将下载的包文件移动到临时目录
将下载的 .tar.gz 文件移动到 C:/temp/ 目录。
