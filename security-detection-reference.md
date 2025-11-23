# Solana Security Detection Command Reference

This document provides a comprehensive list of all program-instruction pairs for running security detection commands.

## Available Detection Commands

Based on the `.claude/commands/` directory, the following detection commands are available:
- `/detect_exfiltration`
- `/detect_dos`
- `/detect_unsynced_wsol_ata`
- `/detect_insufficient_ownership_check`
- `/detect_rounding_bug`
- `/detect_unchecked_type_casting`

## Command Format

```
/detect_[vulnerability_type] [program-name] [instruction-name]
```

## Program: scope

**Program ID:** `HFn8GnPADiny6XqUoWE8uRPPxb29ikn4yTuPa9MF2fWJ`
**Path:** `/home/user/scope/programs/scope`
**Description:** Main Scope oracle aggregator program

### Instructions

1. **initialize**
   ```bash
   /detect_exfiltration scope initialize
   /detect_dos scope initialize
   /detect_unsynced_wsol_ata scope initialize
   /detect_insufficient_ownership_check scope initialize
   /detect_rounding_bug scope initialize
   /detect_unchecked_type_casting scope initialize
   ```

2. **refresh_price_list**
   ```bash
   /detect_exfiltration scope refresh_price_list
   /detect_dos scope refresh_price_list
   /detect_unsynced_wsol_ata scope refresh_price_list
   /detect_insufficient_ownership_check scope refresh_price_list
   /detect_rounding_bug scope refresh_price_list
   /detect_unchecked_type_casting scope refresh_price_list
   ```

3. **refresh_chainlink_price**
   ```bash
   /detect_exfiltration scope refresh_chainlink_price
   /detect_dos scope refresh_chainlink_price
   /detect_unsynced_wsol_ata scope refresh_chainlink_price
   /detect_insufficient_ownership_check scope refresh_chainlink_price
   /detect_rounding_bug scope refresh_chainlink_price
   /detect_unchecked_type_casting scope refresh_chainlink_price
   ```

4. **refresh_pyth_lazer_price**
   ```bash
   /detect_exfiltration scope refresh_pyth_lazer_price
   /detect_dos scope refresh_pyth_lazer_price
   /detect_unsynced_wsol_ata scope refresh_pyth_lazer_price
   /detect_insufficient_ownership_check scope refresh_pyth_lazer_price
   /detect_rounding_bug scope refresh_pyth_lazer_price
   /detect_unchecked_type_casting scope refresh_pyth_lazer_price
   ```

5. **update_mapping_and_metadata**
   ```bash
   /detect_exfiltration scope update_mapping_and_metadata
   /detect_dos scope update_mapping_and_metadata
   /detect_unsynced_wsol_ata scope update_mapping_and_metadata
   /detect_insufficient_ownership_check scope update_mapping_and_metadata
   /detect_rounding_bug scope update_mapping_and_metadata
   /detect_unchecked_type_casting scope update_mapping_and_metadata
   ```

6. **reset_twap**
   ```bash
   /detect_exfiltration scope reset_twap
   /detect_dos scope reset_twap
   /detect_unsynced_wsol_ata scope reset_twap
   /detect_insufficient_ownership_check scope reset_twap
   /detect_rounding_bug scope reset_twap
   /detect_unchecked_type_casting scope reset_twap
   ```

7. **set_admin_cached**
   ```bash
   /detect_exfiltration scope set_admin_cached
   /detect_dos scope set_admin_cached
   /detect_unsynced_wsol_ata scope set_admin_cached
   /detect_insufficient_ownership_check scope set_admin_cached
   /detect_rounding_bug scope set_admin_cached
   /detect_unchecked_type_casting scope set_admin_cached
   ```

8. **approve_admin_cached**
   ```bash
   /detect_exfiltration scope approve_admin_cached
   /detect_dos scope approve_admin_cached
   /detect_unsynced_wsol_ata scope approve_admin_cached
   /detect_insufficient_ownership_check scope approve_admin_cached
   /detect_rounding_bug scope approve_admin_cached
   /detect_unchecked_type_casting scope approve_admin_cached
   ```

9. **create_mint_map**
   ```bash
   /detect_exfiltration scope create_mint_map
   /detect_dos scope create_mint_map
   /detect_unsynced_wsol_ata scope create_mint_map
   /detect_insufficient_ownership_check scope create_mint_map
   /detect_rounding_bug scope create_mint_map
   /detect_unchecked_type_casting scope create_mint_map
   ```

10. **close_mint_map**
    ```bash
    /detect_exfiltration scope close_mint_map
    /detect_dos scope close_mint_map
    /detect_unsynced_wsol_ata scope close_mint_map
    /detect_insufficient_ownership_check scope close_mint_map
    /detect_rounding_bug scope close_mint_map
    /detect_unchecked_type_casting scope close_mint_map
    ```

11. **resume_chainlinkx_price**
    ```bash
    /detect_exfiltration scope resume_chainlinkx_price
    /detect_dos scope resume_chainlinkx_price
    /detect_unsynced_wsol_ata scope resume_chainlinkx_price
    /detect_insufficient_ownership_check scope resume_chainlinkx_price
    /detect_rounding_bug scope resume_chainlinkx_price
    /detect_unchecked_type_casting scope resume_chainlinkx_price
    ```

---

## Program: perpetuals (JUP Perpetual Protocol)

**Program ID:** `PERPHjGBqRHArX4DySjwM6UJHiR3sWAatqfdBS2qQJu`
**Path:** `/home/user/scope/programs/jup-perp-itf`
**Description:** Interface to interact with JUP Perpetual Protocol

### Instructions

1. **get_assets_under_management**
   ```bash
   /detect_exfiltration perpetuals get_assets_under_management
   /detect_dos perpetuals get_assets_under_management
   /detect_unsynced_wsol_ata perpetuals get_assets_under_management
   /detect_insufficient_ownership_check perpetuals get_assets_under_management
   /detect_rounding_bug perpetuals get_assets_under_management
   /detect_unchecked_type_casting perpetuals get_assets_under_management
   ```

---

## Interface-Only Programs (No Instructions)

The following programs are interface definitions only and contain no instruction implementations:

1. **adrena** - `programs/adrena-perp-itf`
2. **flashtrade** - `programs/flashtrade-perp-itf`
3. **perpetuals (LB CLMM)** - `programs/lb-clmm-itf`
4. **redstone-itf** - `programs/redstone-itf`
5. **sbod-itf** - `programs/sbod-itf`
6. **securitize-itf** - `programs/securitize-itf`
7. **switchbord-itf** - `programs/switchbord-itf`

---

## Summary

- **Total Programs:** 9
- **Programs with Instructions:** 2
- **Total Instructions:** 12
  - scope: 11 instructions
  - perpetuals: 1 instruction

## Quick Command List (All Program-Instruction Pairs)

For easy copy-paste, here are all valid program-instruction pairs:

```
scope initialize
scope refresh_price_list
scope refresh_chainlink_price
scope refresh_pyth_lazer_price
scope update_mapping_and_metadata
scope reset_twap
scope set_admin_cached
scope approve_admin_cached
scope create_mint_map
scope close_mint_map
scope resume_chainlinkx_price
perpetuals get_assets_under_management
```
