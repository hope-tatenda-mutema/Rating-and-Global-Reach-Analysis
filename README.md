# Netflix Global Distribution Strategy Analysis
### Statistical Independence Testing: Movie Ratings vs. Global Availability

---

## Business Context

In the competitive streaming media landscape, content distribution decisions require data-driven insights. Netflix and similar platforms face a critical strategic question: **Should high-quality content be prioritized for global distribution, or do other factors determine international availability?**

This analysis addresses a fundamental business question for streaming platforms, content producers, and media distributors:

> **Does a movie's rating influence its likelihood of global distribution on Netflix?**

Understanding this relationship informs:
- **Content acquisition strategies** for international markets
- **Distribution investment decisions** based on quality metrics
- **Performance expectations** for globally vs. regionally distributed content
- **Resource allocation** for marketing and localization efforts

---

## Executive Summary

**Key Finding**: While a statistically significant relationship exists between movie ratings and global availability (χ² = 14.06, p < 0.01), the practical effect is negligible (Cramér's V = 0.0277).

**Business Implication**: Global distribution decisions are driven primarily by factors other than ratings—likely including licensing costs, regional demand, content rights, and strategic partnerships rather than quality scores alone.

**Strategic Recommendation**: Stakeholders should focus on content quality and audience engagement strategies rather than assuming wider distribution automatically correlates with higher ratings or vice versa.

---

## Problem Statement

### Research Question
Is there a significant association between Netflix movie ratings and their global availability?

### Hypotheses

**Null Hypothesis (H₀)**: Movie ratings and global availability are independent—there is no significant relationship between a movie's rating and whether it is available globally.

**Alternative Hypothesis (Hₐ)**: Movie ratings and global availability are dependent—a movie's rating significantly influences its global distribution status.

### Business Stakes
- **If H₀ is true**: Distribution decisions are unrelated to quality metrics; focus should shift to other strategic factors
- **If Hₐ is true**: Quality-driven distribution strategies may be justified; higher-rated content should receive priority for global rollout

---

## Methodology

### Data Source
- **Dataset**: Netflix 2023 Movie Catalog (n = 18,328)
- **Analysis Type**: Chi-Square Test for Independence
- **Significance Level**: α = 0.01 (conservative threshold given large sample size)

### Variables

| Variable | Type | Categories | Role |
|----------|------|------------|------|
| **Movie Rating** | Ordinal Categorical | Poor (0-5), Below Average (5-7), Above Average (7-8.5), Excellent (8.5-10) | Dependent |
| **Global Availability** | Binary Categorical | Yes, No | Independent |

### Rating Classification Rationale

The rating scale was constructed based on industry standards from IMDB and similar platforms:

- **Poor (0-5)**: Below acceptable quality threshold
- **Below Average (5-7)**: Watchable but unremarkable
- **Above Average (7-8.5)**: Quality content worth recommending
- **Excellent (8.5-10)**: Premium content; critical acclaim

---

## Analysis Workflow

The analysis followed a systematic four-phase approach designed to move from raw data to actionable business insights.

**Phase 1: Data Preparation**

The Netflix 2023 dataset was imported and prepared for analysis. Ratings were converted to numeric format and missing values were removed to ensure data integrity. The global availability variable was filtered to include only binary Yes/No responses, eliminating ambiguous cases. The numeric ratings were then recoded into four meaningful ordinal categories based on industry standards from IMDB and similar platforms. This process resulted in a clean analytical dataset of 18,328 movies.

**Phase 2: Exploratory Analysis**

With clean data in hand, the exploratory phase examined the distribution of movies across rating categories and global availability status. Frequency tables revealed the proportion of movies in each rating group, while contingency tables (cross-tabulations) showed how ratings and global availability intersected. Row and column percentages were calculated to understand relative distributions, providing the foundation for statistical testing.

**Phase 3: Statistical Testing**

The Chi-Square Test for Independence served as the primary analytical tool. The test statistic was calculated based on observed versus expected frequencies in the contingency table. With three degrees of freedom (four rating groups minus one), the p-value was computed and compared against the stringent significance level of 0.01. Beyond the basic significance test, two layers of effect size analysis were conducted: unstandardized effects examining raw percentage differences across categories, and Cramér's V providing a standardized measure of association strength. Finally, power analysis evaluated the probability of Type II errors, assessing whether the study had sufficient statistical power to detect real relationships.

**Phase 4: Interpretation & Reporting**

The final phase synthesized statistical findings into business intelligence. Statistical significance was assessed in the context of practical significance, recognizing that p-values alone don't tell the complete story. The negligible effect size revealed that while the relationship was statistically detectable, it held minimal practical importance for distribution strategy. These insights were translated into concrete recommendations for streaming platforms, content producers, and media consultants.

---

## Results

### Statistical Test Results

**Chi-Square Test for Independence:**
- χ²(3, n = 18,328) = 14.06
- p-value = 0.0028
- Critical value at α = 0.01: Significant

**Decision**: Reject H₀ at the 0.01 significance level

**Statistical Conclusion**: There is a statistically significant relationship between movie rating groups and global availability on Netflix.

---

### Effect Size Analysis

#### Unstandardized Effects (Percentage Differences)

Examining the distribution of globally available vs. non-globally available movies across rating categories:

| Rating Group | Available Globally (%) | Not Available Globally (%) | Absolute Difference |
|--------------|----------------------|--------------------------|-------------------|
| Poor | — | — | 1.9% (largest gap) |
| Below Average | — | — | <1% |
| Above Average | — | — | <1% |
| Excellent | — | — | <1% |

**Interpretation**: Percentage differences are minimal across all rating groups, indicating weak practical distinction.

#### Standardized Effect: Cramér's V

**Cramér's V = 0.0277**

**Effect Size Classification:**
- 0.00 - 0.10: Negligible
- 0.10 - 0.30: Weak
- 0.30 - 0.50: Moderate
- 0.50+: Strong

**Interpretation**: The observed effect size of 0.0277 is **negligible**, indicating that while the relationship is statistically detectable, it has minimal practical importance for business decisions.

---

### Power Analysis

**Statistical Power = 0.7474 (74.74%)**

**Type II Error Risk (β) = 0.2526 (25.26%)**

**Interpretation**:
- There is a 74.74% probability of correctly detecting a true relationship if one exists
- There remains a 25.26% chance of failing to detect a real association (false negative)
- The moderate power level is partly driven by the conservative α = 0.01 threshold
- Given the large sample size (n = 18,328), the moderate power suggests the true effect is indeed small

---

## Business Insights

### The Paradox: Significant but Negligible

This analysis reveals a common statistical phenomenon: **statistical significance without practical significance**.

**What the statistics say:**
- ✓ The relationship is real (p < 0.01)
- ✓ The test has adequate power (74.74%)
- ✗ The effect size is negligible (V = 0.0277)

**What this means for business:**

1. **Global availability is not primarily driven by ratings**
   - High-rated movies are not substantially more likely to be globally available
   - Low-rated movies are not systematically excluded from global distribution

2. **Other factors dominate distribution decisions**
   - Licensing and rights agreements
   - Regional content demand and cultural fit
   - Production costs and ROI projections
   - Strategic partnerships and exclusive deals
   - Content localization requirements

3. **Quality matters, but not for distribution decisions**
   - Ratings likely influence viewer engagement and retention
   - Distribution decisions operate on different strategic criteria

---

## Strategic Recommendations

### For Streaming Platforms (Netflix, etc.)

**1. Decouple Quality from Distribution Strategy**
- Recognize that distribution decisions require multi-factor analysis beyond ratings
- Develop separate frameworks for content quality assessment and distribution planning

**2. Focus on Region-Specific Demand Signals**
- Use predictive analytics for regional content preferences
- Prioritize audience demand data over universal quality metrics

**3. Optimize for Engagement, Not Just Ratings**
- High ratings don't guarantee global distribution success
- Focus on watch time, completion rates, and subscriber retention

### For Content Producers

**1. Don't Assume Global = Higher Quality**
- Global availability reflects strategic decisions, not quality validation
- Regional success can be equally valuable

**2. Understand Distribution Criteria Beyond Ratings**
- Build relationships with content buyers
- Understand licensing, rights, and strategic fit
- Focus on unique value propositions for specific markets

### For Media Consultants

**1. Advise Clients on Realistic Distribution Expectations**
- High ratings ≠ automatic global distribution
- Prepare clients for multi-dimensional negotiation factors

**2. Develop Holistic Distribution Strategies**
- Combine quality improvement with strategic positioning
- Address licensing, localization, and market-specific factors

---

## Technical Specifications

### Statistical Methods
- **Primary Test**: Pearson's Chi-Square Test for Independence
- **Effect Size**: Cramér's V
- **Power Analysis**: Post-hoc power calculation
- **Software**: R (version 4.x)

### R Packages Used
```r
library(summarytools)  # Cross-tabulation and descriptive statistics
library(DescTools)     # Cramér's V calculation
library(pwr)          # Statistical power analysis
```

### Sample Characteristics
- **Total Sample Size**: n = 18,328
- **Degrees of Freedom**: df = 3
- **Contingency Table**: 2 (Global Availability) × 4 (Rating Groups)

---

## Limitations & Considerations

### Statistical Limitations

1. **Large Sample Size Sensitivity**
   - With n = 18,328, even tiny effects become statistically significant
   - P-values must be interpreted alongside effect sizes

2. **Binary Independent Variable**
   - Only two categories (Yes/No) limit analytical depth
   - More granular availability data (e.g., number of countries) could reveal nuanced patterns

3. **Observational Data**
   - Correlation does not imply causation
   - Unmeasured confounding variables may influence both ratings and distribution

### Business Limitations

1. **Temporal Dynamics**
   - Analysis uses 2023 snapshot data
   - Distribution strategies may evolve over time

2. **Platform-Specific Findings**
   - Results are specific to Netflix
   - Other platforms may have different distribution logic

3. **Excluded Variables**
   - Content genre, production budget, star power, and marketing spend not considered
   - These factors likely have stronger influence than ratings alone

---

## Reproducibility

### Data Requirements
- Netflix 2023 movie catalog with rating and global availability variables
- Minimum sample size: n > 1,000 for adequate statistical power

### Analysis Steps
1. Clone this repository
2. Install required R packages:
   ```r
   install.packages(c("summarytools", "DescTools", "pwr"))
   ```
3. Run the Quarto document:
   ```r
   quarto::quarto_render("Test_for_independence.qmd")
   ```

### Project Files

The analysis is contained in three primary files: the main analysis document (Test_for_independence.qmd) containing all statistical code and interpretation, an executive memo (Memo.docx) summarizing findings for leadership, and this README providing comprehensive documentation and business context.

---

## Conclusions

### Statistical Verdict
The Chi-Square test confirms a statistically significant relationship between Netflix movie ratings and global availability (p < 0.01). However, the Cramér's V effect size of 0.0277 reveals this relationship is practically negligible.

### Business Verdict
**Global distribution decisions on Netflix are not primarily driven by movie ratings.** Strategic factors such as licensing agreements, regional demand, content rights, and platform partnerships play a far more substantial role than quality metrics alone.

### Actionable Insight
Stakeholders should **focus resources on understanding and optimizing for the true drivers of distribution success**—regional audience preferences, strategic partnerships, licensing efficiency, and engagement metrics—rather than assuming rating quality automatically translates to distribution opportunity.

---

## Author

**Hope Tatenda Mutema**

*Statistical Analyst | Data-Driven Strategy Consultant*

**Prepared For**: Managing Partner, Media & Entertainment Strategy Division

---

## Appendix: Statistical Formulas

### Chi-Square Test Statistic
$$\chi^2 = \sum \frac{(O_i - E_i)^2}{E_i}$$

Where:
- O<sub>i</sub> = Observed frequency
- E<sub>i</sub> = Expected frequency

### Cramér's V
$$V = \sqrt{\frac{\chi^2}{n(k-1)}}$$

Where:
- χ² = Chi-square statistic
- n = Sample size
- k = Minimum of (rows, columns)

### Statistical Power
$$\text{Power} = 1 - \beta = P(\text{Reject } H_0 | H_A \text{ is true})$$

---

## References

1. Agresti, A. (2018). *Statistical Methods for the Social Sciences* (5th ed.). Pearson.
2. Cohen, J. (1988). *Statistical Power Analysis for the Behavioral Sciences* (2nd ed.). Routledge.
3. Field, A., Miles, J., & Field, Z. (2012). *Discovering Statistics Using R*. SAGE Publications.

---

## License

This analysis is available for educational and research purposes.

---

**For questions or collaboration opportunities, please open an issue in this repository.**

---

*Analysis completed: 2024 | Dataset: Netflix 2023*
