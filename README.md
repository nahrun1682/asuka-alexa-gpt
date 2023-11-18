# 1. Asuka-Alexa-GPT

# 2. 目次
- [1. Asuka-Alexa-GPT](#1-asuka-alexa-gpt)
- [2. 目次](#2-目次)
- [3. あとやりたいこと](#3-あとやりたいこと)
- [4. Python-Version](#4-python-version)
- [5. 作り方](#5-作り方)
- [6. Layer作成](#6-layer作成)

# 3. あとやりたいこと

1. memoryを持たせる
2. 音声をvoicecox化

# 4. Python-Version
3.10.0

# 5. 作り方


1. [アレクサのカスタムスキルをAWS Lambdaで作成してみた【Alexa Developer Console】](https://www.kuretom.com/alexa-skill-lambda/)
    ますはここでカスタムスキルを学ぶ
2. [【もはや人間！？】アレクサとChatGPTを連携できるようにカスタマイズしてみた。](https://www.kuretom.com/alexa-chatgpt/)
    gptとlambdaを繋ぐ(簡単に)
3. [[ChatGPT]OpenAI APIでGPT-3.5系のモデル「gpt-3.5-turbo」と「text-davinci-003」をLambdaで試してみた](https://dev.classmethod.jp/articles/open-api-lambda-test/)
    ライブラリをzip化してaws lambdaのLayerに入れる
4. [LangChain 0.0.200 での履歴を持った Chat、シンプルな Agent、長文の要約などの実装サンプル](https://qiita.com/hideki/items/d3a474c85cdb7eb8e936)
    gptアプリケーション用フレームワークライブラリlangchainの使い方

# 6. Layer作成

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
pip install tiktoken -t ./python

zip -r openai_langchain_py10.zip python

```
