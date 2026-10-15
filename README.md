# Community-Institution-AI-and-Data-Governance-Framework
Version 0.1, public draft for comment. Author **Admore Mungwadzi**
# 1. Purpose and scope
This Framework gives U.S. community banks and credit unions a practical, right-sized way to govern artificial intelligence and the data that feeds it. It turns high-level standards into specific controls that a small risk or IT team can put in place in about 90 days.
# Who it is for
Institutions without a dedicated AI-risk function: typically community banks and credit unions under about $10 billion in assets. Larger institutions can use it as a baseline.
# Why it is needed
The U.S. Treasury found that smaller institutions "generally lack sufficient internal data and expertise to build their own anti-fraud AI models" and that smaller firms "solely rely on third-party or core service providers" for AI capabilities (Treasury, March 2024; report, p. 34). Most community institutions will therefore use AI they did not build and cannot fully inspect. Existing standards tell them what good looks like; this Framework tells them what to do on Monday.
# What AI is in scope
1. **Vendor AI** embedded in core, fraud, lending, marketing or service platforms.
2. **Generative AI** tools used by staff (chat assistants, writing and coding tools).
3. **In-house models**, including scorecards and machine-learning models built or tuned by the institution.
# What it is not
It is not regulatory guidance, a legal opinion or a certification scheme. It helps an institution show examiners, auditors and its board that AI risk is identified, owned and controlled.
# 2. How to use the Framework
# Tiers
Every control has a tier, so an institution does only what its AI use requires.
| Tier | Applies when | Typical institution |
|---|---|---|
| **T1 Foundational** | Always, once staff or vendors use any AI | Every community bank and credit union |
| **T2 Enhanced** | AI influences credit, fraud, account-opening or member/customer decisions | Most institutions using vendor fraud or lending tools |
| **T3 Advanced** | The institution builds, trains or materially tunes its own models | Larger community institutions with data science staff |

