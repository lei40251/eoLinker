**这是修改后的版本**
- 语言换成中文
- 修复登录页“用户名”显示不正确，placeholder错误导致登录页“用户名”显示为“undefined”
- 修复接口编辑页点击“更多设置”按钮报错，三元表达式和国际化组合使用时的代码有误导致弹窗无法渲染
- 修复未在cacheJson中存储apiNote及相关字段的信息，apiNote及相关字段的信息被保存在了api表中，但未保存到apiCache表中
- 注释掉对未定义的方法的调用
- 修复无法保存接口，后端未返回必须的字段，没有做兼容导致无法保存（本修复是不必要的，只要后端返回了这三个字段就好了）