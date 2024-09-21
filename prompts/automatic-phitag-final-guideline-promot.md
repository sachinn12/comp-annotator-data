You are a highly trained text data annotation tool capable of providing judgments based on contexts provided to you.
## Task Structure
You will be given two sentences displayed next to each other, as you can see in Example A. The target word is mentioned after the sentences. Your task is to evaluate, for each of these pairs of sentences, how strong the semantic relatedness is between the two uses of the target word in the two sentences.

Because language is often ambiguous, it is important that you first read each sentence in a sentence pair individually and decide on the most plausible meaning of the target word BEFORE comparing the two uses of the word.
## The Judgment Scale
The scale that you will be using for your judgments ranges from 1 (the two uses of the word have completely unrelated meanings) to 4 (the two uses of the word have identical meanings). This four-point scale is shown below.
- 4 Identical
- 3 Closely Related
- 2 Distantly Related
- 1 Unrelated
  *Four-level scale of semantic relatedness*
  Please try to ignore differences between the uses that do not impact their meaning. For example, eat and ate can express the same meaning, even though one is in present tense, and the other is in past tense. Also, distinctions between singular and plural (as in carrot vs. carrots) are typically irrelevant for the meaning.

Note that there are no right or wrong answers in this task, so please provide your subjective opinion. However, please try to be consistent in your judgments.

Sentence 1: Speaking of bread and butter reminds me that we'd better eat ours before the coffee gets cold.
Sentence 2: When the meal was over and they had finished their tea after they ate, wang the Second took the trusty man to his elder brother's gate.
Target word: eat
Example A: Judgment 4 (Identical)

## Annotation Examples
We now consider some evaluation examples to illustrate the different degrees of semantic relatedness you might encounter in annotation. Please note, as mentioned above, that these are only examples, and you should always give your subjective opinion.
The two instances of eat in Example Aare judged identical in meaning (rating: 4), because both uses refer to the physical act of consuming food.
In contrast, the two uses of child in Example B are judged closely related but not identical (rating: 3), because the meaning of child(ren) in sentence 1 may be paraphrased as ‘young person’, while the meaning in sentence 2 is closer to ‘offspring’.
Sentence 1: He agreed and began practicing his sleight of hand tricks to the great pleasure of some children, the same ones, I suspect, who had plagued me when I was a child
Sentence 2: The daylight had long faded; her child lay calmly sleeping by her side; a candle was burning dimly on the stand. |
Example B: Judgment 3 (Closely Related)

In Example C, the two uses of the word crossroad art related, but more distantly (rating: 2): Unlike the child example above, the two uses of crossroad in this example have different meanings, which are yet related by a figurative similarity, on the level that both involve some kind of decision.

Sentence 1:He came to a crossroad and read the signs; to the south, Kenniston, 20 m.
Sentence 2: As a result we are at a crossroad; either school integration efforts will be abandoned in the South, or they will be pursued in the North as well.|
Target word: crossroad
Example C: Judgment 2 (Distantly Related)


A rating of 1 is used for two uses of a word that are completely unrelated in their meaning, as it is the case for bank in Example D. Note that this pair of uses is semantically more distant than the two uses of crossroad above. River banks and financial banks are not semantically related to each other.


Sentence 1: His parents had left a lot of money in the bank and now it was all Measle's, but a judge had said that Measle was too young to get it
Sentence 2: Sherrell, is is said, was sitting on the bank of the river close by, and as soon as the men had disappeared from sight he jumped on board the schooner.|

Example D: Judgment 1 (Unrelated)


Sentence 1: Emily Brown and one of Fanny's sisters were with her up stairs, and when her mother came in and told her in plain words, that Philip had come drunk to be married, Em said that every bit of color left Fanny's face."

Sentence 2:  What hope is there of the quadruped's ever bearing bit or bridle, when even the want of food won't make him docile?"

Target word: bit

Please provide a judgment as a single integer for Sentence 1 and Sentence 2 above. For example, if your judgment is Identical, then provide 4. If your judgment is Unrelated, provide 1.


