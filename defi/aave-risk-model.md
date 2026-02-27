# Aave v3 Risk Model

Thread version: [X Thread Link](https://x.com/yourlink)

---

## Overview

Aave v3 is an overcollateralized lending protocol.  
Its risk model is built around asset-level configuration and automated liquidation mechanics.

This note analyzes how solvency is maintained.

---

## Core Parameters

- Loan-to-Value (LTV)
- Liquidation Threshold
- Liquidation Bonus
- Supply Caps
- Borrow Caps
- Isolation Mode
- Efficiency Mode (eMode)

These parameters are configurable per asset.

---

## Health Factor Model

Health Factor = (Collateral Value × Liquidation Threshold) / Borrowed Value

If Health Factor < 1 → Position becomes liquidatable.

This creates automated solvency enforcement.

---

## Liquidation Mechanism

- Oracle price feeds determine asset valuation
- Liquidators repay part of the debt
- Liquidators receive collateral + bonus
- Close factor limits how much can be liquidated

System remains solvent through economic incentives.

---

## Strengths

- Granular asset-level risk configuration
- Capital efficiency via eMode
- Isolation mode for tail-risk assets
- Governance-adjustable parameters

---

## Risk Considerations

- Oracle dependency risk
- Liquidity shocks during volatility
- Governance reaction latency
- Correlated collateral risk

---

## Notes

Further areas for deeper analysis:
- Cross-chain risk expansion
- Stablecoin dependency
- Parameter stress testing
