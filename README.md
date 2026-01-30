# RGVAI Skills Collection

A curated collection of AI coding agent skills for Claude Code, Codex, and other AI assistants. These skills enhance AI agents with specialized knowledge for software development, marketing, and research tasks.

## 🎯 Overview

This repository serves as a central hub linking to all public skills developed and maintained by RGVAI. Each skill follows the open [Agent Skills standard](https://agentskills.io) and is compatible with Claude Code, OpenAI Codex CLI, Cursor, and other tools adopting this format.

## 📦 Available Skills

### Development & Architecture

| Skill | Description | Repository |
|-------|-------------|------------|
| **Code Architect** | Software architecture design, code structure planning, and technical documentation for building scalable, maintainable systems | [rgvai/code-architect](https://github.com/rgvai/code-architect) |

### Deployment & Infrastructure

| Skill | Description | Repository |
|-------|-------------|------------|
| **OpenClaw Cloudflare Setup** | Step-by-step guidance for deploying OpenClaw on Cloudflare Workers with R2 storage, including Zero Trust security configuration | [rgvai/openclaw-cloudflare-setup](https://github.com/rgvai/openclaw-cloudflare-setup) |

### Marketing & Copywriting

| Skill | Description | Repository |
|-------|-------------|------------|
| **Sell Like Crazy** | Apply Sabri Suby's "Sell Like Crazy" methodology to create high-converting marketing campaigns, buyer personas, lead magnets, sales copy, irresistible offers, Facebook/Google ads, and sales scripts | [rgvai/Sell-Like-Crazy-Skill](https://github.com/rgvai/Sell-Like-Crazy-Skill) |
| **Sabri Suby Headlines** | Generate 20 high-CTR direct-response headlines using Sabri Suby's proven methodology for attention-grabbing copy | [rgvai/Sabri-Suby-Headline-Skill](https://github.com/rgvai/Sabri-Suby-Headline-Skill) |
| **Marketing Skills** *(fork)* | Comprehensive marketing skills suite including CRO, copywriting, SEO, analytics, and growth engineering (25+ skills) | [rgvai/marketingskills](https://github.com/rgvai/marketingskills) |

### Research & Analysis

| Skill | Description | Repository |
|-------|-------------|------------|
| **Deep Research Agent** | A custom Claude skill that mimics Claude's built-in Research feature for comprehensive, multi-step information gathering and analysis | [rgvai/deep-research-agent](https://github.com/rgvai/deep-research-agent) |

### E-Commerce & Protocols

| Skill | Description | Repository |
|-------|-------------|------------|
| **UCP** *(fork)* | Specification and documentation for the Universal Commerce Protocol | [rgvai/ucp](https://github.com/rgvai/ucp) |

## 🚀 Quick Installation

### Using Claude Code CLI

```bash
# Install any skill using Claude Code's plugin system
/plugin marketplace add rgvai/Sell-Like-Crazy-Skill
/plugin install sell-like-crazy

# Or install directly
claude skill add rgvai/code-architect
```

### Using npx skills

```bash
# Install specific skill
npx skills add rgvai/Sell-Like-Crazy-Skill

# Install from repo
npx skills add rgvai/code-architect
```

### Manual Installation

```bash
# Clone and copy to your skills directory
git clone https://github.com/rgvai/[skill-name].git
cp -r [skill-name]/SKILL.md ~/.claude/skills/
```

## 📚 Skill Details

### Code Architect

A comprehensive skill for software architecture design that helps with:

- System architecture design and documentation
- Technology stack decisions and ADRs (Architecture Decision Records)
- Code structure planning and best practices
- Technical documentation generation
- Design pattern recommendations

**Usage:**
```
"Help me architect a microservices system for an e-commerce platform"
"Create an ADR for our database selection"
"Design the folder structure for a React/Node.js application"
```

### OpenClaw Cloudflare Setup

A deployment guide skill for setting up OpenClaw on Cloudflare infrastructure:

- Cloudflare account setup and billing configuration
- Workers and R2 storage service configuration
- GitHub repository integration
- Anthropic API key configuration
- Secure token generation
- Zero Trust security configuration (the critical step most tutorials miss)
- Device authorization for initial access

**Usage:**
```
"Help me deploy OpenClaw on Cloudflare"
"Guide me through the OpenClaw Cloudflare setup"
"Set up Zero Trust for my OpenClaw deployment"
```

### Sell Like Crazy Skill

Based on Sabri Suby's bestselling book, this skill helps create:

- **Buyer Personas**: Detailed customer avatars with demographics, psychographics, pain points, and buying triggers
- **Lead Magnets**: High-value free offers that attract qualified prospects
- **Sales Copy**: Direct-response copy using the "Sell Like Crazy" framework
- **Irresistible Offers**: Godfather offers customers can't refuse
- **Ad Campaigns**: Facebook and Google ad copy optimized for conversions
- **Sales Scripts**: Phone and video sales scripts using proven methodologies

**Usage:**
```
"Create a buyer persona for a SaaS productivity tool"
"Write a Godfather offer for my coaching program"
"Generate Facebook ad copy using the Sell Like Crazy methodology"
```

### Sabri Suby Headline Skill

Generates 20 high-converting headlines using direct-response principles:

- Attention-grabbing hooks
- Curiosity-driven openers
- Benefit-focused headlines
- Problem-agitation headlines
- Social proof headlines

**Usage:**
```
"Generate 20 headlines for my weight loss product"
"Create direct-response headlines for a B2B software launch"
```

### Deep Research Agent

Mimics Claude's built-in Research feature with:

- Multi-step research workflows
- Information gathering and synthesis
- Source evaluation and citation
- Comprehensive report generation

**Usage:**
```
"Research the current state of AI regulations in the EU"
"Conduct deep research on competitor pricing strategies"
```

### Marketing Skills (Fork)

A comprehensive collection of 25+ marketing skills from [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills):

**Conversion Optimization:**
- `page-cro` - Landing page optimization
- `signup-flow-cro` - Registration flow optimization
- `onboarding-cro` - User activation optimization
- `form-cro` - Lead capture form optimization
- `popup-cro` - Modal and overlay optimization
- `paywall-upgrade-cro` - In-app upgrade optimization

**Content & Copy:**
- `copywriting` - Marketing page copy
- `copy-editing` - Copy review and polish
- `email-sequence` - Automated email flows
- `social-content` - Social media content

**SEO & Discovery:**
- `seo-audit` - Technical and on-page SEO
- `programmatic-seo` - Scaled page generation
- `competitor-alternatives` - Comparison pages
- `schema-markup` - Structured data

**Growth & Strategy:**
- `marketing-ideas` - 140+ SaaS marketing ideas
- `marketing-psychology` - Mental models and behavioral science
- `launch-strategy` - Product launch planning
- `pricing-strategy` - Pricing and monetization
- `referral-program` - Referral/affiliate programs
- `free-tool-strategy` - Marketing tools and calculators
- `paid-ads` - Google, Meta, LinkedIn campaigns
- `ab-test-setup` - Experiment design
- `analytics-tracking` - Event tracking setup

## 🔧 Creating Your Own Skills

Skills are simple markdown files with YAML frontmatter:

```markdown
---
name: my-custom-skill
description: A clear description of what this skill does
---

# My Custom Skill

[Instructions that Claude will follow when this skill is active]

## Examples
- Example usage 1
- Example usage 2
```

Place your `SKILL.md` file in `~/.claude/skills/` or your project's `.claude/skills/` directory.

## 🤝 Contributing

Contributions are welcome! If you'd like to:

1. **Report Issues**: Open an issue in the relevant repository
2. **Suggest Improvements**: Fork and submit a PR
3. **Add New Skills**: Follow the skill creation guidelines above

## 📄 License

- **Sell-Like-Crazy-Skill**: MIT License
- **Sabri-Suby-Headline-Skill**: MIT License
- **code-architect**: See repository
- **deep-research-agent**: MIT License
- **openclaw-cloudflare-setup**: MIT License
- **marketingskills**: MIT License (fork of coreyhaines31/marketingskills)
- **ucp**: Apache License 2.0 (fork of Universal-Commerce-Protocol/ucp)

## 🔗 Links

- [Agent Skills Specification](https://agentskills.io)
- [Claude Code Documentation](https://docs.anthropic.com)
- [Skills Marketplace](https://skillsmp.com)

---

*Built with ❤️ by [RGVAI](https://github.com/rgvai)*
