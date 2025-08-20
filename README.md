01-qlora_chatglm3-homework.ipynb：该文件按照课件的代码会OOM，加上了revision='b098244'参数才不会，对此我对这个参数很好奇，于是去
huggingface网站搜索代码里的THUDM/chatglm3-6b这个模型找不到，根据老师在week03课程里提供的THUDM Hugging Face 
主页：https://huggingface.co/THUDM 网址，找到对应的模型为zai-org/chatglm3-6b，发现最新的revision='b098244'，是24年12月份提交的，
尝试将model_name_or_path改成'zai-org/chatglm3-6b'，revision也改成'b098244'，发现还是会OOM，由于当前的依赖包都是较老版本，大概率是
后续提交的版本的一些优化导致显存提升。
02-qlora_chatglm3_timestamp-homework.ipynb：按照openai数据增强后的数据集进行训练，正常训练完成
03-qlora_chatglm3_timestamp-homework(50epoch).ipynb:按照手工制作的数据集进行过度训练，达到过拟合的效果，正常训练完成
04-chatglm_inference-homework.ipynb:分别对不同的数据集训练的模型进行推理，充分体现数据集的质量与一个高效模型是密不可分的！！！
