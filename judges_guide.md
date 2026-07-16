# Emo Corner

> **Playable Reddit experience**
>
> Open Emo Corner here:
>
> **Reddit Playtest:**  
> https://www.reddit.com/r/emo_corner_dev/?playtest=emo-corner
>
> **Devvit App Page:**  
> https://developers.reddit.com/apps/emo-corner
>
> The current demo allows both sides of the experience to be tested from one Reddit account using the mode toggle.
>
> If you face any issue opening or testing the experience, contact:
>
> **khushira2244@gmail.com**

## A world made by others helps a Chrononaut travel through time

Emo Corner is a Reddit Devvit Web experience where one person shares a feeling and another person turns it into an interactive world using objects, words, music, paths, movement, and care.

The person receiving that world becomes a Chrononaut.

After the corner is posted, the Chrononaut enters the exact scene another person created, collects coins, travels through space, and carries the written words into a Time Room.

Emo Corner transforms a Reddit post from something people only read into something they can build, enter, travel through, and remember.

> **Emo Corner is a community world-building system where any human situation can become an interactive journey created by other people.**

---

## What’s Next

The current hackathon build demonstrates the foundation of a much larger community world-building system.

The next version of Emo Corner will connect real Reddit users through Devvit storage so that one person can share a feeling and other people can create, contribute to, and preserve worlds for them.

Planned product additions include:

- persistent feelings and created corners
- real multi-user posting and building
- several makers contributing to one world
- saved Chrononaut journeys
- community reactions and voting
- moderation and safety tools
- accessibility improvements
- revisiting words and moments from earlier journeys
- collaborative paths, objects, messages, and events
- creator profiles
- world histories
- long-term Time Room memories

### Expanding the worlds

The same builder and journey system can support many kinds of environments:

- peaceful forests
- underwater rooms
- dream roads
- cities
- homes
- memory spaces
- rescue missions
- racing worlds
- fantasy adventures
- survival journeys
- space battles
- collaborative cities
- community-created landscapes

### Expanding time

Future Time Worlds can include:

- different Time Rooms
- time wars
- broken timelines
- alternate futures
- memory restoration
- community-built histories
- worlds that change as more people contribute
- moments that return in later journeys
- connected memories across different worlds

These would not be random game levels.

Every world would still begin with something a person shared, and every journey would be shaped by what other people created for them.

For the hackathon, the current scenarios prove that the Emo Corner system can move across:

```txt
feeling
→ community response
→ world builder
→ interactive scenario
→ posted scene
→ coins
→ space
→ time
→ preserved memory
```

After judging, new worlds can be added without changing the core idea:

> **Any human situation can become an interactive journey created by other people.**

---

## Source Code

The source repository is private.

The complete playable build is available through the Reddit Devvit links at the top of this README.

---


## How Emo Corner Works

Emo Corner represents two Reddit-user roles.

### Person 1 — Share mode

One Reddit user shares how they currently feel.

They can:

1. Choose a feeling.
2. Select the closest situation or scenario.
3. Add a short reason.
4. Send the feeling into the waiting flow.

### Person 2 — Make mode

Another Reddit user discovers that feeling and creates a world for the person who shared it.

They can:

1. Open the Waiting Room.
2. View feelings waiting for a corner.
3. Choose one feeling.
4. Build an interactive comfort world.
5. Add objects, words, music, paths, and movement.
6. Post the completed world.

The person receiving the completed world becomes the Chrononaut and continues through the journey.

For the current hackathon demo, both roles can be tested from one Reddit account using the mode toggle in the top-right corner.

Posting and coin rewards are simulated so judges can experience the complete journey without needing two separate Reddit accounts or permanent backend data.

---

## How to Try It

Open the playable Emo Corner experience:

**Playable Reddit post:**  
https://www.reddit.com/r/emo_corner_dev/?playtest=emo-corner

**Devvit App Page:**  
https://developers.reddit.com/apps/emo-corner

For the best test, complete one full journey:

```txt
Share a feeling
→ switch to Make mode
→ choose a feeling from the Waiting Room
→ build and post the world
→ view the posted corner
→ continue to the Coin Room
→ travel through space
→ enter the Time Room
→ arrange the carried words and objects
→ create the final Time Post
```

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
9. Wait for the builder timer to finish.
10. Press **Post comfort**.

The posted corner preserves the objects and words placed by the maker.

Playing the same prepared scenario again starts a fresh builder session. Previous objects and words are removed from the new run.

---

## Text and Time Room

The builder currently allows up to **12 text characters** in one corner.

The words placed during the build are saved in the posted scene and carried into the Time Room later in the journey.

### To test words in the Time Room

1. Add one or more short words in the Section Builder.
2. Place the words on the scene.
3. Wait for the timer and post the corner.
4. Continue to the Coin Room.
5. Enter the Space Journey.
6. Complete the space sequence.
7. Enter the Time Room.
8. The words from the posted corner appear as movable blocks.
9. Move the words and hanging objects during the Time Room timer.
10. Press **Post** after the timer ends.
11. The final Time Post opens with the completed arrangement.

In the current demo, the Time Room uses words from the **current posted corner**.

Playing again starts a new journey. The Time Room does not replay every movement made during the timer.

The final Time Post stores only:

```ts
{
  feelingId,
  storyLine,
  words: [
    {
      id,
      text,
      x,
      y
    }
  ],
  objects: [
    {
      id,
      assetSrc,
      x,
      y,
      size
    }
  ],
  postedAt
}
```

The Time Post displays:

- the same Time Room background
- the final word positions
- the final object positions
- no dragging
- no timer
- no movement replay
- no animation controls

The close button returns the user to the Chrononaut landing screen.

Persistent multi-user and cross-session history is planned with Devvit storage.

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

Different scenarios can become:

- peaceful nature spaces
- underwater worlds
- dream roads
- racing environments
- space journeys
- memory rooms
- Time Worlds

---

## Dream Blocked Racing Scenario

Select the scenario with the feeling:

> **“My dream feels stuck and I cannot move forward.”**

Its scenario ID is:

```txt
dream-blocked
```

This opens the normal Section Builder with:

- dream-road racing background
- movable racing car
- engine sound
- drawing trail
- normal builder timer
- normal text tools
- normal object tools
- normal posting flow

The racing experience is embedded inside the Section Builder. It is not a separate page.

### Racing controls

The four controls appear together on the left:

```txt
↺  ↻  ↑  ↓
```

Current behavior:

- `↺` rotates the car anticlockwise
- `↻` rotates the car clockwise
- `↑` moves the car in reverse
- `↓` drives the car forward

Keyboard arrow controls are also supported.

The car leaves a trail while moving.

There are no checkpoints, required letters, or completion validation. The maker can drive and draw freely while also using the normal builder tools.

---

## Posted Corner

After the maker presses **Post comfort**, the posted Level 1 corner opens.

The posted corner:

- preserves the maker’s exact object arrangement
- preserves written words
- keeps the selected background
- keeps the scenario music
- replays the created scene
- provides a **Next** button to continue the journey

The posted corner does not require the user to rebuild the scene.

The coin data remains available in the parent flow even when detailed upvote, comment, and coin information is hidden from the posted scene.

---

## Coin Room

After viewing the posted corner, the Chrononaut continues to the Coin Room.

The current hackathon version simulates coin rewards so judges can experience the complete journey without requiring live community voting or multiple real users.

Coins are used as a bridge between:

```txt
the created comfort world
→ the larger Chrononaut journey
```

The Coin Room leads into the Space Journey.

---

## Space Journey

The Chrononaut enters a space journey after the Coin Room.

The Space Journey includes:

- a movable ship
- keyboard and touch controls
- planets
- collision behavior
- music and sound
- a black-hole transition
- continuation into the Time Room

Entering the Space Journey does not deduct coins.

Normal planet-hit behavior remains part of the interactive sequence.

The black hole appears after the flight has progressed and leads the Chrononaut into the Time Room.

