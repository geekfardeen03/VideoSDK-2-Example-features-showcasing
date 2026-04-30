# VideoSDK — Example Features Showcasing

**Submitted by:** Fardeen NS Khan  
**College:** B.Tech CSE, SVNIT Surat  
**GitHub:** github.com/geekfardeen03  

---

## What is in this repository

This repository contains two standalone VideoSDK React examples built to demonstrate core real-time communication features:

1. Screen Sharing Example  
2. In-Meeting Chat Example  

Both applications are fully functional React projects and can be run independently.

---

## Folder structure

```bash
VideoSDK-2-Example-features-showcasing/
│
├── videosdk-examples/
│   ├── screen-share-example/   ← Example 1 — screen sharing
│   └── chat-example/           ← Example 2 — real-time chat
│
└── README.md
```

---

## How to run each project

Every project follows the same setup.

### Step 1 — Go into project folder

For screen sharing:

```bash
cd videosdk-examples/screen-share-example
```

For chat:

```bash
cd videosdk-examples/chat-example
```

---

### Step 2 — Install dependencies

```bash
npm install
```

---

### Step 3 — Create `.env`

Create a `.env` file inside that project:

```env
REACT_APP_VIDEOSDK_TOKEN=your_token_here
```

Get your token from:

https://app.videosdk.live

After login:

**Dashboard → API Keys → Auth Token**

---

### Step 4 — Start application

```bash
npm start
```

App runs on:

```bash
localhost:3000
```

---

## What each project does

---

## screen-share-example — Example 1

This example demonstrates how to add screen sharing to a VideoSDK meeting.

Inside a live meeting:

- Click **Share Screen**
- Browser opens native screen picker
- Select tab, window, or full screen
- Screen stream is broadcast live to all participants
- Stop sharing with one click

The core feature is implemented using:

```javascript
toggleScreenShare()
```

from the VideoSDK `useMeeting()` hook.

### Tech used

- React
- VideoSDK React SDK
- Tailwind CSS

---

## chat-example — Example 2

This example demonstrates real-time in-meeting text chat.

Inside a live meeting:

- Type message
- Press Enter
- Message appears instantly for all participants
- Sender name and timestamp are shown

VideoSDK handles messaging internally.

Core APIs used:

```javascript
sendChatMessage()
```

and

```javascript
onChatMessage()
```

### Tech used

- React
- VideoSDK React SDK
- Tailwind CSS

---

## Video Tutorial

Full walkthrough:

https://drive.google.com/file/d/1T5YD2Y-6_ZFdIkeKrybDh0YZzA_6im01/view?usp=drive_link

The tutorial covers:

- Live demo
- Code walkthrough
- Feature explanation
- Debugging process
- Implementation details

---

## Important note about the auth token

The `.env` file is intentionally not committed.

The dashboard token:

- Is temporary
- Expires after some time
- Should never be pushed publicly

To run these examples, generate your own token from:

https://app.videosdk.live

In production, tokens should be generated server-side.

---

*Fardeen NS Khan — geekfardeen03 on GitHub*
