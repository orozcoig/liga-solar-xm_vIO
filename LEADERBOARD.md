# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-11-16 16:27 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 38 | 236.7 | 15.8% | +27.2% |
| 🥈 | SolarNet-Ensamble×5 | profe (reto 5) | 38 | 237.6 | 15.9% | +26.5% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 38 | 239.9 | 16.1% | +28.2% |
| 4 | SolarNet-CNN | profe (reto 4) | 38 | 240.1 | 16.1% | +24.4% |
| 5 | SolarNet-GRU | profe | 38 | 245.9 | 16.5% | +23.7% |
| 6 | SolarNet-Nubes | profe (reto 2) | 38 | 246.4 | 16.5% | +24.9% |
| 7 | SolarNet-Transformer | profe (reto 4) | 38 | 251.4 | 16.8% | +22.9% |
| 8 | Persistencia × radiación | profe | 38 | 287.9 | 19.3% | +17.5% |
| 9 | Persistencia 3 días | profe (reto 1) | 38 | 326.4 | 21.8% | +7.1% |
| 10 | Persistencia | profe | 38 | 402.0 | 26.9% | — |

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
