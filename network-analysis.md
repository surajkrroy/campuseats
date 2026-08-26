# Network Analysis

## Website Tested

Google search results page for the query `instamart`.

## Network DevTools Setup

- Browser DevTools: Chrome
- Panel used: Network
- `Disable cache`: enabled
- Page was reloaded with the Network panel open.

## Results

### 1. Request Count

**134 requests**

### 2. Total Page Size

**11.6 MB resources**

The Network panel also showed **4.1 MB transferred**. The 11.6 MB value is the total resources value displayed by DevTools.

### 3. Single Slowest Resource

The Network panel was sorted by the `Time` column with the largest time first.

- Resource: `gen_204?...`
- Status: `204`
- Type: `ping`
- Time: **4.37 s**

Therefore, the slowest resource observed was the `gen_204?...` ping request, which took 4.37 seconds.

### 4. 3xx/4xx Responses

No 3xx or 4xx status codes were visible in the captured Network panel.

The visible `204` responses are **2xx successful responses**, not 3xx/4xx errors.

## Summary

| Item | Result |
|---|---|
| Request count | 134 |
| Total resources | 11.6 MB |
| Transferred | 4.1 MB |
| Slowest resource | `gen_204?...` |
| Slowest time | 4.37 s |
| 3xx/4xx responses visible | None |
