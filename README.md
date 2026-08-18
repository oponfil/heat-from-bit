# Heat from Bit: The Thermodynamic Price of Objective Collapse

**Author:** [Oleg Ponfilenok](mailto:ponfil@gmail.com) · Independent researcher

Manuscript proposing that any mechanism of **objective collapse** must pay a thermodynamic price of $k\ln 2$ per destroyed bit of coherence *in the pointer basis of the act*—materialized as heat $\Delta Q = kT\ln 2$ in an environment at temperature $T$. Unitarity is free; the working rule conditions the tariff only on physically delivered objective local pointer records.

| Language | Source | PDF | Notes |
|----------|--------|-----|-------|
| English | [`heat_from_bit_en.tex`](heat_from_bit_en.tex) | [`heat_from_bit_en.pdf`](heat_from_bit_en.pdf) | 7 sections + Declarations |
| Russian | [`heat_from_bit_ru.tex`](heat_from_bit_ru.tex) | [`heat_from_bit_ru.pdf`](heat_from_bit_ru.pdf) | 7 sections + Declarations |

## Summary

The work asks about the **thermodynamic price** of objective collapse—not about choosing a criterion for *when* collapse occurs. Landauer's principle links classical bit erasure to dissipation $Q \ge kT\ln 2$; here the tariff is tied to **coherence in the pointer basis of the act** ($H = S_{\mathrm{coh}} = C_r$), not to subsystem entropy growth under unitary decoherence.

- **State rule:** an affine, nonnegative tariff that vanishes on a complete pointer basis is trivial. The working non-affine rule uses conditional states selected by physical local records; global remote conditioning is discussed only as a stronger signaling variant.
- **Case B vs C:** a heralded single-photon superposition $|{+}\rangle_{\mathrm{ptr}}$ pays $\Delta Q = kT\ln 2$ per objectively fixed act; a locally recorded classical which-path preparation pays nothing.
- **Per-outcome tariff (pure states):** $Q_i = kT\ln(1/p_i)$; for $|{+}\rangle$, $\langle Q\rangle = kT\ln 2$.
- **Origin of heat:** in CSL/GRW the tariff may come from the collapse-model energy reservoir. Otherwise Mandelstam–Tamm only sets an allowance $\Delta E\sim\hbar/(2\tau_{\mathrm{col}})$, not a computed $\Delta\langle\hat{H}\rangle$: if $kT\ln 2$ fits in that window, no extra reservoir is required and the leftover may thermalize. A single act is not microscopically auditable; over $N$ acts one observes $\Delta Q_{\mathrm{tot}} = N\,kT\Delta H$. The first law is violated only locally, in a sub-$\tau_{\mathrm{th}}$ act of non-unitary fixation.
- **Thermal sector:** detailed balance, FIRAS, and Earth's radiation budget constrain which physical preparation records may enter the nonlinear tariff; a positive-P decomposition alone does not solve this open consistency condition.
- **Proposed test:** differential calorimetry in a **heralded Mach–Zehnder** setup—$|{+}\rangle_{\mathrm{ptr}}$ channel vs $I/2_{\mathrm{ptr}}$ control at $T \approx 300$~K; target excess $\Delta Q_{\mathrm{bit}} \approx kT\ln 2$ per herald.

## Structure (English)

1. Introduction  
2. Intuition  
3. Pointer basis and coherence entropy  
4. Thermodynamics of objective collapse  
5. Origin of heat energy  
6. Experimental proposal (heralded MZ)  
7. Discussion  

Declarations follow the main text.

## Repository layout

```
heat_from_bit_en.tex   # English manuscript (LaTeX source)
heat_from_bit_en.pdf   # Compiled English PDF
heat_from_bit_ru.tex   # Russian manuscript (LaTeX source)
heat_from_bit_ru.pdf   # Compiled Russian PDF
refs.bib               # Shared bibliography
build.ps1              # Build script (pdflatex + bibtex)
```

## Building the PDF

Requires a TeX distribution with `pdflatex` and `bibtex` (e.g. [TeX Live](https://www.tug.org/texlive/) or [MiKTeX](https://miktex.org/)).

Build both versions:

```powershell
.\build.ps1
```

Build one version:

```powershell
.\build.ps1 -Targets @("heat_from_bit_en")
.\build.ps1 -Targets @("heat_from_bit_ru")
```

Build artifacts (`.aux`, `.log`, `.bbl`, etc.) are listed in [`.gitignore`](.gitignore).

## Keywords

objective collapse · pointer state · quantum Darwinism · Landauer's principle · heat from bit · entropy collection
