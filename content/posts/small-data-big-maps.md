+++
date = '2026-06-16T22:09:28-03:00'
draft = false
title = 'Small Data, Big Maps: notas de campo de um artigo'
tags = ['machine-learning', 'geoespacial', 'amazonia', 'validacao-espacial']
+++

Na Amazônia, ter 150 amostras no Excel não significa ter 150 amostras para o modelo. Significa ter 20 por estrato, em alguns casos menos. E cada parcela custa o equivalente a um bom computador de ML — barco, equipe, equipamento, janela climática. Quando alguém diz "coleta mais dados", está dando um conselho metodologicamente correto e operacionalmente impossível.

Esse foi o ponto de partida do artigo que publiquei no Towards Data Science. Nele, discuto como treinar modelos geoespaciais quando as amostras são escassas, caras e imperfeitas. O foco não é uma receita pronta, mas os trade-offs que aparecem na prática.

O artigo nasceu de momentos de campo e de laboratório em que as métricas de validação pareciam ótimas, mas o mapa não fazia sentido geográfico. O modelo estava interpolando vizinhanças, não generalizando padrões.

Se quiser ler a versão técnica completa, está disponível aqui:

👉 [Small Data, Big Maps: Training Geospatial ML Models When Samples Are Scare](https://towardsdatascience.com/small-data-big-maps-training-geospatial-ml-models-when-samples-are-scarce/)

É um texto para quem trabalha com dados ambientais e já se viu tentando justificar um modelo que performa bem na planilha, mas hesita no terreno.
