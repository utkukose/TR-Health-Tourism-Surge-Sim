<h1 align="center">Türkiye Health Tourism Surge Capacity Simulator</h1> 

<p align="center">
  <strong>Province-level scenarios of how much of the care created by epidemics, disasters and armed conflicts abroad Türkiye's health tourism infrastructure could provide, from 2027 to 2047.</strong><br>
  All scenarios are hypothetical. In English and Turkish, based on published evidence.
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

The results compare options under stated assumptions. They are not forecasts and must not guide decisions about individual patients.

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

## References

The list gives the peer-reviewed articles, official publications and datasets the model draws on. Each record was checked in November 2026 against the publisher, the issuing body or another authoritative record. The same list is in the Sources tab of the simulator. Figures taken from news reports of official statements, or from sources whose details could not be confirmed, are named in the documentation of the main repository and are not listed here.

### Methods

[1] Gardner ES Jr, McKenzie E. Forecasting Trends in Time Series. Management Science. 1985;31(10):1237-1246. https://doi.org/10.1287/mnsc.31.10.1237

[2] Herman J, Usher W. SALib: An open-source Python library for Sensitivity Analysis. Journal of Open Source Software. 2017;2(9):97. https://doi.org/10.21105/joss.00097

[3] Hwang CL, Yoon K. Multiple Attribute Decision Making: Methods and Applications. A State-of-the-Art Survey. Lecture Notes in Economics and Mathematical Systems, vol. 186. Berlin, Heidelberg: Springer; 1981. https://doi.org/10.1007/978-3-642-48318-9

[4] Hyndman RJ, Athanasopoulos G. Forecasting: Principles and Practice. 3rd edition. Melbourne: OTexts; 2021. https://otexts.com/fpp3/

[5] Saltelli A. Making best use of model evaluations to compute sensitivity indices. Computer Physics Communications. 2002;145(2):280-297. https://doi.org/10.1016/S0010-4655(02)00280-1

[6] Sobol′ IM. Global sensitivity indices for nonlinear mathematical models and their Monte Carlo estimates. Mathematics and Computers in Simulation. 2001;55(1-3):271-280. https://doi.org/10.1016/S0378-4754(00)00270-6

### Türkiye: capacity, health tourism and regulation

[7] Aslan K. Fizyoterapi Hizmetlerinde Yönetim ve İşleyiş: Kamu Hastanelerine Teorik Bir Bakış. Sağlık Hizmetleri Araştırma Dergisi. 2026;4:5-14. https://dergipark.org.tr/tr/pub/hes/article/1715503

[8] Becerir HB, Gürdallı S, Yapıcı B, Alkaya F, Çakır A, Yaray K, Gürsoy TO. Radiotherapy Equipment and Workforce in Turkey. Turkish Journal of Oncology. 2021;36(4):512-518. https://doi.org/10.5505/tjo.2021.2896

[9] Çavuş A, Gönenbaba İ. Erzurum'daki Hastanelerin Sağlık Turizmi Açısından Değerlendirilmesi. Atatürk Üniversitesi Sosyal Bilimler Enstitüsü Dergisi. 2020;24(4):1681-1693. https://dergipark.org.tr/tr/pub/ataunisosbil/issue/59389/654143

[10] Çubuk M. Türkiye'de Büyükşehirlerin Sağlık Turizmi Potansiyellerinin CRITIC ve WASPAS Yöntemleri ile Karşılaştırılması. Bingöl Üniversitesi İktisadi ve İdari Bilimler Fakültesi Dergisi. 2022;6(2):147-174. https://doi.org/10.33399/biibfad.1139104

[11] Işıkçelik F. Türkiye'de Seçilmiş İllerin Sağlık Turizmi Kapasitesinin Çok Kriterli Karar Verme Yöntemleriyle Karşılaştırmalı Analizi. Üçüncü Sektör Sosyal Ekonomi Dergisi. 2026;61(1):62-79. https://doi.org/10.63556/tisej.2026.1710

[12] Kaya E. Türkiye Sağlık İstatistikleri Arşivi: Sağlık Bakanlığı yıllıklarından derlenmiş il ve ulusal veri seti, 1964–2024. Version 1.1.0 [dataset]. Zenodo; 2026. https://doi.org/10.5281/zenodo.23325100

