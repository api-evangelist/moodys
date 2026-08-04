# Moody's (moodys)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Moody's provides a comprehensive suite of APIs spanning KYC compliance, economic data and forecasting, credit risk analytics, insurance and catastrophe modeling, climate risk, commercial real estate, and news aggregation. With evolving regulatory pressures and increasingly complex risk landscapes, Moody's technology, data, and analytical capabilities power industry-leading solutions across financial services, insurance, and risk management.

**APIs.json:** [https://github.com/api-search/moodys/apis.yml](https://github.com/api-search/moodys/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening

## Timestamps

- **Created:** 2024-09-25T00:00:00.000Z
- **Modified:** 2026-05-19

## APIs

### Moody's KYC API

With evolving regulatory pressures and bad actors becoming increasingly adept at concealing themselves, the need for deep understanding of business partners, customers, and other third parties is more critical than ever to mitigate reputational damage and risk exposure. Moody s KYC technology, data, and analytical capabilities provide industry-leading customer solutions for Know Your Customer, anti-money laundering, compliance, and counter-party risk.

- **Human URL:** [https://www.kompany.com/kycapi/discover](https://www.kompany.com/kycapi/discover)

#### Tags

- Anti-Money Laundering
- Compliance
- Entity Verification
- KYC
- Risk
- Screening

#### Properties

- [Documentation](https://www.kompany.com/kycapi/console-v2)
- [OpenAPI](
https://www.kompany.com/kycapi/docs/resources/resources/customer-facing-documents/generate-a-client-from-openapi-definition) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Moody's Data Buffet API

Moody's Analytics Data Buffet application program interface enables you to retrieve economic, demographic and financial time series directly from the Data Buffet repository, including international and subnational economic and demographic time series data and forecasts.

- **Human URL:** [https://www.economy.com/products/tools/data-buffet](https://www.economy.com/products/tools/data-buffet)
- **Base URL:** `https://api.economy.com`

#### Tags

- Demographics
- Economic Data
- Forecasts
- Time Series

#### Properties

- [Documentation](https://api.economy.com/data/v1/swagger)
- [GitHub Organization](https://github.com/moodysanalytics/databuffet-api-codesamples)
- [OpenAPI](openapi/moodys-data-buffet-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/moodys-time-series-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/moodys-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Moody's Scenario Studio API

Scenario Studio delivers Moody's Analytics Global Macroeconomic Model that emphasizes stability, forecast accuracy and consistency. The API retrieves custom scenarios generated in the Scenario Studio platform.

- **Human URL:** [https://hub.moodysanalytics.com/products](https://hub.moodysanalytics.com/products)
- **Base URL:** `https://api.economy.com`

#### Tags

- Economic Models
- Forecasting
- Macroeconomic
- Scenarios

#### Properties

- [Documentation](https://api.economy.com/scenario-studio/v2/swagger)
- [GitHub Organization](https://github.com/moodysanalytics/scenario-studio-api-codesamples)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's AutoCycle API

Retrieves forecasts of vehicle prices from AutoCycle models. AutoCycle is a software solution to forecast car prices, incorporating economic data and scenarios from Moody's Analytics.

- **Human URL:** [https://hub.moodysanalytics.com/products](https://hub.moodysanalytics.com/products)
- **Base URL:** `https://api.economy.com`

#### Tags

- Automotive
- Forecasts
- Residual Value
- Vehicle Pricing

#### Properties

- [Documentation](https://api.economy.com/autocycle/v1/swagger)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's Consumer Credit Loss Forecasts API

Retrieves expected consumer credit loss forecasts under baseline and stress scenarios. The ECCL API combines customer data, economic data from Moody's Analytics, and consumer credit data for credit risk modeling.

- **Human URL:** [https://hub.moodysanalytics.com/products](https://hub.moodysanalytics.com/products)
- **Base URL:** `https://api.economy.com`

#### Tags

- Consumer Credit
- Credit Loss
- Forecasts
- Risk

#### Properties

- [Documentation](https://api.economy.com/eccl/v1/swagger)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's Municipal Probability of Default API

Retrieves probability of default and loss rates for the municipal market under baseline and stress scenarios. Enables scoring of municipal credit risk using Moody's Analytics models.

- **Human URL:** [https://hub.moodysanalytics.com/products](https://hub.moodysanalytics.com/products)
- **Base URL:** `https://api.economy.com`

#### Tags

- Credit Risk
- Forecasts
- Municipal
- Probability of Default

#### Properties

- [Documentation](https://api.economy.com/muni/v1/swagger)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's EDF-X API

The EDF-X API provides easy access to probability of default calculations for approximately 400 million companies globally via the Orbis database. It provides a PD term structure with annualized, cumulative, and forward PD values, implied ratings, and confidence indicators.

- **Human URL:** [https://hub.moodysanalytics.com/products](https://hub.moodysanalytics.com/products)
- **Base URL:** `https://hub.moodysanalytics.com`

#### Tags

- Credit Risk
- Expected Default Frequency
- Probability of Default
- Risk Assessment

#### Properties

- [Documentation](https://hub.moodysanalytics.com/products)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)


#### Tags

- Media
- News
- Real-Time Data
- Social Media

#### Properties

- [Documentation](https://hub.moodysanalytics.com/products)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's QUIQSpread API

Moody's Analytics QUIQspread is an intelligent, financial spreading software that will accelerate a company's spreading process. The API enables integration of automated financial statement processing into banking workflows.

- **Human URL:** [https://hub.moodysanalytics.com/products](https://hub.moodysanalytics.com/products)
- **Base URL:** `https://hub.moodysanalytics.com`

#### Tags

- Automation
- Banking
- Financial Spreading
- Financial Statements

#### Properties

- [Documentation](https://hub.moodysanalytics.com/products)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's Capital Risk Analyzer API

Moody's Analytics Capital Risk Analyzer solution is a tool that projects key capital ratios and credit metrics based on various strategic and economic scenarios for capital planning and stress testing such as DFAST and EBA.

- **Human URL:** [https://hub.moodysanalytics.com/products](https://hub.moodysanalytics.com/products)
- **Base URL:** `https://hub.moodysanalytics.com`

#### Tags

- Banking
- Capital Planning
- Risk
- Stress Testing

#### Properties

- [Documentation](https://hub.moodysanalytics.com/products)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's Climate on Demand API

The Climate On Demand API enables financial services organizations to build physical climate risk applications that leverage the power of the Intelligent Risk Platform.

- **Human URL:** [https://developer.rms.com/climate-on-demand](https://developer.rms.com/climate-on-demand)
- **Base URL:** `https://developer.rms.com`

#### Tags

- Climate Risk
- Environmental
- Insurance
- Physical Risk

#### Properties

- [Documentation](https://developer.rms.com/climate-on-demand)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's Location Intelligence API

Location Intelligence API delivers more than 100 data layers across multiple kinds of data including hazard, location, risk score, model, and exposure data to help improve business decisions and better manage risk.

- **Human URL:** [https://hub.moodysanalytics.com/products](https://hub.moodysanalytics.com/products)
- **Base URL:** `https://developer.rms.com`

#### Tags

- Geospatial
- Insurance
- Location
- Risk Data

#### Properties

- [Documentation](https://hub.moodysanalytics.com/products)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's Risk Modeler API

The Risk Modeler API enables you to manage end-to-end catastrophe modeling workflows using Moody's RMS models for portfolios, accounts, and locations on the Intelligent Risk Platform.

- **Human URL:** [https://developer.rms.com/risk-modeler](https://developer.rms.com/risk-modeler)
- **Base URL:** `https://developer.rms.com`

#### Tags

- Catastrophe Modeling
- Insurance
- Risk
- Underwriting

#### Properties

- [Documentation](https://developer.rms.com/risk-modeler)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's Intelligent Risk Platform API

Moody's RMS Platform APIs are a collection of REST APIs that enable Intelligent Risk Platform tenants to work more efficiently. Risk Modeler, UnderwriteIQ, TreatyIQ, and ExposureIQ tenants can use them to manage bulk data transfers, automate catastrophe modeling workflows, and generate reports.

- **Human URL:** [https://developer.rms.com/platform/docs/introduction](https://developer.rms.com/platform/docs/introduction)
- **Base URL:** `https://developer.rms.com`

#### Tags

- Insurance
- Platform
- Reinsurance
- Risk Management

#### Properties

- [Documentation](https://developer.rms.com/platform/docs/introduction)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Moody's Commercial Real Estate API

API solutions to empower commercial real estate developers to build systems and platforms faster. Brings efficiency and automation into your organization, including the Commercial Location Score API and MA CRE API.

- **Human URL:** [https://hub.moodysanalytics.com/products](https://hub.moodysanalytics.com/products)
- **Base URL:** `https://hub.moodysanalytics.com`

#### Tags

- Commercial Real Estate
- CRE
- Location Score
- Property

#### Properties

- [Documentation](https://hub.moodysanalytics.com/products)
- [Postman Collection](collections/moodys-data-buffet-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/moodys-data-buffet-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.kompany.com/)
- [Plans](https://www.kompany.com/kycapi/dashboard/plans)
- [Getting Started](https://www.kompany.com/kycapi/docs/quick-start)
- [Console](https://www.kompany.com/kycapi/console)
- [Blog](https://www.kompany.com/kycapi/community/developer-news)
- [Getting Started](https://www.kompany.com/kycapi/docs/guides/guides/get-started)
- [Sandbox](https://www.kompany.com/kycapi/docs/guides/guides/get-started/sandbox-overview)
- [Use Cases](https://www.kompany.com/kycapi/docs/guides/guides/use-cases)
- [Resources](https://www.kompany.com/kycapi/docs/resources)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Integrations](https://www.kompany.com/kycapi/connections)
- [Status Page](https://kycapi-status.kompany.com/)
- [Portal](https://hub.moodysanalytics.com/)
- [Documentation](https://hub.moodysanalytics.com/products)
- [Getting Started](https://hub.moodysanalytics.com/gettingstarted)
- [Contact](https://hub.moodysanalytics.com/contact)
- [Portal](https://developer.rms.com/)
- [Documentation](https://www.economy.com/products/tools/api)
- [GitHub Organization](https://github.com/moodysanalytics)
- [Resources](https://www.rms.com/developer-resources)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
