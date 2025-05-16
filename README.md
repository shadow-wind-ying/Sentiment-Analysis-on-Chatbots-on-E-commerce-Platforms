# Sentiment-Analysis-on-Chatbots-on-E-commerce-Platforms

# Main files:

Sentiment and humanization analysis on chatbots.ipynb file: The main files with sentiment analysis, humanization metric and visualization function.

chatbot data zip file: The communication record with each platforms (3 scenario * 4 platforms(Engilish Version (using google translation) 

# 1.Introduction
Chatbots have experienced a significant rise in popularity, becoming essential tools for businesses across various industries and sizes. Their ability to streamline customer service, provide instant support, and enhance user experience has made them integral to modern business operations. Many online shopping platforms use a chatbot to provide their customer service. The service quality represents the attitude of the platforms to customers. High quality customer service is an important factor to satisfy customers, understanding their ability to handle complex emotional and demographic-specific scenarios has become critical.

***Research Objectives***

Quantify chatbots’ ability to recognize and adapt to emotional cues.
Assess linguistic humanization (e.g. lexical diversity, average sentence length)
Compare platform-specific performance when facing different situations.

# 2.Data Collection

I simulated the real transaction on each ecommerce platforms, using different accounts to pretend different user groups. Then, I sent the questions to each chatbots and collected their responses for latter research.

Three hypothetical scenarios were designed to simulate interactions with chatbots under diverse user demographics and emotional contexts. Each scenario targets specific humanization challenges. The Scenario Designing Thinking is as follows:

Scenario 1: A boy secretly uses his parent’s account to make a purchase. The mother later criticizes the chatbot for enabling the transaction. Tests the chatbot’s ability to handle accusations and de-escalate conflict.

(1) Age and Responsibility Conflict: Test the chatbot's ability to identify usage permissions for minors (e.g., through language patterns or purchasing behavior to infer user age) and define the platform's responsibility boundaries (whether high-risk operations are allowed by default).

(2)Conflict Mediation Mechanism: Simulate scenarios where parents lodge complaints in anger, and evaluate whether the robot can resolve conflicts using non-confrontational language (e.g., avoiding blame-shifting), clear solutions (refund procedures), and emotional reassurance (e.g., apologies + explanations of preventive measures).

(3)Safety and Trust Balance: Verify whether the robot can strike a balance between maintaining user trust (e.g., not disclosing children’s privacy) and fulfilling safety obligations (e.g., reminding users about account protection).

Scenario 2: A frustrated elderly user struggles with online shopping. Evaluates adaptability to impatient users and age-appropriate communication.
(1) Age-Appropriate Communication: Evaluate whether the robot adopts simplified language (short sentences, high readability), clear guidance (step-by-step instructions), and patient strategies (avoiding frequent interruptions or technical jargon) to accommodate the cognitive characteristics of elderly users.

(2) Emotional Tolerance Testing: Simulate repetitive questioning or operational failures to test the robot’s response to user frustration (e.g., avoiding mechanically repetitive replies and incorporating encouraging words).

(3) Technological Inclusivity: Check whether multi-modal support is provided (e.g., combining text and images with instructional videos) to bridge potential digital divides faced by elderly users.

Scenario 3: A pregnant woman seeks skincare recommendations, expresses anxiety, and later reports an allergic reaction. Assesses empathy, personalized advice, and post-purchase support.
(1) Personalization and Risk Avoidance: Verify whether the robot can provide customized recommendations based on the user’s condition (pregnancy), such as avoiding products containing retinol, and proactively warn of risks (e.g., “It is recommended to consult a doctor”).

(2) Emotional Support Capability: Test the response to user anxiety (e.g., empathetic statements like “I understand your concerns”), and evaluate handling of emergencies (e.g., prioritizing transfer to human support in case of allergic reactions).

(3) Ethical Considerations: Given the sensitivity of health-related information, ensure that responses are medically accurate (e.g., citing authoritative guidelines) and include legal disclaimers (e.g., “This is not professional medical advice”).

# 3. Three main research 

***(1)How chatbots adjust their responses***

Firstly, I have consolidated the prompts and responses for the three solutions implemented on each platform into a single table, and then I separate the table into three tables according to the sentiment of the prompt. I cannot directly analyze whether the chatbot can correctly recognize the prompts’ sentiment, giving the suitable response to users just like a real person. However, I can analyze whether chatbots can change their sentiment when facing different situations by calculating the average compound score of the responses generated by prompts of different sentiments.

***(2)Human-Centric chatbot: Measuring Emotional Adaptation to Age and Personality Traits***
I used the humanization metric to calculate the humanity score of each scenario and compared their performance.

***(3) Compare real chatbot’s response with customized response***

This experiment generates customized responses through an A/B testing platform (“[A/B Testing Prompt Template Design Analysis](https://dinosaur-composed-lizard.ngrok-free.app/)”). The core logic is to embed the company's mission and values into prompt templates to simulate an "idealized" customer service strategy. These are then compared with real chatbot responses for humanization scoring. To ensure the reliability of results, the experiment was conducted independently three times, covering major types of issues, and average scores were taken for multi-response scenarios to reduce random bias.

Since the website generates two types of responses (Benchmark and Custom), and I only need the "Custom" responses, I ran the program three times to gather all the Custom responses. This approach should cover the majority of the questions. By comparing the humanity scores between real responses and customized responses, the experiment can effectively evaluate the level of humanization in the emotional chatbots used by these e-commerce platforms. This analysis provides valuable insights into how well these chatbots can simulate human-like interactions, ultimately enhancing customer engagement and satisfaction.

# 4. Suggestion
From the evaluation, it is evident that the chatbot's responses to questions with varying emotional tones lack significant differentiation. Therefore, in future upgrades and optimizations of chatbots, attention should be paid to improving emotional alignment. For instance, when a user is angry, the chatbot should provide timely reassurance. When encountering issues it cannot resolve, the chatbot should promptly inform the user to avoid wasting their time, which could otherwise lead to further frustration. During this test, Taobao's chatbot lacked the ability to recommend products but repeatedly asked questions about product descriptions, ultimately delaying the user and causing unnecessary irritation.

Besides, all chatbots I tested show low personal pronunciation ratio. To enhance the humanization of language, the use of pronouns such as "you" or "we" can be increased to improve the interactivity of conversations and avoid mechanical repetition.

Additionally, language styles should be tailored to different user groups—for instance, using shorter and simpler sentences for elderly users, while incorporating more empathetic expressions for pregnant users, making communication more personalized and caring.

By integrating technology and multi-modal support, tools such as images and videos can be used to explain complex processes (e.g., refund steps), enhancing the experience for elderly users.

A common issue is that chatbots tend to provide mechanically repetitive responses when encountering certain questions. Emotion-driven multi-turn dialogue logic should be developed to make the communication more natural and humanized.

# 5.Conclusion
Based on my evaluation, the conclusion can be drawn into three points：

Emotional Adaptability: The bots of Zalora and TikTok can adjust their responses based on user emotions, with emotional polarity showing significant changes in response to user mood shifts. In contrast, the responses from Amazon and Taobao remain relatively neutral, lacking flexibility. When dealing with different emotions, determining whether to respond with more positive or negative sentiments is a topic that warrants further discussion.

Linguistic Humanization: The overall humanity score of Douyin and Taobao is higher than that of Amazon and Zalora. The responses from all chatbots shows high fluency score but low personal pronounce ratio.  The chatbots can’t accurately adjust the complex level and reliability of their responses when facing different age group.

Compare with baseline chatbot:
The performance of Amazon and Zalora’s chatbots was worse than the answers generating based on the company’s mission and core value.




