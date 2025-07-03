# Web API Deep Research Template

This template provides a comprehensive research workflow for analyzing web APIs, following industry best practices and leveraging expertise from the Chromium project.

## Research Workflow

### Step 1: API Identification and Selection

**Objective:** Search and identify the most relevant web API

**Process:**
1. Navigate to [MDN Web API Reference](https://developer.mozilla.org/en-US/docs/Web/API)
2. Compare the target API against all available APIs in the reference
3. Select the best-match API based on:
   - Functionality overlap
   - Use case similarity
   - Technical specifications alignment

**Output Template:**
```markdown
## 1. API Identification

**Selected API:** [API Name]
**Reasoning for Selection:** [Brief explanation of why this API was chosen over alternatives]
**Alternative APIs Considered:** [List other APIs that were evaluated]
```

### Step 2: API Overview and Documentation

**Objective:** Provide comprehensive introduction using MDN documentation

**Process:**
1. Extract key information from the API's MDN documentation
2. Summarize core functionality and purpose
3. Include official MDN link

**Output Template:**
```markdown
## 2. API Overview

**API Name:** [Full API Name]
**MDN Documentation:** [Direct link to MDN page]

**Description:**
[Comprehensive description of the API's purpose, functionality, and main use cases]

**Key Features:**
- [Feature 1]
- [Feature 2]
- [Feature 3]

**Primary Use Cases:**
- [Use case 1]
- [Use case 2]
- [Use case 3]
```

### Step 3: Browser Support Analysis

**Objective:** Document current browser support status

**Process:**
1. Extract browser compatibility data from MDN
2. Document support across major browsers
3. Note any significant limitations or partial implementations

**Output Template:**
```markdown
## 3. Browser Support Status

| Browser | Support Status | Version | Notes |
|---------|----------------|---------|-------|
| Chrome | [Full/Partial/None] | [Version] | [Any limitations] |
| Firefox | [Full/Partial/None] | [Version] | [Any limitations] |
| Safari | [Full/Partial/None] | [Version] | [Any limitations] |
| Edge | [Full/Partial/None] | [Version] | [Any limitations] |

**Support Summary:**
[Overall assessment of browser support and any notable patterns]
```

### Step 4: Standards and Specification Research

**Objective:** Locate and analyze official specifications and explainers

**Process:**
1. Search for W3C specifications
2. Look for WHATWG specifications
3. Find any public explainers or proposal documents
4. Check for TC39 proposals (if JavaScript-related)

**Search Queries:**
- "[API Name] specification"
- "[API Name] explainer"
- "[API Name] W3C"
- "[API Name] WHATWG"
- "site:github.com [API Name] explainer"

**Output Template:**
```markdown
## 4. Standards and Specifications

**Official Specification:**
- **Link:** [URL to official spec]
- **Status:** [Working Draft/Candidate Recommendation/etc.]
- **Last Updated:** [Date]

**Explainers and Proposals:**
- **Title:** [Explainer title]
- **Link:** [URL]
- **Summary:** [Brief description of the explainer's content]

**Standards Body:** [W3C/WHATWG/TC39/etc.]
```

### Step 5: GitHub Repository Analysis

**Objective:** Find relevant GitHub repositories and analyze recent activity

**Process:**
1. Search GitHub for repositories related to the API
2. Identify the most active/official repositories
3. Extract the 5 most recent open issues
4. Categorize issues by type (bug, feature request, question, etc.)

**Search Queries:**
- "[API Name] repository"
- "site:github.com [API Name]"
- "[API Name] polyfill"
- "[API Name] implementation"

**Output Template:**
```markdown
## 5. GitHub Repository Analysis

**Primary Repository:**
- **URL:** [Repository URL]
- **Description:** [Repository description]
- **Stars:** [Star count]
- **Last Activity:** [Date]

**Recent Open Issues (Top 5):**

### Issue #1
- **Title:** [Issue title]
- **URL:** [Issue URL]
- **Type:** [Bug/Feature/Question/etc.]
- **Created:** [Date]
- **Summary:** [Brief description]

### Issue #2
- **Title:** [Issue title]
- **URL:** [Issue URL]
- **Type:** [Bug/Feature/Question/etc.]
- **Created:** [Date]
- **Summary:** [Brief description]

[Continue for Issues #3-5]
```

### Step 6: Chromium Bug Tracker Analysis

**Objective:** Identify relevant bugs from Chromium's issue tracker

**Process:**
1. Search [Chromium Bug Tracker](https://issues.chromium.org/issues?q=status:open)
2. Use keywords related to the API
3. Filter by status:open
4. Sort by priority (P0, P1, P2, etc.)
5. Select top 5 bugs based on priority

**Search Queries:**
- `[API Name] status:open`
- `component:[relevant-component] [API Name] status:open`
- `[API Name] type:bug status:open`

**Output Template:**
```markdown
## 6. Chromium Bug Analysis

**Search Query Used:** `[API Name] status:open`

**Top 5 Priority Bugs:**

### Bug #1 (P0/P1/P2)
- **ID:** [Bug ID]
- **URL:** [Chromium bug URL]
- **Title:** [Bug title]
- **Priority:** [P0/P1/P2/P3]
- **Status:** [Open/Assigned/etc.]
- **Component:** [Chromium component]
- **Summary:** [Brief description of the issue]

### Bug #2 (P0/P1/P2)
- **ID:** [Bug ID]
- **URL:** [Chromium bug URL]
- **Title:** [Bug title]
- **Priority:** [P0/P1/P2/P3]
- **Status:** [Open/Assigned/etc.]
- **Component:** [Chromium component]
- **Summary:** [Brief description of the issue]

[Continue for Bugs #3-5]
```

### Step 7: Chromium Implementation Status

**Objective:** Analyze current implementation status in Chromium codebase

**Process:**
1. Search Chromium codebase for API-related files
2. Identify key implementation files
3. Analyze recent commits related to the API
4. Assess implementation completeness

**HaystackSearch Queries:**
- `[API Name]`
- `[API Interface Name]`
- `[API Class Name]`

**Output Template:**
```markdown
## 7. Chromium Implementation Status

**Implementation Overview:**
[Assessment of current implementation status - Complete/Partial/In Progress/Not Started]

**Key Implementation Files:**
- `[file path 1]` - [Description of file's role]
- `[file path 2]` - [Description of file's role]
- `[file path 3]` - [Description of file's role]

**Recent Changes (Last 3):**

### Change #1
- **Date:** [Date]
- **Commit:** [Commit hash/link]
- **Summary:** [Description of change]
- **Impact:** [Effect on API implementation]

### Change #2
- **Date:** [Date]
- **Commit:** [Commit hash/link]
- **Summary:** [Description of change]
- **Impact:** [Effect on API implementation]

### Change #3
- **Date:** [Date]
- **Commit:** [Commit hash/link]
- **Summary:** [Description of change]
- **Impact:** [Effect on API implementation]

**Current Limitations:**
- [Limitation 1]
- [Limitation 2]
- [Limitation 3]
```

### Step 8: Edge Implementation Status

**Objective:** Analyze current implementation status in Edge codebase

**Process:**
1. Search Edge-specific directories for API implementations
2. Look for Edge-specific customizations or patches
3. Identify any Edge-unique features or limitations
4. Analyze recent Edge-specific changes

**HaystackSearch Queries:**
- `[API Name] path:edge_*`
- `[API Name] path:microsoft_*`
- Edge-specific implementation patterns

**Output Template:**
```markdown
## 8. Edge Implementation Status

**Edge-Specific Implementation:**
[Assessment of Edge's implementation - Same as Chromium/Extended/Modified/etc.]

**Edge-Specific Files:**
- `[edge file path 1]` - [Description of Edge-specific functionality]
- `[edge file path 2]` - [Description of Edge-specific functionality]

**Edge Customizations:**
- [Customization 1]
- [Customization 2]
- [Customization 3]

**Recent Edge Changes (Last 3):**

### Change #1
- **Date:** [Date]
- **File(s):** [Changed files]
- **Summary:** [Description of change]
- **Edge Impact:** [Specific impact on Edge functionality]

### Change #2
- **Date:** [Date]
- **File(s):** [Changed files]
- **Summary:** [Description of change]
- **Edge Impact:** [Specific impact on Edge functionality]

### Change #3
- **Date:** [Date]
- **File(s):** [Changed files]
- **Summary:** [Description of change]
- **Edge Impact:** [Specific impact on Edge functionality]

**Edge-Specific Considerations:**
- [Consideration 1]
- [Consideration 2]
- [Consideration 3]
```

### Step 9: Future Evolution Prediction

**Objective:** Provide informed predictions about API evolution

**Process:**
1. Analyze current standards activity
2. Review open issues and proposals
3. Consider industry trends
4. Assess implementation gaps
5. Make informed predictions based on available data

**Output Template:**
```markdown
## 9. Future Evolution Prediction

**Standards Trajectory:**
[Analysis of where the standard is heading based on current activity]

**Implementation Trends:**
[Patterns observed in browser implementations]

**Key Areas for Evolution:**

### Near-term (6-12 months)
- [Prediction 1 with reasoning]
- [Prediction 2 with reasoning]
- [Prediction 3 with reasoning]

### Medium-term (1-2 years)
- [Prediction 1 with reasoning]
- [Prediction 2 with reasoning]
- [Prediction 3 with reasoning]

### Long-term (2+ years)
- [Prediction 1 with reasoning]
- [Prediction 2 with reasoning]
- [Prediction 3 with reasoning]

**Potential Challenges:**
- [Challenge 1]
- [Challenge 2]
- [Challenge 3]

**Opportunities:**
- [Opportunity 1]
- [Opportunity 2]
- [Opportunity 3]

**Recommendation for Edge:**
[Specific recommendations for Edge team based on analysis]
```

## Research Best Practices

### Search Strategy
1. **Use Multiple Sources:** Don't rely on a single source; cross-reference information
2. **Version-Specific Search:** Include version numbers when searching for browser-specific information
3. **Component-Specific Search:** Use Chromium component names for more targeted searches
4. **Date Filtering:** Prioritize recent information when assessing current status

### Quality Assurance
1. **Verify URLs:** Ensure all links are accessible and point to correct resources
2. **Cross-Reference Data:** Validate information across multiple sources
3. **Update Timestamps:** Include when the research was conducted
4. **Source Attribution:** Clearly cite all sources and their access dates

### Documentation Standards
1. **Clear Structure:** Follow the template structure consistently
2. **Concise Summaries:** Provide brief but comprehensive summaries
3. **Actionable Insights:** Focus on information that can inform development decisions
4. **Regular Updates:** Plan for periodic research updates as APIs evolve

## Example Usage

To use this template:

1. **Create a new markdown file** named `[api-name]_research_[date].md`
2. **Follow each step** in the workflow sequentially
3. **Fill in the output templates** with your research findings
4. **Review and validate** all information before finalizing
5. **Share with relevant teams** for review and action planning

## Research Tools and Resources

### Primary Resources
- [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/API)
- [Chromium Bug Tracker](https://issues.chromium.org/)
- [W3C Specifications](https://www.w3.org/TR/)
- [WHATWG Standards](https://spec.whatwg.org/)
- [GitHub](https://github.com/)

### Search Tools
- HaystackSearch (for Edge/Chromium codebase)
- GitHub Advanced Search
- Google Search with site-specific operators
- Chromium Code Search

### Tracking Tools
- Browser compatibility tables
- Can I Use (caniuse.com)
- Web Platform Status trackers
- Standards position trackers

---

**Note:** This template is designed for experienced engineers familiar with web platform development. Adapt the depth and focus of research based on the specific API and current project needs.
