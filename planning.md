# Milestone 1: Domain Selection and Document Collection

## Domain

Student Reviews of Computer Science Professors

## Domain Summary

This project focuses on student-generated reviews of Computer Science professors. Students often rely on scattered online reviews when selecting courses and instructors, making it difficult to compare teaching styles, workload, grading policies, and overall course experiences. This RAG system will help users search and answer questions about professors using information retrieved from student reviews.

## Example Questions

1. Which professor is best for beginners?
2. Which professor gives the hardest exams?
3. Which professor provides the most useful feedback?
4. Which professor has the heaviest workload?
5. Which professor is most recommended by students?

## Sources

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
    
## Document Structure Notes

After reviewing several professor pages, I observed that the documents consist of many short student reviews. Most reviews focus on teaching quality, workload, exam difficulty, grading fairness, and overall course experience. Important information is usually contained within a single review rather than spread across long paragraphs, which will influence the chunking strategy used in the next milestone.
