# Testes de pipelines no rasa

### Quero rodar, como eu faço?

#### Instalação
```
pip install rasa
pip install rasa[spacy]
python -m spacy download en_core_web_md
python -m spacy link en_core_web_md en
```

#### Treinar um novo modelo
```
$ rasa train nlu -c config/{configuration} --fixed-model-name {nomeDoModelo}
```

#### Testar o modelo
```
$ rasa test nlu -u test/{trainDataSet} -m models/{models} --report report/
```

Para mais info, rodar `rasa test nlu -h` ou `rasa train nlu -h`
Ou olhar a documentação do rasa em https://rasa.com/docs/rasa/nlu/using-nlu-only/
