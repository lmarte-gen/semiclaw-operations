# Notes on the SC Ecosystem by Steve Blank

Semiconductor industry is large and generates several trillions of dollars, with hundred of companies at every link in the supply chain. Below we’re breaking down each segment of the chain (simple overview)

# Semiconductor Industry Segments

We’ll break the industry down to seven segments:

1. Chip IP Cores  
2. EDA Tools  
3. Specialized Materials  
4. Wafer Fab Equipment (WFE)  
5. Fabless Companies  
6. Integrated Device Manufacturers  
7. Chip Foundries  
8. Outsourced Semiconductors Assembly and Test

Below we’ll provide a brief overview of each segment, followed by a deep dive in each.

## Chip Intellectual Property

- Companies sell their chip design as building blocks to other chip design firms  
  - Basic example: touch screen code. Instead of having to continuously develop the ability for touch screen, you can license it and use it with your software (Not a real example, but it gets the point across)  
- There are over 150 companies that sell their IP for chips  
- Key Players:  
  - ARM, Synopsis, Cadence

## EDA Tools

- Building on top of the Chip IP, Engineers design chips using specialized   
- It can take about 2-3 years to design logic chips  
- Key Players  
  - Industry is dominated by three US Vendors: Cadence, Mentor, and Synopsis

## Specialized Materials and Chemicals:

- Here is where we begin our trek into the physical world. In order to fabricate chips, special materials are needed:  
  - Silicon Wafers \- which require crystal growing furnaces  
  - Over 100 gasses  
  - Fluids (Phororesist)  
  - Photomasks  
  - Wafer-handling equipment, dicing  
  - RF Generators

## Wafer Fab Equipment

- Machines that manufacture the chips  
- Some of the most complicated machinery humanity has ever created  
- Essentially manipulating atoms on silicon  
- Key Players:  
  - Applied Materials  
  - Tokyo Electron  
  - ASML

## Fabless Companies

- Systems Companies that design their own chips  
- Using the IP cores and their own designs, they send their proprietary designs to foundries with fabs and manufacturer them  
- These could be for internal use (Apple, Google, etc) or to sell to customers (NVIDIA, AMD, Qualcomm, etc)  
- These companies do not own WFE or specialized materials or chemicals  
- They use Chip IP and EDA software to design their chips

## Integrated Device Manufacturers

- IDMs Design, Manufacture, and sell their own chips  
  - They can also manufacture chips for other companies, similar to a foundry, but this is a relatively new phenomenon  
- There are three categories of IDMs:  
  - Memory (SK Hynix, Micron)  
  - Logic (Intel, Samsung)  
  - Analog (TI)  
- They have their own Fabs, but could also use foundries for additional inventory or cutting edge processes not available, or yield issues  
- Cost to tape out new leading-edge chips continues to grow

## Chip Foundries

- Foundries make chips for others in their Fabs  
- They buy and integrate equipment from a variety of manufacturers  
  - WFE and specialized materials and chemicals  
- They design unique processes to make the chips; they don’t design the chips  
- Three major logic Chip Foundries: TSMC, Samsung, Intel  
- Other fabs specialize in making chips for analog, power, rf, displays, military, etc.  
- Each Fab can cost more than $20 Billion to construct

## Fabrication Plant (Fab)

- IDMs and Foundries both have fabs. The only difference being are the manufacturing using their own designs or from external companies.  
- Chip fabrication extremely high level overview:  
  - Engineer designs chip using chip IP and EDA Tools  
  - They select a fab appropriate for their type of chip (mem, logic, etc)  
  - Fab buys raw materials (silicon, chemicals, gases)  
  - Fab buys WFE (etchers, deposition, lithography, testers, packaging)  
  - Chip Fabrication process:  
    - Wafers are sawed out of an ingot of pure crystalline silicon  
    - Wafer is polished  
    - Material deposition or modification  
    - Resist is applied to a spinning wafer to achieve a uniform layer  
    - Using EUV litho the chip patterns are burned into the resist in an exposure step  
    - The print is developed through etching and heating  
    - Ion implantation dope exposed regions  
    - The resist is removed  
    - A wafer processing cycle is complete and one layer has been fabricated  
      - Repeat 40-100 times  
    - Cut chips out of the wafer and test  
      - Mature processes have yields of 30-80%  
    - Package and assemble the chips  
  - Process runs millions of times  
- Simplified overview of about 1000+ steps

## Outsourced Semiconductor Assembly and Test

- Companies that package and test chips made by foundries and IDMs  
- OSAT companies take the Wafer made by foundries, dice (cut) them into individual chips, test them, package them, and then ship them to customers  
- There are a lot of advancements being made at the packaging level to help with the “slowing” of Moore’s law  
- Key Players:  
  - ASE, Siliconware Precision, etc

## Fabrication Issues

- As chips become more dense (trillions of transistors per wafer) the cost of building fabs have sky-rocketed; driven by the cost of the machinery required to manufacture chips  
  - Advanced Litho machines by ASML cost upwards of $150 million  
  - Each Fab can have 500+ machines (not all ASML Litho)  
  - Fab building continue to grow in complexity with complex set of plumbing for gases, power, liquids at the right time and temperature  
- Due to the complexity and price, many companies have decided to drop out of leading-edge manufacturing; leaving 2.5 (with intel being the .5) companies: TSMC and Samsung  
  - This adds geopolitical complexities involving China and the US, along with fault line exposure in Taiwan.

## Technological issues

- Due to the difficulty of building denser, faster, more power efficient chips, designers, manufacturers, and packagers have had to develop creative ways to be able to do their part  
  - Instead of having just one processor doing all the work, designers have put multiple specialized processors inside of a chip  
  - Memory chips are now made denser by stacking them 100+ layers high  
  - EDA companies are now integrating AI into their design process to alleviate some of the complexities and try to meet/exceed the 2-3 year design cycle  
  - WFE manufacturers are designing new equipment to help fabs make chips with lower power, better performance, optimum area-to-cost, and faster time to market

## Business Evolution

- IDM business model is changing. The competitive advantage that used to exist for being vertically integrated in chip manufacturing has eroded.   
- Foundries are more flexible to change  
- AMD, a former IDM and now a Fabless company, has proven that ditching their integrated approach to a fabless approach can pay dividends in the long run.

## Geopolitics

