言語処理 100 本ノック 2020 (Rev 1)
============================
poetry config --list
poetry config virtualenvs.in-project true
poetry install
poetry run jupyter-notebook

sudo apt-get install -y mecab libmecab-dev mecab-ipadic-utf8 git make curl xz-utils file swig


( cd somewhere )
git clone --depth 1 https://github.com/neologd/mecab-ipadic-neologd.git
mecab-ipadic-neologd/bin/install-mecab-ipadic-neologd -n -a
( yes / SUDO_PASSWORD )
`mecab -d /usr/lib/x86_64-linux-gnu/mecab/dic/mecab-ipadic-neologd`

→ MeCab.Tagger('-Owakati -d /usr/local/lib/mecab/dic/mecab-ipadic-neologd') 