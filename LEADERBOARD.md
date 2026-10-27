# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-10-27 12:06 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 18 | 208.9 | 14.7% | +28.6% |
| 🥈 | SolarNet-CNN | profe (reto 4) | 18 | 224.1 | 15.8% | +22.9% |
| 🥉 | SolarNet-Ensamble×5 | profe (reto 5) | 18 | 224.7 | 15.8% | +24.9% |
| 4 | SolarNet-Ponderada | profe (reto 3) | 18 | 225.0 | 15.8% | +26.3% |
| 5 | SolarNet-Transformer | profe (reto 4) | 18 | 226.8 | 16.0% | +22.6% |
| 6 | SolarNet-Nubes | profe (reto 2) | 18 | 231.1 | 16.3% | +21.8% |
| 7 | SolarNet-GRU | profe | 18 | 232.8 | 16.4% | +22.3% |
| 8 | Persistencia × radiación | profe | 18 | 276.6 | 19.5% | +8.7% |
| 9 | Persistencia 3 días | profe (reto 1) | 18 | 303.6 | 21.4% | -3.6% |
| 10 | Persistencia | profe | 18 | 359.4 | 25.3% | — |

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