- Controlling advanced chip manufacturing in the 21st Century will be like controlling the oil in the 20th Century.   
- Ensuring a steady supply of chips has become nat’l priority  
- China & US are rapidly trying to decouple their semiconductor ecosystems from each other  
  - China has spent $100+ Billion in subsidies for SMIC, Huawei, and other indigenous IP, EDA, Materials and WFE (Both because of national priority and sanctions placed by the west regarding state of the art equipment  
- Most, if not all, cutting-edge chip-producing fabs are located in Asia (Taiwan, South Korea), which places the US gov’t in a precarious position and is attempting to on shore some of that capacity.

# Deep Dive: Semiconductor Ecosystem Segments

## EDA & Core IP

There are three major players in the EDA game. Together they control the vast majority of the market for the essential software used to design semiconductors

- Synopsis, Cadence, Siemens EDA  
  - Market share (74%)  
    - Synopsis \- 32%  
    - Cadence \- 30%  
    - Siemens \- 13%  
  - Siemens is in a strong third position  
    - Dominant in specific, critical segments of the design flow; specifically calibre, which is the industry standard for physical verification and signoff  
  - High barrier to entry:  
    - Due to the cost of entry into this space, the “big three’s” position is pretty solidified  
  - Things to look into:  
    - Margins, Revenue, Capex, R\&D

Regarding Core IP (Design IP), there is one dominant player, Arm Holdings, which has a market share of \~40%. Synopsis and Cadence also have 21% and 6% market share, followed by smaller companies like Alphawave Semi and Imagination Technologies

### Key Players

- Synopsis is a pivotal company for both EDA and IP.  
  - EDA: Software chip designers use to create, verify, and test digital and analog circuits. Given the billions of transistors on modern chips, designing them manually is impossible. Synopsis provides a comprehensive suite of EDA tools that automate and manage this intricate process. The key functions of Synopsis tools include:  
    - Design and simulation:  
      - Using verilog or VHDL, engineers describe the chips functionality and then simulate its behavior to ensure it works as intended  
    - Synthesis:  
      - Converts high-level design code into a detailed list of logic gates and their interconnections  
    - Place and route:  
      - Take the synthesized design and physically layout the transistors and wires on the silicon wafer, optimizing for performance, power consumption, and area  
    - Verification:  
      - A critical and time-consuming stage where the design is tested vigorously. Synopsis offers a range of verification tools  
    - Without these sophisticated EDA tools, the design of today’s complex processors, mem chips, and other semiconductor devices would not be feasible.  
  - Core IP: Synopsis is a leading provider of IP cores. These are pre-designed and pre-verified blocks of circuitry that perform a specific function. This allows engineers to not have to design everything from scratch.  
    - This approach offers significant advantages:  
      - Reduced design time  
      - Lower risk  
        - IP cores have already been thoroughly verified and tested  
      - Access to Expertise  
        - Companies can leverage Synopsis’ expertise in specific areas (high speed interfaces, security, etc), without having to develop that expertise in-house  
    - Synopsis offers a vast portfolio of IP cores, including:  
      - Interface IP for standard protocols like USB, PCIe, DDR, etc  
      - Processor cores like ARC processors  
      - Security IP  
        - For encryption and other security functions  
      - Analog IP for functions like data conversion

- Cadence provides a comprehensive suite of software, hardware, and services that are essential for designing integrated circuits and electronic systems. Its offerings include:  
  - EDA:   
    - Custom IC and Analog design  
      - Well known for Virtuosi Platform, which is a cornerstone for designing analog, mixed-signals, and custom digital circuits  
    - Digital design and signoff  
      - Similar to Synopsis, Cadence offers logic synthesis, physical implementation (place and route) and power analysis (signoff)  
    - Verification  
      - Offers a suite of verification tools, including simulation, emulation, and formal verification  
    - System design and analysis  
      - Beyond the chip level, Cadence provides tools for designing and analyzing entire systems, including printed circuit boards (PCB) and advanced packaging (2.5D and 3D ICs)  
  - IP  
    - Tensilica DSPs:   
      - Configurable digital signal processors (DSPs) cores   
      - Widely used in applications like audio/voice, processing, computer vision, AI/ML  
    - Interface IP:  
      - Several standard interfaces (DDR, PCIe, etc)  
    - Analog and Mixed signal IP  
      - Data converters, PLLs, and other analog functions that are essential for interacting with the real world  
    - Verification IP:  
      - Verifies that designs comply with standard protocol

- Siemens EDA, formerly known as Mentor Graphics, was acquired by Siemens in 2017 and integrated the crucial chip design capabilities into Siemens’ broader digital industries software portfolio, creating a unique bridge between semiconductor design and system level engineering. Their key areas of strength are:  
  - EDA:  
    - IC Verification (Calibre Platform): Market leader in physical verification. Calibre is the industry standard used by most Foundries for “signing off” on a chip’s design before the expensive process of manufacturing begins. It checks that the layouts adhere to the foundry’s complex design rules (DRC) and that the physical layout accurately matches the original schematic (LVS)  
    - Design-for-test (Tessent): Complete silicon lifecycle management solution. Provides tools that embed test structures into the chip design itself, making it possible to test the manufactured silicon for defects efficiently.   
    - Emulation and Prototyping: Can verify the functionality of massive complex SOCs before they are physically created using the Veloce platform  
    - IC and PCB Design: Design of PCBs and advanced IC packaging with Xpedition Enterprise platform. This bridges the gap between the chip and the larger electronic system it lives in.  
  - Core IP:  
    - Microcontrollers  
    - Interface IP  
    - Memory IP  
    - Mixed Signal IP  
- Arm Holdings’ business is centered almost exclusively on designing and licensing IP cores. Its primary role is to design the architecture and core components of processors, which it then licenses to hundreds of other companies, which the companies then integrate into the SoC designs. Essentially, Arm is like an architect that builds blueprints for a house, but doesn’t build the house. They design various processor cores with different performance and power characteristics and license those blueprints, along with instruction set architecture (the language the processor speaks) to other companies. They then build these cores and integrate them with other components (GPU, Mem, IO, etc).   
  - This gives ARM a moat of sorts, as it creates:  
    - Standardization by creating a common software ecosystem. Code compiled for the Arm architecture can run on chips from many manufacturers  
    - Focus and efficiency: semiconductor design companies can focus on their service (graphics, modems, etc) without having to spend billions developing CPU from scratch  
    - Arm provides:  
      - Application processors (Cortex-A)  
      - Microcontrollers (Cortex-M)  
      - Real-time Processors (Cortex-R)  
      - GPU IP for gaming, graphics, and parallel processing

### Research Questions

1. Why is EDA considered a “chokepoint” in the supply chain?  
   1. There’s extreme market concentration. The vast majority of the market is controlled by three companies. With no viable alternative, any company wanting to design modern, complex chips has to use software provided by one of these firms; which gives them immense leverage.  
   2. Indispensable gateway to manufacturing: EDA stands as the bridge between conceptual design and the physical manufacturing of the chip. Foundries like TSMC require complex blueprints (design files) to fabricate the chips, which can only be done with EDA tools. All modern semiconductors for any purpose (logic, mem, RF, etc) has to go through this process, mandating all design firms use EDA tools  
   3. Barriers to entry: It would be nearly impossible to start a competitive EDA provider. The reasons include:  
      1. Decades of R\&D: tens of billions of dollars have gone into R and D over the years, along with domain knowledge gained by trial and error, experience, etc.  
      2. Physics and Complexity: The problems the SW has to solve is incredibly complex: modeling quantum effects, complex computational problems, etc.  
      3. Deep Foundry Integration: Current EDA tools are deeply integrated and trusted with foundries, following years of close collaboration  
   4. Geopolitical and strategic importance: The main EDA providers are located in the west (US and Germany), which provides those countries, and the west as a whole, leverage in foreign policy. Access to EDA software, or lack thereof, can effectively cutoff a country’s ability to design its own advanced semiconductors.  
2. How do EDA companies capture value despite being relatively small in revenue compared to chip makers?   
   1. The "tollbooth" on the road to manufacturing. EDA is an unavoidable choke point; companies who want to design modern, sophisticated chips have to use EDA software from one of the big three. This allows them to set the market  
   2. A high-margin software model. This is what differentiates EDA companies from chip makers.  
      1. Chip makers spend billions on R\&D, but they also spend Billions on the complex and capital-intensive process of manufacturing, packaging, and testing their goods.   
      2. EDA companies also spend billions on R\&D, but that is their main expense, along with the workforce. Once the software is written, the cost of selling licenses is near-zero. This results in extremely high margins, around 80-90%.  
   3. EDA companies are able to price their software based on the value it provides to their customers, not by how much it cost for them (EDA companies) to develop. Using Apple as an example:  
      1. A $50 million suite of EDA tools can help Apple in designing a new processor for the iphone, a $250+ Billion product line.  
      2. If the tool can improve power efficiency by 5%, it can make the product more competitive  
      3. Verification can prevent a future bug that could cost time (delay in shipment) and money (cost it would take to fix bug later in the future)  
   4. Extreme customer stickiness and high switching costs. Once a company builds its entire design workflow and trains its thousands of engineers on a specific EDA platform, the cost and disruption of switching to a competitor are astronomical.

### Research Topics

1. Geopolitics:   
   1. What is the current state of export restrictions regarding EDA tools? Can China stand up their own EDA provider? Have they already?

## Specialized Materials and Chemicals

The companies below supply everything from basic silicon wafers to the complex chemicals and gasses required in the fabrication process.

### Silicon Wafer Suppliers

1. Shin-etsu Chemical:  
   1. Japanese  
   2. Leading producer of silicon wafers  
   3. 150-300 mm, epi, SOI  
2. SUMCO:  
   1. Japanese  
   2. High-volume 300 mm prime wafers for advanced logic/memory  
3. Global Wafers  
   1. Taiwan  
   2. Top-tier global supplier; expanding US 300 mm/SOI capacity under the CHIPS act  
4. Siltronic  
   1. German  
   2. Leading hyper-pure 300mm wafers; global customer base  
5. SK Siltron  
   1. Korean  
   2. Korea’s sole silicon wafer maker; scaling globally

### Engineered Substrates

1. Soitec  
   1. France  
   2. World leader in SOI/Engineered Substrates (FD-SOI, RF-SOI)  
   3. For Key RF and low-powered platforms

### Compound-Semiconductor Wafer (SiC/GaN)

1. Wolfspeed  
   1. US  
   2. SiC substrates/epi at scale  
   3. Currently in chapter 11 restructuring (operations continuing)  
2. SK Siltron CSS  
   1. US/Korea  
   2. SiC Wafters (Acquired DuPont’s SiC unit)  
3. Onsemi (via GTAT)  
   1. US  
   2. Vertically securing SiC boules/epi for power devices  
4. Coherent (ex-II-VI)  
   1. US  
   2. Compound substrates include SiC, GaAs, Inp

### Photoresist & Lithography Materials

1. JSR  
   1. Japanese  
   2. Leading supplier of photoresist  
2. Tokyo Ohka Kogyo (TOK)  
   1. Japanese  
   2. Specializes in photoresists and other high purity chemicals  
3. Dupont  
   1. American (Multi-national)  
   2. Chemical company that provides a range of materials for the semiconductor industry, including photoresists  
4. Fujifilm Electronic Materials  
   1. Japan  
   2. Resists \+ Photolithography ancillaries  
5. Shin-etsu Chemical:  
   1. In addition to wafers, they are also a key player in photoresist  
   2. Advancing EUV Pellicle tech  
6. Sumitomo  
   1. Japanese  
   2. A major chemical company with a significant presence in the semiconductor materials market

#### Photomasks blanks and Pellicles

1. Hoya  
   1. Japan  
   2. Leading photomask blank supplier  
2. AGC  
   1. Japan  
   2. EUV mask blanks and EUV capacity expansion  
3. Mitsui Chemicals  
   1. Japan  
   2. First to commercialize EUV pellicles under ASML license

### Chemical Mechanical Planarization Consumables

1. Entegris  
   1. US  
   2. CMP slurries/pads and broader contamination control  
2. Dupont  
   1. US  
   2. CMP pads and slurries portfolio   
      1. Suba  
      2. Optivision  
      3. Klebosol  
3. Fujifilm Electronic Materials  
   1. copper/barrier/FEOL slurries and post-CMP cleaners, expanding capacity  
4. BASF  
   1. Germany  
   2. CMP Chemistries / Cleaners

### Semiconductor Gases and Chemical providers

1. Linde plc  
   1. Global industrial gas and engineering company that supplies a wide range of gasses to the semiconductor industry  
2. Air Liquide  
   1. French  
   2. Supplies industrial gases and services to various industries, including electronics  
3. Air Products and Chemicals:  
   1. American  
   2. Provides essential industrial gases and chemicals  
4. Merck KGaA (EMD Electronics)  
   1. German  
   2. Key supplier of specialty chemicals and materials for the electronic industry  
5. Taiyo Nippon Sanso Corp  
   1. Japanese  
   2. Industrial Gas Manufacturer

#### High Purity Wet Chemicals and Cleans

1. Fujifilm  
   1. High Purity Process Chemicals (HPPC)  
2. Kanto Chemicals  
   1. Japan  
   2. Ultra-pure wet chemicals for etch / clean  
3. Honeywell Electronic Chemicals  
   1. US  
   2. Electronic chemicals portfolio  
4. Avantor  
   1. US  
   2. UHP Wet chemicals (etch/strip/cleat) to ppt specs

### Advanced Packaging Materials

1. ABF  
   1. Japan  
   2. Build-up films, defacto standard for high-performance substrates  
2. Mitsubishi Gas Chemical (MGC)  
   1. Japan  
   2. IC Substrates laminates (BT), high market share  
3. Sumitomo Bakelite  
   1. Japan  
   2. Epoxy molding compounds, die attach, substrate materials  
4. NAMICS  
   1. Japan  
   2. Underfills, encapsulants for flip-chip, board-level reliability

### General End-to-end flow

1. Substrates (Si / SOI / SiC / GaN), Substrate quality sets your yield ceiling; everything else is trying not to erode it  
   1. Crystalline starting point:  
      1. 300 mm Si  
      2. Engineered SOI (FD-SOI, RF SOI)  
      3. Wide-bandgap SiC/GaN for power/RF  
2. Surface preps and cleans (wet chemicals, UPW)  
   1. UPW chemistries  
   2. Surface chemistry is the gatekeeper for adhesion, etch profiles, and defectivity across steps  
3. Deposition (ALD/CVD/PVD) using specialty gases/precursors  
   1. Films for gates, spacers, barriers, seeds, conductors, liners  
   2. Deposition defines what is patterned; uniformity, conformality, and impurities define how forgiving the downstream steps will be  
4. Lithography stack (resists, BARCs/hardmasks) \+ masks/pellicles  
   1. Spin-on resists, BARCs/anti-reflectants, hardmasks, developers, and the reticle stack (mask blanks, pellicles)  
   2. Litho is pattern fidelity. Every other step either prepares or protects what Litho tries to print  
5. Dry/wet etch (gases and chemicals)  
   1. Plasma etch for directional removal and selective wet etches  
   2. Etch shapes device geometry and via profiles; it’s where many “invisible” yield killers originate  
6. CMP planarization (slurries and pads \+ post-CMP cleans)  
   1. Hybrid chemical-mechanical removal to re-establish planarity and stop on a target  
   2. CMP manages topography for multi-layer patterning  
7. Purity/Contamination control  
   1. Point-of-use liquid/gas filtration, oxygen/moisture scavengers in gas delivery, cleanroom ULPA/HEPA, FOUP/mini-environments, AMC scrubbers.  
8. Assembly and advanced packaging (ABF/BT, plating chemistries, underfills, EMC, TIMs)  
   1. Materials to build electronic/mechanical systems from chips:  
      1. ABF/BT build-up substrates  
      2. RDL and pillar planting chemistries  
      3. Underfills and epoxy molding compounds (EMC)  
      4. Die attached and thermal interface materials (TIMs)  
   2. Packaging is performance critical (power delivery, bandwidth, thermals)  
9. Cheat sheet \- What to look for in vendor profiles  
   1. **Substrates:** defect density, epi quality, bow/warp, node alignment (300 mm scaling, SOI flavors, 150/200 mm for SiC/GaN).  
   2. **Litho:** EUV readiness (resist type, LER/stochastics), hardmask options, pellicle availability/transmission/thermal spec.  
   3. **Gases/Chemicals:** precursor portfolio (ALD/CVD), etch gas selectivity/control, dopant gas handling/abatement, wet-chem purity (ppt).  
   4. **CMP:** slurry selectivity (Cu vs low-k), scratch/corrosion suppression, pad lifetime, post-CMP clean synergy.  
   5. **Purity:** point-of-use filtration grades, gas purifier spec (O₂/H₂O sub-ppb), AMC capture efficiency.  
   6. **Packaging:** ABF/BT roadmap, low-Dk/Df options, plating chemistries for fine-pitch RDL, underfill/EMC reliability data, TIM performance.

### Research Questions

1. Which materials are true choke points?  
   1. There are several chokepoints across the materials spectrum for several reasons. It could be due to small supplier sets, long re-qual times, and limited substitutes. Below are some of the stages where these points exist:  
      1. Patterning (EUV/DUV)  
         1. EUV mask blanks \- Essentially a duopoly (HOYA, AGC). If either stumbles, reticle schedules slip industry-wide  
         2. EUV Pellicles \- Commercial supply led by Mitsui Chemicals under ASML license; volumes and specs (transmittance/thermal) are tight, especially for future High-NA  
         3. EUV metal-oxide resists (MOR) \- Inpria (JPR) is the flagship MOR Supplier; concentration is high and re-qualifying alternatives is non trivial  
         4. Photoresists / high-purity HF (DUV) \- Japan’s 2019 export curbs show how concentrated these are (Japan \~ 90% of photoresists; \~70% of high purity HF via players like Stella Chemifa). That single Policy move put Samsung/SK Hynix at risk.  
         5. Neon for excimer lasers (DUV) \- Ukraine historically supplied \~50% of world neon and more than 90% of US semiconductor-grade neon; disruptions immediately tighten DUV capacity  
            1. Not needed for EUV  
      2. Substrates  
         1. RF-SOI / FD-SOI engineered wafers \- Soitec has \~70% market share; others often license it’s tech  
         2. 300 mm Silicon wafers (prime) \- an oligopoly (Shin-Etsu \+ SUMCO \>50% global share; add GlobalWafers/Siltronic/SK Siltron). Not single-sources, but capacity cycles and long lead times make this a structural bottleneck  
         3. SiC (power) \- esp. 200mm \- Supply is concentrated and ramps are delicate; scenario work shows tightness if EV demand accelerates (multiple players exist but near-term imbalance is plausible)  
      3. Wet/process chem and gases  
         1. Mitrogen Trifluoride chamber-clean gas \- capacity is concentrated in East Asia  
      4. Advanced Packaging  
         1. ABF build-up film (core-substrate dielectric) \- Ajinomoto fine-techno holds 95% share for insulating films used in high-performance CPU/GPU substrates.   
      5. Cross-Cutting regulatory risk  
         1. PFAS restrictions (EU REACH) \- fluoropolymers and fluorinated chemistries are embedded across resists, seals, tubing, and membranes; industry warns many uses currently lack drop-in substitutes.  
2. How do material suppliers influence yield and scaling on advanced nodes?  
   1. Materials are not just inputs, but they’re knobs on yield and scaling. Suppliers influence (or limit) what the process window could be.   
      1. Pattern Fidelity (EUV/DUV): resist stacks, hardmasks, masks pellicles. How suppliers move yield:  
         1. [Resist Chemistry](https://docs.google.com/document/u/0/d/1Ly4YgMTquW-x7yWpjZPcuSd_72P-E4Y85x0CUuiXxEM/edit) (EUV Sensitivity vs. Noise): Metal oxide and chemically amplified resists set the dose needed to print and the level of stochastic defects (missing, merged holes, line breaks, etc.). Lower dose equals higher throughput but more shot noise. Suppliers tune polymer, metal cores, quencher load, and solvents to lower LER, LWR, and stochastic fail rate.   
         2. [Underlayers/topcoats & hardmasks](https://docs.google.com/document/u/0/d/1RpwSgsxptxVJER92gJGE9RNfm4qcXjPu4g6qQXPTSqM/edit): Anti-reflectants and dense hard-mask stabilize CDs and protect resistant etch. Widening the edge selectivity window and reducing line collapse.   
         3. [Mask blanks and pellicles](https://docs.google.com/document/u/0/d/1CD03ImvGDbP_pmUsfG-wC9Mpx_yWukga6Fc4w3Cn7_U/edit): Fewer native defects on blanks equal fewer repeating defects. Pellicle transmission and thermal stability affect exposed dose (hence stochastics) and overlay (due to heating).  
         4. Why this hits yield/scaling:   
            1. at single-digit nm, random defects dominate. Materials let you print a slightly higher dose (or with better acid control) can drop stochastic fails dramatically \- direct D0 reduction without new equipment  
            2. At 5 nm, 3nm, and smaller nodes, the biggest enemy of yield is no longer systematic, predictable errors, but the random, stochastic defects described above  
            3. Improving materials provides a direct way to fight this. A slightly better resist might allow the chipmaker to use a slightly higher dose of light (to reduce noise) without sacrificing too much speed. This can cause the rate of stochastic failures to plummet. This is what is meant by a direct D0 reduction – lowering the initial defect density without having to buy a new, more expensive scanner. The materials themselves become the upgrade.  
         5. Signals to check:  
            1. Dose at target CDU, LER, stochastic fail ppm at target pitch, resist outgassing (tool contamination), pellicle transmission/warp vs. power   
      2. [Etch selectivity and profiles](https://docs.google.com/document/u/0/d/1dej6ZuUnHYWTRvQfqGLS2RyNaYJCTbBrZeW26zdN-s4/edit): fluorocarbon/halogen chemistries, inhibitors  
         1. How suppliers move yield:  
            1. Gas mixes and inhibitors control anisotropy and sidewall passivation, which sets up taper, footing, and microtrenching  
            2. High selectivity to low-k dielectrics or to SIGe channels to preserve dimensions and keeps leakage/resistance in spec. Why this hits yield scaling: Better selectivity widens the process window; worse selectivity forces thicker hardmasks (more steps, more variability) or sacrifices CD control  
         2. Metrics to look for:  
            1. Selectivity ratios  
            2. Sidewall angle variability  
            3. Polymer residue composition  
            4. post-etch defectivity  
            5. via resistance distribution tails  
      3. [Planarity & Topography control](https://docs.google.com/document/u/0/d/1aO_IdsrtQOYYAEyfRk_zPh8rh5pKJs_H_04F5vxRKKE/edit): CMP slurries/pads \+ post-CMP cleans  
         1. How suppliers move yield:  
            1. Slurry oxidizers/inhibitors and pad mechanics set dishing/erosion and scratch counts; post-CMP cleaners suppress corrosion/particles  
            2. In BEOL, cmall improvements in within-die planarity preserve litho depth-of-focus and keep line resistance in spec  
         2. Why this hits yield/scaling:  
            1. Uneven topography shrinks your next litho window and pushes timing out of spec; scratches and residual metal ions are classic latent yield killers  
         3. Metrics:  
            1. WIW/WID planarity,  
            2. Scratch density,  
            3. Cu recess (nm)  
            4. Corrosion tests  
            5. Ionic contamination (ppt)   
      4. [Film Quality and Conformality](https://docs.google.com/document/u/0/d/1lby_st_zdmnLO8EPOQ6j55iDKuNe2GmZP_g272hNKEY/edit): ALD/CVD/PVD precursors and processes  
         1. How suppliers move yield:  
            1. High purity precursors and ligands produce films with lower hydrogen/carbon contamination, better conformality and grain structure (e.g., barrier/liner Ru/Co/TaN)  
            2. For gates and spacers (high-k/SiN/SiO), film stoichiometry and stress affect Vt variability and reliability (BTI/TDDB)  
         2. Why this hits yield/scaling: Film defects translate into threshold scatter, leakage, and electromigration risk; conformal liners reduce via resistance at shrinking dimensions  
         3. Metrics:  
            1. Impurity ppm/ppt  
            2. film resistivity  
            3. ALD step coverage at high AR  
            4. stress/strain  
            5. Time-dependent dielectric breakdown (TDDB)  
      5. [Purity and Containment control](https://docs.google.com/document/u/0/d/1Ib0g-u6Gubq6i2Uu2mieBrEL1GjWZXW4BvTt64IleuY/edit): wet chemicals, gases, filters, AMC  
         1. How Suppliers move yield:  
            1. UPW/wet chemical purity (metals, particles, TOC) and gas purity (H2O, O2, CO) directly set killer defect rates and plasma stability  
            2. AMC (amines/acids) control protects EUV/DUV resists; point-of-use liquid/gas filtration prevents particle adders  
         2. Why this hits yield/scaling: At advanced nodes, parts per trillion excursions show up as printable defects or gate oxide failures. Purity is “silent yield”  
         3. Metrics:  
            1. Metals/anion ppt  
            2. particle counts at critical sizes  
            3. AMC capture efficiency  
            4. Filter retention curves  
            5. Chamber clean efficiency gases (NFs/F2) and by-product control  
      6. [Interconnect performance and reliability](https://docs.google.com/document/u/0/d/1nEvcqvx7zmrLW_axf9Kk-kix2dSiLwltTctj_y9x5g8/edit): barriers, seeds, low-k dielectrics  
         1. How Suppliers move yield:  
            1. Next-gen barriers/seeds (e.g., Ru/Co liners, Mn treatments) cut line/via resistance and shore up electromigration  
            2. Low-k/ultra-low-k dielectrics (and caps) from materials vendors reduce RC delay; robust caps improve TDDB and EM margins  
         2. Why this hits yield/ scaling: As lines get narrower, resistance and EM dominate. Materials that lower R or raise EM lifetime keep timing and lifetime in spec at a given geometry  
         3. Metrics  
            1. line/via R distributions (P95/P99)  
            2. EM MTTF at operating J/T  
            3. Dielectric and leakage  
            4. Cap adhesion  
      7. [Advanced packaging enablement](https://docs.google.com/document/u/0/d/1FLlT1yCi3lWoH4EwGgvSooIBE-L1EvDTUDLho-TTP5Q/edit): ABF/BT, planting chemistries, underfills, TIMs  
         1. How suppliers move yield:  
            1. ABF/BT resin properties (Dk/Df, CTE) enable finer substrate lines/space with less warpage – essential HBM/chiplets  
            2. Plating chemistries shape RDL/pillar quality (voids, over-plating); underfills and EMCs determine assembly yield and long-term reliability  
            3. TIMs and die attach set junction-to-case thermal resistance, protecting silicon reliability margins  
         2. Why this hits yield/scaling:  
            1. System-level scaling (fan-out, 2.5D/3D) is now performance critical; substrate and plating materials gate I/O density and assembly yield  
         3. Metrics  
            1. L/S capability on substrate  
            2. Warpage at reflow  
            3. Void rate  
            4. RDL thickness uniformity  
            5. Thermal resistance (C/W)  
            6. Moisture sensitivity level

3. What are the geopolitical vulnerabilities in this stage of the supply chain?  
   1. There are several material-stage geopolitics “pressure-points”. Below they’re grouped by material family  
   2. Lithography chemistry and reticle stack (Japan-centric)  
      1. Photoresists and high purity HF:  
         1. Japan historically supplies \~90% of photoresists; its 2019 export controls to Korea showed how a single policy move can jam leading-edge fabs. HF for advanced nodes also skews to a small Japan/Korea supplier set.  
      2. EUV Pellicles: Commercial EUV Pellicles are licensed by ASML to Mitsui Chemicals (Japan).   
      3. EUV mask blanks: Effectively a Japan Duopoly (AGC, HOYA). Even routine capacity shifts (or disaster risks) move the entire advanced node schedule  
   3. Excimer-laser gases (DUV) and chamber cleans  
      1. Neon: Ukraine’s Cryoin and Ingas historically provided about half of the semiconductor-grade neon; the 2022 invasion abruptly halted output – demonstrating extreme geographic concentration risk for DUV exposure capacity  
      2. NF3 (chamber clean gas):A fatal Kanto Denka plant fire in Japan idled part of a globally important NF3 line, spotlighting just how few suppliers there are  
   4. Engineered substrate and wafers  
      1. **RF-SOI / FD-SOI:** **Soitec** (France) is the anchor with \~**70%** RF-SOI share; most rivals use its tech under license. Any disruption in France or export policy changes ripple into RF front-end supply chains.  
      2. **300 mm prime silicon:** An oligopoly (SEH/SUMCO/GlobalWafers/Siltronic/SK Siltron). Not single-source, but capacity is slow/CapEx-heavy, so **policy or disaster shocks** translate to long lead-time spikes. (Use this as a background structural risk; pair with your vendor ramp intel.)  
   5. Advanced Packaging dielectrics and chemistries  
      1. ABF build-up film: Ajinomoto Fine-techno holds a dominant share (90-95%) and has kept expansions largely inside of Japan; political risk or domestic disruption can bottleneck high-end CPU/GPU substrates  
   6. Critical Minerals and precursors  
      1. **Gallium / Germanium (for GaN/GaAs, optics, and some catalysts):** China imposed and later **tightened export controls**, with 2025 customs data showing **germanium exports down \~95%** vs. January; prices spiked, underscoring leverage over III-V and IR-optics chains. 

### Research Topics

1. Why 300mm? And what is the difference in wafers regarding logic/memory?  
2. Can combinations of masks/resists/etc close the gap between what is possible between DUV and EUV? Especially regarding the scale of nm nodes.

## Wafer Fab Equipment

Below is the WFE landscape by tool category

1. Lithography Scanners  
   1. Arguably the most critical and expensive equipment in the modern fab. Lithography is the process of printing a circuit pattern onto a silicon wafer. A litho scanner projects light through a master template (mask, reticle) and onto a light sensitive chemical layer (photoresist) on the wafer. This transfers circuit design, layer by layer, onto the silicon.  
      1. EUV: Uses extreme short wavelength light (13.5nm) to print the smallest, most advanced features. ASML is the sole manufacturer of these machines.  
      2. DUV: uses longer wavelength (193 or 248 nm) and is the workforce for printing less critical layers.  
      3. NIL (Nanoimprint Litho): An emerging tech that physically presses a patterned template into the resist.  
   2. Key players:  
      1. ASML (EUV, DUV)  
      2. Nikon (DUV)  
      3. Canon (DUV, NIL)  
2. Coaters/Developers (tracks)  
   1. These machines work hand in hand with litho scanners and are often physically linked into a single automated system  
      1. Coaters: Precisely applies various liquid chemical layers onto the wafer before it goes into the scanner. This includes the light-sensitive photoresist and other layers like anti-reflective coatings. The wafer is spun at high speed to create a perfectly uniform, thin film  
      2. Developers: After the wafer has been exposed in the scanner, the developer selectively washes away parts of the photoresists to reveal the printed pattern  
   2. Key Players:  
      1. Tokyo Electron (TEL)  
      2. Screen Semiconductor Solutions  
3. Etch and Strip  
   1. Once a pattern is created in the photoresist layer, etch tools are used to permanently transfer that pattern into the underlying material on the wafer (silicon, metal film). Strip tools then clean off the remaining resist.  
      1. Etch: Uses a plasma of highly reactive gasses (often containing fluorine or chlorine) to selectively remove material from the areas not protected by photoresist. The goal is to create sharp, vertical sidewalls for the circuit features. Think of it as a highly controlled chemical sandblasting process at the atomic scale  
      2. Strip: After the etch is complete, the remaining photoresist mask is stripped away, usually with a different plasma chemistry or wet chemicals, leaving behind the newly patterned layers  
   2. Key Players:  
      1. Lam research  
      2. TEL  
      3. Applied Materials  
      4. China:  
         1. AMEC  
         2. Naura  
4. Deposition  
   1. Deposition tools are used to add thin layers of various materials (metals, dielectrics, semiconductors) onto the wafer. This is how the different components of a transistor and the wiring between them are built up.  
      1. PVD (Physical Vapor Deposition) / Sputter: A physical process where a target material (like copper or titanium) is bombarded with high-energy ions, knocking atoms off the target that then fly and deposit on to the wafer, creating a thin film  
      2. CVD (Chemical Vapor Deposition) / ALD (Atomic Layer Deposition): A chemical process where precursor gases react on the wafer’s hot surface to form the desired solid film  
         1. CVD grows a film continuously  
         2. ALD is a more precise variant where precursor gases are pulsed in one at a time, allowing for the deposition of one single atomic layer at a time. This gives exceptional control over thickness and conformality (The ability to even coat complex 3D structures  
      3. Epitaxy: A specialized form of deposition that grows a single-crystal film on top of a single-crystal substrate. The new film’s crystal structure is an exact extension of the underlying wafer’s, leading to very high quality electronic properties  
   2. Key Players:  
      1. PVD/Sputter  
         1. Applied Materials  
         2. TEL  
         3. ULVAC  
         4. Canon Anelva  
      2. CVD/ALD  
         1. Applied Materials  
         2. TEL  
         3. Lam (via Novellus)  
         4. ASM International (ALD)  
         5. China  
            1. Naura  
            2. Piotech  
      3. Epitaxi (Si and Compound)  
         1. ASM International  
         2. Applied Materials  
         3. AIXTRON  
         4. Veeco  
         5. LPE (SiC)  
5. Wet Clean / Bevel Clean / ECP  
   1. These processes all involve liquids:  
      1. Wet clean: Wafers are cleaned hundreds of times throughout the manufacturing process.Wet clean uses ultra-pure water and specialized chemicals to remove microscopic particles that could kill the chip  
      2. Bevel clean: cleans the slanted edge of the wafer to prevent particles from flaking and contaminating other areas  
      3. ECP (Electro-Chemical Planting): A process used to deposit metal, primarily copper for the interconnect wiring. The process fills the trenches and vias that form the circuit’s wiring  
   2. Key Players:  
      1. SCREEN  
      2. TEL  
      3. ACM Research  
      4. Shibaura Mechatronics  
6. Chemical Mechanical Planarization (CMP)  
   1. As dozens of layers are deposited and etched, the wafer’s surface becomes bumpy and uneven. CMP is a critical step that re-flattens the wafer surface after certain layers are added.   
   2. Key Players:  
      1. Applied Materials  
      2. EBARA  
      3. China:  
         1. Hwatzing  
7. Ion Implantation  
   1. This is the primary method for doping a semiconductor. Doping involves intentionally introducing specific impurities into the silicon crystal lattice to change its electrical properties (creating N-type or P-type regions). An Ion implanter generates a beam of ions (e.g., boron, phosphorous) and accelerates them with high voltage, shooting them directly into the wafer so they embed at specific depth  
   2. Key players:  
      1. Axcelis  
      2. Applied Materials (Varian)  
      3. Nizzan Ion Equipment  
8. Thermal (RTP, Furnace, Anneal)  
   1. These tools use heat to modify the properties of the wafer and the films on it  
      1. Furnace: A large chamber that processes wafers in batches, often 100 to 150 at a time, for long periods. Used for processes like oxidation (growing a silicon dioxide layer) and some types of deposition.   
      2. Rapid Thermal Processing (RTP): Heats a single wafer to very high temperatures, over 1000°C in just a few seconds using high-intensity lamps. It's used for annealing, a process that repairs crystal damage caused by ion implantation and electrically activates the dopant atoms.   
   2. Key players:  
      1. Kokusai Electric (Batch)  
      2. TEL  
      3. Applied Materials  
      4. Mattson  
9. Metrology and Inspection  
   1. Essentially the eyes and ears of the fabrication process; used to monitor the process and ensure quality  
      1. Metrology: Tools that measure Critical Dimensions (CD), film thickness, and layer alignment (overlay). Examples include CD-SEMs (Scanning Electronic Microscopes for measuring feature sizes) and ellipsometers for measuring film thickness  
      2. Inspection: Tools that find defects. They scan the wafer with lasers or electron beams to find tiny particles, scratches, or pattern errors that could cause the chip to fail.   
   2. Key Players:  
      1. KLA (Leader)  
      2. ASML/HMI (e-beam)  
      3. Hitachi High-Tech (CD-SEM)  
      4. Onto Innovation  
      5. Nova  
      6. Camtek  
      7. Lasertec (EUV mask inspection)  
10. Mask and Reticle Equipment  
    1. Specialized tools needed to manufacture and qualify the photomasks used in lithography scanners  
       1. Mask Writers: Use a focused electron beam (e-beam) to “write” the master circuit pattern onto a mask blank (a quartz plate coated with an absorber material like chromium)  
       2. Mask Inspection: Just like wafers, finished masks must be inspected for any defects, as a single defect on the mask would be printed on every wafer, killing the yield.  
    2. Key players:  
       1. NuFlare and JEOL (e-beam mask writers), KLA (reticle Inspection), Lasertec (EUV mask/blank inspection).  
11. Critical Subsystem  
    1. These are not the stand alone machines that process wafers, but rather the highly complex, essential components that are integrated inside the WFE tools. The performance of these subsystems is often the limiting factor for the performance of the entire system  
       1. Optics and Light sourcesZEISS makes the massive, multi-mirror optical systems for ASML’s EUV scanners. Cymer (Owned by ASML) and Gigaphoton make the powerful laser systems that generate the DUV and EUV light  
       2. Vacuum and power: Many processes (Etch, Deposition, Implantation) happen in a vacuum. Companies like Edwards, Pfeiffer, and VAT Group make the pumps, valves, and gauges needed to create and control this environment. MKS instruments provides the radio frequency (RF) power generators needed to create and sustain the plasma used in etch and deposition tools

### Research Questions

1. Why is ASML’s EUV monopoly such a bottleneck for the entire industry?  
   1. Essentially, ASML is the only company in the world that can manufacture the machine that builds the SOTA chips.   
      1. The complexity of EUV Lithography plays a major role in keeping the competition at bay.   
         1. To create the 13.5 nm wavelength light needed, a high-powered, CO2 laser is fired at a microscopic droplet of molten tin 50,000 times per second. The light is emitted by the plasma created by this process  
         2. EUV light is absorbed by almost everything, so the mirrors used (made by ZEISS) are the smoothest objects ever created so that they can reflect the light.  
      2. Additionally, the cost would be astronomical to try to enter this space (Equipment, Research, Customer trust)  
   2. Consequences of a single supplier:  
      1. ASML can only make about 50-60 machines per year. Three major customers fight for that capacity: TSMC, Samsung, Intel.  
      2. The waitlist can be years. If any issues arise and ASML slows or stops production, global supply of cutting-edge chips would be directly affected. (Smartphones, Datacenters, etc)  
   3. Gatekeepers of Moore’s law:  
      1. Chipmakers can only design chips with features as small as ASML’s equipment can make. The progress (5,3,2,1.8 nm) is entirely dependent on the progress made by ASML  
   4. Geopolitical chokepoint:  
      1. EUV technology has been used as a form of leverage against countries like China; essentially blocking them from developing sub 7nm nodes.

## Foundries

Contract Manufacturers fabricate chips to other companies’ designs.

1. ### Key Players

   1. TSMC: Clear leader at the cutting edge  
      1. Q2 2025 \- 70% of foundry revenue on AI GPU and smartphone ramps  
      2. N2 volume production on track for H2’25; N2P H2’26, A16 H2’26, A14 in 2028  
      3. CoWos Advanced \-packaging push: \~75K wafers per month in wow5 (\~2x 2024), still a constraint area  
      4. US footprint: Arizona cluster scaling; mgmt says \~30% of 2nm+ capacity will be in AZ  
   2. Samsung: GAA early adopter, chasing share  
      1. Shipping 3nm GAA/MBCFET; SF2 (2nm-class) targeted from 2025 in roadmap; US Taylor fab building toward 2nm with late-2026/27 HVM targets reported  
   3. Intel Foundry: rebuilding, strong packaging, customer proofs  
      1. External 18A activity continues; 14A still in question due to lack of external customers  
   4. UMC: 22/28 nm specialist, high utilization  
      1. 22/28 nm hit 40% of revenue in Q2 2025; utilization is at 70%; focus areas include display drivers, controllers, connectivity  
   5. Global Foundries: “feature rich” focus (RF, power, FD-SOI, auto  
      1. Strategy is not leading edge logic, but comms/auto/edge logic  
   6. SMIC: Advanced via DUV multipatterning, rising domestic ecosystem  
      1. Working at 7nm and pushing towards 5nm at higher costs (no EUV)  
   7. Tier 2 analog/power specialists:  
      1. Tower, China’s HuaHong/HHGrace, Taiwan’s PSMC/VIS  
   8. Research task: Look tiers and market share

2. ### How Foundries make money

   1. Node mix and ASPs: Advanced nodes carry far higher Wafer Pricing; AI demands shift mix  
   2. Utilization and WSPM (wafer starts per month) by fab/region (can help identify margin leverage)  
   3. Advanced Packaging Capacity (CoWoS, SoIC, Foveros, I-Cube/X-Cube); still a bottle neck  
   4. CapEx and footprint (Where the next fabs are and exposure to Taiwan/US/Japan/EU

3. ### Risks and chokepoints to note

   1. Packaging throughput can cap AI silicon shipments even if frontend capacity exists  
   2. EUV/High NA adoption timeline  
   3. Geopolitics and concentration (Taiwan share of cutting edge; US/EU/Japan onshoring; export controls)

## IDM

An IDM is a Semiconductor Company that designs chips, manufactures them (in own fabs), and sells them (Essentially, they’re vertically integrated)

- IDM owns product \+ process: More control and more capital intensive  
- Foundry: manufacturer for others  
- Fabless: Design, outsources manufacturing

IDMs were the industry standard, but now only a few remain. IDMs Tends to win when:

1. Tight coupling between design and manufacturing is a durable advantage  
2. Scale, quality, or reliability matters more than being at the very cutting edge

Typical IDM advantages:

* Control of supply, Less exposed to foundry shortages for core products  
* Process specialization, especially in analog power, RF, and sensors  
* Quality and reliability: Automotive/industrial qualification, Long life cycles  
* IP plus manufacturing know-how together, harder to copy

Typical IDM tradeoffs:

- Huge fixed costs (Fabs \+ tools \+ long deprecation cycles)  
- Utilization risks (little demand, little margin)  
- Tech pacing pressure

### IDM Types

1. Leading Edge Logic (Often hybrid now)  
   1. Example: Intel moved to hybrid model: keep internal fabs, used external when it makes sense, offer foundry services to external fabless companies  
2. Memory IDM  
   1. Often vertically integrated because scale and process learning dominate  
3. Analog/Embedded/”foundational” IDM  
   1. TI is leaning hard into domestic high-volume manufacturing investment for foundational semiconductors (mature nodes, long tail demand)  
4. Power / Automotive / Industrial  
   1. Example: STMicroelectronics is building highly integrated silicon carbide setup that includes manufacturing \+ test/packaging

## Fabless

Fabless companies design and sell chips, but they outsource the fabrication to a foundry

1. Design inputs:  
   1. EDA Tools  
   2. IP Cores (ARM CPU IP, PCIe, mem controllers, etc)  
2. Manufacturing  
   1. Foundry  
   2. Mask shop and PDK ecosystem (tight coupling between fabless and foundry)  
3. Backend  
   1. OSAT \+ Advanced packaging  
4. Customers  
   1. OEMs (Phones/PC/Auto), hyperscalers, data centers, device makers