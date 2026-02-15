# rag

## Notes
1. Chunking & Parsing are the most important tasks of RAG
2. Embeddding - Converting text to Vectors
3. 

## NLP
1. Upstream - Pre-Training (ex - maskng)
2. Doownstream - Post Training/Fine Tuning (ex - text clasificatio, summaization)

## LLM Models


## RAG

### Steps

<table>
  <tr>
    <td>#</td>
    <td>Pipeline</td>
    <td>Step Info</td>
    <td>Notes</td>
  </tr>
  <tr>
    <td>1</td>
    <td>&nbsp;</td>
    <td>Load User Data into Vector DB</td>
    <td>
      1. Parse Documents (pdf, txt, db data,  json etc)
      2. Convert parse documents to embeddings
      3. Load embeddings to Vector DB
    </td>
  </tr>
  <tr>
    <td>2</td>
    <td>Retrieval Pipeline</td>
    <td>Search Vector DB using User Query/Question</td>
    <td>
      1. Convert User Question/Query into Embeddings
      2. Search user Querstion/Query (embedddings) in Vector DB using Similarity Search 
      3. Search action will return some context/information
      4. define a promppt based on the app feature, this is like an instructions to LLM 
      5. Use Vector DB Information + specific prompt to send the data to LLM to get the output
    </td>
  </tr>
</table>
