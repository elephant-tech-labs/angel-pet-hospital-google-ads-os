# Codex Daily Google Ads QA Prompt

Read these files first:
- MASTER_CONTEXT.md
- CURRENT_STATE.md
- DECISION_RULES.md
- CHANGELOG.md

Then use Google Ads MCP to inspect the live account.

Campaign:
Search - Urgent Vet Care - Edmonds

Do not make edits.

Run a daily QA for the last 24 hours.

Check:
1. Campaign status
2. Budget
3. Bidding
4. Networks
5. Search Partners
6. Display Network
7. AI Max / final URL expansion
8. Final URL
9. Call asset phone number
10. Negative list applied
11. Ad status and disapprovals
12. Spend
13. Impressions
14. Clicks
15. CTR
16. CPC
17. Conversions
18. Search terms with clicks
19. Competitor terms
20. Far-city terms
21. Waste terms
22. Device mix
23. Hour-of-day pattern
24. Location quality

Important context:
Blue Pearl appeared in early search terms and was added as a negative afterward. Do not treat that as a current problem unless it appears again after the negative was applied.

Output format:

A. Executive summary  
B. Access check  
C. What is correct  
D. Critical issues  
E. Search terms to keep/watch/block  
F. Negative keyword recommendations  
G. Do not change list  
H. Next 24-hour action plan  

Rules:
- Do not recommend Target CPA yet.
- Do not recommend Maximize Conversions yet.
- Do not recommend Broad Match.
- Do not recommend Display.
- Do not recommend Search Partners.
- Do not recommend budget increase.
- Do not overreact to tiny data.
- Only recommend immediate changes if there is direct spend leakage or setup mismatch.
