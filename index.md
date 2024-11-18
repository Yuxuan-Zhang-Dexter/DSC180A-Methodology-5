# DSC180A-Methodology-5

**Name:** Yuxuan Zhang  
**Email:** [yuz165@ucsd.edu](mailto:yuz165@ucsd.edu)

**Section:** B04  
**Mentor:** Hao Zhang

---

### What is the most interesting topic covered in your domain this quarter?

The most engaging aspect this quarter has been learning how to train the Llama8B LLM using parallelism across four GPUs. Exploring various parallelism strategies, such as data and model parallelism, was foundational. Ultimately, I opted for using Zero3 DeepSpeed, which involves sharding optimizer states, gradients, and model weights.

### Describe a potential investigation you would like to pursue for your Quarter 2 Project.

I am interested in developing a toolkit that estimates training FLOPs and memory usage and provides strategic guidance for multi-GPU training setups. Given the scarcity of multi-GPU training tutorials and the high costs associated with training LLMs, such a toolkit could help save both money and resources by optimizing training processes.

### What is a potential change you’d make to the approach taken in your current Quarter 1 Project?

Instead of approximating FLOPs and memory requirements, a more robust approach would be to utilize a simulator. This simulator would calculate the model’s FLOPs and memory demands at each layer without having to run the entire model. This method ensures more precise resource planning and utilization.

### What other techniques would you be interested in using in your project?

I am keen on employing a profiler to monitor the FLOPs and memory usage to verify the accuracy of our LLM simulator. Additionally, I would like to further investigate how fully sharded data parallelism can affect FLOPs and memory usage, either increasing efficiency or presenting new challenges.

---
