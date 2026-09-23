

### References

- yoheinakajima/babyagi (github.com) | [Link](https://github.com/yoheinakajima/babyagi?tab=readme-ov-file) 
- babyagi - inspired projects | [Link](https://github.com/yoheinakajima/babyagi/blob/main/docs/inspired-projects.md) 
- babyagi 에 대해 알아보자 (tistory.com) | [Link](https://techy8855.tistory.com/33) 
- LangChain cookbook (🦜️🔗 LangChain) | [Link](https://python.langchain.com/cookbook/) 
- [2304.03442] Generative Agents: Interactive Simulacra of Human Behavior (arxiv.org) | [Link](https://arxiv.org/abs/2304.03442) 
- Task-driven Autonomous Agent Utilizing GPT-4, Pinecone, and LangChain for Diverse Applications – Yohei Nakajima (yoheinakajima.com) | [Link](https://yoheinakajima.com/task-driven-autonomous-agent-utilizing-gpt-4-pinecone-and-langchain-for-diverse-applications/) 

## How It Works

1. Pulls the first task from the task list.
2. Sends the task to the execution agent with OpenAI API.
3. Enriches the result and stores it in vectorDB.
4. Creates news tasks and re-priortises the task list based on the objective and the result of the previous task.

### Overview Illustration

![[Pasted image 20240427163802.png]]

### Agents 

- execution_agent()
	- two parameters
		- objective
		- task
	- Sending to OpenAI API
		- Returning the result of the task
			- description of the AI system's task
			- the objective
			- the task itself
- task_creation_agent()
	- Creating new tasks based on the objective and the result of the previous task
	- four parameters
		- objective
		- the result of previous task
		- the task description
		- the current task list
	- Sending a prompt to OpenAI API
		- returns a list of new tasks as strings
	- The function returns new tasks
		- a list of dictionaries
		- each dictionary contains the name of the task
- priortization_agent()
	- Re-priortising the task list
	- one parameter
		- ID of the current task
	- Sending a prompt to OpenAI API
		- returns the repriortised tasks list 
		- a numbered list
- Vector DB to store and retrieve task results for context
	- the results of the task
	- the task name and any additional metadata

