# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-10-21 11:21 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 12 | 189.8 | 13.1% | +26.6% |
| 🥈 | SolarNet-Ponderada | profe (reto 3) | 12 | 207.7 | 14.3% | +24.9% |
| 🥉 | SolarNet-Ensamble×5 | profe (reto 5) | 12 | 210.2 | 14.5% | +22.1% |
| 4 | SolarNet-GRU | profe | 12 | 211.2 | 14.6% | +21.3% |
| 5 | SolarNet-Nubes | profe (reto 2) | 12 | 215.0 | 14.8% | +18.6% |
| 6 | SolarNet-CNN | profe (reto 4) | 12 | 219.0 | 15.1% | +15.0% |
| 7 | SolarNet-Transformer | profe (reto 4) | 12 | 219.8 | 15.2% | +17.0% |
| 8 | Persistencia 3 días | profe (reto 1) | 12 | 257.8 | 17.8% | +4.2% |
| 9 | Persistencia × radiación | profe | 12 | 310.3 | 21.4% | -8.5% |
| 10 | Persistencia | profe | 12 | 345.7 | 23.8% | — |

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
