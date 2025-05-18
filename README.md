# LLM-Sentiment-SW-Project

This repository is a fork of https://github.com/DAMO-NLP-SG/LLM-Sentiment. Used for a research paper: 
"[Sentiment Analysis in the Era of Large Language Models: A Reality Check](https://arxiv.org/abs/2305.15005)".

The goal of this project is to get this codebase running on my local machine. And if there is room for any improvement, idenfify & implement some of these improvements.

## Python
This project uses dependencies supporting Python version <=3.9. Therefore this project uses Python 3.9.

## Usage
0. fill in your OpenAI api key in the bash files under `script` folder. For example:
```
python predict.py \
--setting zero-shot \
--model chat \
--use_api \
--api #your api here
```

1. Run zero-shot and evaluate
```
bash script/run_zero_shot.sh
bash script/eval_zero_shot.sh
```

2. Run few-shot and evaluate
```
bash script/run_few_shot.sh
bash script/eval_few_shot.sh
```

## Note
1. To view the summary of prompts and evaluation results, please navigate to the output folder and check the respective task folder.
2. You can specify `--selected_tasks` and `--selected_datasets` to only run with certain tasks or datasets.


## Citation
If the code is used in your research, please star our repo and cite our paper as follows:
```
@misc{zhang2023sentiment,
      title={Sentiment Analysis in the Era of Large Language Models: A Reality Check},
      author={Wenxuan Zhang and Yue Deng and Bing Liu and Sinno Jialin Pan and Lidong Bing},
      year={2023},
      eprint={2305.15005},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
