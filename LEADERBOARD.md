# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-11-06 13:44 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 28 | 239.9 | 16.5% | +31.6% |
| 🥈 | SolarNet-Ensamble×5 | profe (reto 5) | 28 | 242.2 | 16.7% | +30.2% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 28 | 249.1 | 17.2% | +30.5% |
| 4 | SolarNet-GRU | profe | 28 | 253.9 | 17.5% | +26.8% |
| 5 | SolarNet-CNN | profe (reto 4) | 28 | 254.2 | 17.5% | +25.7% |
| 6 | SolarNet-Nubes | profe (reto 2) | 28 | 258.9 | 17.8% | +26.5% |
| 7 | SolarNet-Transformer | profe (reto 4) | 28 | 260.5 | 18.0% | +26.1% |
| 8 | Persistencia × radiación | profe | 28 | 300.8 | 20.7% | +15.7% |
| 9 | Persistencia 3 días | profe (reto 1) | 28 | 330.4 | 22.8% | +6.0% |
| 10 | Persistencia | profe | 28 | 416.7 | 28.7% | — |

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
