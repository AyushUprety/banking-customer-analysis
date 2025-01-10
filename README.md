# Czech Bank’s Financial Data Analysis  
**Moving from Gut Feeling to Data-Driven Decisions**

This README provides a comprehensive report integrating key HR considerations—useful for both technical and non-technical audiences.

---

## Table of Contents
1. [Database Schema Overview](#1-database-schema-overview)
2. [Customers & Demographics](#2-customers--demographics)
   - [Clients Distribution by Regions](#21-clients-distribution-by-regions)
3. [Card Products Analysis](#3-card-products-analysis)
   - [Card Products Distribution](#31-card-products-distribution)
4. [Loan Insights](#4-loan-insights)
   - [Correlation Among Loan Attributes](#41-correlation-among-loan-attributes)
   - [Loan Status by District](#42-loan-status-by-district)
5. [Transaction Flows & Trends](#5-transaction-flows--trends)
   - [Collection vs. Remittance Over the Years](#51-collection-vs-remittance-over-the-years)
   - [Overall Inflows & Outflows](#52-overall-inflows--outflows)
6. [Key Takeaways with Integrated HR Implications](#6-key-takeaways-with-integrated-hr-implications)
7. [Strategic Recommendations](#7-strategic-recommendations)
8. [Conclusion](#8-conclusion)

---

## 1. Database Schema Overview
**Figure 1** (below) illustrates the **database schema** for the Czech Bank environment. Here you can see how **Clients**, **Accounts**, **Loans**, **Credit Cards**, **Dispositions**, **Permanent Orders**, **Transactions**, and **District/Demographic** data connect:

> **Figure 1: Database schema**  
> ![Descriptive alt text](https://private-user-images.githubusercontent.com/50670035/401802017-88e46b70-5a4c-40c8-a1dd-93aa5404b122.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDIwMTctODhlNDZiNzAtNWE0Yy00MGM4LWExZGQtOTNhYTU0MDRiMTIyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWYwN2VkZjYxZjJiMDZiNzEyYzZjNDcyNDBlZTgxYzg1ZjA5MDBiMjE0ZTZmNTlkMGM3OTJlMmU4NjM2YTk0ZjEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.QOxf_-AvYE-AnDV2r5P2fVNqLGmoO6rSxFLYmoxuFrc)


Each box represents a table (e.g., `Loan`, `Account`), and the lines represent foreign key relationships. Beyond the purely technical structure, this layout informs which teams and roles likely interact—loan officers, client service reps, credit risk analysts, etc. For HR, understanding these interdependencies supports effective staffing and workflow management across the bank’s operations.

---

## 2. Customers & Demographics

### 2.1 Clients Distribution by Regions
We start by examining how customers are distributed geographically. **Figure 2** shows client counts or percentages across major Czech regions:

> **Figure 2: Clients distribution per regions**  
> *(Insert `clients_regions.png` or the corresponding image here.)*

- **South Moravia**: ~17% share, the largest portion.  
- **North Moravia**: ~14%.  
- **Prague**: ~12% share but higher average salaries.  
- **South/West Bohemia**: smaller relative shares.

Where larger client bases exist, branches may require **larger or better-trained teams**. In higher-income areas like Prague, staff often need **deep product knowledge** to serve affluent customers (e.g., wealth management, premium services). This informs where HR may focus staff training or targeted recruitment.

---

## 3. Card Products Analysis

### 3.1 Card Products Distribution
**Figure 3** highlights the proportion of **classic**, **junior**, and **gold** cards:

> **Figure 3: Card products distribution**  
> *(Insert `cards_distribution.png` or the corresponding image here.)*

- **Classic Cards**: ~74%  
- **Junior Cards**: ~16%  
- **Gold Cards**: ~10%

Overwhelming popularity of classic suggests that branch and call-center staff mainly handle standard services. However, junior and gold cards cater to distinct niches. If the bank expands gold card promotions in higher-salary districts, staff may need **premium service** and **advanced consultative sales** training. Meanwhile, junior card users (often younger) respond better to **digital experiences** and simpler, fee-conscious features—marketing and frontline staff should adapt accordingly.

---

## 4. Loan Insights

### 4.1 Correlation Among Loan Attributes
**Figure 4** is a correlation heatmap showing `amount`, `duration`, `payments`, and `status_numeric` (bad loans = 1, good loans = -1):

> **Figure 4: Loan correlation heatmap**  
> *(Insert `loan_corr_heatmap.png` or corresponding image.)*

Key observations:
- **Higher monthly payments** correlate with a higher risk of delinquency.  
- **Longer durations** slightly increase chances of unpaid or overdue status.

To mitigate risk, the bank’s **loan officers** and **credit analysts** need robust training and guidelines when evaluating applications with high monthly payments or long durations.

### 4.2 Loan Status by District
**Figure 5** shows **Relative loan status** by district:

> **Figure 5: Relative loans status distributed by districts**  
> *(Insert `loans_by_district_heatmap.png` or corresponding image.)*

Districts with 30%+ problematic loans:
- **Strakonice, Sokolov, Opava, Kutna Hora, Klatovy, Domazlice, Bruntal, Beroun**.

Branches in these areas benefit from more **experienced loan officers** or **specialized risk management** training. HR can recruit and place stronger talent in these high-risk zones, incentivize meticulous review processes, and rotate in staff with proven success in reducing delinquencies.

---

## 5. Transaction Flows & Trends

### 5.1 Collection vs. Remittance Over the Years
We focus on two major categories of external bank transfers:
1. **Collection from another bank** (inflows)  
2. **Remittance to another bank** (outflows)

**Figure 6** shows the yearly trend (1994–1999):

> **Figure 6: Collection from and remittance to another banks (years)**  
> *(Insert `collection_remittance_years.png` or corresponding image.)*

- Inflows outpace outflows, resulting in a net positive by 1998–1999.

**Figure 7** offers a monthly perspective:

> **Figure 7: Collection from and remittance to another banks (months)**  
> *(Insert `collection_remittance_months.png` or corresponding image.)*

Monthly spikes often align with **salary** or **pension** payouts, which may necessitate **flexible staffing schedules** in relevant branches to accommodate surges.

### 5.2 Overall Inflows & Outflows
Beyond interbank transfers, standard deposits and withdrawals drive inflows/outflows. **Figures 8 & 9** compare totals at yearly and monthly intervals:

> **Figure 8: Outflows and inflows trends (years)**  
> *(Insert `inflows_outflows_years.png` or corresponding image.)*  

> **Figure 9: Outflows and inflows trends (months)**  
> *(Insert `inflows_outflows_months.png` or corresponding image.)*  

A net surplus emerges overall. **Figure 10** (daily view) highlights sudden spikes on particular days:

> **Figure 10: Outflows and inflows trends (days)**  
> *(Insert `inflows_outflows_days.png` or corresponding image.)*

To handle these peaks, branches may need **seasonal or surge staffing**. Moreover, as digital payment volumes grow, employees with **IT-liaison** or **e-banking** expertise become more critical.

---

## 6. Key Takeaways with Integrated HR Implications
1. **Customer Base**
   - Even gender split, mostly ages 20–60.  
   - **South/North Moravia**: High client counts; **Prague**: Fewer clients but higher incomes.  
   - Staffing needs may vary—basic service in high-population districts, specialized expertise in wealthier ones.

2. **Card Products**
   - **Classic** dominates (74%), with **Junior** (16%) and **Gold** (10%) trailing.  
   - **Gold** expansions call for **premium sales** training; **Junior** suggests staff adept at marketing to younger demographics.

3. **Loans**
   - **Higher payments** or **long durations** → greater default risks.  
   - Certain districts require strict credit policies and **skilled loan officers**.

4. **Transactions**
   - Inflows > outflows overall.  
   - Regular surges around payroll/pension dates—opportunities for **flexible staffing**.  
   - Digital channels on the rise, implying **IT-savvy staff** or specialized training.

---

## 7. Strategic Recommendations
1. **Upsell Gold & Premium Services**
   - **Finance**: Target high-income clients in Prague or Brno.  
   - **HR**: **Train** existing staff in premium product support, recruit relationship managers with advanced sales skills.

2. **Refine Loan Processes in High-Risk Districts**
   - **Finance**: Tighter underwriting or dynamic credit scoring for known hotspots.  
   - **HR**: Assign or hire **experienced loan officers** in these branches, institute performance incentives to reduce delinquencies.

3. **Utilize Net Surplus for Targeted Growth**
   - **Finance**: Expand new product lines (e.g., advanced e-banking).  
   - **HR**: **Align recruitment** with expansions (IT, data analytics), reskill current employees to handle digital transformations.

4. **Manage Transaction Peaks**
   - **Finance**: Track monthly/seasonal spikes in outflows.  
   - **HR**: **Adjust staffing** around peak days, ensuring customer needs are met without burnout. Foster cross-training so employees can flex between roles.

---

## 8. Conclusion
This comprehensive data analysis blends **financial strategy** with **HR insights**, revealing how to optimize staffing, training, and workflows based on client demographics, card usage, loan risks, and transaction cycles. By combining the bank’s net surplus, region-specific product strategies, and well-prepared teams, the Czech Bank can maintain a competitive edge while nurturing a highly effective workforce.

**Prepared by**:  
_Data & HR Collaboration Team – Merging financial analytics and people strategy for sustainable banking growth._
