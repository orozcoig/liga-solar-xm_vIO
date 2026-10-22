# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-10-22 11:21 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 13 | 193.1 | 13.3% | +27.6% |
| 🥈 | SolarNet-Ensamble×5 | profe (reto 5) | 13 | 211.6 | 14.5% | +23.5% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 13 | 211.8 | 14.5% | +25.4% |
| 4 | SolarNet-Transformer | profe (reto 4) | 13 | 219.2 | 15.0% | +19.2% |
| 5 | SolarNet-CNN | profe (reto 4) | 13 | 221.6 | 15.2% | +16.4% |
| 6 | SolarNet-Nubes | profe (reto 2) | 13 | 223.4 | 15.3% | +18.3% |
| 7 | SolarNet-GRU | profe | 13 | 224.6 | 15.4% | +19.6% |
| 8 | Persistencia 3 días | profe (reto 1) | 13 | 245.5 | 16.8% | +9.6% |
| 9 | Persistencia × radiación | profe | 13 | 294.3 | 20.2% | -2.2% |
| 10 | Persistencia | profe | 13 | 348.6 | 23.9% | — |

![último día](resultados/ultimo_dia.png)

## 🧪 Backtest (días pasados, para arrancar en frío)

_Ojo: en el backtest el 'pronóstico' de clima es casi el clima observado → resultados optimistas._

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-GRU | profe | 30 | 149.7 | 9.8% | +43.5% |
| 🥈 | SolarNet-Cuantiles (q50) | profe (reto 6) | 30 | 154.1 | 10.1% | +42.1% |
| 🥉 | SolarNet-Ensamble×5 | profe (reto 5) | 30 | 157.2 | 10.3% | +41.5% |
| 4 | SolarNet-Nubes | profe (reto 2) | 30 | 158.2 | 10.4% | +41.3% |
| 5 | SolarNet-Transformer | profe (reto 4) | 30 | 160.0 | 10.5% | +39.9% |
| 6 | SolarNet-Ponderada | profe (reto 3) | 30 | 171.0 | 11.2% | +37.7% |
| 7 | SolarNet-CNN | profe (reto 4) | 30 | 178.3 | 11.7% | +33.4% |
| 8 | Persistencia × radiación | profe | 30 | 217.0 | 14.2% | +22.4% |
| 9 | Persistencia 3 días | profe (reto 1) | 30 | 268.5 | 17.6% | +14.1% |
| 10 | Persistencia | profe | 30 | 319.4 | 20.9% | — |

![backtest](resultados/backtest.png)
