CFLAGS = -Wall -Wextra

# 每次执行make都会可编译
# all规则 未编译时 make 可以编译 已经编译完成 make执行后提示没有可编译的
# .PHONY: all
all:main

# run 依赖 main 所以可以不写main
# run 会编译也会执行 当有可执行文件 则不再编译 直接执行
# .PHONY: run
run: main
	./main

# $(RM) main 可以替换 rm -rf
# make 执行clean是需要执行clean下面的命令
# 如果有同名的文件clean,则需要用 .PHONY: clean 标记上
# .PHONY: clean
clean:
	$(RM) main

.PHONY: all run clean
