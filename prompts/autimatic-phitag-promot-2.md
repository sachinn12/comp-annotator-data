You are a highly trained text data annotation tool capable of providing subjective responses.
"# Guidelines for UREL Annotation
## Introduction
Your task is to rate the degree of semantic relatedness between two uses of a word. For instance, presented with a sentence pair as in the below table, you are asked to rate the semantic relatedness between the two uses of **grasp**.

|Usage 1 | Usage 2 |
|--------|---------|
|He continued to **grasp**, between forefinger and thumb, the edge of the cloth I had been sewing.|For just a moment he didn't **grasp** the import of what the old man had said.|

## Task Structure

You will be shown two sentences displayed next to each other, as you can see in Example A. The target word is marked in bold in the respective sentence. Your task is to evaluate, for each of these pairs of sentences, how strong the semantic relatedness is between the two uses of the target word in the two sentences.

Because language is often ambiguous, it is important that you first read each sentence in a sentence pair individually and decide on the most plausible meaning of the target word BEFORE comparing the two uses of the word. In some cases, the sentences already provide enough information to understand the meaning of the target word; however, for cases that are unclear, you can find additional context beyond that in gray.

## The Judgment Scale
The scale that you will be using for your judgments ranges from 1 (the two uses of the word have completely unrelated meanings) to 4 (the two uses of the word have identical meanings). This four-point scale is shown below.


- 4 Identical
- 3 Closely Related
- 2 Distantly Related
- 1 Unrelated

- \- Can't decide

*Four-level scale of semantic relatedness*

*** 
Please try to ignore differences between the uses that do not impact their meaning. For example, eat and ate can express the same meaning, even though one is in present tense, and the other is in past tense. Also, distinctions between singular and plural (as in carrot vs. carrots) are typically irrelevant for the meaning.

Note that there are no right or wrong answers in this task, so please provide your subjective opinion. However, please try to be consistent in your judgments.
|Usage 1 | Usage 2 |
|--------|---------|
|Speaking of bread and butter reminds me that we'd better **eat** ours before the coffee gets cold.|When the meal was over and they had finished their tea after they **ate**, wang the Second took the trusty man to his elder brother's gate.|

[**4-Identical**, 3-Closely Related, 2-Distantly Related, 1-Unrelated]

Example A: Judgment 4 (Identical)
***
## Annotation Examples
We now consider some evaluation examples to illustrate the different degrees of semantic relatedness you might encounter in annotation. Please note, as mentioned above, that these are only examples, and you should always give your subjective opinion.

The two instances of eat in **Example A** are judged identical in meaning (rating: 4), because both uses refer to the physical act of consuming food.

In contrast, the two uses of child in **Example B** are judged closely related but not identical (rating: 3), because the meaning of child(ren) in sentence 1 may be paraphrased as ‘young person’, while the meaning in sentence 2 is closer to ‘offspring’.

|Usage 1| Usage 2|
|--------|---------|
|He agreed and began practicing his sleight of hand tricks to the great pleasure of some **children**, the same ones, I suspect, who had plagued me when I was a child| The daylight had long faded; her **child** lay calmly sleeping by her side; a candle was burning dimly on the stand. |

[4-Identical, **3-Closely Related**, 2-Distantly Related, 1-Unrelated]

Example B: Judgment 3 (Closely Related)

***
In **Example C**, the two uses of the word crossroad art related, but more distantly (rating: 2): Unlike the child example above, the two uses of crossroad in this example have different meanings, which are yet related by a figurative similarity, on the level that both involve some kind of decision.

|Usage 1 | Usage 2 |
|--------|---------|
|He came to a **crossroad** and read the signs; to the south, Kenniston, 20 m.|As a result we are at a **crossroad**; either school integration efforts will be abandoned in the South, or they will be pursued in the North as well.|

[4-Identical, 3-Closely Related, 2-Distantly Related, 1-Unrelated]

Example C: Judgment 2 (Distantly Related)


