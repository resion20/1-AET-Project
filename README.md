# 1-AET-Project
AET is a complete, end-to-end study of a mixed air–water HVAC system for the DENERG building at Politecnico di Torino.
It covers building loads, psychrometrics, refrigeration cycle sizing, duct & pipe networks, energy/cost estimates, exergy analysis, and thermal sizing of heat exchangers (fan-coil core).

1) Building Model & Loads

Representative floor modeling; 1958 envelope approximations.

Typical U-values (pre-retrofit): walls ~1.41, windows ~3.68, roof ~1.30, basement ~1.15 W/m²K.

Design conditions:

Winter: indoor 20 °C (offices) / 18 °C (lab), outdoor −8 °C

Summer: indoor 25 °C (offices) / 24 °C (lab), outdoor 30.5 °C

Ventilation: natural for offices (windows), mechanical for labs (e.g., ~0.5 vol/h winter to limit loads).

Solar gains estimated per façade using PV data and window distribution.

Peak loads (baseline):

Heating: ~402 kW total

Cooling: ~177 kW total (≈ 89 kW offices + 88 kW labs)

Envelope upgrade scenario (e.g., 8 cm EPS on walls/roof) reduces loads to ~300 kW heating and 155 kW cooling (≈ −25% / −13%).

2) Psychrometrics (Air Handling)

Winter (lab AHU): Mix → pre-heater → humidifier → supply ~32 °C (to reduce airflow/Δp).

Summer (lab AHU): Mix → cooling coil (dehumidify to ~saturation) → reheat → supply ~15 °C.

Example duty (critical lab storey): cooler ≈ −69 kW; reheat ≈ +9 kW (summer).

3) Refrigeration Cycle Sizing

Refrigerant: R134a (CoolProp/CoolPack properties), compressor η_is ≈ 0.8.

Summer: Q̇L ≈ 177 kW, Ẇc ≈ 39 kW, COP ≈ 4.6, Q̇H ≈ 216 kW (can reuse for reheat).

Winter (heat pump mode): Q̇H ≈ 402 kW, Ẇc ≈ 178 kW, COP ≈ 2.3.

4) Distribution Networks (Ducts & Pipes)

Air (labs): square ducts sized ~1.5 m/s, equivalent diameters (Hübscher), friction (Caleffi), local losses.

Two lab floors example: Δp ≈ 111 Pa, fan power ≈ 1.0 kW.

Water (fan coils, worst loop): Δp totals from friction + fittings + geodetic head.

Example loop: Δp ≈ 3.1×10⁵ Pa, pump power ≈ 0.18 kW.

5) Energy, Cost & Exergy

Daily energy from normalized hourly demand curves (summer/winter).

Summer compressor ≈ 705 kWh/day, Winter ≈ 3247 kWh/day (baseline).

With 8 cm EPS: Summer ≈ 617 kWh/day, Winter ≈ 2425 kWh/day.

Exergy analysis: Dead states set for humid air/water/R134a; compute exergy streams and irreversibilities per component. Major losses concentrate in the cooling coil and compression train—priority areas for improvement.

6) Thermal Design (Heat Exchangers)

ε–NTU approach, convection (e.g., Zhukauskas correlations).

Fan-coil core:

Summer is sizing driver: ~20 tubes with fins (ηₒᵥ ~0.97) vs ~30 without fins to hit duty.

Overall U rises from ~374 → 556 W/m²K with finned design.
