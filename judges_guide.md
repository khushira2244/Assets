

## Emo Corner

> **Public testing notice — July 16, 2026**
>
> Emo Corner is currently being prepared for public testing. I am waiting for the public Reddit testing access and related emails to become active.
>
> If you face any problem opening or testing the experience, please contact:
>
> **khushira2244@gmail.com**

**A world made by others helps a Chrononaut travel through time.**

**A world made by others helps a Chrononaut travel through time.**

Emo Corner is a Reddit Devvit Web experience where one person shares a feeling and another person turns it into an interactive world using objects, words, music, movement, and care.

After the corner is posted, the Chrononaut enters the created world, collects coins, travels through space, and carries the written words into a Time Room.

---

## How to Try It

Open the playable Emo Corner post in the public testing subreddit:

**Playable post:** Add the direct Reddit post link here.

For the best test, complete one full journey from selecting a feeling to reaching the Time Room.

---

## Mode Toggle

A toggle appears in the top-right corner of the main screen.

### Share mode

Use this mode to:

1. Choose how you currently feel.
2. Select the closest scenario.
3. Add a short reason.
4. Send the feeling into the waiting flow.

### Make mode

Turn the toggle on to:

1. Open the Waiting Room.
2. View feelings waiting for a corner.
3. Select one feeling.
4. Build an interactive comfort world for it.

The current hackathon demo uses prepared scenarios so the complete experience can be tested with one Reddit account.

---

## How to Test the Main Builder

1. Turn on **Make mode**.
2. Select a feeling from the Waiting Room.
3. The Section Builder opens with a scenario-specific background, music, and objects.
4. Press the `+` button to open the object collection.
5. Select an object and tap the world to place it.
6. Drag placed objects to move them.
7. Select a placed object to rotate, resize, duplicate, or delete it.
8. Use the writing button to add a short word.
9. Wait for the 60-second timer to finish.
10. Press **Post comfort**.

The posted corner preserves the objects and words placed by the maker.

---

## Text and Time Room

The builder currently allows up to **12 text characters** in one corner.

The words placed during that build are saved in the posted scene and carried into the Time Room later in the journey.

### To test words in the Time Room

1. Add one or more short words in the Section Builder.
2. Place the words on the scene.
3. Wait for the timer and post the corner.
4. Continue to the Coin Room.
5. Enter the Space Journey.
6. Complete the space sequence.
7. Enter the Time Room.
8. The words from the posted corner will appear as movable blocks.

In the current demo, the Time Room uses words from the **current posted corner**. Playing again starts a new journey; words do not permanently accumulate across separate runs yet.

Persistent multi-user history is planned with Devvit storage.

---

## Scenarios

Each feeling is mapped to its own builder preset containing:

- background
- music
- object collection
- world type
- special interaction

The demo includes scenarios around:

- job loss
- heartbreak
- overthinking
- family anger
- blocked dreams or feeling stuck

---

## Dream Blocked Racing Scenario

Select the scenario with the feeling:

> **“My dream feels stuck and I cannot move forward.”**

Its scenario ID is:

```txt
dream-blocked
````

This opens the normal Section Builder with:

* dream-road racing background
* movable racing car
* engine sound
* drawing trail
* normal builder timer
* normal text tools
* normal object tools
* normal posting flow

The racing experience is embedded inside the Section Builder. It is not a separate page.

### Racing controls

The four controls appear together on the left:

```txt
↺  ↻  ↑  ↓
```

Current behavior:

* `↺` rotates the car anticlockwise
* `↻` rotates the car clockwise
* `↑` moves the car in reverse
* `↓` drives the car forward

Keyboard arrow controls are also supported.

The car leaves a trail while moving. There are no checkpoints, required letters, or completion validation. The maker can drive and draw freely while also using the normal builder tools.

---

## Journey After Posting

After the corner is posted:

1. The exact created scene is shown.
2. The Chrononaut enters the Coin Room.
3. Coins are carried into the Space Journey.
4. The Chrononaut flies through space.
5. The journey continues into the Time Room.
6. Words from the posted corner become part of the Time Room interaction.

The main idea is that a Reddit post becomes something another person can build, enter, and remember.

---

## Built With

* Reddit Devvit
* Devvit Web
* React
* TypeScript
* Phaser
* Vite
* HTML5 Canvas
* Web Audio
* CSS

React manages the main application flow, including sharing feelings, the Waiting Room, Section Builder, posting, Coin Room, Space Journey, and Time Room.

Phaser is embedded specifically in the `dream-blocked` Section Builder scenario to power the racing background, car movement, rotation, touch and keyboard controls, engine sound, and drawing trail.

---

## Local Development

Install dependencies:

```bash
npm install
```

Run locally:

```bash
npm run dev
```

Check TypeScript:

```bash
npm run type-check
```

Create a production build:

```bash
npm run build
```

Upload through the local Devvit CLI:

```bash
npx devvit upload
```

---

## Current Demo Notes

* The hackathon version uses prepared feeling scenarios.
* The builder timer is 74 seconds.(its very hard to minimize into 60sec)
* One posted journey carries its own written words into the Time Room.
* Permanent cross-session word accumulation is enabled .

---

## What’s Next

The next version of Emo Corner will connect real Reddit users through Devvit storage.

Planned additions include:

* persistent feelings and created corners
* multiple makers contributing to one world
* saved Chrononaut journeys
* reactions and community voting
* moderation and safety tools
* accessibility improvements
* more interactive scenarios
* revisiting words and moments from previous journeys