[13] Kervan Ü, Koç O, Özatik MA, Bayraktar G, Şener E, Çağlı K, Yekeler İ, Paç M. Türkiye'deki kalp damar cerrahisi kliniklerinin dağılımı ve hizmetlerinin niteliği. Türk Göğüs Kalp Damar Cerrahisi Dergisi. 2011;19(4):483-489. https://doi.org/10.5606/tgkdc.dergisi.2011.074

[14] Odabaşı O. Türkiye Tıp Fakülteleri 2023. Sürekli Tıp Eğitimi Dergisi. 2023;32(1):37-61. https://doi.org/10.17942/sted.1259646

[15] Özgöbek HR. Türkiye'de Fizyoterapist Sayısı Yeterli mi? Mevcut Durum, Gereksinimler ve Politika Önerileri. İzmir Kâtip Çelebi Üniversitesi Sağlık Bilimleri Fakültesi Dergisi. 2026;11(2):483-492. https://doi.org/10.61399/ikcusbfd.1594430

[16] T.C. Sağlık Bakanlığı. Sağlık İstatistikleri Yıllığı 2024. https://www.saglik.gov.tr/TR-114952/saglik-istatistikleri-yilligi-2024.html

[17] Taşar MT, Buluk Eşitti B. Sağlık Turizmi Yetki Belgesi Bulunan Sağlık Tesislerinin Web Sitelerinin İncelenmesi: Çanakkale Örneği. Turar Turizm ve Araştırma Dergisi. 2024;13(2):151-179. https://doi.org/10.7460/turar.1520705

[18] Türkiye İstatistik Kurumu. İstatistiklerle Yaşlılar, 2024. 13 Mart 2025.

[19] Türkiye İstatistik Kurumu. İstatistiklerle Yaşlılar, 2025. 12 Mart 2026.

[20] Türkiye İstatistik Kurumu. Nüfus Projeksiyonları, 2023-2100. Haber Bülteni 53699. 30 Temmuz 2024. https://data.tuik.gov.tr/Bulten/Index?p=Nufus-Projeksiyonlari-2023-2100-53699

[21] Uluslararası Sağlık Turizmi Enstitüsü. Sağlık Turizmi Gelirleri 2025'te 3 Milyar Doları Aştı. 16 Mart 2026. https://www.uste.org.tr/saglik-turizmi-gelirleri-2025te-3-milyar-dolari-asti/

[22] Uluslararası Sağlık Turizmi ve Turistin Sağlığı Hakkında Yönetmelik. T.C. Resmî Gazete, 26 Nisan 2025, Sayı 32882. https://www.resmigazete.gov.tr/eskiler/2025/04/20250426-2.htm

[23] Yorulmaz M, Aksoy MR. Türkiye'de Sağlık Turizmi Açısından Yetkilendirilmiş Hastaneler ve Sağlık Turizmi Acentelerinin Bölgelere Göre Değerlendirilmesi. In: International Artuklu Congress on Medicine, Nursing, Midwifery, and Health Sciences, Congress Proceedings Book; 2024. p. 1029-1037. https://doi.org/10.30546/19023.978-9952-8541-5-2.2024.4098

### Hospital capacity, length of stay and cost

[24] Aylı BI, Demir ME, Akgül A, Şahin H. Environmental footprint of in-center hemodialysis in Türkiye: A national, scenario-based analysis of water, energy, and waste. PLOS ONE. 2026;21(7):e0354903. https://doi.org/10.1371/journal.pone.0354903

[25] Bagust A, Place M, Posnett JW. Dynamics of bed use in accommodating emergency admissions: stochastic simulation model. BMJ. 1999;319(7203):155-158. https://doi.org/10.1136/bmj.319.7203.155

[26] Baş F, Erdoğan NM, Ethemoğlu FB. Cost Analysis of 30,446 Intensive Care Unit Admissions in a Tertiary City Hospital in Türkiye. Research Square [preprint, not peer reviewed]. Posted 17 June 2026. https://doi.org/10.21203/rs.3.rs-9710531/v1

[27] Brick A, Kakoulidou T, Humes H. Projections of national demand and bed capacity requirements for public acute hospitals in Ireland, 2023–2040: Based on the Hippocrates model. ESRI Research Series 213. Dublin: Economic and Social Research Institute; 2025. https://doi.org/10.26504/rs213

