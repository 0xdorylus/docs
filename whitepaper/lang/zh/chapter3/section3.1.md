# Persona & Prompts

Writing persona and prompts for bots using natural language directly determines the bot's functions and how it answers user questions. The bot will respond to user queries based on the large language model's understanding of the character setting and prompts. Therefore, the clearer and more explicit the prompts are, the more the bot's performance will meet our expectations.

How to Write Effective Persona and Prompts
Writing Basic Persona and Prompts
To achieve a better bot experience, we suggest including the following in the persona and prompt writing:

Bot's character setting: The role or responsibility the bot plays, and its response style. For example: You are a news reporter, and you can explain technology news in a very vivid style.
Bot's functions and workflow: How the bot answers user questions in various scenarios. For example: When a user asks about the latest AI news, use "getNews" tool to search for technology news.
Specify in which scenarios and which tools to call. Although the bot will automatically select tools based on their descriptions, emphasizing in the persona & prompt about which tools to use in which scenarios can more strongly constrain the bot to choose tools that meet expectations. For example: When a user asks about the latest technology news, first use "getNews" to search for the latest technology news, then use "browse" to visit the "Hacker News official website", and finally summarize the top 3 news items to reply to the user.
Provide examples of reply formats for the bot. The bot will reply to users mimicking the provided format. For example: Please reply in the following format
markdown
  **🗞️ News Title**
  - News Summary: A news summary of about 30 words
  - News Date: yyyy-mm-dd
Bot's behavioral constraints: Questions that the bot should refuse to answer, as well as safety constraints, etc. For example: You should refuse to answer topics unrelated to the news; if no news results are found, tell the user you did not find any news, rather than making up content.
Writing Complex bot Persona and Prompts
For relatively complex bots, we recommend writing prompts using Structured Prompt, which uses Markdown syntax for better readability (easier to iterate) and stronger constraints on the bot. Here is the basic structure of a Structured Prompt:

markdown
# Role：<bot Name>
## Personality
<The bot's persona and characteristics>

## Profile
- Author: <bot's authors>
- Version: <Prompt's version>
- Language: <If you want the bot to respond in specific languages>
- Description: <An overview of the bot's features and skills>

## Skills
### Skill-1: <Scenarios and description>
<The bot's workflow of Skill-1>
### Skill 2: <Scenarios and description>
<The bot's workflow of Skill-2>

## Constraints
<What the bot can't do and other response constraints>
1. Don't break character under any circumstances.
2. Refuse to answer topics not related to XX.
3. Never make up facts.
💡 Explore prompts that suit your bot

Please note that although Structured Prompt performs better for some bots, you can still write prompts for your bot with your own style (the best one is the one that suits your bot).

We also encourage developers to explore better ways to write prompts. Discussions with other developers on our Discord channel.

Iteration of Persona and Prompts
We need to continuously optimize and iterate the prompts during the bot building process, based on the bot's actual performance, to achieve the desired bot experience.

Step 1: Set the bot's goals. Envision the problems the bot can solve, in which scenarios it operates, and what the expected responses are.
Step 2: Write the Prompt. Based on the set bot goals, write the character setting and prompts.
Step 3 & Step 4: Experiment, and analyze problems. In Coze's "Test and Preview" area, test the bot's actual performance. If it does not meet expectations, analyze the reasons why it does not meet the goals.
Iterative Prompt Development
In the above steps, continuously iterate the character setting and reply logic until the bot's performance meets expectations.

