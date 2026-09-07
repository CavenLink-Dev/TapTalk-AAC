# TapTalk AAC User Flow

This file is the simple, version-controlled source of truth for the app flow. It renders directly in GitHub and can be recreated visually in FigJam or Figma when screen design begins.

## Main app flow

```mermaid
flowchart TD
    A[Open TapTalk AAC] --> B{First time?}
    B -- Yes --> C[Simple onboarding]
    C --> D[Choose voice and card size]
    D --> E[TapBoard]
    B -- No --> E

    E <--> F[TapTalk]
    F <--> G[QuickTalk]
    G <--> E

    E --> H[Settings]
    F --> H
    G --> H
    H --> E
```

## TapBoard flow

```mermaid
flowchart LR
    A[TapBoard] --> B[Tap symbol card]
    B --> C[Add word to message bar]
    C --> D{Next action}
    D -->|Add more| B
    D -->|Speak| E[Speak full message]
    D -->|Backspace| F[Remove last word]
    D -->|Clear| G[Confirm and clear]
    E --> H[Stop or finish speech]
```

## TapTalk flow

```mermaid
flowchart LR
    A[TapTalk] --> B[Type a message]
    B --> C{Next action}
    C -->|Speak| D[Speak typed message]
    C -->|Save| E[Name or confirm phrase]
    E --> F[Save to QuickTalk]
    F --> G[Show saved confirmation]
```

## QuickTalk flow

```mermaid
flowchart LR
    A[QuickTalk] --> B[Tap saved phrase]
    B --> C[Speak phrase]
    A --> D[Add or edit]
    D --> E[Type phrase and label]
    E --> F[Save]
    A --> G[Delete phrase]
    G --> H{Confirm deletion?}
    H -- Yes --> I[Delete]
    H -- No --> A
```

## Settings flow

```mermaid
flowchart TD
    A[Settings] --> B[Speech: voice, preview, speed]
    A --> C[Display: card and text size]
    A --> D[Data: reset, backup or export]
    A --> E[Privacy]
    A --> F[Symbols and licences]
    A --> G[Help and audio troubleshooting]
    A --> H[About and app version]
```

## Flow rules

- TapBoard, TapTalk, and QuickTalk are the three main destinations.
- Settings is available from every main screen but is not a fourth main communication tab.
- The message bar stays familiar across communication screens where practical.
- Speaking, stopping speech, and clearing a message must always be easy to find.
- Destructive actions require confirmation; ordinary communication actions do not.
- Every flow must work with VoiceOver and large touch targets and must not create a dead end.
