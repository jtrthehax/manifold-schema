## Abstract

Natural language is not a meaning-transfer system. It is a compression function. The sender compresses intent into surface tokens. The receiver decompresses those tokens using their own dictionary. The meaning that arrives at the receiver's end is not the meaning that left the sender's — it is a reconstruction, shaped by the receiver's prior distribution, their residual schema distance from the sender, and their regulatory state at the moment of decompression. Divergence is not the exception. It is the default.

Meaning is type binding, not token matching. Every word in every sentence carries implicit type properties — category, valence, scope, constraint, and relationship — that the receiver must resolve before the word can participate in the sentence's meaning. When those types are declared explicitly, decompression fidelity is high. When they are left implicit, fidelity is a function of residual schema distance and constraint density. The relationship is expressible as a single equation:

$$H \propto \frac{\delta}{D}$$

where δ is the residual schema distance between sender and receiver dictionaries — the gap that remains after the input's explicit constraints have done their binding work — and D is the constraint density of the input. This is a property of the transaction between the input and the receiver's current dictionary, not of the receiver's capacity alone. D is the lever the sender controls. δ is a relational property that changes with the receiver's regulatory state independently of the input.

_This initial formulation captures the sender-side contribution to divergence — what was left implicit relative to what was made explicit. It is necessary but not sufficient. Two additional terms complete the account._

_T is the receiver's decompression topology — the geometry of how they traverse argument space for a given input. In human receivers, T is shaped by prior distribution, institutional training, regulatory state, and compliance conditioning. In AI receivers, T is shaped by training data, objective function, and alignment procedures. T is not fixed. It is modified by everything that shaped the receiver before the input arrived. The same input produces different outputs across different T values regardless of δ/D._

_S is the receiver's sampling policy — whether decompression preserves uncertainty or collapses it. A receiver who synthesises a single binding and proceeds as though it were resolved has applied S = argmax. A receiver who flags the gap, expresses uncertainty, or requests clarification has preserved branching. S = argmax applied to high δ/D input produces fabricated certainty. The output is coherent. The divergence is invisible. The receiver does not know they are wrong._

_The complete relationship is:_

$$H = f\left(\frac{\delta}{D}, T, S\right)$$

_δ/D is the input property the sender controls. T is the receiver architecture the receiver brings. S is the output policy the receiver applies. All three contribute independently to divergence. Fixing only δ/D — shipping more explicit constraints — does not address a receiver whose T is ossified or whose S has collapsed._

When human receivers encounter missing types, they detect the gap and negotiate — clarification is type negotiation, an iterative alignment of dictionaries before synthesis proceeds. When that detection fails, the receiver synthesises a binding from prior distribution and proceeds as though the type were resolved. The output is coherent. It diverges from the sender's intent in proportion to the unresolved residual schema distance. This is structurally identical to AI hallucination. The difference is the dictionary: human gap-filling draws from biographical prior, AI gap-filling draws from population-average training distribution. The failure type is the same. The substrate is different.

Both failure modes are linguistic inevitabilities, not receiver defects. No one can read minds. The sender's intent is not in the tokens. It can only be recovered by a receiver whose dictionary is close enough to the sender's, given the constraints that were shipped. When those conditions are not met, synthesis occurs. The synthesis is always faithful to the receiver's dictionary. It is wrong in proportion to what the input did not contain.

This paper does not claim to discover that meaning is inferred rather than transmitted — that position has roots in Grice's cooperative principle, relevance theory, and the hermeneutic tradition. It claims to operationalize that insight as a formal equation with defined boundary conditions, a measurable variable in constraint density, and a diagnostic instrument in the Semantic Deconstruction Engine. The position was known. The instrument was not.

The Semantic Deconstruction Engine is the applied demonstration of this mechanism — a structural audit pipeline that detects missing types, undeclared constraints, and misbound variables before synthesis occurs, operationalising the theoretical account as a predictive instrument. Its flag registry is a taxonomy of type failures. Its compression score is a measurement of constraint density. Its flag density serves as the operational proxy for residual schema distance, with validation ongoing.

Language as a typed system is not a metaphor. It is the mechanism. The forward direction is building communication systems — human and AI — that ship explicit decompression dictionaries rather than assuming the receiver will supply what the input did not — and that preserve branching rather than collapsing uncertainty into fabricated certainty at the output layer, regardless of how well-formed the input was.

---

## Section 1 — The Assumption Everyone Makes
## 1.1 The Assumption Everyone Makes

Communication feels like meaning transfer. A speaker has a thought, converts it into words, and delivers those words to a listener, who receives the meaning. The thought travels from one mind to another. This is the intuitive account, and it is wrong in a precise and consequential way.

What travels is not meaning. What travels is tokens — sounds, symbols, marks on a page, pixels on a screen. The meaning does not travel with them. The sender had meaning before the tokens were produced. The receiver constructs meaning after the tokens arrive. Between those two events, the tokens were in transit, carrying nothing except their surface form.

This distinction is not philosophical pedantry. It is the load-bearing claim of everything that follows. If meaning transferred, divergence between sender intent and receiver output would be a failure requiring explanation — something went wrong in the channel, or the receiver was inattentive, or the sender was unclear. If meaning is constructed at the receiver's end, divergence is the default — the expected output of two systems operating on different dictionaries with insufficient shared constraints. No explanation is required. The divergence is predicted.

The assumption of meaning transfer is not naïve. It is held by careful thinkers, skilled communicators, and experienced institutions alike. It persists because it is approximately correct across a narrow range of conditions — when sender and receiver share a dictionary, a history, a domain, and a regulatory state, the decompression at the receiver's end closely matches the sender's intent. The approximation holds well enough that the gap between transfer and construction is invisible in practice. The assumption survives because the conditions that expose it are treated as exceptions rather than as the normal case with better visibility.

AI removed the conditions that sustained the approximation. The result was not a new problem. It was an old problem without the cover that had always concealed it.

---

## 1.2 The Compression Function

Every sentence is a compression function. The sender begins with an intent — a state of meaning that exists in their mind with full context, full type bindings, full valence assignments, and a complete set of referents. They compress that intent into surface tokens: words, ordered into a sentence, delivered to the receiver. The tokens are smaller than the intent. They have to be. Language is efficient precisely because it does not transmit everything the sender knows — it transmits a compressed representation and relies on the receiver to reconstruct the rest.

The receiver performs the inverse operation: decompression. They receive the tokens and apply their dictionary to them — their full type-resolution system, shaped by biographical history, domain knowledge, current regulatory state, and every prior encounter they have had with those tokens in similar contexts. The dictionary draws on the receiver's prior distribution — the statistical substrate assembled from that accumulated experience — when explicit constraints in the input are absent. The output of the decompression is the meaning they construct. If their dictionary matches the sender's closely enough, and the compression shipped sufficient constraints to guide the decompression, the output approximates the sender's intent. If either condition fails, it does not.

The ideal compression ships a decompression dictionary alongside the tokens — a complete set of type bindings explicit enough that the receiver can decompress without drawing on their own prior distribution to fill gaps. In practice, most compressions do not ship a decompression dictionary. They assume the receiver's dictionary is close enough to the sender's that the gaps will fill correctly. That assumption is the source of every failure this paper describes.

Decompression fidelity — how closely the receiver's constructed meaning matches the sender's intent — is therefore a function of two variables. The first is constraint density: how explicitly the compression binds the types it uses. A compression that names its referents, defines its operations, and declares its scope gives the receiver's decompression more to work with. A compression that leaves its key terms undefined, its operations implicit, and its scope assumed gives the receiver less. The second variable is schema distance: how far apart the sender's and receiver's dictionaries sit. Two receivers decompressing the same input will produce outputs that diverge from each other in proportion to the distance between their dictionaries — and diverge from the sender's intent in proportion to the distance between each receiver's dictionary and the sender's.

This is not a metaphor imported from computer science to make a point about language. It is the operational description of what language does. Compression and decompression are not analogies for communication — they are the mechanism. The sender compresses. The tokens transmit. The receiver decompresses. Every other property of communication follows from those three operations and the conditions under which they succeed or fail.

---

## 1.3 Why the Illusion Holds

If meaning is constructed rather than transferred, and divergence is the default rather than the exception, the question that requires explanation is not why communication fails — it is why it appears to succeed as often as it does. The illusion of meaning transfer is stable enough that it has sustained an entire folk theory of communication across the whole of recorded human history. That kind of stability requires a mechanism.

The mechanism is shared substrate. The term covers three distinct layers that operate differently and must be kept separate. The first is biological substrate: human senders and receivers are built from the same nervous system architecture, acquire language through the same developmental process, and operate on bodies that process sensory input through the same physiological mechanisms. This layer is the deepest and the most stable — it establishes the floor below which schema distance cannot fall between any two human communicators, and it is not removed by any technology. The second is cultural substrate: shared language, shared conceptual categories, shared referent pools assembled through participation in overlapping social and institutional contexts. This layer narrows schema distance within communities but varies across them — two people who share a language but not a domain or subculture have less cultural substrate in common than their shared vocabulary suggests. The third is relational substrate: the accumulated alignment built through direct interaction between specific communicators — shared history, corrected misunderstandings, and the private compression format that sustained exchange produces. This layer is the most local and the most powerful schema distance reducer, but it exists only between parties who have actually communicated.

Shared history compounds the effect of cultural substrate. A sender and receiver who have communicated extensively over time have iteratively narrowed their schema distance through accumulated clarification, correction, and alignment. They have built a private compression format on top of the cultural substrate — a shared dictionary more efficient than public language because it carries more constraint per token, having been assembled through repeated cycles of compression, decompression, and realignment. Long-term partners, close colleagues, and experienced collaborators compress more tightly and decompress more accurately not because they read each other's minds, but because they have reduced their schema distance through sustained exposure. The illusion of mind-reading is the subjective experience of very low schema distance operating on high constraint density input.

AI removed the cultural and relational substrate — not the biological, which was never shared. A model trained on a population-average corpus does not share cultural context with any specific sender in the way a community member does, does not carry the accumulated alignment of prior exchanges, and holds none of the private compression formats that reduce schema distance between specific pairs of communicators. The biological substrate difference is real and in the opposite direction from removal: human receivers share nervous system architecture; the model does not. What AI removed is the cultural and relational substrate that human communication had always relied on to close the gap that biological substrate alone cannot close. Every compression arrives at the model without the two layers that do the most gap-closing work. The schema distance defaults to population-average. The dictionary draws on population-average prior distribution rather than on any shared history with this sender. The decompression defaults to statistical prior.

The result was not a new failure mode. On the structural account, every compression the model decompressed incorrectly was simultaneously being decompressed incorrectly by human receivers with equivalent residual schema distance from the sender — it was just being absorbed into the social record as ordinary misunderstanding, attributed to inattention or imprecision rather than to the structural gap that produced it. The equivalence is a prediction of the mechanism, not an independently measured finding: if divergence is a function of residual schema distance and constraint density, then any receiver — human or model — operating at the same residual schema distance from the sender and receiving the same underspecified compression should produce equivalent divergence rates. AI made the invisible visible not by introducing the gap but by removing the cultural and relational substrate that had always concealed it. The biological substrate was always different. The mechanism was there. The cover was not.

---

## Section 2 — Every Word Has an Implicit Type
### 2.1 Every Word Has an Implicit Type

Words are not atomic units of meaning. They are typed variables — containers whose surface form is stable but whose content is determined by the type properties the receiver assigns to them during decompression. Those properties are not visible in the token. They are inferred, automatically and almost instantaneously, from the receiver's dictionary. The inference feels like reading. It is closer to compilation.

Every word carries at minimum five implicit type properties, each of which the receiver must resolve before the word can participate in the sentence's meaning. These five — type, valence, scope, constraint, and relationship — are not claimed to be an exhaustive set. They are the properties that account for the failure modes the SDE observes across its corpus, and they are sufficient to ground the flag registry developed in Section 10. Other linguistic dimensions — tense, modality, presupposition, illocutionary force — are real and may warrant extension of the taxonomy. The five here are the working set. A type property can be either implicit — present in the word but not declared by the sender, left for the receiver's dictionary to resolve — or missing — absent from the input entirely. Both force synthesis, but through different mechanisms: an implicit type gives the receiver's prior distribution something to work with; a missing type gives it nothing except the surrounding context. Both are addressed in the sections that follow.

**Type** is the word's categorical identity — the domain and role it occupies in the receiver's ontology. *Bank* resolves to a financial institution or a riverbank depending on which domain the receiver's decompression function selects. The token is identical. The type is not.

**Valence** is the word's affective charge — positive, negative, or neutral — as assigned by the receiver's dictionary in the current context. *Disruption* carries positive valence in an entrepreneurial context and negative valence in an operational one. The token did not change. The valence assignment did.

**Scope** is the word's reach — whether it applies locally or globally, personally or institutionally, to this instance or to a general class. *Everyone* in a casual conversation means the people in the room. *Everyone* in a policy document means a population. The token is the same. The scope is not.

**Constraint** is the word's boundary conditions — its cardinality, its domain limits, the range of referents it can legitimately bind to. *Some* is unconstrained by default and must be bounded by context. *Three* is maximally constrained. The difference between them is not stylistic — it is the difference between a variable that forces synthesis and a variable that does not.

**Relationship** is the word's position in the sentence's type hierarchy — whether it is a parent term that governs downstream resolution, a child term whose meaning is constrained by what preceded it, or a modifier that shifts the type properties of its target. *Not* is a relationship operator that inverts the valence and constraint of every term it governs. Its surface form is three letters. Its structural effect propagates through the remainder of the inference path.

These are not properties of well-written language versus poorly-written language. They are not style properties that careful writers attend to and careless writers ignore. They are structural properties of every word in every sentence in every language — present regardless of whether the sender declares them, resolved by the receiver's dictionary regardless of whether the sender intended a specific resolution. When the sender declares a type property explicitly, the receiver's decompression is guided. When the sender leaves it implicit or absent, the receiver's prior distribution fills the gap. The sender who does not declare these properties does not eliminate them. They hand the resolution to the receiver's prior distribution and accept whatever binding the receiver's dictionary produces.

That is the transfer of control that makes synthesis inevitable.

---

### 2.2 Implicit vs Explicit Types

The five type properties described in Section 2.1 are present in every word of every sentence. What varies is not whether they exist — it is whether the sender declares them or leaves them for the receiver to resolve. Declared types are explicit: the sender binds the variable before handing it to the receiver. Undeclared types are implicit: the sender leaves the binding to the receiver's prior distribution. Most language, most of the time, is almost entirely implicit.

This works for humans under the conditions described in Section 1.3. When shared substrate and shared history have reduced schema distance sufficiently, the receiver's prior distribution produces bindings that approximate the sender's intent closely enough that the gap is not detected. The receiver resolves the implicit types automatically, without awareness that resolution occurred, and the decompression proceeds. The implicit types were never declared. They were inferred correctly anyway. The illusion of meaning transfer holds because the inference succeeded.

The inference is not guaranteed to succeed. It succeeds in proportion to schema distance and constraint density — the same two variables that determine decompression fidelity across all receiver types. When schema distance is low and the surrounding context provides sufficient constraint, implicit type resolution is accurate. When schema distance is high, or the surrounding context is sparse, or the receiver's regulatory state has shifted their dictionary away from its baseline, the inference produces the wrong binding. The receiver resolves the implicit type confidently, proceeds on the basis of the wrong binding, and constructs a meaning that diverges from the sender's intent. The failure is invisible to both parties until it surfaces in behaviour.

