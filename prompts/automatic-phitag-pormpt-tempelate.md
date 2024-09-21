## Guideline only

Role: system, message: You are a highly trained text data annotation tool capable of providing subjective responses.

Role: user: [ GUIDELINE]
Role: user, message: Sentence 1: [ SENTENCE 1]

Role: user, message: Sentence 2:  [ SENTENCE 2]

Role: user, message : Target word: [ SENTENCE 2]

Role: user, message : Please provide a judgment as a single integer. For example, if your judgment is Identical, then provide 4. If your judgment is Unrelated, provide 1

## Guideline + Tutorial only

Role: system, message: You are a highly trained text data annotation tool capable of providing subjective responses.

Role: user: [ GUIDELINE]
Role: user: Here are few examples you refer:

Sentence 1: [SENTENCE 1]
Sentence 2:  [ SENTENCE 2]
Target word: [ TARGET WORD]
Judgement:  [ TARGET JUDGEMENT]

Sentence 1: [ SENTENCE 1]
Sentence 2:  [ SENTENCE 2]
Target word: [ TARGET WORD]
Judgement:  [ TARGET JUDGEMENT]

Sentence 1: [ SENTENCE 1]
Sentence 2:  [ SENTENCE 2]
Target word: [ TARGET WORD]
Judgement:  [ TARGET JUDGEMENT]


Role: user, message: Sentence 1: [ SENTENCE 1]

Role: user, message: Sentence 2:  [ SENTENCE 2]

Role: user, message : Target word: [TARGET WORD]

Role: user, message : Please provide a judgment as a single integer. For example, if your judgment is Identical, then provide 4. If your judgment is Unrelated, provide 1.
