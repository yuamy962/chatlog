1.下载的时候要安装go环境，
2.同时要设置代理，下载依赖包
go env -w GOPROXY=https://mirrors.aliyun.com/goproxy/,direct
go env -w GOPRIVATE=

3. # 清理 Go 模块缓存
go clean -modcache
#拉取依赖
go mod tidy


4. 编译生成可执行文件
go build -o chatlog.exe ./
