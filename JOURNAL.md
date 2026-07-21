## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/147

**Issue title:** Resume section detection fails on text with leading whitespace
 #147

**Tier:** [X] Tier 1  [ ] Tier 2  [ ] Tier 3

**Problem summary:**
The bug chosen in the code looks for section headers in resumes. It looks for headers at the start of lines but since some PDF's add spaces before the text of headers (indentation), it incorrectly reads that resumes have no sections. It is an issue with the _detect_sections() portion of resume.py. A successful fix would allow for this whitespace to be detected and acknowledged that an item is still a header without incorrectly assuming all indented text is a header.

**Selection Reasoning:**
I chose this issue because i've never done big codebase changes or fixes like this before and it's within my scope. In college I took some python classes that taught the basics of regex and cleaning data with oddities like whitespaces so I felt this could be a helpful re-hash of those topics to strengthen them while applying them to a real project.

**Branch name:** fix/147-resume-whitespace-detection

**Setup confirmation:** [X] App runs locally at localhost:5173

**Cohort ledger:** [X] Issue added to cohort ledger