# Research basis

Checked 2026-11-02. These sources inform the workflow; none establishes a recipe for virality. Keep **conversation-page ranking**, **Home/For You distribution**, and **people choosing to share** separate.

## X's published documentation

### 1. Conversation order is personalized, not a race to be first

[X: Conversations Recommendations](https://help.x.com/en/resources/recommender-systems/conversations-recommendations) documents algorithmic ordering using factors including followed accounts, replies answered by the original author, verification, and viewer/author relationships. Its engineering overview balances recent and high-ranked candidates, scores predicted positive and negative engagement, and selects conversation branches. Latest and Likes are separate sorting options.

**Workflow implication:** assess relevance, current activity, and whether an unanswered contribution remains possible. A crowded thread can limit discoverability, but reply count alone is not a measured probability of success. An actual author reply is a documented factor; generic praise is not a documented ranking shortcut.

**Limit:** this is the documentation available on the check date, not an independently measured production system. Its architecture and candidate counts may lag deployment. It supplies no universal first-N-replies, minutes-since-post, or minimum-views rule, and no causal effect size for a writing tactic.

### 2. Public replies and Home distribution are different

[X: About conversations](https://help.x.com/en/using-x/x-conversations) explains that public replies can be found in conversations, while Home visibility is limited to relevant people; it suggests reposting or quoting when an author wants more followers to see a reply. It also describes nonchronological sub-conversation ranking and original-author interaction as a factor.

**Workflow implication:** evaluate the reply as part of its actual conversation. Do not promise that replying below a large account exposes the reply to that account's entire audience.

**Limit:** publication, eligibility for a surface, position on that surface, and actual reach are different outcomes. This help page does not quantify reach or prove that reposting guarantees additional distribution.

## Dated public implementation

### 3. A For You snapshot is not the conversation algorithm

[xai-org/x-algorithm README at commit `9106e9f`](https://github.com/xai-org/x-algorithm/blob/9106e9f33ee9cc6a92929fc798ae6c566e2841cb/README.md), [committed 2026-10-31](https://github.com/xai-org/x-algorithm/commit/9106e9f33ee9cc6a92929fc798ae6c566e2841cb), describes the **For You feed**: personalized retrieval, predicted actions and attention, weighted scoring, diversity adjustments, and separate visibility filtering. The README explicitly says weights scale predictions rather than raw engagement counts, and discusses production configuration/experiments.

**Workflow implication:** audience fit and reader value are more useful goals than mechanically farming one visible count. Never translate published weights into claims such as one reply being worth a fixed number of likes.

**Limit:** a public code/configuration snapshot is not a production audit, a causal writing experiment, or documentation of the conversation page. Do not transfer its filters, defaults, or weights into universal reply rules. Recheck dated claims before updating algorithm-specific advice.

## Research on sharing: useful hypotheses, not X rules

### 4. Emotion, interest, surprise, and usefulness

[Berger & Milkman (2012), *What Makes Online Content Viral?*](https://doi.org/10.1509/JMR.10.0353) ([author-hosted paper](https://jonahberger.com/wp-content/uploads/2013/02/ViralityB.pdf)) combines New York Times sharing data with experiments. Its evidence links interesting, surprising, practically useful, and activating emotional content with transmission; experiments examine emotional activation, including amusement.

**Workflow implication:** try a useful explanation, a surprising but supported observation, or fitting humor when it serves the conversation. Give someone a reason to pass the idea along.

**Limit:** much of the observational evidence concerns emailed news articles; the experiments do not establish current X reply performance. Humor is an option, not a requirement. Emotional activation does not justify outrage bait or establish that negativity always wins.

### 5. A message has a recipient and a sharing audience

[Barasch & Berger (2014), *Broadcasting and Narrowcasting*](https://doi.org/10.1509/jmr.13.0238) reports six studies: one-to-one communication increased attention to recipient usefulness, while broadcasting increased self-presentation concerns.

**Workflow implication:** identify who the reply helps and why another reader might want to repeat it. An answer to one person can also contain an insight useful to the wider audience.

**Limit:** these studies concern communication and sharing choices, not X ranking. Applying them to a public reply with both a named recipient and an observing audience is an extrapolation.

## Editorial choices to test locally

The following are design judgments drawn from the sources, not proven ranking inputs:

- Read the original post and existing replies. Add an answer, example, distinction, evidence, useful question, or fitting joke that is still missing.
- Prefer a specific contribution to interchangeable agreement. Praise can work when it explains something concrete; these sources contain no controlled test proving that generic praise always loses.
- Treat timing and crowding as context. Join while a conversation is active and there is room to contribute; retain no universal numeric thresholds.
- Compare like-for-like reply attempts within the user's audience. Record observable outcomes without attributing a result to one tactic from a single example.
- A reply can succeed by helping someone or starting a worthwhile exchange, even when it is not widely shared.
