# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-10-15 11:02 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Ponderada | profe (reto 3) | 6 | 221.0 | 15.7% | -8.3% |
| 🥈 | Persistencia | profe | 6 | 223.7 | 15.9% | — |
| 🥉 | SolarNet-Cuantiles (q50) | profe (reto 6) | 6 | 226.3 | 16.1% | -14.4% |
| 4 | SolarNet-Ensamble×5 | profe (reto 5) | 6 | 235.5 | 16.7% | -16.0% |
| 5 | SolarNet-GRU | profe | 6 | 240.9 | 17.1% | -18.0% |
| 6 | SolarNet-Nubes | profe (reto 2) | 6 | 242.6 | 17.2% | -21.8% |
| 7 | SolarNet-CNN | profe (reto 4) | 6 | 246.5 | 17.5% | -27.3% |
| 8 | SolarNet-Transformer | profe (reto 4) | 6 | 247.1 | 17.5% | -22.9% |
| 9 | Persistencia 3 días | profe (reto 1) | 6 | 249.2 | 17.7% | -28.0% |
| 10 | Persistencia × radiación | profe | 6 | 333.7 | 23.7% | -54.0% |

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
