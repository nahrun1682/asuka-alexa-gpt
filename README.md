# 1. Asuka-Alexa-GPT

# 2. 目次
- [1. Asuka-Alexa-GPT](#1-asuka-alexa-gpt)
- [2. 目次](#2-目次)
- [3. PythonのVersion](#3-pythonのversion)
- [4. Layer作成](#4-layer作成)

# 3. PythonのVersion
3.10.0

# 4. Layer作成

参考：[Lambdaで外部ライブラリを使用(レイヤー使用)](https://www.distant-view.co.jp/column/6513/)

```bash
cd layer_py10_**
mkdir python

pyenv version #3.10.0であることを確認

#pyenv global

#pip install --upgrade pip

#install
pip install openai -t ./python
pip install langchain -t ./python

zip -r openai_langchain_py10.zip python

```
