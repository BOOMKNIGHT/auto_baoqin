# auto_baoqin
自动报寝系统
# 部署方法
建议在云服务器上部署，以保证长期24小时运行。
# 依赖
# 配置
1. 在config.yml中配置：
![image](https://user-images.githubusercontent.com/54172108/135284410-a709b35e-1d03-4fa9-890f-3dc88cdfef56.png)
2. 在rob2>src>test.py中配置
![image](https://user-images.githubusercontent.com/54172108/135284539-af1df7da-f178-401e-9cb2-0f5c9feb70df.png)
# 运行
'''
cd rob2
nohup python bot.py &
cd ..
nohup ./go-cqhttp &
'''

