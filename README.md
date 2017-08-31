# Banco Central do Brasil

[![PyPI version](https://badge.fury.io/py/bancocentralbrasil.svg?1.0)](https://pypi.python.org/pypi/bancocentralbrasil/1.0)
[![Build Status](https://travis-ci.org/leogregianin/bancocentralbrasil.svg)](https://travis-ci.org/leogregianin/bancocentralbrasil)
[![codecov](https://codecov.io/gh/leogregianin/bancocentralbrasil/branch/master/graph/badge.svg)](https://codecov.io/gh/leogregianin/bancocentralbrasil)

Sobre
-------

  * Obtenção de informações sobre taxas oficiais diárias de Inflação, Selic, Poupança e Dólar direto do site do Banco Central do Brasil (http://www.bcb.gov.br)
   
Pré requisitos
-------

  * Instalação de qualquer versão do Python (http://www.python.org/download)
  
Instalação das dependências
-------

```bash
$ pip install -r requirements.txt
```

Utilização
-------

```bash
$ python sample.py
Inflacao Meta: 4,5
Inflacao acumulada 12 ultimos meses: 9,32
Poupanca: 0,7537
Dolar compra: 3,3197
Dolar venda: 3,3203
Selic meta: 14,25
Selic real: 14,15
```

```bash
>>> import bancocentral
>>> infl = bancocentral.Inflacao()
>>> print('%s' % infl.get_acumulada_tax())
9,32
```

```bash
>>> import bancocentral
>>> selic = bancocentral.Selic()
>>> selic.get_selic_meta()
'14,25'
```

Licença
-------

[Licença MIT](LICENSE)
