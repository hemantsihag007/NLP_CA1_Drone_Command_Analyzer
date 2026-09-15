# Smart Drone Command Language Analyzer Using Basic NLP

**Course:** Natural Language Processing (CSE 306) — CA Project

## 1. Project Title
Smart Drone Command Language Analyzer Using Basic NLP

## 2. Problem Statement
This project implements a small rule-based Natural Language Processing system for delivery-drone commands. Each command is expected to contain a Subject, Verb and Object. The program accepts or rejects a new sentence, gives a reason when it is rejected, and shows the role of each word when the sentence is accepted.

## 3. Objective
- Create a small corpus of 20 simple English drone-command sentences.
- Tokenize input sentences into individual words.
- Identify Subject, Verb and Object roles.
- Validate sentences using a Subject + Verb + Object rule.
- Reject invalid commands with a clear reason.
- Check whether a valid command exists in the corpus.
- Allow new valid commands to be added dynamically.
- Display the corpus and vocabulary.

## 4. Dataset Description
The initial corpus contains 20 predefined drone-command sentences. The vocabulary contains two subjects (`drone`, `robot`), six verbs (`carries`, `delivers`, `drops`, `moves`, `picks`, `transports`) and six objects (`box`, `food`, `goods`, `medicine`, `package`, `parcel`). The project uses this custom corpus to demonstrate basic NLP tasks.

The system also supports dynamic addition of a new valid command. For example, `Drone carries medicine` is structurally valid and can be added to the corpus when it is not already present.

## 5. Methodology
1. **Corpus creation:** Define 20 simple English commands.
2. **Tokenization:** Convert the input to lowercase and split it into word tokens using regular expressions.
3. **Role identification:** Match tokens against subject, verb and object vocabularies.
4. **Parsing:** Represent a valid three-token command as a Subject-Verb-Object dictionary.
5. **Validation:** Check empty input, exact word count, vocabulary membership and corpus membership.
6. **Dynamic learning:** Add a structurally valid command to the corpus if it is not already present.

## 6. Key Findings
- Tokenization successfully converts commands into individual words.
- Subject, verb and object roles can be identified using predefined vocabularies.
- Invalid subjects, verbs and objects are rejected with specific reasons.
- Commands with an incorrect number of words are rejected.
- A structurally valid command can still be rejected when it is not present in the corpus.
- New valid commands can be added dynamically and then accepted.

## 7. Test Cases
| Test Sentence | Result | Observation |
|---|---|---|
| Drone delivers package | Accepted | Valid Subject-Verb-Object command in corpus |
| Car delivers package | Rejected | Invalid subject |
| Drone flies package | Rejected | Invalid verb |
| Drone delivers car | Rejected | Invalid object |
| Drone delivers package quickly | Rejected | Incorrect number of words |
| Drone carries medicine | Rejected initially, then accepted after addition | Valid structure but initially absent from corpus |

## 8. Limitations
- The vocabulary is small and predefined.
- Commands must follow exactly the Subject + Verb + Object structure.
- The system does not handle synonyms or complex grammatical structures.
- Exact corpus membership is required for acceptance before a new command is added.
- The project uses basic rule-based NLP rather than an advanced NLP model.

## 9. Conclusion
The Smart Drone Command Language Analyzer demonstrates practical use of basic NLP concepts through Python. It performs corpus creation, tokenization, vocabulary checking, sentence validation, role identification, simple parsing and dynamic corpus addition. The project provides a clear demonstration of how a basic NLP application can understand and validate a restricted language.

## 10. Submission Files
- `NLP_CA1_Drone_Command_Analyzer.ipynb` — complete project notebook.
- `Project_Report.md` — report version included in GitHub.
- `Drone_Command_NLP_Project_Report.docx` — formatted report prepared for submission.
- `Drone_Command_NLP_Project_Report.pdf` — PDF report prepared for submission.
- `Drone_Command_NLP_Project_Presentation.pptx` — project presentation prepared for submission.
