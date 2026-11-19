# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-11-19 14:47 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 41 | 228.5 | 15.4% | +29.4% |
| 🥈 | SolarNet-Ensamble×5 | profe (reto 5) | 41 | 228.9 | 15.4% | +28.9% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 41 | 230.4 | 15.5% | +30.9% |
| 4 | SolarNet-CNN | profe (reto 4) | 41 | 232.0 | 15.6% | +26.8% |
| 5 | SolarNet-Nubes | profe (reto 2) | 41 | 236.6 | 15.9% | +27.5% |
| 6 | SolarNet-GRU | profe | 41 | 238.3 | 16.0% | +25.6% |
| 7 | SolarNet-Transformer | profe (reto 4) | 41 | 240.6 | 16.2% | +25.8% |
| 8 | Persistencia × radiación | profe | 41 | 279.0 | 18.8% | +19.6% |
| 9 | Persistencia 3 días | profe (reto 1) | 41 | 334.1 | 22.5% | +5.1% |
| 10 | Persistencia | profe | 41 | 401.5 | 27.0% | — |

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
