複製文件到rime用戶目錄，然後重新部署&同步用戶資料

```
~/.config/ibus/rime  (Linux)
~/Library/Rime  (Mac OS)
%APPDATA%\Rime  (Windows)
```

文件說明：

```
default.custom.yaml: 自定義的全局配置
方案名.schema.yaml：輸入方案的默認配置文件
方案名.custom.yaml: 自定義方案配置文件
方案名.dict.yaml: 詞典文件
symbols.custom.yaml: 符號設置
installation.yaml: 安裝時自動創建的配置文件
```

輸入方案：

```
朙月拼音	luna_pinyin
朙月拼音·简化字	luna_pinyin_simp
朙月拼音·臺灣正體	luna_pinyin_tw
朙月拼音·語句流  luna_pinyin_fluency
自然碼雙拼	 double_pinyin
智能ABC雙拼  double_pinyin_abc
小鶴雙拼  double_pinyin_flypy
MSPY雙拼  double_pinyin_mspy
```

快捷鍵：

```
Ctrl + ` or F4  # 打卡設置菜單
Ctrl + .        # 切換標點符號
Ctrl + Delete   # 刪除用戶詞條
```

安裝插件：

```
# 下載 plum
curl -fsSL https://git.io/rime-install | bash

# 安裝Emoji https://github.com/rime/rime-emoji
bash plum/rime-install emoji

# 配置到對應的輸入法
bash plum/rime-install emoji:customize:schema=luna_pinyin
```

Rime配置粵語：
Mac：

```
curl -fsSL https://git.io/rime-install | bash -s -- cantonese emoji sgalal/rime-opencc-latest custom:set:config=default,key=installed_from,value=rime-cantonese custom:add:schema=jyut6ping3 lotem/rime-octagram-data lotem/rime-octagram-data@hant lotem/rime-octagram-data:customize:schema=jyut6ping3,model=hant
```

Windows：

https://github.com/rime/rime-cantonese/wiki/Windows-%E5%AE%89%E8%A3%9D%E6%95%99%E7%A8%8B

更多粵語配置：

https://github.com/rime/rime-cantonese/releases



鳴謝：

https://github.com/jayknoxqu/ibus-rime
https://github.com/rime/rime-cantonese/

