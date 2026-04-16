# tech_cells_generic

Vyges catalog mirror of [pulp-platform/tech_cells_generic](https://github.com/pulp-platform/tech_cells_generic) — technology-abstract cells for simulation and FPGA targets.

Provides `tc_clk_*` (clock gating, mux, inverter, buffer, delay), `tc_pwr_*` (power cells), `tc_sram*` (technology-abstract SRAM). Xilinx-specific versions under `fpga/`. Deprecated PULP-prefixed aliases under `deprecated/`.

## Used by

- `vyges-ip/pulp-riscv-dbg` (debug module uses `tc_clk_inverter`, `tc_clk_mux2` in `dmi_jtag_tap`)
- `vyges-ip/common_cells` (runtime tie-offs)
- Any Vyges IP sourced from a PULP upstream that instantiates technology-abstract glue

## License

Solderpad Hardware License 0.51 — Licensees may opt to treat the Work as Apache 2.0 licensed. See `LICENSE`.

## Upstream sync

Commit pinned in `upstream.yaml`. Weekly sync via `.github/workflows/upstream-sync.yml`.
