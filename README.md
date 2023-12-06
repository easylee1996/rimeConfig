基础配置文件使用的是: https://github.com/iDvel/rime-ice

常用配置文件为 squirrel.yaml 和 default.yaml

在其中修改了

配置 vim 中英文切换

```yaml
# 特定App默认中/英文输入 配置vim的中英文切换
app_options:
  com.apple.Spotlight: # 聚焦搜索
    ascii_mode: true # true默认英文,false默认中文
  com.runningwithcrayons.Alfred: # alfred
    ascii_mode: true
  com.apple.Terminal: # 终端
    ascii_mode: true
    vim_mode: true
  com.microsoft.VSCode: # Visual Studio Code
    ascii_mode: true
    ascii_punct: true # 中文状态输出英文标点(半角)
    vim_mode: true
  com.googlecode.iterm2: # iterm2
    ascii_mode: true
    vim_mode: true
  md.obsidian: # obsidian
    ascii_mode: true
    vim_mode: true
```

关闭了 emoji 的建议,方法为直接删除了 opencc 文件夹

隐藏候选词序号,让候选词可以居中,在皮肤的位置进行设置即可

```yaml
label_font_point: 1 # 候选词序号字体大小,设置为1,是为了屏蔽候选词序号,让候选词居中,目前没找到直接隐藏的开关
```