[28] Grasselli G, Pesenti A, Cecconi M. Critical Care Utilization for the COVID-19 Outbreak in Lombardy, Italy: Early Experience and Forecast During an Emergency Response. JAMA. 2020;323(16):1545-1546. https://doi.org/10.1001/jama.2020.4031

[29] Kao YH, Chen Y, Deutsch A, Wen H, Tseng TS. Rehabilitation length of stay and functional improvement among patients with traumatic spinal cord injury. Spinal Cord. 2022;60(3):237-244. https://doi.org/10.1038/s41393-021-00686-6

[30] Kaya B, Balal M, Seyrek N, Mete B, Karayaylali I. Hemodialysis Experience After Kahramanmaraş Earthquake. Journal of Clinical Medicine. 2024;13(21):6610. https://doi.org/10.3390/jcm13216610

[31] Ozer Sensoy NN, Kazan S, Güngör O. In Türkiye, very few internal medicine research assistants consider becoming nephrologists in the future. Scientific Reports. 2025;15:45488. https://doi.org/10.1038/s41598-025-28375-x

[32] Rees EM, Nightingale ES, Jafari Y, Waterlow NR, Clifford S, Pearson CAB, CMMID Working Group, Jombart T, Procter SR, Knight GM. COVID-19 length of hospital stay: a systematic review and data synthesis. BMC Medicine. 2020;18:270. https://doi.org/10.1186/s12916-020-01726-3

[33] Turgut M, Ağırbaş İ, Nergizoğlu G. Cost Analysis of Hemodialysis Session: A Comparison Between Activity-Based Costing and Traditional Costing Methods. Clinical and Experimental Health Sciences. 2024;14(4):1106-1112. https://doi.org/10.33808/clinexphealthsci.1318606

[34] Van den Heede K, Bouckaert N, Van de Voorde C. The impact of an ageing population on the required hospital capacity: results from forecast analysis on administrative data. European Geriatric Medicine. 2019;10(5):697-705. https://doi.org/10.1007/s41999-019-00219-8

[35] World Health Organization. Classification and minimum standards for emergency medical teams. Geneva: World Health Organization; 2021. https://www.who.int/publications/i/item/9789240029330

[36] World Health Organization, Economic Analysis and Evaluation Team, Department of Health Systems Governance and Financing. WHO-CHOICE estimates of cost for inpatient and outpatient health service delivery. https://cdn.who.int/media/docs/default-source/health-economics/who-choice-estimates-of-cost-for-inpatient-and-outpatient-health-service-delivery.pdf

### Care needs after crises

[37] Aebischer Perone S, Martinez E, du Mortier S, Rossi R, Pahud M, Urbaniak V, Chappuis F, Hagon O, Jacquérioz Bausch F, Beran D. Non-communicable diseases in humanitarian settings: ten essential questions. Conflict and Health. 2017;11:17. https://doi.org/10.1186/s13031-017-0119-8

[38] Ankah AH, Alanqar MM, Mansour BM, AlZebda MM, Idris AE, Brown P, Melhem NZ, Ayyad NA. Experiences of children with kidney failure in Gaza. Eastern Mediterranean Health Journal. 2025;31(4):250-253. https://doi.org/10.26719/2025.31.4.250

[39] Bilir EE, Borman P, Ata AM, Alemdaroğlu E, Bodur H, Yanık B, Yurdakul F, Kesikburun B, Güler T, Başkan B, Akkuş S, Uzun O, Yaşar E. Clinical properties and rehabilitation needs of earthquake survivors in a subacute rehabilitation setting. Ulusal Travma ve Acil Cerrahi Dergisi. 2024;30(4):297-304. https://doi.org/10.14744/tjtes.2024.27553

[40] Bilir EE, Ata AM, Borman P, Savtok BE, Afşin B, Eser F. Retrospective Analysis of Functional and Demographic Data of Earthquake-Related Peripheral Nerve Injuries. Archives of Health Science and Research. 2025;12:1-5. https://doi.org/10.5152/ArcHealthSciRes.2024.23161

[41] Bıyıklı K, Taşkın R, Ceylan A, Ulutabanca RÖ, Benli AR. War and Health Tourism: Data of Kayseri Province. International Journal of Health Management and Tourism. 2019;4(1):73-81. https://doi.org/10.31201/ijhmt.441373

