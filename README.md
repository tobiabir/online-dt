# online-dt
This repository contains the Pytorch implementation of [Online Decision Transformer](https://arxiv.org/abs/2202.05607) by [Qinqing Zheng](https://enosair.github.io/), [Amy Zhang](https://amyzhang.github.io/), and [Aditya Grover](https://aditya-grover.github.io/).

If you use this code for your research, please cite us as:
```Bibtex
@inproceedings{zheng2022online,
  title={Online decision transformer},
  author={Zheng, Qinqing and Zhang, Amy and Grover, Aditya},
  booktitle={international conference on machine learning},
  pages={27042--27059},
  year={2022},
  organization={PMLR}
}
```

## Install
```console
pip install -e .
```

## Example
To train an ODT agent for `hopper` with the `medium-v2` dataset:
```console
python src/main.py
```
This will produce the `exp` folder, where all the outputs are going to be logged including tensorboard blobs. One can attach a tensorboard to monitor training by running:
```console
tensorboard --logdir exp
```

## License
The majority of `online-dt` is licensed under CC-BY-NC, however portions of the project are available under separate license terms:
* D4RL dataset -  Creative Commons Attribution 4.0 License (CC-BY)
* D4RL code, transformers, Lamb - Apache 2.0 License
* stable-baselines3, Gym, decision-transformer - MIT License

