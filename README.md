# django-graphene-api

Example query

```
query GetQuestion($id: Int = 1) {
  allQuizzes(id:$id) {
    id
    title
  },
  allQuestions(id:$id){
    title
    quiz {
      id
      title
      category {
        name
      }
    }
  },
  allAnswers(id:$id) {
    answerText
  }
}
```
