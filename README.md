# BUAA_YuKeTang

## 链接

[overdose425/BUAA_YuKeTang: BUAA 雨课堂刷课 (github.com)](https://github.com/overdose425/BUAA_YuKeTang)

## 起因

雨课堂能把一节完整的课截成 N 个片段...刷课刷到心累，遂尝试使用自动刷课 + 自动答题脚本

## 参考

原项目: [heyblackC/yuketangHelper: 大学研究生院雨课堂的脚本仓库，该仓库下的脚本经过小改动后也适用于其他院校的雨课堂网课作业和视频。 (github.com)](https://github.com/heyblackC/yuketangHelper)

## 改动

1. 删除部分不能使用的文件，保留了核心文件
2. 适配 buaa 的 `school_id`
3. 原版本刷课太快，担心被查水表，遂加入刷课后的随机时停

## 使用

1. 登录 buaa 雨课堂[北京航空航天大学研究生院 (yuketang.cn)](https://buaa.yuketang.cn/pro/portal/home/)
2. 查找名为`csrftoken`和`sessionid`的 cookies, (其实也可以找到`school_id`)
![](https://raw.githubusercontent.com/overdose425/ImgStg/main/2022/10/07-18-08-42-2022-10-07-18-08-36-0ef37d6a749ba1e1725e779e379ec1b.png)
3. 更改`videoHelper.py`中 12 和 13 行对应变量值为上述值
4. 运行`videoHelper.py`

## 另外

1. 使用时记得关闭 vpn软件，或设置 `buaa.yuketang.cn` 不使用代理服务器，以免出现网络错误
2. 自动答题油猴脚本[[雨课堂]考试助手 (greasyfork.org)](https://greasyfork.org/zh-CN/scripts/450873-%E8%B6%85%E6%98%9F%E5%AD%A6%E4%B9%A0%E9%80%9A-%E7%BD%91%E8%AF%BE%E5%8F%8A%E8%80%83%E8%AF%95%E5%8A%A9%E6%89%8B-%E7%9F%A5%E5%88%B0%E6%99%BA%E6%85%A7%E6%A0%91-%E7%BD%91%E8%AF%BE%E5%8F%8A%E8%80%83%E8%AF%95%E5%8A%A9%E6%89%8B-%E9%9B%A8%E8%AF%BE%E5%A0%82-%E8%80%83%E8%AF%95%E5%8A%A9%E6%89%8B-%E9%9D%92%E7%89%88-%E8%93%9D%E7%89%88-%E8%81%8C%E6%95%99%E4%BA%91icve-%E6%99%BA%E6%85%A7%E8%81%8C%E6%95%99mooc%E7%AD%94%E9%A2%98%E8%80%83%E8%AF%95%E5%8A%A9%E6%89%8B-%E8%B6%85%E6%98%9F-%E8%80%83%E8%AF%95%E4%B8%93%E7%89%88%E7%AD%94%E9%A2%98%E5%8A%A9%E6%89%8B-%E5%AD%A6%E5%A0%82%E4%BA%914-0-%E7%AD%94%E9%A2%98%E5%8A%A9%E6%89%8B)亲测有效，推荐尝试或在[Greasy Fork - 安全、实用的用户脚本大全](https://greasyfork.org/zh-CN)中自行检索
