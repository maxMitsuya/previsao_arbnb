# 🏠 Airbnb Rio: Modelo de Precificação de Imóveis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0.2-orange)
![Pandas](https://img.shields.io/badge/Pandas-1.4.0-red)

Projeto de machine learning para previsão de diárias de imóveis no Airbnb Rio, ajudando anfitriões e locadores a determinar preços justos.

## 🎯 Objetivo
Desenvolver um modelo preditivo que:
- Estime valores adequados para diárias
- Ajude anfitriões a precificar seus imóveis
- Permita locadores identificar ofertas atrativas

## 📂 Dataset
**Fonte**: Kaggle (Dados do Airbnb Rio 2018-2020)  
**Variáveis Principais**:
- `price`: Preço da diária (target)
- `property_type`: Tipo de imóvel
- `room_type`: Tipo de quarto
- `accommodates`: Capacidade de hóspedes
- `location`: Latitude/Longitude
- 20+ outras características

**Pré-processamento**:
- Tratamento de outliers e valores faltantes
- Conversão de moeda e tipos de dados
- Encoding de variáveis categóricas
- Engenharia de features (ex: contagem de amenities)

## 🔍 Análise Exploratória

### Mapa de Calor de Preços
![Mapa de Densidade](https://github.com/maxMitsuya/previsao_arbnb/blob/main/rio_heat_map.png)
*Concentração de preços por região do Rio*

### Correlações Principais
![Matriz de Correlação](https://github.com/maxMitsuya/previsao_arbnb/blob/main/correlation_matrix.png)
*Relação entre variáveis numéricas*

## 🤖 Modelagem Preditiva

### Comparação de Algoritmos
| Modelo | R² | RMSE |
|--------|----|------|
| Extra Trees | 97.5% | 38.21 |
| Random Forest | 97.3% | 39.85 | 
| Regressão Linear | 62.8% | 142.60 |

### Features Mais Importantes
![Feature Importance](https://github.com/maxMitsuya/previsao_arbnb/blob/main/feature_importance.png)
*Impacto das variáveis no modelo final*

## 💡 Insights e Aplicações

### Fatores que Mais Impactam o Preço:
1. **Capacidade** (número de hóspedes)
2. **Tipo de Imóvel** (apartamentos inteiros valem mais)
3. **Localização** (zonas turísticas têm premium)
4. **Comodidades** (quantidade e qualidade)
5. **Politica de Cancelamento** (flexível aumenta valor)

### Como Usar os Resultados:
- **Para Anfitriões**: 
  - Simule diferentes configurações para maximizar receita
  - Descubra quais melhorias no imóvel trazem maior ROI
  
- **Para Locadores**:
  - Compare preços de imóveis similares
  - Identifique ofertas abaixo da média de mercado

## 📌 Próximos Passos
1. Desenvolver aplicativo web para simulações
2. Adicionar dados sazonais para preços dinâmicos
3. Incorporar avaliações de hóspedes ao modelo
4. Criar sistema de recomendação personalizada
