# Adapting Bioinformatics Data Systems in the Era of Foundational Models: Leveraging RAG and Low-Resource LLMs

### Author Chihiro Higuchi
### Affiliation: National Institutes of Biomedical Innovation, Health and Nutrition (NIBIOHN) / Institute of Science Tokyo

Project Description:

The National Institutes of Biomedical Innovation, Health, and Nutrition (NIBIOHN) and the Bioscience Database Center (NBDC) have been cataloging domestic bioinformatics data. This catalog was integrated into a cross-search system powered by the full-text search engine Elastic Search. However, the landscape changed dramatically with the introduction of ChatGPT in November 2022.

While foundational models like ChatGPT offer considerable convenience, their reliance on token occurrence probabilities in language models is known to lead to hallucinations, independent of the factual accuracy of the texts used during pre-training. Moreover, the widespread use of such models could undermine our longstanding efforts in cataloging bioinformatics data. In response, we are exploring the use of Retrieval-Augmented Generation (RAG) to leverage our accumulated data in conjunction with foundational models.

Although multiple studies have demonstrated the efficacy of RAG, numerous methods have been proposed, and no consensus has been reached on which approach is most effective for bioinformatics data retrieval. Therefore, we believe it is necessary to rigorously evaluate these methods.

For widespread public use, the system must be fully developed. One practical approach for implementing RAG involves using no-code tools like Dify, which simplifies the process but relies heavily on its user interface. Alternatively, although it requires Python coding, a solution utilizing Streamlit in combination with LangChain or LlamaIndex may also prove effective.

As for Large Language Models (LLMs), until early 2024, deploying them required high-performance GPU environments. However, advancements such as model quantization and the release of systems like Ollama have made low-resource operation feasible. The recently introduced Entoropix technology is expected to further enable even more efficient use of LLMs with minimal resources.

During the BLAH workshop, we aim to address these diverse issues and outline a clear path for future initiatives.

## Reference 

- Sourav Banerjee et al. LLMs Will Always Hallucinate, and We Need to Live With This. https://arxiv.org/abs/2409.05746.
- Darren Edge et al. From Local to Global: A Graph RAG Approach to Query-Focused Summarization. https://arxiv.org/abs/2404.16130.
- Ollama. https://github.com/ollama/ollama.
- Dify. https://dify.ai/.
- Llamaindex. https://www.llamaindex.ai/.
- LightRAG. https://arxiv.org/abs/2410.05779.
- entropix. https://github.com/xjdr-alt/entropix/tree/main
