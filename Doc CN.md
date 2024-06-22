# 智绘AI客服技术文档
基于生成式AI的物流客服解决方案

本解决方案旨在使用生成式AI提高对用户请求的理解能力，并通过知识库搜索，训练，提示词工程，让AI客服可以按照预期回复用户，解决用户需求。
考虑到目前大模型的社区生态，使用python + Django + MongoDB 构建后端,并提供通用接口。 前端计划使用React + tailwind构建响应式用户界面Demo + 后台管理Demo， 如果时间充足，可以额外制作一个微信小程序demo用于演示。
## 1. 系统架构
### 1.1 总体架构
![系统设计 drawio (1)](https://github.com/Nilyang404/SFX-Contest-AI-Agent/assets/63556313/a81645fd-f91a-4663-9b2e-2c41dde59060)

### 1.2 后端

![后端架构设计 drawio (2)](https://github.com/Nilyang404/SFX-Contest-AI-Agent/assets/63556313/7b5eeddd-f729-4659-8588-387273b68c42)

### 1.3 前端

![前端架构 drawio (1)](https://github.com/Nilyang404/SFX-Contest-AI-Agent/assets/63556313/ac80dfd2-344a-4a6e-83b0-64e6b468e54e)

## 2. 用户体验设计

### 2.1 用户故事

#### 2.1.1 客户
1. 作为用户，我希望能够通过文字或语音描述，查询我的物流订单信息，费用，或是处理退款
2. 作为用户，我希望我能够拍照上传图片，用来辅助说明我的需求
3. 作为用户，我希望即使我的表述有一些错别字，方言，或者语序错误，客服也可以理解我的需求
4. 作为用户，我希望客服能够更加智能。即使比较复杂的需求，客服也可以理解我的意图
5. 作为用户，我希望当我感到焦虑，着急的时候客服可以安抚我的情绪而不是冷冰冰的机械式回复。
6. 作为用户，当AI客服无法满足我的需求是，我应该可以要求人工客服提供服务

#### 2.1.2 人工客服
1. 作为客服，我希望能够更新AI客服的知识库，以便满足最新的服务需求
2. 作为客服，我希望能够在AI客服无法解决问题的时候主动或被动介入对话
3. 作为客服，我需要保障AI客服不被滥用，有一定的防注入或消息轰炸机制

### 2.2 产品流程图
![image](https://github.com/Nilyang404/SFX-Contest-AI-Agent/assets/63556313/14b11284-ed3c-4671-8879-8a152e35bb42)

### 2.3 Demo UI 设计
![TC`29(ZVP%Z8~NDET@CYE1O](https://github.com/Nilyang404/SFX-Contest-AI-Agent/assets/63556313/3b2f64e7-7b7a-40f5-8f00-f95fd55a4dc1)
![~49~14_TG NJ%D4@P_S}S}G](https://github.com/Nilyang404/SFX-Contest-AI-Agent/assets/63556313/a749a3b7-522a-4271-bfad-b21ec3e5323d)

## 2. 算法设计
![Uml drawio](https://github.com/Nilyang404/SFX-Contest-AI-Agent/assets/63556313/4aa374a8-a549-495b-aab6-ec1327cdcfd8)

## 3. 数据流程

![数据流程 drawio](https://github.com/Nilyang404/SFX-Contest-AI-Agent/assets/63556313/5b846283-d5a1-43ba-b45a-2bc75dc9f965)