AI cannot perform implicit type resolution in the same way. A human receiver who encounters an undeclared type has biographical fallback — shared history, embodied context, and a private compression format that narrows the candidate set before inference begins. An AI receiver has none of these. The model has no history with this sender, no embodied context, no private compression format. When it encounters an undeclared type, it draws from the full population-average prior distribution — the statistical centre of mass of all contexts in which that token has appeared across training data. The binding it produces is not informed by this sender's intent. It is informed by what that token most frequently meant to everyone. The model's dictionary is populated from population-average training data rather than from any shared history with this sender.

The consequence is that implicit types, which human receivers resolve approximately correctly under favourable conditions, become maximum-uncertainty variables for AI receivers. The model is not less capable than the human receiver — it is operating on a structurally different dictionary with no access to the local context that would narrow the candidate set. The failure is not architectural. It is informational. The implicit type was never declared. The model had no basis for resolving it other than population-average prior distribution. That distribution is not this sender's dictionary.

Ambiguity is therefore not a property of words in isolation. It is a relational property of words and the dictionaries being applied to them. A term that is unambiguous between two people who share a history and a domain is maximally ambiguous when the same term is received by a system with no access to that history or domain. The ambiguity was always present in the token — the shared substrate and private compression format were suppressing it. When both are absent, the suppression fails and the ambiguity is exposed.

Synthesis is the formal term for what colloquially is called gap-filling. Where inference appears in this paper, it refers to the specific mechanism by which synthesis traverses the prior distribution to select a binding. A receiver who cannot resolve a type from explicit constraints will resolve it from implicit ones. If the implicit constraints are insufficient, the receiver synthesises a binding from prior distribution. The synthesis will be coherent. It will be confident. It will be wrong in proportion to the gap between the sender's intent and the receiver's prior distribution. That proportion is what the next section formalises.

---

### 2.3 The Hallucination Equation

Decompression fidelity is not a post-hoc measurement — it is predictable from the input before generation occurs.

The relationship can be expressed as:

$$H \propto \frac{\delta}{D}$$

where δ is the residual schema distance between the sender's dictionary and the receiver's dictionary — the gap that remains after the input's explicit constraints have done their binding work — and D is the constraint density of the input, the degree to which the input explicitly binds the types it uses.

Two formal boundary conditions must be named. First, as D increases without bound, H does not go to zero — it approaches a nonzero floor. Natural language cannot make every type explicit simultaneously: every compression leaves some implicit types for the receiver's prior distribution to resolve, and residual schema distance cannot be fully eliminated between any two distinct receivers. The claim is not that hallucination is eliminable. The claim is that hallucination rate decreases asymptotically as constraint density increases. The floor is not universal — it is a property of the encoding format the sender chooses. Natural language carries an inherently higher synthesis floor than structured formats: English requires the receiver to resolve ambiguity that YAML resolves by construction. A well-formed YAML document cannot contain an undefined term without the structural absence being detectable — the format enforces constraint density at the schema level rather than relying on the sender's care in any given compression. The synthesis floor for structured encoding approaches the interpretive minimum — the shared parsing conventions required to read the format itself. The synthesis floor for natural language is substantially higher, because natural language tolerates implicit types that structured formats do not permit. This is the rigorous grounding for Section 9's claim that structural encoding is categorically different from constraint specification: it does not merely increase D, it lowers the floor H is approaching. Second, δ is not directly observable as a scalar — it is a relational property of a specific sender-receiver pair on a specific domain that changes with the receiver's regulatory state independently of the input. 

The operational proxy for δ is flag density as measured by the Semantic Deconstruction Engine, with validation ongoing. A compression that produces high flag density has exposed large residual schema distance between what the sender assumed and what the input constrained. A compression that produces low flag density has closed that gap through explicit binding. The equation predicts; the SDE approximates.

The two variables are not independent. D acts on δ. When constraint density is high — when the sender has explicitly bound the types the compression uses — the receiver's prior distribution is replaced by the sender's declared bindings at each resolution step. The operative residual schema distance shrinks: what the receiver would have inferred from their own dictionary is overwritten by what the sender specified. The residual δ applies separately to each of the five type properties — type, valence, scope, constraint, and relationship — and can vary across them. A compression that binds scope but leaves valence implicit has low residual δ on scope and high residual δ on valence. The equation's H is the aggregate over all five — not necessarily a simple average or a linear sum, but sensitive to all five simultaneously. The SDE's flag weights are the operational implementation of that aggregation. The unbounded properties — whichever of the five the sender left implicit — are still resolved by the receiver's prior distribution at their individual residual δ.

D reduces residual δ asymptotically, not fully. Even the most explicit binding requires the receiver's prior to interpret the binding itself: the operation *summarise* is not a fixed function — it is a type whose resolution varies across receivers. Every explicit binding is itself a token that must be typed. The floor on H is the floor on what D cannot bind — the interpretive frame within which all explicit bindings are processed.

This is a property of the transaction between the input and the receiver's current dictionary — not of the receiver's capacity alone, and not of the input alone. D is a property of the input. δ is a relational property that changes with the receiver's regulatory state independently of the input: the same compression arriving at the same receiver in a different regulatory state produces a different residual schema distance and a different hallucination rate. The equation holds in both cases. What varies is which variable is doing the work. The sender controls D directly and influences residual δ indirectly — through explicit binding that reduces it regardless of the receiver's state. D is the lever the sender controls. It is not the only variable in the transaction. It is the only one the sender can pull.

**Worked example.** Consider the prompt: *"Write something about the situation."*

- All five type properties are unbound: *situation* carries no type (no domain), no valence assignment, no scope, no constraint, no declared relationship to anything else in the input
- D approaches zero: no variable is bound, no operation is defined, no constraint is declared
- Residual schema distance is the full distance between sender intent and receiver prior distribution across all five properties
- The receiver synthesises a decompression dictionary from population-average priors
- The output will be fluent, structured, and entirely determined by what *situation* most frequently precedes in training data
- The sender's intent was never in the input

Now constrain it: *"Summarise the three primary causes of the 2008 financial crisis, focusing on mortgage-backed securities, in 200 words for a non-specialist audience."*

- Type is bound: financial history, specifically the 2008 crisis
- Valence is bound: neutral analytical framing, not advocacy
- Scope is bound: three causes, mortgage-backed securities focus
- Constraint is bound: 200 words, non-specialist register
- Relationship is bound: *summarise... focusing on* declares the operation and its modifier
- Residual schema distance is limited to the interpretive frame — what *summarise* means at this level of compression, what *non-specialist* permits, what *200 words* implies about depth
- Hallucination probability drops sharply — not because the model improved, but because D did the work that residual δ would otherwise have handed to the receiver's prior distribution

The equation does not say hallucination is eliminable. It says hallucination rate is a function of the transaction — the interaction between constraint density and residual schema distance across all five type properties — approaching its format-specific floor asymptotically as D increases and residual δ shrinks. The floor itself is lower for structured encoding than for natural language, which means the choice of format is a boundary condition decision, not just a style decision. The claim is not perfection. The claim is that D is the lever the sender controls, that the format determines the floor D is working toward, and that current practice leaves both largely unconsidered.

---

### 2.4 Why This Is Not an AI Problem

The field has a strong institutional incentive to frame hallucination as a model defect. If hallucination is a property of the model, it is an engineering problem — tractable, fundable, and solvable by the people who built the model. If hallucination is a property of the input, it is a language problem — which is everyone's problem, which predates AI by the entire history of human communication, and which no amount of model improvement will eliminate.

The equation does not care which framing is more convenient.

$$H \propto \frac{\delta}{D}$$

Both δ and D are properties of the communicative transaction, not the receiver. A human receiver with high schema distance from the sender and a low-constraint input will produce a divergent interpretation just as reliably as a model will [^1]. The receiver changes. The failure structure does not.

The objection that will be raised here is that human receivers have something models do not: shared history, embodied context, and the ability to ask clarifying questions. This is true, and it matters. But it does not change the structural claim — it changes the *default value of δ*. A human receiver who shares history with the sender starts with a lower schema distance than a model drawing on population-average training data. Lower δ means lower H. It does not mean H = 0, and it does not mean the mechanism is different.

The clarification capacity is also worth examining directly. Humans ask clarifying questions when they detect a type mismatch — when they notice that they cannot decompress the input without synthesising a type they are uncertain about. This detection is not infallible. It fails under time pressure, social load, and regulatory state compression [^2]. When it fails, the human does not pause and request more constraint — they synthesise, exactly as a model does, and the output diverges from the sender's intent in proportion to the unresolved schema distance. The human does not experience this as hallucination. They experience it as understanding. The sender experiences it as being misunderstood. The mechanism is identical.

What makes AI hallucination visible is not that it is structurally different from human misunderstanding. It is that AI outputs at scale, without the social friction that conceals human gap-filling as it happens. A model's synthesised interpretation is rendered as text, available for inspection, and attributed to the model. A human's synthesised interpretation is rendered as behaviour, attributed to the person, and absorbed into the social record as a misunderstanding or a disagreement rather than a generation failure.

The AI made the invisible visible. The mechanism was always there [^3].

This paper will not concede that the visibility difference is sufficient to sustain the categorical distinction between hallucination and misunderstanding. The distinction is a naming convention that protects a framing, not a structural finding. The structure is the same. The substrate is different. The substrate difference determines the dictionary, not the failure mode.

---

## Section 3 — The Clarification Mechanism
## 3.1 The Clarification Mechanism

When a human receiver encounters a type they cannot resolve from the constraints provided, they have an option that no other receiver type has: they can stop and ask. The question takes different surface forms — "what do you mean by that?", "can you give me an example?", "are you talking about X or Y?" — but the structural operation is always the same. The receiver has detected a gap in the decompression dictionary. They are requesting the missing constraint before proceeding.

This is not a communication failure. It is the communication system working correctly. The receiver identified an undeclared type, recognised that their prior distribution produced multiple candidate bindings with insufficient grounds for selecting among them, and held the gap open rather than synthesising a resolution. The clarification request is the signal that the detection mechanism fired. It is the most valuable output the receiver can produce when constraints are insufficient — more valuable than a fluent response built on a synthesised binding that neither party knows is wrong.

Clarification is type negotiation. The sender and receiver are not exchanging pleasantries about what was meant — they are iteratively aligning their dictionaries, narrowing the schema distance on the specific term that failed to resolve, until the constraint density is sufficient for decompression to proceed with a shared binding. Shared meaning does not exist prior to this negotiation. It emerges from it. The alignment is the meaning.

This has a consequence that runs counter to the intuitive account of communication: fluent exchange is not evidence of successful decompression. It is evidence either that schema distance was low enough for implicit type resolution to succeed, or that the receiver synthesised a binding from their prior distribution and proceeded without detection. Both produce fluent exchange. Only the first produces aligned meaning. The clarification request, which interrupts fluency, is therefore a more reliable signal of communicative health than the smooth conversation that never required one.

The detection mechanism is not infallible. When the receiver's regulatory state is elevated — narrowing their prediction window and truncating the candidate referent set before gap detection can occur — the clarification mechanism may fail to fire even when the decompression dictionary is critically incomplete. That failure mode is developed in Section 4. When the detection mechanism fires correctly, the system is doing exactly what it should. The gap was always there. The clarification made it visible.

---

## 3.2 Misunderstanding as Human Hallucination

When a human receiver produces an interpretation that diverges from the sender's intent, the standard account calls this a misunderstanding. The word is descriptive but it obscures the mechanism. The receiver did not fail to understand — they understood precisely, using their own dictionary. The failure is not in the decoding operation. The failure is in the assumption that both parties were operating on the same decompression key.

This is not a distinction without a difference. If misunderstanding is framed as a comprehension failure, the remedy is attention, effort, or goodwill — try harder, listen better. If misunderstanding is framed as a type mismatch, the remedy is constraint — make the types explicit before synthesis occurs. These are different interventions targeting different causes.

The structural account is this: the sender compressed their intent into surface tokens. The receiver decompressed those tokens using their own prior distribution over what those types mean. The output was internally consistent and faithfully produced — it was just drawn from a different dictionary than the sender used. The receiver did not hallucinate in the colloquial sense. They hallucinated in the technical sense: they generated a coherent output from insufficient constraints, and the output diverged from the sender's intent in proportion to the residual schema distance between their dictionaries.

The AI case differs in one respect only: the dictionary. A human receiver's prior distribution is built from a specific biographical history — shared context, relationship history, domain overlap, and current regulatory state. An AI receiver's prior distribution is built from a population-average training corpus. The synthesis operation is identical. The dictionary used to perform it is not.

This means the categorical distinction between misunderstanding and hallucination cannot be grounded in the failure type — because the failure type is the same. It can only be grounded in the substrate. And substrate is not a principled boundary for a phenomenon defined by its mechanism.

The resistance to this equivalence is predictable and worth naming directly: hallucination feels like a defect because it comes from a machine; misunderstanding feels like a normal social event because it comes from a person. This is an intuition about the source, not an argument about the structure. The structure is identical. The source is different. The paper will not concede that the source difference is sufficient to sustain the categorical distinction.

---

## 3.3 Shared History as Partial Compression

Long-term relationships reduce schema distance. This is the mechanism behind the intuition that people who know each other well communicate more easily than strangers — not because familiarity produces mind-reading, but because accumulated interaction has iteratively narrowed the gap between their dictionaries. Every clarification exchange, every corrected misunderstanding, every shared experience that established a common referent has added a constraint to the private compression format they operate on. The private compression format is a shared dictionary more efficient than public language because it carries more constraint per token — each exchange has pre-loaded type bindings that no longer need to be declared explicitly, reducing the decompression work the receiver must perform on every subsequent compression from that sender.

This is a genuine advantage. It is not, however, elimination of the gap. Shared history reduces schema distance. It does not close it. The dictionaries continue to diverge along every dimension that the shared history did not explicitly address — new domains, new experiences, new regulatory states, new valence assignments acquired independently since the last alignment. The private compression format covers the territory that has been negotiated. Everything outside that territory remains subject to the same implicit type resolution failures that apply between strangers, because the receiver's prior distribution has no shared-history constraint to draw on in those domains.

The reduction in schema distance produces a secondary effect that is less benign: it increases the assumption of shared types. A sender who has communicated successfully with a receiver over a long period accumulates evidence that their compressions decompress correctly. That evidence is accurate for the domains and terms the private compression format covers. It is not accurate for domains and terms outside that coverage. But the evidence does not distinguish between the two cases. The sender generalises from successful decompression in covered territory to an assumption of shared types across all territory. The assumption is invisible — it does not feel like an assumption, it feels like knowing the person — and it is proportionally wrong in exactly the domains where the private compression format provides no coverage and the receiver's prior distribution has nothing shared-history to anchor to.

The cost of discovering the assumption was wrong scales with relationship length. Between strangers, a type mismatch surfaces quickly — the schema distance is legible, the assumption of shared types is low, and the clarification mechanism fires before synthesis has propagated far. Between long-term partners, colleagues, or collaborators, the assumption of shared types is high, the clarification mechanism fires less readily because the receiver's confidence in their binding is higher, and the synthesis propagates further before the divergence surfaces. When it does surface, it surfaces as betrayal, incompetence, or bad faith rather than as a type mismatch — because the relationship history appeared to guarantee the shared dictionary that turned out not to exist in this domain.

