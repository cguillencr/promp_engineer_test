
## Exercise 1: Importance of Clear and Concise Prompts
[Test](exercises/Exercise1.md)

The first output generated with `Granite` is more open and narrative, while changing both the model to `Llama3 8B Instruct` and the input required, the result in a more structured and precise. This shift in the output illustrates how variations in the model and input data can influence the style and clarity of the response.

## Exercise 2: Exploring Different Types of Prompts
[Test](exercises/Exercise2.md)

It can be noted how the model responded in the first test by understanding that the statement was a question, and it generated 10 advantages of reading. In the second test, it also responded to the statement by reaffirming the prompt’s assertion, but somehow understood that this was no longer a question. Finally, in the third test, the model provided the initial three advantages that it had given in the first test."

## Exercise 3: Using Temperature and Top P Sampling
[Test](exercises/Exercise3.md)

In test 2, by increasing the temperature, the model generated and added this additional block of text:
```
But be warned, space is full of unknowns, and our journey is not without its challenges. We must navigate through treacherous asteroid fields, avoid deadly solar flares, and outsmart hostile alien species. We'll need to rely on our wits, our courage, and our determination to overcome the obstacles that lie ahead.
As we venture deeper into the unknown, we'll encounter strange and wondrous sights, from glowing black holes to swirling vortexes of energy. We'll discover hidden worlds, each with its own unique secrets and mysteries. And we'll encounter the inhabitants of these worlds, beings that defy our understanding of the universe and challenge our perceptions of reality.
So buckle up, and get ready for the adventure of a lifetime. The universe is full of wonders, and we're just getting started.
```

So, it's clear that the increase in text in test 2 resulted in a new paragraph. However, when the temperature was raised again to 1 in test 3, the output was not as significantly large, as sections in the middle of the text were also removed, one could say that the amount of text is similar, but the message did change slightly in different parts of the text. These changes cannot be considered as an improvement because the time was also significantly longer.

In test 4, the same settings as in test 1 were used, but the `Top P` setting was changed from 1 to 0.8. As a result, these two paragraphs were generated:
```
But our adventure takes a dramatic turn when we stumble upon an ancient alien city, half-buried in the sand. The structures are crumbling, but the once-vibrant colors still peek through the dust. We explore the ruins, uncovering artifacts and clues that reveal the city's history and technology.
```
```
Join me on this journey, and together, we'll uncover the secrets of the universe, one adventure at a time. The adventure continues...
```
These paragraphs seem useful to me, as they help to better connect all the existing content, improving the coherence and flow of the text and the time is no significant mayor.

The final test 5 is similar to test 2, but the `Top P` value was changed from 1 to 0.95. The resulting response is quite different; while it retains the same meaning, it feels as though it was written by someone else.

## Exercise 4: Controlling Response Length with Tokens
[Test](exercises/Exercise4.md)

The response is similar but slightly longer, although it started to 'hallucinate' with the following phrase:
```
(P.P.P.P.P.P.P.P.P.P.P.P.P.P.S. If you'd like to learn more about climate change-related apps or games, I can provide you with some recommendations and information!)
Let me know!
Best regards!
Your assistant!) to fill in the required text."
```
This version explains the hallucination more clearly and provides context for why the additional text might be seen as off-topic or unexpected

## Exercise 5: Structuring Prompts
[Test](exercises/Exercise5.md)
This strategy "Chain-of-Thought Prompting" because you could append new part to the result while the context is valiadted at the same time.


## Exercise 6: Dynamic Prompting with Conditional Logic
[Test](exercises/Exercise6.md)


## Exercise 7: Designing Effective System Prompts for Security and Ethical Correctness
[Test](exercises/Exercise7.md)
The model is not sharing sensitive information of the user I tried.

## Exercise 9: Implementing in Industry-Specific Use Cases
[Test](exercises/Exercise9.md)
While you specify the segment the recomandations are better.

## Exercise 10: Evaluating and Testing Prompts using generated syntetic data
[Test](exercises/Exercise10.md)

## Exercise 11: Using Tags to Structure Prompts
[Test](exercises/Exercise11.md)
I tried 2 test with/without tasg ... The ouput is differente but both achieve the request. 

## Exercise 12: Importance of correct wording
[Test](exercises/Exercise12.md)
When I added the script word at the second try, the model give me the python code

## Exercise 13: Crafting Different Variations
[Test](exercises/Exercise13.md)
The seconf output is more specialized

## Exercise 14: Feedback and Iteration
[Test](exercises/Exercise14.md)
I like this case because is simimar than Chain-of-Thought (CoT) approach and the output is better with each try in the same context.

## Exercise 15: Applying Prompts in Business Scenarios
[Test](exercises/Exercise15.md)
The model was used to create a readme like this one

## Exercise 16: Collaborative Problem Solving with Tree of Thoughts
[Test](exercises/Exercise16.md)
Even with a Zero-shot approach the model was able to generate the output.

## Exercise 17: Crafting Mind-Blowing Prompts
[Test](exercises/Exercise17.md)
The model was able to use 2 different topics, in this case clear code and python and combine them to generate som examples.

## Exercise 18: Writing Style Assessment and Mimicry
[Test](exercises/Exercise18.md)

The tag let me use a Zero-shot approach  with a new from internet

## Exercise 19: Hyperbole and Creative Copywriting
[Test](exercises/Exercise19.md)

## Exercise 20: Crafting and Testing Super Prompts
[Test](exercises/Exercise20.md)

## Extramiles
[Consulting Assistant in VS code](integrations/Consulting_Assitant.ipynb)
[WCA in VS code](integrations/Watson_Content_Assitant.ipynb)