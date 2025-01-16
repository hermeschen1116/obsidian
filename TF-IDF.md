- A scoring method the **importance of a token** to a document in the database
- Consist of TF（Term Frequency）and IDF（Inverse Document Frequency）
- TF and IDF can be replace with any other scoring function.
- Formula$$tfidf_{i,j}=tf_{i,j}\times idf_i$$
## TF (Term Frequency)
- Formula $$tf_{i,j}=\frac{n_{i,j}}{\Sigma_{k}n_{k,j}}$$
	- $n_{i,j}$: the frequency of token $t_k$ in a document $d_j$ 
	- $\Sigma_{k}n_{k,j}$: the sum of the frequency of token $t_k$ between all documents
## IDF (Inverse Document Frequency)
- Formula$$idf_i=lg(\vert\frac{D}{1+\lbrace j: t_i\in d_j\rbrace}\vert)$$
	- $D$: the number of total documents
	- $\lbrace j: t_i\in d_j\rbrace$: the number of documents which contain token $t_k$