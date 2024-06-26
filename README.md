# OpenAGI: Package for AI Agent Creation
<a href='https://arxiv.org/abs/2304.04370'><img src='https://img.shields.io/badge/Paper-PDF-red'></a>
[![Code License](https://img.shields.io/badge/Code%20License-MIT-green.svg)](https://github.com/agiresearch/OpenAGI/blob/main/LICENSE)
<a href='https://discord.gg/B2HFxEgTJX'><img src='https://img.shields.io/badge/Community-Discord-8A2BE2'></a>


## ✈️ 1. Getting Started
### 1.1 Installation
#### (1) use OpenAGI in AIOS
1. follow [AIOS](https://github.com/agiresearch/AIOS) instruction to install the virtual environment

2. Allow your code to be able to see 'openagi'
```
$ pip install -e .
```

#### (2) use OpenAGI alone
1. set up virtual environment and install the required packages using pip
```bash
conda create -n OpenAGI python=3.11
source activate OpenAGI
cd OpenAGI
pip install -r requirements.txt
```
2. Allow your code to be able to see 'openagi'
```
$ pip install -e .
```

### 1.2 Usage
If you use external tool APIs in your agents, you can follow instructions of setting up tools in [How to setup external tools](./tools.md). 

You can also create .env file from the .env.example file, and then use dotenv to load the environment variables using .env file into your application's environment at runtime.

```bash
cp .env.example .env
```

## 2. Contributing
Run tests: Add your test code into the tests/ directory if any, then run test via pytest
```
cd openagi
pytest -v tests
```
sample output
```
============================================================================================================================= test session starts ==============================================================================================================================
platform darwin -- Python 3.11.9, pytest-8.1.1, pluggy-1.5.0 -- ""
cachedir: .pytest_cache
rootdir: ""
plugins: anyio-4.3.0
collected 2 items                                                                                                                                                                                                                                                              

tests/test_agent_creation.py::test_agent_creation PASSED                                                                                                                                                                                                                 [ 50%]
tests/test_tools.py::test_currency_converter_api PASSED                                                                                                                                                                                                                  [100%]
```

## 🖋️ 3. Research
Please check out our [implementation](./research) for our research paper [OpenAGI: When LLM Meets Domain Experts](https://arxiv.org/abs/2304.04370).

```
@article{openagi,
  title={OpenAGI: When LLM Meets Domain Experts},
  author={Ge, Yingqiang and Hua, Wenyue and Mei, Kai and Ji, Jianchao and Tan, Juntao and Xu, Shuyuan and Li, Zelong and Zhang, Yongfeng},
  journal={In Advances in Neural Information Processing Systems (NeurIPS)},
  year={2023}
}
```

## 🌍 4. OpenAGI Contributors
[![OpenAGI contributors](https://contrib.rocks/image?repo=agiresearch/OpenAGI&max=300)](https://github.com/agiresearch/OpenAGI/graphs/contributors)



## 5. Star History

[![Star History Chart](https://api.star-history.com/svg?repos=agiresearch/OpenAGI&type=Date)](https://star-history.com/#agiresearch/OpenAGI&Date)
