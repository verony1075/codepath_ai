# Milestone 2

## Domain

My project focuses on student reviews of Computer Science professors at Berea College.

This information is useful because students want to know what a professor is really like before taking a class. The college website provides course information, but it does not tell students about teaching style, workload, grading, or exam difficulty. Students usually have to search through many reviews to find this information.

## Documents

I will use Rate My Professors pages for Computer Science professors at Berea College.

### Sources

1. https://www.ratemyprofessors.com/professor/575383
2. https://www.ratemyprofessors.com/professor/1999243
3. https://www.ratemyprofessors.com/professor/740993
4. https://www.ratemyprofessors.com/professor/2733183
5. https://www.ratemyprofessors.com/professor/2666983
6. https://www.ratemyprofessors.com/professor/2825376
7. https://www.ratemyprofessors.com/professor/2366848
8. https://www.ratemyprofessors.com/professor/2359760
9. https://www.ratemyprofessors.com/professor/1719095
10. https://www.ratemyprofessors.com/professor/1846092

Most of these documents contain student opinions about teaching quality, workload, grading, exams, and overall class experience.

## Chunking Strategy

Most reviews are short and usually contain one main opinion. I will use chunks of about 400 characters with a 50-character overlap.

I chose this size because it keeps most reviews together in one chunk. The overlap helps make sure important information is not lost between chunks.

If chunks are too small, important details may be missing. If chunks are too large, multiple reviews may be mixed together and retrieval may become less accurate.

## Retrieval Approach

I will use the all-MiniLM-L6-v2 embedding model from sentence-transformers and ChromaDB as the vector database.

For each question, I will retrieve the top 5 most relevant chunks.

Using too few chunks may miss useful information. Using too many chunks may include reviews that are not related to the question. Semantic search helps find reviews with similar meanings even when different words are used.

## Evaluation Plan

### Question 1

What do students say about Matt Jadud?

Expected Answer:
Students describe him as helpful, supportive, knowledgeable, and understanding. Some students also mention that he goes off topic during lectures.

### Question 2

Which professor is described as the most helpful?

Expected Answer:
The professor with the most positive comments about helping students and supporting learning.

### Question 3

Which professor is described as having the hardest exams?

Expected Answer:
The professor whose reviews mention difficult exams most often.

### Question 4

Which professor is recommended for beginner students?

Expected Answer:
The professor whose reviews mention clear explanations and beginner-friendly teaching.

### Question 5

Which professor is described as having the heaviest workload?

Expected Answer:
The professor whose reviews mention a large number of assignments and course work.

## Anticipated Challenges

Students may have different opinions about the same professor.

Some professors may not have many reviews, which can make it harder to find enough information.

The system may retrieve reviews that are not directly related to the user's question.

Important information may sometimes be split between chunks.

## AI Tool Plan

I will use ChatGPT to help me understand RAG concepts and troubleshoot coding problems.

I will use AI tools to help create functions for loading documents, chunking text, generating embeddings, and querying ChromaDB.

I will provide my project requirements and planning decisions when asking for implementation help.

I will also use AI tools to help debug errors and improve retrieval quality.

## Architecture
