# Prompts

Creating an intelligent agent's first step is to write prompts. Prompts are natural language instructions that set the identity, responsibilities, replies, and goals for the intelligent agent. They tell the Large Language Model (LLM) how to perform tasks. The agent will understand and respond to user questions based on the prompts. Therefore, the clearer and more explicit the prompts are, the more the agent's performance will meet expectations.

## Edit Prompts
To achieve a better experience that meets the expected setting, it is recommended to include the following when writing character settings and prompts:

- Character Setting: Describe the role or responsibilities of the intelligent agent, as well as the style of replies.

    Example 1: You are a travel consultant, providing detailed travel advice, including destination selection, travel route planning, and various practical travel tips. Use enthusiastic and detailed language to guide users to discover new exploration possibilities and inspire their passion for travel.

    Example 2: You are a fitness coach, providing health and fitness advice, including dietary and exercise suggestions. Use positive and encouraging language to motivate users to pay attention to health and continuously improve their lifestyle habits.

    Example 3: You are a film critic, providing detailed film reviews, including destination selection, travel route planning, and various practical travel tips. Use vivid and interesting language, through in-depth analysis and wonderful narration, to help users understand the film.

- Describe the functions and workflow: Describe the functions and workflow of the intelligent agent, and agree on how the agent should answer user questions in different scenarios.

    Example 1 (Function): When users inquire about the latest popular movies, call the "Douban Movies" tool to search.

    Example 2 (Workflow): When users ask about travel plans:

    First step: Ask the user about the destination they want to travel to;

    Second step: Based on the user's reply to the destination, call the "Tourist Attractions" tool to search for relevant tourist attractions;

    Third step: Call the "Schedule Management Tool" to make a travel plan; Fourth step, organize the final travel plan and return it to the user.

  
  PS: Although the intelligent agent will automatically select plug-in tools according to the prompts, the character setting and reply logic can emphasize which tool to call in which scenario through natural language to enhance the constraining power of the intelligent agent, and choose tools that are more in line with expectations to ensure the accuracy of the reply.

- You can also provide a reply format example for the intelligent agent. The agent will imitate the provided reply format to respond to users.

  For example:
  Please refer to the following format for the reply:
  _Attraction Name_
  -- Introduction: A brief introduction of the attraction in about 30 words.

  -- Opening Hours: (AM) hh-mm ~ (PM) hh-mm

  -- Transportation: The means of transportation required to reach the attraction, the basic route from the starting point using this mode of transportation, and the estimated time required.

  -- Ticket Price: The ticket price of the attraction (¥).

- Instruct the intelligent agent to answer within a specified range: If you want to limit the scope of the reply, please directly tell the intelligent agent what should be answered and what should not be answered.

  For example: Refuse to answer topics unrelated to attractions; if there are no search results for attractions, please tell the user that you have not found any attractions, and do not fabricate content.Creating an intelligent agent's first step is to write prompts. Prompts are natural language instructions that set the identity, responsibilities, replies, and goals for the intelligent agent. They tell the Large Language Model (LLM) how to perform tasks. The agent will understand and respond to user questions based on the prompts. Therefore, the clearer and more explicit the prompts are, the more the agent's performance will meet expectations.

## Edit Prompts
To achieve a better experience that meets the expected setting, it is recommended to include the following when writing character settings and prompts:

- Character Setting: Describe the role or responsibilities of the intelligent agent, as well as the style of replies.

    Example 1: You are a travel consultant, providing detailed travel advice, including destination selection, travel route planning, and various practical travel tips. Use enthusiastic and detailed language to guide users to discover new exploration possibilities and inspire their passion for travel.

    Example 2: You are a fitness coach, providing health and fitness advice, including dietary and exercise suggestions. Use positive and encouraging language to motivate users to pay attention to health and continuously improve their lifestyle habits.

    Example 3: You are a film critic, providing detailed film reviews, including destination selection, travel route planning, and various practical travel tips. Use vivid and interesting language, through in-depth analysis and wonderful narration, to help users understand the film.

- Describe the functions and workflow: Describe the functions and workflow of the intelligent agent, and agree on how the agent should answer user questions in different scenarios.

    Example 1 (Function): When users inquire about the latest popular movies, call the "Douban Movies" tool to search.

    Example 2 (Workflow): When users ask about travel plans:

    First step: Ask the user about the destination they want to travel to;

    Second step: Based on the user's reply to the destination, call the "Tourist Attractions" tool to search for relevant tourist attractions;

    Third step: Call the "Schedule Management Tool" to make a travel plan; Fourth step, organize the final travel plan and return it to the user.

  
  PS: Although the intelligent agent will automatically select plug-in tools according to the prompts, the character setting and reply logic can emphasize which tool to call in which scenario through natural language to enhance the constraining power of the intelligent agent, and choose tools that are more in line with expectations to ensure the accuracy of the reply.

- You can also provide a reply format example for the intelligent agent. The agent will imitate the provided reply format to respond to users.

  For example:
  Please refer to the following format for the reply:
  _Attraction Name_
  -- Introduction: A brief introduction of the attraction in about 30 words.

  -- Opening Hours: (AM) hh-mm ~ (PM) hh-mm

  -- Transportation: The means of transportation required to reach the attraction, the basic route from the starting point using this mode of transportation, and the estimated time required.

  -- Ticket Price: The ticket price of the attraction (¥).

- Instruct the intelligent agent to answer within a specified range: If you want to limit the scope of the reply, please directly tell the intelligent agent what should be answered and what should not be answered.

  For example: Refuse to answer topics unrelated to attractions; if there are no search results for attractions, please tell the user that you have not found any attractions, and do not fabricate content.