Start with all T1 controls. Add T2 and T3 controls only where the trigger applies.
# Alignment with existing U.S. guidance
The Framework does not create new requirements. It organizes existing ones so a small team can act on them.
| Source | How the Framework uses it |
|---|---|
| [National Institute of Standards and Technology (NIST) Artificial Intelligence Risk Management Framework 1.0](https://www.nist.gov/itl/ai-risk-management-framework) | Every control is linked to one of its four functions: Govern, Map, Measure and Manage |
| [National Institute of Standards and Technology Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework) | Security and incident controls use the same terms, so they fit into an institution's existing security programme |
| [Federal Reserve Supervisory Letter SR 11-7, Guidance on Model Risk Management](https://www.federalreserve.gov/supervisionreg/srletters/sr1107.htm) | Basis for the model risk and fairness controls, scaled down for models bought from vendors |
| [Federal Reserve Supervisory Letter SR 23-4, Interagency Guidance on Third-Party Relationships: Risk Management](https://www.federalreserve.gov/supervisionreg/srletters/SR2304.htm) (June 2023) | Basis for the third-party AI controls |
| [Federal Financial Institutions Examination Council (FFIEC) Information Technology Examination Handbook](https://ithandbook.ffiec.gov/) | The evidence for each control is described so that bank examiners can find it |
| The [computer-security incident notification rule for banks](https://www.federalreserve.gov/newsevents/pressreleases/bcreg20211118a.htm) (report within 36 hours) and the [National Credit Union Administration (NCUA) cyber incident notification rule, Title 12 of the Code of Federal Regulations, Part 748](https://www.ecfr.gov/current/title-12/chapter-VII/subchapter-A/part-748) (credit unions, report within 72 hours) | Built into the AI incident controls  Since September 1, 2023, a federally insured credit union must notify the NCUA "as soon as possible and **no later than 72 hours** after it reasonably believes a reportable cyber incident has occurred  |
| The [Equal Credit Opportunity Act (ECOA) and its Regulation B rule on adverse action notices, Title 12 of the Code of Federal Regulations, section 1002.9](https://www.ecfr.gov/current/title-12/chapter-X/part-1002/section-1002.9) | Basis for the requirement that AI used in lending decisions can explain why an applicant was turned down |

### Control format

Each control has an ID, a plain statement of what to do, its tier, the function it supports under the NIST Artificial Intelligence Risk Management Framework (Govern, Map, Measure or Manage), and the evidence an auditor or examiner can ask for.

Each control ID starts with a two-letter code for its group: GV for governance, DG for data governance, TP for third-party AI, MR for model risk and fairness, SE for security, and IR for incidents and resilience.

## 3. Control catalogue

Thirty controls in six domains. Twelve are T1 Foundational and apply to every institution. The "AI risk function" column shows which of the four functions of the NIST Artificial Intelligence Risk Management Framework each control supports.

### GV: Governance and accountability
| ID | Control | Tier | AI risk function | Evidence |
|---|---|---|---|---|
| GV-1 | Keep an inventory of every AI use: vendor features, staff generative AI tools and in-house models, with owner, purpose and data used. | T1 | Govern / Map | Current AI inventory, reviewed at least twice a year |
| GV-2 | Name one accountable executive for AI risk and report AI risk to the board or a board committee at least annually. | T1 | Govern | Board minutes; charter or delegation |
| GV-3 | Adopt an AI acceptable-use policy covering what staff may and may not enter into generative AI tools. | T1 | Govern | Approved policy; staff attestations |
| GV-4 | Rate each AI use as low, medium or high risk based on customer impact, data sensitivity and autonomy; apply T2 controls to medium and high. | T1 | Map | Risk rating in the inventory |
| GV-5 | Train staff annually on the AI policy and on AI-enabled fraud such as deepfakes. | T1 | Govern | Training records |

### DG: Data governance for AI
| ID | Control | Tier | AI risk function | Evidence |
|---|---|---|---|---|
| DG-1 | Classify the data each AI use consumes (public, internal, confidential, nonpublic personal information) and record it in the inventory. | T1 | Map | Data classification per AI use |
| DG-2 | Prohibit nonpublic personal information in AI tools not approved for it; enforce with technical controls where possible. | T1 | Manage | Policy; data-loss-prevention rules or tool settings |
| DG-3 | Record the lineage of data feeding medium- and high-risk AI: source systems, transformations and refresh frequency. | T2 | Map | Lineage records |
| DG-4 | Run data quality checks (completeness, accuracy, timeliness) on inputs to medium- and high-risk AI before use and on a schedule. | T2 | Measure | Data quality reports |
| DG-5 | Set retention and deletion rules for AI inputs, outputs and logs, including data held by vendors. | T2 | Manage | Retention schedule; vendor confirmation |

### TP: Third-party AI
| ID | Control | Tier | AI risk function | Evidence |
|---|---|---|---|---|
| TP-1 | Before buying or enabling any AI feature, complete the due-diligence questionnaire in Appendix A. | T1 | Map | Completed questionnaire |
| TP-2 | Include the AI contract clauses in Appendix A (data use, no training on institution data without consent, incident notice, change notice, audit rights). | T2 | Govern | Executed contract or addendum |
| TP-3 | Get the vendor's model documentation and performance evidence for medium- and high-risk AI at least annually. | T2 | Measure | Vendor documentation on file |
| TP-4 | Monitor vendor AI for changes in behavior or version and require notice before material model changes. | T2 | Manage | Change notices; monitoring log |
| TP-5 | Keep an exit or fallback plan for critical vendor AI, including manual processing. | T2 | Manage | Documented exit plan |

### MR: Model risk and fairness
| ID | Control | Tier | AI risk function | Evidence |
|---|---|---|---|---|
| MR-1 | Test medium- and high-risk AI before use for accuracy on the institution's own population, not only the vendor's. | T2 | Measure | Pre-deployment test results |
| MR-2 | For AI used in credit decisions, confirm it can produce specific principal reasons for adverse action. | T2 | Measure | Sample adverse-action reasons; compliance sign-off |
| MR-3 | Test credit and account decisions for disparate outcomes across protected groups, using available proxies where needed. | T2 | Measure | Fair lending analysis |
| MR-4 | Define human review and override for high-risk AI decisions and record overrides. | T2 | Manage | Procedure; override log |
| MR-5 | Monitor performance and drift monthly or quarterly with thresholds that trigger review. | T3 | Measure | Monitoring reports |
| MR-6 | Independently validate in-house models before use and after material change. | T3 | Measure | Validation report |

### SE: Security of AI systems
| ID | Control | Tier | AI risk function | Evidence |
|---|---|---|---|---|
| SE-1 | Restrict access to AI systems, prompts, configurations and training data by role, with multi-factor authentication. | T1 | Manage | Access reviews |
| SE-2 | For generative AI connected to internal data, test for prompt injection and data leakage before use. | T2 | Measure | Test results |
| SE-3 | Add controls against deepfake and synthetic-identity fraud: call-back verification for payment changes and large wires, liveness checks in digital onboarding. | T1 | Manage | Procedures; exception reports |
| SE-4 | Log AI inputs, outputs and administrative actions for medium- and high-risk AI and keep logs long enough to investigate incidents. | T2 | Manage | Log configuration; sample logs |
| SE-5 | Include AI systems in vulnerability management and penetration testing scope. | T3 | Manage | Test scope and reports |

### IR: AI incidents and resilience
| ID | Control | Tier | AI risk function | Evidence |
|---|---|---|---|---|
| IR-1 | Define an AI incident (for example model failure, data poisoning, data leakage through AI, AI-enabled fraud) and add it to the incident response plan. | T1 | Govern | Updated incident response plan |
| IR-2 | Map AI incidents to regulatory notification duties (36-hour rule for banks, 72-hour rule for credit unions) and to customer notice duties. | T1 | Govern | Notification decision tree |
| IR-3 | Keep a playbook for the most likely AI incident; see Appendix B. | T2 | Manage | Playbook; exercise record |
| IR-4 | Exercise one AI incident scenario each year, with the vendor where relevant. | T2 | Manage | Tabletop exercise report |

## 4. 90-day adoption plan and self-assessment

### 90-day plan for T1 controls
| Days | Actions | Controls |
|---|---|---|
| 1 to 30 | Name the accountable executive; build the AI inventory by surveying departments and reviewing vendor release notes; rate each use. | GV-1, GV-2, GV-4 |
| 31 to 60 | Approve the acceptable-use policy; classify data per AI use; block nonpublic personal information in unapproved tools; run the vendor questionnaire on existing AI vendors. | GV-3, DG-1, DG-2, TP-1, SE-1 |
| 61 to 90 | Update the incident response plan and notification tree; add deepfake call-back and liveness controls; train staff; first board report. | IR-1, IR-2, SE-3, GV-5 |

### Maturity self-assessment

Score each applicable control from 0 to 3.

| Score | Meaning |
|---|---|
| 0 | Not in place |
| 1 | Partly in place or informal |
| 2 | In place and documented |
| 3 | In place, documented and tested or reviewed in the last 12 months |

Report the average score per domain. A domain average below 2 on applicable controls is a priority for the next quarter.

## 5. Board and examiner one-page report

Report these items to the board or risk committee at least annually, and keep the latest version ready for examiners.

| Item | What to report |
|---|---|
| AI inventory | Number of AI uses by risk rating (low, medium, high); new and retired uses since last report |
| Control status | Domain maturity averages from the self-assessment; open gaps and target dates |
| Vendors | AI vendors reviewed with the Appendix A questionnaire; contracts missing AI clauses |
| Performance and fairness | Any T2 or T3 model outside its thresholds; results of fair lending testing |
| Incidents | AI incidents and near misses, including AI-enabled fraud attempts; regulatory notifications made |
| Staff | Training completion; policy exceptions granted |
| Decisions needed | New high-risk AI uses awaiting approval; risk acceptances |

## Appendix A. Third-party AI due diligence

### A1. Questionnaire (TP-1)

Ask every vendor before enabling an AI feature. Twenty questions in five groups.

**Purpose and design**

1. What does the AI feature do, and what decisions or outputs does it produce?
2. Is it a machine-learning model, a generative AI model, a rules engine, or a mix?
3. Which third-party models or AI services does it rely on (for example a foundation model provider)?
4. Can we turn the feature off without losing the core service?

**Data**

5. What of our data does the feature use, and where is it processed and stored?
6. Will our data, or our customers' or members' data, be used to train or improve models for you or others? Can we opt out?
7. How long are inputs, outputs and logs kept, and how are they deleted?
8. Is nonpublic personal information encrypted in transit and at rest, and who at your company can access it?

**Performance and fairness**

9. How was the model tested, on what data, and with what results?
10. How do you test for disparate outcomes across protected groups? Can we see the results?
11. For credit uses, can the system give specific principal reasons for adverse action?
12. How do you detect performance drift, and how often do you retrain or update the model?

**Security**

13. How do you protect the model and its data from manipulation, data poisoning and prompt injection?
14. Has the AI feature been included in independent security testing? Can we see a summary?
15. What logs of AI activity can we access for our own investigations?

**Change, incidents and exit**

16. How much notice will you give before a material change to the model or its data sources?
17. How quickly will you notify us of an incident affecting the AI feature or our data?
18. Do you carry insurance or indemnities covering AI-related errors or incidents?
19. What happens to our data and any institution-specific tuning if we leave?
20. Who is our contact for AI risk questions?

## Appendix B. Example playbook: deepfake-enabled payment fraud (IR-3)

**Scenario.** A staff member receives a video or voice call that appears to come from the CEO or a known business customer, asking for an urgent wire or a change to payment instructions. The voice or video is AI-generated.

| Phase | Actions | Owner |
|---|---|---|
| Prevent | Call-back to a number on file (never one given in the request) for payment changes and wires over **[threshold]**; two-person approval; staff trained to treat urgency and secrecy as red flags (SE-3, GV-5) | Operations; training |
| Detect | Staff report suspected impersonation to a single contact point; fraud team reviews recent requests from the same channel | All staff; fraud team |
| Contain | Stop or recall the payment; contact the receiving bank; lock affected accounts or credentials; preserve call recordings, emails and logs (SE-4) | Payments; IT security |
| Assess | Decide whether it is a notifiable incident under the notification tree (IR-2): consider losses, systems affected and customer data exposed | Incident lead; compliance |
| Notify | Notify the regulator within the applicable deadline if required; notify affected customers or members; file a Suspicious Activity Report if thresholds are met; report to law enforcement | Compliance; Bank Secrecy Act officer |
| Recover and learn | Review what failed; update thresholds, training and the AI inventory; record in the board report (Section 5) | Accountable executive |
## Versioning, feedback, license and disclaimer

- **Version:** 0.1, public draft for comment, released **September 13th, 2026**
