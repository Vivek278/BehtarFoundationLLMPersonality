**INDUCING PERSONALITY IN LLMs (PROMPTING AND EVALUATION)**

1. *Personality Prompting using OCEAN traits* ([paper link](https://arxiv.org/pdf/2206.07550))

Summary:
* 3 step prompting:-
(i) Single line summary of personality
(ii) List of keywords and negative list of keywords
(iii) Self prompting (LLM itself generates descriptions of keywords)
Final system prompt: Use all of the above 3
* Evaluation:-
(i) 10 traits: OCEAN * 2 (+ve, -ve for each trait in OCEAN)
(ii) Dataset: Labelled dataset of behavioural statements and their corresponding personality trait (from 10)
(iii) LLM rates itself from 1 to 5 for each statement, trait.
(iv) Mean and variance of score calculated to measure personality and consistency. The score is compared to that of a human.



2. *Controlling personality intensity + 16 traits* ([paper link](https://arxiv.org/pdf/2506.20993))
Novelty:
(i) Manually created list of adjectives for each intensity level for each of the 16 traits.
(ii) 5 dimensions of measurement for each trait: frequency, depth, thereshold, effort, willingness (these dimensions used to create dataset of questions for evaluation)
(iii) Prompt during evaluation as LLM rates itself: Traits + Intensities + Adjective list + Dimension-based question
