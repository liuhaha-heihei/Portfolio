# 塔罗万事屋
## 一、链接
https://www.coze.cn/s/Bu3IaaojoFw/
## 二、简介
一款基于用户星盘和抽取的塔罗牌进行运势预测的智能体

<img width="400" height="350" alt="image" src="https://github.com/user-attachments/assets/b468ec33-41d3-4ead-918b-0091492321b4" />

## 三、实现路径
1. 设计逻辑
   <img width="3000" height="1680" alt="根据图进行美化(1)" src="https://github.com/user-attachments/assets/920c84a3-d50c-4b45-a890-d806b4fa621a" />

3. 工作流

   <img width="2648" height="1201" alt="image" src="https://github.com/user-attachments/assets/973d8570-09a4-42e7-b670-0a1b8afc2cbf" />

## 四、代码
### 用于拆分用户提供的城市名的经度和纬度，以供后续星盘的测算

async def main(args: Args) -> Output:
    params = args.params
    # 构建输出对象
    ret: Output = {
        "latitude": params['input'][0],
        "longitude": params['input'][1],
    }
    return ret
