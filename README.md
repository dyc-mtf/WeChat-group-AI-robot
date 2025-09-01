# WeChat-group-AI-robot
WeChat Group Auto-Reply Robot Implemented by Calling the DeepSeek API
通过调用deepseekAPI实现的微信群自动回复机器人

# User Manual (使用须知)
## I. Robot Information Section (Robot_Data)
1. You can modify the character setting section (the first part) of the "Robot Information.txt" file in the Robot_Data folder. This includes adjustments to personality, birthday, characteristics, and other basic information. At the end of the file, you can fill in names and a nickname. Multiple names are allowed (remember to label the identity of each name, such as pet name, full name, chat name, etc.). There is only one nickname, which refers to the WeChat name. It is not recommended to modify other sections.
2. You can modify the "Robot Proposed Topics.txt" file in the Robot_Data folder, where you can change the topics proactively proposed by the robot.

---

## II. Configuration Section (Config)
1. You can modify the "Active Sending Start Limit.txt" and "Active Sending End Limit.txt" in the Config folder (enter numbers in them) to change the time range for the robot to propose topics (Distance Time: the time since the robot last sent a message; if the distance time equals a random number within the range of the numbers in the two files, the robot will proactively propose a topic. The topic can be changed, see above).
2. You can modify the "Emoticon Sending Start Limit.txt" and "Emoticon Sending End Limit.txt" in the Config folder (enter numbers in them) to change the frequency of the robot sending emoticons (Distance Message Count: the number of message intervals since the last emoticon was sent, i.e., how many messages are there between the two; if the distance message count equals a random number within the range of the numbers in the two files, an emoticon will be sent).
3. You can modify the "Whether to Proactively Propose Topics.txt" in the Config folder. Enter "True" or "False" to indicate whether you want to enable the function of the robot proactively proposing topics.

---

## III. API Key Section (ApiKey_Data)
1. You must enter your own obtained deepseek_api_key in the "AI_api_key.txt" file. If you enter an incorrect api_key or do not enter one (initially empty), the robot will not work properly.

### Acquisition Tutorial:
1. Visit the deepseek official website: https://www.deepseek.com/
2. Click the button at the top: "API Open Platform ↗". After entering, register an account if you don’t have one, or log in directly if you have an account.
3. Click the "API keys" option in the left-side list.
4. After entering the page, click the "Create API key" button. Enter the name of the api key and then click "Create". After obtaining the api key, you must copy it in a timely manner, as you will not be able to find the api key later (deepseek will not provide it again after creation to avoid api key leakage; if you forget it, you can create a new one).
5. Copy the api key into the "AI_api_key.txt" file in the ApiKey_Data folder.
6. Recharge: API calls incur costs, but the cost is very low. Even with heavy usage, the maximum cost per day is only 0.1 yuan. Click "Recharge" in the list, select online payment, choose the payment method and the amount to pay (the amount can be customized), and complete the payment.



# 使用须知
## 一、机器人信息部分（Robot_Data）
1. 您可以修改Robot_Data文件夹中“Robot Information.txt”文件的角色设置部分（第一部分），包括调整性格、生日、特点等基础信息。在该文件末尾，您可填写姓名及一个昵称。姓名可填写多个（需标注每个姓名的身份，如小名、全名、聊天用名等）。昵称仅有一个，指微信名称。不建议修改其他部分。
2. 您可以修改Robot_Data文件夹中的“Robot Proposed Topics.txt”文件，在该文件中可更改机器人主动发起的话题。


---


## 二、配置部分（Config）
1. 您可以修改Config文件夹中的“Active Sending Start Limit.txt”和“Active Sending End Limit.txt”（在文件内输入数字），以更改机器人发起话题的时间范围（间隔时间：自机器人上次发送消息起算的时间；若间隔时间等于上述两个文件内数字范围中的任意一个随机数，机器人将主动发起话题。话题可按上文所述方法修改）。
2. 您可以修改Config文件夹中的“Emoticon Sending Start Limit.txt”和“Emoticon Sending End Limit.txt”（在文件内输入数字），以更改机器人发送表情的频率（消息间隔数：自上次发送表情起算的消息间隔数量，即两条表情消息之间有多少条其他消息；若消息间隔数等于上述两个文件内数字范围中的任意一个随机数，机器人将发送表情）。
3. 您可以修改Config文件夹中的“Whether to Proactively Propose Topics.txt”文件，输入“True”（开启）或“False”（关闭），以设置是否启用机器人主动发起话题的功能。

---

## 三、API密钥部分（ApiKey_Data）
1. 您必须在“AI_api_key.txt”文件中输入自行获取的deepseek_api_key。若输入的api_key有误或未输入（初始状态为空），机器人将无法正常运行。

### 获取教程：
1. 访问deepseek官方网站：https://www.deepseek.com/
2. 点击顶部的“API开放平台 ↗”按钮。进入页面后，若未注册账号请先注册，若已注册则直接登录。
3. 点击左侧列表中的“API keys”（API密钥）选项。
4. 进入页面后，点击“Create API key”（创建API密钥）按钮。输入API密钥名称，然后点击“Create”（创建）。获取API密钥后，请及时复制保存，因为后续将无法再次查看该API密钥（为防止API密钥泄露，deepseek在创建后不再提供密钥查询服务；若遗忘密钥，可重新创建一个）。
5. 将复制的API密钥粘贴到ApiKey_Data文件夹中的“AI_api_key.txt”文件内。
6. 充值：调用API会产生费用，但费用极低，即便高频使用，每日最高费用也仅0.1元。点击列表中的“Recharge”（充值）选项，选择在线支付，挑选支付方式并设定充值金额（金额可自定义），完成支付即可。