[42] Buyurgan ÇS, Bozkurt Babuş S, Yarkaç A, Köse A, Usluer HO, Ayrık C, Narcı H, Orekici Temel G. Demographic and Clinical Characteristics of Earthquake Victims Presented to the Emergency Department with and without Crush Injury upon the 2023 Kahramanmaraş (Turkey) Earthquake. Prehospital and Disaster Medicine. 2023;38(6):707-715. https://doi.org/10.1017/S1049023X23006416

[43] Fily F, Ronat JB, Malou N, Kanapathipillai R, Seguin C, Hussein N, Fakhri RM, Langendorf C. Post-traumatic osteomyelitis in Middle East war-wounded civilians: resistance to first-line antibiotics in selected bacteria over the decade 2006–2016. BMC Infectious Diseases. 2019;19(1):103. https://doi.org/10.1186/s12879-019-3741-9

[44] Gosney JE, Reinhardt JD, von Groote PM, Rathore FA, Melvin JL. Medical rehabilitation of spinal cord injury following earthquakes in rehabilitation resource-scarce settings: implications for disaster research. Spinal Cord. 2013;51(8):603-609. https://doi.org/10.1038/sc.2013.50

[45] Halacli B, Guven G, Kaya EK, Yildirim M, Bulut Yuksel ND, Kocak G, Bulut K, Gulen D, Erdemir Sullu B, Kilicaslan B, Seven AE, Gemcioglu E, Simsek M, Yuksel RC, Temel S, Kaynar AS, Deveci K, Alptekinoglu Mendil N, Aydin E, Ulger B, Esmaoglu A, Boyaci Dundar N, Ortac Ersoy E, Gundogan K, Akinci SB, Topeli A, on behalf of the Turkish Intensive Care Studies-Network (TRICS-Net). Evaluation of the clinical characteristics and outcomes of patients admitted to intensive care units after the Kahramanmaras (Türkiye) earthquake: a multicenter observational study. Frontiers in Medicine. 2025;12:1517344. https://doi.org/10.3389/fmed.2025.1517344

[46] Hanna TP, King WD, Thibodeau S, Jalink M, Paulin GA, Harvey-Jones E, O'Sullivan DE, Booth CM, Sullivan R, Aggarwal A. Mortality due to cancer treatment delay: systematic review and meta-analysis. BMJ. 2020;371:m4087. https://doi.org/10.1136/bmj.m4087

[47] Idrees MHD, Bashir MMI, Mohamed BAA, Ahmed AEA, Abdalla HMM, Shaaban KMA. April 15th war and hemodialysis patients in Sudan: a cross-sectional study. BMC Public Health. 2025;25:230. https://doi.org/10.1186/s12889-025-21369-4

[48] Mendeş E, Gümüşburun N. A 10-Year Analysis of Surgical Interventions Applied to Migrants: A Border Hospital Experience During the Syrian Civil War. Turkish Journal of Anaesthesiology and Reanimation. 2025;53(5):263-276. https://doi.org/10.4274/TJAR.2025.252054

[49] Moitinho de Almeida M, van Loenhout JAF, Thapa SS, Kumar KC, Schlüter BS, Singh R, Banse X, Putineanu D, Mahara DP, Guha-Sapir D. Clinical and demographic profile of admitted victims in a tertiary hospital after the 2015 earthquake in Nepal. PLoS ONE. 2019;14(7):e0220016. https://doi.org/10.1371/journal.pone.0220016

[50] Norton I, von Schreeb J, Aitken P, Herard P, Lajolo C. Classification and Minimum Standards for Foreign Medical Teams in Sudden Onset Disasters. World Health Organization; 2013. https://cdn.who.int/media/docs/default-source/documents/publications/classification-and-minimum-standards-for-foreign-medical-teams-in-suddent-onset-disasters65829584-c349-4f98-b828-f2ffff4fe089.pdf

