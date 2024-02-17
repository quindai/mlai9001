# Modelo de Previsão com Azure Machine Learning

## Tutorial Pages 
| Tutorial Pages                            | Best Model                            | 
| ----------------------------------- | ----------------------------------- |
| <img src="utils/azure1.png" alt="Tutorial Pages" width="250vw"/> | ![Best Model](utils/azure2.jpeg) |

## Melhor modelo encontrado pelo AutoML
Observe que as métricas do melhor modelo `maroon_line_k4hh47vg` algoritmo `MaxAbsScaler, LightGBM`, estão descritas abaixo e print da tela em seguida:
```
Variância explicada
0.77238
Erro absoluto de média
189.81
Erro de percentual absoluto de média
37.659
Erro mediano absoluto
112.35
Erro absoluto de média normalizado
0.055694
Erro mediano absoluto normalizado
0.032966
Erro de quadrado de média de raiz normalizado
0.092708
Erro de log de quadrado de média raiz normalizado
0.059429
Pontuação R2
0.77234
Erro de raiz do valor quadrático médio
315.95
Erro de log de raiz do valor quadrático médio
0.41815
Correlação de Spearman
0.91543
```
| Print das Métricas do melhor modelo                       
| ----------------------------------- |
| <img src="utils/azure3.jpeg" alt="Print das Métricas do melhor modelo"/> |

### Considerações sobre o RMSE - Erro Quadrático Médio Normalizado
Observe que dentre os 3 algoritmos, o que apresenta melhor RMSE é o VotingEnsemble com 92,71% de RMSE.
Sendo um forte candidato para implantação num ponto de extremidade.
| Print das Métricas do melhor modelo                       
| ----------------------------------- |
| <img src="utils/azure4.jpeg" alt="RMSE"/> |

Para replicar os passos acima, usei as seguintes configurações do modelo:
> Com o modelo criado, você poderá visualizar essas configurações indo em `Tarefas (Jobs)` no menu lateral, e depois clicar em `mslearn-bike-automl`.
| Print das Métricas do melhor modelo                       
| ----------------------------------- |
| <img src="utils/azure5.jpeg" alt="RMSE"/> |

Links Importantes:
* https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/02-content-safety.html
* https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html
* https://learn.microsoft.com/pt-br/azure/machine-learning/how-to-use-automated-ml-for-ml-models?view=azureml-api-2
* https://learn.microsoft.com/pt-br/azure/machine-learning/tutorial-first-experiment-automated-ml?view=azureml-api-2
* https://learn.microsoft.com/pt-br/azure/machine-learning/concept-endpoints?view=azureml-api-2
