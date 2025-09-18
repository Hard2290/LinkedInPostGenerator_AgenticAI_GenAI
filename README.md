# **LinkedIn Post Generator - AI Workflow & Automation - Make.com**
## **Project Overview :**
- Built an AI agents workflow to generate quality text and image content and post it on LinkedIn platform.

## **Tools Used :**
- **Make.com** - to visualise and create AI agents workflow. 
- **Google Sheets** - to store generated contents and coordinate with AI agents.
- **Google Drive** - to store and extract generated content.
- **OpenAI** - LLM driving the AI workflow
- **ClaudeAI** - to generate AI-friendly system and user prompts.

# **Walkthrough :**
- Create a google sheet with following columns *Channel*, *Post Idea*, *LinkedIn Post Draft*, *Image Link* and *Control* to store the outputs and coordinate with AI agents accordingly.
	- **Channel** - mentioning the social media channel to generate content for and to post on it.
	- **Post Idea** - seed idea given by user as input to the AI workflow. 
	- **LinkedIn Post Draft** - store the generated engaging and social media friendly content based on research done on the seed idea by AI agents.
	- **Image Link** - store the google drive link of the AI generated image content relevant to the seed idea.
	- **Control** - help control the direction of workflow with the help of 4 keys, *Prepare Content*, *Ready for review*, *Post Content*, *Posted Content* mentioning current status of the workflow.

	![Image](https://github.com/user-attachments/assets/fa79fd25-dafe-4d52-aa60-75a9a9abcd12)


- Create an empty google drive folder to give its access to AI agents for to store the generated images.
- Start creating *Agentic Workflow Layout* on **Make.com** platform by creating a *Google Sheets Module* and connecting it to the google sheet using our *Spreadsheet ID* to give AI its access.
- Using keys *Prepare Content* and *Post Content* in control column, set *Router Module* parameters to drive the workflow first towards content research and creation and then towards posting those generated content on *LinkedIn*.
- Create *OpenAI Modules* using **OPENAI_API_KEY** to allow agents to use LLM to do research, generate content, generate image prompt aligning with the content objectives and finally generate image using that prompt.
- Use *ClaudeAI* to generate **System Prompts** and **User Prompts** for *OpenAI Modules* tailored to our personalised content needs given to claude preferrably in detailed *Markdown Prompting Style*. 
- Use *Google Drive Module* to give AI access to google drive folder for it to save the generated image and further save its corresponding link to the google sheet.
- Now, when the status of workflow is "Post Content", allow AI agents to retrieve the generated image and using *LinkedIn Module* give agents access to LinkedIn platform to create a post.
- Finally, direct the agents to set the status of workflow to *Posted Content* on succesful creation of post on LinkedIn.

**Visual representation of the AI Agentic Workflow**

![Image](https://github.com/user-attachments/assets/6b7090f7-c3fc-49f3-8bb9-df8d82114c15)

## **Results :**
- After succesful generation of the content and related image, AI agent updated the google sheet and changed the status from "Prepare Content" to "Ready for review".

**Before and During Content Generation -**

![Image](https://github.com/user-attachments/assets/7bff60b9-a86b-47ce-ac36-5e37288f1096)

**After Content Generation -**

![Image](https://github.com/user-attachments/assets/fcbc2a89-913f-44ff-9305-375d8bf6390e)

- Image added to google drive by AI agent.

![Image](https://github.com/user-attachments/assets/46385b1d-201e-4277-8545-b1f653cd8b06)
![Image](https://github.com/user-attachments/assets/d9be29ae-2a1e-4428-8563-9a859ae258b6)

- Post created by AI agent on LinkedIn.

![Image](https://github.com/user-attachments/assets/cd18086d-4ba4-4cf1-9fc7-9239f9bc2c5e)
