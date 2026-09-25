# Gate4C to final confirmation

All comparisons pair predicted and measured pose at eligible 50-Hz blocks and apply the same frozen downstream consumer. Statistical confirmation uses **users**, not blocks, as the independent units. Flip is consumer-output disagreement; hard preservation is one minus ordinary Flip. Class-balanced risk averages supported measured-pose reference classes. Continuous Fisher-space error and probability total variation are different endpoints.

| Stage | Frozen population and target | Observed aggregate result | Interpretation |
|---|---|---|---|
| Gate4C | 27 users, 926 files; 19 development, eight validation | Validation median hard preservation 0.6571 (IQR 0.5533–0.7042; range 0.1632–0.7592); balanced preservation 0.3331; probability TV 0.2260 | Descriptive heterogeneity; no preregistered pass threshold or semantic labels |
| Gate4D | 19 development users, 654 files; continuous Fisher-space error | Median user error 2.012 at full coverage to 1.624 at 30%; 18/19 improved | Development evidence for a continuous endpoint, not final Flip confirmation |
| Gate4E Requirement-U | Development selection, then frozen ordinary usage-weighted Flip contract | Development median ordinary risk 0.4034 to 0.1775 at 30%; 19/19 lower | Development result only; class-balanced secondary preservation fell |
| Gate4F Requirement-B | Development selection, then frozen class-balanced Flip contract | Development median balanced risk 0.6816 to 0.5066 at 30%; 19/19 lower | Development result only; ordinary secondary risk rose |
| Final joint confirmation | 20 CommonPose-development-untouched users, 702 files; fixed 30% within-user acceptance | E paired median ordinary-risk improvement 17.08 pp; F paired median balanced-risk improvement 16.11 pp; each 20/20 positive, Holm p 1.9073486e-6 | Confirms each frozen primary contract on this cohort; upstream training-user exposure unknown |

At final 30% acceptance, median absolute user risks were E ordinary 32.86% to 14.19%, E balanced secondary 65.29% to 68.40%, F balanced 65.29% to 47.48%, and F ordinary secondary 32.86% to 34.88%. The paired median improvement is **not** the subtraction of separately computed absolute-risk medians. F's residual balanced risk is substantial.

Full-coverage pooled consumer-reference ACC was 65.19% on 1,828,243 eligible blocks. E's accepted-block pooled ACC was 83.42% and F's 64.09%, each on 548,481 accepted blocks. These selective ACC values exclude the abstained blocks and are not semantic human-label accuracy. [Exact aggregate data](../results/final_confirmation_summary.json) and [definitions](../results/README.md) are provided separately.