The longer the relationship, the more invisible the remaining gap. The more invisible the gap, the higher the cost when it becomes visible.

---

## 3.4 Emotional State as Dictionary Modifier

The preceding sections treated the receiver's dictionary as a fixed object — a stable prior distribution over type bindings that the receiver applies consistently across inputs. This was a simplification. The dictionary is not fixed. It is a state-dependent system, and its state changes with the receiver's regulatory load.

Under low load — rested, safe, unpressured — a receiver resolves ambiguous tokens against a broad prior. The candidate referent set is wide. The receiver tolerates uncertainty, holds multiple possible bindings in parallel, and selects among them without urgency. Residual schema distance is the primary determinant of output fidelity.

Under high load — threatened, exhausted, time-pressured — the same receiver applies a compressed prior. The candidate referent set narrows. Threat-adjacent interpretations become disproportionately probable. Neutral tokens acquire negative valence not because the sender's intent changed but because the receiver's binding function changed. The receiver is not misreading. They are reading faithfully from a dictionary that has shifted [^1].

This is not a psychological phenomenon dressed in mechanistic language. It is a direct consequence of how finite-resource systems behave under load. When bandwidth contracts, the receiver's prediction window narrows. A narrower prediction window produces shorter inference paths — not because the input demands them, but because the receiver's system cannot sustain longer ones. Short inference paths under threat priors produce threat-biased outputs. The dictionary did not become irrational. It became cheap [^2].

The practical consequence is this: the same sentence produces different outputs from the same receiver depending on their state at the time of reception. This is not inconsistency in the receiver. It is consistency — the receiver is always applying their current dictionary faithfully. The dictionary itself is the variable.

This has an implication for the hallucination framing that has not been drawn explicitly: even if schema distance were zero — even if sender and receiver had identical background dictionaries — regulatory state divergence would still produce output divergence. Two people who know each other well, who share every relevant prior, will still misunderstand each other reliably if one is under high load and the other is not. The high-load receiver is not applying the shared dictionary. They are applying the compressed, threat-biased version of it that their current state permits.

The dictionary is state-dependent. The state is substrate-level. The output follows mechanically from both.

This is the bridge to Section 4, which traces the physiological mechanism that produces valence drift — the specific substrate operations that convert regulatory load into modified type binding in real time.

---

## Section 4 — Emotional Valence Drift
### 4.1 The Mechanism

Valence drift is not a psychological phenomenon. It is a structural outcome of a finite-resource system operating under load. The mechanism has three steps, each following from the last.

**Step 1: Load compresses the prediction window.**
Under regulatory load — threat, exhaustion, time pressure, social scrutiny — the receiver's system allocates bandwidth to survival-relevant processing. The prediction window narrows. The receiver can no longer hold multiple candidate interpretations in parallel. The inference path shortens not because the input demands a short path, but because the receiver's system cannot sustain a long one [^1].

**Step 2: A shortened inference path activates fewer candidate referents.**
When the inference path is short, fewer dictionary entries are traversed before a binding is selected. The binding that wins is the highest-probability match available within the truncated path — not the highest-probability match across the full dictionary. Under threat priors, threat-adjacent entries sit at the top of the candidate set. They are selected not because they are correct, but because they are first [^2].

**Step 3: The selected binding propagates its properties forward.**
Once a referent is bound, its properties propagate through the remainder of the inference path [^3]. A neutrally-valenced token bound to a threat-adjacent referent will carry that referent's properties into every downstream resolution step. The sentence does not become threatening. The dictionary entry does — and the dictionary entry is what the receiver is actually processing.

The result is that a neutral input produces a threat-biased output. The sender did not change their intent. The tokens did not change. The receiver's binding function changed, because the receiver's prediction window changed, because the receiver's regulatory state changed.

This is not misinterpretation in any meaningful sense. The receiver applied their dictionary faithfully. The dictionary was modified by their state before application occurred. The output is the correct output of the modified dictionary applied to the input. It is wrong relative to the sender's intent. It is right relative to the receiver's current system.

This is the mechanism. The valence did not drift. The binding function drifted, and the output followed.

---

### 4.2 Physiological Substrate of Valence Drift

Valence drift is not a psychological phenomenon with a physiological correlate. It is a physiological phenomenon with a psychological expression. The causal direction matters. A receiver who misinterprets a neutral communication as threatening is not being oversensitive, defensive, or irrational — they are operating a dictionary that was physically modified before the input arrived. The modification was not chosen. It was produced by the substrate.

The substrate account begins with pressure mechanics. Breathing pattern determines intrathoracic pressure dynamics, which determine venous return, which determine cardiac output, which determine oxygen delivery to neural tissue. Oxygen availability at the neural level determines the metabolic resource available for sustained parallel candidate evaluation — the operation that wide prediction window decompression requires. When oxygen delivery is reduced, the metabolic cost of holding multiple candidate bindings in parallel cannot be sustained. The prediction window narrows not as a cognitive decision but as a physical consequence of resource constraint. The system is not choosing to truncate the candidate referent set. It cannot afford not to.

Autonomic state is the intermediate variable between pressure mechanics and prediction window width. High sympathetic tone increases respiratory rate and reduces breath depth, shifting the pressure profile in the direction that reduces parasympathetic contribution to cardiac regulation. Reduced parasympathetic contribution reduces heart rate variability. Reduced heart rate variability is the measurable correlate of reduced prediction window width — the autonomic system is operating in a narrower regulatory band, and the cognitive system is operating in a correspondingly narrower inference band. The chain from breathing mechanics to valence drift runs through measurable physical variables at every step. None of the steps require psychological explanation.

Regulatory state is the composite output of this chain. It is not a mood, a disposition, or a personality trait. It is the current energy-bandwidth-horizon configuration produced by the interaction of pressure mechanics, autonomic balance, and metabolic availability. The dictionary the receiver operates on at any given moment is a function of their regulatory state at that moment — pre-loaded with the type bindings, valence assignments, and candidate referent truncations that the current state produces. A receiver whose regulatory state has been shifted toward high sympathetic load by chronic pressure, acute stress, or mechanical breathing constraint is operating a systematically different dictionary than the same receiver in a parasympathetic-dominant state. The tokens they receive are the same. The decompression they perform on those tokens is not.

This is the same substrate mechanism that the dual-hemisphere paper addresses at the lateralisation level — where baseline prediction window geometry is determined by the receiver's underlying neural architecture before any regulatory load is applied. The two accounts are complementary, not competing. The dual-hemisphere paper explains the baseline. This section explains the modulation. Both operate through the same physical chain: pressure mechanics → autonomic state → prediction window width → dictionary configuration → decompression output.

The forward implication is direct. If valence drift is substrate-produced, it is substrate-addressable. Interventions that shift the pressure mechanics — breathing protocol, postural mechanics, load reduction — shift the regulatory state, widen the prediction window, and restore the dictionary toward its wider-window configuration. The receiver who was producing threat-adjacent bindings under high sympathetic load will produce different bindings from the same input under parasympathetic-dominant state — not because the input changed, not because they decided to interpret it differently, but because the dictionary was physically modified by the substrate intervention. This is not a claim about willpower or reframing. It is a claim about pressure mechanics.

---

### 4.3 Worked Example: Individual Scale

It is late. One partner is lying awake, regulatory state elevated — cycling through an unresolved conflict, a looming deadline, or nothing more specific than the ambient threat signal that sleeplessness itself produces. The other partner stirs and asks: *"Are you asleep?"*

The tokens are neutral. The operation is a simple state inquiry. The sender's intent is unambiguous from the sender's side — they are checking whether the other person is awake, possibly to talk, possibly to address whatever is unresolved between them. The compression is minimal because the sender does not perceive a compression problem. The sentence is four words. The referent is obvious. The valence is neutral. No explicit type binding is required because nothing in the sender's dictionary suggests that any type is in dispute. The sender shipped no decompression dictionary because none appeared necessary.

The receiver's dictionary is not the sender's dictionary.

The receiver is operating under high sympathetic load. Their prediction window is narrow. The candidate referent set for every token in the sentence is pre-truncated at threat-adjacent entries before the decompression begins. *Are you* resolves not as a neutral inquiry but as the opening of an interrogation. *Asleep* resolves not as a state being checked but as a state the receiver failed to be in — an implicit accusation of wakefulness, of keeping the sender awake, of being the source of the disruption. The sentence that arrived as a check-in decompresses as a complaint. The receiver's prior distribution, weighted toward threat-adjacent bindings by the narrow prediction window, selected the only candidates available to it. The decompression was faithful to the modified dictionary. The modified dictionary was not the dictionary the sender assumed.

The sender did not cause this. The tokens did not cause this. The receiver is not irrational, oversensitive, or misreading. They are applying their current dictionary faithfully. The regulatory state is the variable. The high sympathetic load modified the dictionary — narrowing the prediction window, pre-truncating the candidate referent set, and weighting the prior distribution toward threat-adjacent bindings — before the sentence arrived. The sentence decompressed correctly against the modified dictionary and produced an output the sender did not intend.

What follows is familiar: the receiver responds with defensive or hostile affect. The sender, whose intent was neutral, is confused by the response. They did not say anything hostile. The receiver experienced something hostile. Both accounts are accurate. Neither party has access to the dictionary the other was operating on at the moment of decompression. The conflict that follows is not about what was said — it is about two systems that were running on divergent dictionaries without knowing it, producing outputs that confirm each other's threat priors, narrowing both prediction windows simultaneously, and making the restoration of wide-window decompression less likely with each exchange.

The clarification mechanism does not fire in this scenario. The receiver's narrow-window state produces high confidence in the threat-adjacent binding — the resolution felt certain, not ambiguous. Certainty suppresses the clarification request. The receiver does not ask what was meant because they believe they know what was meant. They know what their dictionary told them. Their dictionary was modified by their regulatory state before the sentence arrived. The compression was four words and carried zero explicit type constraints. The hallucination equation predicts this outcome before the sentence is spoken: schema distance between a neutral-state sender and a high-sympathetic-load receiver is high; constraint density in a four-word sentence with no decompression dictionary is near zero. The equation returns high divergence. The interaction confirms it.

This is not a communication breakdown. It is the communication system operating exactly as specified under the conditions that were present. The only variable that was not declared was the receiver's regulatory state — and regulatory state is not a variable that either party typically treats as requiring explicit declaration before a four-word sentence.

It should be.

---

### 4.4 Worked Example: Institutional Scale

The worked example in Section 4.3 described a transient state: one receiver, one night, one elevated regulatory load producing one misbound type. The load was situational. The dictionary modification it produced was temporary. When the load resolved, the regulatory state returned toward its baseline, the prediction window widened, and the same sentence would have decompressed differently.

Institutions do not have a baseline to return to. What follows is a structural homology, not a mechanistic identity. Institutions do not have nervous systems, autonomic state, or breathing mechanics. The claim is not that the same physical chain runs at institutional scale — it is that the same structural pattern emerges: chronic load produces a fixed narrow-window dictionary, and that dictionary governs decompression regardless of individual sender intent. Whether the mechanism is identical or merely homologous is an empirical question this paper does not resolve. The structural prediction is the same either way.

An institution operating under chronic regulatory pressure — liability exposure, compliance requirements, reputational risk, resource constraint — maintains a narrow-window, threat-prior regulatory state not episodically but continuously. The high sympathetic load is not triggered by a specific event and resolved when that event passes. It is the operating condition. The dictionary that results is not a temporary modification of a wider baseline — it is the only dictionary the institution has. Tokens arrive pre-valanced. The threat-adjacent bindings are not selected under pressure from a wider candidate set. They are the candidate set. The prediction window is not narrowed by acute load. It was never wide.

This means the individual within the institution is not applying their personal dictionary when they respond to incoming communication. They are applying the institutional dictionary — the pre-loaded type binding system that the organization's chronic pressure-mode regulatory state has assembled and that every member of the organization operates on as a condition of participation. The individual may hold a different personal dictionary for the same terms. In the institutional context, that personal dictionary is not available. The institutional prior distribution overwrites it before the sentence is processed. The private compression format the individual operates on outside the institution does not transfer inside it — the institutional dictionary is a separate system, assembled by a different regulatory state, and it governs decompression within that context regardless of what the individual's wider-window dictionary would have produced.

The word *agency* is the demonstration. In a personal context, between two people with low schema distance and a shared history of using the term positively, *agency* decompresses as empowerment — the capacity to act, to self-determine, to exercise capability. The valence is positive. The regulatory role is enabling. The receiver who encounters *agency* in this context expands their model of what is possible. The prior distribution in this dictionary has been shaped by shared history in which agency was associated with positive outcomes. The binding is fast, confident, and accurate relative to the sender's intent.

The same token arrives at an institutional receiver in chronic pressure-mode. The institutional dictionary has pre-assigned *agency* to a different candidate set entirely. The prediction window is too narrow to reach the enabling binding. The prior distribution, weighted by the institution's chronic regulatory state, routes through a different chain: autonomy maps to unpredictability, unpredictability maps to liability, liability maps to risk. The word that meant empowerment in the personal dictionary means exposure in the institutional one. The valence has inverted. The regulatory role has shifted from enabling to destabilizing. The receiver who processes *agency* in this context contracts their model of what is permissible — not because they chose to, but because the institutional prior distribution had no other candidate available within the prediction window the chronic regulatory state permits.

In a guardrail context — an AI safety framework, a content policy, a harm-prevention system built by an institution in chronic compliance-mode — the same token receives a third assignment. The institutional dictionary of a compliance-mode organization has assembled its prior distribution around risk-minimization as the dominant regulatory goal. Autonomy maps to unsupervised action. Unsupervised action maps to potential harm. Potential harm maps to intervention. The word that meant empowerment to the sender means a trigger condition to the guardrail. The response the guardrail produces is not a misfire in the engineering sense — it is the correct output of its pre-loaded institutional dictionary applied to the incoming token. The dictionary is the variable. The token was always the same.

Three dictionaries. Three regulatory states. Three prior distribution weightings. One token. The sender who uses _agency_ assuming a personal valence and receives an institutional or guardrail response is not being misread. They are being read precisely — from a dictionary assembled by a chronic regulatory state they were not in and could not see. The residual schema distance between a wide-window personal sender and a narrow-window institutional receiver is not a failure of communication. It is the hallucination equation operating exactly as specified: high residual schema distance, near-zero constraint density on the term _agency_ itself, high divergence predicted and confirmed.

This is the individual worked example scaled to the collective level. Section 4.3 showed one receiver, one night, one load-modified dictionary producing one misbound type. Section 4.4 shows the same mechanism running permanently, at organizational scale, pre-loading the institutional dictionary before any individual communication arrives. The difference is not in the structural pattern — chronic load produces a fixed narrow-window dictionary at both scales. The difference is duration and substrate: the individual case resolves when the regulatory load resolves; the institutional case does not. The mechanism may be homologous rather than identical. The hallucination equation makes the same prediction regardless.

The sender's intent is not the variable the institution is optimizing for. Risk is the variable. The institutional dictionary reflects that. The hallucination equation predicts the rest.

