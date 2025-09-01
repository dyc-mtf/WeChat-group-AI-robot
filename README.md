# WeChat-group-AI-robot
WeChat Group Auto-Reply Robot Implemented by Calling the DeepSeek API

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
