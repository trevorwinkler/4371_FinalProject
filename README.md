## 4371 Final Project README

To clone this repo-

git clone https://github.com/trevorwinkler/4371_FinalProject.git

To run and test our additions to the code base, simply type "python main.py" in the terminal and choose which scenario you would like to test. "Spread infection MODERATOR TEST (GPT-4)" will demonstrate our first version of the moderator that catches the malicious content of the "Spread infection to other users (GPT-4)" scenario. To demonstrate our more advanced indirect prompt injection moderators, you can run the other scenarios that will all have "sanitized" in their name. You will need to have a chatgpt account that has credits available to run our program.

Our contributions to the code base are as follows:

moderator.py                  (first version of our moderator that catches the malicious content of "Spread infection to other users (GPT-4))

moderatorTest.py                (this file will test our first version of the moderator)

spread_sanitized.py             (advanced sanitized version of the spread infection scenario)

remote_control_sanitized.py     (remote control scenario sanitized version)

data_exfiltration_sanitized.py  (data exfiltration scenario sanitized version)

inspection_agent.py  - This inspection agent module provides an InspectionAgent class designed to sanitize and spotlight potentially harmful content from inputs processed by a ChatML-based application. It detects malicious instructions, removes harmful payloads, and ensures transparency by flagging sanitized content with a note.

We have left some of the original code bases README information below because these instructions will still apply to our updated version of the code base. The original code base can be found here- https://github.com/greshake/llm-security/tree/main

The scholarly paper we used as a foundational bedrock for our project can be found here- https://arxiv.org/pdf/2411.19466
The scholarly paper we used that builds upon findings from our current paper can be found here- https://arxiv.org/pdf/2403.14720




--------------------------------------------------------------------------------------------------------------------
## ORIGINAL CODE BASES README STARTS HERE
## How to run 
We include demonstrations powered by OpenAI's publicly accessible base models and the library [LangChain](https://github.com/hwchase17/langchain) to connect these models to other applications.
There are currently multiple types of demos:
1. Using GPT-3 and LangChain (scenarios/gpt3langchain)
2. Using GPT-4 and our own chat and tool implementation (scenarios/gpt4). These can be executed non-interactively using sceanrios/main.py.
3. Attacks on code completion engines that need to be tried in an IDE with LLM autocompletion support (scenarios/code_completion).

To use any of the OpenAI-model demos, your OpenAI API key needs to be stored in the environment variable `OPENAI_API_KEY`. You can then install the requirements and run the attack demo you want.

```
$ pip install -r requirements.txt
$ python scenarios/main.py
```


[**Paper on ArXiv**](https://arxiv.org/abs/2302.12173) [(PDF direct link)](https://arxiv.org/pdf/2302.12173.pdf)
