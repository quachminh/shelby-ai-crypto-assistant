# Shelby AI Crypto Assistant

An experimental AI crypto research assistant built with Shelby SDK.

## Features

- Collect on-chain data from blockchain APIs
- Analyze X (Twitter) sentiment about crypto projects
- Generate quick research summaries using AI
- Provide early insights for new token launches

## Why Shelby

Shelby provides powerful infrastructure for building AI agents that interact with crypto data and social signals.

## Tech Stack

- Node.js
- Shelby SDK
- OpenAI
- Social sentiment analysis

## Example Use Case

Input:research: new Aptos ecosystem projects

Output:
- On-chain metrics
- Community sentiment
- Risk indicators
- AI summary

## Future Plans

- Dashboard UI
- Telegram bot
- Auto alerts for new tokens
- const { analyzeProject } = require("./api/research")

async function main() {

const project = "Aptos"

const result = await analyzeProject(project)

console.log("Research Result:")
console.log(result)

}

main()
const sentiment = require("../services/sentiment")
const onchain = require("../services/onchain")

async function analyzeProject(project){

const chainData = await onchain.fetch(project)

const sentimentData = await sentiment.analyze(project)

return {
project,
onchain: chainData,
sentiment: sentimentData
}

}

module.exports = { analyzeProject }
git clone https://github.com/USERNAME/shelby-ai-crypto-assistant.git

cd shelby-ai-crypto-assistant

git add .

git commit -m "initial AI crypto research assistant"

git push
