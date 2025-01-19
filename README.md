# zno-golden-medalist
Golden Medalist That solves ZNO for you .... for 20$

This is the amount of money I have used to train Qwen-32B-4bit on VAST.ai 

## Description

Qwen models have competitive advantage of advanced Ukrainian reasoning, hence they are better in predicting the next token of the quiz 
I am not sure about correctness of results. The smart way of training is firstly train LLM on large corpus of Ukrainian Literature Text, but where is this dataset? Nobody knows...

## Results 

After 20 epochs the training loss is 0.13 and validation loss 0.19

## Methods 

I have used only SFT (Supervised Fine-tuning Trainer) to create submission because neither DPO or KTO haven't lead to valuable results.

I tried to use various models to solve the quizes:

 "Qwen/Qwen2.5-3B-Instruct"
 "meta-llama/Llama-2-7b-chat-hf"
 "Qwen/Qwen2.5-3B-Instruct-GGUF"
 "unsloth/Qwen2.5-3B-Instruct-bnb-4bit" 
 "unsloth/Qwen2.5-32B-bnb-4bit"

I used LoRa to decrease time of training using low rank approximations with various numbers of r from 1 to 16 but this doesn't really affected the training.
To quatize some models I have used BitsAndBytes.

## The best score:

Supervised Fine Tuning - 0.588

## Conclusions:

### Правильна відповідь:
<|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|> <|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|><|im_end|>
