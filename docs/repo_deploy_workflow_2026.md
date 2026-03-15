# Micro Mirror Snapshot + VitalScope Deployment Workflow Guide

## TL;DR

The long-term active repository is now intended to be:
- `vitalscope`
- `https://github.com/uplinkira/vitalscope`

This repository remains:
- `micro-mirror-deploy`
- the archived March 14, 2026 Shenzhen hackathon snapshot

## What This Means Operationally

- develop future product work in `vitalscope`
- keep `micro-mirror-deploy` as the historical snapshot and deploy mirror for the hackathon version
- if you want a future-facing Vercel project, bind Vercel to `vitalscope`

## What Vercel Is Actually Doing

For this project, Vercel is mainly doing four things:

1. Git integration
- it watches a connected GitHub repository
- pushes to connected branches trigger deployments

2. Build and package
- it turns a commit snapshot into a deployable output
- for this project, that output is a static front-end bundle

3. Preview vs production routing
- production branch pushes become production deployments
- non-production branches can become preview deployments

4. Hosted delivery
- it serves the deployment output from its platform edge network

## Why Free Deployment Works Right Now

The current snapshot and the future VitalScope main repo are both lightweight enough that `Hobby` is acceptable for low-traffic preview use:

- mostly static HTML, CSS, and browser-side JavaScript
- camera flow runs in the browser
- wallet flow runs in the browser
- no heavy always-on backend

## Important Boundary

According to Vercel's current plan documentation:
- `Hobby` is free
- `Hobby` is intended for personal, non-commercial use

So free deployment works now because:
- the app is light
- the traffic is small
- the project is still in preview / prototype stage

It should not be read as:
- permanent production advice
- a commercial scaling strategy

## Pricing Snapshot

At the time of writing, Vercel publicly lists:
- `Hobby`
  - free
- `Pro`
  - `$20` per user per month
  - plus additional usage
- `Enterprise`
  - custom pricing

## Recommended Repo Strategy

- active repo:
  - `vitalscope`
- archive repo:
  - `micro-mirror-deploy`

That keeps:
- the long-term product clean
- the hackathon snapshot preserved
- the deployment story easier to explain

## Fastest Path To Future Deployment

Open:
- `https://vercel.com/new/clone?repository-url=https://github.com/uplinkira/vitalscope`

Then:
- log in
- import the repo
- click `Deploy`

## `VERCEL_TOKEN` Quick Guide

1. Log in to `https://vercel.com`
2. Open account settings
3. Create an access token
4. Keep it out of Git

Example:

```bash
export VERCEL_TOKEN="your_token_here"
cd /Users/orangesnail/Desktop/agent_yaqi/D+20260314+goat/vitalscope
./node_modules/.bin/vercel --prod --token "$VERCEL_TOKEN"
```

## Local Preview

For the future main repo:

```bash
cd /Users/orangesnail/Desktop/agent_yaqi/D+20260314+goat/vitalscope
python3 -m http.server 8000
```

For this historical snapshot repo:

```bash
cd /Users/orangesnail/Desktop/agent_yaqi/D+20260314+goat/micro-mirror-deploy
python3 -m http.server 8000
```

## One-Sentence Version

Use `vitalscope` for all future product work, and keep `micro-mirror-deploy` as the March 14, 2026 Shenzhen hackathon snapshot.
