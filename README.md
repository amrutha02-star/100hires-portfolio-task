# 100Hires Portfolio Task

This repo is my portfolio project for the 100Hires Junior Growth Marketing Specialist application. It has two stages: a tool setup task (stage 1) and a research project (stage 2). Both are documented below.

## Stage 1: Setup

The task: install some new tools, set up a GitHub repo, and document the journey.

### Tools I installed

| Tool | Purpose | Source |
|------|---------|--------|
| Cursor IDE | Code editor with built-in AI | cursor.com |
| Claude Code (Cursor extension) | Anthropic's AI assistant inside Cursor | Cursor Marketplace |
| Codex (Cursor extension) | OpenAI's AI assistant inside Cursor | Cursor Marketplace |
| GitHub Desktop | App for managing GitHub without using the terminal | desktop.github.com |
| GitHub account | Hosting this repo (`amrutha02-star`) | github.com |

### Steps I completed

1. Installed Cursor IDE on macOS.
2. Opened the Extensions panel inside Cursor and installed the official Claude Code extension by Anthropic. (I later learnt that Cmd + Shift + X is the keyboard shortcut for opening Extensions.) 
3. Installed the official Codex extension by OpenAI in the same way. 
4. Sent a test message to make sure Claude Code was working.
5. Created a public GitHub repository called `100hires-portfolio-task`.
6. Installed GitHub Desktop and signed in.
7. Cloned the repository to my laptop using GitHub Desktop.
8. Opened the cloned folder in Cursor.
9. Replaced the placeholder README with this document.
10. Committed and pushed the changes back to GitHub.

### Issues I ran into and how I fixed them

**1. Forty-nine results when I searched "Claude Code" in extensions.**
I wasn't sure which one was the real one. I figured out the official extension by checking three things: the publisher name (Anthropic), a blue verified checkmark next to the publisher, and the highest download count (17M). The other 48 are third-party tools by independent developers.

**2. Two "Claude Code" entries appeared in the sidebar.**
After installing, the same name showed up twice. I clicked both. One was Cursor's built-in panel and the other was the extension I installed. Both work. I used the installed extension for sign-in.

**3. Codex error: "Add a project to use Codex".**
Codex wouldn't let me send a message at first. I learned that AI coding tools need a folder or project to work in, since they don't just chat without context. The error went away once I opened my repository as a folder in Cursor.

**4. A popup about installing terminal commands in Cursor.**
A small popup at the bottom of Cursor asked if I wanted to install `code` and `cursor` shell commands. I looked it up. It's a shortcut for launching Cursor from the terminal. Not needed for this task, so I dismissed it.

**5. GitHub Desktop only offered "Open in Visual Studio Code".**
There was no button for Cursor. I opened the folder manually inside Cursor through File then Open Folder, which worked the same way.

### Notes

I had previously used Claude Code (the chat version) to create videos with HyperFrames, so I was already familiar with how conversational AI coding tools work. Cursor, the Cursor extensions, GitHub, and Markdown were all new for this task.

I used Claude (the chat version) throughout the process as a teacher. I asked it what unfamiliar things meant, why errors were happening, and how concepts like commit and push actually work. I drafted this README with its help, then edited it so it sounds like me and reflects what I actually did. Every decision was mine: which extensions to trust, which folder to use, what to include here.

## Stage 2: Research Project

For stage 2 I built a research project on one topic: cold outreach pipeline for B2B SaaS. I picked this because it is a mature space with a lot of real practitioners, and it overlaps with my own work selling a B2B SaaS product, so I can usually tell whether someone's advice is practical or just theory.

The goal was to find genuine practitioners (people who actually run outbound, not just write about it), collect their recent content, and organize it so it could support a real playbook later.

### How the repo is organized

- research/sources.md: the list of experts with links, dates, and short notes
- research/linkedin-posts/: saved posts, one folder per author
- research/youtube-transcripts/: saved transcripts, one folder per author
- research/other/: space for any extra material

### Experts collected so far

Still in progress. I add someone only after I've reviewed their actual content, and only when they cover a part of the pipeline the others don't already cover, so the set doesn't repeat the same advice. That filter matters more to me than hitting a round number, so the count grows slowly. It currently stands at 8, each owning a distinct layer: outbound systems, cold email, deliverability, copywriting, the phone, LinkedIn and social selling, discovery and qualification, and signal-based prospecting. I keep adding only when a genuinely different layer turns up.

