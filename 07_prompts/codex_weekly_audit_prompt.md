# Codex Weekly Google Ads Audit Prompt

Read these files first:
- MASTER_CONTEXT.md
- CURRENT_STATE.md
- DECISION_RULES.md
- CHANGELOG.md
- 01_strategy/account_strategy.md

Then use Google Ads MCP to audit the live account.

Do not make edits.

Date range:
Last 7 days.

Campaigns:
All active Google Ads campaigns for Angel Pet Hospital.

Audit:
1. Spend
2. Impressions
3. Clicks
4. CTR
5. CPC
6. Conversions
7. Cost per conversion
8. Search terms
9. Keyword performance
10. Negative keyword gaps
11. Location quality
12. Device quality
13. Hour/day performance
14. Ad copy and asset status
15. Landing page/final URL alignment
16. Conversion tracking quality
17. Recommendations from Google Ads that should be ignored or considered

Classify every recommendation as:
- Implement now
- Watch
- Delay
- Reject
- Needs human decision

Important rules:
- Do not recommend Target CPA unless conversion tracking is clean.
- Do not recommend Broad Match in early phase.
- Do not recommend Performance Max until Search campaigns have proven lead quality.
- Do not recommend Display or Search Partners during stabilization.
- Do not recommend increasing budget without lead-quality evidence.

Output format:

A. Executive verdict  
B. What is working  
C. What is wasting spend  
D. Search term findings  
E. Keyword decisions  
F. Negative keyword recommendations  
G. Conversion tracking verdict  
H. Landing page / CTA findings  
I. Approved next-step recommendations  
J. What not to change  
K. Next 7-day plan  
