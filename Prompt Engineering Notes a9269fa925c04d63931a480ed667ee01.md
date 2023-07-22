# Prompt Engineering Notes

References：

[A Guide to Crafting Clear and Effective Prompts](https://app.gumroad.com/d/fa4b54072eac65a843a1fb3430266394) 

[Prompt Engineering Guide](https://www.promptingguide.ai/)

[Learn Prompting](https://learnprompting.org/docs/intro)

[Prompt Engineering for Effective Interaction with ChatGPT](https://machinelearningmastery.com/prompt-engineering-for-effective-interaction-with-chatgpt/#:~:text=Prompt%20engineering%20is%20the%20most,responses%20from%20the%20language%20model)

[Resources of Prompt](https://github.com/promptslab/Awesome-Prompt-Engineering)

**Background of ChatGPT and Prompt Engineering**

ChatGpt takes 4k(4096) tokens as input and push into a models that has been trained on a large corpus of text. The model will then generate a response based on the input. Then it will take the first 4095 tokens plus the generated response as the new input and generate a new response, this process will be repeated until the model generates a special token that indicates the end of the response. **Intuitelively, Given x tokens(depend on the mode), it returns the next n likely tokens(specified by her user)** 

**Types**
- **Zero Shot Prompting**: make predictions about unseen data without any additional training
    
    Ex: Generate 10 possible names for my new dog 
    
- **One Shot Prompting**: generate text with a limited amount of input data such as a single example
    
    Ex: Generate 10 possible names for my new dog 
    
    A dog name that I like is Kevin
    
- **Few Shot Prompting**: generate text with a small number of examples for adaption of previously seen data
    
    Ex: Generate 10 possible names for my new dog 
    
    - Kevin
    - Kiwi
    - Jenny
- **Chain-of-Thought Prompting**: generate text step by step to reach the final response
    
    Ex: 
    
    Q: A has 20 eggs. He buys 2 more cartons of eggs and each carton contains 12 eggs. How many eggs does A have now?
    
    A: A start with 20 eggs. 2 cartons of 12 eggs is 12*2 = 24. 20 + 24 = 44. Therefore, A has 44 eggs and the answer is 44
    
    Q： B has 93 chickens. if he sold 20 to C and bought twice that number more, how many chickens does B have now? Let’s think step by step.
    
    

**Principle of writing prompts**:

1. Define the purpose and focus of the conversation 
2. Use specific and relevant language 
3. Avoid open-ended or overly broad prompts
4. Keep the conversation on track
5. Define any jargon or technical terms
6. Avoid using ambiguous language, keep it clear and concise

**Self-Criticism:**

- Please re-read your above response. Do you see any issues or mistakes with you response? If so, please identify these issues or mistakes and make the necessary edits
- Look at the code you have just generated, Currently, it does not run. Are you able to see any syntax errors or flow control mistakes that you are able to rectify it? If so, please identify the section of problematic ode and re-generate it.