---

## Time Room

The Time Room carries forward the words written in the Section Builder.

Inside the room:

- words appear as movable memory blocks
- random objects initially hang around the room
- objects can be moved
- objects do not rotate
- words and objects can be freely arranged
- the room timer runs for 30 seconds
- the Post button appears when the timer reaches zero

The room assets preload before the timer begins so the user does not lose arrangement time while the background and objects are loading.

The Time Room uses:

- a central wall
- angled left and right walls
- a perspective floor
- a dark vignette
- a deeper, hypnotic room effect
- gentle hanging motion before the final post

When the user presses **Post**, only the final arrangement is preserved.

---

## Time Post

The Time Post is a separate, non-interactive final screen.

It displays:

- `TIME POSTED`
- the same Time Room background
- final word positions
- final object positions
- one close button

It does not include:

- dragging
- a timer
- movement timestamps
- replay controls
- screenshots
- the full 30-second timeline

The only stored time is:

```ts
postedAt: Date.now()
```

Closing the Time Post returns to:

```txt
Make the world, become Chrononaut
[Waiting Room]
```

---

## Journey After Posting

After the corner is posted:

1. The exact created scene is shown.
2. The Chrononaut continues to the Coin Room.
3. Coins are carried into the Space Journey.
4. The Chrononaut flies through space.
5. The journey continues through the black hole.
6. Words from the posted corner enter the Time Room.
7. The Chrononaut arranges the words and objects.
8. Pressing **Post** preserves the final arrangement as a Time Post.
9. Closing the Time Post returns to the Chrononaut landing screen.

The Time Post stores only the final arrangement. It does not save screenshots or replay the complete movement history.

The central idea is that a Reddit post becomes something another person can build, enter, carry forward, and remember.

---

## Built With

- Reddit Devvit
- Devvit Web
- React
- TypeScript
- Phaser
- Vite
- HTML5 Canvas
- Web Audio
- CSS

React manages the main application flow, including:

- sharing feelings
- the Waiting Room
- Section Builder
- object and text placement
- builder timer
- posted scenes
- Coin Room
- Space Journey
- Time Room
- Time Post

Phaser is embedded specifically in the `dream-blocked` Section Builder scenario to power:

- the racing background
- car movement
- car rotation
- touch controls
- keyboard controls
- engine sound
- drawing trail

---

## How We Built It

Emo Corner was built as a Reddit Devvit Web experience using React, TypeScript, Phaser, Vite, HTML5 Canvas, Web Audio, and CSS.

React manages the feeling flow, waiting room, builder tools, scene posting, Coin Room, Space Journey, Time Room, and Time Post.

Phaser powers the embedded racing experience inside the `dream-blocked` scenario.

Scenario-based presets connect each feeling to its own:

- background
- music
- object collection
- world type
- interaction style

When the maker posts a corner, the arrangement of objects and words is preserved so the Chrononaut sees the same world that was created.

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

- The hackathon version uses prepared feeling scenarios.
- The builder timer is approximately 74 seconds so makers have enough time to place objects, write words, and interact with scenario tools.
- Posting and coin rewards are simulated in the current demo.
- Both user roles can be tested from one Reddit account through the mode toggle.
- The posted Level 1 corner preserves the maker’s arrangement.
- One posted journey carries its own written words into the Time Room.
- The Time Room timer is 30 seconds.
- The Time Post saves the final word and object arrangement.
- The full Time Room movement timeline is not stored.
- A fresh builder is created when the same scenario is selected again.
- Permanent real-user and cross-session history will be connected through Devvit storage in a future version.
- The playable Reddit link is available to organizers and judges.
- The source repository is private.

---


## Contact

For testing or access issues:

**Email:** khushira2244@gmail.com

**Reddit username:** u/Various_Elevator_503

**Playable experience:**  
https://www.reddit.com/r/emo_corner_dev/?playtest=emo-corner

**Devvit App Page:**  
https://developers.reddit.com/apps/emo-corner