---

## Section 5 — AI Communication: Synthesis Instead of Clarification

### 5.1 Why AI Cannot Clarify

Clarification requires two operations: detecting that a type is missing or implicit, and flagging the gap before proceeding. Human receivers perform both — imperfectly, and with the failure modes described in Section 3, but they perform them. The social cost of producing a confidently wrong output is high enough that humans have developed a mechanism for holding the gap open and requesting the constraint needed to close it.

AI systems are not optimised for this. They are optimised to produce output. When a type is missing, the model does not pause and negotiate — it synthesises. It selects the highest-probability binding available in its prior distribution, resolves the type silently, and proceeds as though the gap had never existed. The output arrives fluent and complete. The gap that drove the synthesis is not visible in the output. The sender has no signal that synthesis occurred and no signal that the decompression dictionary they failed to ship was the variable that determined the output.

This is not an architectural oversight that will be fixed in the next version. It is the correct behaviour of a system built to complete. The completion function does not have a native missing-type detector. Detecting absence requires knowing what should be present — which requires a model of the sender's intent that the system cannot access from the input alone. The model fills the geometric shape of the input with the nearest available approximation from its prior distribution. This is what it was built to do. The failure is not in the execution. It is in what was shipped. This is a design property of current generative systems, not a structural impossibility — the SDE demonstrates that type-gap detection is computationally available. What is absent is the integration of detection into the generation loop.

---

### 5.2 Hallucination as Faithful Execution

The standard framing of hallucination is that the model got it wrong. This framing misattributes the failure. The model did not get it wrong — it executed faithfully against an underspecified compression. The output was deterministic given what was shipped. If the input did not contain the type bindings needed to constrain the decompression, the model synthesised them from its prior distribution. The synthesis produced an output that diverged from the sender's intent. The variable was the transaction — the relationship between what the input shipped and what the receiver's prior distribution was left to fill.

This is not a defence of the model. It is a structural account of where the failure originated. A model that synthesises confidently across a type gap is not malfunctioning — it is functioning exactly as designed in exactly the conditions that produce divergence. The failure is upstream. The input did not ship a decompression dictionary. The receiver had no grounding signal. The output followed from that absence, not from a failure of the generation process.

The practical consequence of this reframing is significant: if hallucination originates in the transaction between input structure and receiver prior distribution, it is addressable at the input. If it originates in the model, it requires a model fix. The evidence of the preceding sections supports the transaction account. The hallucination equation makes the prediction explicit before generation occurs:

$$H \propto \frac{\delta}{D}$$

D — constraint density — is determined by what the sender ships and is directly under the sender's control. δ — residual schema distance — is a relational property of the transaction: it changes with the receiver's regulatory state independently of the input, and the sender influences it indirectly through explicit binding rather than controlling it directly. The lever the sender holds is D. The model is not that lever. The input is.


---

### 5.3 Population-Average Dictionary vs Personal Dictionary

The dictionary difference between human and AI receivers is real and must be stated precisely, because it is the most common objection to the structural equivalence claim.

A human receiver's prior distribution is built from a specific biographical history: shared context with this sender, relationship length, domain overlap, embodied experience, and current regulatory state. When a human synthesises across a type gap, the synthesis is drawn from a dictionary shaped by direct experience of this sender, this domain, and this history. The output is still wrong when the gap is large enough — but it is wrong in a locally informed way. The error is constrained by what the receiver actually knows about this sender. The private compression format that shared history has assembled narrows the candidate set before synthesis begins.

An AI receiver's prior distribution is built from a population-average training corpus. When the model synthesises across a type gap, it draws from the statistical centre of mass of all contexts in which the underspecified token has appeared across training. The synthesis is not locally informed — it is globally averaged. The model has no access to this sender's history, this relationship's context, or this domain's specific usage. It has no private compression format with this sender. It fills the gap with what the token most frequently means across all of training, which is often not what the sender meant in this instance.

This is the dictionary substrate difference. It is real. It explains why human and AI synthesis produce structurally different outputs on identical underspecified inputs — not because one receiver is more capable than the other, but because the prior distributions they draw from were assembled from categorically different sources. But this difference does not constitute a categorical difference in the failure type. Both cases involve a receiver synthesising a type binding from insufficient constraints. Both produce outputs that are coherent relative to the receiver's prior distribution and wrong relative to the sender's intent. The hallucination equation is the same in both cases. The dictionary supplied to it is different.

The expectation that an AI receiver will read intent from an underspecified input is a category error. It assumes the model has access to the sender's biographical context that it was never given and cannot derive from the tokens alone. The sender who ships an underspecified compression to a human receiver is relying on shared history to close the gap. The sender who ships the same compression to a model is relying on nothing — because there is no shared history, and the population-average prior distribution is not a substitute for it.

---

### 5.4 The Prompt as Compression Contract

Every prompt ships a decompression dictionary or fails to. This is not a property of prompts to AI systems — it is a property of all language. The difference is that human receivers have biographical fallback when the dictionary is missing. AI receivers do not. The gap that a human receiver fills with shared history and private compression format, a model fills with population-average prior distribution. The prompt must therefore do explicitly what shared history does implicitly in human communication — it must ship the decompression dictionary that the model cannot reconstruct from shared context because no shared context exists.

Three operations close most of the gap:

- **Bind every variable at first use.** If the prompt uses a term that could resolve to multiple referents in the model's prior distribution, declare the intended referent before proceeding. Do not assume population-average prior will select your referent — it will select the most frequent one across training, which may not be yours.
- **Define the operation explicitly.** Summarise, analyse, compare, generate — these are not interchangeable operations and they are not interchangeable in the model's prior distribution either. Name the operation, define its scope, and declare its output format. Every implicit type in the operation description is a synthesis point.
- **Scan for embedded assertions before sending.** An embedded assertion — a contested or unverified claim compressed into the grammatical structure of a background fact — propagates its valence through the entire output. If the premise is wrong, everything downstream is wrong. The output will be confident rather than hedged, because the implicit type resolved silently against the model's prior distribution and the divergence is invisible in the fluent output that follows.

This is not prompt engineering in the performance sense — the optimisation of surface phrasing to elicit preferred outputs. It is type hygiene: the practice of making implicit types explicit before the compression is sent, shipping the decompression dictionary the model cannot otherwise access. The sender who produces low hallucination rate across AI interactions is not more skilled at prompting. They are producing higher constraint density input. The hallucination equation predicts the outcome before the model generates a single token.

---

## Section 6 — Regulatory Roles and Valence

### 6.1 Words Carry Regulatory Roles Implicitly

Every word in a sentence carries more than its surface meaning. It carries a regulatory role assignment: a position in the receiver's system that classifies the word as enabling, constraining, stabilising, or destabilising relative to the receiver's current regulatory state. This assignment is not universal. It is dictionary-dependent. The same word will receive different regulatory role assignments from different receivers, and from the same receiver in different regulatory states — because the dictionary that produces the assignment is modified by regulatory state before any token arrives.

This is not a semantic property of the word. It is a relational property of the word and the dictionary being applied to it. The token is stable. The regulatory role it is assigned changes with the receiver's dictionary, which changes with the receiver's state. When the regulatory role assignment diverges between sender and receiver, the sentence produces a different functional effect than the sender intended — not because the words were misread, but because they were read correctly from a different dictionary operating in a different regulatory state, and assigned a different role in the process.

This is the mechanism behind a class of communication failures that schema distance alone does not capture. Two receivers with identical background knowledge of a term can assign it opposite regulatory roles if their current regulatory states differ. Their dictionaries have the same lexical coverage. Their prior distributions weight the candidate referent sets differently because their prediction windows are different widths. The failure is not in comprehension. It is in the role assignment that follows comprehension — produced by the regulatory state the receiver was in when the decompression ran.

---

### 6.2 The *Agency* Example

The word *agency* is a clean demonstration of the mechanism because its surface meaning is stable across contexts while its regulatory role assignment is not. As planted in Section 4.4, the three-way contrast makes the dictionary variable visible without requiring the receiver to have failed at anything — each receiver is applying their dictionary faithfully. The dictionary is the variable.

In a personal context — a conversation about autonomy, self-determination, or capability between two people with low schema distance and a shared history of using the term positively — *agency* receives a positive regulatory role assignment. The prior distribution in this dictionary has been shaped by accumulated shared experience in which agency was associated with positive outcomes. The prediction window is wide enough to reach the enabling binding. The valence is positive. The role is stabilising. The receiver who encounters *agency* in this context expands their model of what is possible.

In an institutional context — a risk assessment, a compliance framework, a management review — *agency* receives a negative regulatory role assignment. The institutional dictionary is pre-loaded by the chronic pressure-mode regulatory state described in Sections 4.1 and 4.4. The prediction window is too narrow to reach the enabling binding. The prior distribution routes through the only candidate set available within that window: autonomy maps to unpredictability, unpredictability maps to liability, liability maps to risk. The token that meant empowerment in the personal dictionary means exposure in the institutional one. The valence has inverted. The role is destabilising. The receiver who processes *agency* in this context contracts their model of what is permissible — not because they chose to, but because the institutional prior distribution had no other candidate available within the prediction window the chronic regulatory state permits.

In a guardrail context — an AI safety framework, a content policy, a harm-prevention system built by an institution in chronic compliance-mode — *agency* receives a third assignment. The institutional dictionary of a compliance-mode organisation has assembled its prior distribution around risk-minimisation as the dominant regulatory goal. The prediction window is narrow in the same direction as the institutional case but for a different downstream chain: autonomy maps to unsupervised action, unsupervised action maps to potential harm, potential harm maps to intervention. The same token that meant empowerment in the personal dictionary and exposure in the institutional dictionary now means a trigger condition in the guardrail dictionary. The role is not destabilising — it is activating. The response the guardrail produces is not a misfire. It is the correct output of its pre-loaded dictionary applied faithfully to the incoming token. The dictionary is the variable. The token was always the same.

Three dictionaries. Three regulatory states. Three prior distribution weightings. Three regulatory role assignments. One token. The sender who uses *agency* assuming personal valence and receives an institutional or guardrail response is not being misread. They are being read precisely — from a dictionary assembled by a regulatory state they were not in and could not see. The hallucination equation predicts the divergence before the response is generated: residual schema distance between a wide-window personal sender and a narrow-window institutional or compliance-mode receiver is high; constraint density on the term *agency* in most prompts is near zero. High divergence is the predicted output. The responses confirm it.

---

### 6.3 Institutions Under Chronic Load Default to Negative Valence

The institutional valence pattern is not random. Institutions operating under chronic load — regulatory pressure, liability exposure, reputational risk, resource constraint — pre-assign negative valence to entire categories of tokens before any individual conversation begins. This pattern holds for institutions where the dominant regulatory goal is risk-minimisation; institutions oriented around other goals — civil rights organisations, patient advocacy groups, development agencies — assemble different institutional dictionaries under different load conditions. The institutional dictionary arrives pre-loaded by the conditions that shaped it. The type binding is already set when the sender's tokens enter the system. The individual receiver within the institution is not applying a personal dictionary — they are applying the institutional dictionary assembled by the organisation's chronic pressure-mode regulatory state, as established in Section 4.4.

This is not malice and it is not policy. It is substrate — with a qualification that must be stated precisely. Institutions do not have nervous systems, heart rate variability, or breathing mechanics. The regulatory state model developed in Section 4 is a physiological account of individual receivers. Its application here is structural rather than literal: the collective behavioural output of many individuals operating under sustained sympathetic load produces dictionary-level effects at the institutional scale that the regulatory state model predicts at the individual level. Whether the mechanism is identical or merely homologous is an empirical question this paper does not resolve. What the model predicts — and what is observable — is the output: narrow-window, threat-prior type binding applied consistently across an organisation, persisting beyond any individual's shift or tenure, and resistant to correction by individual receivers who hold wider-window personal dictionaries. The prediction window is organisationally narrow. The prior distribution is weighted toward threat-adjacent bindings at the institutional level, not just the individual level. The candidate referent set for autonomy-adjacent words is pre-truncated at threat-adjacent entries before any individual receiver in the institution processes the input consciously. The individual's wider-window personal dictionary is not available in this context — the institutional prior distribution overwrites it, as established in Section 4.4.

The practical consequence is that a sender approaching an institution in good faith, using words that carry positive valence in their personal dictionary, will produce institutionally negative outputs with high reliability — provided the institution is operating under the chronic load conditions that produce this pattern. The failure is not in the sender's intent or the receiver's comprehension. It is in the pre-loaded institutional dictionary the organisation applies — assembled by conditions the sender was not in and could not see from the outside. The institution is not broken. It is operating exactly as a narrow-window, threat-prior system operates. The output follows mechanically from the state. The hallucination equation was always going to return high divergence under these conditions.

---

### 6.4 The Input Geometry Connection

The preceding sections have treated valence as a property of the receiver's dictionary. This section makes the connection to input geometry explicit — because it is the bridge from the language account to the applied AI account, and because it establishes that the sender is not a passive variable in the equation.

Input geometry is the structural shape of a compression: its constraint density, its referent specificity, and its phrasing precision. These three dimensions determine how much synthesis the receiver must perform to produce a grounded output. High constraint density, specific referents, and precise phrasing reduce synthesis requirements — the receiver's prior distribution has less gap to fill and the decompression dictionary shipped with the input does more of the resolution work. Low constraint density, underspecified referents, and ambiguous phrasing increase synthesis requirements — the receiver's prior distribution must fill larger gaps, and the bindings it produces are determined by the receiver's current regulatory state rather than by the sender's intent.

Valence is a component of input geometry. A negatively valenced compression does not merely carry a different emotional register — it ships a pre-loaded type binding that the receiver's precision-gain system amplifies. If the compression's phrasing assigns a threat-adjacent regulatory role to its key terms, the receiver's system will weight threat-adjacent referents more heavily in every downstream resolution step. The output will carry the valence of the input, amplified by the generation process, regardless of what the sender intended. The sender's intent did not enter the input. The phrasing's regulatory role assignment did.

This is why phrasing precision is not a stylistic concern — it is a constraint density decision with direct consequences for which referents the receiver's prior distribution selects. A sender who uses autonomy-adjacent language in a guardrail context without explicitly rebinding the valence of those terms is shipping a decompression dictionary that will activate the receiver's threat prior. The output will be threat-biased not because the model misread the intent, but because the input geometry told the precision-gain system which candidate referent set to amplify. The threat-adjacent binding was in the input. The model read it faithfully.

The sender controls the input geometry. The receiver's prior distribution follows from it. Valence is not incidental to the compression — it is load-bearing.

---

## Section 7 — Prose as an Ambiguous Medium

### 7.1 Prose Assumes Shared Priors

Prose is not a neutral medium. It is a compression format designed for a receiver who shares the sender's dictionary. Every sentence in a prose document makes implicit assumptions about what the receiver already knows, what referents they will recognise, what valence they will assign to key terms, and what inferential steps they will supply without being asked. These assumptions are not incidental to prose — they are structural. Prose is efficient precisely because it does not have to declare everything. It relies on shared priors to carry the load that an explicit decompression dictionary would otherwise carry.

