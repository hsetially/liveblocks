<p align="center">
  <a href="https://liveblocks.io#gh-light-mode-only">
    <img src="https://raw.githubusercontent.com/liveblocks/liveblocks/main/.github/assets/header-light.svg" alt="Liveblocks" />
  </a>
  <a href="https://liveblocks.io#gh-dark-mode-only">
    <img src="https://raw.githubusercontent.com/liveblocks/liveblocks/main/.github/assets/header-dark.svg" alt="Liveblocks" />
  </a>
</p>

# TipTap Notifications Emails (Resend)

<p>
  <a href="https://liveblocks.io/examples/text-editor-emails/nextjs-tiptap-emails-resend">
    <img src="https://img.shields.io/badge/live%20preview-message?style=flat&logo=data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggZD0iTTE2Ljg0OSA0Ljc1SDBsNC44NDggNS4wNzV2Ny4wMDhsMTItMTIuMDgzWk03LjE1IDE5LjI1SDI0bC00Ljg0OS01LjA3NVY3LjE2N2wtMTIgMTIuMDgzWiIgZmlsbD0iI2ZmZiIvPjwvc3ZnPg==&color=333" alt="Live Preview" />
  </a>
  <a href="https://codesandbox.io/s/github/liveblocks/liveblocks/tree/main/examples/nextjs-tiptap-emails-resend">
    <img src="https://img.shields.io/badge/open%20in%20codesandbox-message?style=flat&logo=codesandbox&color=333&logoColor=fff" alt="Open in CodeSandbox" />
  </a>
  <img src="https://img.shields.io/badge/react-message?style=flat&logo=react&color=0bd&logoColor=fff" alt="React" />
  <img src="https://img.shields.io/badge/next.js-message?style=flat&logo=next.js&color=07f&logoColor=fff" alt="Next.js" />
  <img src="https://img.shields.io/badge/TipTap-message?style=flat&color=7bf" alt="TipTap" />
</p>

This example shows how to send email notifications when a user has an unread mention in a text editor with [Liveblocks](https://liveblocks.io), [Tiptap](https://tiptap.dev) [React Email](https://react.email/), [Resend](https://resend.com/), and [Next.js](https://nextjs.org/).

<img src="https://raw.githubusercontent.com/liveblocks/liveblocks/main/.github/assets/examples/text-editor-email.png" width="536" alt="Text Editor Emails" />

## Getting started

Run the following command to try this example locally:

```bash
npx create-liveblocks-app@latest --example nextjs-tiptap-emails-resend --api-key
```

This will download the example and ask permission to open your browser, enabling you to automatically get your API key from your [liveblocks.io](https://liveblocks.io) account.

`npm run dev:email` will open live previews of your emails, and `npm run dev` will run the Comments app.

### Setting up webhooks

You need to set up webhooks to make this example run.

- Follow our guide on [testing webhooks locally](https://liveblocks.io/docs/guides/how-to-test-webhooks-on-localhost), making sure to [check the “**notification**” event](https://liveblocks.io/docs/platform/webhooks#edit-endpoint-events) when creating the webhook
- Copy your **webhook secret key** from the webhooks dashboard
- Add your webhook secret key to `.env.local` as the `LIVEBLOCKS_WEBHOOK_SECRET_KEY` environment variable

### Setting up Resend

You need your own Resend API key to send the emails.

- Create an account on [Resend](https://resend.com)
- Create a new API key from the [Resend Dashboard](https://resend.com/api-keys)
- Add your Resend API key to `.env.local` as the `RESEND_API_KEY` environment variable

### Manual setup

<details><summary>Read more</summary>

<p></p>

Alternatively, you can set up your project manually:

- Install all dependencies with `npm install`
- Create an account on [liveblocks.io](https://liveblocks.io/dashboard)
- Copy your **secret** key from the [dashboard](https://liveblocks.io/dashboard/apikeys)
- Create an `.env.local` file and add your **secret** key as the `LIVEBLOCKS_SECRET_KEY` environment variable
- Run `npm run dev:email` and go to [http://localhost:3000](http://localhost:3000)
- Run `npm run dev` and go to [http://localhost:3001](http://localhost:3001)

</details>

### Deploy on Vercel

<details><summary>Read more</summary>

<p></p>

To both deploy on [Vercel](https://vercel.com), and run the example locally, use the following command:

```bash
npx create-liveblocks-app@latest --example nextjs-tiptap-emails-resend --vercel
```

This will download the example and ask permission to open your browser, enabling you to deploy to Vercel.

</details>

### Develop on CodeSandbox

<details><summary>Read more</summary>

<p></p>

After forking [this example](https://codesandbox.io/s/github/liveblocks/liveblocks/tree/main/examples/nextjs-tiptap-emails-resend) on CodeSandbox, create the `LIVEBLOCKS_SECRET_KEY` environment variable as a [secret](https://codesandbox.io/docs/secrets).

</details>
