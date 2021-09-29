# auto_baoqin
自动报寝系统
# 部署方法
建议在云服务器上部署，以保证长期24小时运行。
# 依赖

```
pip install -r requirements.txt
```
# 配置
1. 在config.yml中配置：
```
uin:  # QQ账号
password: '' # 密码为空时使用扫码登录
```

2. 在rob2>src>test.py中配置

```
async def dy_sched():
    bot = nonebot.get_bots()['你的QQ号']
    print(bot)
    return await bot.call_api('send_group_msg', **{
        'message': 'XXX校内在寝',
        'group_id': '群号'
    })
```
# 运行
```python
cd rob2
nohup python bot.py &
cd ..
nohup ./go-cqhttp &
```