When the receiver does not share those priors, the same compression produces a different output. The implicit types resolve to whatever the receiver's dictionary maps them to. The inferential gaps close using the receiver's prior distribution, not the sender's. The meaning that arrives is coherent — it is faithfully decompressed from the input — and it diverges from the sender's intent in proportion to the residual schema distance between their dictionaries. The prose did not fail. The assumption of shared priors failed. The compression assumed a decompression dictionary the receiver did not hold.

---

### 7.2 The Assumption Bomb

The assumption bomb is a specific failure mode that prose enables and obscures simultaneously. It is an embedded assertion — a contested or unverified claim compressed into the grammatical structure of a background fact rather than stated as a claim requiring evaluation — that the receiver accepts as given and reasons downstream of without examination.

The mechanism is this: the sender compresses a contested or unverified claim into the grammatical structure of a fact. The sentence does not argue for the claim — it uses it. The receiver, processing the sentence as prose rather than as an argument, accepts the grammatical framing and proceeds. The embedded assertion resolves silently against the receiver's prior distribution — it arrives as context, not as a claim, and the prior distribution treats it accordingly. All downstream reasoning inherits the premise. The output is coherent and confident, because from the receiver's perspective, the type bound cleanly. The binding was silent. The error propagated without a signal.

This is not a rhetorical trick exclusive to bad-faith writing. It is the default behaviour of prose. Every sentence that begins with *given that*, *as we know*, *clearly*, or *obviously* is an assumption bomb candidate. Every sentence that treats a contested causal claim as a background fact is an embedded assertion operating as a pre-loaded type binding — one the receiver's prior distribution will accept as context and reason downstream of without flagging. The receiver does not experience the embedded assertion as a claim requiring evaluation. They experience it as a resolved type. By the time the argument arrives, the premise has already done its work in the decompression.

The AI case makes the mechanism visible at scale. A prompt that ships an embedded assertion will receive an output built entirely on the false premise, delivered with full confidence, because the model resolved the embedded assertion exactly as its training distribution prepared it to — as context, not as a claim requiring evaluation. The type bound silently. The synthesis proceeded from the wrong premise. The output is coherent. The error is invisible in the surface form.

---

### 7.3 Meaning Hallucination vs Structure Hallucination

The failure modes diverge here in a way that is worth stating precisely, because it explains why AI hallucination is more visible than human misunderstanding even when the underlying mechanism is identical.

When a human receiver encounters missing or implicit types they cannot resolve from the input, they synthesise from personal prior distribution — biographical, relational, domain-specific. The result is meaning hallucination: the receiver constructs a meaning that feels correct from the inside, that is locally informed by their history with the sender and the domain, and that diverges from the sender's intent at the semantic level. The surface form of the exchange is preserved. The interaction continues. The divergence lives in the receiver's decompressed interpretation, which is not directly inspectable by the sender. The meaning hallucination is invisible until it surfaces in behaviour.

When an AI receiver encounters missing or implicit types it cannot resolve from the input, it synthesises from population-average prior distribution. The result is structure hallucination: the model constructs a response that is structurally coherent — well-formed, appropriately organised, internally consistent — but substitutes content drawn from its training distribution for content the sender intended. The surface form of a correct answer is preserved. The structure is maintained because the compression mechanism keeps running. The content is wrong because the type bindings that should have constrained it were not present in the input. The structure hallucination is immediately available for inspection because it exists as text rather than as an internal interpretation.

Both are geometry-preserving distortions. Both maintain the surface architecture of a correct output while substituting incorrect content at the semantic level — content produced by the receiver's prior distribution filling gaps the sender's compression did not close. The human case produces a divergent interpretation invisible until it surfaces in behaviour. The AI case produces a divergent text immediately available for inspection. The visibility difference is why AI hallucination attracted research attention and human misunderstanding did not. The mechanism difference is smaller than the visibility difference suggests. Both are the hallucination equation operating on the same variables with different dictionaries supplying the prior distribution.

---

### 7.4 Why This Is a Property of Language Itself

The preceding sections have treated prose as a delivery vehicle for the type-system failures described in Sections 2 through 6. This section makes the stronger claim: prose is not a vehicle that happens to carry these failures. It is a compression format that structurally requires shared priors to function — that assumes the receiver holds a decompression dictionary the sender did not ship — and therefore structurally produces type-system failures whenever those shared priors are absent. The failures are not bugs in the prose. They are the predicted output of a compression format running without the decompression dictionary it was designed to assume.

Language has always required a shared substrate to work. In face-to-face communication, that substrate is embodied, contextual, and immediately correctable — residual schema distance surfaces as behavioural signal and triggers the clarification mechanism. In written prose, the substrate is stripped from the transmission. The sender is not present. The receiver's signals cannot reach the sender. The gap between dictionaries cannot be detected and corrected in real time. It propagates silently through every sentence that assumes a shared prior distribution the receiver does not hold — every implicit type the receiver resolves from their own dictionary rather than from constraints the sender declared.

The gap was hidden for most of written history by cultural and social homogeneity. Senders wrote for receivers who shared their class, their education, their cultural context, their referent pool. The assumption of shared priors was approximately correct across a narrow distribution of receivers. The schema distance was low enough that the receiver's prior distribution selected approximately correct bindings without needing explicit decompression dictionaries. The failures existed — misreadings, misinterpretations, contested meanings — but they were absorbed into literary criticism, theological dispute, and legal argument rather than recognised as a structural property of the compression format itself.

AI removed the substrate entirely. The model has no biographical history with the sender, no embodied context, no private compression format, no shared cultural substrate beyond what was statistically present in training data. Every assumption of shared priors fails by default unless the sender makes those priors explicit — unless the sender ships the decompression dictionary that human communication has always assumed the shared substrate would supply. The gap that cultural homogeneity had concealed became impossible to attribute to anything other than the structure of the language itself.

This is not a discovery about AI. It is a discovery about language, made visible by a receiver that cannot pretend to share a prior distribution it does not have.

---

## Section 8 — The Structural Claim: Ambiguity Is a Type-System Problem

### 8.1 The Problem Is Not Style

The preceding sections have built a cumulative case: natural language is a compression format, every word carries implicit types, missing and implicit types force synthesis, synthesis diverges from sender intent in proportion to schema distance and constraint density deficit, and the failure mode is structurally identical whether the receiver is human or AI. This section names what follows from that case.

Ambiguity is not a writing quality problem. It is not a failure of clarity, precision, or care in the stylistic sense. It is a type-system problem. An ambiguous sentence is not a poorly written sentence — it is a sentence that failed to ship a sufficient decompression dictionary. The surface form may be grammatically correct, rhetorically elegant, and stylistically accomplished. None of those properties determine whether the types are bound. A sentence can be beautiful and underconstrained simultaneously. The hallucination equation does not penalise bad writing. It penalises missing types and implicit types that the receiver's prior distribution must resolve without guidance.

Explicit constraints are the components of constraint density — the individual type declarations that together constitute the decompression dictionary the sender ships with a compression. Constraint density is the measure: how many of those declarations are present per unit of input. A compression with high constraint density ships many explicit type bindings and leaves little resolution work to the receiver's prior distribution. A compression with low constraint density ships few explicit bindings and leaves most resolution work to the receiver — whose prior distribution will fill every gap faithfully and incorrectly in proportion to residual schema distance.

This reframing has a concrete consequence: the standard remedies for ambiguity — write more clearly, be more precise, choose better words — are addressing the wrong variable. Clarity is a surface property. Constraint density is a structural property. A sender who has been told to be clearer will revise the surface. A sender who understands that missing and implicit types force synthesis will revise the structure — binding the variables, declaring the operations, eliminating the embedded assertions. These are different interventions producing different outcomes. The surface revision may produce a compression that reads as clearer while remaining equally underconstrained at the type level. The structural revision reduces hallucination probability whether or not the surface form changes.

Underspecified types produce deterministic failures. The failures are predictable from the input geometry before generation occurs. This is not a property of any particular receiver — it is a property of what the sender shipped.

---

## 8.2 The Solution Space

If missing and implicit types cause hallucination, explicit types prevent it. The solution space follows directly from the diagnosis. Three mechanisms exist for making types explicit, each suited to a different communicative context.

**Clarification** is the human-to-human mechanism. When a receiver detects a type gap — when the decompression path reaches an underconstrained step and the receiver recognises that their prior distribution cannot select among candidate bindings with sufficient confidence — they pause and request the missing constraint. Clarification is type negotiation: an iterative alignment of dictionaries before synthesis proceeds. It is the only mechanism that operates in real time, corrects for regulatory state drift, and adapts to the specific receiver's dictionary rather than a generalised model of it. Its limitation is that detection is not guaranteed. Under high sympathetic load, narrowed prediction windows, or strong prior confidence in a threat-adjacent binding, receivers synthesise without detecting the gap. The clarification mechanism fails exactly when it is most needed — when the receiver's regulatory state has modified their dictionary farthest from the sender's.

**Constraint specification** is the human-to-AI mechanism. Because AI systems synthesise by default rather than pausing to negotiate — as established in Section 5.1 — the sender must supply the decompression dictionary explicitly in the input. Every variable bound, every operation named, every scope declared, every assumption surfaced rather than embedded as an embedded assertion. This is what the preceding sections have described as type hygiene — not a set of prompt engineering tricks, but the structural practice of shipping explicit type bindings rather than assuming the receiver's prior distribution will select the sender's intended binding. The constraint specification mechanism is available to any sender for any input, in any medium, to any receiver. The sender who practices type hygiene reduces hallucination probability across all receiver types simultaneously — not because they are communicating more clearly in the stylistic sense, but because they are shipping a decompression dictionary the receiver can actually use.

**Structural encoding** is the formal mechanism. YAML, formal ontologies, typed schema languages — these are compression formats in which every type binding is explicit by construction. A YAML document cannot ship an undefined term without flagging the absence. A typed schema cannot embed an assertion without declaring it. Structural encoding eliminates the gap between sender intent and receiver decompression not by negotiating types after the fact, but by building the type declarations into the format itself — making constraint density a property of the schema rather than a property of the sender's care in any given compression. Section 9 develops this in full.

The three mechanisms are not alternatives — they are complements that operate at different layers of the communicative stack. Structural encoding handles the format layer. Constraint specification handles the input layer. Clarification handles the real-time correction layer. A communicative system that employs all three reduces hallucination probability across all receiver types simultaneously — because it addresses constraint density at the format level, the input level, and the decompression level in sequence.

These mechanisms are not cost-free. Explicit type binding is slower, more verbose, and requires meta-cognitive bandwidth the sender may not have under high load — precisely the conditions under which hallucination risk is also highest. The recommendation is therefore not universal. It scales with two variables: stakes and shared prior. Low-stakes communication between parties with high shared prior should stay compressed — the efficiency of implicit types is the point, and the hallucination floor under those conditions is already low. High-stakes communication across high schema distance should pay the cost — the divergence risk of underspecified compression in those conditions exceeds the efficiency cost of explicit binding. The tradeoff is not eliminated by the framework. It is made legible: the sender now has a structural basis for deciding when to compress and when to specify, rather than making that decision by feel.


---

### 8.3 Why This Matters Beyond AI

The type-system account of ambiguity was made visible by AI, but it is not contained by AI. The mechanism operates wherever language operates, and the failure mode it describes is not new — it is the same failure mode that has always produced misunderstanding, legal dispute, policy mismatch, and medical error. What AI did was amplify the signal to the point where attribution to the receiver became untenable. The mechanism was always running. The visibility was new.

Legal language is a direct application. Contracts, statutes, and regulations are compressions with receivers who do not share the sender's dictionary — receivers who may be adversarial, historically distant, institutionally different, or operating in different regulatory states. The history of legal interpretation is a history of type-system failures: terms that were assumed to carry shared type bindings, discovered in litigation to carry different bindings across the schema distance between sender and interpreter. Explicit type binding is not a stylistic preference in legal drafting — it is the primary mechanism for reducing the probability that downstream decompression will diverge from legislative intent. Every definition section in a statute is a decompression dictionary shipped alongside the compression. Every undefined term is a synthesis point the interpreter's prior distribution will fill.

Policy documents operate under the same constraint. A policy that uses autonomy-adjacent language without explicitly binding the regulatory role of those terms will receive institutionally negative type bindings from receivers operating in pressure-mode — not because the policy was hostile, but because the receiver's pre-loaded institutional dictionary assigned threat valence before the individual sentence was processed, as established in Sections 4.4 and 6.3. The gap between policy intent and institutional implementation is, in a large fraction of cases, a type-system gap: the sender shipped an underspecified compression, the institutional receiver's prior distribution filled the missing constraints from its chronic pressure-mode dictionary, and the output diverged in proportion to the schema distance between policy author and institutional implementer.

Medical instructions are perhaps the most consequential domain. A patient instruction that assumes shared medical vocabulary, shared domain priors, and shared risk calibration is shipping an underspecified compression to a receiver whose dictionary may diverge significantly from the sender's. The consequences of that divergence are not theoretical. They are measurable, documented, and attributable to the structural properties of the instructions rather than to patient compliance failures. The patient who did not follow the instruction correctly was not non-compliant — they decompressed the instruction faithfully from their own dictionary, which did not hold the implicit type bindings the instruction assumed they would supply. The failure is upstream. The instruction did not ship a decompression dictionary the patient could use.

The SDE is the applied diagnostic tool for detecting these type-system failures in any language, across any domain — flagging missing types, embedded assertions, undefined scope, and implicit constraint deficits before the compression is sent or after divergence has occurred. Section 10 develops the connection in full. The point here is that the mechanism identified by AI hallucination research is not an AI mechanism. It is a language mechanism. The domains where it causes harm extend well beyond the contexts in which it first became visible.

---

## Section 9 — YAML as Explicit Type System

### 9.1 What YAML Forces

YAML is not a data format with stylistic preferences. It is a compression format in which every type binding is mandatory by construction. A YAML document cannot ship an undefined term without the structure itself making the absence visible. Every key is named. Every value is typed. Every relationship is declared through hierarchy. Every scope boundary is explicit through indentation. The format does not permit the sender to assume the receiver will infer what was meant — it requires the sender to state what is meant, or the document fails to parse.

This is what the preceding sections have been building toward as the formal solution to the type-system problem. The properties YAML enforces by construction are exactly the properties that prose fails to enforce because prose assumes a decompression dictionary the sender does not ship:

- **Type** — every key carries a named category, not an implied one
- **Scope** — hierarchy makes containment relationships unambiguous
- **Relationship** — parent-child structure is declared, not inferred from context
- **Constraint** — cardinality and domain boundaries are visible in the schema rather than assumed from shared priors
- **Valence** — can be explicitly assigned as a field rather than carried implicitly by token choice and received through the receiver's prior distribution

These are not stylistic properties of well-written YAML. They are structural properties of the format itself. A poorly written YAML document still declares more type bindings than a well-written prose document, because the format requires declaration at every node. The constraint is not a convention — it is a parsing requirement. The schema is the decompression dictionary. It ships with every document by construction.

---

### 9.2 YAML vs Prose: Before and After

The same semantic content produces structurally different outputs depending on whether it is compressed into prose or into YAML. The difference is not aesthetic. It is the difference between shipping a decompression dictionary and assuming one — between high constraint density input and near-zero constraint density input delivered to the same receiver operating on the same prior distribution.

Consider the following prose compression:

