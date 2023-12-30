# Fine Tuning Facebook-bart-large-cnn on the Samsum Text Summarization dataset
Training and benchmarking text-summarization models against Rouge score on the Samsum Dataset. 
### Results  : 
![image](https://github.com/dhivyeshrk/FineTuning-Facebook-bart-large-cnn/assets/99530121/807875cf-1efb-4346-9fbe-c667320299c5)

The fine-tuned model can be found at https://huggingface.co/dhivyeshrk/bart-large-cnn-samsum
Runtime Logs and GPU utilization can be found in wandb_logs.pdf
Trained on Nvidia Tesla P100 
### Training hyperparameters
The following hyperparameters were used during training:
- learning_rate: 5e-05
- train_batch_size: 1
- eval_batch_size: 1
- seed: 42
- gradient_accumulation_steps: 16
- total_train_batch_size: 16
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 500
- num_epochs: 1
### Streamlit App
Open Streamlit_App_Text_Summarizer.ipynb for a live demo
It is recommended to use colab.
