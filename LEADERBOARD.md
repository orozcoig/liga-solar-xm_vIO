# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-11-13 13:59 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Ensamble×5 | profe (reto 5) | 35 | 242.3 | 16.4% | +24.4% |
| 🥈 | SolarNet-Cuantiles (q50) | profe (reto 6) | 35 | 242.9 | 16.5% | +24.7% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 35 | 247.4 | 16.8% | +25.5% |
| 4 | SolarNet-CNN | profe (reto 4) | 35 | 250.0 | 16.9% | +20.8% |
| 5 | SolarNet-GRU | profe | 35 | 251.7 | 17.1% | +21.3% |
| 6 | SolarNet-Nubes | profe (reto 2) | 35 | 253.3 | 17.2% | +22.3% |
| 7 | SolarNet-Transformer | profe (reto 4) | 35 | 256.9 | 17.4% | +20.6% |
| 8 | Persistencia × radiación | profe | 35 | 287.3 | 19.5% | +17.1% |
| 9 | Persistencia 3 días | profe (reto 1) | 35 | 333.6 | 22.6% | +4.6% |
| 10 | Persistencia | profe | 35 | 403.1 | 27.3% | — |

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
