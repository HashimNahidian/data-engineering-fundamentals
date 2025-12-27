# Slowly Changing Dimensions (SCD)

Slowly Changing Dimensions (SCD) describe how changes to dimension data are managed over time in a data warehouse. Different SCD types represent different strategies for handling historical data.

---

## SCD Type 0 – Retain Original Value
- No changes are allowed
- Original data is preserved permanently

**Use case:**  
Immutable attributes such as date of birth or initial signup date.

---

## SCD Type 1 – Overwrite
- Old data is overwritten with new values
- No historical tracking

**Pros:**
- Simple to implement
- Requires minimal storage

**Cons:**
- Loss of historical data

**Use case:**  
Correcting data errors or updating non-historical attributes.

---

## SCD Type 2 – Full History Tracking
- New row created for each change
- Historical records preserved
- Uses effective dates or version numbers

**Pros:**
- Complete history tracking
- Most commonly used in analytics

**Cons:**
- Increased storage requirements

**Use case:**  
Tracking customer address changes or job title history.

---

## SCD Type 3 – Limited History
- Adds new columns to store previous values
- Tracks limited history only

**Pros:**
- Simple historical comparison
- Minimal storage overhead

**Cons:**
- Limited to a fixed number of changes

**Use case:**  
Tracking current and previous status values.

---

## Summary

| SCD Type | History Tracked | Storage Impact | Common Use |
|--------|----------------|----------------|------------|
| Type 0 | None | Low | Immutable data |
| Type 1 | None | Low | Corrections |
| Type 2 | Full | High | Analytics |
| Type 3 | Limited | Medium | Status tracking |

Understanding SCD strategies is critical for designing accurate and reliable analytical data models.
