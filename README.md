# E-commerce Customer Journey & Checkout Funnel Analysis

## Product Analytics Case Study

**Tools:** SQL, Excel, Python, Power BI, Product Analytics  
**Project Type:** E-commerce Product Analytics / UX Optimization  
**Data:** Synthetic dataset created for portfolio and interview practice

---

## 1. Problem Statement

The objective of this case study is to understand where customers drop off during the e-commerce purchase journey and identify product improvements that could increase conversion.

The customer journey analyzed is:

**Discovery → Search → Product Detail Page (PDP) → Add to Cart → Checkout → Purchase**

The analysis focuses on identifying funnel friction, generating product hypotheses, prioritizing improvements, and defining measurable success criteria.

---

## 2. Business Question

> Where are customers dropping out of the purchase journey, why might they be dropping out, and which product improvements should be prioritized?

---

## 3. Dataset

The synthetic dataset contains:

- 5,000 unique users
- 12,000+ customer journey events
- Multiple device types
- New vs. returning customers
- Traffic sources
- Product categories
- Search behavior
- Cart and checkout events
- Purchase and revenue information

### Main Event Stages

| Stage | Event |
|---|---|
| Discovery | `Discovery` |
| Search | `Search` |
| Product Page | `PDP_View` |
| Add to Cart | `Add_to_Cart` |
| Checkout | `Checkout_Start` |
| Purchase | `Purchase` |

---

## 4. Funnel Analysis

| Stage | Users | Stage Conversion | Drop-off |
|---|---:|---:|---:|
| Discovery | 5,000 | — | — |
| Search | 3,621 | 72.42% | 27.58% |
| PDP View | 2,729 | 75.37% | 24.63% |
| Add to Cart | 705 | 25.83% | 74.17% |
| Checkout Start | 434 | 61.56% | 38.44% |
| Purchase | 320 | 73.73% | 26.27% |

### Key Finding

The largest funnel bottleneck is:

**PDP → Add to Cart**

Only **25.83%** of PDP visitors add a product to their cart.

This indicates that users are reaching product pages but a large proportion are not sufficiently confident or motivated to proceed with the purchase.

Overall purchase conversion is **6.40%**.

---

## 5. Product Hypotheses

### H1 — Improve PDP Purchase Confidence

**Priority:** P0

Potential friction areas:

- Product information
- Price and discount visibility
- Reviews and ratings
- Delivery information
- Trust signals
- Add-to-Cart CTA visibility

### Proposed Solution

Improve the PDP information hierarchy by making important purchase-decision information immediately visible.

Proposed elements:

- Clear product title
- Rating and review count
- Price and discount
- Key product benefits
- Delivery estimate
- Shipping information
- Trust signals
- Strong Add-to-Cart CTA
- Relevant recommendations

---

### H2 — Reduce Cart-to-Checkout Friction

**Priority:** P1

Only **61.56%** of cart users proceed to checkout.

Potential causes include:

- Unexpected delivery charges
- Coupon complexity
- Unclear delivery ETA
- Too many interactions before checkout

### Proposed Solution

Make total cost and delivery information more transparent and reduce unnecessary steps between cart and checkout.

---

### H3 — Improve Paid Search Landing Relevance

**Priority:** P2

Paid Search shows lower purchase conversion than higher-intent sources such as Email and Direct.

### Proposed Solution

Improve alignment between:

**Search Intent → Landing Page → Product → Recommendation**

This can be tested through more relevant category/product landing experiences.

---

## 6. Recommended MVP

The first experiment focuses on **PDP optimization** because PDP → Add to Cart is the largest observed bottleneck.

### Proposed PDP Improvements

1. Keep price, discount, rating, and CTA above the fold.
2. Show delivery ETA near the purchase CTA.
3. Present 3–5 concise product benefits.
4. Add trust and return-policy information.
5. Improve review visibility.
6. Test a sticky Add-to-Cart CTA on mobile.
7. Add relevant complementary product recommendations.

---

## 7. KPI Framework

### Primary KPI

**PDP → Add to Cart Conversion**

```text
Add-to-Cart Users / PDP Visitors