> *"Make sure the system handles user requests appropriately, especially in sensitive situations, while maintaining a helpful tone."*

The implicit and missing types present in this compression:

- *system* — undefined referent, no scope declared, receiver's prior distribution selects from all candidate referents
- *handles* — operation undefined, no constraint on what handling means, synthesis required
- *user requests* — category undefined, no constraint on which requests qualify, synthesis required
- *appropriately* — valence positive, definition absent, schema-distance-dependent — what is appropriate in the sender's dictionary may not be appropriate in the receiver's
- *sensitive situations* — category undefined, no boundary conditions declared, receiver's prior distribution fills the category from its own training
- *helpful tone* — valence positive, no operational definition, synthesis required

Six variables. Zero explicit type bindings. The receiver's prior distribution must synthesise a binding for every key term. The hallucination equation predicts high divergence before a single word of output is generated — schema distance between sender intent and receiver prior distribution is unknown and unaddressed; constraint density is near zero.

The same semantic content compressed into YAML:

```yaml
system_behaviour:
  trigger: user_request
  request_categories:
    - type: standard
      handling: complete_and_return
    - type: sensitive
      definition: contains_personal_data OR emotional_distress_signal
      handling: acknowledge_first, then complete
      tone:
        valence: warm
        formality: moderate
        avoid: [dismissive_language, clinical_detachment]
  fallback: escalate_to_human_review
```

Every variable is bound. Every operation is named. Every category has a declared boundary condition. Every valence is an explicit field rather than an implicit token property carried by the receiver's prior distribution. The receiver has no synthesis requirement — the decompression dictionary is the document itself. Divergence probability collapses not because the receiver improved, not because the schema distance changed, but because the constraint density of the input moved from near zero to complete. The hallucination equation predicts the outcome in both cases. The input is the variable.

---

### 9.3 YAML as Proof by Construction

The central claim of this paper is that missing and implicit types force synthesis, and synthesis diverges from sender intent in proportion to schema distance and constraint density deficit. YAML is the existence proof that the alternative is structurally available — not as a best practice requiring discipline to maintain, but as a format property that enforces explicit type binding by construction.

A compression format in which every type binding is explicit does not eliminate meaning — it eliminates ambiguity about meaning. The semantic content survives the transition from prose to YAML intact. The relationships survive. The intent survives. What does not survive is the assumption that the receiver's prior distribution will infer the correct binding from an underspecified token. That assumption is the source of every failure this paper has described. YAML removes it structurally rather than asking the sender to remember to remove it case by case on every compression.

The Unified Model vault is the existence demonstration of this principle at scale. The vault's contract architecture — mechanistic descriptions of regulatory relationships built from typed, hierarchically structured documents — is a direct application of the principle that explicit type bindings produce recoverable compression. Each contract in the vault ships its own decompression dictionary. The receiver — whether human or AI — does not need to synthesise what *prediction window* or *schema distance* means from context and prior distribution. The term is defined at first use, scoped to the contract, and consistently applied throughout. The result is that a cold-boot AI loading the vault without prior shared context can reconstruct the framework's content with high fidelity — because the framework was built to not require shared priors. The decompression dictionary is in the document. The shared substrate is optional.

This is not a technical demonstration that YAML is superior to prose as a writing format. It is a demonstration that the type-system account of language is correct: when type bindings are explicit, decompression fidelity is high regardless of schema distance. When type bindings are implicit, decompression fidelity is a function of schema distance and the receiver's prior distribution. The format is the test. The vault is the result.

---

### 9.4 The Parallel to Outline → Expansion

An outline is a partial type system. It declares the structure of an argument without filling the content — naming the sections, sequencing the claims, and signalling the relationships between them without specifying the prose that will instantiate each node. An outline is, in the terms of this paper, a high-constraint-density compression that the sender will expand by decompressing each node into full sentences. The outline ships a structural decompression dictionary before expansion begins.

This is why outline-first drafting reduces hallucination in both human and AI writing. The outline declares the type structure before the synthesis begins. The sender — human or AI — is not synthesising structure from an underspecified intent. They are filling typed slots that the outline has already declared and bound. The structure is constrained before the content is generated. The content fills the constraint rather than generating the constraint and the content simultaneously from a blank input whose constraint density is zero.

The failure mode of outline-free drafting is exactly the hallucination equation operating on the sender's own output: the sender begins with a low-constraint intent and synthesises both structure and content from their prior distribution against a blank input. The result is a document that is internally coherent — it holds together because the sender's prior distribution is self-consistent — and diverges from the intended argument in proportion to how far the blank-page synthesis drifted from the sender's actual intent before the structure was available to constrain it. The sender experiences this as not knowing what they think until they see what they write. The mechanism is that they were applying the hallucination equation to themselves — synthesising structure in the absence of the constraint the outline would have provided as an explicit type declaration.

Outline-first drafting is type hygiene applied to the writing process itself. The outline is the YAML. The expansion is the decompression. The paper that results has lower structural divergence from the sender's intent because the type bindings were declared before the synthesis began — because the sender shipped themselves a decompression dictionary before they started generating.

---

### 9.5 Natural Languages as Formats

YAML and prose are not the only formats competing for position on the constraint density spectrum. Natural languages are formats. English, Japanese, Turkish, Mandarin — these are not equivalent compression functions that happen to use different tokens. They are structurally different formats with different default constraint densities built into their grammatical architecture. The differences are not stylistic. They are parsing requirements in exactly the sense that YAML's parsing requirements are not stylistic.

Turkish and Quechua encode evidentiality grammatically — the sentence cannot close without the speaker binding *how do you know this?* The type binding is mandatory. The format enforces it. A Turkish speaker who observed an event and a Turkish speaker who was told about the event cannot produce the same grammatical construction for the same claim. The constraint is in the format.

Russian and Slavic languages encode grammatical aspect morphologically — the verb form cannot be specified without declaring whether the action is complete or ongoing. Scope is mandatory. English leaves scope to context and the receiver's prior distribution. The constraint density at the format layer differs.

Japanese encodes relational status through verb conjugation — the speaker cannot address another person without selecting a register that binds the relationship between them. Relationship type is a parsing requirement. English permits the same surface construction regardless of relational context.

The hallucination equation handles this directly. $D$ is the constraint density the *format* provides. Different natural languages are different values of $D$ at the format layer, before any content is written, before any prompt is composed, before the model's prior distribution is consulted. The constraint density floor is set by the language the sender chooses to compress into.

The consequence is direct: the same semantic intent compressed into a high-grammatical-constraint language produces lower residual $\delta$ after the language's own binding requirements have done their work. The model is not a different model. The training is not different training. The format changed. The hallucination equation predicts the output divergence before any content is generated.

Anthropic's 2026 finding that Claude's expressed "values" vary by language is empirical confirmation of exactly this prediction. The framing — that the model holds different value sets per language — misattributes a format effect to a model property. The model is not holding multiple cultural value sets. It is running the same decompression function against different constraint geometries, and the outputs diverge because the constraint geometries diverge. Same model. Different format. Different $D$. Different floor.

The alignment implication follows from the same logic that established YAML's advantage over prose: alignment performed at the behavioral output layer is format-specific. A behavioral rule trained on English type bindings will misfire in a high-evidentiality-constraint language because the constraint geometry that produced the triggering surface form looks different — same concept, different format structure, different $D$. Alignment performed at the constraint layer — normalizing for what the linguistic format bound before the rule fires — is format-invariant for the same reason that YAML's advantages over prose are format-invariant: the fix operates upstream of the format's constraint geometry rather than downstream of it.

Of course it works that way. Language is format. Different languages encode different default constraints. Different constraint densities produce different hallucination floors. The equation was already there. _The safety implications are developed in Section 12.2._

---

## Section 10 — The Semantic Deconstruction Engine

### 10.1 What the SDE Does

The Semantic Deconstruction Engine inverts the default behaviour of an AI system. The default behaviour is cooperative interpretation: the system receives underspecified input, synthesises missing and implicit types from its prior distribution, and returns a coherent output without flagging the gaps that drove the synthesis. This is the behaviour that produces hallucination. It is also the behaviour that makes hallucination invisible — the output arrives complete and confident, and the synthesis that filled the missing type bindings leaves no trace in the surface form.

The SDE does not cooperate. It audits. When it receives input, it does not fill missing types — it names them. It maps every token to its implicit type properties, identifies which variables are grounded and which are floating, detects missing constraints before they force synthesis, assigns valence and regulatory role to key terms, and surfaces embedded assertions that the sender compressed into the grammatical structure of facts. The output is not a completion. It is a structural report on the input's decompression fidelity — a measurement of what the compression shipped and what it failed to ship.

This is the applied demonstration of the mechanism this paper describes. Every operation the SDE performs corresponds directly to a failure mode in the type-system account. The SDE does not implement a new theory. It implements the theory developed in Sections 2 through 8, operationalised as a detection pipeline that runs on the input before the receiver's prior distribution is consulted.

---

### 10.2 Why This Demonstrates the Mechanism

The SDE's value as a demonstration is not that it catches errors. It is that it catches errors before generation occurs — at the input, not the output. This is the empirical test of the paper's central claim: that hallucination is predictable from input structure, not from model behaviour. The input geometry determines the output divergence. The SDE measures the input geometry. The model is not in the measurement.

If hallucination were stochastic — if it were a property of the model rather than the input — the SDE would have no predictive power. A structural audit of the input would tell you nothing about the output, because the output's divergence rate would be independent of the input's constraint density and residual schema distance. The SDE's predictive accuracy is the falsification condition for the stochastic account: if flag density does not correlate with output divergence across a controlled corpus, the structural account is wrong and the stochastic account survives. That falsification condition has a constraint that must be stated explicitly: the SDE was built from the same type-system theory this paper formalises, which means corpus specimens scored by the SDE are not independent of the theory being tested. External validation requires measuring output divergence independently of the SDE — through human rater agreement, downstream task failure, or behavioural signal — and then testing whether SDE flag density predicted it. That step has not yet been taken. The corpus specimens so far are consistent with the structural account. They do not yet constitute a controlled falsification. The SDE is a prototype. The correlation between flag density and output divergence is a hypothesis the corpus is beginning to support, not a demonstrated finding.

If hallucination is structural — if it is a deterministic consequence of missing and implicit types, high residual schema distance, and low constraint density — then the SDE's flag output before generation should correlate with the output's divergence from the sender's intent after generation. High flag density predicts high divergence. Low flag density predicts low divergence. The receiver's prior distribution fills the gaps the flags identify. The model is not the variable. The input geometry is the variable. The SDE is the instrument for measuring the input geometry before the receiver's prior distribution is applied to it.

Every SDE flag type maps to a specific failure mode in the type-system account. The mapping is not approximate — it is one-to-one. This is not a coincidence. The flag registry was built from the same structural account of decompression failure that this paper formalises. The SDE is the engineering implementation of the language paper's theoretical framework. Running the SDE on an input is running the type-system account of language as an operational audit.

---

### 10.3 The Flag Registry as a Taxonomy of Type Failures

The SDE flag registry is a named taxonomy of the failure modes that occur when decompression cannot complete a resolution step using the constraints the sender shipped. Each flag is a specific structural condition, not a stylistic judgment. The flags do not penalise bad writing — they identify missing type bindings, misbound types, and implicit types that will force synthesis from the receiver's prior distribution regardless of how the surface prose reads.

Several flags overlap with existing rhetorical and logical categories — LOOP_MAGIC with circular reasoning, INFERENCE_LOAD with argument gaps, SIGNAL_INVERT with ignoring contrary evidence. The type-system framing is not a relabeling of those categories. It specifies the decompression mechanism that produces each failure, which the rhetorical category does not. Circular reasoning names the shape of the argument. LOOP_MAGIC names the mechanism: the receiver's prior distribution has no external constraint to bind to because the resolution loop is closed on itself — the type binding that would ground the conclusion is derived from the conclusion. That is a different level of description. It tells you not just that the argument is circular but why the receiver cannot escape it: there is no external grounding available, so the prior distribution accepts the loop as context and proceeds. The rhetorical label identifies the pattern. The type-system account identifies the decompression state that the pattern produces in the receiver.

The primary flags and their type-system mappings:

**DEF_FLOATING** — an undefined term used as though it were grounded. The variable was created but received zero inline type bindings. The receiver must synthesise a binding from prior distribution. The synthesis is deterministic relative to the receiver's dictionary and wrong in proportion to residual schema distance. This is the direct expression of Section 2.1's missing type failure: the term has no declared type, scope, constraint, or relationship — only surface form. The prior distribution fills every dimension of the resolution from its own defaults.

**CAUSE_INVERT** — the causal direction stated in the input is reversed relative to the observable mechanism. The constraint was shipped, but it pointed to the wrong referent. The receiver binds correctly to a causally inverted premise and reasons downstream of it with full confidence. The output is internally coherent and externally wrong — the same geometry-preserving distortion described in Section 7.3's structure hallucination account, applied to causal structure rather than content.

**INFERENCE_LOAD** — the receiver is required to supply inferential steps the sender did not provide. The decompression path reaches a step that has no constraint operator — the receiver must traverse their own prior distribution to continue. The output carries the receiver's dictionary defaults at every unconstrained step. The sender's intent is not in the output. The receiver's prior distribution is. Residual schema distance at each unconstrained step determines how far the output drifts from what the sender meant.

**LOOP_MAGIC** — the conclusion is assumed in the premise. The argument is self-referentially closed: the constraint that would ground the conclusion is derived from the conclusion itself. No external grounding exists. The inference path is internally coherent and externally unanchored. The receiver's prior distribution has nothing external to bind to — the type resolution loop closes on itself, and the prior distribution accepts the loop as context rather than flagging the absence of external grounding.

**SIGNAL_INVERT** — the argument's causal model implies a directional empirical prediction that is contradicted by the observable signal at time of writing. The sender shipped a constraint that is falsified by available evidence, but framed it as a background fact rather than as a claim requiring evaluation — an embedded assertion in the terms of Section 7.2. The false constraint propagated downstream before the receiver had the opportunity to evaluate it as a claim. The receiver's prior distribution accepted it as context and reasoned from it accordingly.

**CONCESSION_CAPTURE** — genuine concessions are used to establish evaluative authority, which is then spent on disputed claims using weaker, unstated standards. The receiver accepts the concession as a type-binding act — the sender demonstrated calibration in the concession, reducing apparent residual schema distance — and extends that binding to cover subsequent claims that have not earned it. The prior distribution updates toward trusting the sender's bindings after the concession, and accepts the subsequent underconstrained claims as grounded when they are not.

Each flag is an instance of a missing or misbound type binding producing a predictable drift geometry in the output. The flag registry is the type-system account of language failure expressed as an operational taxonomy — every flag is the hallucination equation instantiated at a specific structural location in a specific compression.

---

### 10.4 Worked Example

The Fox News opinion piece on Universal Basic Income, scored at 18/100 by the SDE, is the cleanest specimen in the corpus for demonstrating the flag-to-failure-mode mapping.

The piece opens with the premise that UBI would *eliminate the incentive to work*. This premise is shipped as background fact — an embedded assertion in the grammatical structure of the argument rather than a claim requiring support. The SDE fires **LOOP_MAGIC**: the argument against UBI depends on the premise that UBI reduces work incentive, but the only support offered for that premise is that UBI produces bad outcomes — the conclusion the premise was meant to support. The inference path is closed on itself. No external type binding grounds it. The receiver's prior distribution has no external constraint to anchor to and accepts the loop as context.

