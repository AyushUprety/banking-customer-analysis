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
> ![Database Schema](https://private-user-images.githubusercontent.com/50670035/401802017-88e46b70-5a4c-40c8-a1dd-93aa5404b122.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDIwMTctODhlNDZiNzAtNWE0Yy00MGM4LWExZGQtOTNhYTU0MDRiMTIyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWYwN2VkZjYxZjJiMDZiNzEyYzZjNDcyNDBlZTgxYzg1ZjA5MDBiMjE0ZTZmNTlkMGM3OTJlMmU4NjM2YTk0ZjEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.QOxf_-AvYE-AnDV2r5P2fVNqLGmoO6rSxFLYmoxuFrc)


Each box represents a table (e.g., `Loan`, `Account`), and the lines represent foreign key relationships. Beyond the purely technical structure, this layout informs which teams and roles likely interact—loan officers, client service reps, credit risk analysts, etc. For HR, understanding these interdependencies supports effective staffing and workflow management across the bank’s operations.

---

## 2. Customers & Demographics

### 2.1 Clients Distribution by Regions
We start by examining how customers are distributed geographically. **Figure 2** shows client counts or percentages across major Czech regions:

> **Figure 2: Clients distribution per regions**  
> ![Clients Distribution by Regions](https://private-user-images.githubusercontent.com/50670035/401802116-01046f30-93c1-4f61-91b8-70788e51ca00.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDIxMTYtMDEwNDZmMzAtOTNjMS00ZjYxLTkxYjgtNzA3ODhlNTFjYTAwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWZhMzg5MjFlNTVhYzEwNWEyNTQ2NjNmZTJlMGZiZTc0NzFjOGEzYWJiODljOGY3MTVjZDI5ZmZkNzA4NTNiODgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.9t63skrvZFl4i57uNFWLFZ9KgXUj-fJmy7b2awYGmOo)

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
> ![Card products distribution](https://private-user-images.githubusercontent.com/50670035/401802157-fe48c46f-b0bb-4765-ae6c-51b4f85993c4.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDIxNTctZmU0OGM0NmYtYjBiYi00NzY1LWFlNmMtNTFiNGY4NTk5M2M0LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTU0N2Y0ZmQwMDI2ZTk0NGM4MDA5M2FkMTVmOTFjZjYwNGRhZDU3OGJhNmMyYmQwZDc4ZTQ3ZDhlNzNmMjlkYjkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.Z4Yxty74bLIz_Ljn5W4Xy0rr8OegIVa6RDFNPanN2Vs)

- **Classic Cards**: ~74%  
- **Junior Cards**: ~16%  
- **Gold Cards**: ~10%

Overwhelming popularity of classic suggests that branch and call-center staff mainly handle standard services. However, junior and gold cards cater to distinct niches. If the bank expands gold card promotions in higher-salary districts, staff may need **premium service** and **advanced consultative sales** training. Meanwhile, junior card users (often younger) respond better to **digital experiences** and simpler, fee-conscious features—marketing and frontline staff should adapt accordingly.

---

## 4. Loan Insights

### 4.1 Correlation Among Loan Attributes
**Figure 4** is a correlation heatmap showing `amount`, `duration`, `payments`, and `status_numeric` (bad loans = 1, good loans = -1):

> **Figure 4: Loan correlation heatmap**  
> ![Loan correlation heatmap](https://private-user-images.githubusercontent.com/50670035/401802198-6a19329a-ed27-480d-baf6-7c9eb5919b4d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDIxOTgtNmExOTMyOWEtZWQyNy00ODBkLWJhZjYtN2M5ZWI1OTE5YjRkLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTcyM2Q1NmFmMTg3NGZhMzhlOWM3YWViMWU0MWY4MDg2MGE4NjlhZDBlZmFlYTk0N2FlZjAzNTQ4YmQ3YTEyZDkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.Y6GlY06DtkhtMvZFQ7kNkKoun0MZ0NQ3WDIxIH4PrPQ)

Key observations:
- **Higher monthly payments** correlate with a higher risk of delinquency.  
- **Longer durations** slightly increase chances of unpaid or overdue status.

To mitigate risk, the bank’s **loan officers** and **credit analysts** need robust training and guidelines when evaluating applications with high monthly payments or long durations.

### 4.2 Loan Status by District
**Figure 5** shows **Relative loan status** by district:

> **Figure 5: Relative loans status distributed by districts**  
> *![image](https://private-user-images.githubusercontent.com/50670035/401802241-b0c26133-0fb8-49bc-aaed-90d6569a7932.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDIyNDEtYjBjMjYxMzMtMGZiOC00OWJjLWFhZWQtOTBkNjU2OWE3OTMyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTkxNzA2YTc3MDNmYTcxN2QyNjUyNmQ3NjUzNjc3ZDFjMDExMGMyYTVjMTViMzhkYjE4ODkzYzhkZmUyYWY3MzkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.K1AqFqfFP6yy_QZedSNSwrzdRRJl44xeSUErRI9F-gk)
)*

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
>![](https://private-user-images.githubusercontent.com/50670035/401802347-311fd934-488d-449b-ab2b-5e8b0186cbe8.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDIzNDctMzExZmQ5MzQtNDg4ZC00NDliLWFiMmItNWU4YjAxODZjYmU4LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQwNGJlNDVkNWM2NzMyMmZiZmE1YjIyMDYyZmZlMmJhMzc1NzcyMjJiY2VlZDkxNTQ3YjM2NGRlYzQ4OTAwMDEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.vDtSEDTn7lS8zPoF_iuNyVno-jcgWENfJUveZOY8Zlc)

- Inflows outpace outflows, resulting in a net positive by 1998–1999.

**Figure 7** offers a monthly perspective:

> **Figure 7: Collection from and remittance to another banks (months)**  
> ![](https://private-user-images.githubusercontent.com/50670035/401802374-c9a05f98-bf62-428d-9b1d-25344ed4b6d2.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDIzNzQtYzlhMDVmOTgtYmY2Mi00MjhkLTliMWQtMjUzNDRlZDRiNmQyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBiOGEzYmZhOGJiNTJhMTQ3NmE1NWI0MzEwZDYxM2U1ZTRkMTk0YWViMDNiMzI2MGE2NjNmZjY4ZTlkNWIxYmEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.J5yFYGPLHqiVeMAtq8KGSulSxk_YKqMTbd0j7F4DBaQ)

Monthly spikes often align with **salary** or **pension** payouts, which may necessitate **flexible staffing schedules** in relevant branches to accommodate surges.

### 5.2 Overall Inflows & Outflows
Beyond interbank transfers, standard deposits and withdrawals drive inflows/outflows. **Figures 8 & 9** compare totals at yearly and monthly intervals:

> **Figure 8: Outflows and inflows trends (years)**  
> [](https://private-user-images.githubusercontent.com/50670035/401802413-8ab4bb8b-167e-4f1a-904a-17586bf0ce28.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDI0MTMtOGFiNGJiOGItMTY3ZS00ZjFhLTkwNGEtMTc1ODZiZjBjZTI4LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWIyOWJjYmQxZjJjZTVkMDVlN2M0YWNlOTU4MmNhN2E5MjViMDc0NWZmOWFlZjU0OGFkMjdhOWU0ZTg2NjMxNDQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.fGj6lfHcGRZExDQhy6OQ6EV1WcamQHClvBRU8Cq-Jg0))*  

> **Figure 9: Outflows and inflows trends (months)**  
> ![](https://private-user-images.githubusercontent.com/50670035/401802443-6a85629d-5abc-428e-8d9e-895f2d273651.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDI0NDMtNmE4NTYyOWQtNWFiYy00MjhlLThkOWUtODk1ZjJkMjczNjUxLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTFjYjU3ODU4ZjZmNjM5NGRjZDgyNTMzZWE0ZTdmZTEwNDZhMjUyMzY5OTljMzEzNzI2MmI0ZjBjZmY0MTk4MGUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.USSCnec42zCGI0oSWv8tcquwPeoKLaqtvtkQ9ZRWNb4)  

A net surplus emerges overall. **Figure 10** (daily view) highlights sudden spikes on particular days:

> **Figure 10: Outflows and inflows trends (days)**  
> ![](https://private-user-images.githubusercontent.com/50670035/401802466-736ee244-f97b-4d72-90a4-d28eb08c1097.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzY0ODEzNTMsIm5iZiI6MTczNjQ4MTA1MywicGF0aCI6Ii81MDY3MDAzNS80MDE4MDI0NjYtNzM2ZWUyNDQtZjk3Yi00ZDcyLTkwYTQtZDI4ZWIwOGMxMDk3LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTEwVDAzNTA1M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTRiN2ZjN2U0ZGUxOTBkNmZjM2ZlNmI1NGE2YTllOTZlODcyZmNjZTYzNmYxNmRlNWJhODY0NWE4MGJmYTAyMTQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.9jswyqemC4wHQdx46PrWivg99eF1DfcbAq3CfOQbRMg)*

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
