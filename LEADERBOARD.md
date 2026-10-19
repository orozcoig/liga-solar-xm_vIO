# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-10-19 13:00 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 10 | 197.2 | 13.4% | +18.3% |
| 🥈 | SolarNet-Ponderada | profe (reto 3) | 10 | 216.4 | 14.7% | +17.0% |
| 🥉 | SolarNet-Ensamble×5 | profe (reto 5) | 10 | 218.3 | 14.8% | +13.7% |
| 4 | SolarNet-GRU | profe | 10 | 219.8 | 14.9% | +12.6% |
| 5 | SolarNet-Nubes | profe (reto 2) | 10 | 223.3 | 15.1% | +9.6% |
| 6 | SolarNet-CNN | profe (reto 4) | 10 | 224.4 | 15.2% | +6.0% |
| 7 | SolarNet-Transformer | profe (reto 4) | 10 | 231.5 | 15.7% | +7.2% |
| 8 | Persistencia 3 días | profe (reto 1) | 10 | 279.3 | 18.9% | -8.6% |
| 9 | Persistencia | profe | 10 | 311.6 | 21.1% | — |
| 10 | Persistencia × radiación | profe | 10 | 333.6 | 22.6% | -22.8% |

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
