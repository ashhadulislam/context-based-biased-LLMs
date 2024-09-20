# Context-Based Biased LLMs (CB-LLM)

## Overview
This project introduces **Context-Based Biased Large Language Models (CB-LLM)**, aimed at addressing bias in mainstream AI models by utilizing a comprehensive data collection methodology that integrates both structured and unstructured data sources. CB-LLMs ensure contextually rich and ethically responsible generation of responses, prioritizing high-quality, evidence-based information.

The **AI for Palestine** initiative is a demonstration of this technology, designed to amplify marginalized voices by ensuring that generated responses reflect accurate narratives through an unbiased retrieval mechanism.

## Key Features
- **Retrieval-Augmented Generation (RAG) System**: The system retrieves data in a context-aware manner, using Voronoi clustering for optimized search and retrieval.
- **Voronoi Clustering**: Efficient partitioning of data into clusters to ensure faster and more accurate retrieval of relevant information.
- **Paraphrasing LLM**: The system generates multiple query variations to widen the search scope and capture diverse search results.
- **Meta Prompting**: The final query prompt includes instructions, persona, context, and the original user query to enhance the LLM's ability to provide precise, contextually relevant answers.
- **Bias Mitigation**: Randomized retrieval and paraphrasing ensure diverse and balanced data usage to minimize biases in the generated output.

## Workflow
1. **Optimized Data Store with Voronoi Clusters**:
   - Data chunks are embedded and organized into clusters using Inverted File Index (IVF) and Voronoi clustering for fast retrieval.
2. **LLM for Paraphrasing**:
   - A user query is paraphrased into multiple variations to generate a broader set of search inputs.
3. **Search Results Retrieval**:
   - The paraphrased queries are used to retrieve top-k chunks from the data store for each paraphrase.
4. **Shuffling and Cropping**:
   - The search results are concatenated and shuffled to avoid bias, then cropped to fit within the LLM's context window.
5. **Meta Prompting**:
   - A meta prompt is constructed with instructions, persona, and the original user query, which is fed into the LLM to generate a final answer.

## AI for Palestine Case Study
This project showcases the **AI for Palestine** initiative, which uses CB-LLMs to promote social justice by generating transparent, evidence-based content that accurately reflects the Palestinian narrative. By countering biases in traditional AI models, this project demonstrates how CB-LLMs can be applied to amplify underrepresented voices.

## Key Innovations
- **Voronoi Clustering** for optimized search.
- **Randomized Retrieval** to avoid dominance of any single data source.
- **Paraphrasing** to enhance query diversity and information retrieval.
- **Meta Prompting** for precise, contextually rich responses.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/context-based-biased-LLMs.git
   cd context-based-biased-LLMs
   ```

## Contributors

- **Ashhadul Islam**  
  Email: [asislam@hbku.edu.qa](mailto:asislam@hbku.edu.qa), [ashhadulislam@gmail.com](mailto:ashhadulislam@gmail.com)
  
- **Hurmat Ali Shah**  
  Email: [hshah@hbku.edu.qa](mailto:hshah@hbku.edu.qa)

- **Dr. Samir Brahim Belhaouari**

- **Dr. Mowafa Househ**  
  Information & Computing Technology  
  College of Science and Engineering  
  Hamad Bin Khalifa University

---

### Want to be a part of the project?

We welcome contributors! If you're interested in collaborating, feel free to get in touch with any of the contributors above or reach out via email.
