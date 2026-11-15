# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-11-15 13:16 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 37 | 238.3 | 16.0% | +26.5% |
| 🥈 | SolarNet-Ensamble×5 | profe (reto 5) | 37 | 238.9 | 16.0% | +25.9% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 37 | 242.1 | 16.2% | +27.4% |
| 4 | SolarNet-CNN | profe (reto 4) | 37 | 243.1 | 16.3% | +23.3% |
| 5 | SolarNet-GRU | profe | 37 | 247.3 | 16.6% | +23.1% |
| 6 | SolarNet-Nubes | profe (reto 2) | 37 | 248.2 | 16.7% | +24.2% |
| 7 | SolarNet-Transformer | profe (reto 4) | 37 | 253.9 | 17.0% | +22.0% |
| 8 | Persistencia × radiación | profe | 37 | 286.1 | 19.2% | +17.9% |
| 9 | Persistencia 3 días | profe (reto 1) | 37 | 328.8 | 22.1% | +6.4% |
| 10 | Persistencia | profe | 37 | 403.0 | 27.0% | — |

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
