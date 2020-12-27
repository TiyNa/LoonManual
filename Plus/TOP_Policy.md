# 正确分辨母策略组和子策略组

正确识别 `母策略组` ，对于理解 `俄罗斯套娃` 的逻辑会有很大的帮助

## 方法

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 其实 `母策略组` 非常容易辨认，打开 Loon 点击下方 `配置` 栏，点击 `订阅规则`

![image](https://raw.githubusercontent.com/TiyNa/LoonManualimg/main/Plus/TOP_Policy_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 查看每个订阅的规则左下角蓝色字体的名称，除 `DIRECT` 和 `REJECT` 的名称外，剩下名称的策略组就为 `母策略组`

![image](https://raw.githubusercontent.com/TiyNa/LoonManualimg/main/Plus/TOP_Policy_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 点击下方 `配置` 栏，点击 `策略组`

![image](https://raw.githubusercontent.com/TiyNa/LoonManualimg/main/Plus/Proxy_Group.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 查看名称为 `𝐏𝐫𝐨𝐱𝐲` 的母策略组，可以看到 `𝐏𝐫𝐨𝐱𝐲` 的母策略组下有 `手动选择`、`优选低延迟`、`健康检测` 三个子策略组

![image](https://raw.githubusercontent.com/TiyNa/LoonManualimg/main/Plus/TOP_Policy_3.jpg)

# 多说几句

- 除 `DIRECT` 和 `REJECT` 的外的原因是： Loon 已经内置了 `DIRECT` 和 `REJECT` 策略组，因而在 `策略组` 面板中不可能出现名称为 `DIRECT` 或 `REJECT` 策略组

- 可以出现名称为特殊字体的 `DIRECT` 或 `REJECT` 策略组，例如名称为 `𝐃𝐈𝐑𝐄𝐂𝐓` 的策略组

- `订阅规则` 选择的策略组只能是 `母策略组` ，不可能是 `子策略组` ，但除该 `母策略组` 嵌套在其他 `母策略组` 内成为 `子策略组` 的情况外
