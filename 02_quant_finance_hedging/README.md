# Couverture d'options dans le modèle de Black-Scholes

*Projet de mathématiques appliquées — École Polytechnique, CMAP. Binôme avec **Vincent Neves**.*

## Sujet

Construction d'un **portefeuille de couverture** d'une option sous Black-Scholes discrétisé, et étude de la convergence de l'erreur de réplication, en trois temps :

1. **Théorie** — mesure risque-neutre, **formule de Black-Scholes**, parité call-put, et prix solution d'une **EDP**.
2. **Couverture discrète** — stratégie *delta* ; erreur $\Delta_T^h = V_T^h - \Phi(S_T)$ (empiriquement $\mathbb{E}[|\Delta_T^h|]\propto N^{-1/3}$) ; estimation du *delta* par **Monte-Carlo** ; *payoff* **digital** discontinu (rééchantillonnage adaptatif près de la maturité).
3. **Données de marché** — estimateur de volatilité convergent, appliqué au **DAX**.

## Contenu

- `hedging_black_scholes.ipynb` — notebook complet (démonstrations + code + figures).
- `DAX.csv` — données de clôture pour la calibration.

```bash
pip install numpy scipy matplotlib pandas yfinance
jupyter lab hedging_black_scholes.ipynb
```
