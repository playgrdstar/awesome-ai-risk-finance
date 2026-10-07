# Awesome AI Risk Management in Finance [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources for managing the risk of AI in financial services: supervisory guidance, standards, model risk management practice, tooling, research, and reading.

AI is landing in banks, insurers, asset managers, and the authorities that supervise them. The discipline for managing it is not new. Firms that already run model risk management, third-party risk, and technology risk already have most of what is needed; AI stretches each of them rather than replacing them. This list gathers the primary sources that matter, with a finance lens throughout.

The focus is deliberately narrow. It is about **AI risk in financial services**, not AI governance in general. Where a horizontal standard or tool is included, it is because it is routinely applied in finance.

Maintained by [Gary Ang](https://quaintitative.com/), who developed Singapore's AI Risk Management Guidelines (AIRG) while leading AI risk supervision at the MAS. Contributions are welcome: see [Contributing](CONTRIBUTING.md).

## Contents

- [Financial regulators and supervisory guidance](#financial-regulators-and-supervisory-guidance)
- [International bodies and standards](#international-bodies-and-standards)
- [Industry and consortium frameworks](#industry-and-consortium-frameworks)
- [Model risk management foundations](#model-risk-management-foundations)
- [Tools and open source](#tools-and-open-source)
- [Research, reports, and reading](#research-reports-and-reading)
- [From the maintainer](#from-the-maintainer)
- [Contributing](#contributing)
- [Licence](#licence)

## Financial regulators and supervisory guidance

Supervisory guidance from the authorities that regulate financial institutions, organised by jurisdiction. These are the texts a firm is actually held to.

### Singapore (MAS)

- [Guidelines on AI Risk Management (AIRG) (MAS, 2026)](https://www.mas.gov.sg/regulation/guidelines/guidelines-on-artificial-intelligence-risk-management-for-financial-institutions) - MAS' final sector-wide Guidelines on AI Risk Management for all financial institutions, issued on 7 October 2026 after consultation in November 2025, and taking effect in phases from 7 October 2027 to 7 October 2028, covering AI oversight, lifecycle controls, risk materiality and governance, and explicitly including generative AI and AI agents.
- [Information Paper on AI Model Risk Management (MAS, 2024)](https://www.mas.gov.sg/publications/monographs-or-information-paper/2024/artificial-intelligence-model-risk-management) - Good practices on AI and generative-AI model risk management observed in MAS' 2024 thematic review of banks, which informed the later AIRG.
- [Principles to Promote Fairness, Ethics, Accountability and Transparency (FEAT) (MAS, 2018)](https://www.mas.gov.sg/publications/monographs-or-information-paper/2018/feat) - MAS's founding principles for responsible use of AI and data analytics in Singapore finance, which later MAS AI guidance builds on.
- [Project MindForge (MAS, 2023 onward)](https://www.mas.gov.sg/schemes-and-initiatives/project-mindforge) - MAS-led consortium that produced a generative-AI risk framework and the AI Risk Management Toolkit covering traditional, generative and agentic AI.
- [Safeguards for Agentic Finance at Runtime (SAFR) (MAS, 2026)](https://www.mas.gov.sg/publications/monographs-or-information-paper/2026/safeguards-for-agentic-finance-at-runtime) - Framework of runtime safeguards for agentic AI in finance, governing agents while they act rather than only at approval.
- [MAS partners industry to develop an AI Risk Management Toolkit for the financial sector (MAS, 2026)](https://www.mas.gov.sg/news/media-releases/2026/mas-partners-industry-to-develop-ai-risk-management-toolkit-for-the-financial-sector) - The MindForge-consortium toolkit providing practical implementation resources aligned with the AIRG.
- [Consultation Paper on Proposed Guidelines on Third-Party Risk Management (MAS, 2026)](https://www.mas.gov.sg/-/media/mas-media-library/publications/consultations/bd/2026/consultation-paper---tprmg.pdf) - Extends oversight to all third-party arrangements, including a register, concentration-risk monitoring, and sub-contractor oversight; it does not address AI specifically but applies to third-party AI providers.

### United States

- [Regulatory Notice 24-09: Generative AI and LLMs (FINRA, 2024)](https://www.finra.org/rules-guidance/notices/24-09) - Reminds broker-dealers that FINRA rules and securities laws apply to AI, including generative AI and large language models, as to any other technology.
- [Artificial Intelligence key topic page (FINRA)](https://www.finra.org/rules-guidance/key-topics/artificial-intelligence) - FINRA's consolidated hub of AI guidance, regulatory notices and oversight-report findings for member firms.
- [Responsible AI in Financial Markets (CFTC Technology Advisory Committee, 2024)](https://www.cftc.gov/media/10626/TAC_AIReport050224/download) - TAC subcommittee report with recommendations on responsible AI governance in CFTC-regulated derivatives markets.
- [Artificial Intelligence in Financial Services (US Treasury, 2024)](https://home.treasury.gov/news/press-releases/jy2760) - Treasury's December 2024 report synthesising its AI request for information, covering data, bias and third-party risks and recommending next steps for AI oversight in finance.
- [Managing AI-Specific Cybersecurity Risks in the Financial Services Sector (US Treasury, 2024)](https://home.treasury.gov/system/files/136/Managing-Artificial-Intelligence-Specific-Cybersecurity-Risks-In-The-Financial-Services-Sector.pdf) - March 2024 report on AI-related cyber and fraud risks and risk-management practices for financial firms.
- [Consumer Financial Protection Circular 2022-03: Adverse Action and Complex Algorithms (CFPB, 2022)](https://www.consumerfinance.gov/compliance/circulars/circular-2022-03-adverse-action-notification-requirements-in-connection-with-credit-decisions-based-on-complex-algorithms/) - Confirms ECOA / Regulation B adverse-action notice duties apply even when black-box AI/ML models make specific reasons hard to identify.
- [Interagency Request for Information on Financial Institutions' Use of AI (Federal Reserve, OCC, FDIC, CFPB, NCUA, 2021)](https://www.federalregister.gov/documents/2021/03/31/2021-06607/request-for-information-and-comment-on-financial-institutions-use-of-artificial-intelligence) - An early US interagency request for views on how financial institutions use AI and the appropriate governance, risk management and controls.
- [SEC proposes conflicts-of-interest rules on predictive data analytics by broker-dealers and investment advisers (SEC, 2023)](https://www.sec.gov/newsroom/press-releases/2023-140) - Proposed rules requiring firms to eliminate or neutralise conflicts from AI and predictive analytics in investor interactions (later withdrawn in 2025).
- [SEC charges two investment advisers over false and misleading AI claims (SEC, 2024)](https://www.sec.gov/newsroom/press-releases/2024-36) - Settled AI-washing enforcement actions against advisers that misrepresented their use of artificial intelligence.

### United Kingdom

- [DP5/22: Artificial Intelligence and Machine Learning (Bank of England / PRA / FCA, 2022)](https://www.bankofengland.co.uk/prudential-regulation/publication/2022/october/artificial-intelligence) - Joint discussion paper on AI/ML risks and whether a technology-neutral, outcomes-based supervisory approach suffices.
- [FS2/23: Feedback Statement on AI and Machine Learning (Bank of England / FCA, 2023)](https://www.bankofengland.co.uk/prudential-regulation/publication/2023/october/artificial-intelligence-and-machine-learning) - Summary of responses to DP5/22 on definitions, governance, accountability and model risk management for AI.
- [Artificial intelligence in UK financial services 2024 (Bank of England / FCA, 2024)](https://www.bankofengland.co.uk/report/2024/artificial-intelligence-in-uk-financial-services-2024) - The third joint survey measuring AI adoption, use cases and risk perceptions across UK financial firms.
- [Financial Stability in Focus: AI in the Financial System (Bank of England, 2025)](https://www.bankofengland.co.uk/financial-stability-in-focus/2025/april-2025) - Financial Policy Committee assessment of AI's systemic risks, including model risk, concentration and market correlation.

### European Union and member states

- [Special topic: Artificial Intelligence (European Banking Authority, 2024)](https://www.eba.europa.eu/publications-and-media/publications/special-topic-artificial-intelligence) - The AI section of the EBA's November 2024 Risk Assessment Report, covering banks' adoption of AI and generative AI and the associated risks.
- [Public Statement on AI and Investment Services (ESMA, 2024)](https://www.esma.europa.eu/press-news/esma-news/esma-provides-guidance-firms-using-artificial-intelligence-investment-services) - Guidance that firms using AI with retail clients must still meet MiFID II organisational, conduct and best-interest obligations.
- [The Rise of Artificial Intelligence: Benefits and Risks for Financial Stability (ECB, 2024)](https://www.ecb.europa.eu/press/financial-stability-publications/fsr/special/html/ecb.fsrart202405_02~58c3ce5246.en.html) - ECB Financial Stability Review feature on AI's operational, concentration and herding implications for the euro-area financial system.
- [Follow-up Report on the Use of Machine Learning for IRB Models (EBA, 2023)](https://www.eba.europa.eu/publications-and-media/press-releases/eba-publishes-follow-report-use-machine-learning-internal) - Principle-based recommendations for the prudent use of machine learning in regulatory credit-risk (IRB) models, including interactions with the GDPR and the EU AI Act.
- [Machine Learning in Risk Models: Characteristics and Supervisory Priorities (BaFin and Deutsche Bundesbank, 2021)](https://www.bundesbank.de/en/tasks/financial-supervision/individual-aspects/risk-management/machine-learning-methods/machine-learning-methods-623122) - Joint German consultation proposing a technology-neutral, characteristics-based supervisory approach to machine learning in banks' and insurers' risk models.
- [Governance of Artificial Intelligence in Finance (ACPR, Banque de France, 2020)](https://acpr.banque-france.fr/system/files/import/acpr/medias/documents/20200612_ai_governance_finance.pdf) - Sets four evaluation criteria (data management, performance, stability, explainability) and governance expectations for AI used by French financial institutions.
- [General Principles for the Use of Artificial Intelligence in the Financial Sector (DNB, 2019)](https://www.dnb.nl/media/voffsric/general-principles-for-the-use-of-artificial-intelligence-in-the-financial-sector.pdf) - The Dutch central bank's SAFEST principles (soundness, accountability, fairness, ethics, skills, transparency) for responsible AI in finance.
- [Financial consumer protection and market conduct considerations of AI in finance (Central Bank of Ireland, 2024)](https://www.centralbank.ie/news/article/speech-colm-kincaid-financial-consumer-protection-and-market-conduct-considerations-of-AI-in-finance-22-may-2024) - Supervisory address outlining the Central Bank's consumer-protection and conduct considerations for firms' use of AI.
- [Second thematic review on the use of Artificial Intelligence in the Luxembourg financial sector (CSSF and Banque centrale du Luxembourg, 2025)](https://www.cssf.lu/en/2025/05/second-thematic-review-on-the-use-of-artificial-intelligence-in-the-luxembourg-financial-sector/) - Survey of AI and generative-AI adoption across 461 institutions, covering bias, explainability, auditability, human oversight and EU AI Act risk classification.
- [Artificial intelligence in credit scoring: an analysis of some experiences in the Italian financial system (Banca d'Italia, 2022)](https://www.bancaditalia.it/pubblicazioni/qef/2022-0721/index.html) - Occasional Paper No. 721 on how Italian intermediaries use AI/ML for creditworthiness assessment and their awareness of the attendant model risks.
- [Accuracy of explanations of machine learning models for credit decisions (Banco de España, 2022)](https://www.bde.es/f/webbde/SES/Secciones/Publicaciones/PublicacionesSeriadas/DocumentosTrabajo/22/Files/dt2222e.pdf) - Working Paper No. 2222 proposing a synthetic-data framework to test the fidelity of interpretability techniques (SHAP, permutation importance) for ML credit models.

### Canada (OSFI)

- [OSFI-FCAC Risk Report: AI Uses and Risks at Federally Regulated Financial Institutions (OSFI / FCAC, 2024)](https://www.osfi-bsif.gc.ca/en/about-osfi/reports-publications/osfi-fcac-risk-report-ai-uses-risks-federally-regulated-financial-institutions) - Joint report on AI adoption trends and the prudential and consumer risks at Canadian federally regulated institutions.
- [Best Practices for the Responsible Use of AI in the Financial Sector (AMF Quebec, 2024)](https://lautorite.qc.ca/fileadmin/lautorite/grand_public/publications/professionnels/tous-les-pros/IssuesDiscussion_PaperAI_2024.pdf) - Quebec regulator's consultation proposing 30 best practices across consumer protection, transparency, responsibility and AI risk management.
- [AI in Capital Markets: Exploring Use Cases in Ontario (OSC, 2023)](https://www.osc.ca/en/industry/artificial-intelligence/ai-capital-markets-exploring-use-cases-ontario) - Maps current AI use cases, benefits and risks across Ontario's capital markets and the governance challenges they raise.
- [Financial Industry Forum on AI: A Canadian Perspective on Responsible AI (OSFI and Global Risk Institute, 2023)](https://globalriskinstitute.org/mp-files/financial-industry-forum-on-artificial-intelligence-a-canadian-perspective-on-responsible-ai.pdf) - Joint report setting out explainability, data, governance, and ethics principles for responsible AI in Canadian finance.

### Switzerland

- [Guidance on Governance and Risk Management when Using Artificial Intelligence (FINMA, 2024)](https://www.finma.ch/en/news/2024/12/20241218-mm-finma-am-08-24/) - The Swiss supervisor's guidance on the operational, data, IT, cyber, legal, and reputational risks of AI, drawn from its ongoing supervision.

### Asia-Pacific and other

- [High-level Principles on Artificial Intelligence (HKMA, 2019)](https://brdr.hkma.gov.hk/eng/doc-ldg/docId/getPdf/20191101-1-EN/20191101-1-EN.pdf) - HKMA circular setting guiding principles for authorised institutions on governance, model risk, fairness, transparency and accountability in AI use.
- [Consumer Protection in respect of Use of Generative AI (HKMA, 2024)](https://brdr.hkma.gov.hk/eng/doc-ldg/docId/20241107-1-EN) - Circular with guiding principles for banks' customer-facing generative AI, addressing governance, fairness, human oversight, transparency, hallucination and data privacy.
- [Circular to Licensed Corporations: Use of Generative AI Language Models (SFC, 2024)](https://apps.sfc.hk/edistributionWeb/gateway/EN/circular/doc?refNo=24EC55) - Four core principles (senior management, model risk management, cybersecurity and data, third-party risk) for licensed firms using generative AI, with extra controls for high-risk uses.
- [Reshaping Banking with Artificial Intelligence (HKMA, 2019)](https://www.hkma.gov.hk/media/eng/doc/key-functions/financial-infrastructure/Whitepaper_on_AI.pdf) - White paper mapping AI use cases, enabling technologies and risk-management considerations for banks adopting AI.
- [Letter to Industry on Artificial Intelligence (APRA, 2026)](https://www.apra.gov.au/news-and-publications/apra-letter-industry-artificial-intelligence-ai) - Observations and prudential expectations from APRA's review of large Australian banks, insurers and superannuation trustees on AI governance, risk management and operational resilience.
- [Preliminary Discussion Points for the Sound Utilisation of AI in the Financial Sector (Japan FSA, 2025)](https://www.fsa.go.jp/en/news/2025/20250304/aidp.html) - Discussion paper on principles and challenges for responsible AI, including generative AI, in finance.
- [FREE-AI Committee Report: Framework for Responsible and Ethical Enablement of AI in the Financial Sector (RBI, 2025)](https://rbi.org.in/Scripts/PublicationReportDetails.aspx?ID=1306&UrlPage=) - Reserve Bank of India expert-committee report setting seven guiding principles and 26 recommendations across six pillars for responsible AI adoption by regulated financial entities.
- [REP 798 Beware the gap: Governance arrangements in the face of AI innovation (ASIC, 2024)](https://www.asic.gov.au/regulatory-resources/find-a-document/reports/rep-798-beware-the-gap-governance-arrangements-in-the-face-of-ai-innovation) - ASIC review of how 23 Australian licensees use AI, finding governance and risk frameworks lagging adoption.
- [Financial Stability Review September 2024, Focus Topic: Financial Stability Implications of AI (RBA, 2024)](https://www.rba.gov.au/publications/fsr/2024/sep/focus-topic-financial-stability-implications-of-artificial-intelligence.html) - Reserve Bank of Australia analysis of how AI adoption could amplify systemic risks through provider concentration, herd behaviour, cyber threats and model and governance weaknesses.
- [Discussion Paper on Artificial Intelligence in the Malaysian Financial Sector (Bank Negara Malaysia, 2025)](https://www.bnm.gov.my/-/dp-aifs25) - Bank Negara Malaysia consultation on its proposed regulatory and development approach to responsible AI adoption by banks, insurers, takaful operators and payment institutions.
- [Policy Guideline on Risk Management of the Use of Artificial Intelligence Systems (Bank of Thailand, 2025)](https://www.bot.or.th/content/dam/bot/fipcs/documents/FOG/2568/ThaiPDF/25680178.pdf) - Bank of Thailand guideline requiring financial service providers to govern AI across its lifecycle under FEAT principles, covering data, model and cyber-risk controls including generative AI (Thai-language).
- [Revised AI Guidelines in the Financial Sector (FSC Korea, 2026)](https://www.fsc.go.kr/eng/pr010101/87140) - Financial Services Commission guidelines setting seven principles (governance, legitimacy, means of assistance, credibility, financial stability, good faith, security) for AI use by financial companies.
- [Guidance Note on the Consumer Protection and Responsible Adoption and Use of AI and ML by Licensed Financial Institutions (Central Bank of the UAE, 2026)](https://rulebook.centralbank.ae/en/rulebook/guidance-note-consumer-protection-and-responsible-adoption-and-use-artificial-intelligence) - Principles-based guidance on governance, fairness, transparency, data, monitoring and human oversight for AI/ML affecting consumers.
- [DFSA SEO Letters, including the 2026 Dear SEO letter on AI risk management in the DIFC (DFSA, 2026)](https://www.dfsa.ae/your-resources/publications-reports/seo-letters-1) - The DFSA's letters page, where the AI letter maps existing Rulebook requirements (governance, risk, operational risk, outsourcing, cyber) to firms' use of AI.

## International bodies and standards

Cross-border financial bodies and the horizontal standards that finance firms map onto.

### Global financial standard-setters and cross-border bodies

- [The Financial Stability Implications of Artificial Intelligence (FSB, 2024)](https://www.fsb.org/2024/11/the-financial-stability-implications-of-artificial-intelligence/) - FSB stocktake identifying systemic AI vulnerabilities in finance: third-party concentration, market correlations, cyber risk, and model risk and governance.
- [Monitoring Adoption of AI and Related Vulnerabilities in the Financial Sector (FSB, 2025)](https://www.fsb.org/2025/10/monitoring-adoption-of-artificial-intelligence-and-related-vulnerabilities-in-the-financial-sector/) - Follow-up giving authorities direct and proxy indicators to monitor AI adoption, with a case study on AI supply-chain concentration risk.
- [Artificial Intelligence and Machine Learning in Financial Services (FSB, 2017)](https://www.fsb.org/2017/11/artificial-intelligence-and-machine-learning-in-financial-service/) - An early FSB report on the financial-stability implications of AI/ML, including interconnectedness, third-party dependencies and model interpretability.
- [Sound Practices for Responsible Adoption of AI (FSB, 2026, consultation)](https://www.fsb.org/2026/06/sound-practices-for-responsible-adoption-of-artificial-intelligence-ai-consultation-report/) - Distils sound practices for financial institutions across governance, risk frameworks, materiality, model selection, data, explainability, oversight, cyber, and third-party risk; reads as a common skeleton for an AI risk programme.
- [The Use of AI and Machine Learning by Market Intermediaries and Asset Managers (IOSCO, 2021)](https://www.iosco.org/library/pubdocs/pdf/IOSCOPD684.pdf) - Final report setting six measures on governance, testing, data quality and bias, and transparency for AI/ML in securities markets.
- [Artificial Intelligence in Capital Markets: Use Cases, Risks, and Challenges (IOSCO, 2025)](https://www.iosco.org/library/pubdocs/pdf/IOSCOPD788.pdf) - Consultation report updating IOSCO's view on AI and generative-AI risks to investor protection, market integrity and financial stability.
- [Supervisory Toolkit for AI Use in Capital Markets (IOSCO, FR/02/2026)](https://www.iosco.org/library/pubdocs/pdf/IOSCOPD823.pdf) - The operational follow-up to IOSCO's capital-markets report: supervisory approaches, tools, and indicators for overseeing AI use in securities markets.
- [Application Paper on the Supervision of Artificial Intelligence (IAIS, 2025)](https://www.iais.org/2025/07/the-iais-publishes-application-paper-on-the-supervision-of-artificial-intelligence/) - The global insurance supervisors' guidance applying the Insurance Core Principles to AI across governance, robustness, transparency and fairness.
- [Regulating AI in the Financial Sector: Recent Developments and Main Challenges (BIS FSI Insights No. 63, 2024)](https://www.bis.org/fsi/publ/insights63.htm) - Financial Stability Institute survey of how financial authorities are and are not regulating AI, flagging model risk, data governance and third-party gaps.
- [Project Gaia: Enabling Climate Risk Analysis Using Generative AI (BIS Innovation Hub, 2024)](https://www.bis.org/publ/othp84.htm) - Proof-of-concept showing how supervisors can use large language models for data extraction, documenting controls for hallucination and non-repeatability.
- [Digitalisation of Finance (Basel Committee on Banking Supervision, 2024)](https://www.bis.org/bcbs/publ/d575.htm) - BCBS report assessing AI/ML and other technologies across the banking value chain and their implications for banks and supervisors.
- [Generative Artificial Intelligence and Cyber Security in Central Banking (BIS Papers No 145, 2024)](https://www.bis.org/publ/bppdf/bispap145.htm) - BIS survey of cyber-security experts at major central banks on how generative AI both strengthens and threatens their cyber security.
- [Global Financial Stability Report, Chapter 3: Advances in AI (IMF, 2024)](https://www.elibrary.imf.org/display/book/9798400277573/CH003.xml) - IMF assessment of how AI and generative AI affect trading, market liquidity and financial stability in capital markets.
- [Generative Artificial Intelligence in Finance: Risk Considerations (IMF Fintech Note 2023/006, 2023)](https://www.imf.org/en/Publications/fintech-notes/Issues/2023/08/18/Generative-Artificial-Intelligence-in-Finance-Risk-Considerations-537570) - IMF note on the distinct risks generative AI adds to the financial sector beyond earlier AI/ML.
- [Powering the Digital Economy: Opportunities and Risks of Artificial Intelligence in Finance (IMF, 2021)](https://www.imf.org/en/Publications/Departmental-Papers-Policy-Papers/Issues/2021/10/21/Powering-the-Digital-Economy-Opportunities-and-Risks-of-Artificial-Intelligence-in-Finance-494717) - Departmental paper categorising the risks AI/ML pose to financial integrity and stability and outlining regulatory approaches.
- [Generative Artificial Intelligence in Finance (OECD, 2023)](https://www.oecd.org/en/publications/generative-artificial-intelligence-in-finance_ac7149cc-en.html) - OECD analysis of generative-AI use cases, benefits and policy and risk considerations across financial services.
- [Artificial Intelligence, Machine Learning and Big Data in Finance (OECD, 2021)](https://www.oecd.org/en/publications/artificial-intelligence-machine-learning-and-big-data-in-finance_98e761e7-en.html) - Assesses the benefits and risks of AI in finance and policy responses on explainability, data governance and financial stability.
- [Regulatory Approaches to Artificial Intelligence in Finance (OECD, 2024)](https://www.oecd.org/en/publications/regulatory-approaches-to-artificial-intelligence-in-finance_f1498c02-en.html) - Cross-jurisdictional analysis of how financial regulators are approaching AI.
- [OECD AI Principles (OECD, 2019, updated 2024)](https://oecd.ai/en/ai-principles) - The five influential cross-sector values for trustworthy AI, updated for the generative-AI era.
- [Governing AI for Humanity (UN AI Advisory Body, 2024)](https://www.un.org/sites/un2.un.org/files/governing_ai_for_humanity_final_report_en.pdf) - The UN high-level body's seven recommendations for global AI governance, including a scientific panel, standards exchange, and capacity development.
- [The AI supply chain (BIS Paper 154, 2025)](https://www.bis.org/publ/bppdf/bispap154.htm) - Maps the five-layer AI supply chain and its concentration, operational-resilience, cyber-security and financial-stability implications.
- [The use of artificial intelligence for policy purposes (BIS, 2025)](https://www.bis.org/publ/othp100.htm) - Report to the G20 on how central banks, regulators and supervisors use AI, covering data governance, human capital and infrastructure challenges.
- [In data we trust? Emerging policy and supervisory approaches to AI data use in financial services (BIS FSI Insights 73, 2026)](https://www.bis.org/fsi/publ/insights73.htm) - Examines data privacy, quality, security and third-party concentration risks in financial firms' AI use and the supervisory expectations addressing them.
- [Peering through the hype: assessing suptech tools' transition from experimentation to supervision (BIS FSI Insights 58, 2024)](https://www.bis.org/fsi/publ/insights58.htm) - Analyses authorities' deployment of suptech tools, including AI, generative AI and machine learning, in financial supervision.
- [Project Aurora: the power of data, technology and collaboration to combat money laundering across institutions and borders (BIS Innovation Hub, 2023)](https://www.bis.org/publications/project-aurora-power-data-technology-and-collaboration-combat-money-laundering-across-institutions-and-borders) - Proof of concept applying machine learning, network analysis and privacy-enhancing technologies to anti-money-laundering, with implications for AML model governance.
- [Project Raven: using AI to assess the financial system's cyber security and resilience (BIS Innovation Hub, 2024)](https://www.bis.org/about/bisih/topics/cyber_security/raven.htm) - Project building an AI tool for authorities to assess the cyber-security and resilience maturity of financial systems.
- [Newsletter on artificial intelligence and machine learning (BCBS, 2022)](https://www.bis.org/publ/bcbs_nl27.htm) - Basel Committee statement on banks' use of AI/ML and the related explainability, governance, model-risk and resilience challenges for supervisors.
- [AI Projects in Financial Supervisory Authorities: A Toolkit for Successful Implementation (IMF Working Paper WP/25/199, 2025)](https://www.imf.org/-/media/files/publications/wp/2025/english/wpiea2025199-source-pdf.pdf) - Proposes a project-management methodology for supervisory authorities to adopt AI while managing explainability, data and governance risks.
- [Artificial Intelligence for Financial Sector Supervision: An Emerging Market and Developing Economies Perspective (World Bank, 2025)](https://documents.worldbank.org/en/publication/documents-reports/documentdetail/099110525115015626) - Reviews AI adoption by emerging-market and developing-economy financial-sector supervisors and the practical issues, challenges and risks they face.
- [Supervision of artificial intelligence in finance: Challenges, policies and practices (OECD, 2026)](https://www.oecd.org/en/publications/supervision-of-artificial-intelligence-in-finance_92743dc1-en.html) - Analyses supervisory approaches to AI in finance that balance responsible adoption with stability, integrity and consumer protection.
- [Artificial intelligence in Asia's financial sector: A review of country policies (OECD, 2025)](https://www.oecd.org/en/publications/artificial-intelligence-in-asia-s-financial-sector_3385bbd8-en.html) - Compares AI-in-finance policy frameworks across 15 Asian jurisdictions and the vulnerabilities and novel risks AI can introduce.

### Horizontal standards and frameworks that can be applied to finance

- [AI Risk Management Framework (AI RMF 1.0) (NIST, 2023)](https://www.nist.gov/itl/ai-risk-management-framework) - Voluntary US framework (Govern, Map, Measure, Manage) widely used by financial firms and referenced by regulators to structure AI risk programmes.
- [AI RMF Generative AI Profile (NIST-AI-600-1) (NIST, 2024)](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-generative-artificial-intelligence) - Companion profile mapping generative-AI-specific risks and suggested actions onto the AI RMF, relevant to financial generative-AI deployments.
- [ISO/IEC 42001:2023, AI Management System (ISO/IEC, 2023)](https://www.iso.org/standard/81230.html) - The first certifiable AI management system standard, giving firms an auditable basis for AI governance.
- [ISO/IEC 23894:2023, AI Guidance on Risk Management (ISO/IEC, 2023)](https://www.iso.org/standard/77304.html) - AI-specific adaptation of ISO 31000 risk-management processes for organisations developing or using AI.
- [ISO/IEC 42005:2025, AI System Impact Assessment (ISO/IEC, 2025)](https://www.iso.org/standard/44545.html) - Guidance for documenting AI system impacts on individuals and society, supporting assessments increasingly expected by regulators.
- [ISO/IEC 5338:2023, AI System Life Cycle Processes (ISO/IEC, 2023)](https://www.iso.org/standard/81118.html) - Defines lifecycle processes for AI systems, useful for structuring model development and validation controls.
- [ISO/IEC TR 24028:2020, Overview of Trustworthiness in AI (ISO/IEC, 2020)](https://www.iso.org/standard/77608.html) - Technical report surveying transparency, explainability, controllability and related trustworthiness concepts underpinning AI risk work.

### Horizontal laws and conventions

- [Regulation (EU) 2024/1689, the Artificial Intelligence Act (European Union, 2024)](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng) - The official published text of the EU AI Act, whose high-risk and generative-AI obligations reach financial use cases such as creditworthiness assessment.
- [Regulatory framework for AI (European Commission, 2024)](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) - The Commission's official portal explaining the Act's risk tiers and obligations.
- [Framework Convention on Artificial Intelligence (Council of Europe, 2024)](https://www.coe.int/en/web/artificial-intelligence/the-framework-convention-on-artificial-intelligence) - The first legally binding international AI treaty, anchoring AI to human rights, democracy and the rule of law.

## Industry and consortium frameworks

Frameworks and toolkits from industry consortia and professional bodies, built for financial services.

### Consortium and industry-body frameworks

- [CRI Financial Services AI Risk Management Framework (Cyber Risk Institute, 2026)](https://cyberriskinstitute.org/artificial-intelligence-risk-management/) - Industry-led, sector-specific framework aligned to the NIST AI RMF, with 230 control objectives mapped to AI adoption stages, developed with over 100 financial institutions; includes a downloadable Risk and Control Matrix, Guidebook, and Control Objective Reference Guide.
- [CRI Profile v2.2 (Cyber Risk Institute, 2025)](https://cyberriskinstitute.org/cri-profile-overview/) - The financial-sector cyber and technology risk framework (built on the NIST CSF) that the CRI Financial Services AI Risk Management Framework sits alongside, harmonising 3,500+ regulatory expectations into 318 diagnostic statements.
- [FINOS AI Governance Framework (Fintech Open Source Foundation / Linux Foundation, 2025)](https://air-governance-framework.finos.org/) - Open-source, vendor-neutral catalogue of AI risks and mitigations for financial institutions; v2.0 adds agentic-AI risks.
- [FINOS AI Governance Framework, source repository (Fintech Open Source Foundation, 2024)](https://github.com/finos/ai-governance-framework) - The open GitHub project where the framework and its Financial Services AI Readiness reference model are developed by member firms, academics, and practitioners.
- [Veritas Initiative and FEAT assessment methodology (MAS-led consortium, 2022)](https://www.mas.gov.sg/schemes-and-initiatives/veritas) - MAS-co-created Fairness, Ethics, Accountability and Transparency (FEAT) principles with downloadable assessment-methodology documents for banking and insurance AI use cases.
- [Veritas Diagnosis Toolkit (MAS-led consortium, 2023)](https://github.com/mas-veritas2/veritastool) - Open-source Python toolkit implementing the Veritas FEAT fairness and transparency assessment methodology for financial-sector AI.
- [Veritas Document 3 - FEAT Principles Assessment Methodology (MAS, 2022)](https://www.mas.gov.sg/-/media/mas-media-library/news/media-releases/2022/veritas-document-3---feat-principles-assessment-methodology.pdf) - Consolidated MAS Veritas whitepaper translating the FEAT principles into an assessment methodology for financial-sector AI and data-analytics systems.
- [Veritas Document 3A - FEAT Fairness Principles Assessment Methodology (MAS, 2022)](https://www.mas.gov.sg/-/media/mas-media-library/news/media-releases/2022/veritas-document-3a---feat-fairness-principles-assessment-methodology.pdf) - Methodology for defining fairness objectives and detecting unintentional bias in financial-sector AI, with credit-scoring and insurance-underwriting examples.
- [Veritas Document 3B - FEAT Ethics and Accountability Principles Assessment Methodology (MAS, 2022)](https://www.mas.gov.sg/-/media/mas-media-library/news/media-releases/2022/veritas-document-3b---feat-ethics-and-accountability-principles-assessment-methodology.pdf) - Methodology for quantifiable measurement of ethical practice and internal and external accountability in financial-institution AI.
- [Veritas Document 3C - FEAT Transparency Principles Assessment Methodology (MAS, 2022)](https://www.mas.gov.sg/-/media/mas-media-library/news/media-releases/2022/veritas-document-3c---feat-transparency-principles-assessment-methodology.pdf) - Methodology for determining how much internal and external transparency is needed to explain and interpret ML predictions in finance.
- [GFMA Artificial Intelligence / Machine Learning hub (Global Financial Markets Association)](https://www.gfma.org/global-market-policies/opportunities-risks-from-new-technology/artificial-intelligence-machine-learning/) - GFMA's collection of AI-in-capital-markets reports and policy positions on responsible AI adoption.
- [SIFMA AI white paper: Promoting Investor Success, Industry Innovation, and Efficiency with AI (SIFMA, 2024)](https://www.sifma.org/research/white-papers/ai-white-paper-promoting-investor-success-industry-innovation-and-efficiency) - Industry-association white paper outlining a risk-based approach to AI use and oversight across the securities industry.

### Professional-body certifications and training

- [GARP Risk and AI (RAI) Certificate (Global Association of Risk Professionals, 2024)](https://www.garp.org/rai) - Professional certificate covering AI/ML tools, AI risks and risk factors, responsible AI, and governance frameworks, aimed at risk practitioners.
- [PRMIA AI Risk Management Certificate (Professional Risk Managers' International Association, 2026)](https://prmia.org/Public/Public/Certificate/AI.aspx) - Practitioner-focused certificate on understanding and governing AI risk, with self-study materials.

### Trade-association and survey research

- [GenAI in the Derivatives Market: A Future Perspective (ISDA Future Leaders in Derivatives, 2024)](https://www.isda.org/2024/04/17/genai-in-the-derivatives-market-a-future-perspective/) - ISDA whitepaper on generative-AI opportunities, risks, and governance considerations for derivatives-market stakeholders.
- [IIF-EY Global Annual Survey Report on AI Use in Financial Services (Institute of International Finance and EY, 2026)](https://www.iif.com/Publications/ID/6722/2026-IIF-EY-Global-Annual-Survey-Report-on-AI-Use-in-Financial-Services) - Long-running annual survey of AI/ML development, governance, third-party model use, and regulation across financial institutions.
- [Artificial Intelligence: Challenges and Opportunities for Compliance (AFME and PwC, 2023)](https://www.afme.eu/publications/reports/artificial-intelligence-challenges-and-opportunities-for-compliance/) - Examines how AI reshapes the compliance function and how compliance teams can oversee AI use across the firm.
- [Benchmarking Generative AI for CSA Clause Extraction and CDM Representation (ISDA, 2025)](https://www.isda.org/2025/05/15/benchmarking-generative-ai-for-csa-clause-extraction-and-cdm-representation/) - Whitepaper testing the accuracy and reliability of generative AI for digitising derivatives legal clauses, addressing model-reliability risk in documentation workflows.
- [Machine Learning Governance Summary Report (IIF, 2020)](https://www.iif.com/Publications/ID/4198/Machine-Learning-Governance-Summary-Report-) - Public summary of a global survey on end-to-end governance of the machine-learning lifecycle in financial institutions.
- [Common Controls for AI Services (FINOS, 2025)](https://www.finos.org/common-cloud-controls-project) - Open, technology-neutral baseline controls for AI usage across cloud and hybrid environments, extending FINOS Common Cloud Controls and aligned to the FINOS AI Governance Framework.
- [AI and Open Source in Financial Services (The Linux Foundation and FINOS, 2026)](https://www.linuxfoundation.org/research/ai-open-source-financial-services) - Research report on deploying AI in production in financial services, covering machine-scale cyber risk, governance of agentic workflows and token-consumption controls.
- [AI in financial services (The Alan Turing Institute, 2021)](https://www.turing.ac.uk/news/publications/ai-financial-services) - FCA-commissioned report on responsible AI in finance, mapping benefits and harms and the role of transparency in responsible innovation.
- [The AI Playbook for Financial Services (World Economic Forum, 2026)](https://reports.weforum.org/docs/WEF_The_AI_Playbook_for_Financial_Services_2026.pdf) - Practical guidance on AI strategy, governance, model risk, security and agentic systems for firms scaling AI.
- [2026 Global AI in Financial Services Report (Cambridge Centre for Alternative Finance, 2026)](https://www.jbs.cam.ac.uk/faculty-research/centres/alternative-finance/publications/2026-global-ai-in-financial-services-report/) - Global survey (with the WEF, BIS, IMF and others) of more than 600 institutions, regulators and vendors across 151 countries on AI adoption, impact and emerging risks.
- [AI Risks and Opportunities: Adopting an AGILE Framework in Canadian Financial Services (Global Risk Institute, 2026)](https://globalriskinstitute.org/publication/fifai-ii-ai-risks-and-opportunities/) - Financial Industry Forum on AI Phase II report proposing an AGILE framework for AI governance and oversight.
- [Artificial Intelligence Regulatory Developments Tracker (ICMA, ongoing)](https://www.icmagroup.org/fintech-and-digitalisation/fintech-advisory-committee-and-related-groups/artificial-intelligence-regulatory-developments-tracker) - ICMA-maintained tracker of global AI regulatory and policy developments relevant to capital markets.

### Professional-services frameworks

- [Deloitte Trustworthy AI framework (Deloitte)](https://www.deloitte.com/us/en/what-we-do/capabilities/applied-artificial-intelligence/services/ethics-of-ai-framework.html) - Advisory firm's responsible-AI framework spanning transparency, accountability, fairness, privacy, safety, and robustness across the AI lifecycle; firm-branded, with financial-services applications.
- [KPMG Trusted AI framework (KPMG, 2026)](https://kpmg.com/xx/en/what-we-do/services/ai/trusted-ai-framework.html) - Advisory firm's framework for embedding governance across the AI and AI-agent lifecycle; firm-branded, with financial-services applications.

## Model risk management foundations

The supervisory and practitioner base that AI risk management in finance builds on, and how it extends to machine learning and generative AI.

### Supervisory foundations

- [SR 11-7 / OCC 2011-12: Supervisory Guidance on Model Risk Management (Federal Reserve / OCC, 2011)](https://elischolar.library.yale.edu/cgi/viewcontent.cgi?article=1576&context=ypfs-documents) - The original US supervisory guidance that defined model risk and the practice of "effective challenge", and set out model development, independent validation, and governance as the structure of model risk management; superseded by the 2026 interagency revision but still the reference point the discipline is built on (archived full text of the guidance, as the official pages were withdrawn).
- [SR 26-2 / OCC Bulletin 2026-13: Model Risk Management, Revised Guidance (Federal Reserve / OCC / FDIC, 2026)](https://www.occ.gov/news-issuances/bulletins/2026/bulletin-2026-13.html) - The April 2026 interagency revision that replaces the 2011 guidance with a more explicitly risk-based, tailored approach; it puts generative AI and agentic AI expressly out of scope, with a separate request for information on AI model risk planned.
- [SS1/23: Model risk management principles for banks (Bank of England / PRA, 2023)](https://www.bankofengland.co.uk/prudential-regulation/publication/2023/may/model-risk-management-principles-for-banks-ss) - Five MRM principles (identification and tiering, governance, development, independent validation, risk mitigants) applying to all model and risk types, including AI/ML; the May 2023 version took effect May 2024, with a minor clarifying amendment in April 2026.
- [Guideline E-23: Model Risk Management (OSFI, 2025, effective 2027)](https://www.osfi-bsif.gc.ca/en/guidance/guidance-library/guideline-e-23-model-risk-management-2027) - Principles-based, technology-neutral enterprise-wide MRM guideline for Canadian federally regulated institutions, written to cover the rise of AI/ML and self-learning models.
- [SR 15-18: Supervisory Assessment of Capital Planning and Positions (Federal Reserve, 2015, rev. 2021)](https://www.federalreserve.gov/supervisionreg/srletters/sr1518.htm) - Capital-planning guidance (with a companion, SR 15-19, for other large firms) whose model-risk and validation expectations extended SR 11-7 into the stress-testing context.
- [Guide for the Targeted Review of Internal Models (TRIM) (ECB Banking Supervision, 2017)](https://www.bankingsupervision.europa.eu/ecb/pub/pdf/trim_guide.en.pdf) - The ECB's detailed supervisory expectations for the development, validation and governance of banks' internal risk models, carried forward in its guide to internal models.
- [ECB Guide to internal models (European Central Bank, 2025)](https://www.bankingsupervision.europa.eu/ecb/pub/pdf/ssm.supervisory_guide202507.en.pdf) - The revised SSM supervisory guide (July 2025) with a new dedicated section on using machine-learning techniques in regulatory models; distinct from the 2019 TRIM guide.

### Extending MRM to AI, ML and generative AI

- [Derisking machine learning and artificial intelligence (McKinsey, 2019)](https://www.mckinsey.com/capabilities/risk-and-resilience/our-insights/derisking-machine-learning-and-artificial-intelligence) - Argues banks can manage ML model risk within an SR 11-7-consistent framework, modifying existing risk elements and adding new ones such as interpretability, bias and production readiness.
- [Managing the Risk of Machine Learning (Oliver Wyman, 2018)](https://www.oliverwyman.com/our-expertise/insights/2018/aug/managing-the-risk-of-machine-learning.html) - Practitioner view on the new failure modes of ML models and how validation, monitoring and governance need to adapt.
- [Managing Next Generation Artificial Intelligence in Banking (Oliver Wyman, 2017)](https://www.oliverwyman.com/our-expertise/insights/2017/dec/managing-next-generation-artificial-intelligence-in-banking.html) - Recommends designating AI as a distinct model type in model-risk policy and folding it into existing model-tiering and validation processes.
- [Model Risk Management for Generative AI in Financial Institutions (Bhattacharyya et al., 2025)](https://arxiv.org/abs/2503.15668) - Practitioner paper by bank model-risk authors on the additional validation and control practices generative AI needs, focusing on hallucination and toxicity risks.
- [Generative AI Risk Management in Financial Institutions (Alliance for Innovative Regulation and Google Cloud, 2024)](https://services.google.com/fh/files/misc/wp_generative_ai_risk_management_in_fs.pdf) - A publicly available framework mapping generative-AI risks to model-validation and ongoing-monitoring controls for regulated financial firms.
- [Modern Risk Management for AI Models (KPMG)](https://hub.kpmg.de/modern-risk-management-for-ai-models) - Whitepaper on re-imagining the MRM function for AI/ML models, including validation and governance adaptations.

### Validation practice

- [Adapting model validation in the age of AI (Deloitte, 2024)](https://www.deloitte.com/global/en/Industries/financial-services/perspectives/adapting-model-validation.html) - How independent model validation must change for AI and large language models, covering data volume, interpretability and new testing techniques.
- [Beyond Accuracy: Deloitte's Journey to Robust GenAI Model Validation (Deloitte UK)](https://www.deloitte.com/uk/en/services/consulting/analysis/beyond-accuracy-deloittes-journey-to-robust-genai-model-validation.html) - Draws on a global bank's generative-AI validation programme, extending validation to prompt injection and risks beyond raw model performance.
- [Journal of Risk Model Validation (Risk.net)](https://www.risk.net/journal-of-risk-model-validation) - Peer-reviewed journal dedicated to model-validation methods, backtesting and benchmarking, including recent work on generative AI in model risk management.

### Books and long-form

- [The Validation of Risk Models: A Handbook for Practitioners (Scandizzo, 2016)](https://link.springer.com/book/10.1057/9781137436962) - A practitioner handbook on the tools, techniques and processes of risk-model validation, by a head of model validation at the European Investment Bank.
- [Model Risk Management: Risk Bounds under Uncertainty (Rüschendorf, Vanduffel and Bernard, 2023)](https://www.cambridge.org/core/books/model-risk-management/20D77F4ED791C2339297777A70333533) - A systematic quantitative treatment of model uncertainty, deriving risk bounds that supervisors and institutions can use to challenge models.
- [Validation of Risk Management Models for Financial Institutions (Lynch, Hasan and Siddique, 2023)](https://www.cambridge.org/core/books/validation-of-risk-management-models-for-financial-institutions/643DA518B981853D142806EEA5E1E7AA) - An edited practitioner and academic volume of 17 contributions on validating market, credit, retail and operational risk models in banks.

## Tools and open source

Very little AI risk tooling is built for finance specifically; the main finance-native option, the open-source Veritas toolkit, sits under [Industry and consortium frameworks](#industry-and-consortium-frameworks). What follows is the general-purpose toolbox financial institutions actually use, grouped by the control each one serves:

- **Fairness and bias** tools run the fair-lending and underwriting testing behind ECOA and Regulation B in the US and the FEAT principles in Singapore.
- **Explainability** tools produce the adverse-action reasons credit decisions require, and feed independent model validation.
- **Validation, monitoring and drift** tools run the ongoing monitoring and validation that SR 11-7, SS1/23 and OSFI E-23 expect.
- **LLM and GenAI evaluation** and **AI security** tools cover generative-AI model risk and red-teaming.
- **Risk catalogues and databases** help populate an AI inventory and risk register.

Open source unless marked commercial. A few canonical references are flagged where no longer actively maintained.

### Fairness and bias

- [AI Fairness 360 / AIF360 (IBM / Trusted-AI)](https://github.com/Trusted-AI/AIF360) - Open-source library of bias metrics and mitigation algorithms for datasets and models, with Python and R support and documentation aimed at credit and lending fairness.
- [Fairlearn (Microsoft and community)](https://github.com/fairlearn/fairlearn) - Python toolkit to assess and mitigate allocation and quality-of-service harms, directly relevant to fair-lending and insurance underwriting decisions.
- [Aequitas (Center for Data Science and Public Policy, University of Chicago)](https://github.com/dssg/aequitas) - Bias auditing and fair-ML toolkit for binary classifiers with a disparity-report workflow, useful for documenting adverse-impact testing in credit scoring.

### Explainability

- [SHAP (Scott Lundberg and community)](https://github.com/shap/shap) - Game-theoretic Shapley-value method to attribute a model's output to its input features, widely used to generate adverse-action reasons and support model validation.
- [LIME (Marco Tulio Ribeiro)](https://github.com/marcotcr/lime) - Local interpretable model-agnostic explanations for individual predictions on tabular, text and image data; a standard for per-decision reason codes.
- [InterpretML (Microsoft)](https://github.com/interpretml/interpret) - Unified framework offering glassbox models (Explainable Boosting Machines) and blackbox explainers, valued where regulators expect inherently interpretable credit models.
- [Alibi (Seldon)](https://github.com/SeldonIO/alibi) - Library of explanation algorithms including counterfactuals and anchors, helpful for actionable recourse and adverse-action narratives.
- [Captum (Meta / PyTorch)](https://github.com/meta-pytorch/captum) - Model interpretability library for PyTorch (attributions, integrated gradients), relevant to validating deep-learning models in finance.
- [DALEX (ModelOriented)](https://github.com/ModelOriented/DALEX) - Model-agnostic explanation framework in R and Python emphasising model exploration and fairness checks, common in actuarial and credit-risk workflows.
- [Responsible AI Toolbox (Microsoft)](https://github.com/microsoft/responsible-ai-toolbox) - Dashboards and libraries combining error analysis, interpretability, fairness and counterfactuals for structured model assessment and governance documentation.
- [Amazon SageMaker Clarify (AWS, commercial)](https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-configure-processing-jobs.html) - Managed service for bias detection and feature-attribution explainability across the ML lifecycle; now limited availability and not open to new customers.
- [PiML (SelfExplainML)](https://github.com/SelfExplainML/PiML-Toolbox) - Open-source Python toolbox for interpretable machine learning and model diagnostics, used in model validation.
- [Modeva (SelfExplainML, commercial)](https://modeva.ai/) - Model validation and diagnostics toolkit aimed at interpretable and well-tested models.
- [AI Explainability 360 / AIX360 (IBM / Trusted-AI)](https://github.com/Trusted-AI/AIX360) - Open-source Python toolkit of model-explainability algorithms with credit-approval tutorials; the explainability counterpart to AIF360.

### Validation, monitoring and drift

- [Evidently AI (Evidently)](https://github.com/evidentlyai/evidently) - Open-source framework to evaluate, test and monitor ML and LLM systems with 100+ metrics for data and prediction drift, central to production model-risk monitoring.
- [Deepchecks (Deepchecks)](https://github.com/deepchecks/deepchecks) - Holistic testing library for data and model validation from research to production, supporting the continuous validation expected under model-risk frameworks.
- [whylogs (WhyLabs)](https://github.com/whylabs/whylogs) - Open-source data-logging library that produces statistical profiles for data-quality and drift tracking; WhyLabs offers a commercial observability platform on top.
- [NannyML (NannyML)](https://github.com/NannyML/nannyml) - Open-source library that estimates post-deployment model performance without labels and links drift to performance impact, addressing silent model degradation in production.
- [Giskard (Giskard-AI)](https://github.com/Giskard-AI/giskard-oss) - Open-source evaluation, testing and red-teaming library for LLM and agent systems, with an automated vulnerability scanner; its earlier tabular-ML scanning is now a legacy feature.
- [Great Expectations (GX / Fivetran)](https://github.com/fivetran/great_expectations) - Widely used data-validation framework that enforces expectations on pipelines, central to the data-quality controls underpinning model inputs.
- [Arize Phoenix (Arize AI)](https://github.com/Arize-ai/phoenix) - Open-source AI observability and evaluation platform (tracing, evals, drift), with a commercial Arize counterpart for managed production monitoring.
- [AI Verify (AI Verify Foundation / IMDA Singapore)](https://github.com/aiverify-foundation/aiverify) - Open-source AI governance testing framework running technical tests and process checks against internationally recognised AI principles.

### LLM and GenAI evaluation

- [DeepEval (Confident AI)](https://github.com/confident-ai/deepeval) - Open-source LLM evaluation framework with metrics for hallucination, relevancy and more in a unit-test style, useful for GenAI model-risk sign-off.
- [Ragas (Vibrant Labs)](https://github.com/vibrantlabsai/ragas) - Evaluation library focused on RAG pipelines (faithfulness, context precision and recall), relevant where finance GenAI must stay grounded in source documents.
- [promptfoo (promptfoo)](https://github.com/promptfoo/promptfoo) - Declarative CLI/CI tool for LLM evals and red-teaming across providers, enabling repeatable regression and vulnerability testing of GenAI features.
- [OpenAI Evals (OpenAI)](https://github.com/openai/evals) - Framework and open registry of benchmarks for evaluating LLMs and LLM systems, usable to build private domain-specific evals.
- [LangSmith SDK (LangChain)](https://github.com/langchain-ai/langsmith-sdk) - Open-source client SDK for the LangSmith platform (tracing, datasets, evaluation); the SDK is open, the hosted platform commercial.
- [TruLens (TruEra / Snowflake)](https://github.com/truera/trulens) - Open-source library to evaluate and track LLM apps and agents with feedback functions (groundedness, relevance, toxicity), supporting GenAI assurance.
- [Project Moonshot (AI Verify Foundation / IMDA Singapore)](https://github.com/aiverify-foundation/moonshot) - Open-source toolkit combining benchmarking and red-teaming to evaluate the safety and reliability of large language models and LLM applications.

### AI security and red-teaming

- [garak (NVIDIA)](https://github.com/NVIDIA/garak) - Open-source LLM vulnerability scanner probing for prompt injection, jailbreaks, data leakage and toxicity, analogous to a port scanner for language models.
- [PyRIT (Microsoft)](https://github.com/microsoft/PyRIT) - Python Risk Identification Tool, an open-source framework to proactively red-team and identify risks in generative-AI systems.
- [Adversarial Robustness Toolbox / ART (Trusted-AI, LF AI and Data)](https://github.com/Trusted-AI/adversarial-robustness-toolbox) - Python library for ML security covering evasion, poisoning, extraction and inference attacks and defences, relevant to adversarial testing of fraud and credit models.
- [OWASP Top 10 for LLM Applications / GenAI Security Project (OWASP)](https://github.com/GenAI-Security-Project/GenAI-LLM-Top10) - Community risk framework cataloguing the top GenAI application risks; a standard reference for GenAI threat modelling in finance.

### Risk catalogues and databases

- [MIT AI Risk Repository (MIT FutureTech)](https://airisk.mit.edu/risks) - Structured, regularly updated database of over 1,600 documented AI risks with a causal and domain taxonomy, usable as a starting catalogue for enterprise AI risk registers.
- [AI Incident Database (Responsible AI Collaborative)](https://incidentdatabase.ai/) - Searchable index of real-world AI harms and near-harms, a source of loss scenarios and precedent for operational-risk and model-risk analysis.
- [AI Vulnerability Database / AVID (AVID)](https://avidml.org/) - Open knowledge base of failure modes for general-purpose AI systems with reproducible evidence and a taxonomy library, supporting structured GenAI vulnerability tracking.
- [MITRE ATLAS (MITRE)](https://atlas.mitre.org/) - An ATT&CK-style knowledge base of real-world tactics and techniques against ML systems, useful for threat modelling AI in financial infrastructure.

## Research, reports, and reading

Reports, papers, books, courses, and people worth following.

### Reports and research

- [The Impact of AI on the Financial Sector and Supervision (DNB and AFM, 2024)](https://www.dnb.nl/en/sector-news/supervision-2024/afm-and-dnb-publish-report-on-the-impact-of-ai-on-the-financial-sector-and-supervision/) - Joint Dutch supervisory report on AI risks (explainability, data quality, bias, big-tech dependence) and the supervisory response.
- [Governance of AI Adoption in Central Banks (BIS Consultative Group on Risk Management, 2025)](https://www.bis.org/publ/othp90.htm) - Report proposing a three-lines-of-defence governance and risk-management framework for AI, transferable to financial supervisors.
- [Navigating Artificial Intelligence in Banking (Bank Policy Institute, 2024)](https://bpi.com/navigating-artificial-intelligence-in-banking/) - Industry white paper mapping existing bank risk frameworks (model risk, third-party, data) onto AI use cases.
- [AI and Financial Stability: Mitigating Risks, Harnessing Benefits (Brookings, 2024)](https://www.brookings.edu/articles/ai-and-financial-stability-mitigating-risks-harnessing-benefits/) - Summary of an FSOC-Brookings conference on AI's financial-stability implications.
- [Tail Risk for Banks Posed by Investments in Generative AI (Federal Reserve Bank of Chicago, 2026)](https://www.chicagofed.org/publications/chicago-fed-insights/2026/ai-tail-risk-for-banks) - Chicago Fed analysis of concentration and tail risks banks face from the generative-AI investment cycle.

### Academic and practitioner papers

- [Large Language Models in Finance: A Survey (Li et al., 2023)](https://arxiv.org/abs/2311.10723) - Survey of LLM solutions and adoption guidance for financial tasks, including associated risks.
- [A Survey of Large Language Models for Financial Applications (Nie et al., 2024)](https://arxiv.org/abs/2406.11903) - Broad review of financial LLM applications and the challenges they raise.
- [A Survey of Large Language Models in Finance / FinLLMs (Lee et al., 2024)](https://arxiv.org/abs/2402.02315) - Survey tracing the evolution of finance-specific LLMs, datasets, benchmarks and open challenges.
- [RiskLabs: Predicting Financial Risk Using Large Language Models (Cao et al., 2024)](https://arxiv.org/abs/2404.07452) - Research on applying LLMs with multimodal, multi-source data to financial risk prediction, and its limitations.
- [Explainability and Fairness in Machine Learning for Credit Underwriting (FinRegLab, 2023)](https://finreglab.org/research/explainability-and-fairness-in-machine-learning-for-credit-underwriting/) - Empirical and policy work with Stanford GSB assessing model-diagnostic tools for fairness and adverse-action explanations in lending.
- [Performance, Fairness, and Explainability in AI-Based Credit Scoring: A Systematic Literature Review (Journal of Risk and Financial Management, 2026)](https://www.mdpi.com/1911-8074/19/2/104) - Systematic review of 43 studies (2020-2025) synthesising the performance, fairness and explainability trade-offs in AI credit scoring.
- [Confronting Machine Learning With Financial Research (Lommers, El Harzli and Kim, 2021)](https://arxiv.org/abs/2103.00366) - Sets out the tension between machine-learning methodology and financial-economics research and the adjustments needed to avoid spurious inference.
- [The Probability of Backtest Overfitting (Bailey, Borwein, Lopez de Prado and Zhu, 2016)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2326253) - Formalises how repeated strategy selection inflates in-sample performance; a key model-risk result for any data-driven or ML trading model.

### Data management for AI

- [Data Collection and Quality Challenges in Deep Learning: A Data-Centric AI Perspective (Whang et al., 2023)](https://arxiv.org/abs/2112.06409) - A taxonomy for data-centric AI from collection to quality assurance, arguing that perfect cleaning is impossible so robust training must share the load.
- [Failing Loudly: An Empirical Study of Methods for Detecting Dataset Shift (Rabanser et al., 2019)](https://arxiv.org/abs/1810.11953) - Compares methods for detecting distribution shift, pairing dimensionality reduction with statistical testing.
- [Datasheets for Datasets (Gebru et al., 2021)](https://arxiv.org/abs/1803.09010) - Proposes a standard datasheet documenting a dataset's motivation, composition, collection, and recommended uses across its lifecycle.
- [DMOps: Data Management Operation and Recipes (Choi and Park, 2023)](https://arxiv.org/abs/2301.01228) - A 12-step recipe for the data lifecycle from business goals to delivery, with external-factor and model verification.
- [Data-centric Artificial Intelligence: A Survey (Zha et al., 2023)](https://arxiv.org/abs/2303.10158) - Organises the data lifecycle into training-data development, inference-data development, and data maintenance; a good single overview of the landscape.
- [A Survey of LLM × DATA (Zhou et al., 2025)](https://arxiv.org/abs/2505.18458) - Surveys how data is collected, constructed, and used for language models, and the shift to web-scale unstructured corpora.
- [Scaling Trends for Data Poisoning in LLMs (Bowen et al., 2024)](https://arxiv.org/abs/2408.02946) - Finds that larger models can be more susceptible to data poisoning, learning harmful behaviours from minimal exposure.
- [Data Quality Challenges in Retrieval-Augmented Generation (Müller et al., 2025)](https://arxiv.org/abs/2510.00552) - Identifies 15 data-quality dimensions across four RAG stages and how issues propagate through the pipeline.
- [Episodic Memory in AI Agents Poses Risks that Should be Studied and Mitigated (DeChant, 2025)](https://arxiv.org/abs/2501.11739) - Examines the retention, privacy, and unintended-learning risks that agent memory introduces.
- [What's the Next Frontier for Data-Centric AI? Data Savvy Agents (Seedat et al., 2025)](https://arxiv.org/abs/2511.01015) - Argues autonomous agents need data-savvy capabilities: proactive acquisition, context-aware processing, and continual adaptation.

### Evaluation and testing

- [Machine Learning Testing: Survey, Landscapes and Horizons (Zhang et al., 2020)](https://arxiv.org/abs/1906.10742) - A map of ML testing before generative AI, broken down by properties, components, and workflows.
- [Model Evaluation, Model Selection, and Algorithm Selection in Machine Learning (Raschka, 2018)](https://arxiv.org/abs/1811.12808) - A standard reference on why simple accuracy misleads, separating performance estimation, model selection, and algorithm selection with the statistics to compare them.
- [A Survey on Evaluation of Large Language Models (Chang et al., 2024)](https://arxiv.org/abs/2307.03109) - Comprehensive survey of what, where, and how to evaluate LLMs across tasks, and where the gaps remain.
- [On Robustness and Reliability of Benchmark-Based Evaluation of LLMs (Lunardi et al., 2025)](https://arxiv.org/abs/2509.04013) - Shows how paraphrasing undermines benchmark reliability, arguing for going beyond static benchmarks.
- [Your AI Product Needs Evals (Hamel Husain, 2024)](https://hamel.dev/blog/posts/evals/) - A practitioner guide to moving from vibe checks to a three-level hierarchy of unit tests, human and model evals, and A/B testing.
- [Evaluation and Benchmarking of LLM Agents: A Survey (Mohammadi et al., 2025)](https://arxiv.org/abs/2507.21504) - A taxonomy for agent evaluation across objectives and process, including enterprise hurdles like access control and policy compliance.
- [Evolutionary Perspectives on the Evaluation of LLM-Based AI Agents: A Comprehensive Survey (Zhu et al., 2025)](https://arxiv.org/abs/2506.11102) - Frames agent evaluation as an evolutionary process across environments, feedback, perception, and capabilities.
- [LLMs-as-Judges: A Comprehensive Survey on LLM-based Evaluation Methods (Li et al., 2024)](https://arxiv.org/abs/2412.05579) - Surveys using LLMs as judges, and the biases and vulnerabilities they inherit.
- [Agent-as-a-Judge: Evaluate Agents with Agents (Zhuge et al., 2024)](https://arxiv.org/abs/2410.10934) - Argues static judges miss intermediate steps and proposes an agentic evaluator that inspects the full trajectory.
- [NIST AI Measurement and Evaluation Projects (NIST)](https://www.nist.gov/programs-projects/ai-measurement-and-evaluation/nist-ai-measurement-and-evaluation-projects) - NIST's portfolio of AI measurement and evaluation projects.
- [AI Verify Global AI Assurance Sandbox (AI Verify Foundation / IMDA Singapore)](https://assurance.aiverifyfoundation.sg/) - Case studies of organisations pairing with AI testing specialists under Singapore's assurance programme.
- [ISO/IEC TR 29119-11:2020, Testing of AI-based systems (ISO/IEC, 2020)](https://www.iso.org/standard/79016.html) - Guidelines on testing AI-based systems within the software-testing standards series.

### Human oversight

- [Towards a Science of Human-AI Decision Making: A Survey of Empirical Studies (Lai et al., 2021)](https://arxiv.org/abs/2112.11471) - Organises AI assistance into predictions, prediction-specific information, global model insights, and interaction elements.
- [Human-AI Collaboration is Not Very Collaborative Yet: A Taxonomy of Interaction Patterns (Gomez et al., 2023)](https://arxiv.org/abs/2310.19778) - Finds static paradigms invite anchoring and confirmation bias, and maps dynamic patterns that mitigate them.
- [Human-in-the-Loop Machine Learning (Monarch, 2021)](https://www.manning.com/books/human-in-the-loop-machine-learning) - A book on integrating human judgment into ML through annotation, active learning, and transfer learning.
- [Knowing About Knowing: An Illusion of Human Competence Can Hinder Appropriate Reliance on AI (He et al., 2023)](https://arxiv.org/abs/2301.11333) - Shows overconfident users under-rely on superior AI, and that interventions help some users but hurt others.
- [Effect of Confidence and Explanation on Accuracy and Trust Calibration (Zhang, Liao and Bellamy, 2020)](https://arxiv.org/abs/2001.02114) - Finds confidence scores can calibrate trust but local explanations help little, and human and AI blind spots may coincide.
- [Fewer Than 1% of Explainable AI Papers Validate Explainability with Humans (Suh et al., 2025)](https://arxiv.org/abs/2503.16507) - A review finding under 1% of XAI papers test their claims with human subjects.
- [Designing Meaningful Human Oversight in AI (Zhu et al., 2025)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5501939) - Argues humans should hold evaluative agency with clear handover points, traceability, and top-level control rather than a nominal human-in-the-loop.
- [Should I Follow AI-based Advice? Measuring Appropriate Reliance (Schemmer et al., 2022)](https://arxiv.org/abs/2204.06916) - Proposes relative positive AI-reliance and self-reliance as better measures of effective oversight.
- [Does the Whole Exceed its Parts? The Effect of AI Explanations on Complementary Team Performance (Bansal et al., 2021)](https://arxiv.org/abs/2006.14779) - Finds humans over-rely on AI explanations even when wrong, and that explanations add no benefit over simply showing the AI's confidence.
- [Trust and Reliance in XAI: Distinguishing Between Attitudinal and Behavioral Measures (Scharowski et al., 2022)](https://arxiv.org/abs/2203.12318) - Distinguishes trust (an attitude) from reliance (a behaviour) and questions anthropomorphic framing.
- [To Rely or Not to Rely? Evaluating Interventions for Appropriate Reliance on LLMs (Bo, Wan and Anderson, 2024)](https://arxiv.org/abs/2412.15584) - Finds friction-based interventions reduce over-reliance but can cause under-reliance, and simple disclaimers can outperform complex ones.
- [Unraveling Human-AI Teaming: A Review and Outlook (Lou et al., 2025)](https://arxiv.org/abs/2504.05755) - Examines how agentic AI changes team dynamics, including when AI should delegate tasks to humans.
- [LLM-Based Human-Agent Collaboration and Interaction Systems: A Survey (Zou et al., 2025)](https://arxiv.org/abs/2505.00753) - Surveys human-agent systems by feedback type, interaction mode, orchestration, and communication structure.

### Third-party AI

- [AI Auditing: The Broken Bus on the Road to AI Accountability (Birhane et al., 2024)](https://arxiv.org/abs/2401.14462) - Taxonomises current AI audit practice and finds only a subset translates into accountability outcomes.
- [Dislocated Accountabilities in the AI Supply Chain (Widder and Nafus, 2023)](https://arxiv.org/abs/2209.09780) - Shows developers assume responsible AI belongs to someone else up or down the supply chain.
- [Understanding Accountability in Algorithmic Supply Chains (Cobbe, Veale and Singh, 2023)](https://arxiv.org/abs/2304.14749) - Explores distributed responsibility, the accountability horizon, and cross-border regulatory arbitrage in algorithmic supply chains.
- [AEF-1: Minimum Operating Conditions for Independent Third Party AI Evaluations (AI Evaluator Forum, 2025)](https://www.aef.one/aef-one.pdf) - A voluntary standard setting what independent evaluators need: independence, sufficient access, and transparency of methods and findings.
- [Outsider Oversight: Designing a Third Party Audit Ecosystem for AI Governance (Raji et al., 2022)](https://arxiv.org/abs/2206.04737) - Draws lessons from financial, environmental, and health regulation on designing effective external oversight.
- [Model Cards for Model Reporting (Mitchell et al., 2019)](https://arxiv.org/abs/1810.03993) - The proposal that released models ship with documentation of their performance characteristics and intended use.
- [Third-party compliance reviews for frontier AI safety frameworks (Homewood et al., 2025)](https://arxiv.org/abs/2505.01643) - Examines independent reviews of whether a provider complies with its own safety framework, with the benefits and real costs.
- [Implementing AI Bill of Materials (AI BOM) with SPDX 3.0 (Bennet et al., 2025)](https://arxiv.org/abs/2504.16743) - Extends the software bill of materials to AI: algorithms, data, frameworks, licensing, and compliance.
- [AgentFacts: Universal KYA Standard for Verified AI Agent Metadata (Grogan, 2025)](https://arxiv.org/abs/2506.13794) - Proposes a Know-Your-Agent standard with signed capability declarations and multi-authority validation.

### Explainability and interpretability

- [Stop Explaining Black Box Machine Learning Models for High-Stakes Decisions and Use Interpretable Models Instead (Rudin, 2019)](https://arxiv.org/abs/1811.10154) - An influential argument against post-hoc explanation of black boxes in high-stakes settings in favour of inherently interpretable models.
- [Why Should I Trust You? Explaining the Predictions of Any Classifier, LIME (Ribeiro, Singh and Guestrin, 2016)](https://arxiv.org/abs/1602.04938) - The paper that introduced LIME, learning a local interpretable surrogate around each prediction.
- [A Unified Approach to Interpreting Model Predictions, SHAP (Lundberg and Lee, 2017)](https://arxiv.org/abs/1705.07874) - The paper that introduced SHAP and unified prior attribution methods under local accuracy, missingness, and consistency.
- [One Explanation Does Not Fit All: A Toolkit and Taxonomy of AI Explainability Techniques (Arya et al., 2019)](https://arxiv.org/abs/1909.03012) - Introduces the AI Explainability 360 toolkit; goes beyond SHAP and LIME with a taxonomy of methods and persona-based explanation needs.
- [Interpretable Machine Learning (Molnar, 3rd ed., 2025)](https://christophm.github.io/interpretable-ml-book/) - An open-access textbook covering the full spectrum from linear models and trees to SHAP and counterfactuals.
- [A Comprehensive Guide to Explainable AI: From Classical Models to LLMs (Hsieh et al., 2024)](https://arxiv.org/abs/2412.00800) - A textbook-style guide spanning intrinsically interpretable models, post-hoc methods, and LLM-specific techniques.
- [From Anecdotal Evidence to Quantitative Evaluation Methods: A Systematic Review on Evaluating Explainable AI (Nauta et al., 2023)](https://arxiv.org/abs/2201.08164) - Proposes 12 properties across three dimensions for evaluating explanations.
- [How can I choose an explainer? An Application-grounded Evaluation of Post-hoc Explanations (Jesus et al., 2021)](https://arxiv.org/abs/2101.08758) - A real-world study finding explanations can speed decisions but reduce accuracy versus reviewing raw data.
- [Fooling LIME and SHAP: Adversarial Attacks on Post hoc Explanation Methods (Slack et al., 2020)](https://arxiv.org/abs/1911.02508) - Shows explanation methods can be gamed by adversarial models that hide their bias.
- [Explainability for Large Language Models: A Survey (Zhao et al., 2024)](https://arxiv.org/abs/2309.01029) - A starting overview of LLM explainability across fine-tuning and prompting paradigms and how to evaluate explanations.
- [XAI meets LLMs: A Survey of the Relation between Explainable AI and Large Language Models (Cambria et al., 2024)](https://arxiv.org/abs/2407.15248) - Maps how XAI improves LLMs and how LLMs generate explanations, balancing interpretability with performance.
- [Explainable and Interpretable Multimodal Large Language Models: A Comprehensive Survey (Dang et al., 2024)](https://arxiv.org/abs/2412.02104) - Surveys multimodal LLM interpretability across data, model, and training or inference perspectives.
- [A Survey on Mechanistic Interpretability for Multi-Modal Foundation Models (Lin et al., 2025)](https://arxiv.org/abs/2502.17516) - Compares how LLM interpretability methods adapt to multimodal settings and the gaps that remain.
- [A Survey on Sparse Autoencoders: Interpreting the Internal Mechanisms of Large Language Models (Shu et al., 2025)](https://arxiv.org/abs/2503.05613) - Surveys sparse autoencoders for mechanistic interpretability, covering architecture, training, and evaluation.
- [Mapping the Mind of a Large Language Model (Anthropic, 2024)](https://www.anthropic.com/research/mapping-mind-language-model) - A demonstration of sparse autoencoders at scale on Claude, showing that amplifying or suppressing a feature causally changes the model's behaviour.
- [Persona Vectors: Monitoring and Controlling Character Traits in Language Models (Anthropic, 2025)](https://www.anthropic.com/research/persona-vectors) - Shows how to identify and steer behavioural features such as sycophancy using mechanistic-interpretability methods.
- [TRiSM for Agentic AI: Trust, Risk, and Security Management in LLM-based Agentic Multi-Agent Systems (Raza et al., 2025)](https://arxiv.org/abs/2506.04133) - Adapts trust, risk, and security management for agentic AI with explainability as a pillar.
- [Integrating Counterfactual Simulations with Language Models for Explaining Multi-Agent Behaviour (Gyevnár et al., 2025)](https://arxiv.org/abs/2505.17801) - The AXIS framework uses LLMs to interrogate simulators with what-if prompts to explain agent behaviour.

### Financial stability

- [Intelligent financial system: how AI is transforming finance (BIS Working Paper No 1194, 2024)](https://www.bis.org/publ/work1194.htm) - Maps how AI reshapes intermediation, insurance, asset management and payments, and the financial-stability and prudential implications.
- [Financial Stability Implications of Generative AI: Taming the Animal Spirits (arXiv, 2025)](https://arxiv.org/abs/2510.01451) - Uses LLM-based laboratory experiments to replicate herd-behaviour trading studies, finding AI agents can both reduce and be induced into herding.

### Fairness in credit

- [The Fairness of Credit Scoring Models (Hurlin, Perignon and Saurin, 2024)](https://arxiv.org/abs/2205.10200) - A formal framework to test the algorithmic fairness of scoring models and optimise the fairness-performance trade-off for lenders and regulators.
- [Algorithmic Fairness (Annual Review of Financial Economics, 2023)](https://www.annualreviews.org/content/journals/10.1146/annurev-financial-110921-125930) - Reviews the algorithmic-fairness literature with a credit-scoring emphasis, covering bias measurement and competing metrics, applied to US mortgage data.

### LLMs in finance

- [Deficiency of Large Language Models in Finance: An Empirical Examination of Hallucination (Kang and Liu, 2023)](https://arxiv.org/abs/2311.15548) - Documents serious hallucination by off-the-shelf LLMs on financial concepts and prices, and tests few-shot, DoLa, RAG and tool-use mitigations.
- [FAITH: A Framework for Assessing Intrinsic Tabular Hallucinations in Finance (arXiv, 2025)](https://arxiv.org/abs/2508.05201) - Builds a masked-span benchmark from S&P 500 annual reports to measure numerical hallucination in financial LLMs over tabular data.
- [The New Quant: A Survey of Large Language Models in Financial Prediction and Trading (arXiv, 2025)](https://arxiv.org/abs/2510.05533) - Surveys LLM use across equity prediction and trading and catalogues production risks including temporal leakage, hallucination, interpretability, governance and evaluation standards.

### Agentic AI in finance

- [Strategic Collusion of LLM Agents: Market Division in Multi-Commodity Competitions (arXiv, 2024)](https://arxiv.org/abs/2410.00031) - Shows LLM agents in Cournot markets can autonomously monopolise commodities and divide markets without explicit collusion instructions.
- [Evaluating LLM Agent Collusion in Double Auctions (arXiv, 2025)](https://arxiv.org/abs/2507.01413) - Continuous-double-auction experiments find LLM seller agents collude more when able to communicate, with propensity varying by model and oversight pressure.
- [AI Agents in Financial Markets: Architecture, Applications, and Systemic Implications (arXiv, 2026)](https://arxiv.org/abs/2603.13942) - Proposes a four-layer agent architecture and a stylised agent-based market model linking autonomy, coupling and infrastructure concentration to liquidity resilience and systemic risk.

### Books

- [Machine Learning for High-Risk Applications: Approaches to Responsible AI (Hall, Curtis and Pandey, 2023)](https://www.oreilly.com/library/view/machine-learning-for/9781098102425/) - Practitioner guide to responsible AI covering explainability, model validation and debugging, bias and security, grounded in the NIST AI RMF.
- [AI Snake Oil (Narayanan and Kapoor, 2024)](https://press.princeton.edu/books/hardcover/9780691249131/ai-snake-oil) - Princeton University Press book distinguishing credible AI from hype, relevant to predictive AI in high-stakes decisions.
- [Machine Learning for Financial Risk Management with Python (Karasan, 2021)](https://www.oreilly.com/library/view/machine-learning-for/9781492085249/) - Hands-on text applying ML algorithms to market, credit, liquidity and operational risk modelling.
- [A First Course in Model Validation and Model Risk Management (Schachter, Goldberg and Maheshwari, 2026)](https://shop.elsevier.com/books/a-first-course-in-model-validation-and-model-risk-management/schachter/978-0-443-33746-8) - Textbook on model validation and model risk management for financial engineers.

### Courses and training

- [Cambridge FinTech and Regulatory Innovation Accelerator (Cambridge CCAF)](https://www.jbs.cam.ac.uk/faculty-research/centres/alternative-finance/courses/fintech-regulatory-innovation/) - Cambridge Judge executive online programme for financial regulators and supervisors, covering AI and emerging-technology oversight.
- [Capacity Building and Education (Cambridge SupTech Lab)](https://cambridgesuptechlab.org/capacity-building-education/) - Training and tools for financial authorities on supervisory technology and AI readiness.
- [Artificial Intelligence for Financial Services: Tools, Opportunities, and Challenges (MIT Sloan Executive Education)](https://executive.mit.edu/course/artificial-intelligence-for-financial-services/a05U100000BIm1RIAT.html) - In-person executive course led by Professor Andrew Lo on how AI and machine learning are applied across investment, banking, insurance and risk management, including the capabilities, limits and regulatory implications of current AI tools.
- [Leading AI Adoption in Financial Services Programme (Oxford Saïd Business School)](https://www.sbs.ox.ac.uk/programmes/online-learning/oxford-leading-ai-adoption-financial-services-programme) - Five-week online programme on adopting AI across regulated financial institutions, with a dedicated module on scaling AI responsibly while managing governance, risk and compliance.
- [AI in Finance: Strategy, Applications and Impact (Imperial College Business School)](https://www.imperial.ac.uk/business-school/executive-education/finance-economics/ai-finance-strategy-applications-Impact/online/) - Six-week online programme covering AI across trading, lending and credit risk, fraud detection and compliance, aimed at evaluating and implementing AI responsibly in finance functions.
- [Digital Finance & Fintech with AI Programme (Singapore Management University)](https://smu.emeritus.org/digital-finance-and-fintech-with-ai-programme) - A 21-week online executive programme on AI applications in finance, finance automation and RegTech.
- [Fintech Revolution (Wharton Executive Education)](https://executiveeducation.wharton.upenn.edu/online-learning/self-paced-online-programs/fintech-revolution-program/) - Self-paced programme on fintech disruption across banking, lending and payments, including AI and machine learning applications in financial services.
- [Artificial Intelligence for Financial Supervision Program (Toronto Centre)](https://www.torontocentre.org/index.php?option=com_jem&view=event&id=199:artificial-intelligence-for-financial-supervision-program&Itemid=158) - Virtual programme for financial-sector supervisors on identifying AI risks and opportunities, emerging governance and regulatory expectations, and overseeing AI-enabled systems proportionately.
- [FSI capacity development and FSI Connect (BIS Financial Stability Institute)](https://www.bis.org/about/fsi/capacity-development) - The Financial Stability Institute's e-learning platform and online courses for central banks and supervisors, covering prudential standards and supervisory practices including AI-related topics (access restricted to eligible public-sector authorities).
- [Machine Learning and Reinforcement Learning in Finance (New York University, Coursera)](https://www.coursera.org/specializations/machine-learning-reinforcement-finance) - NYU specialisation applying machine learning and reinforcement learning to finance problems such as trading, asset management and banking.
- [MSc in Financial Engineering (WorldQuant University)](https://www.wqu.edu/mscfe) - Tuition-free, accredited online master's covering quantitative finance, machine learning and financial risk modelling.
- [Generative AI for Compliance in Financial Services (CFTE)](https://courses.cfte.education/generative-ai-for-compliance-in-financial-services-online-course/) - IBF-accredited online course for compliance officers and risk managers on using and overseeing generative AI responsibly in compliance, monitoring and risk oversight.

### Blogs, newsletters and people

- [Eugene Yan (eugeneyan.com)](https://eugeneyan.com/) - Applied ML practitioner writing substantively on LLM evaluation, eval design and production ML, directly useful for AI risk and model testing.
- [AI as Normal Technology, formerly AI Snake Oil (Narayanan and Kapoor)](https://www.normaltech.ai/) - Princeton-led newsletter critically analysing AI capabilities, evaluation and overclaiming, including predictive AI in consequential domains.

### Reference hubs

- [AI RMF Resources and Knowledge Base (NIST AI Resource Center)](https://airc.nist.gov/airmf-resources/) - NIST's hub for the AI RMF Playbook, glossary, use cases and crosswalks mapping the RMF to other standards.
- [AI Standards Hub (NPL, BSI and UKAS)](https://aistandardshub.org/) - UK platform for tracking AI standards, with tools, training and a standards database; as of 2026 transitioning to new operators, so parts may be temporarily unavailable.
- [OECD.AI Policy Observatory (OECD)](https://oecd.ai/en/) - Repository of national AI policies, live data and analysis anchored on the OECD AI Principles.
- [Global AI Law and Policy Tracker (IAPP)](https://iapp.org/resources/article/global-ai-legislation-tracker) - Country-by-country tracker of AI legislative and policy developments across jurisdictions; the full tracker requires IAPP membership.
- [AI Watch: Global Regulatory Tracker (White & Case)](https://www.whitecase.com/insight-our-thinking/ai-watch-global-regulatory-tracker) - Law-firm tracker analysing each jurisdiction's approach to AI regulation.
- [EU AI Act Explorer (Future of Life Institute)](https://artificialintelligenceact.eu/ai-act-explorer/) - An interactive navigator for the EU AI Act's text and obligations by risk category.

## From the maintainer

Public writing from the maintainer on AI risk management in finance. Included as curation, clearly flagged as self-authored.

- [AI risk management, explained](https://quaintitative.com/ai-risk-management/) - a plain-language guide to what AI risk management is and the areas it covers.
- [The AIRG, explained](https://quaintitative.com/airg/) - Singapore's AI risk management guidelines, by the person who wrote them.
- [The AIRG is final](https://quaintitative.com/airg-final/) - what changed in the final MAS guidelines of 7 October 2026, and what it means for firms.
- [The AIRG compared to the EU AI Act, NIST, and ISO 42001](https://quaintitative.com/airg-vs-eu-ai-act-nist-iso-42001/) - how the main frameworks line up, area by area.
- [AIRG, Project MindForge, and the CRI Financial Services AI Risk Management Framework](https://quaintitative.com/airg-mindforge-cri/) - a structural map of three financial-services references: expectations, risks and practices, and controls.
- [AI Risk Management for Regulators and Supervisors](https://quaintitative.com/ai-governance-for-regulators/) - a short book, serialised, on how a supervisor judges whether a firm's AI risk management is adequate.
- [AI Risk Management for Risk and Compliance](https://quaintitative.com/ai-risk-management-for-compliance/) - a short book, serialised, on how the second line runs and challenges AI from inside a firm.
- [The MindForge Toolkit guides](https://quaintitative.com/mindforge-toolkit/) - a guide per area of the Project MindForge AI Risk Management Toolkit, each linked to the AIRG.
- [Gary Ang on SSRN](https://papers.ssrn.com/sol3/cf_dev/AbsByAuth.cfm?per_id=11129509) and [Google Scholar](https://scholar.google.com/citations?user=KEfvMvUAAAAJ) - peer-reviewed research, including work on AI and networks in finance.

### Books by the maintainer

- [AI Risk Management from First Principles](https://www.learn.simplyboring.ai/shop/p/ai-risk-management-from-first-principles-a-primer) - AI risk management as three questions, from machine learning to agents, in plain English.
- [Boring Questions on AI Risk Management for Directors](https://www.learn.simplyboring.ai/shop/p/ai-risk-management-for-directors) - A board-facing guide: five questions to take into the next board meeting, through the financial sector's risk lens.
- [AI Risk Management for Agents](https://www.learn.simplyboring.ai/shop/p/the-primer-ai-risk-management-for-agents) - Governing what an AI agent may do when you cannot review every path it might take.
- [Scaling AI Governance](https://www.learn.simplyboring.ai/shop/p/scaling-ai-governance) - Three moves to collapse many AI governance frameworks into one backbone you can scale.
- [The Boring Reading List for AI Risk Management](https://www.learn.simplyboring.ai/shop/p/the-boring-reading-list-for-ai-risk-management) - Six short reading lists by area, each reading with a note on why it is worth reading.
- [AI Agents for Investing](https://www.learn.simplyboring.ai/shop/p/ai-agents-for-investing) - Four agent patterns, with code, to build AI investing tools grounded in real data and auditable calculations.
- [AI Agents for Forecasting](https://www.learn.simplyboring.ai/shop/p/ai-agents-for-forecasting-a-primer) - Why a language model cannot forecast on its own, and the agent architecture that drives the real forecasting tools.

## Contributing

Additions, corrections, and removals are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for what belongs here and the one-line entry format.

## Licence

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

To the extent possible under law, the maintainer has waived all copyright and related or neighbouring rights to this work. See [LICENSE](LICENSE).
