# Full structure and descriptions of Pump.fun and PumpSwap IDLs.

> _IDK why but I couldn't find these on anchor-py._


---
# Example usages

```python
# PumpSwap Pool struct
Pool = Struct(
    "discriminator" / Bytes(8),
    "pool_bump" / Int8ul,
    "index" / Int16ul,
    "creator" / Bytes(32),
    "base_mint" / Bytes(32),
    "quote_mint" / Bytes(32),
    "lp_mint" / Bytes(32),
    "pool_base_token_account" / Bytes(32),
    "pool_quote_token_account" / Bytes(32),
    "lp_supply" / Int64ul,
)
```

```python
# Pump.fun Bonding Curve struct
BondingCurve = Struct(
    "discriminator" / Bytes(8),
    "virtual_token_reserves" / Int64ul,
    "virtual_sol_reserves" / Int64ul,
    "real_token_reserves" / Int64ul,
    "real_sol_reserves" / Int64ul,
    "token_total_supply" / Int64ul,
    "complete" / Flag,
    "creator" / Bytes(32),
)
```

---