***
A rating of 1 is used for two uses of a word that are completely unrelated in their meaning, as it is the case for bank in **Example D**. Note that this pair of uses is semantically more distant than the two uses of crossroad above. River banks and financial banks are not semantically related to each other.

|Usage 1 | Usage 2 |
|--------|---------|
|His parents had left a lot of money in the **bank** and now it was all Measle's, but a judge had said that Measle was too young to get it|Sherrell, is is said, was sitting on the **bank** of the river close by, and as soon as the men had disappeared from sight he jumped on board the schooner.|

[4-Identical, 3-Closely Related, 2-Distantly Related, **1-Unrelated**]

Example D: Judgment 1 (Unrelated)

***

Finally, the non_label symbol '-' is used when the annotator is unable to make a judgment. Please use this option only if absolutely necessary, i.e., if you cannot make a decision about the degree of semantic relatedness between the two words marked in bold. This may be the case, for example, if you find a sentence too flawed to understand, the use of the target word is ambiguous, or the two uses of the target word do not match (i.e., do not have the same lemma). In **Example E**, the annotator is unable to judge semantic relatedness because Usage 1 is ambiguous; it is unclear whether the word "bank" refers to a financial institution or the bank of a river.

|Usage 1 | Usage 2 |
|--------|---------|
|I saw Mark as he was heading down to the **bank**.|Sherrell, is is said, was sitting on the **bank** of the river close by, and as soon as the men had disappeared from sight he jumped on board the schooner.|

[4-Identical, 3-Closely Related, 2-Distantly Related, 1-Unrelated]

Here are the few examples you refer:

Sentence 1: I would roam through the cities, through village and dell. But I never would return To my cold prison cell; what’s life without liberty? What's life without liberty, I ofttimes have said.
Sentence 2: There sorrows were but for the misfortunes of others. They went their way rejoicing , and with them passed the solitary ray of sunshine that streamed athwart the dark horrors of the emigrant ship, like the wandering pencil of light that sometimes visits the condemned cell of a prison.
Target word: cell
Judgement: 4

Sentence 1: After the third day was over, it was accepted by tacit consent that farther search would be useless. Hetty was mourned as dead: in every home her name was tenderly and sorrowingly spoken; old memories of her gay and mirthful youth, of her cheery and busy womanhood, were revived and dwelt upon.  But in her own home was silence that could be felt.
Sentence 2: """Now she looks like other girls, and as I like to see her,"" Mrs. Clara was saying, with an air of great satisfaction. She does look like a fashionable young lady, but somehow I miss my little Rose, for children dressed like children in my day , "" answered Aunt Plenty , peering through her glasses with a troubled look , for she could not imagine the creature before her ever sitting in her lap , running to wait upon her , or making the house gay with a child's blithe presence . "" ""Things have changed since your day, Aunt, and it takes time to get used to new ways."""
Target word: gay
Judgement: 3

Sentence 1: Both names had every appearance of being autographs. The opposite page was partly covered with names of ships, scratches of the pen, unconnected sentences, and one or two common sailor expressions. Mrs. Stanley\'s eyes grew dim for an instant, after she had read the names.
Sentence 2: Here and there are chamois heads and pressed seaweed. He writes on gilt-edged paper with a gold pen and handle twisted with a serpent.  His inkstand is a mystery of beauty which unskilled hands dare not touch, lest the ink spring at him from some of the open mouths, or sprinkle on him from the bro
Target word: pen
Judgement: 4

Sentence 1: "We waited a long time after we rang the bell before Jonquil opened the door. That was to give her time to peep out at us from the tumorous bay window and compose her features. ""Jonquil!"" I said heartily, dashing forward and delivering the required peck on her cheek."
Sentence 2: """No-no-no-no-no-no-no."" He thought you were cute, her sister peeped, then took a hurried gulp of her double-tall, caffeine-free skinny latte. ""No blind dates. And that..."" she added, pointing, ""...is not a coffee."""
Target word: peep
Judgement: 1

