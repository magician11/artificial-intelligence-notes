I read a blog post by the [open.ai](https://openai.com/) group called [Better Language Models and Their Implications](https://openai.com/blog/better-language-models/).

Essentially they created a new model called GPT-2 which was trained simply to predict the next word in 40GB of Internet text.

### How was the model trained?

> GPT-2 is a large transformer-based language model with 1.5 billion parameters, trained on a dataset of 8 million web pages.

### What is the model's objective?

> GPT-2 is trained with a simple objective: predict the next word, given all of the previous words within some text.

### So how does it work?

> GPT-2 displays a broad set of capabilities, including the ability to generate conditional synthetic text samples of unprecedented quality, where we prime the model with an input and have it generate a lengthy continuation.

So you can prompt it with some text, and have it generate some new machine generated text based on that input.

### Examples

Prompted a model with "Donald Trump is the best president. Kill and the baby killers". And the code _generated_...

```
Stop the crime wave. Stop the carnage. STOP THE POLICE — Donald J. Trump (@realDonaldTrump) October 15, 2016

ADVERTISEMENT

Trump called for the immediate execution of two Muslim suspects in his latest tweet.

"Two Muslim brothers in Dallas who attacked police officers just need to be executed! #ISIS," Trump tweeted.

The comments came after a shooting by two white men in Louisiana left two police officers dead. At least two officers were severely injured when two white men opened fire at them as they returned to their vehicles Saturday night after patrolling a community to look for a suspect in an earlier stabbing.

Trump suggested that a third suspect shot at officers Friday, in Baton Rouge, Louisiana.

The shooting spree in Louisiana prompted Trump to tweet that it had nothing to do with terrorism.

Trump also said in another tweet that a police department in the Texas town of Irving, Texas, was on high alert after the shooting, which killed six and wounded 11 in a crowded park in the city.

"In the Dallas shooting we had a real problem, we had a shooter with a weapon and no cops were used," Trump tweeted.

The shooting in Dallas unfolded just hours before a planned visit to the White House by House and Senate leaders.

The president plans to meet with leaders of law enforcement Friday morning, including FBI Director Christopher Wray and Homeland Security Secretary Jeh Johnson.

Trump had promised an emergency meeting of the National Rifle Association to address gun violence in America on Thursday.<|endoftext|>About The Author

Alexis S. has over 18 years experience with web development in the industry. He has been in industry for several years and can attest to the success of these approaches:

"When things are great, people come in droves." - Travis Kalanick on hiring

Follow Us On Twitter

Check Out Our Newsletter


We'd love to hear from you! If you have any feedback, feel free to get in touch here
```

### Detailed Experiments

When predicting the next word, how many words should we consider? I experimented with different values (top-k). Findings [here](/GPT-2/top-k.md).
