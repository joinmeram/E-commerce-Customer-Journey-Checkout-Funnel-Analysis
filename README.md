E-commerce Customer Journey & Checkout Funnel Analysis

Product Analytics Case Study

Tools: SQL, Excel, Python, Power BI, Product AnalyticsProject Type: E-commerce Product Analytics / UX OptimizationData: Synthetic dataset created for portfolio and interview practice

1. Problem Statement

The objective of this case study is to understand where customers drop off during the e-commerce purchase journey and identify product improvements that could increase conversion.

The customer journey analyzed is:

Discovery → Search → Product Detail Page (PDP) → Add to Cart → Checkout → Purchase

The analysis focuses on identifying funnel friction, generating product hypotheses, prioritizing improvements, and defining measurable success criteria.

2. Business Question

Where are customers dropping out of the purchase journey, why might they be dropping out, and which product improvements should be prioritized?

3. Dataset

The synthetic dataset contains:

5,000 unique users

12,000+ customer journey events

Multiple device types

New vs. returning customers

Traffic sources

Product categories

Search behavior

Cart and checkout events

Purchase and revenue information

Main event stages

Stage

Event

Discovery

Discovery

Search

Search

Product Page

PDP_View

Add to Cart

Add_to_Cart

Checkout

Checkout_Start

Purchase

Purchase

4. Funnel Analysis

Stage

Users

Stage Conversion

Drop-off

Discovery

5,000

—

—

Search

3,621

72.42%

27.58%

PDP View

2,729

75.37%

24.63%

Add to Cart

705

25.83%

74.17%

Checkout Start

434

61.56%

38.44%

Purchase

320

73.73%

26.27%

Key finding

The largest funnel bottleneck is:

PDP → Add to Cart

Only 25.83% of PDP visitors add a product to their cart.

This indicates that users are reaching product pages but a large proportion are not sufficiently confident or motivated to proceed with the purchase.

Overall purchase conversion is 6.40%.

5. Product Hypotheses

H1 — Improve PDP Purchase Confidence

Priority: P0

Potential friction areas:

Product information

Price and discount visibility

Reviews and ratings

Delivery information

Trust signals

Add-to-Cart CTA visibility

Proposed solution

Improve the PDP information hierarchy by making important purchase-decision information immediately visible.

Proposed elements:

Clear product title

Rating and review count

Price and discount

Key product benefits

Delivery estimate

Shipping information

Trust signals

Strong Add-to-Cart CTA

Relevant recommendations

H2 — Reduce Cart-to-Checkout Friction

Priority: P1

Only 61.56% of cart users proceed to checkout.

Potential causes include:

Unexpected delivery charges

Coupon complexity

Unclear delivery ETA

Too many interactions before checkout

Proposed solution

Make total cost and delivery information more transparent and reduce unnecessary steps between cart and checkout.

H3 — Improve Paid Search Landing Relevance

Priority: P2

Paid Search shows lower purchase conversion than higher-intent sources such as Email and Direct.

Proposed solution

Improve alignment between:

Search Intent → Landing Page → Product → Recommendation

This can be tested through more relevant category/product landing experiences.

6. Recommended MVP

The first experiment focuses on PDP optimization because PDP → Add to Cart is the largest observed bottleneck.

Proposed PDP improvements

Keep price, discount, rating, and CTA above the fold.

Show delivery ETA near the purchase CTA.

Present 3–5 concise product benefits.

Add trust and return-policy information.

Improve review visibility.

Test a sticky Add-to-Cart CTA on mobile.

Add relevant complementary product recommendations.

7. KPI Framework

Primary KPI

PDP → Add to Cart Conversion

Add-to-Cart Users / PDP Visitors

Secondary KPIs

Purchase Conversion Rate

Cart → Checkout Conversion

PDP CTA Click-Through Rate

Average Order Value

Revenue per Visitor

Guardrail Metrics

Refund / cancellation rate

Customer complaints

Checkout errors

Page load performance

8. Experiment Design

A/B Test

Control: Existing PDP

Treatment: Improved PDP with revised information hierarchy, delivery/trust signals, and improved CTA visibility.

Success criterion

The treatment should increase PDP → Add to Cart conversion without negatively affecting downstream purchase conversion or guardrail metrics.

Results should also be segmented by:

Device

New vs. returning customers

Traffic source

9. User Flow

Discovery
    ↓
Search
    ↓
Product Detail Page
    ↓
Add to Cart
    ↓
Cart
    ↓
Checkout
    ↓
Payment
    ↓
Purchase Success

10. Wireframe Deliverable

The wireframe covers:

Discovery / Homepage

Search Results

Product Detail Page

Add-to-Cart Confirmation

Cart

Checkout

Payment

Order Success

The PDP specifically emphasizes the product information and trust signals required to address the primary funnel bottleneck.

11. Product Decision

Prioritize PDP optimization first.

If the experiment improves PDP → Add to Cart conversion while maintaining downstream purchase conversion and acceptable guardrail metrics, roll out the winning experience.

After that, prioritize Cart → Checkout optimization.

12. Project Files

ecommerce-customer-journey-analysis/
│
├── data/
│   ├── ecommerce_customer_journey_events.csv
│   └── ecommerce_customer_journey_project_data.xlsx
│
├── sql/
│   └── ecommerce_funnel_sql_queries.sql
│
├── analysis/
│   └── ecommerce_funnel_sql_analysis.xlsx
│
├── product/
│   └── ecommerce_product_case_study_prd_hypotheses.docx
│
├── wireframes/
│   └── ecommerce_user_flow_wireframes.png
│
└── README.md
