# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-10-28 12:43 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 19 | 209.6 | 14.7% | +30.3% |
| 🥈 | SolarNet-Ensamble×5 | profe (reto 5) | 19 | 223.6 | 15.7% | +27.0% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 19 | 224.7 | 15.8% | +28.2% |
| 4 | SolarNet-CNN | profe (reto 4) | 19 | 226.0 | 15.9% | +24.6% |
| 5 | SolarNet-Transformer | profe (reto 4) | 19 | 227.4 | 16.0% | +24.5% |
| 6 | SolarNet-Nubes | profe (reto 2) | 19 | 229.7 | 16.1% | +24.1% |
| 7 | SolarNet-GRU | profe | 19 | 230.8 | 16.2% | +24.7% |
| 8 | Persistencia × radiación | profe | 19 | 275.1 | 19.3% | +11.2% |
| 9 | Persistencia 3 días | profe (reto 1) | 19 | 300.9 | 21.1% | -0.4% |
| 10 | Persistencia | profe | 19 | 371.1 | 26.0% | — |

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
