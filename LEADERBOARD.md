# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-10-13 13:43 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Ponderada | profe (reto 3) | 4 | 187.7 | 13.2% | -6.8% |
| 🥈 | Persistencia | profe | 4 | 192.5 | 13.5% | — |
| 🥉 | SolarNet-Ensamble×5 | profe (reto 5) | 4 | 208.7 | 14.7% | -18.9% |
| 4 | SolarNet-Cuantiles (q50) | profe (reto 6) | 4 | 210.5 | 14.8% | -19.9% |
| 5 | SolarNet-GRU | profe | 4 | 213.6 | 15.0% | -21.0% |
| 6 | SolarNet-Transformer | profe (reto 4) | 4 | 220.8 | 15.5% | -25.6% |
| 7 | SolarNet-Nubes | profe (reto 2) | 4 | 225.6 | 15.8% | -27.6% |
| 8 | SolarNet-CNN | profe (reto 4) | 4 | 229.4 | 16.1% | -31.2% |
| 9 | Persistencia 3 días | profe (reto 1) | 4 | 234.4 | 16.5% | -32.9% |
| 10 | Persistencia × radiación | profe | 4 | 344.6 | 24.2% | -79.2% |

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
