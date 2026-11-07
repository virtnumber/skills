# Virtnumber Agent Skills

Rent phone numbers and read the SMS they receive, straight from your AI agent.

Virtnumber rents dedicated virtual phone numbers in 14 countries, one number to one customer. All numbers receive SMS. Two-way numbers in the US and Sweden can also send. This plugin adds the [Virtnumber MCP server](https://github.com/virtnumber/mcp) to your agent and two skills that teach it how to use it.

| Skill | Use it when |
|---|---|
| [`receive-sms`](skills/receive-sms/SKILL.md) | You need a phone number that receives SMS, want to wait for the next SMS, or test an app that sends SMS |
| [`send-sms`](skills/send-sms/SKILL.md) | You want to text someone from a US or Swedish number of your own and read the replies |

## Install

### Claude Code

```bash
/plugin marketplace add virtnumber/skills
/plugin install virtnumber@virtnumber
```

### Other agents (Codex, Cursor and more)

```bash
npx skills add virtnumber/skills
```

Then connect the MCP server in your client (see [virtnumber/mcp](https://github.com/virtnumber/mcp)).

## Setup

On first use your agent opens the Virtnumber sign-in (OAuth). You choose its permissions and a spending limit on the consent screen. Paid numbers come out of your prepaid balance, which you top up in your account at [virtnumber.com](https://www.virtnumber.com). Your agent asks before it rents a number or sends an SMS.

## Links

- [API and MCP reference](https://www.virtnumber.com/developer)
- [JavaScript SDK](https://github.com/virtnumber/virtnumber-js) (`npm install virtnumber`)
- [Privacy](https://www.virtnumber.com/privacy) · [Terms](https://www.virtnumber.com/terms)
- Support: tech@virtnumber.com