[51] Ozturk I, Gungor O, Ozturk S, Olmaz R, Gunes Keskin AJ, Kocyigit I, Sipahioglu MH, Dede F, Ulu S, Turgutalp K, Torun D, Sahutoglu T, Erdur FM, Altunoren O, Danis R, Yildiz G, Gurel A, Horoz M, Kucuksu M, Karakose S, Yildirim T, Altiparmak MR, Ayli MD, Tugcu M, Eren Z, Eroglu E, Coskun Yavuz Y, Akcali E, Sit D, Polat M, Yildirim S, Alagoz S, Gokcay Bek S, Pembegul I, Karaaslan T, Keles M, Sari F, Yilmaz U, Gorgulu N, Sahin G, Aydin Z, Yadigar S, Ulutas O, Selcuk NY, Ayar Y, Turgut D, Oto OA, Koc M, Yıldız A, Tuglular S, Sever MS. Epidemiological analysis of the victıms wıth crush syndrome in earthquakes of southeastern Turkey. Journal of Nephrology. 2024;37(9):2589-2599. https://doi.org/10.1007/s40620-024-02051-1

[52] Redmond AD, Mardel S, Taithe B, Calvot T, Gosney J, Duttine A, Girois S. A Qualitative and Quantitative Study of the Surgical and Rehabilitation Response to the Earthquake in Haiti, January 2010. Prehospital and Disaster Medicine. 2011;26(6):449-456. https://doi.org/10.1017/S1049023X12000088

[53] Yilmaz S. Transportation model utilized in the first week following the Kahramanmaraş earthquakes in Turkey - transport health centers. Scandinavian Journal of Trauma, Resuscitation and Emergency Medicine. 2023;31:40. Correction: 2023;31:67. https://doi.org/10.1186/s13049-023-01108-7

### Official reports and datasets

[54] European Commission. Coronavirus: European Solidarity in action. Factsheet. 26 June 2020. https://ec.europa.eu/commission/presscorner/api/files/attachment/865847/Covid19_factsheet_EuropeanSolidarity_EN_26JUne.pdf.pdf

[55] Mathieu E, Ritchie H, Rodés-Guirao L, Appel C, Gavrilov D, Giattino C, Hasell J, Macdonald B, Dattani S, Beltekian D, Ortiz-Ospina E, Roser M. COVID-19 Pandemic. Our World in Data; 2020. https://ourworldindata.org/coronavirus

[56] Medical evacuation of Gaza patients: Oct 2023 - 1 Dec 2025. Summary sheet hosted by the World Health Organization Regional Office for the Eastern Mediterranean. https://www.emro.who.int/images/stories/palestine/Medevac_1Dec25.pdf

[57] Ministry of Health of Ukraine. Medevac Ukraine: over 5,600 Ukrainian patients have participated in the medical evacuation program abroad. 6 June 2025. https://moz.gov.ua/en/medevac-ukraine-over-5-600-ukrainian-patients-have-participated-in-the-medical-evacuation-program-abroad

[58] Natural Earth. Free vector and raster map data. https://www.naturalearthdata.com

[59] WHO Regional Office for Europe. Over 6400 Ukrainians receive life-saving treatment abroad through medical evacuations. News release. 3 March 2026. https://www.who.int/europe/news/item/03-03-2026-over-6400-ukrainians-receive-life-saving-treatment-abroad-through-medical-evacuations

[60] World Health Organization. Health Access Barriers for patients in the occupied Palestinian territory. Monthly report, October 2022. Published 7 December 2022. https://www.emro.who.int/images/stories/palestine/Oct_2022_Monthly.pdf

[61] World Health Organization, Office for the occupied Palestinian territory. Estimating Trauma Rehabilitation Needs in Gaza: September 2025 Update. Technical note. 2 October 2025. https://cdn.who.int/media/docs/default-source/hq-whe/estimating-trauma-rehabilitation-needs-in-gaza-september-2025.pdf

[62] World Health Organization, Regional Office for the Eastern Mediterranean. One in four injuries in Gaza is life-changing while rehabilitation services struggle to keep pace, WHO reports. 12 May 2026. https://www.emro.who.int/opt/news/one-in-four-injuries-in-gaza-is-life-changing-while-rehabilitation-services-struggle-to-keep-pace-who-reports.html

[63] World Health Organization. Rehabilitation needs of people recovering from COVID-19. Scientific brief. WHO/2019-nCoV/Sci_Brief/Rehabilitation/2021.1. 29 November 2021. https://www.who.int/docs/default-source/coronaviruse/scientific-brief-rehabilitation-and-covid-19_.pdf

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