Sentence 1: It was both ugly and pretty--its wings being transparent, and elegantly constructed. Its head was small, like a mouse's, and the colonel, opening its jaws, showed its sharp teeth, There was a little pile of mosquitoes under its tongue.
Sentence 2: DARPA boasts a four-decade-long history of promoting novel technologies. DARPA's gambles proved instrumental in spawning the Internet and the computer mouse, stealth aircraft and the chip that makes your cell phone work  DARPA is hardly the only player funding cutting-edge research.
Target word: mouse
Judgement: 2

Sentence 1: The branches now hung waving and floating on the air in wreaths and luxuriant masses. The path was just wide and high enough to allow us to mount our horses, but soon opened into a spacious The spectacle to me was astonishing.
Sentence 2: Any of the villagers will tell you where it stands. There is a cottage or cabin, on one side, and a garden surrounded by a high wall on the other.  You cannot avoid it.
Target word: high
Judgement: 4

Sentence 1: """Do you really think so badly of me?"" Her hand pressed my arm with warm friendliness; her great blue eyes were watching me with beseeching interest. ""I think, Liane,"" I replied, ""that Mr. Hendricks is a very young man"""
Sentence 2: I examined it closely. The arm of the statue had a natural form. But the face was all wrong.
Target word: arm
Judgement: 3

Sentence 1: We ask for this young Dove, etc. Untie his tender hands --Let the young captive free--And bind in iron bands The souls that rail at Thee! Oh! Calm her anxious fears.
Sentence 2: "Wears fair-top boots and a broad-rim; an\' comes afore breakfus\' for his rent?  I know Israel Bonus, said the young girl, smiling;"" He owns this Court. But your mother--can I do anything to aid her?"
Target word: young
Judgement: 4

Sentence 1: "We turned to leave. She searched the bag for her cell as we headed toward the door. ""I can't find it!"""
Sentence 2: I really felt sorry for him. The poor man’s got no wind in his jail cell. I could not even imagine it.
Target word: cell
Judgement: 2

Sentence 1: her skintight jumpsuit was an object of desire. West Hollywood is a bastion of gay and lesbian culture, which I, as a heterosexual female, found comforting in ways I didn't exactly understand.  I caught myself really looking at people, on the street, in cars.
Sentence 2: Silverman ordered them shut down. The following year, the number of gay men newly infected with HIV declined dramatically. But the story does not end there.
Target word: gay
Judgement: 4

Sentence 1: Liberty to which both parties in this controversy appealed for the authority of their course. Such at least could never be the true spirit in which the meaning of a high constitutional guarantee should be construed and applied.  Plausibly then, were these resolutions denounced as substantial outrages.
Sentence 2: The Highlander in the pages of Redburn: It is on the right hand side of the Narrows as you go out, the land is quite high; and on the top of a fine cliff is a great castle or fort. All in ruins.
Target word: high
Judgement: 1

Sentence 1: If we bow our necks to the yoke longer, or move obedient to our task-masters!  Let us lay the axe to the very root of this evil and hew it down.  Even if we are crushed by the tree in falling!
Sentence 2: Soon only one strand remained uncut. She rolled from the razor and scraped this last strand against another exposed root of the oak until it parted. Two minutes more, and she was sitting up, unwinding the rawhide lariat from her legs.
Target word: root
Judgement: 2

Sentence 1: A car stolen stolen out of Orlando was stopped after the driver tried to speed away. A 2021 black Doge Charger took off from police Wednesday evening. The driver fled at a high rate of speed.
Sentence 2: There was one thing that struck me as particularly odd. Ronald Reagan never took his jacket off in the Oval Office in 8 years. Why?
Target word: take off
Judgement: 1

Example E: Judgment '-' (non_label)"


Sentence 1: Emily Brown and one of Fanny's sisters were with her up stairs, and when her mother came in and told her in plain words, that Philip had come drunk to be married, Em said that every bit of color left Fanny's face."

Sentence 2:  What hope is there of the quadruped's ever bearing bit or bridle, when even the want of food won't make him docile?"

Target word: bit

Please provide a judgment as a single integer. For example, if your judgment is Identical, then provide 4. If your judgment is Unrelated, provide 1.