# Query_Pdf_OpenAI_LANGCHAIN
This project is created to demonstrate how to query a pdf and store in Vector databse Cassandra for any query.<br />

Steps :<br /> 

1.Read the pdf document using Pypdf.
2.Create text chunks - split text into seprate packets/chunks for Natural Language processing.<br /> 
3.Text embeddings - convert text chunks into text embeddings /vectors.(Bag of words , tf -idf)/word to vec.<br />
To convert text into vectors will using embeddings from langchain.embeddings and import OpenAIEmbeddings.<br />
4.Create vector database - My goal is to store vector in Cassandra.Apache cassandra is an open source NOSQL database,<br />
  store massive amt of data , no sql distributed for scalability and high availability and fault taulerance.<br /> 
  Datastax will help me create vector casandra db.Create Astra Db id and Astra Db Application token.<br />
  Vector database helps in Vector Search.<br />
5.Create the LangChain embedding and LLM model object. Am going to use Open AI LLM model.<br />
6.We need to split the text using Character Text Split such that it should not increse token size.<br />
7.Now load the Astra Db vector store.<br />
8.Now I will query which will apply similarity search and text embeddings stored in vector database and going to<br /> 
  get that specific response from LLM model.<br />


Conclusion :

**Vector search** enhances machine learning models by allowing **similarity comparisons of embeddings** which are mathematical representation of 
high dimensional data.AstraDb , vector serch supports LLM models .So am using Serverless Cassandra with Vector Search.
Also I have utilized **langchain** for seamless integration with LLMS.**Pypdf** library is a great way to read text inside pdf very conveniently.
