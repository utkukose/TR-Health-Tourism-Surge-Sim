<h1 align="center">TR-Health-Tourism-Surge-Sim</h1>

<p align="center">
  <strong>If a crisis happened in a country you choose, how much of the care it needs could Türkiye's health tourism infrastructure provide, today and by 2047?</strong><br>
  A province-level simulation of hypothetical scenarios, in English and Turkish, based on published evidence.
</p>

> **This is a companion page, not the code.**
> The source code, data, results and full documentation are in the repository of the first author, Gamze Köse:
> **[github.com/gamze-kose/TR-Health-Tourism-Surge-Sim](https://github.com/gamze-kose/TR-Health-Tourism-Surge-Sim)**
>
> The simulator runs in any browser, with no installation:
> **[gamze-kose.github.io/TR-Health-Tourism-Surge-Sim](https://gamze-kose.github.io/TR-Health-Tourism-Surge-Sim/)**
>
> Please open issues and pull requests upstream.

<p align="center">
  <img src="https://img.shields.io/badge/license-MIT-black.svg" alt="MIT">
  <img src="https://img.shields.io/badge/provinces-81%20(60%20receiving)-0F7A7F.svg" alt="81 provinces, 60 receiving">
  <img src="https://img.shields.io/badge/course-2027%20to%202047-0F7A7F.svg" alt="2027 to 2047">
  <img src="https://img.shields.io/badge/care%20needs-17-B52AA8.svg" alt="17 care needs">
  <img src="https://img.shields.io/badge/languages-EN%20%7C%20TR-1A5FCF.svg" alt="English and Turkish">
  <img src="https://img.shields.io/badge/Monte%20Carlo-2%2C000%20runs-555.svg" alt="Monte Carlo">
</p>

<p align="center"><img src="https://raw.githubusercontent.com/gamze-kose/TR-Health-Tourism-Surge-Sim/main/docs/img/en/07-results.png" width="900" alt="The simulator after a run: patients travelling to Turkish cities, with key findings under the map"></p>

## About the work

Epidemics, natural disasters and armed conflicts can create care needs that the affected health system cannot meet. The people concerned do not travel for elective treatment. They need limb reconstruction, prostheses, rehabilitation, burn care, kidney support, and the cancer or dialysis treatment that the crisis has cut off. This work asks how much of that care Türkiye's health tourism infrastructure could provide, in which cities, under what conditions, and how the answer changes by 2047.

The user chooses a country, a type and size of crisis, a year and a development path, and can change the capacity of any Turkish city before the run. A stochastic, capacity-constrained network model with a daily time step then sends patients to the 60 provinces that hold an authorised hospital. **All scenarios are hypothetical.** Past events enter the model only as published numbers, and no real event is simulated.

## Key findings

**The reserve is real, but it sits in few places.** In each reference scenario, 10 to 17 cities take 80% of the patients. After a hypothetical earthquake next door, 96% of referred patients are admitted (5th to 95th percentile: 91 to 98). In a year of armed conflict with an open corridor the share is 72% (55 to 91).

**Beds are not what runs short.** Cancer care is the first limit, and inpatient rehabilitation saturates at two to four times the reference casualties. When the exit from the country is restricted, only 20% (8 to 33) are admitted, and daily exit clearance explains 82% of the variance. In conflict, 63% are admitted with an unplanned response and 81% with a coordinated response prepared in advance.

**Over 20 years, preparation matters more than new buildings.** By 2047, domestic demand for hospital beds is 31% above 2024. The share admitted in conflict is then 75% on the current course, 82% on a planned expansion and 93% on an ambitious programme. Most of this gain comes from preparing the national response, and new units in small provinces add little.

The results compare options under stated assumptions and must not guide decisions about individual patients.

## Using the simulator

The application guides the user through five steps: choose a country, describe the crisis, choose the year and the development path, change any city or leave them as they are, and read the results. The [README of the main repository](https://github.com/gamze-kose/TR-Health-Tourism-Surge-Sim#english) explains each screen in English and Turkish.

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/gamze-kose/TR-Health-Tourism-Surge-Sim/main/docs/img/en/04-year.png" width="430" alt="Choosing the year of the crisis and the development path"></td>
    <td><img src="https://raw.githubusercontent.com/gamze-kose/TR-Health-Tourism-Surge-Sim/main/docs/img/en/05-cities.png" width="430" alt="Changing the capacity of a city"></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/gamze-kose/TR-Health-Tourism-Surge-Sim/main/docs/img/en/08-key-findings.png" width="430" alt="Key findings under the map"></td>
    <td><img src="https://raw.githubusercontent.com/gamze-kose/TR-Health-Tourism-Surge-Sim/main/docs/img/en/09-twenty-years.png" width="430" alt="The same crisis in any year to 2047"></td>
  </tr>
</table>

## Citation

> Köse, G. & Köse, U. (2026). Health Tourism Infrastructure as a Cross-Border Healthcare Reserve in Extraordinary Situations: A Province-Level Simulation and 2047 Projection for Türkiye. *INHSC2026, 5th International / 8th National Health Services Congress*, 13-14 November 2026, Isparta, Türkiye.

## Authors

**Gamze Köse**, Independent Researcher, MSc in Health Tourism. [ORCID 0000-0003-1225-5118](https://orcid.org/0000-0003-1225-5118) · [github.com/gamze-kose](https://github.com/gamze-kose)

**Prof. Dr. Utku Köse**, Department of Computer Engineering and Artificial Intelligence Application and Research Center, Süleyman Demirel University; University of North Dakota; Universidad Panamericana; VelTech University. [ORCID 0000-0002-9652-6415](https://orcid.org/0000-0002-9652-6415) · [utkukose.com](https://utkukose.com) · [github.com/utkukose](https://github.com/utkukose)

## Acknowledgements

The authors acknowledge the open statistics of the Ministry of Health of Türkiye, the Türkiye Sağlık İstatistikleri Arşivi compiled by E. Kaya, Natural Earth, the authors of SALib, and Tabler Icons by Paweł Kuna (MIT License).

---

<p align="center">
  Gamze Köse &nbsp;&amp;&nbsp; Prof. Dr. Utku Köse<br>
  Süleyman Demirel University, Isparta, Türkiye
</p>
