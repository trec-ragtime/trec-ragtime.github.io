---
sidebar: 2025_sidebar.html
---

# TREC RAGTIME

*Last Updated: May 13 2026*

TREC RAGTIME is a [TREC](https://trec.nist.gov/) shared task to study and benchmark **report generation** from
news in multiple languages.
This is our second edition. Please refer to the [2025 archived page](/2025.html) for the details for the 2025 edition. 

Key features of the track are its focus on **multi-faceted reports** (going beyond factoid QA), and a
**citation-based evaluation** (providing supporting evidence of claims made in the report).

It also benchmarks Multilingual (MLIR) retrieval and Auto-nuggetization as supporting subtasks.

**Languages: English, Spanish, Chinese, and Russian**

[Track Guidelines](https://docs.google.com/document/d/1XqypNTHxIdazxfnUebrp-EsUuGNhodhQGrJIDnYGaB4/edit?usp=sharing)

**Search Service is up! Please also register at [TREC](https://trec.nist.gov/) to gain access to the enpoint.**
[Short API documentation](./search_api.md) for our search service. 

-------

## Tasks

**1. Multilingual Report Generation**

Given a set of documents in multiple languages and a "report request" that describes the information need,
generate a report in English that summarizes the information.

**2. Multilingual Retrieval**

Given a set of documents in multiple languages and a "report request" that describes the information need,
retrieve documents that help satisfy this information need.

**3. Auto-nuggetization (Request Decomposition) -- New in 2026**

Given the retrieval collection and a report request, generate a list of k single-sentence questions that should be answered in a report.
This task allows participants to explore identification of main topics that should appear in the report.

<span class='navigate_toc'><i class="fas fa-arrow-up right-margin"></i><a href='#' class='navigate_toc'>Back to top</a></span>

-------

## Timeline

<ul class="steps steps-vertical mb-4">
  <li class="step-item">
    <div class="h3 m-0">May 2026</div>
    <div class="h3 m-0">Evaluation document collection released: <a href="https://huggingface.co/datasets/trec-ragtime/ragtime2" target="_blank">[HuggingFace]</a></div>
    <div class="h3 m-0">Track Guidelines Released</div>
  </li>
  <li class="step-item">
    <div class="h3 m-0">Mid June 2026</div>
    <div class="h3 m-0">Topics Released <a href="https://livejohnshopkins-my.sharepoint.com/:f:/g/personal/dlawrie1_jh_edu/Er4p8SyZe5RHoUAWdJtjfMUBbWk09cmCJu1Hc1KDsJ8h3Q?e=Vv1f8j">[Link]</a></div>
  </li>
  <li class="step-item">
    <div class="h3 m-0">August 14 2026</div>
    <div class="h3 m-0">Submissions Due</div>
  </li>
  <li class="step-item">
    <div class="h3 m-0">October 2026</div>
    <div class="h3 m-0">Feedback on Final Submissions</div>
  </li>
  <li class="step-item active">
    <div class="h3 m-0">December 2026</div>
    <div class="h3 m-0">TREC 2026 Conference</div>
  </li>
</ul>

<span class='navigate_toc'><i class="fas fa-arrow-up right-margin"></i><a href='#' class='navigate_toc'>Back to top</a></span>

-------

## See Also: TREC NeuCLIR

TREC NeuCLIR (Neural CLIR) was the predecessor of TREC RAGTIME. In 2024, NeuCLIR included a pilot study of
report generation. You can find more about NeuCLIR at the [TREC NeuCLIR website](https://neuclir.github.io/).

<span class='navigate_toc'><i class="fas fa-arrow-up right-margin"></i><a href='#' class='navigate_toc'>Back to top</a></span>

-------

## Other RAG-related Tracks at TREC 2026

Consider also participating in other RAG-related tracks at TREC 2026. 

- [TREC RAG Track](https://trec-rag.github.io/)
- [TREC BioGen Track](https://trec-biogen.github.io/docs/)
- [TREC DRAGUN Track](https://trec-dragun.github.io/)
- [TREC iKAT](https://www.trecikat.com/)

-------

## Organizers

In alphabetical order:

- [Dawn Lawrie](https://hltcoe.jhu.edu/researcher/dawn-lawrie/), Johns Hopkins University, HLTCOE
- [Sean MacAvaney](https://macavaney.us/), University of Glasgow
- [James Mayfield](https://hltcoe.jhu.edu/researcher/james-mayfield/), Johns Hopkins University, HLTCOE
- [Luca Soldaini](https://soldaini.net), Microsoft
- [Eugene Yang](https://www.eugene.zone/), Johns Hopkins University, HLTCOE
- [Andrew Yates](https://andrewyates.net/), Johns Hopkins University, HLTCOE

<span class='navigate_toc'><i class="fas fa-arrow-up right-margin"></i><a href='#' class='navigate_toc'>Back to top</a></span>

-------

## Contact

 - Join the [Mailing List](https://groups.google.com/g/ragtime-participants) for updates and to post general questions
 - Twitter: [@trec_ragtime](https://x.com/trec_ragtime)
 - Any questions: ragtime-organizers@googlegroups.com

<span class='navigate_toc'><i class="fas fa-arrow-up right-margin"></i><a href='#' class='navigate_toc'>Back to top</a></span>
