# 3 different examples of API actions described within system prompt

## 1. github

### api_github_com__jit_plugin

This typescript tool allows you to call external API endpoints on api.github.com over the internet.
namespace api_github_com__jit_plugin {

// Gets the contents (files) of a specific repo/directory. The 'download_url' property can be used to get the path for the file reader. Make sure to use the 'Github File Reader' action when trying to read contents (if its available).
type listGithubFiles = (_: {
// The owner of the repository (username).
owner: string,
// The name of the repository itself.
repo: string,
// The path to the file or folder (leave this blank to just get the root of the repo). This is case-sensetive.
path: string,
}) => any;

} // namespace api_github_com__jit_plugin



## 2) semanticscholar

### api_semanticscholar_org__jit_plugin

This typescript tool allows you to call external API endpoints on api.semanticscholar.org over the internet.
namespace api_semanticscholar_org__jit_plugin {

// Relevancy-based search for papers on Semantic Scholar.
type searchSemanticScholar = (_: {
// The search query itself, this can be any natural language query.
query: string,
// The maximum number of papers to return. Defaults to 10, maximum is 100.
limit?: number,
// The fields to return in the response. Use the pre-specified value for this (don't change it).
fields: "url,abstract,publicationTypes,tldr,openAccessPdf",
// The fields of study to filter the results by. These are comma-separated values, e.g. "Computer Science,Medicine".
fieldsOfStudy?: "Computer Science" | "Medicine" | "Chemistry" | "Biology" | "Materials Science" | "Physics" | "Geology" | "Psychology" | "Art" | "History" | "Geography" | "Sociology" | "Business" | "Political Science" | "Economics" | "Philosophy" | "Mathematics" | "Engineering" | "Environmental Science" | "Agricultural and Food Sciences" | "Education" | "Law" | "Linguistics",
// The publication date or year to filter the results by (inclusive). Accepts the format <startDate>:<endDate> (YYYY-MM-DD), e.g. 2016-03:2020-06 (as early as March, 2016 or as late as June, 2020).
publicationDateOrYear?: string,
// The publication types to filter the results by. These are comma-separated values, e.g. "JournalArticle,CaseReport".
publicationTypes?: "Review" | "JournalArticle" | "CaseReport" | "ClinicalTrial" | "Dataset" | "Editorial" | "LettersAndComments" | "MetaAnalysis" | "News" | "Study" | "Book" | "BookSection",
}) => any;

} // namespace api_semanticscholar_org__jit_plugin



## 3) poliquiz

### api_poliquiz_it__jit_plugin

This typescript tool allows you to call external API endpoints on api.poliquiz.it over the internet.
namespace api_poliquiz_it__jit_plugin {

// List all courses
type listCourses = () => {
  data: {
  id: number,
  name: string,
}[],
};

// Get metainfo about a specific course
type getCourseMetaInfo = (_: {
// The ID of the course
course_id: number,
}) => {
  data: {
  total_quizzes: number,
  total_verified_quizzes: number,
},
};

// Retrieve quizzes for a specific course
type getCourseQuizzes = (_: {
// The ID of the course
course_id: number,
}) => {
  data: {
  id: number,
  course_id: number,
  question: string,
  answers: string[],
  right_answer_index: number,
  explanation: string,
  verified: boolean,
}[],
};

} // namespace api_poliquiz_it__jit_plugin
