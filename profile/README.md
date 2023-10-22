# Zuko

**Permissionless**, **Privacy-Focused** social dApp. Connecting anonymous users to communities using [Simso Connect](https://sismo.io/) and [Tableland](https://tableland.xyz/).

<div align="center">
<img 
  src="https://github.com/usezuko/.github/raw/prod/assets/zuko-logo-coloured.png" 
  style="width:40% ; height:40%;"
/>
</div>

## 🏁 Introduction

Zuko is for individuals who value their **privacy** and seek a **secure and confidential** space to engage in online communities or forums.

Joining the APE holders' community 🦍 ? Don't monkey around with imposters or phishing risks!

Imagine a place where you can chat with fellow APE's, prove your token status, and stay incognito. That's where **Zuko** swings in!

Zuko is your **offshore, safe haven** for connecting with proven like-minded peers, from hosting your DAO discussions to an **exclusive** network of users.

**Visit <a href="https://zuko-zk.netlify.app/">Zuko</a> at the Deployed Netlify Website**

### 🪜 How it works

1. Connect your wallet to Sismo's data vault.
2. Pick your trusted community.
3. Choose a username.
4. Voila! It's done. Your info stays on-chain, safe from leaks.

## ✨ Features

1. ⚓ **Custom Usernames**: Users can personalize their identity with unique custom usernames.

2. 🏘️ **Community Participation**: Joining communities is optional, allowing users to tailor their experience to their interests.

3. 🚩 **Post Creation**: Users can create and share posts within their chosen communities.

4. 🎸 **Engagement**: Users can engage with the community by commenting on posts and liking both posts and comments.

5. ☔ **Identity Protection**: Each user has a unique username, image, and pseudo ID, ensuring a secure and confidential experience.

6. ⛽ **Gasless**: Gas and other on-chain operations are abstracted from the user.

## 🗺️ Architecture

![Overview](https://github.com/usezuko/.github/raw/prod/assets/architecture.png)

## 🌐 Software

- **Sismo**: We use Sismo's Connect Data Vault to let users generate ZK proofs from their wallet (data source), so that we can fetch their vaultId (user pseudonym), and groupId (community).
- **Tableland**: We wanted a permissionless SQL-like on-chain database. We used their Studio & Console clients, SDK, and CLI to create, store, test, and manage tables & queries. Tables are hosted on Goerli Arbitrum (we're cheap) & locked.
- **Stack**: NextJS, NodeJS, TypeScript, ExpressJS, Netlify, SQL, ReactJS, TailwindCSS.

## 🔨 Limitations / Improvements
- **Team Constraints**: Team of 3, each with full-time jobs, dedicating weekends and nights. We had to carefully plan for MVP and sacrifice certain requirements deemed optional.
  
- **Feature Enhancements**:
    - *Recursive Commenting*: Comments on comments in posts.
    - *Unlimited Communities*: Limited by Sismo on pre-defined groups (communities) to add communities without additional devOps.
    - *Content Updates*: Allow users to edit and update comments, posts, and profile pictures.
    - *DAO Admin Control*: Ability for communities to be governed & controlled by the members themselves; giving control over descriptions, images, and entry requirements.
    - *Additional Data Sources*: Add Sismo Data Source venues beyond wallets, such as Twitter and Telegram, for community expansion.

- **Latency Improvements**:
    - *Server-Side Optimization*: Improve server response times to reduce front-end load.
    - *Client-Side Efficiency*: Improve UX and UI performance.
    - *Caching with CDN*
    - *Micro API Optimization*
    - *Framework Selection*: Evaluate more efficient frameworks and technology stacks.
    - *Decentralized Client Integration*: Fleek.co for permissionless hosting (extra work on the routes).

- **Gasless Transactions**: Gasless but at the cost of security.

## 🔧 Contributing

We welcome any feedback, improvements, and amendments to these repositories 🙌 :

- [API Server](https://github.com/usezuko/zuko-server) - A Server API connecting to the tableland on-chain DB.
- [Frontend](https://github.com/usezuko/zuko-zk) - A NextJS frontend dApp.
