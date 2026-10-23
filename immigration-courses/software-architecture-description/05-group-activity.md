# Group Activity: From Context to Architecture

Now the floor is yours.

The activity is deliberately open-ended. The goal is not to reproduce one predetermined diagram, but to **reason from the problem statement to a defensible architecture**.

## Part 1 · Discuss and define requirements

Identify requirements for the Train Station Simulator and organize them into:

- **functional requirements**;
- **non-functional requirements**;
- **basic requirements**;
- **creative requirements**.

:::{note} Questions that can guide the discussion
### Understanding the system and its context
- What are the primary goals and objectives of the Train Station Simulator?
- What is a typical user scenario?
- In which operational environments will it be used?
- Who are the primary stakeholders?

### Functional requirements
- Which functionalities are needed to reproduce a real railway station?
- Which commands and responses must be exchanged between Central Control and Station Simulator?
- How should the Train Simulator interact with field entities?

### Non-functional requirements
- What are the performance requirements, especially for communication speed and responsiveness?
- What levels of reliability and accuracy are needed?
- How usable should the operator interfaces be?
- Which scalability and integration properties are needed for future expansion?
- Which security measures are necessary?
:::

## Part 2 · Design an abstract architecture

On paper or a whiteboard:

1. identify the major architectural components;
2. assign responsibilities;
3. draw the important interactions;
4. identify architectural styles or patterns that may be useful, if applicable;
5. connect important architectural choices back to requirements.

:::{important} Do not optimize the drawing
The quality of the exercise is in the **reasoning and discussion**, not in producing a polished diagram. Boxes and arrows are enough if the responsibilities and rationale are clear.
:::

## Part 3 · Iterate

If time allows, challenge your first design:

- What happens if Central Control is replaced by a real station?
- Where should safety checks occur?
- Which communication paths must respect the 300 ms constraint?
- Which responsibilities are currently coupled too tightly?
- Which components may need to evolve independently?

:::{dropdown} Hint 1 · If a group is stuck
:class: hint
Start from nouns and verbs in the problem statement. Nouns often suggest domain concepts or responsibilities; verbs often suggest behavior and interactions. Do **not** assume every noun must become a component.
:::

:::{dropdown} Hint 2 · If a group jumps straight to implementation
:class: hint
Bring the discussion back to an **abstract architecture**: responsibilities, interfaces, interactions, and constraints. Specific technologies are secondary at this stage.
:::

:::{dropdown} Hint 3 · If a group ignores non-functional requirements
:class: hint
Ask them to locate the 300 ms constraint, safety expectations, reliability/accuracy, future integration, maintainability, and operator usability in their architecture.
:::

## What each group should be ready to explain

At the end, each group should be able to present:

- its main requirements;
- its proposed architectural components;
- at least two important architectural decisions;
- the requirement or constraint motivating each of those decisions.