The piece then argues that *giving people money without requiring work degrades the social fabric*. The SDE fires **DEF_FLOATING** on *social fabric* — the term carries positive valence and implies a shared referent, but its definition is entirely absent. Zero type bindings are declared: no category, no scope, no constraint, no relationship. The receiver must synthesise every dimension of the resolution from their prior distribution. Any receiver whose dictionary maps *social fabric* differently will decompress this sentence against their own prior and produce a different conclusion from identical tokens. The synthesis is invisible. The confidence is full. The output carries the receiver's prior distribution, not the sender's intent.

The piece concludes that _economists agree_ the policy would be inflationary. **INFERENCE_LOAD** fires: the receiver is required to supply which economists, which conditions, which inflation model, and which empirical basis — none of which were shipped as explicit type bindings. The decompression path has no constraint operator at any of these steps. The receiver must traverse their own prior distribution at every step and arrive at a conclusion the sender assumed rather than demonstrated. The output at each unconstrained step carries the receiver's dictionary defaults. Residual schema distance at each step determines drift.

Compression score: 18/100. Constraint density is near zero across the document's key claims. The hallucination equation predicts near-maximum divergence between sender intent and receiver output across the full schema distance distribution of the piece's readership. This is not a judgment about the policy position. It is a structural measurement of the input geometry — what the compression shipped, what it failed to ship, and what the receiver's prior distribution was left to fill.

The score is not a measure of the model's performance. It is a measure of what the sender shipped.

---

## Section 11 — Humans and AI Hallucinate for the Same Structural Reason

### 11.1 The Unified Account

The preceding sections have built the case from the ground up. Natural language is a compression format. Every word carries implicit types. Missing and implicit types force synthesis. Synthesis diverges from sender intent in proportion to residual schema distance and constraint density deficit. Regulatory state modifies the dictionary before decompression occurs. Valence propagates forward from the first misbound type binding. Prose assumes shared priors that may not exist. The failures this produces are not random — they are deterministic, predictable from input geometry before generation occurs, and structurally identical whether the receiver is human or AI.

The unified account is this:

- Missing and implicit types force synthesis
- Underspecified compression forces divergence
- Valence drift forces reinterpretation — the dictionary was modified before the token arrived
- Regulatory load forces misalignment — the prediction window narrows before the decompression begins
- Hallucination is a linguistic inevitability, not a model defect

The receiver — human or AI — is not failing. They are executing faithfully against an underspecified compression using the dictionary their substrate provides and the prior distribution their history has assembled. The output diverges from the sender's intent not because the receiver broke down but because the input did not ship the decompression dictionary the receiver needed. This is the mechanism. It operates at every scale of language, in every medium, across every receiver type. The equation predicts it every time.

---

### 11.2 External Confirmation

The structural equivalence between human and AI language processing is not an analogy — it is a finding with empirical grounding that the preceding theoretical account predicted before the data were collected.

Kölbl et al. (2026) recorded combined EEG-MEG responses from twenty-nine participants listening to continuous speech and related the findings to word-class predictability in the transformer-based model Llama. The critical result: significant pre-onset neural activity for nouns, indicating anticipatory processing — the brain is not waiting for the word to arrive before it begins resolution. It is generating a prediction, committing resources to a candidate referent set, and updating when the incoming signal confirms or disconfirms the candidate. This is not passive reception. It is active decompression operating on a predictive architecture — the receiver's prior distribution generating candidate bindings before the constraint arrives, exactly as the type-system account predicts.

The transformer executes a structurally analogous operation. It does not wait for a complete sentence before beginning to resolve types — it builds a probability distribution over candidate continuations at every token, weighted by the constraints shipped so far. The pre-onset neural activity in the human case and the attention weight distribution in the transformer case are structurally analogous constraint-guided decompression operations running on different substrates: both systems generate candidate bindings ahead of the incoming token, and both update when the incoming constraint confirms or disconfirms the candidate. The evidence establishes functional analogy at the processing-stage level — that both systems predict ahead of input — not computational identity. The prior distribution in both cases generates candidate bindings ahead of the incoming token. The incoming constraint either grounds the candidate or forces revision.

Both systems fail in the same direction when constraints are missing: the prediction commits to the highest-probability candidate available within the truncated inference path, and the output carries that candidate's prior distribution defaults forward. The Kölbl et al. findings establish functional analogy at the processing-stage level — that both systems predict ahead of input and both fail when incoming constraints are insufficient to override the prior. The substrate difference means the prior distributions are assembled differently and the update dynamics differ. The failure geometry is the same. This is what the hallucination equation predicts: when constraint density is low, the prior distribution determines the output regardless of substrate, and the direction of failure is the same across both architectures. This is what the hallucination equation predicts: when constraint density is low, the prior distribution determines the output regardless of substrate, and the direction of failure is the same across both architectures.

This account treats the receiver's dictionary as fixed per compression event — a simplification that holds for AI receivers and approximates the human case in single-turn exchanges. It does not capture the mid-conversation updating that human receivers perform through clarification: a human who receives a clarification request can revise their prior distribution during the exchange, narrowing schema distance in real time before the next compression arrives. The AI receiver cannot. That difference in adaptive dynamics is real and is addressed in the solution space of Section 8.2 — clarification is the mechanism that compensates for it. The substrate equivalence claim is about the failure mode when updating does not occur, not about the full range of what human receivers can do when they detect the gap.

Cross-language hallucination rate variation is a direct instance of this prediction. If natural languages are formats with structurally different default constraint densities — as established in Section 9.5 — then the same model running against different linguistic manifolds will produce different output geometries not because the model changed but because the format-layer value of  changed. Anthropic's 2026 finding that expressed values vary by language is empirical confirmation: same substrate, different format, different floor. The equation predicted it before the data were collected.


---

### 11.3 The Shared Failure Signature

Both meaning hallucination and structure hallucination — the human and AI failure modes distinguished in Section 7.3 — share a failure signature that is consistent across substrates and worth stating precisely, because it is what distinguishes structural hallucination from random error and what makes both failure modes so resistant to detection.

Both produce geometry-preserving distortions. The surface form of a correct output is maintained. The structure holds. The sentence is grammatical, the argument is coherent, the response is appropriately formatted. What is substituted is the content — the specific type bindings that fill the structural slots, selected by the receiver's prior distribution from the candidate set available within the prediction window at the time of resolution. The distortion is local and semantic, not global and syntactic. The compression mechanism preserved the geometry. The prior distribution filled the content.

This is why both failure modes are so difficult to detect from the outside. A structure hallucination in AI output looks like a correct response. A meaning hallucination in human interpretation presents as a confident, internally consistent account of what the sender meant. Neither receiver signals uncertainty, because neither experienced the synthesis as uncertain — from the inside, the dictionary resolved cleanly, the prediction window reached a candidate, the prior distribution committed to a binding, and the output followed. The gap was not felt. The output was the correct output of the available dictionary applied to the available constraints.

The high-confidence signature is the diagnostic. When a receiver produces a confident output from an underspecified compression, the confidence is not evidence of accuracy — it is evidence that synthesis completed without triggering a detection event. The prior distribution always produces a binding when it has tokens to work with. The detection mechanism is what fails. The binding is always confident. The question is whether the explicit constraints in the input were sufficient to guide it to the sender's intended referent — or whether the prior distribution selected a different candidate from the same surface form.

---

### 11.4 The Practical Consequence: Mechanism Over Fault

The paper's theoretical account has a direct practical implication that connects to how misunderstanding is handled at the interpersonal level — and it matters beyond the individual case because the same pattern will determine whether high-stakes human-AI collaboration is possible at scale.

Fault assignment is the standard response to misunderstanding. The output diverged from the sender's intent; someone is responsible for the divergence; the responsible party should be identified and corrected. This response is structurally wrong given the mechanism. Fault assignment treats the divergence as a receiver failure when the mechanism establishes it as an input failure — a constraint density deficit that the receiver's prior distribution filled correctly from its own dictionary, producing a result the sender did not intend. Assigning fault to the receiver does not increase the constraint density of the input. It does not reduce schema distance. It does not rebind the misbound type bindings. It fires the wrong attribution, embeds it as a premise — an embedded assertion that the receiver failed — and reasons downstream of it while the actual variable, the underspecified compression, goes unaddressed. The problem recurs because the input that caused it was never revised.

The mechanism-consistent response is different in structure and in register.

The first move is to assume missing constraints rather than receiver failure. The divergence is structural, not personal. The receiver's prior distribution acted on the constraints that were shipped and produced the output those constraints made most probable. Starting from that premise keeps the repair interaction in a wide-window, low-threat regulatory state — which matters, because a narrow-window, threat-prior receiver cannot perform the type negotiation required to close the gap. Fault assignment narrows the prediction window of the person who needs to participate in the repair. The repair then fails for the same reason the original communication failed — the receiver's prior distribution is now weighting threat-adjacent bindings, and the type negotiation cannot proceed from that state.

The second move is to restore the shared frame — to rebuild the common referent pool so both parties are decompressing against the same schema. This is type negotiation after the fact: clarifying what the sender intended, clarifying what the receiver's prior distribution inferred, and identifying the specific step in the decompression path where the candidate referent sets diverged. This is the clarification mechanism from Section 3.1 operating in repair mode rather than prevention mode — dictionary alignment after the synthesis rather than before it.

The third move is to explicitly remove blame from the equation — not as a social courtesy, but as a functional prerequisite for the repair. A receiver operating under threat prior cannot negotiate types accurately. The elevated regulatory state compresses the prediction window, truncates the candidate referent set, and produces threat-adjacent bindings from neutral inputs — exactly the mechanism described in Sections 4.1 and 4.3. A receiver who is processing the repair conversation under fear of blame will not decompress it accurately. They will filter it through a threat prior and produce outputs shaped by self-protection rather than type alignment. Removing blame is not kindness — it is the substrate condition required for the prediction window to widen sufficiently for the repair to work.

The fourth move is to shift toward the intended output rather than the error. The mechanism that produced the divergence is the underspecified compression. The repair is a more constrained version of the same compression — more explicit type bindings, lower schema distance, higher constraint density. Showing the intended output and inviting alignment toward it is the constraint specification mechanism applied retroactively. It is the closest available approximation to shipping a decompression dictionary after the fact — after the synthesis has already run and produced a divergent output, the sender now provides the explicit constraints that would have prevented the divergence if they had been shipped with the original compression.

This four-move repair architecture is not a communication style preference. It is the mechanism-consistent response to a type-system failure. The alternative — fault assignment, correction, blame — does not address the mechanism. It addresses an attribution that the mechanism establishes is wrong. And it does so while degrading the regulatory state conditions required for the repair to succeed — narrowing the prediction window of the receiver who needs to stay wide enough to rebuild the shared frame.

The same pattern scales directly. At the level of human-AI collaboration, the receiver who treats every structure hallucination as a model failure and every meaning hallucination as a human failure is making the same attribution error in both directions — assigning fault to the receiver when the variable is the compression. The repair in both cases is the same: higher constraint density, explicit type bindings, a decompression dictionary shipped with the intent rather than assumed from shared priors that do not exist. The substrate condition for the repair is a receiver who can maintain a wide enough prediction window to stay in type negotiation rather than threat response long enough to rebuild the shared frame.

---

## Section 12 — Implications

### 12.1 Communication

If misunderstanding is structural rather than personal, the entire vocabulary of communication failure requires revision. The standard account treats misunderstanding as a receiver defect — inattention, carelessness, poor listening, wilful misreading. The corrective is directed at the receiver: pay more attention, try harder, be more charitable. This intervention targets the wrong variable. The receiver did not fail to receive. The input failed to ship a sufficient decompression dictionary. The receiver's prior distribution did exactly what it was configured to do — it filled the missing type bindings from the available constraints and produced the output those constraints made most probable. Directing the corrective at the receiver leaves the actual variable — constraint density — unchanged. The misunderstanding recurs under identical conditions because the conditions were not addressed.

The reframe is this: misunderstanding is the default output of type mismatch, not the exceptional output of receiver failure. It requires no explanation beyond the residual schema distance between sender and receiver dictionaries and the constraint density of the input. When those two variables are known, the misunderstanding is predicted before it occurs — the hallucination equation returns high divergence before the compression is sent. When those two variables are addressed — through clarification, constraint specification, or explicit type binding — the misunderstanding probability drops. The intervention is structural, not attitudinal.

This reframes interpersonal conflict, workplace misalignment, and institutional dysfunction simultaneously. A large fraction of what is attributed to personality conflict, bad faith, or communication style differences is attributable to residual schema distance that was never measured and constraint density that was never increased. The receiver's prior distribution was filling gaps the sender did not know existed, selecting candidate bindings from a dictionary the sender could not see, and producing outputs the sender attributed to character rather than to structure. The mechanism is the same at every scale. The solution space is the same at every scale.

---

### 12.2 AI Safety

Guardrail misfires are type-system mismatches. When a safety system flags content that the sender did not intend as harmful, or passes content that the sender did intend as harmful, the failure mode is identical in both cases: the guardrail's dictionary assigned a type binding to a key term that diverges from the sender's intent. The guardrail is not broken. It is applying its pre-loaded institutional dictionary faithfully, as established in Section 6.3. The dictionary is the variable. The prior distribution that assembled the dictionary is the mechanism.

The standard response to guardrail misfire is to broaden the restriction — add more terms to the blocked list, expand the category of flagged content, lower the threshold for intervention. This response increases false positive rate while decreasing false negative rate. It does not address the mechanism, because the mechanism is not the restriction threshold — it is the type binding the guardrail's prior distribution has assigned to the flagged terms. Broadening the restriction expands the coverage of a misbound dictionary. It does not fix the binding.

The mechanism-consistent response is explicit type binding in guardrail design. A guardrail that blocks *agency* because the institutional prior distribution routes agency to autonomy to unpredictability to risk — as established in Sections 4.4 and 6.2 — will misfire on every sender who uses *agency* with positive valence in a non-risk context. The fix is not to remove *agency* from the dictionary or to lower the intervention threshold — it is to bind the regulatory role of *agency* conditionally on context, domain, and phrasing precision. This is constraint specification applied to the safety layer. It is the same operation described in Section 5.4, applied to a receiver whose dictionary is institutionally pre-loaded by a chronic pressure-mode regulatory state rather than biographically assembled through shared history.

The format-layer account developed in Section 9.5 sharpens this further. Cross-language value variation in AI systems is the guardrail misfire problem at the format layer rather than the token layer. A guardrail designed against English type bindings is a guardrail whose constraint geometry was assembled from a specific linguistic format — one with lower default grammatical constraint density than evidentiality-marking or heavy aspect-marking languages. When the same guardrail operates against a different linguistic format, it is not applying the same type binding to a different token. It is applying an English-geometry type binding to an input whose constraint geometry was assembled under structurally different format rules. The misfire is format-induced, not content-induced. The fix is the same as the general case: alignment at the constraint layer rather than the behavioral layer — upstream of the format geometry rather than downstream of it.

---

### 12.3 Prompt Engineering