1. Mark Colgan: outbound systems, account selection, AI-assisted research
2. Jason Bay: cold email frameworks and outbound execution
3. Nick Abraham: deliverability and sending infrastructure (agency, high-volume angle)
4. Josh Braun: cold email messaging and copywriting, quality-first
5. Kevin Hopp: cold calling and the phone channel, permission-based openers
6. Laura Erdem: LinkedIn and social selling tied to B2B SaaS pipeline
7. Jen Allen-Knuth: discovery and qualification, cost of inaction
8. Anthony Natoli: signal-based prospecting, turning a signal into real context

### How I collected the content

YouTube transcripts: I used an open source tool called youtube-transcript-api to pull transcripts. It fetches the captions YouTube already generates for a video, so it doesn't need an API key. My first attempts went through Codex and failed, because Codex runs in the cloud and YouTube blocks requests from datacenter IP addresses. I fixed this by running the tool locally on my own Mac, which uses a normal home connection, so YouTube treats it like a regular viewer. Each transcript is saved as a clean Markdown file with the source link and the date it was fetched.

LinkedIn posts: LinkedIn blocks automated scraping, so I collected posts manually. I checked the text against the original post before saving, since automated extraction sometimes drops or changes words.

### Decisions I made and what I learned

A few choices shaped the project, and I want to be open about why I made them.

- Recent over famous. Alex asked for recent posts, so when one of Josh Braun's videos turned out to be from late 2023, I swapped it for a 2024 one on the same topic. Someone being well known is not enough if the actual post or video is old.
- I kept the honest bits in. Nick Abraham works from a high-volume agency side, which is different from the careful, low-volume style most of the others teach. Instead of hiding that, I wrote it into his notes. I want the set to show a real range of views, not pretend everyone agrees.
- Coverage over numbers. I add experts one at a time, and only when they cover a part of the pipeline the others don't already cover (strategy, frameworks, deliverability, copywriting, account targeting). Five people who each say something different help more for a real playbook than ten who repeat each other.
- Cleaning up transcripts without changing the words. Some YouTube captions come with no punctuation, so a raw transcript reads as one giant block. I had the tool split those into paragraphs based on the timing of the captions. It only adds breaks to make it readable, it never changes the actual words, so the source stays true to what was said.
- Check the saved text against the real post. When I pulled LinkedIn posts automatically, the tool sometimes dropped or changed a few words. So I read every saved post against the live one before I commit it.
- Picked a topic I can judge. I chose cold outreach for B2B SaaS because I sell a B2B SaaS product myself, so I can usually tell whether someone's advice is practical or just theory. On a topic I knew nothing about, I would not be able to pick the right experts as well.
- Real practitioners, not just people who write about it. Before adding anyone, I checked they actually run outbound. I went through each person's LinkedIn and YouTube feeds, often more than once, to see how often they post, what they post about, and whether it is relevant to this project, and then I picked the one post or video that fit best. That is how Nick Abraham went in as the founder of a cold email agency and Kevin Hopp as someone who has made hundreds of thousands of cold calls himself, instead of me just trusting a name.
- Built one small tool I can reuse. The transcript script saves every file with the source link and the date I pulled it, so anyone can trace it back, and I can use the same tool for the next expert without setting it up again.
- Read the full content before trusting it, and cut what did not hold up. A matching title is not enough, so I read each piece end to end and kept only what delivers real substance and fits the quality-first idea of the set. That meant dropping several picks: Eric Nowoslawski (six million emails a month), a Josh Braun video that only teased its idea, a cold calling pick that was actually about email, Kevin Hopp's 2022 product-demo video (replaced with a recent post), and a Laura Erdem interview that drifted into marketing measurement. For Jen Allen-Knuth I skipped her cold email posts and a strong but 2024 video, and used a recent cost-of-inaction post instead. I would rather leave a slot open than keep something that repeats the set, fights its main idea, or only sounds relevant.

### A note on AI use

Same as stage 1, I used Claude as an assistant to research, fetch transcripts, and draft notes. I reviewed and approved every expert and every piece of content myself, and I verified the LinkedIn post text against the originals.
