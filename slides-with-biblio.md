
---

:::: {.columns}
::: {.column width="50%"}
### Machine 3: Part Resistance

**Settings:** 373 K, 300 kPa

This control chart analyzes the individual measurements for `PartResistance`. 

Key Parameters:
- **Variable:** PartResistance (Ohms)
- **Control Limits:** $\pm 3\sigma$

If the points remain within the dashed red lines, the process variation is considered stable.
:::

::: {.column width="50%"}
<iframe
  data-src='media/plots/control_m3_t373_p300.html'
  width='100%'
  height='500px'
  style='border:none;'>
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1: Distribution Analysis

This histogram shows the frequency distribution of `PartLength` for Machine 1.

Key Insights:
- **Center:** The average measurement value.
- **Spread:** The variation in part production.
- **Shape:** Checks for normality or skewness in the process.
:::

::: {.column width="50%"}
<iframe
  data-src='media/plots/hist_m1.html'
  width='100%'
  height='500px'
  style='border:none;'>
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2: Process Capability

Evaluation of Machine 2's ability to meet specifications ($48mm - 52mm$).

**Capability Metrics:**
- **Cp**: Potential process capability.
- **Cpk**: Actual capability (accounts for centering).

Machine 2 typically demonstrates higher stability and centering compared to Machine 1.
:::

::: {.column width="50%"}
<iframe
  data-src='media/plots/capability_m2.html'
  width='100%'
  height='500px'
  style='border:none;'>
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2: Process Stability

This control chart monitors the `PartLength` for all Machine 2 observations to ensure the process remains in statistical control.

**Analysis:**
- **Stability:** Checks if measurements stay within the control limits ($\pm 3\sigma$).
- **Center Line:** Represents the process average.
- **Control Limits:** Define the boundaries of natural process variation.
:::

::: {.column width="50%"}
<iframe
  data-src='media/plots/control_m2_all.html'
  width='100%'
  height='500px'
  style='border:none;'>
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2: Process Stability

Individual control chart for `PartLength` across all observations for Machine 2.

- **Stability:** Process shows consistent performance within $\pm 3\sigma$.
- **Center:** Closely aligned with the target.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/control_m2.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2: Process Capability

Capability analysis with limits set at [48mm, 52mm].

- **Cpk:** Significant improvement over Machine 1.
- **Yield:** High probability of conforming parts.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/capability_m2.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---
# Bibliography
<div id="refs"></div>
