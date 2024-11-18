# DSC180A-Methodology-5

Yuxuan Zhang (yuz165@ucsd.edu)

Section: B04 Hao Zhang

The most interesting part is to train llama8b LLM in parallelism with four GPUs. I need to explore many parallelism strategies such as data parallelism and model parallelism. Finally, I choose to use zero3 deepspeed by sharding optimizer state, gradients, and weights.

I probably want to delve deeper into a toolkit which help estimate training flops and memory and provide training strategy in multi-gpus. In the parallelism, there are not so many tutorials in multi-gpu training. Also, training llm is expensive so if people could set up and estimate flops and memory cost, they could save money and resources in the training。

We probably try to use a more robust way to calculate flops and memory. We dont want to approximate the flop and memory requirement so we probably try to run a similator to calculate model flops and memory based on simulator. Without running the whole model, we need to run this model simulator to calculate the number of operation and memory cost at each layer. 

I am instereted in using profilier to monitor flops and memory cose to verify the correctness of our llm simulator. Also, I want further research how fully shard data parallelism work in a way to increase or decrease flops and memory. 


