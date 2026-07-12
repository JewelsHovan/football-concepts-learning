# Teaching casual fans to read football

Research notes and product direction for **The Football Field Guide**.

## Audience and outcome

**Primary learner:** curious casual fans who know football's basic rules and want to understand tactics, decisions, and statistics while watching a real match.

The product should not optimize for memorizing vocabulary. Its central outcome is **better match observation**: notice a useful cue, form a conditional explanation, predict what may happen next, and revise that explanation after the play unfolds.

## What the evidence suggests

### 1. Teach purposeful noticing, not “everything at once”

A match contains too much simultaneous information for a novice to process indiscriminately. The FA's observation guidance recommends narrowing attention to two or three purposeful cues; its “art of noticing” guidance similarly emphasizes specific observation targets and recording what was noticed. The FA also recommends looking away from the ball to understand player and unit relationships.

**Product implication:** each exercise and each real-match mission should provide one visual lens, such as space behind a press, the distance between units, or the reaction after a turnover.

Sources:
- [The FA — Developing the art of noticing](https://www.thefa.com/bootroom/resources/coaching/developing-the-art-of-noticing)
- [The FA — How to improve your matchday observation skills](https://www.thefa.com/bootroom/resources/coaching/how-to-improve-your-matchday-observation-skills)
- [The FA — How closely do your practices replicate the real game?](https://www.thefa.com/bootroom/resources/coaching/how-closely-do-your-practices-replicate-the-real-game)

### 2. Make learners commit before the explanation

Retrieval practice with feedback improves retention compared with rereading, including after multi-week delays. A meta-analysis of test-enhanced learning found transfer to new contexts, particularly when retrieval is elaborated and asks for application or inference rather than simple repetition.

**Product implication:** use a repeated loop of **look → choose/predict → reveal → explain → transfer prompt**. Do not reveal the expert overlay before the learner makes a call.

Sources:
- [Pan & Rickard (2018) — Transfer of test-enhanced learning: meta-analysis](https://pubmed.ncbi.nlm.nih.gov/29733621/)
- [Wiklund-Hörnqvist et al. (2014) — Repeated testing with feedback](https://pubmed.ncbi.nlm.nih.gov/24313425/)

### 3. Space and revisit ideas

A large review of 317 experiments found a robust distributed-practice effect; the most useful spacing depends on how long the learner needs to retain the material.

**Product implication:** save completed pictures locally, invite learners back to unseen or previously missed situations, and vary surface details while testing the same principle. Avoid a one-time “completed” badge as the learning endpoint.

Source:
- [Cepeda et al. (2006) — Distributed practice review and quantitative synthesis](https://pubmed.ncbi.nlm.nih.gov/16719566/)

### 4. Use visual cues carefully

Multimedia-learning research supports segmenting complex material, pre-training key concepts, worked examples for initial acquisition, and visual signaling that directs attention to relevant relationships. Research cited in the Cambridge multimedia-learning literature also warns that novices can attend to salient animation without extracting the important structure.

**Product implication:** show uncluttered pitch pictures, reveal one overlay only after a prediction, pair it with a concise verbal explanation, and then fade guidance on later scenarios.

Sources:
- [Cambridge Handbook — Worked Examples Principle](https://www.cambridge.org/core/books/cambridge-handbook-of-multimedia-learning/worked-examples-principle-in-multimedia-learning/8753055D1FB47CF1E2BB897FD44FBEF8)
- [Cambridge Handbook — Segmenting, Pre-training, and Modality](https://www.cambridge.org/core/books/abs/cambridge-handbook-of-multimedia-learning/principles-for-managing-essential-processing-in-multimedia-learning/DD24C2F48B9B1277CE59F78276110258)
- [Cambridge Handbook — Signaling or Cueing Principle](https://www.cambridge.org/core/books/cambridge-handbook-of-multimedia-learning/signaling-or-cueing-principle-in-multimedia-learning/3972D4ACC628D5B53F7B2B4785DB2B06)

### 5. Train attention away from the ball

Football visual-search research found that more experienced participants spent less time attending to the ball or ball carrier and extracted more information from other parts of the display in representative 3-v-3 situations.

**Product implication:** scenarios should explicitly ask learners to inspect runners, defenders, unit distances, and the next space—not only the player in possession.

Source:
- [Williams et al. — Visual search strategy, selective attention, and expertise in soccer](https://shura.shu.ac.uk/13272/)

### 6. Keep tactical problems representative and conditional

Ecological and representative-learning research treats decisions as emerging from interactions among players, opponents, space, time, and task constraints. Small changes to pitch size, numerical balance, or starting positions change the available decisions.

**Product implication:** teach “best given this picture,” not universal rules. Feedback should state the evidence, trade-off, and condition that would change the answer. Contrasting scenarios should vary one meaningful constraint.

### 7. Teach statistics as model literacy

Opta defines xG as the probability that a shot is scored based on similar historical shots, using context such as distance, angle, goalkeeper position, pressure, shot type, pattern of play, and previous action. Opta also explicitly warns that higher match xG does not mean a team “should have won,” and that variance is expected.

**Product implication:** retain the toy-model label, compare chances rather than claiming precision, expose important omitted variables, and always connect a number back to the match process that created it. For PPDA, field tilt, progressive actions, high turnovers, and possession-value models, state the guide’s counting rule because provider definitions and pitch zones differ.

Sources:
- [Opta Analyst — What Is Expected Goals (xG)?](https://theanalyst.com/articles/what-is-expected-goals-xg)
- [Stats Perform — Opta event definitions](https://www.statsperform.com/opta-event-definitions/)
- [StatsBomb — Possession value models explained](https://statsbomb.com/soccer-metrics/possession-value-models-explained/)
- [StatsBomb — Unpacking ball progression](https://statsbomb.com/articles/soccer/unpacking-ball-progression/)

## Product principles

1. **Transfer before trivia:** every concept ends with something to watch for in a real match.
2. **One lens at a time:** do not ask a learner to observe the whole game at once.
3. **Prediction before reveal:** require a small commitment before showing the cue.
4. **Conditional feedback:** explain evidence, trade-off, and what would change the read.
5. **Representative pictures:** include score, time, phase, teammates, opponents, and space where relevant.
6. **Contrast cases:** vary one detail and ask whether the best read changes.
7. **Stats need context:** numbers are clues, never verdicts.
8. **Accessible by default:** text alternatives, non-color cues, native buttons, keyboard use, reduced motion, and 44px touch targets.
9. **No empty gamification:** progress should support revisiting and practice, not points or streak anxiety.

## Recommended learning sequence

1. **See the space** — distance, angle, width, depth, and open lanes.
2. **See the shape** — listed formation versus in-possession and out-of-possession shape.
3. **Read the decision** — use pressure, support, and opponent positioning to compare actions.
4. **Read the turnover** — watch the first five seconds after possession changes.
5. **Read the numbers** — use xG, possession, and PPDA to ask better process questions.
6. **Take one lens into a match** — focus, mark an example, and reflect at halftime/full time.

## Development roadmap

### Implemented in the current development pass

- Four-picture Match Reader using look → commit → reveal → explain → watch.
- Scenario-specific text equivalents and explicit best-read feedback.
- One-lens match missions with three prompts tailored to the selected lens.
- Formation phase views for 4–3–3, 4–2–3–1, and 3–5–2, preserving player IDs while roles change.
- A segmented first-five-seconds transition lab comparing counterpressing with recovering shape.
- Three game-state variants showing how the clock and score change the interpretation of xG and possession.
- A predict-before-reveal xG range activity with a 100-shot replay.
- A three-round Sofa Stats Huddle introducing field tilt, box entries, high turnovers, progressive actions, and xA through shared interpretation.
- Purposeful, user-triggered motion for estimate reveals and comparative data bars, with reduced-motion support.
- A draggable offside diagram with snapping, live law feedback, and equivalent tap/arrow-key controls.
- Expandable stat cards that pair each definition with a concrete example and a better follow-up question.
- Animated scoreline contexts that explain how game state changes statistical interpretation.

### Phase 1 — match-reading loop

- [x] Add a reusable **Match Reader** with four illustrated scenarios.
- [x] Use the loop: look → commit → reveal overlay → explain → “watch for it.”
- [x] Save which pictures were attempted in local storage.
- [x] Add a **one-lens match mission** selector.

### Phase 2 — deepen existing modules

- [x] Add `Listed / With ball / Without ball` views to the formation explorer.
- [x] Add a segmented first-five-seconds transition sequence.
- [ ] Add pressing triggers to the existing pressing workshop.
- [x] Ask learners to estimate an xG range before revealing the toy model.
- [x] Add game-state variants to the scoreline/statistics exercise.

### Phase 3 — retrieval and contrast

- Revisit previously attempted concepts with changed player positions or match context.
- Add paired “what changed?” scenarios.
- Track concepts that need another look locally, without accounts or streaks.

### Later, only if validated

- Set-piece reader.
- Substitution and game-state scenarios.
- Curated real-clip links with licensing and accessibility reviewed.

Avoid for now: accounts, leaderboards, live data feeds, a large video library, or claims that the teaching xG model is provider-grade.

## How to evaluate success

Completion is not enough. Test whether a casual fan can handle an **unseen** match picture or clip and:

- identify the most useful space;
- look away from the ball;
- predict a plausible next action using evidence;
- name the tactical trade-off;
- interpret a statistic conditionally;
- revise the explanation after seeing what happened.
