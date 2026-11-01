# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-11-01 12:27 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | Persistencia × radiación | profe | 23 | 1416.3 | 49.6% | -5.8% |
| 🥈 | Persistencia | profe | 23 | 1452.5 | 50.9% | — |
| 🥉 | SolarNet-CNN | profe (reto 4) | 23 | 1452.6 | 50.9% | -10.1% |
| 4 | SolarNet-Ensamble×5 | profe (reto 5) | 23 | 1456.4 | 51.0% | -10.2% |
| 5 | SolarNet-GRU | profe | 23 | 1457.4 | 51.0% | -10.5% |
| 6 | SolarNet-Cuantiles (q50) | profe (reto 6) | 23 | 1459.0 | 51.1% | -11.1% |
| 7 | SolarNet-Ponderada | profe (reto 3) | 23 | 1460.4 | 51.1% | -11.0% |
| 8 | Persistencia 3 días | profe (reto 1) | 23 | 1461.1 | 51.2% | -5.2% |
| 9 | SolarNet-Nubes | profe (reto 2) | 23 | 1463.9 | 51.3% | -10.9% |
| 10 | SolarNet-Transformer | profe (reto 4) | 23 | 1473.4 | 51.6% | -11.9% |

![último día](resultados/ultimo_dia.png)

## 🧪 Backtest (días pasados, para arrancar en frío)

_Ojo: en el backtest el 'pronóstico' de clima es casi el clima observado → resultados optimistas._

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-GRU | profe | 30 | 267.2 | 16.1% | +33.1% |
| 🥈 | SolarNet-Cuantiles (q50) | profe (reto 6) | 30 | 273.3 | 16.5% | +31.6% |
| 🥉 | SolarNet-Transformer | profe (reto 4) | 30 | 273.6 | 16.5% | +30.1% |
| 4 | SolarNet-Ensamble×5 | profe (reto 5) | 30 | 275.1 | 16.6% | +31.2% |
| 5 | SolarNet-Nubes | profe (reto 2) | 30 | 278.6 | 16.8% | +30.4% |
| 6 | SolarNet-Ponderada | profe (reto 3) | 30 | 288.4 | 17.4% | +27.7% |
| 7 | SolarNet-CNN | profe (reto 4) | 30 | 289.9 | 17.5% | +24.5% |
| 8 | Persistencia × radiación | profe | 30 | 317.7 | 19.2% | +14.8% |
| 9 | Persistencia 3 días | profe (reto 1) | 30 | 335.0 | 20.2% | +12.7% |
| 10 | Persistencia | profe | 30 | 376.8 | 22.7% | — |

![backtest](resultados/backtest.png)