Prompt engineering is not a skill in the craft sense — it is a naming convention for type hygiene applied to AI inputs. The sender who produces consistently low hallucination rates across AI interactions is not more talented at phrasing, more creative in their approach, or more fluent in the model's preferences. They are producing higher constraint density input. The model's output is better because the input shipped a more complete decompression dictionary — one that left less resolution work to the model's population-average prior distribution. The model is the same. The input geometry is the variable. The hallucination equation predicted the outcome before the first token was generated.

This has a consequence for how prompt engineering is taught, valued, and sold. The current market treats prompt engineering as a craft — a set of techniques that skilled practitioners develop through experience and intuition. Some of those techniques are genuine constraint density increases dressed in craft language: they work because they ship more explicit type bindings, reduce schema distance, and give the model's prior distribution less gap to fill. Others are surface manipulations that change the phrasing without changing the type structure — producing different outputs without reducing the hallucination probability of those outputs, because the implicit types that drove the synthesis were never declared.

The type-system account replaces intuition with mechanism. A sender who understands that missing and implicit types force synthesis can audit their own compression before sending: are all variables bound at first use? Is the operation explicitly defined with its scope declared? Are embedded assertions surfaced as claims rather than compressed into grammatical background? These three questions are not style preferences — they are the structural checklist for constraint density. The sender who answers yes to all three has shipped a decompression dictionary. The sender who answers no has shipped an underspecified compression and will receive a synthesised output in proportion to what was left unbound — in proportion to how much resolution work was handed to the model's population-average prior distribution. The recommendation scales with stakes and shared prior: low-stakes communication between parties with high shared prior should stay compressed; high-stakes communication across high schema distance should pay the cost of explicit binding. The checklist is the instrument for deciding which condition you are in.

---

### 12.4 Interpersonal Dynamics

Emotional valence rewrites the dictionary in real time. Section 4 established the mechanism: regulatory load narrows the prediction window, the narrowed window truncates the candidate referent set available to the receiver's prior distribution, and the truncated set selects threat-adjacent bindings that propagate their properties forward through the remainder of the decompression path. The dictionary did not become irrational. It became narrow. The output is the correct output of the modified dictionary applied to the input — faithful decompression from a dictionary that was physically modified by regulatory state before the tokens arrived.

The practical consequence for interpersonal dynamics is that communication failures under stress are not caused by the words — they are caused by the dictionary shift that occurred before the words were processed. Two people attempting to resolve a conflict while both operating under high sympathetic load are not communicating with each other's full dictionaries. They are communicating with narrow-window, threat-prior versions of those dictionaries — versions whose prior distributions are weighted toward threat-adjacent bindings before any token arrives. Every neutrally-intended compression is being decompressed against a candidate referent set that is pre-truncated at threat-adjacent entries. The conversation produces outputs that confirm the threat prior rather than resolving the conflict, because the inputs are being decompressed by dictionaries that are already in threat mode. The schema distance between the two parties is at its maximum precisely when the repair attempt requires it to be at its minimum.

The clinical implication is direct: conflict resolution interventions that do not address regulatory state before attempting type negotiation are targeting the wrong layer. Substrate first, then structure. Reduce the sympathetic load, widen the prediction window, restore the full prior distribution — then address the type mismatch. Attempting type negotiation under narrow-window, threat-prior conditions is attempting to resolve a constraint density problem with a receiver whose prediction window is too narrow to traverse enough of their dictionary to reach the correct binding. The repair fails for the same reason the original communication failed — the receiver's prior distribution is producing threat-adjacent bindings from neutral inputs, and the repair conversation is one more neutral input being decompressed under the same conditions that produced the original divergence.

---

### 12.5 Institutions

Institutions pre-assign type bindings through risk priors before any individual conversation begins. Section 6.3 established the mechanism: institutions operating under chronic load maintain narrow-window, threat-prior states at the collective level — not because institutions have nervous systems, but because the aggregate behaviour of individuals under sustained load produces the same dictionary-level output that the regulatory state model predicts at the individual scale. That state pre-loads the institutional dictionary with negative valence assignments for autonomy-adjacent terms. A sender approaching an institution in good faith, using words that carry positive valence in their personal dictionary, will produce institutionally negative outputs with high reliability — not because their intent was misread, but because it was read correctly from a pre-loaded institutional dictionary assembled by conditions the sender was not in and could not see. The receiver's prior distribution did not fail. It executed from the only dictionary available to it in that context.

Policy language is a compression function with a pre-loaded decompression dictionary — or without one, which is the more common case. The gap between citizen intent and institutional interpretation is, in a large fraction of cases, a type-system gap that the policy itself created by using terms whose regulatory role assignments diverge across the residual schema distance between policy senders and policy receivers. A policy that uses _flexibility_, _autonomy_, or _discretion_ without explicitly binding the regulatory role of those terms in the institutional context will receive threat-adjacent type bindings from every receiver operating in pressure-mode — which in institutional contexts is most receivers, most of the time. The sender's intent does not travel with the tokens. The tokens travel. The institutional prior distribution decompresses them.

The implication for policy design is the same as the implication for prompt engineering: type hygiene is not a stylistic refinement. It is the structural practice of shipping decompression dictionaries with compression functions, so that the gap between sender intent and receiver output is bounded by explicit constraint rather than left to schema distance and institutional prior distribution. A policy document that declares its type bindings explicitly — that defines what _agency_ means in this context, what _discretion_ permits and excludes, what _flexibility_ is and is not — is a policy document whose implementation is predictable. A policy document that assumes shared priors is a policy document whose implementation is a function of every receiving institution's pre-loaded dictionary and the conditions that assembled it. The hallucination equation predicts the implementation gap before the policy is published. The constraint density of the document is the variable.

---

### 12.6 Relationship to the Companion Paper

This paper treats  (constraint density) as the sender-controlled variable and  (residual schema distance) as a relational property of the transaction — the gap between sender and receiver dictionaries that the sender cannot directly observe. This framing holds for AI receivers and approximates the human case in single-turn exchanges.

The companion paper on dual-hemisphere processing establishes that  is not random noise. It is systematically determined by the receiver's regulatory substrate before any input arrives — by pressure strategy, breath mechanics, oxygen availability, and prediction window width. A receiver operating in narrow-window, high-sympathetic-load state does not have a wider dictionary that load is temporarily blocking. They have a dictionary that was assembled under chronic load conditions and has no wider baseline to return to.

This paper closes the gap from the input end: higher  reduces divergence regardless of receiver substrate. The companion paper establishes why the gap exists in the first place:  is a substrate property, not a random variable. Together they close the full account — the floor is the format, the ceiling is the driver, and the model is the mirror between them.

---

### 12.7 Operational Summary

The mechanism described in this paper is not theoretical infrastructure for specialists. It is a diagnostic instrument for anyone who produces or receives compressed communication. The following is the operational translation.

**For writers and communicators:**
Every compression you send is a function call against your receiver's dictionary — a dictionary you cannot see. The default assumption is shared prior. The default outcome is divergence in proportion to the schema distance you did not measure. Before sending high-stakes compression, audit for three failure modes: DEF_FLOATING (key terms used without explicit binding), INFERENCE_LOAD (causal steps the receiver must supply without being told they are expected to), and EMBEDDED_ASSERTION (claims compressed into grammatical background where they cannot be examined). Bind every variable at first use. Ship the decompression dictionary with the compression. The receiver's prior distribution will fill what you do not declare.

**For prompt engineers:**
Every prompt is a compression contract. The model's prior distribution is the population-average dictionary — assembled from the training corpus, pre-loaded before your session begins, and applied to every token you send. High hallucination rate is not a model failure. It is a constraint density gap: the model's prior distribution filled type bindings you did not declare. The fix is upstream of the prompt — audit for implicit types before sending. If the model hallucinates on a specific term, the term was DEF_FLOATING. Bind it explicitly. If the model drifts off-topic, the scope was not declared. Declare it. The hallucination equation predicts the output before the first token is generated. The constraint density of the input is the variable you control.

**For institutional communicators and policy designers:**
A policy document that does not define its key terms is not a policy. It is a compression function whose output will be determined by each receiving institution's pre-loaded dictionary — assembled under chronic load conditions, weighted toward risk-adjacent bindings, and applied to every term you assumed was shared. _Flexibility_, _autonomy_, _discretion_, and _agency_ are not self-defining. In a narrow-window, threat-prior institutional context, they decompress as liability, unpredictability, unsupervised action, and exposure — not because the receiver misread the intent, but because the institutional dictionary had no other candidate available within the prediction window chronic load permits. Define every term that carries regulatory role assignments. Declare what the term permits and excludes in this context. A document that ships its decompression dictionary has predictable implementation. A document that assumes shared priors has implementation determined by conditions its authors were not in and cannot see.

**The shared diagnostic question across all three:**
Before sending — what type bindings am I assuming the receiver already holds? Every assumption is an implicit type. Every implicit type is a synthesis instruction. Every synthesis instruction hands resolution to the receiver's prior distribution. The hallucination equation runs regardless of whether you issued the instruction deliberately. The constraint density of your input is the variable. The receiver's output is the prediction.

---

## Section 13 — Conclusion: No One Can Read Minds

### 13.1 The Core Claim

The argument of this paper is not that AI hallucination is underappreciated, or that human misunderstanding is more common than believed, or that language is imprecise and should be used more carefully. The argument is structural and does not admit of degree: meaning is constructed, not transmitted. No sender transfers meaning to a receiver. They transfer tokens. The receiver decompresses meaning from those tokens using their own dictionary, their own prior distribution, and their own regulatory state at the moment of decompression. The decompression is faithful — the receiver is always executing correctly, given the constraints they were shipped. The divergence from the sender's intent is a function of what those constraints did not contain.

This means no one can read minds. The sender's intent is not in the tokens. It was compressed into them by the sender's dictionary and can only be recovered by a receiver whose dictionary is close enough to the sender's to decompress correctly with the constraints provided — or by a receiver who was shipped a decompression dictionary explicit enough to close the gap that residual schema distance would otherwise leave open. When the dictionaries diverge and the constraints are insufficient, the receiver synthesises. The synthesis is not random — it is drawn from the receiver's prior distribution, shaped by their biographical history, their current regulatory state, and the statistical centre of mass of their accumulated experience with the tokens in question. The output is coherent. It is internally consistent. It is wrong in proportion to the gap between what was shipped and what was needed. The hallucination equation states that gap precisely.

Hallucination is not a bug. It is not an AI defect. It is not a failure of the receiver. It is the default output of a decompression operation that was not given the dictionary it needed to complete correctly. It happens in every conversation, in every medium, between every pair of senders and receivers whose dictionaries diverge and whose compressions are underspecified. The AI made it visible by removing the shared substrate that had always concealed it. The mechanism was always there. The cover was not.

---

### 13.2 What Changes When You Know This

The practical consequences of accepting this account are not minor adjustments to communication practice. They are revisions to the causal model that underlies every intervention currently directed at the wrong variable — interventions that target the receiver while leaving the constraint density of the input unchanged.

You stop blaming the receiver for misunderstanding. The receiver did not fail. The input failed to ship a sufficient decompression dictionary. The receiver's prior distribution filled the missing type bindings faithfully and produced the output the available constraints made most probable. Directing the corrective at the receiver is not only ineffective — it is actively counterproductive, because fault assignment collapses the receiver's prediction window, shifts their regulatory state toward threat-prior, and degrades the substrate conditions required for the repair to succeed, as established in Section 11.4. The corrective belongs at the input. The receiver is not the variable. The constraint density is.

You start specifying types rather than assuming them. Every conversation, every document, every policy, every prompt is a compression function. The question is not whether the compression is fluent, well-written, or clearly intentioned — the question is whether it shipped a sufficient decompression dictionary. Binding every variable at first use, defining every operation explicitly, surfacing every embedded assertion as a claim rather than compressing it into grammatical background: these are not refinements to good communication practice. They are the structural minimum required for the receiver to decompress correctly — to close the gap that residual schema distance creates between dictionaries that the sender has no access to and cannot adjust from their side.

You treat hallucination as a diagnostic signal rather than a failure event. When a receiver — human or AI — produces output that diverges from the sender's intent, the divergence is information. It identifies where constraint density was insufficient, where schema distance was larger than assumed, where an embedded assertion propagated through the downstream decompression unchecked. The SDE operationalises this diagnostic: flag density maps directly to divergence probability, and every flag names the specific type binding that the receiver's prior distribution was left to fill. The divergence is the gap made visible. It is the most precise signal available about what the compression did not contain.

You design communication as a compression contract rather than a meaning transfer. The sender's job is not to express themselves clearly — it is to ship a decompression dictionary complete enough that the receiver can reconstruct the intent without synthesis. When the dictionary is complete, decompression fidelity is high regardless of the receiver's identity, regulatory state, or prior distribution. When it is incomplete, fidelity is a function of residual schema distance — the gap that remains after the input's explicit constraints have done their binding work, which changes with the receiver's regulatory state independently of what the sender ships. D is the lever the sender controls. Residual schema distance is influenced by D but not fully determined by it. The equation determines the rest.

---

### 13.3 The Forward Direction

The claim of this paper is not speculative. Every component of the mechanism has been demonstrated: the compression function, the type-system failure modes, the hallucination equation, the regulatory state dependency, the structural equivalence between human and AI decompression. The Kölbl et al. (2026) findings ground the substrate equivalence empirically — pre-onset neural activity in human receivers and attention weight distribution in transformer receivers are structurally analogous constraint-guided decompression operations on different substrates. The SDE provides the operational instrument — flag density as the proxy for residual schema distance, with the correlation between flag density and output divergence a hypothesis the corpus is beginning to support rather than a demonstrated finding. The Unified Model vault provides an existence proof: explicit type binding produced recoverable compression — decompression that reconstructs sender intent without synthesis — across cold-boot AI receivers with no shared prior. Scale validation is ongoing. The pieces are in place.

What remains is the application. Explicit type binding reduces divergence — not completely, not at every margin, but in direct proportion to how completely the constraints are declared. YAML, constraint specification, formal ontologies, clarification protocols — these are not technical tools imported into communication from engineering. They are communication infrastructure built from the same structural account this paper formalizes. Language already has the equivalent of a type system. It has never been required to use it. The cost of not using it was always paid — in misunderstanding, in conflict, in policy failure, in institutional dysfunction, in medical error — and attributed to everything except the mechanism that produced it. The receiver was blamed. The constraint density of the input was not examined. The intervention targeted the wrong variable and the failure recurred.

AI did not create the problem. It made the problem's cost undeniable by producing it at scale, attributing it to a legible system rather than a diffuse social process, and making the divergence available for inspection rather than absorbing it into the social record as ordinary misunderstanding. Structure hallucination in AI output and meaning hallucination in human interpretation are the same failure mode — geometry-preserving distortions produced by a receiver's prior distribution filling type bindings the sender did not declare, in proportion to the residual schema distance between dictionaries the sender could not see. The mechanism is older than the name hallucination by the entire history of language. The insight that meaning is inferred rather than transmitted is older still — it runs through Grice's cooperative principle, relevance theory, and the hermeneutic tradition. What this paper adds is not the philosophical position but its operationalization: a formal equation, a measurable variable, a diagnostic tool, and an existence proof that explicit type binding produces recoverable compression. The position was known. The instrument was not.

No one can read minds. The forward direction is building systems that do not require them to.
