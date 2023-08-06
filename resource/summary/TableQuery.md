# Summarization

## Abstract

This paper presents TableQuery, a novel tool for querying tabular data using deep learning models pre-trained to
answer questions on free text. Existing deep learning methods for question answering on tabular data have various
limitations, such as having to feed the entire table as input into a neural network model, making them unsuitable for
most real-world applications. Since real-world data might contain millions of rows, it may not entirely fit into the
memory. Moreover, data could be stored in live databases, which are updated in real-time, and it is impractical to
serialize an entire database to a neural network-friendly format each time it is updated. In TableQuery, we use deep
learning models pre-trained for question answering on free text to convert natural language queries to structured
queries, which can be run against a database or a spreadsheet. This method eliminates the need for fitting the entire
data into memory as well as serializing databases. Furthermore, deep learning models pre-trained for question
answering on free text are readily available on platforms such as HuggingFace Model Hub (7). TableQuery does
not require re-training; when a newly trained model for question answering with better performance is available, it
can replace the existing model in TableQuery

## ChatGPT

The paper presents a new tool called TableQuery, which is designed to allow users to query tabular data using natural language. The tool is based on deep learning models that are pre-trained on free text, which eliminates the need for fine-tuning when the data domain changes. This approach is more efficient and user-friendly than existing deep learning models for question answering on tabular data, which require the entire table to be fed into a neural network model.

TableQuery allows users to query large datasets without memory restrictions by storing tables into a database or spreadsheet. The system architecture of TableQuery is described in detail, including the main modules and how they are connected. The tool is designed to convert natural language queries to structured queries and run them against a database or spreadsheet.

The paper also shares qualitative results from experiments conducted on the WikiSQL dataset, which is a dataset for developing language interfaces for relational databases. The results demonstrate the effectiveness of TableQuery, particularly in cases where the table is large. The paper concludes by highlighting the limitations of existing work and how TableQuery improves upon them. Overall, TableQuery provides a more efficient and user-friendly solution for querying tabular data using natural language.