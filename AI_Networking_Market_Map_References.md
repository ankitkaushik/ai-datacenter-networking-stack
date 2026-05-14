# AI Datacenter Networking Supply Chain — References

Companion document to `AI_Networking_Market_Map.html`. Each numbered reference is cited in the visualization by its [#] tag. Primary sources (company press releases, 10-Ks, official documentation) are preferred; secondary sources (trade press) are used for synthesis and verification.

Last verified: May 14, 2026.

---

## Layer 1 — Frontier AI Companies

[1] xAI, "Colossus: The World's Largest AI Supercomputer." — Confirms 100K → 200K NVIDIA Hopper GPUs on Spectrum-X Ethernet. https://x.ai/colossus

[2] NVIDIA Newsroom, "NVIDIA Ethernet Networking Accelerates World's Largest AI Supercomputer, Built by xAI." — Spectrum-X 95% throughput vs 60% standard Ethernet. https://nvidianews.nvidia.com/news/spectrum-x-ethernet-networking-xai-colossus

[3] xAI, "New Compute Partnership with Anthropic" (2026). — Anthropic renting Colossus 1 capacity, Spectrum-X exposure. https://x.ai/news/anthropic-compute-partnership

[4] OpenAI, "MRC: Multipath Reliable Connection — Supercomputer Networking." — OpenAI custom transport stack signal. https://openai.com/index/mrc-supercomputer-networking/

[5] Meta Engineering, "Meta open-sources transport stack to scale AI training to over 100K GPUs." — Meta's RDMA-over-Ethernet stack on Arista. https://www.sdxcentral.com/news/meta-open-sources-transport-stack-to-scale-ai-training-to-over-100k-gpus/

[6] Arista Networks Blog, "Meta and Arista Build AI at Scale." — Meta's 24K H100 cluster using 7800 + Minipack2 + Wedge400 RoCE fabric. https://blogs.arista.com/blog/meta-and-arista-build-ai-at-scale

[7] Data Center Frontier, "Closer Look: Meta's Custom ASIC for AI Computing (MTIA)." — Meta MTIA v2 inference accelerator. https://www.datacenterfrontier.com/servers/article/33005340/closer-look-metas-custom-asic-for-ai-computing

[8] Data Center Dynamics, "Meta places order for its next-gen ASIC-powered AI servers, partners with Broadcom and Quanta." — Meta–Broadcom MTIA training collaboration. https://www.datacenterdynamics.com/en/news/meta-places-order-for-its-next-gen-asic-powered-ai-servers-partners-with-broadcom-and-quanta-computer/

---

## Layer 2 — Hyperscalers & Neoclouds (and in-house networking)

[9] Google Cloud Blog, "The evolution of Google's Jupiter data center network." — Jupiter + MEMS OCS, 5x speed, 40% less power. https://cloud.google.com/blog/topics/systems/the-evolution-of-googles-jupiter-data-center-network

[10] Google Research, "Jupiter Evolving: Transforming Google's Datacenter Network via Optical Circuit Switches and Software-Defined Networking" (SIGCOMM '22). https://research.google/pubs/jupiter-evolving-transforming-googles-datacenter-network-via-optical-circuit-switches-and-software-defined-networking/

[11] SemiAnalysis, "Google OCS Apollo: The >$3 Billion Game-Changer in Datacenter Networking." — Apollo OCS scale, custom TPU pod interconnect. https://newsletter.semianalysis.com/p/google-apollo-the-3-billion-game

[12] Introl Blog, "Google TPU Architecture: 7 Generations Explained" — TPU v4/v5/Ironwood OCS pod topology. https://introl.com/blog/google-tpu-architecture-complete-guide-7-generations

[13] HPCwire, "Google Aims to Flip the Script on AI Inference with New Ironwood TPUs" — Ironwood 9,216 chips, 48 OCS units. https://www.hpcwire.com/2025/11/10/google-aims-to-flip-the-script-on-ai-inference-with-new-ironwood-tpus/

[14] AWS, "Elastic Fabric Adapter (EFA)." — In-house OS-bypass NIC with SRD protocol on Nitro card. https://aws.amazon.com/hpc/efa/

[15] IEEE Xplore, Shalev et al., "A Cloud-Optimized Transport Protocol for Elastic and Scalable HPC" — AWS SRD paper. https://ieeexplore.ieee.org/document/9167399/

[16] Microsoft Azure Blog, "SONiC: the network innovation powerhouse behind Azure." — SONiC powers Azure + AI platforms; multi-ASIC. https://azure.microsoft.com/en-us/blog/sonic-the-network-innovation-powerhouse-behind-azure/

[17] NVIDIA Technical Blog, "Choosing NVIDIA Spectrum for Microsoft Azure SONiC." — Azure runs SONiC on NVIDIA Spectrum silicon. https://developer.nvidia.com/blog/choosing-spectrum-for-microsoft-azure-sonic/

[18] HUBER+SUHNER, "Strengthening collaboration with Microsoft for HCF" (Apr 2026). — Hollow-core fiber deployment in Azure backbone. https://www.hubersuhner.com/en/newsroom/company-news/news-ad-hoc-news/hubersuhner-strengthens-collaboration-with-microsoft-to-advance-global-deployment-of-hollow-core-fi

[19] Network World, "Neoclouds roll in, challenge hyperscalers for AI workloads." — CoreWeave / Lambda / Nebius / Crusoe positioning. https://www.networkworld.com/article/4011187/neoclouds-roll-in-challenge-hyperscalers-for-ai-workloads.html

[20] SemiAnalysis, "ClusterMAX™ 2.0: The Industry Standard GPU Cloud Rating System." — Neocloud NIC/fabric tracking (InfiniBand vs Spectrum-X). https://newsletter.semianalysis.com/p/clustermax-20-the-industry-standard

[21] DigitalOcean, "7 CoreWeave Alternatives for Cloud GPU Computing in 2025." — Voltage Park scale (24K H100s), neocloud fabric strategies. https://www.digitalocean.com/resources/articles/coreweave-alternatives

---

## Layer 3 — Networking Equipment Suppliers

### NVIDIA

[22] NVIDIA Newsroom, "NVIDIA Announces New Switches Optimized for Trillion-Parameter GPU Computing and AI Infrastructure." — Spectrum-X800, Quantum-X800, BlueField-3, LinkX. https://nvidianews.nvidia.com/news/networking-switches-gpu-computing-ai

[23] NVIDIA Docs, "NVIDIA Quantum, Spectrum, and LinkX Product Lines." — Product catalog including Spectrum-4 SN5600, Quantum-2/3, ConnectX-8, LinkX optics. https://docs.nvidia.com/networking/display/400g100gpam4ovpub/nvidia-quantum,-spectrum,-and-linkx-product-lines

[24] The Next Platform, "Nvidia Weaves Silicon Photonics Into InfiniBand And Ethernet" (Mar 2025). — CPO integration into Quantum-X and Spectrum-X. https://www.nextplatform.com/2025/03/18/nvidia-weaves-silicon-photonics-into-infiniband-and-ethernet/

[25] Network World, "Nvidia networking roadmap: Ethernet, InfiniBand, co-packaged optics will shape data center of the future." — Quantum 3450-LD (late 2025), SN6810/SN6800 (2026), Vera Rubin CPO roadmap. https://www.networkworld.com/article/4050881/nvidia-networking-roadmap-ethernet-infiniband-co-packaged-optics-will-shape-data-center-of-the-future.html

### Broadcom

[26] Broadcom Investors, "Broadcom Announces Tomahawk® 6 – Davisson, the Industry's First 102.4-Tbps Ethernet Switch with Co-Packaged Optics." — 3rd-gen CPO, 70% optical interconnect power reduction. https://investors.broadcom.com/news-releases/news-release-details/broadcom-announces-tomahawkr-6-davisson-industrys-first-1024

[27] Broadcom Blog, "Broadcom Advances Industry Support for Ethernet for AI Networking at the 2025 OCP Global Summit." — Tomahawk 6, Tomahawk Ultra, Jericho4, Thor Ultra 800G NIC. https://www.broadcom.com/blog/2025-ocp-global-summit-broadcom-advances-industry-support-for-ethernet-for-ai-networking

[28] NADDOD Blog, "Broadcom's Tomahawk 6 Delivers 102.4 Tb/sec Ethernet for AI-Scale Fabrics" — Chiplet architecture, 200G SerDes specifics. https://www.naddod.com/blog/broadcom-tomahawk-6-102-4-t-ethernet-switch-chip-for-ai-fabrics

### Marvell

[29] Marvell Investor Relations, "Marvell to Acquire Celestial AI, Accelerating Scale-up Connectivity for Next-Generation Data Centers" (Dec 2025). — $3.25B deal, scale-up optical I/O. https://investor.marvell.com/news-events/press-releases/detail/1000/marvell-to-acquire-celestial-ai-accelerating-scale-up-connectivity-for-next-generation-data-centers

[30] The Next Platform, "With Celestial AI Buy, Marvell Scales Up The Datacenter And Itself." — Celestial AI 16 Tbps Photonic Fabric chiplet integration. https://www.nextplatform.com/2025/12/04/with-celestial-ai-buy-marvell-scales-up-the-datacenter-and-itself/

[31] Marvell, "Marvell Extends Connectivity Leadership with AEC Ecosystem Demonstrations at OFC 2025." — Alaska A 1.6T AEC DSP, partners Amphenol/TE/Molex. https://www.marvell.com/company/newsroom/marvell-extends-connectivity-leadership-with-aec-ecosystem-demonstrations-at-ofc-2025.html

[32] Marvell, "Marvell Optical DSPs | Powering the Future of AI Infrastructure." — Inphi-derived optical DSP roadmap. https://www.marvell.com/solutions/data-center/optical-dsp.html

### Cisco

[33] Cisco Newsroom, "Cisco Announces New Silicon One G300, Advanced Systems and Optics to Power and Scale AI Data Centers for the Agentic Era" (Feb 2026). — 102.4 Tbps G300 ASIC, LPO-aligned optics. https://newsroom.cisco.com/c/r/newsroom/en/us/a/y2026/m02/cisco-announces-new-silicon-one-g300.html

[34] Cisco Data Sheet, "Cisco Silicon One G300." — 64x 1600 GbE, 512x 200G SerDes, scale-up/scale-out roles. https://www.cisco.com/c/en/us/solutions/collateral/silicon-one/silicon-one-g300-ds.html

[35] The Register, "Cisco unveils 102.4T Silicon One G300 switch chip." — Independent confirmation of specs and AI positioning. https://www.theregister.com/2026/02/10/cisco_challenges_broadcom_nvidia_switch_chips/

### Arista

[36] Arista Networks Press Release, "Arista Unveils Etherlink AI Networking Platforms." — 7060X6 (Tomahawk 5), 7800R4 (Jericho3-AI), 7700R4 DES. https://www.arista.com/en/company/news/press-release/19493-arista-unveils-etherlink-ai-networking-platforms

[37] Arista 7700R4 Data Sheet — Distributed Etherlink Switch specifications. https://www.arista.com/assets/data/pdf/Datasheets/7700R4-Distributed-Etherlink-Switch-Datasheet.pdf

[38] Arista Press Release, "Arista Networks Unveils Next Generation Data and AI Centers" (Oct 2025). — Latest AI portfolio expansion. https://www.arista.com/en/company/news/press-release/22541-pr-10292025

### HPE

[39] The Next Platform, "HPE Upgrades Supercomputer Lineup Top To Bottom In 2025." — Slingshot 400 with Rosetta-2 switch + Cassini-2 NIC, in-house silicon. https://www.nextplatform.com/2024/11/26/hpe-upgrades-supercomputer-lineup-top-to-bottom-in-2025/

[40] The Next Platform, "How Will Juniper Change HPE's Datacenter Networking Strategy?" — Aruba uses mix of own ASICs and Broadcom; AMD DPU partnership. https://www.nextplatform.com/2025/07/02/how-will-juniper-change-hpes-datacenter-networking-strategy/

### Credo

[41] Credo Investor Relations, "Credo Agrees to Acquire DustPhotonics" (Apr 2026). — $750M cash + ~0.92M shares; vertically integrated SerDes/DSP/SiPho. https://investors.credosemi.com/news-events/news/news-details/2026/Credo-Agrees-to-Acquire-DustPhotonics-Accelerating-Expansion-into-Silicon-Photonics-and-Next-Generation-Optical-Connectivity/default.aspx

[42] BusinessWire/Credo, full release with $500M FY2027 optical revenue target. https://www.businesswire.com/news/home/20260413933103/en/Credo-Agrees-to-Acquire-DustPhotonics

### Astera Labs

[43] Astera Labs Product Page, "Aries PCIe/CXL Smart DSP Retimers." — Aries 6 PCIe Gen 6 retimers, AECs. https://www.asteralabs.com/products/pcie-cxl-smart-dsp-retimers/

[44] Astera Labs Products Overview — Aries (retimers), Taurus (Ethernet smart cable), Leo (CXL memory), Scorpio (fabric switch), COSMOS (software). https://www.asteralabs.com/products/

[45] Astera Labs Press Release, "Astera Labs Ramps Production of PCIe 6 Connectivity Portfolio." — Scorpio P-Series PCIe 6 fabric switches. https://ir.asteralabs.com/news-releases/news-release-details/astera-labs-ramps-production-pcie-6-connectivity-portfolio

### MaxLinear

[46] MaxLinear Investors, "MaxLinear Unveils Rushmore: Low-Power 1.6T PAM4 DSP for AI/ML and Data Center Networks." — 200G/lane, <25W optical module support, Ethernet + InfiniBand compatible. https://investors.maxlinear.com/press-releases/detail/569/maxlinear-unveils-rushmore-low-power-1-6t-pam4-dsp-for

[47] MaxLinear Investors, "MaxLinear Unveils Annapurna 224G Scale-Up Retimer to Extend Copper Connectivity in AI Data Centers." — 224G PAM4 retimer for AECs / backplanes; Q2 2026 availability. https://investors.maxlinear.com/press-releases/detail/603/maxlinear-unveils-annapurna-224g-scale-up-retimer-to-extend

### Ayar Labs

[48] Ayar Labs, "Ayar Labs Unveils World's First UCIe Optical Chiplet for AI Scale-Up Architectures" (Mar 2025). — TeraPHY 8 Tbps + SuperNova 16-wavelength laser. https://ayarlabs.com/news/ayar-labs-unveils-worlds-first-ucie-optical-chiplet-for-ai-scale-up-architectures/

[49] Semiwiki, "Alchip and Ayar Labs' Co-Packaged Optics Breakthrough at TSMC OIP 2025." — 100+ Tbps per accelerator scale-up demo. https://semiwiki.com/semiconductor-services/362133-revolutionizing-ai-infrastructure-alchip-and-ayar-labs-co-packaged-optics-breakthrough-at-tsmc-oip-2025/

### Lightmatter

[50] Lightmatter, "Lightmatter Unveils Passage M1000 Photonic Superchip, World's Fastest AI Interconnect." — 114 Tbps optical, 4,000 mm² interposer, 256 fibers. https://lightmatter.co/press-release/lightmatter-unveils-passage-m1000-photonic-superchip-worlds-fastest-ai-interconnect/

[51] ServeTheHome, "Lightmatter Passage M1000 at Hot Chips 2025." — Architecture detail; runs on GF Fotonix SiPho process. https://www.servethehome.com/lightmatter-passage-m1000-at-hot-chips-2025/

### Celestial AI

[52] Photonics Spectra, "Marvell to Acquire Celestial AI for $3.25B." — Photonic Fabric chiplet, scale-up optical I/O. https://www.photonics.com/Articles/Marvell-to-Acquire-Celestial-AI-for-325B/a71734

### POET Technologies

[53] POET Technologies, "POET Technologies Redefines Optical Integration with Its Hybrid-Integrated 1.6T 2xFR4 Transmitter PIC." — POET Optical Interposer scalable to 3.2T. https://www.poet-technologies.com/blog/poet-technologies-redefines-optical-integration-with-its-hybrid-integrated-1-6t-2xfr4-transmitter-pic

[54] POET Technologies, "POET Technologies Receives $5 Million Production Order for 800G Optical Engines." https://www.poet-technologies.com/news/poet-technologies-receives-5-million-production-order-for-800g-optical-engines

[55] POET Technologies / Quantum Computing Inc., "Co-Develop 3.2 Tbps Optical Engines for CPO." — TFLN modulator + POET interposer collaboration. https://www.poet-technologies.com/news/poet-technologies-and-quantum-computing-inc-to-co-develop-3-2-tbps-optical-engines-for-cpo-and-next-gen-ai-connectivity

### Zhongji Innolight & Eoptolink (transceiver wrappers)

[56] IP-Fiber, "Nvidia Orders Surge: InnoLight and Eoptolink Dominate 60% of 800G SFP Optical Modules Supply." — NVIDIA supplier-share split. https://ip-fiber.com/blogs/news/nvidia-orders-surge-innolight-and-eoptolink-dominate-60-of-800g-sfp-optical-modules-supply

[57] Eoptolink, "Eoptolink Unveils Industry-First 800G Optical Transceiver for Multicore Fiber at OFC 2025/2026." — 1.6T OSFP-XD product line. https://www.eoptolink.com/news/358-eoptolink-unveils-industry-first-800g-optical-transceiver-for-multicore-fiber-at-ofc-2026

[58] SemiAnalysis, "Nvidia's Optical Ascent: >$1B Revenue; The Missing 800G Ramp." — NVIDIA optical revenue and Innolight/Eoptolink role. https://newsletter.semianalysis.com/p/nvidias-optical-ascent-1b-revenue

### Huber+Suhner

[59] HUBER+SUHNER + Microsoft Azure — Hollow-core fiber rollout (2026). https://opticalconnectionsnews.com/2026/04/hubersuhner-and-microsoft-azure-to-announce-new-investment-to-advance-hollow-core-fibre/

---

## Layer 4 — EML/Laser & Optical-Component Suppliers

[60] TrendForce, "AI Data Centers Ignite a Laser Shortage Wave; Nvidia's Strategic Lock-In Reshapes the Global Laser Supply Chain." — 200G EML constraint, multi-supplier capacity. https://www.trendforce.com/presscenter/news/20251208-12823.html

[61] Chipstrat (Austin Lyons), "Lumentum and the Laser Bottleneck." — Lumentum 50–60% EML share; only volume supplier of 200G/lane EML. https://www.chipstrat.com/p/lumentum-and-the-laser-bottleneck

[62] FinancialContent, "The Light Engine of AI: A Deep Dive into Lumentum Holdings (LITE) and the 1.6T Revolution." — Lumentum $663M capacity expansion. https://markets.financialcontent.com/stocks/article/finterra-2026-3-26-the-light-engine-of-ai-a-deep-dive-into-lumentum-holdings-lite-and-the-16t-revolution

[63] Compound Semiconductor Magazine, "A tough 12 months for CS shares." — Coherent 6-inch InP wafer ramp. https://compoundsemiconductor.net/article/121810/A_tough_12_months_for_CS_shares

[64] Sumitomo Electric, "53 GBaud Electro-Absorption Modulator Integrated Lasers." — EML technical paper and product line. https://sumitomoelectric.com/sites/default/files/2023-04/download_documents/E96-05.pdf

[65] Sumitomo Electric, "Growth strategy for data-center-related business" (Nov 2025 deck). — Vertical InP-to-EML strategy. https://sumitomoelectric.com/sites/default/files/2025-11/download_documents/Growth%20strategy%20for%20data%20center-related%20business_2025.pdf

[66] Mordor Intelligence, "Indium Phosphide (InP) Wafer Market — Size, Share & Industry Analysis." — AXT, Sumitomo, Coherent (II-VI) as InP substrate leaders. https://www.mordorintelligence.com/industry-reports/indium-phosphide-wafer-market

[67] Journal of Semiconductors, "High-speed electro-absorption modulated laser." — EML technical baseline; Mitsubishi Electric, Hamamatsu cited among manufacturers. https://www.jos.ac.cn/en/article/doi/10.1088/1674-4926/25030015

---

## Layer 5 — Physical Layer & Advanced Packaging

### Passive copper / AECs / DACs

[68] Molex, "Active Electrical Cable Solutions." — AEC product family for AI rack interconnect. https://www.molex.com/en-us/products/connectors/high-speed-pluggable-io/active-electrical-cables-aec

[69] Introl, "Cables and Interconnects: DAC, AOC, AEC, and Fiber for 800G AI Data Centers (2025)." — Inventory of copper-vs-optical reach and economics. https://introl.com/blog/cables-interconnects-dac-aoc-aec-800g-ai-data-center-2025

[70] OpenPR / IntelMarketResearch, "AI Data Center Active Electrical Cable (AEC) Modules Research." — Molex/Amphenol/TE Connectivity collectively >45% AEC market share, 22% CAGR. https://www.intelmarketresearch.com/aec-active-cable-for-data-centers-market-27749

### Advanced packaging (CoWoS / COUPE / Foundries)

[71] TrendForce, "Silicon Photonics in the Spotlight: TSMC Lifts the Curtain on COUPE at SEMICON Taiwan" (Sep 2025). — COUPE = SoIC-X stacked optical engine on CoWoS roadmap. https://www.trendforce.com/news/2025/09/09/news-silicon-photonics-in-the-spotlight-tsmc-lifts-the-curtain-on-coupe-at-semicon-taiwan/

[72] 3D InCites, "IFTLE 642: TSMC Advanced Co-packaged Optics Integrated CoWoS and COUPE." — Technical detail: 6nm EIC + 65nm SOI PIC. https://www.3dincites.com/2025/10/iftle-642-tsmc-advanced-co-packaged-optics-integrated-cowos-and-coupe/

[73] DigiTimes, "TSMC integrates CoWoS packaging with Coupe photonics for AI performance boost." — Broadcom Tomahawk 6 CPO uses TSMC COUPE. https://www.digitimes.com/news/a20250812VL210/tsmc-cowos-performance-silicon-interposer.html

[74] TechSoda, "IP Insight #3: TSMC Accelerates in Silicon Photonics While Intel Becomes More Selective." — Intel Foundry SiPho positioning and hybrid-laser IP. https://techsoda.substack.com/p/ip-insight-3-tsmc-accelerates-in

[75] Lightmatter Hot Chips 2025 paper — GlobalFoundries Fotonix silicon-photonics platform used by Lightmatter Passage. https://lightmatter.co/wp-content/uploads/2025/08/57-lightmatter_hotchips_2025_final.pdf

---

## Cross-Cutting: Protocols & Software

### RoCEv2 / Ultra Ethernet vs InfiniBand

[76] Ultra Ethernet Consortium official site — founding members AMD, Arista, Broadcom, Cisco, Eviden, HPE, Intel, Meta, Microsoft; 100+ members by 2024. https://ultraethernet.org/

[77] HPCwire, "Ultra Ethernet Has Arrived: One Network to Rule Them All?" — UEC 1.0 (Jun 2025), 1.0.1 update. https://www.hpcwire.com/2025/09/09/ultra-ethernet-has-arrived-one-network-to-rule-them-all/

[78] Tom's Hardware, "AMD unveils industry's first Ultra Ethernet ready network card for AI and HPC." — Pensando Pollara 400 UEC NIC. https://www.tomshardware.com/networking/amd-unveils-industrys-first-ultra-ethernet-ready-network-card-for-ai-and-hpc

[79] SemiAnalysis, "The New AI Networks: Ultra Ethernet UEC, UALink, Broadcom SUE." — Scale-up vs scale-out framing. https://newsletter.semianalysis.com/p/the-new-ai-networks-ultra-ethernet-uec-ualink-vs-broadcom-scale-up-ethernet-sue

### CPO vs LPO

[80] The Register, "Copackaged optics have officially found their killer app." — CPO momentum at Broadcom + NVIDIA. https://www.theregister.com/2025/11/22/cpo_ai_nvidia_broadcom

[81] HPCwire, "Photonic Switches Promise to Keep GPUs Fed, Cool." — CPO power/latency benefits at scale. https://www.hpcwire.com/2025/10/01/photonic-switches-promise-to-keep-gpus-fed-cool/

### Collective communication libraries (NCCL / RCCL / MSCCL)

[82] NVIDIA Developer, "NVIDIA Collective Communications Library (NCCL)." https://developer.nvidia.com/nccl

[83] ROCm/rccl on DeepWiki — RCCL drop-in NCCL-compatible AMD library. https://deepwiki.com/ROCm/rccl

[84] arXiv, "MSCCL++: Rethinking GPU Communication Abstractions for Cutting-Edge AI Applications." — MSCCL/MSCCL++ background, up to 5.4x speedup. https://arxiv.org/html/2504.09014v2

