# Mac配置环境变量的地方:
1.~/.profile （建议不修改这个文件 ）
全局（公有）配置，不管是哪个用户，登录时都会读取该文件。

2.~/.bashrc （一般在这个文件中添加系统级环境变量）
全局（公有）配置，bash shell执行时，不管是何种方式，都会读取此文件。

3.~/.bash_profile （一般在这个文件中添加用户级环境变量）
每个用户都可使用该文件输入专用于自己使用的shell信息,当用户登录时,该文件仅仅执行一次!
背景：比如我在.bash_profile中设置了别名ll,每次都需要重新使用source .bash_profile才能生效。

原因：在 ~/.bash_profile 中配置环境变量, 可是每次重启终端后配置的不生效.需要重新执行 : $source ~/.bash_profile
zsh加载的是 ~/.zshrc文件，而 ‘.zshrc’ 文件中并没有定义任务环境变量。

解决办法：在.zshrc里面添加一行source .bash_profile
注意：如果mac上没有安装.zshrc或.bash_profile文件，需要手动添加!
