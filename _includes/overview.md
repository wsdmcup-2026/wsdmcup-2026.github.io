Retrieval-Augmented Generation (RAG) systems provide an opportunity to expand the scope of available information to users, since they are able to retrieve and synthesize information from documents in languages that the user does not necessarily understand. The ability to retrieve documents only based on their relevance, regardless of language, is crucial for modern retrieval models to support better coverage of perspectives from different parts of the world. Thus, WSDM Cup 2026 features a multilingual retrieval task. 

The participants will develop systems that receive English queries and search a collection of about [10 million documents](https://huggingface.co/datasets/neuclir/neuclir1) in Chinese (3.1M), Persian (2.2M), and Russian (4.6M). For each query, the system must produce a ranked list of 1,000 documents selected from the entire multilingual collection, ordered by likelihood and relevance to the topic. All systems should operate automatically without human intervention. Submissions must be in the TREC run file format. **Each team may submit up to 5 submissions and will be evaluated using nDCG@20.**


### Participation and Submission Instructions

There are 41 development queries that the participants can use in system development. Participants are free to use other data, such as MIRACL. However, **using the TREC NeuCLIR Track data besides the development queries provided by the organizers is strongly prohibited.** The participants should not use the publicly available relevance assessments on this specific collection (NeuCLIR) besides the development queries and labels provided by the Cup. Participants will be asked to provide code for their training and inference process either through a tarball submission or a publicly available repository. 

All participants are expected to submit a short write-up about their submissions (similar to the TREC system paper). Selected teams (including the winner of the Cup) will receive a slot at WSDM for oral presentation. 

Submissions will also be made to the submission Google Form. All test queries should have at least 20 retrieved documents in each submission file. The following is an example of the submission format (the TREC run format).

```
212 Q0 a6c8f37a-8847-4b56-bd45-146bcecd78f3 1 29.3672 your-run-name
212 Q0 f3081151-21ca-4c8f-a1b5-2c1299420e24 2 29.3174 your-run-name
212 Q0 5c9f4b65-ea91-4c8a-a7f2-0d384728e573 3 29.2985 your-run-name
212 Q0 711933a6-04c5-42fe-aace-9834f7c6e028 4 29.0986 your-run-name
212 Q0 3a179067-46ee-46e7-a184-d794580e2bcb 5 29.0889 your-run-name
212 Q0 e9fc0c92-e67c-4197-af29-17d4dd250877 6 29.0679 your-run-name
```

If you have any question, please [raise issues in our Github Repository](https://github.com/wsdmcup-2026/wsdmcup-2026.github.io/issues).

### Data

- Document Collection: [Huggingface Datasets](https://huggingface.co/datasets/neuclir/neuclir1).
- Development Queries: [Download Link](/resource/wsdm-cup.dev.queries.tsv)
- Development Qrels: [Download Link](/resource/wsdm-cup.dev.qrels)
- **Test Queries:** [Download Link](/resource/wsdm-cup.test.queries.tsv) 

Your submission should contains queries in the **test queries** file. 


### Important Dates
- November 17, 2025: Document collection, development/test queries, and the submission portal are available.
- December 1, 2025: Online Q&A session if needed
- February 2, 2025: Submission due
- February 22-26, 2026: WSDM Conference; winner and evaluation result announcement. An overview technical report will be released along with the final results.  


### Other Additional Data and Resources

Besides the development queries, there are other cross-language, multilingual, and monolingual retrieval datasets that can be used to develop the systems. Here is an incomplete list of them

- [Evaluation: ir-measure](https://ir-measur.es/en/latest/)
- [Accessing IR datasets](https://ir-datasets.com/)
- [CLIRMatrix](https://aclanthology.org/2020.emnlp-main.340/)
- [MIRACL](https://github.com/project-miracl/miracl)
- [MKQA](https://github.com/apple/ml-mkqa)
