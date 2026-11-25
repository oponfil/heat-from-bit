# Heat from Bit: The Thermodynamic Price of Objective Collapse

**Author:** Oleg Ponfilenok · Independent researcher

Manuscript proposing the hypothesis that any mechanism of **objective collapse** must pay a thermodynamic price of $k\ln 2$ per destroyed bit of coherence *in the pointer basis of the act*. The price is paid as heat $\Delta Q = kT\ln 2$ in an absorber at temperature $T$. This is new energy: the first law is violated, while unitary evolution is free.

| Language | Source | PDF | Notes |
|----------|--------|-----|-------|
| English | [`heat_from_bit_en.tex`](heat_from_bit_en.tex) | [`heat_from_bit_en.pdf`](heat_from_bit_en.pdf) | 7 sections + Declarations + 2 appendices |
| Russian | [`heat_from_bit_ru.tex`](heat_from_bit_ru.tex) | [`heat_from_bit_ru.pdf`](heat_from_bit_ru.pdf) | 7 sections + Declarations + 2 appendices |

The two versions have the same content.

## Summary

The work asks about the **thermodynamic price** of objective collapse, not about a criterion for *when* collapse occurs. The tariff is tied to **coherence in the pointer basis of the act** ($H = S_{\mathrm{coh}} = C_r$), not to the growth of subsystem entropy under unitary decoherence.

- **Hypothesis:** $\delta Q = T\,\mathrm{d}S_{\mathrm{col}}$. The entropy created by objective collapse behaves as if it had been supplied as heat. The first law is violated by exactly this amount; the addition does not follow from Landauer's principle and is a postulate.
- **State rule:** the tariff is evaluated on the state conditioned only on a physically delivered local record. Unpolarized thermal light pays nothing. A nontrivial nonnegative tariff that vanishes on pointer-diagonal states cannot be an affine functional of one local density matrix.
- **Per-outcome tariff (pure states):** $Q_i = kT\ln(1/p_i)$; for $|{+}\rangle$, $\langle Q\rangle = kT\ln 2$.
- **Absorption site:** a bit exists only if the two branches lead to different states of the absorber by the moment of collapse, as in a two-slit experiment where both paths meet at one point of the screen and no which-slit bit arises.
- **Proposed tests:** calorimetry of a heralded single-photon qubit in a Mach–Zehnder interferometer ($|{+}\rangle_{\mathrm{ptr}}$ against the $I/2_{\mathrm{ptr}}$ control, $kT\ln 2$ per act, about 2.2% of the photon energy at 1550 nm and 300 K), and a simpler test with polarized incoherent light from two light-emitting diodes.
- **Existing data:** calorimetric and radiometric constraints, and why they do not exclude the hypothesis.

## Structure

1. Introduction  
2. Intuition  
3. Pointer basis and coherence entropy  
4. Thermodynamics of objective collapse  
5. Energy of the payment and the first law  
6. Experimental proposal  
7. Discussion  

Statements and Declarations follow the main text. Two appendices: dephasing and the moment of collapse on photon absorption; calorimetry of the collapse of nuclear coherence ($^{129}$Xe).

## Repository layout

```
heat_from_bit_en.tex   # English manuscript (LaTeX source)
heat_from_bit_en.pdf   # Compiled English PDF
heat_from_bit_ru.tex   # Russian manuscript (LaTeX source)
heat_from_bit_ru.pdf   # Compiled Russian PDF
refs.bib               # Shared bibliography
build.ps1              # Windows build script (pdflatex + bibtex)
```

## Building the PDF

On macOS, build with [Tectonic](https://tectonic-typesetting.github.io/), which runs all passes and BibTeX itself:

```bash
tectonic heat_from_bit_en.tex
tectonic heat_from_bit_ru.tex
```

The Russian version is typeset in Avenir Next (a macOS system font) and needs XeTeX, i.e. Tectonic or `xelatex`. Under `pdflatex` it falls back to Comfortaa.

On Windows, with a TeX distribution that has `pdflatex` and `bibtex` (e.g. [TeX Live](https://www.tug.org/texlive/) or [MiKTeX](https://miktex.org/)):

```powershell
.\build.ps1
.\build.ps1 -Targets @("heat_from_bit_en")
```

Build artifacts (`.aux`, `.log`, `.bbl`, etc.) are listed in [`.gitignore`](.gitignore).

## Keywords

objective collapse · pointer basis · quantum Darwinism · Landauer's principle · heat from bit · tariff per bit

## License

The text of the manuscript is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
