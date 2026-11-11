# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-11-11 14:04 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Ensamble×5 | profe (reto 5) | 33 | 245.1 | 16.9% | +23.7% |
| 🥈 | SolarNet-Cuantiles (q50) | profe (reto 6) | 33 | 246.2 | 17.0% | +23.9% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 33 | 250.0 | 17.3% | +25.0% |
| 4 | SolarNet-GRU | profe | 33 | 254.6 | 17.6% | +20.5% |
| 5 | SolarNet-CNN | profe (reto 4) | 33 | 255.7 | 17.7% | +19.0% |
| 6 | SolarNet-Nubes | profe (reto 2) | 33 | 258.4 | 17.9% | +20.9% |
| 7 | SolarNet-Transformer | profe (reto 4) | 33 | 260.7 | 18.0% | +19.6% |
| 8 | Persistencia × radiación | profe | 33 | 294.0 | 20.3% | +15.6% |
| 9 | Persistencia 3 días | profe (reto 1) | 33 | 321.5 | 22.2% | +9.3% |
| 10 | Persistencia | profe | 33 | 408.4 | 28.2% | — |

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
