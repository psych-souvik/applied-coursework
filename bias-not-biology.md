# 404: Myth Not Found

An evidence dashboard built to debunk one specific myth: that older employees can't adapt to tech.

Originally built for an HR Analytics class submission, but i'm putting it up here because the approach felt worth showing on its own, not just the conclusion.

## why this exists

most dashboards that try to debunk a workplace myth do it the same way: throw every stat you found at the reader and hope the volume does the convincing. that's not analysis, it's just noise that looks rigorous.

the actual question isn't "is this myth true or false." it's "what would i need to know, in order, to even evaluate whether it's true." so instead of a stat dump, this dashboard is built around five questions, asked in the sequence you'd actually need to ask them. each one either kills the myth or it doesn't. by question five, it doesn't survive any of them.

## the five questions

1. **origin** — where did "boomers can't adapt" actually come from? (a marketing consultant, 2001, never empirically tested. it's bias with a 23-year head start, not biology.)
2. **relevance** — what tech do senior roles actually require? (mostly shallow fluency, not the deep technical skills the myth assumes everyone needs.)
3. **training** — if adoption is lower, is that unwillingness or access? (94% of older workers say they're willing when actually asked. only 12% of orgs design upskilling for 65+. that's a denial-of-access problem, not a motivation problem.)
4. **sectors** — does the generational gap actually show up at work? (healthcare, finance, smartphone ownership, tech spend: parity, wherever access is equal.)
5. **AI era** — what happens when this specific cohort meets AI specifically? (domain experts get a 40% output uplift from AI vs 14% for novices. experience turns out to be the multiplier, not the liability.)

the myth doesn't survive a single one of these in order. that's the whole argument, the dashboard just makes you walk through it instead of telling you the answer upfront.

## stack

plain HTML/CSS/JS, no framework, no build step.

- [Chart.js](https://www.chartjs.org/) for the generational AI-adoption bar chart
- [GSAP](https://gsap.com/) + ScrollTrigger for scroll reveals, hover micro-interactions, and the confirm-debunk celebration animation
- Google Fonts (DM Mono for data labels, Figtree for body text)

Everything's self-contained in one `.html` file, so it runs anywhere, just open it in a browser or host it with GitHub Pages.

## sources

SHRM Foundation 2025, AARP Tech Trends 2025–26, OECD Employment Outlook 2025, WEF Future of Jobs 2025, Microsoft Work Trend Index 2024, HBS/BCG 2023–25, BLS Employee Tenure 2024, Mercer, Brynjolfsson/ADP 2025, Scottsdale Institute 2024, Deloitte State of AI 2026.

---

built by [Souvik Rajbanshi](https://www.linkedin.com/in/souvik-r/) as part of an HR Analytics coursework submission, repurposed here as a sample of approach: behavioural-science framing applied to data visualisation, not just decoration on top of a chart.
