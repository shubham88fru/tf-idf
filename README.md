# tf-idf

Per the TF-IDF algorithm, for a given set of search query (search terms) 
search query = [term1, term2, ... termN]
the score of a document i (indicating how relevant that document is to the search terms) is
given by Score(doc_i) = 
        tf("term1", doc_i) * idf("term1") + tf("term2", doc_i) * idf("term2")
        + tf("term3", doc_i) * idf("term3") ....

Here, the term frequency tf("term1", doc_i) is defined as -
tf("term1", doc_i) = term1_count/words_count

And, inverse document frequency idf("term1") is defined as - 
idf("term1") = log(N/nt)
where, N = Number of documents
and nt = Number of documents containing the term.