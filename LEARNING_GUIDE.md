# Discussing this project accurately

## Five questions to understand before putting it on your CV
1. Why use the original study repository? It documents provenance, measures and a licence, and provides trial-level behaviour.
2. What is the main result? In the AI-labelled sample, mean participant accuracy increased, but incorrect advice sometimes led initially correct participants to switch.
3. Why resample participants? Trials from the same person are dependent. Resampling rows would treat repeated decisions as independent. Our intervals still condition on the observed items.
4. Why not call slider strength calibration? We have not established that a slider magnitude represents a subjective probability of being correct. We analyse strength and behaviour, without inventing probability calibration.
5. How does it connect to DC13? It is a foundation for reasoning about advice-taking, not evidence about early-career professionals or workplace learning. A future longitudinal design could address those questions.

## A hands-on review
- Open README and REPORT, then read derive() in src/analyse.py.
- Work through the five examples in check_metrics.py by hand.
- Run the metric checks and the full analysis locally.
- Inspect the denominators in results/summary.csv.
- Compare the main and sensitivity results.
- Add a dated contribution note describing only what you personally reviewed, changed or ran.

## CV wording now
AI-assisted exploratory secondary-analysis project using open human advice-taking data; analysis draft under review.

## CV wording after personal review and reproduction
Use only if accurate: Reviewed and reproduced a Python secondary analysis of 35,670 public advice-taking trials; examined decision accuracy and conditional switching with participant-level bootstrap intervals and sensitivity checks. Analysis code developed with AI assistance; original data collected by Vodrahalli et al.

Avoid: collected 35,670 trials; validated co-agency scale; proved AI improves professional judgement; independently developed all code; published research; longitudinal evidence on early-career professionals.
